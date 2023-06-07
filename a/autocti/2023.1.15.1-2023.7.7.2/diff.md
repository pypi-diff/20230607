# Comparing `tmp/autocti-2023.1.15.1.tar.gz` & `tmp/autocti-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocti-2023.1.15.1.tar", last modified: Sun Jan 15 17:36:28 2023, max compression
+gzip compressed data, was "autocti-2023.7.7.2.tar", last modified: Wed Jun  7 09:59:30 2023, max compression
```

## Comparing `autocti-2023.1.15.1.tar` & `autocti-2023.7.7.2.tar`

### file list

```diff
@@ -1,145 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.552070 autocti-2023.1.15.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-01-15 17:36:28.552070 autocti-2023.1.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.532070 autocti-2023.1.15.1/autocti/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.536070 autocti-2023.1.15.1/autocti/charge_injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/ci_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/hyper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.536070 autocti-2023.1.15.1/autocti/charge_injection/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/imaging/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/imaging/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.536070 autocti-2023.1.15.1/autocti/charge_injection/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/mock/mock_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.536070 autocti-2023.1.15.1/autocti/charge_injection/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/model/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/ou_sim_ci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.540070 autocti-2023.1.15.1/autocti/charge_injection/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/plot/fit_ci_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/charge_injection/plot/imaging_ci_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.540070 autocti-2023.1.15.1/autocti/clocker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/clocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/clocker/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/clocker/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/clocker/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.540070 autocti-2023.1.15.1/autocti/config/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.540070 autocti-2023.1.15.1/autocti/config/priors/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/config/priors/ccd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/config/priors/hyper.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/config/priors/traps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/config/visualize.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.540070 autocti-2023.1.15.1/autocti/cosmics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/cosmics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/cosmics/cosmics.py
--rw-r--r--   0 runner    (1001) docker     (123)    41101 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/cosmics/cr_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/cosmics/cr_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.540070 autocti-2023.1.15.1/autocti/dataset_1d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.544070 autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.544070 autocti-2023.1.15.1/autocti/dataset_1d/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.544070 autocti-2023.1.15.1/autocti/dataset_1d/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/plot/dataset_1d_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/dataset_1d/plot/fit_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.544070 autocti-2023.1.15.1/autocti/extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.544070 autocti-2023.1.15.1/autocti/extract/one_d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/one_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/one_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/one_d/eper.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/one_d/fpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/one_d/master.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/one_d/overscan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/extract/two_d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/extract_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/extract/two_d/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/parallel/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/parallel/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/parallel/eper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/parallel/fpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/parallel/overscan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/extract/two_d/serial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/eper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/fpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/overscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/extract/two_d/serial/prescan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/instruments/acs/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/acs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/acs/acs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/acs/array_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/acs/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/acs/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/acs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/instruments/euclid/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/euclid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/euclid/array_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/euclid/euclid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/euclid/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/instruments/euclid/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/layout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/layout/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/layout/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/mask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/mask/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/mask/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/model/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.548070 autocti-2023.1.15.1/autocti/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.552070 autocti-2023.1.15.1/autocti/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/plot/get_visuals/two_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/preloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.552070 autocti-2023.1.15.1/autocti/util/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/autocti/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:36:28.552070 autocti-2023.1.15.1/autocti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-01-15 17:36:28.000000 autocti-2023.1.15.1/autocti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 17:36:28.552070 autocti-2023.1.15.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-15 17:36:19.000000 autocti-2023.1.15.1/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.411546 autocti-2023.7.7.2/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.889546 autocti-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.934546 autocti-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/.github/workflows/draft-pdf.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2608 2023-06-03 12:16:24.000000 autocti-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1111 2022-12-19 11:17:33.000000 autocti-2023.7.7.2/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18831 2022-12-19 11:17:33.000000 autocti-2023.7.7.2/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2470 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2022-11-28 11:07:42.000000 autocti-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9800 2023-06-07 09:59:30.410546 autocti-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8950 2023-06-03 09:39:55.000000 autocti-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.942547 autocti-2023.7.7.2/autocti/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3412 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/autocti/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.955546 autocti-2023.7.7.2/autocti/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      281 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/autocti/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7455 2023-05-25 17:24:17.000000 autocti-2023.7.7.2/autocti/aggregator/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/autocti/aggregator/cti.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2276 2023-05-25 17:24:17.000000 autocti-2023.7.7.2/autocti/aggregator/dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3925 2023-06-03 10:36:19.000000 autocti-2023.7.7.2/autocti/aggregator/fit_dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3578 2023-06-03 09:42:32.000000 autocti-2023.7.7.2/autocti/aggregator/fit_imaging_ci.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2277 2023-05-25 17:24:17.000000 autocti-2023.7.7.2/autocti/aggregator/imaging_ci.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.968546 autocti-2023.7.7.2/autocti/charge_injection/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/charge_injection/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2899 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/ci_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4971 2023-06-03 09:58:57.000000 autocti-2023.7.7.2/autocti/charge_injection/fit.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/hyper.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.976546 autocti-2023.7.7.2/autocti/charge_injection/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/charge_injection/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8478 2023-06-03 10:26:41.000000 autocti-2023.7.7.2/autocti/charge_injection/imaging/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1833 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/imaging/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10080 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/imaging/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17201 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/layout.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1174 2023-01-13 16:58:40.000000 autocti-2023.7.7.2/autocti/charge_injection/master.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.980546 autocti-2023.7.7.2/autocti/charge_injection/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/charge_injection/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3790 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/mock/mock_result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.989545 autocti-2023.7.7.2/autocti/charge_injection/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/charge_injection/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13653 2023-06-03 10:26:41.000000 autocti-2023.7.7.2/autocti/charge_injection/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2023-06-03 10:26:26.000000 autocti-2023.7.7.2/autocti/charge_injection/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12970 2023-06-03 09:42:58.000000 autocti-2023.7.7.2/autocti/charge_injection/model/visualizer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9610 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/charge_injection/ou_sim_ci.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:29.996546 autocti-2023.7.7.2/autocti/charge_injection/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/charge_injection/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20366 2023-06-03 09:58:40.000000 autocti-2023.7.7.2/autocti/charge_injection/plot/fit_ci_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14182 2023-06-03 09:50:54.000000 autocti-2023.7.7.2/autocti/charge_injection/plot/imaging_ci_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.004546 autocti-2023.7.7.2/autocti/clocker/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/clocker/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2667 2022-12-20 20:16:56.000000 autocti-2023.7.7.2/autocti/clocker/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7166 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/clocker/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30176 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/clocker/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.010545 autocti-2023.7.7.2/autocti/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      367 2023-01-15 20:17:47.000000 autocti-2023.7.7.2/autocti/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      688 2022-12-02 15:59:51.000000 autocti-2023.7.7.2/autocti/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.017546 autocti-2023.7.7.2/autocti/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      648 2023-02-27 14:53:06.000000 autocti-2023.7.7.2/autocti/config/priors/ccd.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-12-02 15:59:51.000000 autocti-2023.7.7.2/autocti/config/priors/hyper.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2022-12-05 10:42:13.000000 autocti-2023.7.7.2/autocti/config/priors/traps.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      369 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/config/visualize.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.025546 autocti-2023.7.7.2/autocti/cosmics/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/cosmics/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11375 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/cosmics/cosmics.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41101 2022-12-17 13:44:39.000000 autocti-2023.7.7.2/autocti/cosmics/cr_distances.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13590 2022-12-17 13:44:38.000000 autocti-2023.7.7.2/autocti/cosmics/cr_lengths.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.029546 autocti-2023.7.7.2/autocti/dataset_1d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/dataset_1d/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.039546 autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6766 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       92 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5606 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      970 2022-12-13 16:21:22.000000 autocti-2023.7.7.2/autocti/dataset_1d/fit.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.047547 autocti-2023.7.7.2/autocti/dataset_1d/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/dataset_1d/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9268 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/autocti/dataset_1d/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      101 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/dataset_1d/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12051 2023-06-03 10:17:27.000000 autocti-2023.7.7.2/autocti/dataset_1d/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.054546 autocti-2023.7.7.2/autocti/dataset_1d/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/dataset_1d/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9670 2023-06-03 09:50:54.000000 autocti-2023.7.7.2/autocti/dataset_1d/plot/dataset_1d_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13682 2023-06-03 10:16:35.000000 autocti-2023.7.7.2/autocti/dataset_1d/plot/fit_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      560 2023-02-14 15:40:54.000000 autocti-2023.7.7.2/autocti/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.058546 autocti-2023.7.7.2/autocti/extract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/extract/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.072547 autocti-2023.7.7.2/autocti/extract/one_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/extract/one_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7551 2023-05-16 14:13:25.000000 autocti-2023.7.7.2/autocti/extract/one_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/one_d/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1059 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/one_d/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10366 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/one_d/master.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1227 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/one_d/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2146 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.081545 autocti-2023.7.7.2/autocti/extract/two_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/extract/two_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16148 2023-05-16 14:13:12.000000 autocti-2023.7.7.2/autocti/extract/two_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/extract_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19949 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/two_d/master.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.099547 autocti-2023.7.7.2/autocti/extract/two_d/parallel/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13507 2023-05-25 17:24:09.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11608 2023-06-03 10:32:33.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/calibration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7164 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4280 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4619 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5472 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/parallel/pedestal.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.120547 autocti-2023.7.7.2/autocti/extract/two_d/serial/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5951 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10782 2023-06-03 10:32:33.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/calibration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6160 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3793 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4595 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3790 2023-05-15 17:37:57.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/overscan_no_eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3110 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/autocti/extract/two_d/serial/prescan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5622 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.123546 autocti-2023.7.7.2/autocti/instruments/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      122 2022-10-21 09:42:48.000000 autocti-2023.7.7.2/autocti/instruments/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.137546 autocti-2023.7.7.2/autocti/instruments/acs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      151 2022-10-24 13:23:41.000000 autocti-2023.7.7.2/autocti/instruments/acs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6053 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/acs/acs_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11226 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/acs/array_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3037 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/acs/header.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4794 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/acs/image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1061 2022-10-21 13:55:34.000000 autocti-2023.7.7.2/autocti/instruments/acs/layout.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.150545 autocti-2023.7.7.2/autocti/instruments/euclid/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      107 2022-10-21 13:47:30.000000 autocti-2023.7.7.2/autocti/instruments/euclid/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12883 2023-01-13 16:58:40.000000 autocti-2023.7.7.2/autocti/instruments/euclid/array_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      711 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/euclid/euclid_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      851 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/euclid/header.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17129 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/instruments/euclid/layout.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.156546 autocti-2023.7.7.2/autocti/layout/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/autocti/layout/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2819 2023-05-30 13:00:37.000000 autocti-2023.7.7.2/autocti/layout/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11677 2023-05-25 17:24:17.000000 autocti-2023.7.7.2/autocti/layout/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.163546 autocti-2023.7.7.2/autocti/mask/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/autocti/mask/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2447 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/mask/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11085 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/mask/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      193 2023-02-08 17:48:18.000000 autocti-2023.7.7.2/autocti/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.174546 autocti-2023.7.7.2/autocti/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/autocti/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3711 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/model/model_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/autocti/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1632 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/model/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1106 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/autocti/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.178546 autocti-2023.7.7.2/autocti/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2811 2023-06-03 09:48:03.000000 autocti-2023.7.7.2/autocti/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2752 2023-06-03 10:38:40.000000 autocti-2023.7.7.2/autocti/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.185546 autocti-2023.7.7.2/autocti/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 16:14:32.000000 autocti-2023.7.7.2/autocti/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1215 2022-11-11 16:14:32.000000 autocti-2023.7.7.2/autocti/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3107 2023-06-03 09:58:40.000000 autocti-2023.7.7.2/autocti/plot/get_visuals/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2885 2022-12-18 14:37:25.000000 autocti-2023.7.7.2/autocti/preloads.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.187546 autocti-2023.7.7.2/autocti/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/autocti/util/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.409546 autocti-2023.7.7.2/autocti.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7804 2023-06-07 09:59:29.000000 autocti-2023.7.7.2/autocti.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.192546 autocti-2023.7.7.2/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.194546 autocti-2023.7.7.2/docs/_static/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/_static/.gitignore
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.198546 autocti-2023.7.7.2/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autocti-2023.7.7.2/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autocti-2023.7.7.2/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.201546 autocti-2023.7.7.2/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6858 2022-11-25 11:55:02.000000 autocti-2023.7.7.2/docs/advanced/database.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.212546 autocti-2023.7.7.2/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2022-12-20 20:00:42.000000 autocti-2023.7.7.2/docs/api/arctic.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      545 2022-12-20 20:00:42.000000 autocti-2023.7.7.2/docs/api/clocking.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1208 2023-01-13 16:58:40.000000 autocti-2023.7.7.2/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      303 2022-12-20 20:00:42.000000 autocti-2023.7.7.2/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1480 2022-12-20 20:00:42.000000 autocti-2023.7.7.2/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2944 2022-12-20 20:00:42.000000 autocti-2023.7.7.2/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4623 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.221546 autocti-2023.7.7.2/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1111 2022-12-19 11:17:33.000000 autocti-2023.7.7.2/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1015 2022-11-27 17:21:24.000000 autocti-2023.7.7.2/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-27 17:21:24.000000 autocti-2023.7.7.2/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2256 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/general/workspace.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5281 2022-12-20 20:00:42.000000 autocti-2023.7.7.2/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.236546 autocti-2023.7.7.2/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1381 2022-12-06 16:43:06.000000 autocti-2023.7.7.2/docs/installation/arctic.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3203 2022-12-06 16:40:25.000000 autocti-2023.7.7.2/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3360 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2450 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2784 2022-12-06 16:40:25.000000 autocti-2023.7.7.2/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4642 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5204 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.248546 autocti-2023.7.7.2/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.263546 autocti-2023.7.7.2/docs/overview/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   397515 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/ccd.gif
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   281375 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/ccd_schematic.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   514636 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/cti.gif
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132888 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/cti_time_evolution.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.272546 autocti-2023.7.7.2/docs/overview/images/overview_1/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21797 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_1/array_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23382 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_1/array_1d_cti_corrected.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22695 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_1/array_1d_with_cti.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.286546 autocti-2023.7.7.2/docs/overview/images/overview_2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22121 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_2/array_2d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23664 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_2/array_2d_cti_corrected.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22519 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_2/array_2d_parallel_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24358 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_2/array_2d_parallel_serial_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22449 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_2/array_2d_serial_cti.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.302546 autocti-2023.7.7.2/docs/overview/images/overview_3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24750 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_3/density_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24719 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_3/density_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26412 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_3/timescale_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25030 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_3/timescale_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26471 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_3/volume_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26695 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_3/volume_2.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.328546 autocti-2023.7.7.2/docs/overview/images/overview_4/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34116 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/binned_parallel_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25079 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/binned_parallel_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32451 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/binned_serial_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31453 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/binned_serial_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    79377 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/imaging_ci.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47970 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/imaging_ci_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44395 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/imaging_ci_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   351059 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/imaging_ci_non_uniform_cosmic_rays.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32372 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_4/pre_cti_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.368546 autocti-2023.7.7.2/docs/overview/images/overview_5/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28538 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36932 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/chi_squared_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29730 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/chi_squared_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31056 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/chi_squared_map_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35482 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/ci_image_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51137 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/dataset_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31199 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45032 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/normalized_residual_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31927 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/normalized_residual_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33155 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/normalized_residual_map_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31172 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47426 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/residual_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30360 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/residual_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34986 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_5/residual_map_masked.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.391546 autocti-2023.7.7.2/docs/overview/images/overview_6/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107188 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_1d_100.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   120106 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_1d_200000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   102590 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_1d_25000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   105434 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_1d_5000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80847 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_2d_100.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    86775 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_2d_200000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80846 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_2d_25000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    76721 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/overview_6/fit_2d_5000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   542080 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/docs/overview/images/what_is_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12544 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/overview/overview_1_what_is_cti.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10805 2023-05-15 17:43:12.000000 autocti-2023.7.7.2/docs/overview/overview_2_parallel_and_serial.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10013 2023-01-13 16:58:40.000000 autocti-2023.7.7.2/docs/overview/overview_3_cti_features.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11491 2023-06-03 09:42:32.000000 autocti-2023.7.7.2/docs/overview/overview_4_charge_injection_data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14975 2023-06-03 10:29:07.000000 autocti-2023.7.7.2/docs/overview/overview_5_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14938 2023-06-03 10:36:19.000000 autocti-2023.7.7.2/docs/overview/overview_6_cti_calibration.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      163 2022-11-26 18:13:45.000000 autocti-2023.7.7.2/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       30 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.397546 autocti-2023.7.7.2/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14795 2022-11-27 17:05:27.000000 autocti-2023.7.7.2/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1436 2022-11-27 17:05:27.000000 autocti-2023.7.7.2/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2049 2022-11-27 17:10:36.000000 autocti-2023.7.7.2/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       13 2023-06-03 12:21:40.000000 autocti-2023.7.7.2/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:30.407546 autocti-2023.7.7.2/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   881609 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/paper/cti_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    98062 2023-05-15 17:37:58.000000 autocti-2023.7.7.2/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9817 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      917 2022-11-23 10:12:20.000000 autocti-2023.7.7.2/profiling
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       13 2023-03-21 12:51:53.000000 autocti-2023.7.7.2/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:59:30.411546 autocti-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1705 2023-06-07 09:57:48.000000 autocti-2023.7.7.2/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1875 2022-10-20 11:42:04.000000 autocti-2023.7.7.2/to_do_list
```

### Comparing `autocti-2023.1.15.1/CITATIONS.rst` & `autocti-2023.7.7.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/LICENSE` & `autocti-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/PKG-INFO` & `autocti-2023.7.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocti
-Version: 2023.1.15.1
+Version: 2023.7.7.2
 Summary: PyAutoCTI: Charge Transfer Inefficiency Modeling
 Home-page: https://github.com/jammy2211/PyAutoCTI
 Author: James Nightingale, Richard Massey, Jacob Kegerreis and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -176,16 +176,16 @@
         shape_2d=shape_native,
         region_list=regions_list,
     )
 
     """
     Load the charge injection image from fits.
     """
-    imaging_ci = ac.ImagingCI.from_fits(
-        image_path=path.join(dataset_path, f"data.fits"),
+    dataset = ac.ImagingCI.from_fits(
+        data_path=path.join(dataset_path, f"data.fits"),
         noise_map_path=path.join(dataset_path, f"noise_map.fits"),
         pre_cti_data_path=path.join(dataset_path, f"pre_cti_data.fits"),
         layout=layout,
         pixel_scales=0.1,
     )
 
     """
@@ -216,15 +216,15 @@
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
 
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the cti model to the data.
     """
-    analysis = ac.AnalysisImagingCI(dataset=imaging_ci, clocker=clocker_2d)
+    analysis = ac.AnalysisImagingCI(dataset=dataset, clocker=clocker_2d)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autocti-2023.1.15.1/README.rst` & `autocti-2023.7.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,16 @@
         shape_2d=shape_native,
         region_list=regions_list,
     )
 
     """
     Load the charge injection image from fits.
     """
-    imaging_ci = ac.ImagingCI.from_fits(
-        image_path=path.join(dataset_path, f"data.fits"),
+    dataset = ac.ImagingCI.from_fits(
+        data_path=path.join(dataset_path, f"data.fits"),
         noise_map_path=path.join(dataset_path, f"noise_map.fits"),
         pre_cti_data_path=path.join(dataset_path, f"pre_cti_data.fits"),
         layout=layout,
         pixel_scales=0.1,
     )
 
     """
@@ -194,15 +194,15 @@
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
 
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the cti model to the data.
     """
-    analysis = ac.AnalysisImagingCI(dataset=imaging_ci, clocker=clocker_2d)
+    analysis = ac.AnalysisImagingCI(dataset=dataset, clocker=clocker_2d)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autocti-2023.1.15.1/autocti/__init__.py` & `autocti-2023.7.7.2/autocti/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,22 @@
 from .charge_injection.hyper import HyperCINoiseScalar
 from .charge_injection.hyper import HyperCINoiseCollection
 from .charge_injection.imaging.imaging import ImagingCI
 from .charge_injection.imaging.settings import SettingsImagingCI
 from .charge_injection.imaging.simulator import SimulatorImagingCI
 from .charge_injection.layout import Layout2DCI
 from .cosmics.cosmics import SimulatorCosmicRayMap
+from .extract.settings import SettingsExtract
 from .extract.two_d.parallel.overscan import Extract2DParallelOverscan
 from .extract.two_d.parallel.fpr import Extract2DParallelFPR
 from .extract.two_d.parallel.eper import Extract2DParallelEPER
+from .extract.two_d.parallel.pedestal import Extract2DParallelPedestal
 from .extract.two_d.serial.prescan import Extract2DSerialPrescan
 from .extract.two_d.serial.overscan import Extract2DSerialOverscan
+from .extract.two_d.serial.overscan_no_eper import Extract2DSerialOverscanNoEPER
 from .extract.two_d.serial.fpr import Extract2DSerialFPR
 from .extract.two_d.serial.eper import Extract2DSerialEPER
 from .extract.two_d.parallel.calibration import Extract2DParallelCalibration
 from .extract.two_d.serial.calibration import Extract2DSerialCalibration
 from .extract.two_d.master import Extract2DMaster
 from .instruments import euclid
 from .instruments import acs
@@ -47,22 +50,26 @@
 from .extract.one_d.master import Extract1DMaster
 from .layout.one_d import Layout1D
 from .dataset_1d.dataset_1d.settings import SettingsDataset1D
 from .dataset_1d.dataset_1d.dataset_1d import Dataset1D
 from .dataset_1d.dataset_1d.simulator import SimulatorDataset1D
 from .dataset_1d.fit import FitDataset1D
 from .dataset_1d.model.analysis import AnalysisDataset1D
+from .dataset_1d.model.result import ResultDataset1D
 from .charge_injection.model.analysis import AnalysisImagingCI
+from .charge_injection.model.result import ResultImagingCI
 from .model.model_util import CTI1D
 from .model.model_util import CTI2D
 from .model.settings import SettingsCTI1D
 from .model.settings import SettingsCTI2D
 from .clocker.one_d import Clocker1D
 from .clocker.two_d import Clocker2D
+from . import aggregator as agg
 from . import util
 from . import plot
+from . import mock as m  # noqa
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.1.15.1"
+__version__ = "2022.7.11.1"
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/ci_util.py` & `autocti-2023.7.7.2/autocti/charge_injection/ci_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     Generate a non-uniform charge injection region from an input list of normalization values across columns.
     """
 
     ci_rows = region_dimensions[0]
     ci_region = np.zeros(region_dimensions)
 
     for column_index, injection_norm in enumerate(injection_norm_list):
-
         ci_region[0:ci_rows, column_index] = generate_column(
             size=ci_rows, norm=injection_norm, row_slope=row_slope
         )
 
     return ci_region
 
 
@@ -51,48 +50,42 @@
     injection_total: int,
     parallel_size: int,
     serial_size: int,
     serial_prescan_size: int,
     serial_overscan_size: int,
     roe_corner: Tuple[int, int],
 ):
-
     region_list_ci = []
 
     for index in range(injection_total):
-
         if roe_corner == (0, 0):
-
             ci_region = (
                 parallel_size - (injection_start + injection_on),
                 parallel_size - injection_start,
                 serial_prescan_size,
                 serial_size - serial_overscan_size,
             )
 
         elif roe_corner == (1, 0):
-
             ci_region = (
                 injection_start,
                 injection_start + injection_on,
                 serial_prescan_size,
                 serial_size - serial_overscan_size,
             )
 
         elif roe_corner == (0, 1):
-
             ci_region = (
                 parallel_size - (injection_start + injection_on),
                 parallel_size - injection_start,
                 serial_overscan_size,
                 serial_size - serial_prescan_size,
             )
 
         elif roe_corner == (1, 1):
-
             ci_region = (
                 injection_start,
                 injection_start + injection_on,
                 serial_overscan_size,
                 serial_size - serial_prescan_size,
             )
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/fit.py` & `autocti-2023.7.7.2/autocti/charge_injection/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,32 +39,30 @@
 
     @property
     def imaging_ci(self) -> ImagingCI:
         return self.dataset
 
     @property
     def noise_map(self) -> aa.Array2D:
-
         if self.hyper_noise_scalar_dict is not None:
-
             return hyper_noise_map_from(
                 hyper_noise_scalar_dict=self.hyper_noise_scalar_dict,
                 noise_scaling_map_dict=self.noise_scaling_map_dict,
                 noise_map=self.dataset.noise_map,
             )
 
         return self.dataset.noise_map
 
     @property
     def model_data(self) -> aa.Array2D:
         return self.post_cti_data
 
     @property
     def layout(self):
-        return self.imaging_ci.layout
+        return self.dataset.layout
 
     @property
     def pre_cti_data(self):
         return self.dataset.pre_cti_data
 
     @property
     def chi_squared(self) -> float:
@@ -82,27 +80,27 @@
         and offering faster tune times.
         """
 
         return aa.util.fit.chi_squared_with_mask_fast_from(
             data=self.dataset.data,
             noise_map=self.noise_map,
             mask=self.mask,
-            model_data=self.model_data
+            model_data=self.model_data,
         )
 
     @property
     def noise_normalization(self) -> float:
         """
         Returns the noise-map normalization term of the noise-map, summing the noise_map value in every pixel as:
 
         [Noise_Term] = sum(log(2*pi*[Noise]**2.0))
         """
 
-     #   if self.preloads.noise_normalization is not None:
-     #       return self.preloads.noise_normalization
+        if self.preloads.noise_normalization is not None:
+            return self.preloads.noise_normalization
 
         return aa.util.fit.noise_normalization_with_mask_from(
             noise_map=self.noise_map, mask=self.mask
         )
 
     @property
     def chi_squared_map_of_regions_ci(self):
@@ -137,13 +135,12 @@
         An arrays describing the RMS standard deviation error in each pixel, preferably in units of electrons per
         second.
     """
 
     noise_map = copy.copy(noise_map)
 
     for key, hyper_noise_scalar in hyper_noise_scalar_dict.items():
-
         noise_map += hyper_noise_scalar.scaled_noise_map_from(
             noise_scaling=noise_scaling_map_dict[key]
         )
 
     return noise_map
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/hyper.py` & `autocti-2023.7.7.2/autocti/charge_injection/hyper.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,21 @@
     def __init__(
         self,
         regions_ci: Optional[HyperCINoiseScalar] = None,
         parallel_eper: Optional[HyperCINoiseScalar] = None,
         serial_eper: Optional[HyperCINoiseScalar] = None,
         serial_overscan_no_eper: Optional[HyperCINoiseScalar] = None,
     ):
-
         self.regions_ci = regions_ci
         self.parallel_eper = parallel_eper
         self.serial_eper = serial_eper
         self.serial_overscan_no_eper = serial_overscan_no_eper
 
     @property
     def as_dict(self):
-
         hyper_dict = {
             "regions_ci": self.regions_ci,
             "parallel_eper": self.parallel_eper,
             "serial_eper": self.serial_eper,
             "serial_overscan_no_eper": self.serial_overscan_no_eper,
         }
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/imaging/imaging.py` & `autocti-2023.7.7.2/autocti/charge_injection/imaging/imaging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 import numpy as np
+from typing import Optional, List, Dict
 
 import autoarray as aa
 
 from autocti.charge_injection.imaging.settings import SettingsImagingCI
 from autocti.charge_injection.layout import Layout2DCI
+from autocti.extract.settings import SettingsExtract
 from autocti.mask import mask_2d
 from autocti import exc
 
-from typing import Dict, Optional, List
-
 
 class ImagingCI(aa.Imaging):
     def __init__(
         self,
-        image: aa.Array2D,
+        data: aa.Array2D,
         noise_map: aa.Array2D,
         pre_cti_data: aa.Array2D,
         layout: Layout2DCI,
         cosmic_ray_map: Optional[aa.Array2D] = None,
         noise_scaling_map_dict: Optional[Dict] = None,
+        fpr_value: Optional[float] = None,
+        settings_dict: Optional[Dict] = None,
     ):
-
-        super().__init__(image=image, noise_map=noise_map)
+        super().__init__(data=data, noise_map=noise_map)
 
         self.data = self.image.native
         self.noise_map = self.noise_map.native
         self.pre_cti_data = pre_cti_data.native
 
         if cosmic_ray_map is not None:
             cosmic_ray_map = cosmic_ray_map.native
 
         self.cosmic_ray_map = cosmic_ray_map
 
         if noise_scaling_map_dict is not None:
-
             noise_scaling_map_dict = {
                 key: noise_scaling_map.native
                 for key, noise_scaling_map in noise_scaling_map_dict.items()
             }
 
         self.noise_scaling_map_dict = noise_scaling_map_dict
 
         self.layout = layout
 
-        self.imaging_full = self
+        if fpr_value is None:
+            fpr_value = np.round(
+                np.mean(
+                    self.layout.extract.parallel_fpr.median_list_from(
+                        array=self.data,
+                        settings=SettingsExtract(
+                            pixels_from_end=min(
+                                10, self.layout.smallest_parallel_rows_within_ci_regions
+                            )
+                        ),
+                    )
+                ),
+                2,
+            )
+
+        self.fpr_value = fpr_value
+        self.settings_dict = settings_dict
 
     @property
     def mask(self):
         return self.image.mask
 
     @property
     def region_list(self):
@@ -73,123 +89,111 @@
         return [
             np.ma.median(masked_image[region.y0 : region.y1, column_index])
             for region in self.region_list
             for column_index in range(region.x0, region.x1)
         ]
 
     def apply_mask(self, mask: mask_2d.Mask2D) -> "ImagingCI":
-
         image = aa.Array2D(values=self.image.native, mask=mask)
-
         noise_map = aa.Array2D(values=self.noise_map.native, mask=mask)
 
         if self.cosmic_ray_map is not None:
-
-            cosmic_ray_map = aa.Array2D(
-            values=self.cosmic_ray_map.native, mask=mask
-            )
+            cosmic_ray_map = aa.Array2D(values=self.cosmic_ray_map.native, mask=mask)
 
         else:
-
             cosmic_ray_map = None
 
         if self.noise_scaling_map_dict is not None:
-
             noise_scaling_map_dict = {
                 key: aa.Array2D(values=noise_scaling_map.native, mask=mask)
                 for key, noise_scaling_map in self.noise_scaling_map_dict.items()
             }
 
         else:
             noise_scaling_map_dict = None
 
         return ImagingCI(
-            image=image,
+            data=image,
             noise_map=noise_map,
             pre_cti_data=self.pre_cti_data.native,
             layout=self.layout,
             cosmic_ray_map=cosmic_ray_map,
             noise_scaling_map_dict=noise_scaling_map_dict,
+            fpr_value=self.fpr_value,
+            settings_dict=self.settings_dict,
         )
 
     def apply_settings(self, settings: SettingsImagingCI):
-
         if settings.parallel_pixels is not None:
-
-            imaging = self.layout.extract.parallel_calibration.imaging_ci_from(
-                imaging_ci=self, columns=settings.parallel_pixels
+            dataset = self.layout.extract.parallel_calibration.imaging_ci_from(
+                dataset=self, columns=settings.parallel_pixels
             )
 
             mask = self.layout.extract.parallel_calibration.mask_2d_from(
                 mask=self.mask, columns=settings.parallel_pixels
             )
 
         elif settings.serial_pixels is not None:
-
-            imaging = self.layout.extract.serial_calibration.imaging_ci_from(
-                imaging_ci=self, rows=settings.serial_pixels
+            dataset = self.layout.extract.serial_calibration.imaging_ci_from(
+                dataset=self, rows=settings.serial_pixels
             )
 
             mask = self.layout.extract.serial_calibration.mask_2d_from(
                 mask=self.mask, rows=settings.serial_pixels
             )
 
         else:
-
             return self
 
-        imaging = imaging.apply_mask(mask=mask)
-
-        imaging.imaging_full = self.imaging_full
+        dataset = dataset.apply_mask(mask=mask)
 
-        return imaging
+        return dataset
 
     def set_noise_scaling_map_dict(self, noise_scaling_map_dict: Dict):
-
         self.noise_scaling_map_dict = {
             key: noise_scaling_map.native
             for key, noise_scaling_map in noise_scaling_map_dict.items()
         }
 
     @classmethod
     def from_fits(
         cls,
         layout,
         pixel_scales,
-        image_path=None,
+        data_path=None,
         image=None,
-        image_hdu=0,
+        data_hdu=0,
         noise_map_path=None,
         noise_map_hdu=0,
         noise_map_from_single_value=None,
         pre_cti_data_path=None,
         pre_cti_data_hdu=0,
         pre_cti_data=None,
         cosmic_ray_map_path=None,
         cosmic_ray_map_hdu=0,
-    ):
-
-        if image_path is not None and image is None:
-
+        settings_dict: Optional[Dict] = None,
+    ) -> "ImagingCI":
+        if data_path is not None and image is None:
             ci_image = aa.Array2D.from_fits(
-                file_path=image_path, hdu=image_hdu, pixel_scales=pixel_scales
+                file_path=data_path, hdu=data_hdu, pixel_scales=pixel_scales
             )
 
         elif image is not None:
-
             ci_image = image
 
         if noise_map_path is not None:
             ci_noise_map = aa.util.array_2d.numpy_array_2d_via_fits_from(
                 file_path=noise_map_path, hdu=noise_map_hdu
             )
         else:
             ci_noise_map = np.ones(ci_image.shape_native) * noise_map_from_single_value
 
-        ci_noise_map = aa.Array2D.no_mask(values=ci_noise_map, pixel_scales=pixel_scales)
+        ci_noise_map = aa.Array2D.no_mask(
+            values=ci_noise_map, pixel_scales=pixel_scales
+        )
 
         if pre_cti_data_path is not None and pre_cti_data is None:
             pre_cti_data = aa.Array2D.from_fits(
                 file_path=pre_cti_data_path,
                 hdu=pre_cti_data_hdu,
                 pixel_scales=pixel_scales,
             )
@@ -199,49 +203,47 @@
             )
 
         pre_cti_data = aa.Array2D.no_mask(
             values=pre_cti_data.native, pixel_scales=pixel_scales
         )
 
         if cosmic_ray_map_path is not None:
-
             cosmic_ray_map = aa.Array2D.from_fits(
                 file_path=cosmic_ray_map_path,
                 hdu=cosmic_ray_map_hdu,
                 pixel_scales=pixel_scales,
             )
 
         else:
             cosmic_ray_map = None
 
         return ImagingCI(
-            image=ci_image,
+            data=ci_image,
             noise_map=ci_noise_map,
             pre_cti_data=pre_cti_data,
             cosmic_ray_map=cosmic_ray_map,
             layout=layout,
+            settings_dict=settings_dict,
         )
 
     def output_to_fits(
         self,
-        image_path,
+        data_path,
         noise_map_path=None,
         pre_cti_data_path=None,
         cosmic_ray_map_path=None,
         overwrite=False,
     ):
-
-        self.image.output_to_fits(file_path=image_path, overwrite=overwrite)
+        self.image.output_to_fits(file_path=data_path, overwrite=overwrite)
 
         if noise_map_path is not None:
             self.noise_map.output_to_fits(file_path=noise_map_path, overwrite=overwrite)
 
         if pre_cti_data_path is not None:
             self.pre_cti_data.output_to_fits(
                 file_path=pre_cti_data_path, overwrite=overwrite
             )
 
         if self.cosmic_ray_map is not None and cosmic_ray_map_path is not None:
-
             self.cosmic_ray_map.output_to_fits(
                 file_path=cosmic_ray_map_path, overwrite=overwrite
             )
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/imaging/settings.py` & `autocti-2023.7.7.2/autocti/charge_injection/imaging/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class SettingsImagingCI(aa.SettingsImaging):
     def __init__(
         self,
         parallel_pixels: Tuple[int, int] = None,
         serial_pixels: Tuple[int, int] = None,
     ):
-
         super().__init__()
 
         self.parallel_pixels = parallel_pixels
         self.serial_pixels = serial_pixels
 
     def modify_via_fit_type(self, is_parallel_fit, is_serial_fit):
         """
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/imaging/simulator.py` & `autocti-2023.7.7.2/autocti/charge_injection/imaging/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+import copy
 import numpy as np
-from typing import List, Tuple
+from typing import List
 
 import autoarray as aa
 
 from autoarray.dataset.imaging.simulator import SimulatorImaging
 
 from autocti.charge_injection.imaging.imaging import ImagingCI
 from autocti.charge_injection.layout import Layout2DCI
 from autocti.clocker.two_d import Clocker2D
+from autocti.extract.settings import SettingsExtract
 from autocti.model.model_util import CTI2D
 
-from autocti.charge_injection import ci_util
-
 from typing import Optional
 
 
 class SimulatorImagingCI(SimulatorImaging):
     def __init__(
         self,
         pixel_scales: aa.type.PixelScales,
         norm: float,
         max_norm: float = np.inf,
         column_sigma: Optional[float] = None,
         row_slope: Optional[float] = 0.0,
         non_uniform_norm_limit=None,
         read_noise: Optional[float] = None,
+        charge_noise: Optional[float] = None,
         noise_if_add_noise_false: float = 0.1,
         noise_seed: int = -1,
         ci_seed: int = -1,
     ):
         """A class representing a Imaging observation, using the shape of the image, the pixel scale,
         psf, exposure time, etc.
 
@@ -48,52 +49,47 @@
         self.pixel_scales = pixel_scales
 
         self.norm = norm
         self.max_norm = max_norm
         self.column_sigma = column_sigma
         self.row_slope = row_slope
         self.non_uniform_norm_limit = non_uniform_norm_limit
+        self.charge_noise = charge_noise
 
         self.ci_seed = ci_seed
 
     @property
     def _ci_seed(self) -> int:
-
         if self.ci_seed == -1:
             return np.random.randint(0, int(1e9))
         return self.ci_seed
 
     def median_list_from(self, total_columns: int) -> List[float]:
-
         np.random.seed(self._ci_seed)
 
         injection_norm_list = []
 
         for column_number in range(total_columns):
-
             injection_norm = 0
 
             while injection_norm <= 0 or injection_norm >= self.max_norm:
-
                 injection_norm = np.random.normal(self.norm, self.column_sigma)
 
             injection_norm_list.append(injection_norm)
 
         return injection_norm_list
 
     def injection_norm_list_with_limit_from(self, total_columns: int) -> List[float]:
-
         injection_norm_list = self.median_list_from(
             total_columns=self.non_uniform_norm_limit
         )
 
         injection_norm_limited_list = []
 
         for i in range(total_columns):
-
             injection_norm = np.random.choice(injection_norm_list)
 
             injection_norm_limited_list.append(injection_norm)
 
         return injection_norm_limited_list
 
     def pre_cti_data_uniform_from(self, layout: Layout2DCI) -> aa.Array2D:
@@ -132,15 +128,14 @@
             The power-law slope of non-uniformity in the row charge injection profile.
         ci_seed
             Input ci_seed for the random number generator to give reproducible results. A new ci_seed is always used for each \
             pre_cti_datas, ensuring each non-uniform ci_region has the same column non-uniformity layout_ci.
         """
 
         for region in layout.region_list:
-
             if self.non_uniform_norm_limit is None:
                 injection_norm_list = self.median_list_from(
                     total_columns=region.total_columns
                 )
             else:
                 injection_norm_list = self.injection_norm_list_with_limit_from(
                     total_columns=region.total_columns
@@ -154,15 +149,14 @@
 
     def via_layout_from(
         self,
         layout: Layout2DCI,
         clocker: Optional[Clocker2D],
         cti: Optional[CTI2D],
         cosmic_ray_map: Optional[aa.Array2D] = None,
-        name: Optional[str] = None,
     ) -> ImagingCI:
         """Simulate a charge injection image, including effects like noises.
 
         Parameters
         ----------
         pre_cti_data
         cosmic_ray_map
@@ -198,26 +192,34 @@
     def via_pre_cti_data_from(
         self,
         pre_cti_data: aa.Array2D,
         layout: Layout2DCI,
         clocker: Optional[Clocker2D],
         cti: Optional[CTI2D],
         cosmic_ray_map: Optional[aa.Array2D] = None,
-        name: Optional[str] = None,
     ) -> ImagingCI:
-
         pre_cti_data = pre_cti_data.native
 
         if cosmic_ray_map is not None:
             pre_cti_data += cosmic_ray_map.native
 
+        if self.charge_noise is not None:
+            pre_cti_data = layout.extract.parallel_fpr.add_gaussian_noise_to(
+                array=pre_cti_data,
+                noise_sigma=self.charge_noise,
+                noise_seed=self.noise_seed,
+                settings=SettingsExtract(
+                    pixels_from_end=layout.extract.parallel_fpr.total_rows_min
+                ),
+            )
+
         if cti is not None:
             post_cti_data = clocker.add_cti(data=pre_cti_data, cti=cti)
         else:
-            post_cti_data = pre_cti_data
+            post_cti_data = copy.copy(pre_cti_data)
 
         if cosmic_ray_map is not None:
             pre_cti_data -= cosmic_ray_map.native
 
         return self.via_post_cti_data_from(
             post_cti_data=post_cti_data,
             pre_cti_data=pre_cti_data,
@@ -227,17 +229,15 @@
 
     def via_post_cti_data_from(
         self,
         post_cti_data: aa.Array2D,
         pre_cti_data: aa.Array2D,
         layout: Layout2DCI,
         cosmic_ray_map: Optional[aa.Array2D] = None,
-        name: Optional[str] = None,
     ) -> ImagingCI:
-
         if self.read_noise is not None:
             ci_image = aa.preprocess.data_with_gaussian_noise_added(
                 data=post_cti_data, sigma=self.read_noise, seed=self.noise_seed
             )
 
             ci_image = aa.Array2D.no_mask(
                 values=ci_image, pixel_scales=self.pixel_scales
@@ -254,15 +254,15 @@
             ci_noise_map = aa.Array2D.full(
                 fill_value=self.noise_if_add_noise_false,
                 shape_native=layout.shape_2d,
                 pixel_scales=self.pixel_scales,
             ).native
 
         return ImagingCI(
-            image=aa.Array2D.no_mask(
+            data=aa.Array2D.no_mask(
                 values=ci_image.native, pixel_scales=self.pixel_scales
             ),
             noise_map=aa.Array2D.no_mask(
                 values=ci_noise_map, pixel_scales=self.pixel_scales
             ),
             pre_cti_data=aa.Array2D.no_mask(
                 values=pre_cti_data.native, pixel_scales=self.pixel_scales
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/layout.py` & `autocti-2023.7.7.2/autocti/charge_injection/layout.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,28 +65,26 @@
             serial_overscan=serial_overscan,
         )
 
         self.electronics = electronics
 
     @property
     def extract(self) -> Extract2DMaster:
-
         from autocti.extract.two_d.master import Extract2DMaster
 
         return Extract2DMaster(
             shape_2d=self.shape_2d,
             region_list=self.region_list,
             parallel_overscan=self.parallel_overscan,
             serial_prescan=self.serial_prescan,
             serial_overscan=self.serial_overscan,
         )
 
     @classmethod
     def from_euclid_fits_header(cls, ext_header):
-
         serial_overscan_size = ext_header.get("OVRSCANX", default=None)
         serial_prescan_size = ext_header.get("PRESCANX", default=None)
         serial_size = ext_header.get("NAXIS1", default=None)
         parallel_size = ext_header.get("NAXIS2", default=None)
 
         electronics = ElectronicsCI.from_ext_header(ext_header=ext_header)
 
@@ -177,15 +175,14 @@
             Input ci_seed for the random number generator to give reproducible results. A new ci_seed is always used for each \
             pre_cti_datas, ensuring each non-uniform ci_region has the same column non-uniformity layout_ci.
         """
 
         pre_cti_data = np.zeros(self.shape_2d)
 
         for region in self.region_list:
-
             pre_cti_data[region.slice] += ci_util.region_ci_from(
                 region_dimensions=region.shape,
                 injection_norm_list=injection_norm_list,
                 row_slope=row_slope,
             )
 
         return aa.Array2D.no_mask(values=pre_cti_data, pixel_scales=pixel_scales)
@@ -219,23 +216,87 @@
             Input ci_seed for the random number generator to give reproducible results. A new ci_seed is always used for each \
             pre_cti_datas, ensuring each non-uniform ci_region has the same column non-uniformity layout_ci.
         """
 
         pre_cti_data = np.zeros(self.shape_2d)
 
         for region_index, region in enumerate(self.region_list):
-
             pre_cti_data[region.slice] += ci_util.region_ci_from(
                 region_dimensions=region.shape,
                 injection_norm_list=injection_norm_lists[region_index],
                 row_slope=row_slope,
             )
 
         return aa.Array2D.no_mask(values=pre_cti_data, pixel_scales=pixel_scales)
 
+    def noise_map_non_uniform_from(
+        self,
+        injection_std_list: List[float],
+        pixel_scales: aa.type.PixelScales,
+        read_noise: float = 0.0,
+    ) -> aa.Array2D:
+        """
+        Use this charge injection layout to generate the noise-map of a charge injection image. This is performed by
+        going to its charge injection regions and adding an input RMS standard deviation value to each column, which
+        are passed in as a list.
+
+        For one column of a non-uniform charge injection noise-map, this function assumes that each non-uniform
+        charge injection region has the same overall noise value.
+
+        A read-noise can also be be included when creating the noise map, which is added in quadrature to the
+        charge injection noise values.
+        """
+
+        noise_map = np.full(fill_value=read_noise, shape=self.shape_2d)
+
+        for region in self.region_list:
+            noise_region = ci_util.region_ci_from(
+                region_dimensions=region.shape,
+                injection_norm_list=injection_std_list,
+            )
+
+            noise_map[region.slice] = np.sqrt(
+                np.square(read_noise) + np.square(noise_region)
+            )
+
+        return aa.Array2D.no_mask(values=noise_map, pixel_scales=pixel_scales)
+
+    def noise_map_non_uniform_via_lists_from(
+        self,
+        injection_std_lists: List[List[float]],
+        pixel_scales: aa.type.PixelScales,
+        read_noise: float = 0.0,
+    ) -> aa.Array2D:
+        """
+        Use this charge injection layout to generate the noise-map of a charge injection image. This is performed by
+        going to its charge injection regions and adding an input RMS standard deviation value to each column, which
+        are passed in as a list.
+
+        For one column of a non-uniform charge injection pre-cti image, this function assumes that each non-uniform
+        charge injection region can have a different noise value. The alues `injection_std_lists` are passed as a
+        list of lists so that the RMS standard deviation of each injection in each region can be specified.
+
+        A read-noise can also be be included when creating the noise map, which is added in quadrature to the
+        charge injection noise values.
+        """
+
+        noise_map = np.full(fill_value=read_noise, shape=self.shape_2d)
+
+        for region_index, region in enumerate(self.region_list):
+            noise_region = ci_util.region_ci_from(
+                region_dimensions=region.shape,
+                injection_norm_list=injection_std_lists[region_index],
+            )
+
+            noise_map[region.slice] = np.sqrt(
+                np.square(read_noise) + np.square(noise_region)
+            )
+
+        return aa.Array2D.no_mask(values=noise_map, pixel_scales=pixel_scales)
+
 
 class ElectronicsCI:
     def __init__(
         self,
         injection_on: Optional[int] = None,
         injection_off: Optional[int] = None,
         injection_start: Optional[int] = None,
@@ -337,16 +398,14 @@
         """
         The total number of charge injection regions for these electronics settings.
         """
 
         injection_range = self.injection_end - self.injection_start
 
         for injection_total in range(100):
-
             total_pixels = math.floor(
                 (injection_total + 1) * (self.injection_on)
                 + injection_total * self.injection_off
             )
 
             if total_pixels > injection_range:
-
                 return injection_total
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/master.py` & `autocti-2023.7.7.2/autocti/charge_injection/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/mock/mock_result.py` & `autocti-2023.7.7.2/autocti/charge_injection/mock/mock_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         model_image=None,
         noise_scaling_map_dict_list_of_regions_ci=None,
         noise_scaling_map_dict_list_of_parallel_eper=None,
         noise_scaling_map_dict_list_of_serial_eper=None,
         noise_scaling_map_dict_list_of_serial_overscan_no_eper=None,
         use_as_hyper_dataset=False,
     ):
-
         super().__init__(
             samples=samples,
             instance=instance,
             model=model,
             analysis=analysis,
             search=search,
         )
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/ou_sim_ci.py` & `autocti-2023.7.7.2/autocti/charge_injection/ou_sim_ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 """
 
 
 def quadrant_id_from(iquad: int) -> str:
     """
     The ELVIS simulator uses the `iquad` parameter to determine how images are rotated before clocking via arctic.
 
-    This script converts this parameter to the the `quadrant_id` used by PyAutoCTI, which in turn gives the appropriate
+    This script converts this parameter to the `quadrant_id` used by PyAutoCTI, which in turn gives the appropriate
     `roe_corner` for rotation.
 
     The mapping of `iquad` to `quadrant_id` does not depend on the CCD id, because ELVIS has already performed
     extractions / rotations on the quadrant data beforehand.
 
     Parameters
     ----------
@@ -84,15 +84,14 @@
     """
     The total number of charge injection regions for these electronics settings.
     """
 
     injection_range = injection_end - injection_start
 
     for injection_total in range(100):
-
         total_pixels = math.floor(
             (injection_total + 1) * (injection_on) + injection_total * injection_off
         )
 
         if total_pixels > injection_range:
             return injection_total
 
@@ -186,27 +185,25 @@
     """
     The simulator object creates simulations of charge injeciton imaging.
     """
     """
     Create every pre-cti charge injection image using each `Layout2DCI`
     """
     if use_non_uniform_pattern:
-
         simulator = SimulatorImagingCI(
             pixel_scales=pixel_scales,
             norm=injection_norm,
             row_slope=0.0,
             column_sigma=100.0,
             max_norm=200000,
             ci_seed=ci_seed,
         )
 
         pre_cti_data = simulator.pre_cti_data_non_uniform_from(layout=layout)
     else:
-
         simulator = SimulatorImagingCI(pixel_scales=pixel_scales, norm=injection_norm)
 
         pre_cti_data = simulator.pre_cti_data_uniform_from(layout=layout)
 
     """
     The OU-SIM parameter iquad defines the quadrant_id of the data (e.g. "E", "F", "G" or "H").
     """
@@ -229,15 +226,14 @@
     quadrant_id: str,
     clocker: Clocker2D,
     parallel_trap_list: List[TrapInstantCapture],
     parallel_ccd: CCDPhase,
     serial_trap_list: List[TrapInstantCapture],
     serial_ccd: CCDPhase,
 ) -> Union[np.ndarray, Array2D]:
-
     #  quadrant_id = quadrant_id_from(iquad=iquad)
 
     roe_corner = euclid_util.roe_corner_from(ccd_id=ccd_id, quadrant_id=quadrant_id)
 
     pre_cti_data = layout_util.rotate_array_via_roe_corner_from(
         array=pre_cti_data, roe_corner=roe_corner
     )
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/plot/fit_ci_plotters.py` & `autocti-2023.7.7.2/autocti/dataset_1d/plot/fit_plotters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,440 +1,350 @@
-from typing import Callable
+import numpy as np
+from typing import Callable, Optional
 
 import autoarray.plot as aplt
 
-from autoarray.fit.plot.fit_imaging_plotters import FitImagingPlotterMeta
 from autoarray.plot.auto_labels import AutoLabels
 
 from autocti.plot.abstract_plotters import Plotter
-from autocti.charge_injection.fit import FitImagingCI
+from autocti.dataset_1d.fit import FitDataset1D
 
 
-class FitImagingCIPlotter(Plotter):
+class FitDataset1DPlotter(Plotter):
     def __init__(
         self,
-        fit: FitImagingCI,
-        mat_plot_2d: aplt.MatPlot2D = aplt.MatPlot2D(),
-        visuals_2d: aplt.Visuals2D = aplt.Visuals2D(),
-        include_2d: aplt.Include2D = aplt.Include2D(),
+        fit: FitDataset1D,
         mat_plot_1d: aplt.MatPlot1D = aplt.MatPlot1D(),
         visuals_1d: aplt.Visuals1D = aplt.Visuals1D(),
         include_1d: aplt.Include1D = aplt.Include1D(),
     ):
         """
-        Plots the attributes of `FitImagingCI` objects using the matplotlib methods `imshow()`, `plot()` and many other
-        matplotlib functions which customize the plot's appearance.
+        Plots the attributes of `FitDataset1D` objects using the matplotlib method `line()` and many other matplotlib
+        functions which customize the plot's appearance.
 
-        The `mat_plot_1d` and `mat_plot_2d` attribute wraps matplotlib function calls to make the figure. By default,
-        the settings passed to every matplotlib function called are those specified in
-        the `config/visualize/mat_wrap/*.ini` files, but a user can manually input values into `MatPlot1D` and
-        `MatPlot2D` to customize the figure's appearance.
-
-        Overlaid on the figure are visuals, contained in the `Visuals1D` and `Visuals2D` object. Attributes may be
-        extracted from the `FitImagingCI` and plotted via the visuals object, if the corresponding entry
-        is `True` in the `Include1D` and `Include2D` object or the `config/visualize/include.ini` file.
+        The `mat_plot_1d` attribute wraps matplotlib function calls to make the figure. By default, the settings
+        passed to every matplotlib function called are those specified in the `config/visualize/mat_wrap/*.ini` files,
+        but a user can manually input values into `MatPlot1d` to customize the figure's appearance.
+
+        Overlaid on the figure are visuals, contained in the `Visuals1D` object. Attributes may be extracted from
+        the `Imaging` and plotted via the visuals object, if the corresponding entry is `True` in the `Include1D`
+        object or the `config/visualize/include.ini` file.
 
         Parameters
         ----------
         fit
-            The fit to an imaging dataset the plotter plots.
-        get_visuals_2d
-            A function which extracts from the `FitImaging` the 2D visuals which are plotted on figures.
-        mat_plot_2d
-            Contains objects which wrap the matplotlib function calls that make the plot.
-        visuals_2d
-            Contains visuals that can be overlaid on the plot.
-        include_2d
-            Specifies which attributes of the `Array2D` are extracted and plotted as visuals.
+            The fit to the dataset of a 1D dataset the plotter plots.
         mat_plot_1d
             Contains objects which wrap the matplotlib function calls that make 1D plots.
         visuals_1d
             Contains 1D visuals that can be overlaid on 1D plots.
         include_1d
             Specifies which attributes of the `ImagingCI` are extracted and plotted as visuals for 1D plots.
         """
-        super().__init__(
-            mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
-        )
-
-        self.visuals_1d = visuals_1d
-        self.include_1d = include_1d
-        self.mat_plot_1d = mat_plot_1d
-
         self.fit = fit
 
-        self._fit_imaging_meta_plotter = FitImagingPlotterMeta(
-            fit=self.fit,
-            get_visuals_2d=self.get_visuals_2d,
-            mat_plot_2d=self.mat_plot_2d,
-            include_2d=self.include_2d,
-            visuals_2d=self.visuals_2d,
+        super().__init__(
+            dataset=fit.dataset,
+            mat_plot_1d=mat_plot_1d,
+            include_1d=include_1d,
+            visuals_1d=visuals_1d,
         )
 
-    def get_visuals_2d(self):
-        return self.get_2d.via_fit_imaging_ci_from(fit=self.fit)
+    def get_visuals_1d(self) -> aplt.Visuals1D:
+        return self.visuals_1d
 
     @property
     def extract_region_from(self) -> Callable:
-        return self.fit.imaging_ci.layout.extract_region_from
+        return self.fit.dataset.layout.extract_region_from
 
-    def figures_2d(
+    def figures_1d(
         self,
-        image: bool = False,
+        region: Optional[str] = None,
+        data: bool = False,
+        data_logy: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         pre_cti_data: bool = False,
         post_cti_data: bool = False,
         residual_map: bool = False,
+        residual_map_logy: bool = False,
         normalized_residual_map: bool = False,
         chi_squared_map: bool = False,
     ):
         """
-        Plots the individual attributes of the plotter's `FitImagingCI` object in 2D.
+        Plots the individual attributes of the plotter's `FitDataset1D` object in 1D.
 
-        The API is such that every plottable attribute of the `FitImagingCI` object is an input parameter of type bool
+        The API is such that every plottable attribute of the `FitDataset1D` object is an input parameter of type bool
         of the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
-        image
-            Whether or not to make a 2D plot (via `imshow`) of the image data.
+        region
+            The region on the 1D dataset where data is extracted and binned {fpr", "eper"}
+        data
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars.
+        data_logy
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars and the y-axis on a log10 scale.
         noise_map
-            Whether or not to make a 2D plot (via `imshow`) of the noise map.
+            Whether to make a 1D plot (via `plot`) of the noise map.
         signal_to_noise_map
-            Whether or not to make a 2D plot (via `imshow`) of the signal-to-noise map.
+            Whether to make a 1D plot (via `plot`) of the signal-to-noise map.
         pre_cti_data
-            Whether or not to make a 2D plot (via `imshow`) of the pre-cti data.
+            Whether to make a 1D plot (via `plot`) of the pre-cti data.
         post_cti_data
-            Whether or not to make a 2D plot (via `imshow`) of the post-cti data.
+            Whether to make a 1D plot (via `plot`) of the post-cti data.
         residual_map
-            Whether or not to make a 2D plot (via `imshow`) of the residual map.
+            Whether to make a 1D plot (via `plot`) of the residual map, with the noise-map values included as error
+            bars.
+        residual_map_logy
+            Whether to make a 1D plot (via `plot`) of the residual map, with the noise-map values included as error
+            bars and the y-axis on a log10 scale.
         normalized_residual_map
-            Whether or not to make a 2D plot (via `imshow`) of the normalized residual map.
+            Whether to make a 1D plot (via `plot`) of the normalized residual map.
         chi_squared_map
-            Whether or not to make a 2D plot (via `imshow`) of the chi-squared map.
+            Whether to make a 1D plot (via `plot`) of the chi-squared map.
         """
-        self._fit_imaging_meta_plotter.figures_2d(
-            image=image,
-            noise_map=noise_map,
-            signal_to_noise_map=signal_to_noise_map,
-            residual_map=residual_map,
-            normalized_residual_map=normalized_residual_map,
-            chi_squared_map=chi_squared_map,
-        )
 
-        if pre_cti_data:
+        suffix = f"_{region}" if region is not None else ""
+        title_str = self.title_str_from(region=region)
 
-            self.mat_plot_2d.plot_array(
-                array=self.fit.pre_cti_data,
-                visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(
-                    title="CI Pre CTI Image", filename="pre_cti_data"
-                ),
-            )
+        y_errors = self.extract_region_from(array=self.fit.noise_map, region=region)
+        y_extra = self.extract_region_from(array=self.fit.model_data, region=region)
 
-        if post_cti_data:
+        if data:
+            y = self.extract_region_from(array=self.fit.data, region=region)
 
-            self.mat_plot_2d.plot_array(
-                array=self.fit.post_cti_data,
-                visuals_2d=self.get_visuals_2d(),
+            self.mat_plot_1d.plot_yx(
+                y=y,
+                x=range(len(y)),
+                plot_axis_type_override="errorbar",
+                y_errors=y_errors,
+                y_extra=y_extra,
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title="CI Post CTI Image", filename="post_cti_data"
+                    title=f"Data {title_str}",
+                    yunit="e-",
+                    filename=f"data{suffix}",
                 ),
             )
 
-    def figures_1d_of_region(
-        self,
-        region,
-        image: bool = False,
-        noise_map: bool = False,
-        signal_to_noise_map: bool = False,
-        pre_cti_data: bool = False,
-        post_cti_data: bool = False,
-        residual_map: bool = False,
-        normalized_residual_map: bool = False,
-        chi_squared_map: bool = False,
-    ):
-        """
-        Plots the individual attributes of the plotter's `FitImagingCI` object in 1D.
-
-        These 1D plots correspond to a region in 2D on the charge injection image, which is binned up over the parallel
-        or serial direction to produce a 1D plot. For example, for the input `region=parallel_fpr`, this
-        function extracts the FPR over each charge injection region and bins such that the 1D plot shows the FPR
-        in the parallel direction.
-
-        The API is such that every plottable attribute of the `FitImagingCI` object is an input parameter of type bool
-        of the function, which if switched to `True` means that it is plotted.
-
-        Parameters
-        ----------
-        region
-            The region on the charge injection image where data is extracted and binned over the parallel or serial
-            direction {"parallel_fpr", "parallel_eper", "serial_fpr", "serial_eper"}
-        image
-            Whether or not to make a 1D plot (via `plot`) of the image data extracted and binned over the region.
-        noise_map
-            Whether or not to make a 1D plot (via `plot`) of the noise-map extracted and binned over the region.
-        signal_to_noise_map
-            Whether or not to make a 1D plot (via `plot`) of the signal-to-noise map data extracted and binned over
-            the region.
-        pre_cti_data
-            Whether or not to make a 1D plot (via `plot`) of the pre-cti data extracted and binned over the region.
-        post_cti_data
-            Whether or not to make a 1D plot (via `plot`) of the post-cti data extracted and binned over the
-            region.
-        residual_map
-            Whether or not to make a 1D plot (via `plot`) of the residual map extracted and binned over the region.
-        normalized_residual_map
-            Whether or not to make a 1D plot (via `plot`) of the normalized residual map extracted and binned over the
-            region.
-        chi_squared_map
-            Whether or not to make a 1D plot (via `plot`) of the chi-squared map extracted and binned over the
-            region.
-        """
-        if image:
-
-            y = self.extract_region_from(array=self.fit.image, region=region)
+        if data_logy:
+            y = self.extract_region_from(array=self.fit.data, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                plot_axis_type_override="errorbar_logy",
+                y_errors=y_errors,
+                y_extra=y_extra,
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Image {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"image_{region}",
+                    title=f"Data {title_str} [log10]",
+                    yunit="e-",
+                    filename=f"data_logy{suffix}",
                 ),
             )
 
         if noise_map:
-
-            y = self.extract_region_from(array=self.fit.image, region=region)
+            y = self.extract_region_from(array=self.fit.noise_map, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Noise-Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"noise_map_{region}",
+                    title="Noise-Map",
+                    yunit="e-",
+                    filename=f"noise_map{suffix}",
                 ),
             )
 
         if signal_to_noise_map:
-
             y = self.extract_region_from(
                 array=self.fit.signal_to_noise_map, region=region
             )
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Signal-To-Noise Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"signal_to_noise_map_{region}",
+                    title="Signal-To-Noise Map",
+                    yunit="",
+                    filename=f"signal_to_noise_map{suffix}",
                 ),
             )
 
-        if pre_cti_data:
-
-            y = self.extract_region_from(array=self.fit.pre_cti_data, region=region)
+        if residual_map:
+            y = self.extract_region_from(array=self.fit.residual_map, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                plot_axis_type_override="errorbar",
+                y_errors=y_errors,
+                y_extra=np.zeros(shape=y.shape),
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"CI Pre CTI {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"pre_cti_data_{region}",
+                    title=f"Residual Map {title_str}",
+                    yunit="e-",
+                    filename=f"residual_map{suffix}",
                 ),
             )
 
-        if post_cti_data:
-
-            y = self.extract_region_from(array=self.fit.post_cti_data, region=region)
+        if residual_map_logy:
+            y = self.extract_region_from(array=self.fit.residual_map, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                plot_axis_type_override="errorbar_logy",
+                y_errors=y_errors,
+                y_extra=1.0001 * np.zeros(shape=y.shape),
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"CI Post CTI {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"post_cti_data_{region}",
+                    title=f"Residual Map {title_str}",
+                    ylabel="e-",
+                    filename=f"residual_map_logy{suffix}",
                 ),
             )
 
-        if residual_map:
-
-            y = self.extract_region_from(array=self.fit.residual_map, region=region)
+        if normalized_residual_map:
+            y = self.extract_region_from(
+                array=self.fit.normalized_residual_map, region=region
+            )
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Resdial-Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"residual_map_{region}",
+                    title="Normalized Residual Map",
+                    yunit=r"\sigma",
+                    filename=f"normalized_residual_map{suffix}",
                 ),
             )
 
-        if normalized_residual_map:
+        if chi_squared_map:
+            y = self.extract_region_from(array=self.fit.chi_squared_map, region=region)
 
-            y = self.extract_region_from(
-                array=self.fit.normalized_residual_map, region=region
+            self.mat_plot_1d.plot_yx(
+                y=y,
+                x=range(len(y)),
+                visuals_1d=self.get_visuals_1d(),
+                auto_labels=AutoLabels(
+                    title="Chi-Squared Map",
+                    yunit=r"\chi^2",
+                    filename=f"chi_squared_map{suffix}",
+                ),
             )
 
+        if pre_cti_data:
+            y = self.extract_region_from(array=self.fit.pre_cti_data, region=region)
+
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Normalized Residual Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"normalized_residual_map_{region}",
+                    title="CI Pre CTI Image",
+                    yunit="e-",
+                    filename=f"pre_cti_data{suffix}",
                 ),
             )
 
-        if chi_squared_map:
-
-            y = self.extract_region_from(array=self.fit.chi_squared_map, region=region)
+        if post_cti_data:
+            y = self.extract_region_from(array=self.fit.post_cti_data, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
-                visuals_1d=self.visuals_1d,
+                visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Chi-Squared Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"chi_squared_map_{region}",
+                    title="CI Post CTI Image",
+                    yunit="e-",
+                    filename=f"post_cti_data{suffix}",
                 ),
             )
 
     def subplot(
         self,
-        image: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         pre_cti_data: bool = False,
         post_cti_data: bool = False,
         residual_map: bool = False,
         normalized_residual_map: bool = False,
         chi_squared_map: bool = False,
-        auto_filename: str = "subplot_fit_ci",
+        auto_filename="subplot_fit",
+        **kwargs,
     ):
         """
-        Plots the individual attributes of the plotter's `FitImagingCI` object in 2D on a subplot.
+        Plots the individual attributes of the plotter's `FitDataset1D` object in 1D on a subplot.
 
-        The API is such that every plottable attribute of the `FitImagingCI` object is an input parameter of type bool
+        The API is such that every plottable attribute of the `FitDataset1D` object is an input parameter of type bool
         of the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
-        image
-            Whether or not to include a 2D plot (via `imshow`) of the image data.
+        data
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars.
         noise_map
-            Whether or not to include a 2D plot (via `imshow`) noise map.
+            Whether to include a 1D plot (via `plot`) of the noise map.
         signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) signal-to-noise map.
+            Whether to include a 1D plot (via `plot`) of the signal-to-noise map.
         pre_cti_data
-            Whether or not to include a 2D plot (via `imshow`) of the pre-cti data.
+            Whether to include a 1D plot (via `plot`) of the pre-cti data.
         post_cti_data
-            Whether or not to include a 2D plot (via `imshow`) of the post-cti data.
+            Whether to include a 1D plot (via `plot`) of the post-cti data.
         residual_map
-            Whether or not to include a 2D plot (via `imshow`) residual map.
+            Whether to include a 1D plot (via `plot`) of the residual map.
         normalized_residual_map
-            Whether or not to include a 2D plot (via `imshow`) normalized residual map.
+            Whether to include a 1D plot (via `plot`) of the normalized residual map.
         chi_squared_map
-            Whether or not to include a 2D plot (via `imshow`) chi-squared map.
-        auto_filename
-            The default filename of the output subplot if written to hard-disk.
+            Whether to include a 1D plot (via `plot`) of the chi-squared map.
         """
+
+        region = kwargs.get("region", None)
+        suffix = f"_{region}" if region is not None else ""
+
         self._subplot_custom_plot(
-            image=image,
+            data=data,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
             pre_cti_data=pre_cti_data,
             post_cti_data=post_cti_data,
             residual_map=residual_map,
             normalized_residual_map=normalized_residual_map,
             chi_squared_map=chi_squared_map,
-            auto_labels=AutoLabels(filename=auto_filename),
+            auto_labels=AutoLabels(
+                yunit="e-",
+                xlabel="Pixel No.",
+                filename=f"{auto_filename}{suffix}",
+            ),
         )
 
-    def subplot_fit_ci(self):
+    def subplot_fit(self, region: Optional[str] = None):
         """
-        Standard subplot of the attributes of the plotter's `FitImaging` object.
+        Standard subplot of the attributes of the plotter's `FitDataset1D` object.
         """
         return self.subplot(
-            image=True,
+            region=region,
+            data=True,
             signal_to_noise_map=True,
             pre_cti_data=True,
             post_cti_data=True,
             normalized_residual_map=True,
             chi_squared_map=True,
         )
-
-    def subplot_1d_of_region(self, region: str):
-        """
-        Plots the individual attributes of the plotter's `FitImagingCI` object in 1D on a subplot.
-
-        These 1D plots correspond to a region in 2D on the charge injection image, which is binned up over the parallel
-        or serial direction to produce a 1D plot. For example, for the input `region=parallel_fpr`, this
-        function extracts the FPR over each charge injection region and bins such that the 1D plot shows the FPR
-        in the parallel direction.
-
-        The function plots the image, noise map, pre-cti data and signal to noise map in 1D on the subplot.
-
-        Parameters
-        ----------
-        region
-            The region on the charge injection image where data is extracted and binned over the parallel or serial
-            direction {"parallel_fpr", "parallel_eper", "serial_fpr", "serial_eper"}
-        """
-
-        self.open_subplot_figure(number_subplots=6)
-
-        self.figures_1d_of_region(image=True, region=region)
-        self.figures_1d_of_region(signal_to_noise_map=True, region=region)
-        self.figures_1d_of_region(pre_cti_data=True, region=region)
-        self.figures_1d_of_region(post_cti_data=True, region=region)
-        self.figures_1d_of_region(normalized_residual_map=True, region=region)
-        self.figures_1d_of_region(chi_squared_map=True, region=region)
-
-        self.mat_plot_1d.output.subplot_to_figure(
-            auto_filename=f"subplot_1d_fit_ci_{region}"
-        )
-        self.close_subplot_figure()
-
-    def subplot_noise_scaling_map_dict(self):
-        """
-        Plots the noise-scaling maps of the plotter's `FitImagingCI` object in 2D on a subplot.
-        """
-
-        self.open_subplot_figure(number_subplots=len(self.fit.noise_scaling_map_dict))
-
-        for key, noise_scaling_map in self.fit.noise_scaling_map_dict.items():
-
-            self.mat_plot_2d.plot_array(
-                array=noise_scaling_map,
-                visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(title=f"Noise Scaling Map {key}"),
-            )
-
-        self.mat_plot_2d.output.subplot_to_figure(
-            auto_filename=f"subplot_noise_scaling_map_dict"
-        )
-        self.mat_plot_2d.figure.close()
```

### Comparing `autocti-2023.1.15.1/autocti/charge_injection/plot/imaging_ci_plotters.py` & `autocti-2023.7.7.2/autocti/charge_injection/plot/imaging_ci_plotters.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,277 +46,287 @@
             Contains objects which wrap the matplotlib function calls that make 1D plots.
         visuals_1d
             Contains 1D visuals that can be overlaid on 1D plots.
         include_1d
             Specifies which attributes of the `ImagingCI` are extracted and plotted as visuals for 1D plots.
         """
         super().__init__(
-            mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
+            dataset=dataset,
+            mat_plot_2d=mat_plot_2d,
+            include_2d=include_2d,
+            visuals_2d=visuals_2d,
         )
 
         self.visuals_1d = visuals_1d
         self.include_1d = include_1d
         self.mat_plot_1d = mat_plot_1d
 
-        self.dataset = dataset
-
         self._imaging_meta_plotter = ImagingPlotterMeta(
-            imaging=self.imaging,
+            dataset=self.dataset,
             get_visuals_2d=self.get_visuals_2d,
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
         )
 
-    @property
-    def imaging(self):
-        return self.dataset
-
     def get_visuals_1d(self):
         return self.visuals_1d
 
     def get_visuals_2d(self):
-        return self.get_2d.via_mask_from(mask=self.imaging.mask)
+        return self.get_2d.via_mask_from(mask=self.dataset.mask)
 
     @property
     def extract_region_from(self) -> Callable:
-        return self.imaging.layout.extract_region_from
+        return self.dataset.layout.extract_region_from
+
+    @property
+    def extract_region_noise_map_from(self) -> Callable:
+        return self.dataset.layout.extract_region_noise_map_from
 
     def figures_2d(
         self,
-        image: bool = False,
+        data: bool = False,
         noise_map: bool = False,
-        inverse_noise_map: bool = False,
         signal_to_noise_map: bool = False,
-        absolute_signal_to_noise_map: bool = False,
-        potential_chi_squared_map: bool = False,
         pre_cti_data: bool = False,
         cosmic_ray_map: bool = False,
     ):
         """
         Plots the individual attributes of the plotter's `ImagingCI` object in 2D.
 
         The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
-        image
-            Whether or not to make a 2D plot (via `imshow`) of the image data.
+        data
+            Whether to make a 2D plot (via `imshow`) of the image data.
         noise_map
-            Whether or not to make a 2D plot (via `imshow`) of the noise map.
-        inverse_noise_map
-            Whether or not to make a 2D plot (via `imshow`) of the inverse noise map.
+            Whether to make a 2D plot (via `imshow`) of the noise map.
         signal_to_noise_map
-            Whether or not to make a 2D plot (via `imshow`) of the signal-to-noise map.
-        absolute_signal_to_noise_map
-            Whether or not to make a 2D plot (via `imshow`) of the absolute signal to noise map.
-        potential_chi_squared_map
-            Whether or not to make a 2D plot (via `imshow`) of the potential chi squared map.
+            Whether to make a 2D plot (via `imshow`) of the signal-to-noise map.
         pre_cti_data
-            Whether or not to make a 2D plot (via `imshow`) of the pre-cti data.
+            Whether to make a 2D plot (via `imshow`) of the pre-cti data.
         cosmic_ray_map
-            Whether or not to make a 2D plot (via `imshow`) of the cosmic ray map.
+            Whether to make a 2D plot (via `imshow`) of the cosmic ray map.
         """
 
         self._imaging_meta_plotter.figures_2d(
-            image=image,
+            data=data,
             noise_map=noise_map,
-            inverse_noise_map=inverse_noise_map,
             signal_to_noise_map=signal_to_noise_map,
-            absolute_signal_to_noise_map=absolute_signal_to_noise_map,
-            potential_chi_squared_map=potential_chi_squared_map,
         )
 
         if pre_cti_data:
-
             self.mat_plot_2d.plot_array(
-                array=self.imaging.pre_cti_data,
+                array=self.dataset.pre_cti_data,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
                     title="CI Pre CTI Image", filename="pre_cti_data"
                 ),
             )
 
         if cosmic_ray_map:
-
             self.mat_plot_2d.plot_array(
-                array=self.imaging.cosmic_ray_map,
+                array=self.dataset.cosmic_ray_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
                     title="Cosmic Ray Map", filename="cosmic_ray_map"
                 ),
             )
 
-    def figures_1d_of_region(
+    def figures_1d(
         self,
         region: str,
-        image: bool = False,
+        data: bool = False,
+        data_logy: bool = False,
         noise_map: bool = False,
         pre_cti_data: bool = False,
         signal_to_noise_map: bool = False,
     ):
         """
-        Plots the individual attributes of the plotter's `ImagingCI` object in 1D.
+        Plots the individual attributes of the plotter's `ImagingCI` object in 2D.
 
-        These 1D plots correspond to a region in 2D on the charge injection image, which is binned up over the parallel
-        or serial direction to produce a 1D plot. For example, for the input `region=parallel_fpr`, this
-        function extracts the FPR over each charge injection region and bins such that the 1D plot shows the FPR
-        in the parallel direction.
+        The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
+        the function, which if switched to `True` means that it is plotted.
+
+        if a `region` string is input, the 1D plots correspond to a region in 2D on the charge injection image, which
+        is binned up over the parallel or serial direction to produce a 1D plot. For example, for the
+        input `region=parallel_fpr`, this function extracts the FPR over each charge injection region and bins such
+        that the 1D plot shows the FPR in the parallel direction.
 
         The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
         region
             The region on the charge injection image where data is extracted and binned over the parallel or serial
             direction {"parallel_fpr", "parallel_eper", "serial_fpr", "serial_eper"}
-        image
-            Whether or not to make a 1D plot (via `plot`) of the image data extracted and binned over the region.
+        data
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars.
+        data_logy
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars and the y-axis on a log10 scale.
         noise_map
-            Whether or not to make a 1D plot (via `plot`) of the noise-map extracted and binned over the region.
+            Whether to make a 1D plot (via `plot`) of the noise-map extracted and binned over the region.
         pre_cti_data
-            Whether or not to make a 1D plot (via `plot`) of the pre-cti data extracted and binned over the region.
+            Whether to make a 1D plot (via `plot`) of the pre-cti data extracted and binned over the region.
         signal_to_noise_map
-            Whether or not to make a 1D plot (via `plot`) of the signal-to-noise map data extracted and binned over
+            Whether to make a 1D plot (via `plot`) of the signal-to-noise map data extracted and binned over
             the region.
         """
 
-        if image:
+        if region == "fpr_non_uniformity":
+            ls_errorbar = "-"
+        else:
+            ls_errorbar = ""
+
+        title_str = self.title_str_from(region=region)
+
+        if data:
+            y = self.extract_region_from(array=self.dataset.data, region=region)
+            y_errors = self.extract_region_noise_map_from(
+                array=self.dataset.noise_map, region=region
+            )
+
+            self.mat_plot_1d.plot_yx(
+                y=y,
+                x=range(len(y)),
+                plot_axis_type_override="errorbar",
+                y_errors=y_errors,
+                ls_errorbar=ls_errorbar,
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
+                visuals_1d=self.get_visuals_1d(),
+                auto_labels=AutoLabels(
+                    title=f"Data {title_str}",
+                    yunit="e-",
+                    filename=f"data_{region}",
+                ),
+            )
 
-            y = self.extract_region_from(array=self.imaging.image, region=region)
+        if data_logy:
+            y = self.extract_region_from(array=self.dataset.data, region=region)
+            y_errors = self.extract_region_noise_map_from(
+                array=self.dataset.noise_map, region=region
+            )
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
+                plot_axis_type_override="errorbar_logy",
+                y_errors=y_errors,
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
                 visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title=f"Image {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"image_{region}",
+                    title=f"Data {title_str} [log10 y]",
+                    yunit="e-",
+                    filename=f"data_logy_{region}",
                 ),
             )
 
         if noise_map:
-
-            y = self.extract_region_from(array=self.imaging.noise_map, region=region)
+            y = self.extract_region_from(array=self.dataset.noise_map, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title=f"Noise Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
+                    title=f"Noise Map {title_str}",
+                    ylabel="Noise (e-)",
                     filename=f"noise_map_{region}",
                 ),
             )
 
         if pre_cti_data:
-
-            y = self.extract_region_from(array=self.imaging.pre_cti_data, region=region)
+            y = self.extract_region_from(array=self.dataset.pre_cti_data, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title=f"CI Pre CTI {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
+                    title=f"CI Pre CTI {title_str}",
+                    yunit="e-",
                     filename=f"pre_cti_data_{region}",
                 ),
             )
 
         if signal_to_noise_map:
-
             y = self.extract_region_from(
-                array=self.imaging.signal_to_noise_map, region=region
+                array=self.dataset.signal_to_noise_map, region=region
             )
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title=f"Signal To Noise Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
+                    title=f"Signal To Noise Map {title_str}",
+                    ylabel="Signal To Noise (e-)",
                     filename=f"signal_to_noise_map_{region}",
                 ),
             )
 
     def subplot(
         self,
-        image=False,
-        noise_map=False,
-        inverse_noise_map=False,
-        signal_to_noise_map=False,
-        absolute_signal_to_noise_map=False,
-        potential_chi_squared_map=False,
-        pre_cti_data=False,
-        cosmic_ray_map=False,
-        auto_filename="subplot_imaging_ci",
+        data: bool = False,
+        noise_map: bool = False,
+        signal_to_noise_map: bool = False,
+        pre_cti_data: bool = False,
+        cosmic_ray_map: bool = False,
+        auto_filename="subplot_dataset",
     ):
         """
         Plots the individual attributes of the plotter's `ImagingCI` object in 2D on a subplot.
 
         The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
-        image
-            Whether or not to include a 2D plot (via `imshow`) of the image data.
+        data
+            Whether to include a 2D plot (via `imshow`) of the image data.
         noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the noise map.
-        inverse_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the inverse noise map.
+            Whether to include a 2D plot (via `imshow`) of the noise map.
         signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the signal-to-noise map.
-        absolute_signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the absolute signal to noise map.
-        potential_chi_squared_map
-            Whether or not to include a 2D plot (via `imshow`) of the potential chi squared map.
+            Whether to include a 2D plot (via `imshow`) of the signal-to-noise map.
         pre_cti_data
-            Whether or not to include a 2D plot (via `imshow`) of the pre-cti data.
+            Whether to include a 2D plot (via `imshow`) of the pre-cti data.
         cosmic_ray_map
-            Whether or not to include a 2D plot (via `imshow`) of the cosmic ray map.
+            Whether to include a 2D plot (via `imshow`) of the cosmic ray map.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
         self._subplot_custom_plot(
-            image=image,
+            data=data,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
-            inverse_noise_map=inverse_noise_map,
-            absolute_signal_to_noise_map=absolute_signal_to_noise_map,
-            potential_chi_squared_map=potential_chi_squared_map,
             pre_cti_data=pre_cti_data,
             cosmic_ray_map=cosmic_ray_map,
             auto_labels=AutoLabels(filename=auto_filename),
         )
 
-    def subplot_imaging_ci(self):
+    def subplot_dataset(self):
         """
         Standard subplot of the attributes of the plotter's `ImagingCI` object.
         """
         self.subplot(
-            image=True,
+            data=True,
             noise_map=True,
             signal_to_noise_map=True,
             pre_cti_data=True,
-            inverse_noise_map=True,
             cosmic_ray_map=True,
         )
 
-    def subplot_1d_of_region(self, region: str):
+    def subplot_1d(self, region: str):
         """
         Plots the individual attributes of the plotter's `ImagingCI` object in 1D on a subplot.
 
         These 1D plots correspond to a region in 2D on the charge injection image, which is binned up over the parallel
         or serial direction to produce a 1D plot. For example, for the input `region=parallel_fpr`, this
         function extracts the FPR over each charge injection region and bins such that the 1D plot shows the FPR
         in the parallel direction.
@@ -328,16 +338,16 @@
         region
             The region on the charge injection image where data is extracted and binned over the parallel or serial
             direction {"parallel_fpr", "parallel_eper", "serial_fpr", "serial_eper"}
         """
 
         self.open_subplot_figure(number_subplots=4)
 
-        self.figures_1d_of_region(image=True, region=region)
-        self.figures_1d_of_region(noise_map=True, region=region)
-        self.figures_1d_of_region(pre_cti_data=True, region=region)
-        self.figures_1d_of_region(signal_to_noise_map=True, region=region)
+        self.figures_1d(data=True, region=region)
+        self.figures_1d(noise_map=True, region=region)
+        self.figures_1d(pre_cti_data=True, region=region)
+        self.figures_1d(signal_to_noise_map=True, region=region)
 
         self.mat_plot_1d.output.subplot_to_figure(
             auto_filename=f"subplot_1d_ci_{region}"
         )
         self.close_subplot_figure()
```

### Comparing `autocti-2023.1.15.1/autocti/clocker/abstract.py` & `autocti-2023.7.7.2/autocti/clocker/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/clocker/one_d.py` & `autocti-2023.7.7.2/autocti/clocker/one_d.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         express: int = 0,
         window_start: int = 0,
         window_stop: int = -1,
         time_start=0,
         time_stop=-1,
         prune_n_electrons=1e-18,
         prune_frequency=20,
+        allow_negative_pixels=1,
+        pixel_bounce=None,
         verbosity: int = 0,
     ):
         """
         Performs clocking of a 1D signal via the c++ arctic algorithm.
 
         This corresponds to a single row or column of a CCD in the parallel or serial direction. Given the notion of
         parallel and serial are not relevent in 1D, these prefixes are dropped from parameters (unlike the `Clocker2D`)
@@ -59,14 +61,17 @@
         self.window_start = window_start
         self.window_stop = window_stop
         self.time_start = time_start
         self.time_stop = time_stop
         self.prune_n_electrons = prune_n_electrons
         self.prune_frequency = prune_frequency
 
+        self.allow_negative_pixels = allow_negative_pixels
+        self.pixel_bounce = pixel_bounce
+
     def _traps_ccd_from(self, cti: CTI1D):
         """
         Unpack the `CTI1D` object to retries its traps and ccd.
         """
         if cti.trap_list is not None:
             trap_list = list(cti.trap_list)
         else:
@@ -113,14 +118,16 @@
             parallel_window_offset=data.readout_offsets[0],
             parallel_window_start=self.window_start,
             parallel_window_stop=self.window_stop,
             parallel_time_start=self.time_start,
             parallel_time_stop=self.time_stop,
             parallel_prune_n_electrons=self.prune_n_electrons,
             parallel_prune_frequency=self.prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
         return aa.Array1D.no_mask(
             values=image_post_cti.flatten(), pixel_scales=data.pixel_scales
         )
 
@@ -164,13 +171,15 @@
             parallel_window_offset=data.readout_offsets[0],
             parallel_window_start=self.window_start,
             parallel_window_stop=self.window_stop,
             parallel_time_start=self.time_start,
             parallel_time_stop=self.time_stop,
             parallel_prune_n_electrons=self.prune_n_electrons,
             parallel_prune_frequency=self.prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
         return aa.Array1D.no_mask(
             values=image_post_cti.flatten(), pixel_scales=data.pixel_scales
         )
```

### Comparing `autocti-2023.1.15.1/autocti/clocker/two_d.py` & `autocti-2023.7.7.2/autocti/clocker/two_d.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         serial_window_start: int = 0,
         serial_window_stop: int = -1,
         serial_time_start=0,
         serial_time_stop=-1,
         serial_prune_n_electrons=1e-18,
         serial_prune_frequency=0,
         serial_fast_mode: Optional[bool] = None,
+        allow_negative_pixels=1,
+        pixel_bounce=None,
         verbosity: int = 0,
         poisson_seed: int = -1,
     ):
         """
         Performs clocking of a 2D image via the c++ arctic algorithm.
 
         This corresponds to a full read out of a CCD including clocking in the parallel and / or serial direction.
@@ -88,14 +90,17 @@
         serial_window_start
             The pixel index of the input image where serial arCTIc clocking ends, for example if `window_start=20`
             any pixels after the 20th pixel are omitted and not clocked.
         serial_fast_mode
             If input, serial CTI is added via arctic efficiently by calling arctic once and mapping the 1D output over
             the full 2D image. This requires every row in the image has the same signal (such that each column gives
             an identical arctic output).
+        allow_negative_pixels
+            If True, negative electrons in a pixel are allowed and modeled via arCTIc, if Falss they are explicitly
+            not allowed.
         verbosity
             Whether to silence print statements and output from the c++ arctic call.
         poisson_seed
             A seed for the random number generator which draws the Poisson trap densities from a Poisson distribution.
         """
 
         super().__init__(iterations=iterations, verbosity=verbosity)
@@ -119,14 +124,17 @@
         self.serial_window_stop = serial_window_stop
         self.serial_time_start = serial_time_start
         self.serial_time_stop = serial_time_stop
         self.serial_prune_n_electrons = serial_prune_n_electrons
         self.serial_prune_frequency = serial_prune_frequency
         self.serial_fast_mode = serial_fast_mode
 
+        self.allow_negative_pixels = allow_negative_pixels
+        self.pixel_bounce = pixel_bounce
+
         self.poisson_seed = poisson_seed
 
     def _parallel_traps_ccd_from(self, cti: CTI2D):
         """
         Unpack the `CTI1D` object to retries its traps and ccd.
         """
         if cti.parallel_trap_list is not None:
@@ -167,25 +175,25 @@
         data
             The 1D data that is clocked via arctic and has CTI added to it.
         cti
             An object which represents the CTI properties of 2D clocking, including the trap species which capture
             and release electrons and the volume-filling behaviour of the CCD for parallel and serial clocking.
         """
 
-        data = data.native
-
         if self.parallel_poisson_traps:
             return self.add_cti_poisson_traps(data=data, cti=cti)
 
         if self.parallel_fast_mode:
             return self.add_cti_parallel_fast(data=data, cti=cti, preloads=preloads)
 
         if self.serial_fast_mode:
             return self.add_cti_serial_fast(data=data, cti=cti, preloads=preloads)
 
+        data = data.native_skip_mask
+
         parallel_trap_list, parallel_ccd = self._parallel_traps_ccd_from(cti=cti)
         serial_trap_list, serial_ccd = self._serial_traps_ccd_from(cti=cti)
 
         self.check_traps(trap_list_0=parallel_trap_list, trap_list_1=serial_trap_list)
         self.check_ccd(ccd_list=[parallel_ccd, serial_ccd])
 
         parallel_ccd = self.ccd_from(ccd_phase=parallel_ccd)
@@ -218,19 +226,23 @@
             serial_window_offset=serial_window_offset,
             serial_window_start=self.serial_window_start,
             serial_window_stop=self.serial_window_stop,
             serial_time_start=self.serial_time_start,
             serial_time_stop=self.serial_time_stop,
             serial_prune_n_electrons=self.serial_prune_n_electrons,
             serial_prune_frequency=self.serial_prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
         try:
-            return aa.Array2D(values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True)
+            return aa.Array2D(
+                values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True
+            )
         except AttributeError:
             return image_post_cti
 
     def add_cti_poisson_traps(self, data: aa.Array2D, cti: CTI2D) -> aa.Array2D:
         """
         Add CTI to a 2D dataset by passing it to the c++ arctic clocking algorithm.
 
@@ -260,24 +272,23 @@
         parallel_ccd = self.ccd_from(ccd_phase=parallel_ccd)
 
         try:
             parallel_window_offset = data.readout_offsets[0]
         except AttributeError:
             parallel_window_offset = self.parallel_window_offset
 
-        image_pre_cti = data.native
+        image_pre_cti = data.native_skip_mask
         image_post_cti = np.zeros(data.shape_native)
 
         total_rows = image_post_cti.shape[0]
         total_columns = image_post_cti.shape[1]
 
         parallel_trap_column_list = []
 
         for column in range(total_columns):
-
             parallel_trap_poisson_list = [
                 parallel_trap.poisson_density_from(
                     total_pixels=total_rows, seed=self.poisson_seed
                 )
                 for parallel_trap in parallel_trap_list
             ]
 
@@ -291,14 +302,16 @@
                 parallel_ccd=parallel_ccd,
                 parallel_roe=self.parallel_roe,
                 parallel_traps=parallel_trap_poisson_list,
                 parallel_express=self.parallel_express,
                 parallel_window_offset=parallel_window_offset,
                 parallel_window_start=self.parallel_window_start,
                 parallel_window_stop=self.parallel_window_stop,
+                allow_negative_pixels=self.allow_negative_pixels,
+                pixel_bounce=self.pixel_bounce,
                 verbosity=self.verbosity,
             )[:, 0]
 
         self.parallel_trap_column_list = parallel_trap_column_list
 
         serial_ccd = self.ccd_from(ccd_phase=serial_ccd)
 
@@ -316,31 +329,35 @@
             serial_window_offset=serial_window_offset,
             serial_window_start=self.serial_window_start,
             serial_window_stop=self.serial_window_stop,
             serial_time_start=self.serial_time_start,
             serial_time_stop=self.serial_time_stop,
             serial_prune_n_electrons=self.serial_prune_n_electrons,
             serial_prune_frequency=self.serial_prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
         try:
-            return aa.Array2D(values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True)
+            return aa.Array2D(
+                values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True
+            )
         except AttributeError:
             return image_post_cti
 
     def fast_indexes_from(self, data: aa.Array2D, for_parallel: bool):
         """
         For 2D images where the same signal is repeated over many columns (e.g. uniform charge injection imaging)
         the CTI added to each column for parallel CTI via arctic is identical. The same is true of serial CTI
         addition, where many rows of data are repeated.
 
         Therefore, this function speeds up CTI addition via arCTIc by extracting all identical columns (for parallel
         clocking) or rows (for serial clocking), adding CTI via arcitc to only these extracted stripes and copying the
-        output stripes to construct the the final post-cti image.
+        output stripes to construct the final post-cti image.
 
         This function inspects the input image and extracts the indexes of every unique stripe, alongside
         a list which maps this unique stripe to all other stripes it is identical to. These are used in the functions
         `add_cti_parallel_fast` and `add_cti_serial_fast` to create the extracted image that is passed to arctic and
         rebuild the final post CTI image.
 
         Parameters
@@ -356,44 +373,39 @@
 
         fast_index_list = []
         fast_column_lists = []
 
         unchecked_list = range(0, total_stripes)
 
         for stripe_index in range(total_stripes):
-
             paired = False
 
             pair_list = []
             unchecked_list_new = []
 
             if stripe_index in unchecked_list:
-
                 for pair_index in unchecked_list:
-
                     if for_parallel:
                         residual_map = np.abs(
                             data[:, stripe_index] - data[:, pair_index]
                         )
                     else:
                         residual_map = np.abs(
                             data[stripe_index, :] - data[pair_index, :]
                         )
 
                     if np.all(residual_map < 1.0e-8):
-
                         if not paired:
                             fast_index_list.append(stripe_index)
 
                         paired = True
 
                         pair_list.append(pair_index)
 
                     else:
-
                         unchecked_list_new.append(pair_index)
 
                 fast_column_lists.append(pair_list)
                 unchecked_list = unchecked_list_new
 
         return fast_index_list, fast_column_lists
 
@@ -406,15 +418,15 @@
         Clocking is performed towards the readout register and electronics, with parallel CTI added first followed
         by serial CTI. If both parallel and serial CTI are added, parallel CTI is added and the post-CTI image
         (therefore including trailing after parallel clocking) is used to perform serial clocking and add serial CTI.
 
         For 2D images where the same signal is repeated over many columns (e.g. uniform charge injection imaging)
         the CTI added to each column via arctic is identical. Therefore, this function speeds up CTI addition by
         extracting all identical columns, adding CTI via arcitc to only these columns and copying the output columns
-        to construct the the final post-cti image.
+        to construct the final post-cti image.
 
         Parameters
         ----------
         data
             The 1D data that is clocked via arctic and has CTI added to it.
         cti
             An object which represents the CTI properties of 2D clocking, including the trap species which capture
@@ -422,56 +434,61 @@
         perform_checks
             Check that it is value for the input data to use the fast clocking speed up (e.g. all columns are identical
             and all entries outside this region are zero).
         """
 
         parallel_trap_list, parallel_ccd = self._parallel_traps_ccd_from(cti=cti)
 
-        image_pre_cti = data.native
+        image_pre_cti = data.native_skip_mask
 
         self.check_traps(trap_list_0=parallel_trap_list)
         self.check_ccd(ccd_list=[parallel_ccd])
 
         parallel_ccd = self.ccd_from(ccd_phase=parallel_ccd)
 
         if preloads.parallel_fast_index_list is None:
             fast_index_list, fast_column_lists = self.fast_indexes_from(
                 data=image_pre_cti, for_parallel=True
             )
         else:
             fast_index_list = preloads.parallel_fast_index_list
             fast_column_lists = preloads.parallel_fast_column_lists
 
-        image_pre_cti_pass = np.zeros(shape=(data.shape[0], len(fast_index_list)))
+        image_pre_cti_pass = np.zeros(
+            shape=(data.shape_native[0], len(fast_index_list))
+        )
         for i, fast_index in enumerate(fast_index_list):
             image_pre_cti_pass[:, i] = image_pre_cti[:, fast_index]
 
         image_post_cti_pass = add_cti(
             image=image_pre_cti_pass,
             parallel_ccd=parallel_ccd,
             parallel_roe=self.parallel_roe,
             parallel_traps=parallel_trap_list,
             parallel_express=self.parallel_express,
             parallel_window_offset=self.parallel_window_offset,
             parallel_time_start=self.parallel_time_start,
             parallel_time_stop=self.parallel_time_stop,
             parallel_prune_n_electrons=self.parallel_prune_n_electrons,
             parallel_prune_frequency=self.parallel_prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
         image_post_cti = np.zeros(shape=data.shape_native)
 
         for i, fast_column_list in enumerate(fast_column_lists):
             for fast_column in fast_column_list:
-
                 image_post_cti[:, fast_column] = image_post_cti_pass[:, i]
 
         if cti.serial_trap_list is None:
-            return aa.Array2D(values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True)
+            return aa.Array2D(
+                values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True
+            )
 
         serial_trap_list, serial_ccd = self._serial_traps_ccd_from(cti=cti)
 
         self.check_traps(trap_list_0=serial_trap_list)
         self.check_ccd(ccd_list=[serial_ccd])
 
         serial_ccd = self.ccd_from(ccd_phase=serial_ccd)
@@ -483,32 +500,36 @@
             serial_traps=serial_trap_list,
             serial_express=self.serial_express,
             serial_window_offset=self.serial_window_offset,
             serial_time_start=self.serial_time_start,
             serial_time_stop=self.serial_time_stop,
             serial_prune_n_electrons=self.serial_prune_n_electrons,
             serial_prune_frequency=self.serial_prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
-        return aa.Array2D(values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True)
+        return aa.Array2D(
+            values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True
+        )
 
     def add_cti_serial_fast(
         self, data: aa.Array2D, cti: CTI2D, preloads: Preloads = Preloads()
     ):
         """
         Add CTI to a 2D dataset by passing it to the c++ arctic clocking algorithm.
 
         Clocking is performed towards the readout register and electronics, with parallel CTI added first followed
         by serial CTI. If both parallel and serial CTI are added, serial CTI is added and the post-CTI image
         (therefore including trailing after serial clocking) is used to perform serial clocking and add serial CTI.
 
         For 2D images where the same signal is repeated over all columns (e.g. uniform charge injection imaging)
         the CTI added to each row via arctic is identical. Therefore, this function speeds up CTI addition by
-        only a single column to arcitc once and copying the output column the NumPy array to construct the the final
+        only a single column to arcitc once and copying the output column the NumPy array to construct the final
         post-cti image.
 
         This only works for serial CTI when parallel CTI is omitted.
 
         By default, checks are performed which ensure that the input data fits the criteria for this speed up.
 
         Parameters
@@ -521,55 +542,60 @@
         perform_checks
             Check that it is value for the input data to use the fast clocking speed up (e.g. all columns are identical
             and all entries outside this region are zero).
         """
 
         serial_trap_list, serial_ccd = self._serial_traps_ccd_from(cti=cti)
 
-        image_pre_cti = data.native
+        image_pre_cti = data.native_skip_mask
 
         self.check_traps(trap_list_0=serial_trap_list)
         self.check_ccd(ccd_list=[serial_ccd])
 
         serial_ccd = self.ccd_from(ccd_phase=serial_ccd)
 
         if preloads.serial_fast_index_list is None:
             fast_index_list, fast_row_lists = self.fast_indexes_from(
                 data=image_pre_cti, for_parallel=False
             )
         else:
             fast_index_list = preloads.serial_fast_index_list
             fast_row_lists = preloads.serial_fast_row_lists
 
-        image_pre_cti_pass = np.zeros(shape=(len(fast_index_list), data.shape[1]))
+        image_pre_cti_pass = np.zeros(
+            shape=(len(fast_index_list), data.shape_native[1])
+        )
         for i, fast_index in enumerate(fast_index_list):
             image_pre_cti_pass[i, :] = image_pre_cti[fast_index, :]
 
         image_post_cti_pass = add_cti(
             image=image_pre_cti_pass,
             serial_ccd=serial_ccd,
             serial_roe=self.serial_roe,
             serial_traps=serial_trap_list,
             serial_express=self.serial_express,
             serial_window_offset=self.serial_window_offset,
             serial_time_start=self.serial_time_start,
             serial_time_stop=self.serial_time_stop,
             serial_prune_n_electrons=self.serial_prune_n_electrons,
             serial_prune_frequency=self.serial_prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
             verbosity=self.verbosity,
         )
 
         image_post_cti = np.zeros(shape=data.shape_native)
 
         for i, fast_row_list in enumerate(fast_row_lists):
             for fast_row in fast_row_list:
-
                 image_post_cti[fast_row, :] = image_post_cti_pass[i, :]
 
-        return aa.Array2D(values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True)
+        return aa.Array2D(
+            values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True
+        )
 
     def remove_cti(self, data: aa.Array2D, cti: CTI2D) -> aa.Array2D:
         """
         Remove CTI from a 2D dataset by passing it to the c++ arctic clocking algorithm. The removal of CTI is
         performed by adding CTI to the data to understand how electrons are moved on the CCD, and using this
         image to then move them back to their original pixel.
 
@@ -616,12 +642,18 @@
             serial_window_offset=data.readout_offsets[1],
             serial_window_start=self.serial_window_start,
             serial_window_stop=self.serial_window_stop,
             serial_time_start=self.serial_time_start,
             serial_time_stop=self.serial_time_stop,
             serial_prune_n_electrons=self.serial_prune_n_electrons,
             serial_prune_frequency=self.serial_prune_frequency,
+            allow_negative_pixels=self.allow_negative_pixels,
+            pixel_bounce=self.pixel_bounce,
         )
 
         return aa.Array2D(
-            values=image_cti_removed, mask=data.mask, header=data.header, store_native=True, skip_mask=True
+            values=image_cti_removed,
+            mask=data.mask,
+            header=data.header,
+            store_native=True,
+            skip_mask=True,
         )
```

### Comparing `autocti-2023.1.15.1/autocti/config/notation.yaml` & `autocti-2023.7.7.2/autocti/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/config/priors/ccd.yaml` & `autocti-2023.7.7.2/autocti/config/priors/ccd.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CCDPhase:
   full_well_depth:
     type: Uniform
     lower_limit: 0.0
-    upper_limit: 84700.0
+    upper_limit: 200000.0
     width_modifier:
       type: Absolute
       value: 0.2
     gaussian_limits:
       lower: 0.0
       upper: 1.0
   well_fill_power:
@@ -25,7 +25,10 @@
     upper_limit: 1.0
     width_modifier:
       type: Absolute
       value: 0.2
     gaussian_limits:
       lower: 0.0
       upper: 1.0
+  first_electron_fill:
+    type: Constant
+    value: 0.0
```

### Comparing `autocti-2023.1.15.1/autocti/config/priors/traps.yaml` & `autocti-2023.7.7.2/autocti/config/priors/traps.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/cosmics/cosmics.py` & `autocti-2023.7.7.2/autocti/cosmics/cosmics.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,14 @@
         jhi[mask] = self.shape_native[0]
         jhi = jhi.astype(np.int)
 
         offending_delta = 1.0
 
         # loop over the individual events
         for i, luminosity in enumerate(luminosities):
-
             n = 0  # count the intercepts
 
             u = []
             x = []
             y = []
 
             # Compute X intercepts on the pixel grid
@@ -292,15 +291,14 @@
 
         covering = 0.0
         lengths = []
         energies = []
         total_cosmics = 0
 
         while covering < cover_fraction:
-
             # pseudo-random numbers taken from a uniform distribution between 0 and 1
             luck = np.random.rand(cr_n)
 
             # draw the length of the tracks
             ius = interp1d(self.lengths[:, 1], self.lengths[:, 0], kind="slinear")
             length = ius(luck)
 
@@ -328,10 +326,8 @@
 
             # count the covering factor
             area = np.count_nonzero(cosmic_ray_map)
             covering = 100.0 * area / (self.shape_native[1] * self.shape_native[0])
 
             total_cosmics += cr_n
 
-        return aa.Array2D.no_mask(
-            values=cosmic_ray_map, pixel_scales=self.pixel_scale
-        )
+        return aa.Array2D.no_mask(values=cosmic_ray_map, pixel_scales=self.pixel_scale)
```

### Comparing `autocti-2023.1.15.1/autocti/cosmics/cr_distances.py` & `autocti-2023.7.7.2/autocti/cosmics/cr_distances.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/cosmics/cr_lengths.py` & `autocti-2023.7.7.2/autocti/cosmics/cr_lengths.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/dataset_1d.py` & `autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/dataset_1d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,69 @@
 import numpy as np
+from typing import Optional, Dict
 
 import autoarray as aa
 
 from autocti import exc
 from autocti.dataset_1d.dataset_1d.settings import SettingsDataset1D
+from autocti.extract.settings import SettingsExtract
 from autocti.layout.one_d import Layout1D
 
 
 class Dataset1D(aa.AbstractDataset):
     def __init__(
         self,
         data: aa.Array1D,
         noise_map: aa.Array1D,
         pre_cti_data: aa.Array1D,
         layout: Layout1D,
+        fpr_value: Optional[float] = None,
         settings: SettingsDataset1D = SettingsDataset1D(),
+        settings_dict: Optional[Dict] = None,
     ):
-
         super().__init__(data=data, noise_map=noise_map, settings=settings)
 
         self.data = data
         self.noise_map = noise_map
         self.pre_cti_data = pre_cti_data
         self.layout = layout
 
-    def apply_mask(self, mask: aa.Mask1D) -> "Dataset1D":
+        if fpr_value is None:
+            fpr_value = np.round(
+                np.median(
+                    self.layout.extract.fpr.stacked_array_1d_from(
+                        array=self.data,
+                        settings=SettingsExtract(
+                            pixels_from_end=min(
+                                5, self.layout.extract.fpr.total_pixels_min
+                            )
+                        ),
+                    )
+                ),
+                2,
+            )
 
+        self.fpr_value = fpr_value
+
+        self.settings_dict = settings_dict
+
+    def apply_mask(self, mask: aa.Mask1D) -> "Dataset1D":
         data = aa.Array1D(values=self.data, mask=mask).native
-        noise_map = aa.Array1D(
-            values=self.noise_map.astype("float"), mask=mask
-        ).native
+        noise_map = aa.Array1D(values=self.noise_map.astype("float"), mask=mask).native
 
         return Dataset1D(
             data=data,
             noise_map=noise_map,
             pre_cti_data=self.pre_cti_data,
             layout=self.layout,
+            fpr_value=self.fpr_value,
+            settings_dict=self.settings_dict,
         )
 
     def apply_settings(self, settings: SettingsDataset1D) -> "Dataset1D":
-
         return self
 
     @classmethod
     def from_fits(
         cls,
         layout,
         data_path,
@@ -51,16 +71,16 @@
         data_hdu=0,
         noise_map_path=None,
         noise_map_hdu=0,
         noise_map_from_single_value=None,
         pre_cti_data_path=None,
         pre_cti_data_hdu=0,
         pre_cti_data=None,
+        settings_dict: Optional[Dict] = None,
     ):
-
         data = aa.Array1D.from_fits(
             file_path=data_path, hdu=data_hdu, pixel_scales=pixel_scales
         )
 
         if noise_map_path is not None:
             noise_map = aa.util.array_1d.numpy_array_1d_via_fits_from(
                 file_path=noise_map_path, hdu=noise_map_hdu
@@ -82,21 +102,24 @@
             )
 
         pre_cti_data = aa.Array1D.no_mask(
             values=pre_cti_data.native, pixel_scales=pixel_scales
         )
 
         return Dataset1D(
-            data=data, noise_map=noise_map, pre_cti_data=pre_cti_data, layout=layout
+            data=data,
+            noise_map=noise_map,
+            pre_cti_data=pre_cti_data,
+            layout=layout,
+            settings_dict=settings_dict,
         )
 
     def output_to_fits(
         self, data_path, noise_map_path=None, pre_cti_data_path=None, overwrite=False
     ):
-
         self.data.output_to_fits(file_path=data_path, overwrite=overwrite)
         self.noise_map.output_to_fits(file_path=noise_map_path, overwrite=overwrite)
         self.pre_cti_data.output_to_fits(
             file_path=pre_cti_data_path, overwrite=overwrite
         )
 
     @classmethod
```

### Comparing `autocti-2023.1.15.1/autocti/dataset_1d/dataset_1d/simulator.py` & `autocti-2023.7.7.2/autocti/dataset_1d/dataset_1d/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 import autoarray as aa
 
 from autoarray.dataset.imaging.simulator import SimulatorImaging
 from autoarray.dataset import preprocess
 
 from autocti.dataset_1d.dataset_1d.dataset_1d import Dataset1D
+from autocti.extract.settings import SettingsExtract
 from autocti.layout.one_d import Layout1D
 from autocti.clocker.one_d import Clocker1D
 from autocti.model.model_util import CTI1D
 
 
 class SimulatorDataset1D(SimulatorImaging):
     def __init__(
         self,
         pixel_scales: aa.type.PixelScales,
         norm: float,
         read_noise: Optional[float] = None,
         add_poisson_noise: bool = False,
+        charge_noise: Optional[float] = None,
         noise_if_add_noise_false: float = 0.1,
         noise_seed: int = -1,
     ):
         """
         A class representing a Imaging observation, using the shape of the data, the pixel scale,
         psf, exposure time, etc.
 
@@ -38,14 +40,15 @@
             add_poisson_noise=add_poisson_noise,
             noise_if_add_noise_false=noise_if_add_noise_false,
             noise_seed=noise_seed,
         )
 
         self.pixel_scales = pixel_scales
         self.norm = norm
+        self.charge_noise = charge_noise
 
     def pre_cti_data_from(
         self, layout: Layout1D, pixel_scales: aa.type.PixelScales
     ) -> aa.Array1D:
         """Use this charge injection layout_ci to generate a pre-cti charge injection image. This is performed by \
         going to its charge injection regions and adding the charge injection normalization value.
 
@@ -94,25 +97,33 @@
         return self.via_pre_cti_data_from(
             pre_cti_data=pre_cti_data.native, layout=layout, clocker=clocker, cti=cti
         )
 
     def via_pre_cti_data_from(
         self, pre_cti_data: aa.Array1D, layout: Layout1D, clocker: Clocker1D, cti: CTI1D
     ) -> Dataset1D:
+        if self.charge_noise is not None:
+            pre_cti_data = layout.extract.fpr.add_gaussian_noise_to(
+                array=pre_cti_data,
+                noise_sigma=self.charge_noise,
+                noise_seed=self.noise_seed,
+                settings=SettingsExtract(
+                    pixels_from_end=layout.extract.fpr.total_pixels_min
+                ),
+            )
 
         post_cti_data = clocker.add_cti(data=pre_cti_data.native, cti=cti)
 
         return self.via_post_cti_data_from(
             post_cti_data=post_cti_data, pre_cti_data=pre_cti_data, layout=layout
         )
 
     def via_post_cti_data_from(
         self, post_cti_data: aa.Array1D, pre_cti_data: aa.Array1D, layout: Layout1D
     ) -> Dataset1D:
-
         if self.read_noise is not None:
             data = preprocess.data_with_gaussian_noise_added(
                 data=post_cti_data, sigma=self.read_noise, seed=self.noise_seed
             )
             noise_map = (
                 self.read_noise
                 * aa.Array1D.ones(
@@ -124,17 +135,15 @@
             noise_map = aa.Array1D.full(
                 fill_value=self.noise_if_add_noise_false,
                 shape_native=layout.shape_1d,
                 pixel_scales=self.pixel_scales,
             ).native
 
         return Dataset1D(
-            data=aa.Array1D.no_mask(
-                values=data.native, pixel_scales=self.pixel_scales
-            ),
+            data=aa.Array1D.no_mask(values=data.native, pixel_scales=self.pixel_scales),
             noise_map=aa.Array1D.no_mask(
                 values=noise_map, pixel_scales=self.pixel_scales
             ),
             pre_cti_data=aa.Array1D.no_mask(
                 values=pre_cti_data.native, pixel_scales=self.pixel_scales
             ),
             layout=layout,
```

### Comparing `autocti-2023.1.15.1/autocti/dataset_1d/fit.py` & `autocti-2023.7.7.2/autocti/dataset_1d/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/dataset_1d/plot/dataset_1d_plotters.py` & `autocti-2023.7.7.2/autocti/dataset_1d/plot/dataset_1d_plotters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import numpy as np
-from typing import Callable
+from typing import Callable, Optional
 
 import autoarray.plot as aplt
 
 from autoarray.plot.auto_labels import AutoLabels
 
 from autocti.plot.abstract_plotters import Plotter
 from autocti.dataset_1d.dataset_1d.dataset_1d import Dataset1D
@@ -37,257 +36,208 @@
             Contains objects which wrap the matplotlib function calls that make 1D plots.
         visuals_1d
             Contains 1D visuals that can be overlaid on 1D plots.
         include_1d
             Specifies which attributes of the `ImagingCI` are extracted and plotted as visuals for 1D plots.
         """
         super().__init__(
-            mat_plot_1d=mat_plot_1d, include_1d=include_1d, visuals_1d=visuals_1d
+            dataset=dataset,
+            mat_plot_1d=mat_plot_1d,
+            include_1d=include_1d,
+            visuals_1d=visuals_1d,
         )
 
-        self.dataset = dataset
-
-    @property
-    def dataset_1d(self):
-        return self.dataset
-
     def get_visuals_1d(self) -> aplt.Visuals1D:
         return self.visuals_1d
 
     @property
     def extract_region_from(self) -> Callable:
         return self.dataset.layout.extract_region_from
 
     def figures_1d(
         self,
+        region: Optional[str] = None,
         data: bool = False,
+        data_logy: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         pre_cti_data: bool = False,
     ):
         """
         Plots the individual attributes of the plotter's `Dataset1D` object in 1D.
 
         The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
-        Parameters
-        ----------
-        image
-            Whether or not to make a 1D plot (via `plot`) of the data.
-        noise_map
-            Whether or not to make a 1D plot (via `plot`) of the noise map.
-        signal_to_noise_map
-            Whether or not to make a 1D plot (via `plot`) of the signal-to-noise map.
-        pre_cti_data
-            Whether or not to make a 1D plot (via `plot`) of the pre-cti data.
-        """
-
-        if data:
-
-            self.mat_plot_1d.plot_yx(
-                y=self.dataset_1d.data,
-                x=self.dataset_1d.data.grid_radial,
-                visuals_1d=self.get_visuals_1d(),
-                auto_labels=AutoLabels(title="Dataset 1D Data", filename="data"),
-            )
-
-        if noise_map:
-
-            self.mat_plot_1d.plot_yx(
-                y=self.dataset_1d.noise_map,
-                x=self.dataset_1d.noise_map.grid_radial,
-                visuals_1d=self.get_visuals_1d(),
-                auto_labels=AutoLabels(
-                    title="Dataset 1D Noise Map", filename="noise_map"
-                ),
-            )
-
-        if signal_to_noise_map:
-
-            self.mat_plot_1d.plot_yx(
-                y=self.dataset_1d.signal_to_noise_map,
-                x=self.dataset_1d.signal_to_noise_map.grid_radial,
-                visuals_1d=self.get_visuals_1d(),
-                auto_labels=AutoLabels(
-                    title="Dataset 1D Signal-To-Noise Map",
-                    filename="signal_to_noise_map",
-                ),
-            )
-
-        if pre_cti_data:
-
-            self.mat_plot_1d.plot_yx(
-                y=self.dataset_1d.pre_cti_data,
-                x=self.dataset_1d.pre_cti_data.grid_radial,
-                visuals_1d=self.get_visuals_1d(),
-                auto_labels=AutoLabels(
-                    title="Dataset 1D Pre CTI Data", filename="pre_cti_data"
-                ),
-            )
-
-    def figures_1d_of_region(
-        self,
-        region: str,
-        data: bool = False,
-        noise_map: bool = False,
-        pre_cti_data: bool = False,
-        signal_to_noise_map: bool = False,
-    ):
-        """
-        Plots the individual attributes of the plotter's `Dataset1D` object in 1D.
-
-        These 1D plots correspond to regions in 1D on the charge injection image, which are binned up to produce a
-         1D plot.
+        If a `region` string is input, the 1D plots correspond to regions in 1D on the 1D dataset, which are binned up
+        to produce a1D plot.
 
-         For example, for the input `region=fpr`, this function extracts the FPR over each charge region and bins them
+        For example, for the input `region=fpr`, this function extracts the FPR over each charge region and bins them
         such that the 1D plot shows the average FPR.
 
         The API is such that every plottable attribute of the `Dataset1D` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
         region
             The region on the 1D dataset where data is extracted and binned {fpr", "eper"}
-        image
-            Whether or not to make a 1D plot (via `plot`) of the image data extracted and binned over the region.
+        data
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars.
+        data_logy
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars and the y-axis on a log10 scale.
         noise_map
-            Whether or not to make a 1D plot (via `plot`) of the noise-map extracted and binned over the region.
+            Whether to make a 1D plot (via `plot`) of the noise-map extracted and binned over the region.
         pre_cti_data
-            Whether or not to make a 1D plot (via `plot`) of the pre-cti data extracted and binned over the region.
+            Whether to make a 1D plot (via `plot`) of the pre-cti data extracted and binned over the region.
         signal_to_noise_map
-            Whether or not to make a 1D plot (via `plot`) of the signal-to-noise map data extracted and binned over
+            Whether to make a 1D plot (via `plot`) of the signal-to-noise map data extracted and binned over
             the region.
         """
 
+        suffix = f"_{region}" if region is not None else ""
+        title_str = self.title_str_from(region=region)
+
         if data:
+            y = self.extract_region_from(array=self.dataset.data, region=region)
+            y_errors = self.extract_region_from(
+                array=self.dataset.noise_map, region=region
+            )
 
+            self.mat_plot_1d.plot_yx(
+                y=y,
+                x=range(len(y)),
+                plot_axis_type_override="errorbar",
+                y_errors=y_errors,
+                visuals_1d=self.get_visuals_1d(),
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
+                auto_labels=AutoLabels(
+                    title=f"Data 1D {title_str}",
+                    yunit="e-",
+                    filename=f"data{suffix}",
+                ),
+            )
+
+        if data_logy:
             y = self.extract_region_from(array=self.dataset.data, region=region)
+            y_errors = self.extract_region_from(
+                array=self.dataset.noise_map, region=region
+            )
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
+                plot_axis_type_override="errorbar_logy",
+                y_errors=y_errors,
                 visuals_1d=self.get_visuals_1d(),
+                text_manual_dict=self.text_manual_dict_from(region=region),
+                text_manual_dict_y=self.text_manual_dict_y_from(region=region),
                 auto_labels=AutoLabels(
-                    title=f"Image {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"data_{region}",
+                    title=f"Data 1D {title_str} [log10]",
+                    yunit="e-",
+                    filename=f"data_logy{suffix}",
                 ),
             )
 
         if noise_map:
             y = self.extract_region_from(array=self.dataset.noise_map, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title=f"Noise Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"noise_map_{region}",
+                    title=f"Noise Map {title_str}",
+                    yunit="e-",
+                    filename=f"noise_map{suffix}",
                 ),
             )
 
         if pre_cti_data:
             y = self.extract_region_from(array=self.dataset.pre_cti_data, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title=f"CI Pre CTI {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"pre_cti_data_{region}",
+                    title=f"CI Pre CTI {title_str}",
+                    yunit="e-",
+                    filename=f"pre_cti_data{suffix}",
                 ),
             )
 
         if signal_to_noise_map:
             y = self.extract_region_from(
                 array=self.dataset.signal_to_noise_map, region=region
             )
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title=f"Signal To Noise Map {region}",
-                    ylabel="Image",
-                    xlabel="Pixel No.",
-                    filename=f"signal_to_noise_map_{region}",
+                    title=f"Signal To Noise Map {title_str}",
+                    yunit="",
+                    filename=f"signal_to_noise_map{suffix}",
                 ),
             )
 
     def subplot(
         self,
-        data=False,
+        data: bool = False,
+        data_logy: bool = False,
         noise_map=False,
         signal_to_noise_map=False,
         pre_cti_data=False,
-        auto_filename="subplot_dataset_1d",
+        auto_filename="subplot_dataset",
+        **kwargs,
     ):
         """
         Plots the individual attributes of the plotter's `Dataset1D` object in 1D on a subplot.
 
         The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
-        image
-            Whether or not to include a 1D plot (via `plot`) of the data.
+        data
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars.
+        data_logy
+            Whether to make a 1D plot (via `plot`) of the image data extracted and binned over the region, with the
+            noise-map values included as error bars and the y-axis on a log10 scale.
         noise_map
-            Whether or not to include a 1D plot (via `plot`) of the noise map.
+            Whether to include a 1D plot (via `plot`) of the noise map.
         signal_to_noise_map
-            Whether or not to include a 1D plot (via `plot`) of the signal-to-noise map.
+            Whether to include a 1D plot (via `plot`) of the signal-to-noise map.
         pre_cti_data
-            Whether or not to include a 1D plot (via `plot`) of the pre-cti data.
+            Whether to include a 1D plot (via `plot`) of the pre-cti data.
         """
+
+        region = kwargs.get("region", None)
+        suffix = f"_{region}" if region is not None else ""
+
         self._subplot_custom_plot(
             data=data,
+            data_logy=data_logy,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
             pre_cti_data=pre_cti_data,
-            auto_labels=AutoLabels(filename=auto_filename),
+            auto_labels=AutoLabels(filename=f"{auto_filename}{suffix}"),
+            **kwargs,
         )
 
-    def subplot_dataset_1d(self):
+    def subplot_dataset(self, region: Optional[str] = None):
         """
         Standard subplot of the attributes of the plotter's `Dataset1D` object.
         """
         self.subplot(
-            data=True, noise_map=True, signal_to_noise_map=True, pre_cti_data=True
+            region=region,
+            data=True,
+            noise_map=True,
+            signal_to_noise_map=True,
+            pre_cti_data=True,
         )
-
-    def subplot_1d_of_region(self, region: str):
-        """
-        Plots the individual attributes of the plotter's `Dataset1D` object in 1D on a subplot.
-
-        These 1D plots correspond to a region in 1D on the dataset, which is binned up to produce a 1D plot.
-
-        For example, for the input `region=fpr`, this function extracts the FPR over each charge region and bins such
-        that the 1D plot shows the average FPR.
-
-        The function plots the data, noise map, pre-cti data and signal to noise map in 1D on the subplot.
-
-        Parameters
-        ----------
-        region
-            The region on the charge injection image where data is extracted and binned over the parallel or serial
-            direction {"parallel_fpr", "parallel_eper", "serial_fpr", "serial_eper"}
-        """
-
-        self.open_subplot_figure(number_subplots=4)
-
-        self.figures_1d_of_region(data=True, region=region)
-        self.figures_1d_of_region(noise_map=True, region=region)
-        self.figures_1d_of_region(pre_cti_data=True, region=region)
-        self.figures_1d_of_region(signal_to_noise_map=True, region=region)
-
-        self.mat_plot_1d.output.subplot_to_figure(auto_filename=f"subplot_1d_{region}")
-        self.close_subplot_figure()
```

### Comparing `autocti-2023.1.15.1/autocti/extract/one_d/abstract.py` & `autocti-2023.7.7.2/autocti/extract/one_d/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import copy
 import numpy as np
 from typing import List, Optional, Tuple
 
 import autoarray as aa
 
+from autocti.extract.settings import SettingsExtract
+
 
 class Extract1D:
     def __init__(
         self,
+        shape_1d: Optional[Tuple[int]] = None,
         region_list: Optional[aa.type.Region1DList] = None,
         prescan: Optional[aa.type.Region1DLike] = None,
         overscan: Optional[aa.type.Region1DLike] = None,
     ):
         """
         Abstract class containing methods for extracting regions from a 1D line dataset which contains some sort of
         original signal whose profile before CTI is known (e.g. warm pixel, charge injection).
@@ -18,14 +22,17 @@
         This uses the `region_list`, which contains the signal's regions in pixel coordinates (x0, x1).
 
         Parameters
         ----------
         region_list
             Integer pixel coordinates specifying the corners of signal (x0, x1).
         """
+
+        self.shape_1d = shape_1d
+
         self.region_list = (
             list(map(aa.Region1D, region_list)) if region_list is not None else None
         )
 
         if isinstance(prescan, tuple):
             prescan = aa.Region1D(region=prescan)
 
@@ -38,52 +45,64 @@
     @property
     def total_pixels_min(self) -> int:
         """
         The number of rows between the read-out electronics and the signal closest to them.
         """
         return np.min([region.total_pixels for region in self.region_list])
 
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    @property
+    def parallel_rows_between_regions(self):
+        return [
+            self.region_list[i + 1].x0 - self.region_list[i].x1
+            for i in range(len(self.region_list) - 1)
+        ]
+
+    @property
+    def trail_size_to_array_edge(self):
+        return self.shape_1d[0] - np.max([region.x1 for region in self.region_list])
+
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         raise NotImplementedError
 
     def array_1d_list_from(
-        self, array: aa.Array1D, pixels: Tuple[int, int]
+        self, array: aa.Array1D, settings: SettingsExtract
     ) -> List[aa.Array1D]:
         """
         Extract a specific region from every region on the line dataset and return as a list of 1D arrays.
 
         For example, this might extract the EPERs trailing every signal.
 
-        The `region_1d_list_from()` of each `Extract1D` class describes the exact extraction performed for each
+        The `region_list_from()` of each `Extract1D` class describes the exact extraction performed for each
         extract when this function is called.
 
         Parameters
         ----------
         array
             The array from which the regions are extracted and put into the returned list of rrays.
         pixels
             The integer range of pixels between which the extraction is performed.
         """
 
         arr_list = [
             array.native[region.slice]
-            for region in self.region_list_from(pixels=pixels)
+            for region in self.region_list_from(settings=settings)
         ]
 
         mask_1d_list = [
-            array.mask[region.slice] for region in self.region_list_from(pixels=pixels)
+            array.mask[region.slice]
+            for region in self.region_list_from(settings=settings)
         ]
 
         return [
             aa.Array1D(values=arr, mask=mask_1d).native
             for arr, mask_1d in zip(arr_list, mask_1d_list)
         ]
 
     def stacked_array_1d_from(
-        self, array: aa.Array1D, pixels: Tuple[int, int]
+        self, array: aa.Array1D, settings: SettingsExtract
     ) -> aa.Array1D:
         """
         Extract a region (e.g. the FPR) of every region on the line dataset and stack them by taking their mean.
 
         This returns the 1D average of the extracted regions (e.g. the FPRs) of all of the regions, which for certain
         calibration datasets one may expect to be similar.
 
@@ -98,45 +117,87 @@
         pixels
             The pixel index to extract the region between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd
             FPR rows)
         """
 
         arr_list = [
             np.ma.array(data=array.native[region.slice], mask=array.mask[region.slice])
-            for region in self.region_list_from(pixels=pixels)
+            for region in self.region_list_from(settings=settings)
         ]
 
         stacked_array_1d = np.ma.mean(np.ma.asarray(arr_list), axis=0)
 
         mask_1d_list = [
-            array.mask[region.slice] for region in self.region_list_from(pixels=pixels)
+            array.mask[region.slice]
+            for region in self.region_list_from(settings=settings)
         ]
 
         return aa.Array1D(
             values=np.asarray(stacked_array_1d.data),
             mask=sum(mask_1d_list) == len(mask_1d_list),
         ).native
 
     def add_to_array(
-        self, new_array: aa.Array1D, array: aa.Array1D, pixels: Tuple[int, int]
+        self, new_array: aa.Array1D, array: aa.Array1D, settings: SettingsExtract
     ) -> aa.Array1D:
         """
         Extracts the region (e.g. the FPRs) from the line dataset and adds them to a line dataset.
 
         Parameters
         ----------
         new_array
             The 1D array which the extracted region (e.g. the FPRs) are added to.
         array
             The 1D array which contains the 1D line dataset from which the region (e.g. the FPRs) are extracted.
         pixels
             The row pixel index which determines the region extracted (e.g. `pixels=(0, 3)` will compute the region
             corresponding to the 1st, 2nd and 3rd pixels).
         """
-        region_list = self.region_list_from(pixels=pixels)
+        region_list = self.region_list_from(settings=settings)
 
-        array_1d_list = self.array_1d_list_from(array=array, pixels=pixels)
+        array_1d_list = self.array_1d_list_from(array=array, settings=settings)
 
         for arr, region in zip(array_1d_list, region_list):
             new_array[region.x0 : region.x1] += arr
 
         return new_array
+
+    def add_gaussian_noise_to(
+        self,
+        array: aa.Array1D,
+        settings: SettingsExtract,
+        noise_sigma: float,
+        noise_seed: int = -1,
+    ) -> aa.Array2D:
+        """
+        Adds Gaussian noise of an input sigma value to the regions of the `Extract` object and returns the overall
+        input array with this noise added.
+
+        Parameters
+        ----------
+        array
+            The 1D array which contains the charge injection where regions of Gaussian noise is added.
+        noise_sigma
+            The sigma value (standard deviation) of the Gaussian from which noise values are drann.
+        noise_seed
+            The seed of the random number generator, used for the random noises maps.
+        pixels
+            The row pixel index which determines the region of the FPR (e.g. `pixels=(0, 3)` will compute the region
+            corresponding to the 1st, 2nd and 3rd FPR rows).
+        pixels_from_end
+            Alternative row pixex index specification, which extracts this number of pixels from the end of
+            each region (e.g. FPR / EPER). For example, if each FPR is 100 pixels and `pixels_from_end=10`, the
+            last 10 pixels of each FPR (pixels (90, 100)) are extracted.
+        """
+
+        region_list = self.region_list_from(settings=settings)
+
+        array_1d_list = self.array_1d_list_from(array=array, settings=settings)
+
+        array = copy.copy(array.native)
+
+        for arr, region in zip(array_1d_list, region_list):
+            array[region.x0 : region.x1] = aa.preprocess.data_with_gaussian_noise_added(
+                data=arr, sigma=noise_sigma, seed=noise_seed
+            )
+
+        return array
```

### Comparing `autocti-2023.1.15.1/autocti/extract/one_d/eper.py` & `autocti-2023.7.7.2/autocti/extract/one_d/eper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 import numpy as np
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.one_d.abstract import Extract1D
+from autocti.extract.settings import SettingsExtract
 
 
 class Extract1DEPER(Extract1D):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region1D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region1D]:
         """
         Returns a list of the (x0, x1) regions containing the EPERs of a 1D CTI dataset.
 
         These are used for extracting the EPER regions of 1D data.
 
-        Negative pixel values are supported to the `pixels` tuple, whereby pixels in front of the EPERs (e.g.
-        the FPR) are also extracted.
+        Negative pixel values can be input into the `pixels` tuple, whereby pixels in front of the EPERs (e.g.
+        the FPR) are extracted.
 
         Parameters
-    ----------
+        ----------
         pixels
             The row indexes to extract the trails between (e.g. pixels(0, 3) extracts the 1st, 2nd and 3rd pixels)
         """
 
-        return list(
-            map(
-                lambda region: region.trailing_region_from(pixels=pixels),
-                self.region_list,
-            )
-        )
+        pixels = settings.pixels
+
+        region_list = []
+
+        for i, region in enumerate(self.region_list):
+            if settings.pixels_from_end is not None:
+                parallel_row_spaces = self.parallel_rows_between_regions + [
+                    self.trail_size_to_array_edge
+                ]
+
+                pixels = (
+                    parallel_row_spaces[i] - settings.pixels_from_end,
+                    parallel_row_spaces[i],
+                )
+
+            region_list.append(region.trailing_region_from(pixels=pixels))
+
+        return region_list
 
     def array_1d_from(self, array: aa.Array1D) -> aa.Array1D:
         """
         Extract all of the data values in an input `array1D` that do not overlap the charge regions or the
         prescan / overscan regions.
 
         This  extracts a `array1D` that contains only regions of the data where there are parallel trails (e.g. those
```

### Comparing `autocti-2023.1.15.1/autocti/extract/one_d/fpr.py` & `autocti-2023.7.7.2/autocti/extract/one_d/fpr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.one_d.abstract import Extract1D
+from autocti.extract.settings import SettingsExtract
 
 
 class Extract1DFPR(Extract1D):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region1D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region1D]:
         """
         Returns a list of the (x0, x1) regions containing the FPRs of a 1D CTI dataset.
 
         These are used for extracting the FPR regions of 1D data.
 
-        Negative pixel values are supported to the `pixels` tuple, whereby pixels in front of the FPRs  are also
+        Negative pixel values can be input into the `pixels` tuple, whereby pixels in front of the FPRs  are also
         extracted.
 
         Parameters
-    ----------
+        ----------
         pixels
             The row indexes to extract the front edge between (e.g. pixels(0, 3) extracts the 1st, 2nd and 3rd pixels)
         """
         return list(
             map(
-                lambda region: region.front_region_from(pixels=pixels), self.region_list
+                lambda region: region.front_region_from(
+                    pixels=settings.pixels, pixels_from_end=settings.pixels_from_end
+                ),
+                self.region_list,
             )
         )
```

### Comparing `autocti-2023.1.15.1/autocti/extract/one_d/master.py` & `autocti-2023.7.7.2/autocti/extract/one_d/master.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from typing import Tuple
+from typing import Optional, Tuple
 
 from autocti.extract.one_d.overscan import Extract1DOverscan
 from autocti.extract.one_d.fpr import Extract1DFPR
 from autocti.extract.one_d.eper import Extract1DEPER
+from autocti.extract.settings import SettingsExtract
 
 import autoarray as aa
 
 
 class Extract1DMaster:
     def __init__(
         self,
         region_list,
-        prescan: aa.type.Region1DLike = None,
-        overscan: aa.type.Region1DLike = None,
+        shape_1d: Optional[Tuple[int]] = None,
+        prescan: Optional[aa.type.Region1DLike] = None,
+        overscan: Optional[aa.type.Region1DLike] = None,
     ):
         """
         Abstract class containing methods for extracting regions from a 1D line dataset which contains some sort of
         original signal whose profile before CTI is known (e.g. warm pixel, charge injection).
 
         This uses the `region_list`, which contains the signal's regions in pixel coordinates (x0, x1).
 
@@ -30,27 +32,35 @@
             Integer pixel coordinates specifying the corners of the overscan (x0, x1).
         """
 
         self.region_list = (
             list(map(aa.Region1D, region_list)) if region_list is not None else None
         )
 
+        self.shape_1d = shape_1d
+
         self._prescan = prescan
         self._overscan = overscan
 
     @property
     def fpr(self):
         return Extract1DFPR(
-            region_list=self.region_list, prescan=self._prescan, overscan=self._overscan
+            shape_1d=self.shape_1d,
+            region_list=self.region_list,
+            prescan=self._prescan,
+            overscan=self._overscan,
         )
 
     @property
     def eper(self):
         return Extract1DEPER(
-            region_list=self.region_list, prescan=self._prescan, overscan=self._overscan
+            shape_1d=self.shape_1d,
+            region_list=self.region_list,
+            prescan=self._prescan,
+            overscan=self._overscan,
         )
 
     @property
     def overscan(self):
         return Extract1DOverscan(overscan=self._overscan)
 
     def regions_array_1d_from(self, array: aa.Array1D) -> aa.Array1D:
@@ -100,15 +110,14 @@
                <---------S----------
 
         """
 
         array_1d_of_regions = array.native.copy() * 0.0
 
         for region in self.region_list:
-
             array_1d_of_regions[region.slice] += array.native[region.slice]
 
         return array_1d_of_regions
 
     def non_regions_array_1d_from(self, array: aa.Array1D) -> aa.Array1D:
         """
         Extract all of the data values in an input `array1D` that do not overlap the charge injection regions. This
@@ -168,81 +177,83 @@
     def array_1d_of_edges_and_eper_from(
         self,
         array: aa.Array1D,
         fpr_pixels: Tuple[int, int] = None,
         eper_pixels: Tuple[int, int] = None,
     ) -> aa.Array1D:
         """
-        Extract all of the data values in an input `array1D` corresponding to the parallel front edges and trails of
-        each the charge-injection region.
-
-        One can specify the range of rows that are extracted, for example:
-
-        fpr_pixels = (0, 1) will extract just the first leading front edge row.
-        fpr_pixels = (0, 2) will extract the leading two front edge rows.
-        trails_pixels = (0, 1) will extract the first row of trails closest to the charge injection region.
-
-        The diagram below illustrates the arrays that are extracted from the input array for `fpr_pixels=(0,1)`
-        and `trails_pixels=(0,1)`:
-
-        ---KEY---
-        ---------
-
-        [] = read-out electronics   [==========] = read-out register
-
-        [xxxxxxxxxx]                [..........] = serial prescan       [ssssssssss] = serial overscan
-        [xxxxxxxxxx] = CCDPhase panel    [pppppppppp] = parallel overscan    [cccccccccc] = charge injection region
-        [xxxxxxxxxx]                [tttttttttt] = parallel / serial charge injection region trail
-
-        P = Parallel Direction      S = Serial Direction
-
-               [tptpptptptpptpptpptpt]
-               [tptptptpptpttptptptpt]
-          [...][ttttttttttttttttttttt][sss]
-          [...][ccccccccccccccccccccc][sss]
-        | [...][ccccccccccccccccccccc][sss]    |
-        | [...][ttttttttttttttttttttt][sss]    | Direction
-        P [...][ttttttttttttttttttttt][sss]    | of
-        | [...][ccccccccccccccccccccc][sss]    | clocking
-          [...][ccccccccccccccccccccc][sss]    |
+            Extract all of the data values in an input `array1D` corresponding to the parallel front edges and trails of
+            each the charge-injection region.
 
-        []     [=====================]
-               <---------S----------
+            One can specify the range of rows that are extracted, for example:
 
-        The extracted array keeps just the leading edges and trails following all charge injection scans and
-        replaces all other values with 0s:
-
-               [000000000000000000000]
-               [000000000000000000000]
-          [000][ttttttttttttttttttttt][000]
-          [000][000000000000000000000][000]
-        | [000][ccccccccccccccccccccc][000]    |
-        | [000][000000000000000000000][000]    | Direction
-        P [000][ttttttttttttttttttttt][000]    | of
-        | [000][000000000000000000000][000]    | clocking
-          [000][ccccccccccccccccccccc][000]    |
+            fpr_pixels = (0, 1) will extract just the first leading front edge row.
+            fpr_pixels = (0, 2) will extract the leading two front edge rows.
+            trails_pixels = (0, 1) will extract the first row of trails closest to the charge injection region.
+
+            The diagram below illustrates the arrays that are extracted from the input array for `fpr_pixels=(0,1)`
+            and `trails_pixels=(0,1)`:
+
+            ---KEY---
+            ---------
+
+            [] = read-out electronics   [==========] = read-out register
+
+            [xxxxxxxxxx]                [..........] = serial prescan       [ssssssssss] = serial overscan
+            [xxxxxxxxxx] = CCDPhase panel    [pppppppppp] = parallel overscan    [cccccccccc] = charge injection region
+            [xxxxxxxxxx]                [tttttttttt] = parallel / serial charge injection region trail
+
+            P = Parallel Direction      S = Serial Direction
+
+                   [tptpptptptpptpptpptpt]
+                   [tptptptpptpttptptptpt]
+              [...][ttttttttttttttttttttt][sss]
+              [...][ccccccccccccccccccccc][sss]
+            | [...][ccccccccccccccccccccc][sss]    |
+            | [...][ttttttttttttttttttttt][sss]    | Direction
+            P [...][ttttttttttttttttttttt][sss]    | of
+            | [...][ccccccccccccccccccccc][sss]    | clocking
+              [...][ccccccccccccccccccccc][sss]    |
+
+            []     [=====================]
+                   <---------S----------
+
+            The extracted array keeps just the leading edges and trails following all charge injection scans and
+            replaces all other values with 0s:
+
+                   [000000000000000000000]
+                   [000000000000000000000]
+              [000][ttttttttttttttttttttt][000]
+              [000][000000000000000000000][000]
+            | [000][ccccccccccccccccccccc][000]    |
+            | [000][000000000000000000000][000]    | Direction
+            P [000][ttttttttttttttttttttt][000]    | of
+            | [000][000000000000000000000][000]    | clocking
+              [000][ccccccccccccccccccccc][000]    |
 
-        []     [=====================]
-               <---------S----------
+            []     [=====================]
+                   <---------S----------
 
-        Parameters
-    ----------
-        fpr_pixels
-            The row indexes to extract the front edge between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows).
-        trails_pixels
-            The row indexes to extract the trails between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows)
+            Parameters
+        ----------
+            fpr_pixels
+                The row indexes to extract the front edge between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows).
+            trails_pixels
+                The row indexes to extract the trails between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows)
         """
         array_1d_of_edges_and_eper = array.native.copy() * 0.0
 
         if fpr_pixels is not None:
-
             array_1d_of_edges_and_eper = self.fpr.add_to_array(
-                new_array=array_1d_of_edges_and_eper, array=array, pixels=fpr_pixels
+                new_array=array_1d_of_edges_and_eper,
+                array=array,
+                settings=SettingsExtract(pixels=fpr_pixels),
             )
 
         if eper_pixels is not None:
-
             array_1d_of_edges_and_eper = self.eper.add_to_array(
-                new_array=array_1d_of_edges_and_eper, array=array, pixels=eper_pixels
+                new_array=array_1d_of_edges_and_eper,
+                array=array,
+                settings=SettingsExtract(pixels=eper_pixels),
             )
 
         return array_1d_of_edges_and_eper
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/abstract.py` & `autocti-2023.7.7.2/autocti/extract/two_d/abstract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
 from typing import Optional, List, Tuple, Union
 
 import autoarray as aa
 
 from autocti.charge_injection.imaging.imaging import ImagingCI
 from autocti.dataset_1d.dataset_1d.dataset_1d import Dataset1D
+from autocti.extract.settings import SettingsExtract
 from autocti.layout.one_d import Layout1D
 
 
 class Extract2D:
     def __init__(
         self,
+        shape_2d: Optional[Tuple[int, int]] = None,
         region_list: Optional[aa.type.Region2DList] = None,
         parallel_overscan: Optional[aa.type.Region2DLike] = None,
         serial_prescan: Optional[aa.type.Region2DLike] = None,
         serial_overscan: Optional[aa.type.Region2DLike] = None,
     ):
         """
         Abstract class containing methods for extracting regions from a 2D charge injection image.
@@ -24,14 +26,16 @@
         Parameters
         ----------
         region_list
             Integer pixel coordinates specifying the corners of each charge injection region (top-row, bottom-row,
             left-column, right-column).
         """
 
+        self.shape_2d = shape_2d
+
         self.region_list = (
             list(map(aa.Region2D, region_list)) if region_list is not None else None
         )
 
         self.parallel_overscan = (
             aa.Region2D(region=parallel_overscan)
             if isinstance(parallel_overscan, tuple)
@@ -45,14 +49,28 @@
         self.serial_overscan = (
             aa.Region2D(region=serial_overscan)
             if isinstance(serial_overscan, tuple)
             else serial_overscan
         )
 
     @property
+    def pedestal(self) -> aa.Region2D:
+        """
+        The region of the charge injection image containing the pedestal.
+        """
+        return aa.Region2D(
+            region=(
+                self.parallel_overscan.y0,
+                self.shape_2d[0],
+                self.serial_overscan.x0,
+                self.shape_2d[1],
+            )
+        )
+
+    @property
     def total_rows_min(self) -> int:
         """
         The number of rows between the read-out electronics and the charge injection region closest to them.
         """
         return np.min([region.total_rows for region in self.region_list])
 
     @property
@@ -67,247 +85,315 @@
         """
         The axis over which binning is performed to turn a 2D FPR into a 1D FPR.
 
         For a parallel extract `axis=1` such that binning is performed over the rows containing the FPR.
         """
         raise NotImplementedError
 
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    @property
+    def parallel_rows_between_regions(self) -> List[int]:
+        """
+        Returns a list where each entry is the number of pixels a charge injection region and its neighboring
+        charge injection region.
+        """
+        return [
+            self.region_list[i + 1].y0 - self.region_list[i].y1
+            for i in range(len(self.region_list) - 1)
+        ]
+
+    @property
+    def parallel_rows_to_array_edge(self) -> int:
+        """
+        The number of pixels from the edge of the parallel EPERs to the edge of the array.
+
+        This is the number of pixels from the last charge injection FPR edge to the read out register and electronics
+        and will include the parallel overscan if the CCD has one.
+        """
+        return self.shape_2d[0] - np.max([region.y1 for region in self.region_list])
+
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         raise NotImplementedError
 
     def array_2d_list_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> List[aa.Array2D]:
         """
         Extract a specific region from every signal region (e.g. the charge injection region of charge injection data)
         on the CTI calibration data and return as a list of 2D arrays.
 
         For example, this might extract the parallel EPERs of every charge injection region.
 
-        The `region_2d_list_from()` of each `Extract2D` class describes the exact extraction performed for each
+        The `region_list_from()` of each `Extract2D` class describes the exact extraction performed for each
         extract when this function is called.
 
         Parameters
         ----------
         array
             The array from which the regions are extracted and put into the returned list of arrays.
-        pixels
-            The integer range of pixels between which the extraction is performed.
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
-        arr_list = [
-            array.native[region.slice]
-            for region in self.region_list_from(pixels=pixels)
-        ]
+        region_list = self.region_list_from(settings=settings)
+        region_list = settings.region_list_from(region_list=region_list)
 
-        mask_2d_list = [
-            array.mask[region.slice] for region in self.region_list_from(pixels=pixels)
-        ]
+        arr_list = [array.native[region.slice] for region in region_list]
+        mask_2d_list = [array.mask[region.slice] for region in region_list]
 
         return [
             aa.Array2D(values=arr, mask=mask_2d).native
             for arr, mask_2d in zip(arr_list, mask_2d_list)
         ]
 
     def stacked_array_2d_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> np.ndarray:
         """
         Extract a region (e.g. the parallel FPR) of every signal region (e.g. the charge injection region of charge
         injection data) on the CTI calibration data and stack them by taking their mean.
 
         This returns the 2D average of the extracted regions (e.g. the parallel FPRs) of all of the charge injection
         regions, which for certain CCD charge injection electronics one may expect to be similar.
 
         For fits to charge injection data this function is also used to create images like the stacked 2D residuals,
         which therefore quantify the goodness-of-fit of a CTI model.
 
         Parameters
-    ----------
+        ----------
         array
             The 2D array which contains the charge injection image from which the regions (e.g. the parallel FPRs)
             are extracted and stacked.
-        pixels
-            The row pixel index to extract the FPR between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd
-            FPR rows)
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
 
         arr_list = [
             np.ma.array(data=array.native[region.slice], mask=array.mask[region.slice])
-            for region in self.region_list_from(pixels=pixels)
+            for region in self.region_list_from(settings=settings)
         ]
 
         stacked_array_2d = np.ma.mean(np.ma.asarray(arr_list), axis=0)
 
         mask_2d_list = [
-            array.mask[region.slice] for region in self.region_list_from(pixels=pixels)
+            array.mask[region.slice]
+            for region in self.region_list_from(settings=settings)
         ]
 
         return aa.Array2D(
             values=np.asarray(stacked_array_2d.data),
             mask=sum(mask_2d_list) == len(mask_2d_list),
         ).native
 
     def stacked_array_2d_total_pixels_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> np.ndarray:
         """
         The function `stacked_array_2d_from` extracts a region (e.g. the parallel FPR) of every charge injection
         region on the charge injection image and stacks them by taking their mean.
 
         If the data being stacked is a noise-map, we need to know how many pixels were used in the stacking of every
         final pixel on the stacked 2d array in order to compute the new noise map via quadrature.
 
         Parameters
-    ----------
+        ----------
         array
             The 2D array which contains the charge injection image from which the regions (e.g. the parallel FPRs)
             are extracted and stacked.
-        pixels
-            The row pixel index to extract the FPR between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd
-            FPR rows)
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
 
         mask_2d_list = [
-            array.mask[region.slice] for region in self.region_list_from(pixels=pixels)
+            array.mask[region.slice]
+            for region in self.region_list_from(settings=settings)
         ]
 
         arr_total_pixels = sum([np.invert(mask_2d) for mask_2d in mask_2d_list])
 
         return aa.Array2D(
             values=np.asarray(arr_total_pixels),
             mask=sum(mask_2d_list) == len(mask_2d_list),
         ).native
 
     def binned_array_1d_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> aa.Array1D:
         """
-        Extract a region (e.g. the parallel FPR) of every signal region (e.g. the charge injection region of charge injection data) on the CTI calibration data, stack
-        them by taking their mean and then bin them up to a 1D region (e.g. the 1D parallel FPR) by taking the mean
-        across the direction opposite to clocking (e.g. bin over the serial direction for a parallel FPR).
+        Extract a region (e.g. the parallel FPR) of every signal region (e.g. the charge injection region of
+        charge injection data) on the CTI calibration data, stack them by taking their mean and then bin them up to
+        a 1D region (e.g. the 1D parallel FPR) by taking the mean across the direction opposite to
+        clocking (e.g. bin over the serial direction for a parallel FPR).
 
         This returns the 1D average region (e.g. of the parallel FPR) of all of the charge injection regions. When
         binning a uniform charge injection this binning process removes noise to clearly reveal the FPR or EPER.
         For non-uniform injections this will provide an average FPR or EPER.
 
         For fits to charge injection data this function is also used to create images like the stacked 1D residuals,
         which therefore quantify the goodness-of-fit of a CTI model.
 
         Parameters
-    ----------
+        ----------
         array
             The 2D array which contains the charge injeciton image from which the parallel FPRs are extracted and
             stacked.
-        pixels
-            The column / row pixel index to extract the region (e.g. FPR, EPER) between (e.g. `pixels=(0, 3)` extracts
-            the 1st, 2nd and 3rd columns / rows)
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
 
+        region_list = self.region_list_from(settings=settings)
+        region_list = settings.region_list_from(region_list=region_list)
+
         arr_list = [
             np.ma.array(data=array.native[region.slice], mask=array.mask[region.slice])
-            for region in self.region_list_from(pixels=pixels)
+            for region in region_list
         ]
+
         stacked_array_2d = np.ma.mean(np.ma.asarray(arr_list), axis=0)
         binned_array_1d = np.ma.mean(
             np.ma.asarray(stacked_array_2d), axis=self.binning_axis
         )
         return aa.Array1D.no_mask(
             values=binned_array_1d, pixel_scales=array.pixel_scale
         )
 
     def binned_array_1d_total_pixels_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> aa.Array1D:
         """
         The function `binned_array_1d_from` extracts a region (e.g. the parallel FPR) of every charge injection region
         on the charge injection image, stacks them by taking their mean and then bin them up to a 1D region
         (e.g. the 1D parallel FPR) by taking the mean across the direction opposite to clocking (e.g. bin over the
         serial direction for a parallel FPR).
 
         If the data being stacked is a noise-map, we need to know how many pixels were used in the stacking of every
         final pixel on the binned 1D array in order to compute the new noise map via quadrature.
 
         Parameters
-    ----------
+        ----------
         array
             The 2D array which contains the charge injeciton image from which the parallel FPRs are extracted and
             stacked.
-        pixels
-            The column / row pixel index to extract the region (e.g. FPR, EPER) between (e.g. `pixels=(0, 3)` extracts
-            the 1st, 2nd and 3rd columns / rows)
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
 
         mask_2d_list = [
-            array.mask[region.slice] for region in self.region_list_from(pixels=pixels)
+            array.mask[region.slice]
+            for region in self.region_list_from(settings=settings)
         ]
 
         arr_total_pixels = sum([np.invert(mask_2d) for mask_2d in mask_2d_list])
 
         binned_total_pixels = np.ma.sum(
             np.ma.asarray(arr_total_pixels), axis=self.binning_axis
         )
 
         return aa.Array1D.no_mask(
             values=binned_total_pixels, pixel_scales=array.pixel_scale
         )
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
         raise NotImplementedError
 
     def add_to_array(
-        self, new_array: aa.Array2D, array: aa.Array2D, pixels: Tuple[int, int]
+        self, new_array: aa.Array2D, array: aa.Array2D, settings: SettingsExtract
     ) -> aa.Array2D:
         """
         Extracts the region (e.g. the parallel FPRs) from a charge injection image and adds them to a new image.
 
         Parameters
         ----------
         new_array
             The 2D array which the extracted parallel FPRs are added to.
         array
             The 2D array which contains the charge injection image from which the parallel FPRs are extracted.
-        pixels
-            The row pixel index which determines the region of the FPR (e.g. `pixels=(0, 3)` will compute the region
-            corresponding to the 1st, 2nd and 3rd FPR rows).
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
 
-        region_list = self.region_list_from(pixels=pixels)
+        region_list = self.region_list_from(settings=settings)
 
-        array_2d_list = self.array_2d_list_from(array=array, pixels=pixels)
+        array_2d_list = self.array_2d_list_from(array=array, settings=settings)
 
         for arr, region in zip(array_2d_list, region_list):
             new_array[region.y0 : region.y1, region.x0 : region.x1] += arr
 
         return new_array
 
     def dataset_1d_from(
-        self, dataset_2d: ImagingCI, pixels: Tuple[int, int]
+        self, dataset_2d: ImagingCI, settings: SettingsExtract
     ) -> Dataset1D:
-
-        binned_data_1d = self.binned_array_1d_from(array=dataset_2d.data, pixels=pixels)
+        binned_data_1d = self.binned_array_1d_from(
+            array=dataset_2d.data, settings=settings
+        )
 
         binned_noise_map_1d = self.binned_array_1d_from(
-            array=dataset_2d.noise_map, pixels=pixels
+            array=dataset_2d.noise_map, settings=settings
         )
 
         binned_noise_map_1d_total_pixels = self.binned_array_1d_total_pixels_from(
-            array=dataset_2d.noise_map, pixels=pixels
+            array=dataset_2d.noise_map, settings=settings
         )
 
         binned_noise_map_1d /= np.sqrt(binned_noise_map_1d_total_pixels)
 
         binned_pre_cti_data_1d = self.binned_array_1d_from(
-            array=dataset_2d.pre_cti_data, pixels=pixels
+            array=dataset_2d.pre_cti_data,
+            settings=settings,
         )
 
-        binned_region_1d = self.binned_region_1d_from(pixels=pixels)
+        binned_region_1d = self.binned_region_1d_from(settings=settings)
 
         layout_1d = Layout1D(
             shape_1d=binned_data_1d.shape_native, region_list=[binned_region_1d]
         )
 
         return Dataset1D(
             data=binned_data_1d,
             noise_map=binned_noise_map_1d,
             pre_cti_data=binned_pre_cti_data_1d,
             layout=layout_1d,
         )
+
+    def add_gaussian_noise_to(
+        self,
+        array: aa.Array2D,
+        settings: SettingsExtract,
+        noise_sigma: float,
+        noise_seed: int = -1,
+    ) -> aa.Array2D:
+        """
+        Adds Gaussian noise of an input sigma value to the regions of the `Extract` object and returns the overall
+        input array with this noise added.
+
+        Parameters
+        ----------
+        array
+            The 2D array which contains the charge injection where regions of Gaussian noise is added.
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
+        noise_sigma
+            The sigma value (standard deviation) of the Gaussian from which noise values are drann.
+        noise_seed
+            The seed of the random number generator, used for the random noises maps.
+        """
+
+        region_list = self.region_list_from(settings=settings)
+
+        array_2d_list = self.array_2d_list_from(array=array, settings=settings)
+
+        array = array.native
+
+        for arr, region in zip(array_2d_list, region_list):
+            array[
+                region.y0 : region.y1, region.x0 : region.x1
+            ] = aa.preprocess.data_with_gaussian_noise_added(
+                data=arr, sigma=noise_sigma, seed=noise_seed
+            )
+
+        return array
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/extract_2d_util.py` & `autocti-2023.7.7.2/autocti/extract/two_d/extract_2d_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     This is performed by binning up the data via the `binned_array_1d_from` function.
 
     In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
     charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
 
     The function returns the this region if the 1D dataset is extracted from the FPRs. This is the full range of
-    the `pixels` tuple, unless negative entries are included, meaning that pixels before the FPRs are also extracted.
+    the `pixels` tuple, unless negative entries are included, meaning that pixels before the FPRs are extracted.
 
     Parameters
     ----------
     pixels
         The row / column pixel index to extract the FPRs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd
         FPR rows / columns)
     """
@@ -27,15 +27,15 @@
     elif pixels[0] >= 0:
         return aa.Region1D(region=(0, pixels[1]))
     return aa.Region1D(region=(abs(pixels[0]), pixels[1] + abs(pixels[0])))
 
 
 def binned_region_1d_eper_from(pixels: Tuple[int, int]) -> aa.Region1D:
     """
-    The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
+    `Extract` objects extract arrays and other values from a 2D CTI dataset, which is used to perform
     CTI modeling in 1D.
 
     This is performed by binning up the data via the `binned_array_1d_from` function.
 
     In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
     charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/master.py` & `autocti-2023.7.7.2/autocti/extract/two_d/master.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import Optional, Tuple
 
 import autoarray as aa
 
+from autocti.extract.settings import SettingsExtract
 from autocti.extract.two_d.parallel.overscan import Extract2DParallelOverscan
 from autocti.extract.two_d.parallel.fpr import Extract2DParallelFPR
 from autocti.extract.two_d.parallel.eper import Extract2DParallelEPER
+from autocti.extract.two_d.parallel.pedestal import Extract2DParallelPedestal
 from autocti.extract.two_d.serial.overscan import Extract2DSerialOverscan
 from autocti.extract.two_d.serial.prescan import Extract2DSerialPrescan
 from autocti.extract.two_d.serial.fpr import Extract2DSerialFPR
 from autocti.extract.two_d.serial.eper import Extract2DSerialEPER
+from autocti.extract.two_d.serial.overscan_no_eper import Extract2DSerialOverscanNoEPER
 from autocti.extract.two_d.parallel.calibration import Extract2DParallelCalibration
 from autocti.extract.two_d.serial.calibration import Extract2DSerialCalibration
 
 
 class Extract2DMaster:
     def __init__(
         self,
@@ -56,47 +59,65 @@
         self._parallel_overscan = parallel_overscan
         self._serial_prescan = serial_prescan
         self._serial_overscan = serial_overscan
 
     @property
     def parallel_fpr(self):
         return Extract2DParallelFPR(
+            shape_2d=self.shape_2d,
             region_list=self.region_list,
             parallel_overscan=self._parallel_overscan,
             serial_prescan=self._serial_prescan,
             serial_overscan=self._serial_overscan,
         )
 
     @property
     def parallel_eper(self):
         return Extract2DParallelEPER(
+            shape_2d=self.shape_2d,
+            region_list=self.region_list,
+            parallel_overscan=self._parallel_overscan,
+            serial_prescan=self._serial_prescan,
+            serial_overscan=self._serial_overscan,
+        )
+
+    @property
+    def parallel_pedestal(self):
+        return Extract2DParallelPedestal(
+            shape_2d=self.shape_2d,
             region_list=self.region_list,
             parallel_overscan=self._parallel_overscan,
             serial_prescan=self._serial_prescan,
             serial_overscan=self._serial_overscan,
         )
 
     @property
+    def parallel_overscan(self):
+        return Extract2DParallelOverscan(parallel_overscan=self._parallel_overscan)
+
+    @property
     def parallel_calibration(self):
         return Extract2DParallelCalibration(
             shape_2d=self.shape_2d, region_list=self.region_list
         )
 
     @property
     def serial_fpr(self):
         return Extract2DSerialFPR(
+            shape_2d=self.shape_2d,
             region_list=self.region_list,
             parallel_overscan=self._parallel_overscan,
             serial_prescan=self._serial_prescan,
             serial_overscan=self._serial_overscan,
         )
 
     @property
     def serial_eper(self):
         return Extract2DSerialEPER(
+            shape_2d=self.shape_2d,
             region_list=self.region_list,
             parallel_overscan=self._parallel_overscan,
             serial_prescan=self._serial_prescan,
             serial_overscan=self._serial_overscan,
         )
 
     @property
@@ -105,31 +126,37 @@
             shape_2d=self.shape_2d,
             region_list=self.region_list,
             serial_prescan=self._serial_prescan,
             serial_overscan=self._serial_overscan,
         )
 
     @property
-    def parallel_overscan(self):
-        return Extract2DParallelOverscan(parallel_overscan=self._parallel_overscan)
+    def serial_prescan(self):
+        return Extract2DSerialPrescan(serial_prescan=self._serial_prescan)
 
     @property
     def serial_overscan(self):
         return Extract2DSerialOverscan(serial_overscan=self._serial_overscan)
 
     @property
-    def serial_prescan(self):
-        return Extract2DSerialPrescan(serial_prescan=self._serial_prescan)
+    def serial_overscan_no_eper(self):
+        return Extract2DSerialOverscanNoEPER(
+            shape_2d=self.shape_2d,
+            region_list=self.region_list,
+            parallel_overscan=self._parallel_overscan,
+            serial_prescan=self._serial_prescan,
+            serial_overscan=self._serial_overscan,
+        )
 
     def regions_array_2d_from(self, array: aa.Array2D) -> aa.Array2D:
         """
           Extract all of the charge-injection regions from an input `Array2D` object and returns them as a new `Array2D`
           where these extracted regions are included and all other entries are zeros.
 
-          The dimensions of the input array therefore do not change (unlike other `Layout2DCI` methods).
+          The dimensions of the input array therefore do not change (unlike other ``Extract`` methods).
 
           The diagram below illustrates the extraction:
 
           [] = read-out electronics
           [==========] = read-out register
           [..........] = serial prescan
           [pppppppppp] = parallel overscan
@@ -178,15 +205,15 @@
          Extract all of the areas of an `Array2D` that are not within any of the layout's charge-injection regions
          and return them as a new `Array2D` where these extracted regions are included and the charge injection regions
          are zeros
 
          The extracted array therefore includes all EPER trails and other regions of the image which may contain
          signal but are not in the FPR.
 
-         The dimensions of the input array therefore do not change (unlike other `Layout2DCI` methods).
+         The dimensions of the input array therefore do not change (unlike other ``Extract`` methods).
 
          The diagram below illustrates the extraction:
 
          [] = read-out electronics
          [==========] = read-out register
          [..........] = serial prescan
          [pppppppppp] = parallel overscan
@@ -233,161 +260,165 @@
     def parallel_fpr_and_eper_array_2d_from(
         self,
         array: aa.Array2D,
         fpr_pixels: Tuple[int, int] = None,
         eper_pixels: Tuple[int, int] = None,
     ) -> aa.Array2D:
         """
-        Extract all of the data values in an input `array2D` corresponding to the parallel front edges and trails of
-        each the charge-injection region.
+            Extract all of the data values in an input `array2D` corresponding to the parallel front edges and trails of
+            each the charge-injection region.
 
-        One can specify the range of rows that are extracted, for example:
+            One can specify the range of rows that are extracted, for example:
 
-        fpr_pixels = (0, 1) will extract just the first leading front edge row.
-        fpr_pixels = (0, 2) will extract the leading two front edge rows.
-        trails_pixels = (0, 1) will extract the first row of trails closest to the charge injection region.
-
-        The diagram below illustrates the arrays that are extracted from the input array for `fpr_pixels=(0,1)`
-        and `trails_pixels=(0,1)`:
-
-        The diagram below illustrates the extraction:
-
-        [] = read-out electronics
-        [==========] = read-out register
-        [..........] = serial prescan
-        [pppppppppp] = parallel overscan
-        [ssssssssss] = serial overscan
-        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-        [tttttttttt] = parallel / serial charge injection region trail
-
-               [tptpptptptpptpptpptpt]
-               [tptptptpptpttptptptpt]
-          [...][ttttttttttttttttttttt][sss]
-          [...][ccccccccccccccccccccc][sss]
-        | [...][ccccccccccccccccccccc][sss]    |
-        | [...][ttttttttttttttttttttt][sss]    | Direction
-        P [...][ttttttttttttttttttttt][sss]    | of
-        | [...][ccccccccccccccccccccc][sss]    | clocking
-          [...][ccccccccccccccccccccc][sss]    |
-
-        []     [=====================]
-               <--------Ser---------
-
-        The extracted array keeps just the leading edges and trails following all charge injection scans and
-        replaces all other values with 0s:
-
-               [000000000000000000000]
-               [000000000000000000000]
-          [000][ttttttttttttttttttttt][000]
-          [000][000000000000000000000][000]
-        | [000][ccccccccccccccccccccc][000]    |
-        | [000][000000000000000000000][000]    | Direction
-        P [000][ttttttttttttttttttttt][000]    | of
-        | [000][000000000000000000000][000]    | clocking
-          [000][ccccccccccccccccccccc][000]    |
+            fpr_pixels = (0, 1) will extract just the first leading front edge row.
+            fpr_pixels = (0, 2) will extract the leading two front edge rows.
+            trails_pixels = (0, 1) will extract the first row of trails closest to the charge injection region.
+
+            The diagram below illustrates the arrays that are extracted from the input array for `fpr_pixels=(0,1)`
+            and `trails_pixels=(0,1)`:
+
+            The diagram below illustrates the extraction:
+
+            [] = read-out electronics
+            [==========] = read-out register
+            [..........] = serial prescan
+            [pppppppppp] = parallel overscan
+            [ssssssssss] = serial overscan
+            [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+            [tttttttttt] = parallel / serial charge injection region trail
+
+                   [tptpptptptpptpptpptpt]
+                   [tptptptpptpttptptptpt]
+              [...][ttttttttttttttttttttt][sss]
+              [...][ccccccccccccccccccccc][sss]
+            | [...][ccccccccccccccccccccc][sss]    |
+            | [...][ttttttttttttttttttttt][sss]    | Direction
+            P [...][ttttttttttttttttttttt][sss]    | of
+            | [...][ccccccccccccccccccccc][sss]    | clocking
+              [...][ccccccccccccccccccccc][sss]    |
+
+            []     [=====================]
+                   <--------Ser---------
+
+            The extracted array keeps just the leading edges and trails following all charge injection scans and
+            replaces all other values with 0s:
+
+                   [000000000000000000000]
+                   [000000000000000000000]
+              [000][ttttttttttttttttttttt][000]
+              [000][000000000000000000000][000]
+            | [000][ccccccccccccccccccccc][000]    |
+            | [000][000000000000000000000][000]    | Direction
+            P [000][ttttttttttttttttttttt][000]    | of
+            | [000][000000000000000000000][000]    | clocking
+              [000][ccccccccccccccccccccc][000]    |
 
-        []     [=====================]
-               <--------Ser---------
+            []     [=====================]
+                   <--------Ser---------
 
-        Parameters
-    ----------
-        fpr_pixels
-            The row indexes to extract the front edge between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows).
-        trails_pixels
-            The row indexes to extract the trails between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows)
+            Parameters
+        ----------
+            fpr_pixels
+                The row indexes to extract the front edge between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows).
+            trails_pixels
+                The row indexes to extract the trails between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows)
         """
         new_array = array.native.copy() * 0.0
 
         if fpr_pixels is not None:
-
             new_array = self.parallel_fpr.add_to_array(
-                new_array=new_array, array=array, pixels=fpr_pixels
+                new_array=new_array,
+                array=array,
+                settings=SettingsExtract(pixels=fpr_pixels),
             )
 
         if eper_pixels is not None:
-
             new_array = self.parallel_eper.add_to_array(
-                new_array=new_array, array=array, pixels=eper_pixels
+                new_array=new_array,
+                array=array,
+                settings=SettingsExtract(pixels=eper_pixels),
             )
 
         return new_array
 
     def serial_fpr_and_eper_array_2d_from(
         self, array: aa.Array2D, fpr_pixels=None, eper_pixels=None
     ) -> aa.Array2D:
         """
-        Extract an array of all of the serial FPRs and EPERs of each the charge-injection scans from a charge
-        injection array.
+            Extract an array of all of the serial FPRs and EPERs of each the charge-injection scans from a charge
+            injection array.
 
-        One can specify the range of columns that are extracted, for example:
+            One can specify the range of columns that are extracted, for example:
 
-        fpr_pixels = (0, 1) will extract just the leading front edge column.
-        fpr_pixels = (0, 2) will extract the leading two front edge columns.
-        trails_pixels = (0, 1) will extract the first column of trails closest to the charge injection region.
-
-        The diagram below illustrates the arrays that is extracted from a array for `fpr_pixels=(0,2)` and
-        `trails_pixels=(0,2)`:
-
-        [] = read-out electronics
-        [==========] = read-out register
-        [..........] = serial prescan
-        [pppppppppp] = parallel overscan
-        [ssssssssss] = serial overscan
-        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-        [tttttttttt] = parallel / serial charge injection region trail
-
-               [ppppppppppppppppppppp]
-               [ppppppppppppppppppppp]
-          [...][xxxxxxxxxxxxxxxxxxxxx][sss]
-          [...][ccccccccccccccccccccc][sts]
-        | [...][ccccccccccccccccccccc][tst]    |
-        | [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | Direction
-        P [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | of
-        | [...][ccccccccccccccccccccc][sts]    | clocking
-          [...][ccccccccccccccccccccc][tst]    |
-
-        []     [=====================]
-               <--------Ser---------
-
-        The extracted array keeps just the leading edge and trails following all charge injection scans and
-        replaces all other values with 0s:
-
-               [000000000000000000000]
-               [000000000000000000000]
-          [000][000000000000000000000][000]
-          [000][cc0000000000000000000][st0]
-        | [000][cc0000000000000000000][ts0]    |
-        | [000][000000000000000000000][000]    | Direction
-        P [000][000000000000000000000][000]    | of
-        | [000][cc0000000000000000000][st0]    | clocking
-          [000][cc0000000000000000000][st0]    |
+            fpr_pixels = (0, 1) will extract just the leading front edge column.
+            fpr_pixels = (0, 2) will extract the leading two front edge columns.
+            trails_pixels = (0, 1) will extract the first column of trails closest to the charge injection region.
+
+            The diagram below illustrates the arrays that is extracted from a array for `fpr_pixels=(0,2)` and
+            `trails_pixels=(0,2)`:
+
+            [] = read-out electronics
+            [==========] = read-out register
+            [..........] = serial prescan
+            [pppppppppp] = parallel overscan
+            [ssssssssss] = serial overscan
+            [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+            [tttttttttt] = parallel / serial charge injection region trail
+
+                   [ppppppppppppppppppppp]
+                   [ppppppppppppppppppppp]
+              [...][xxxxxxxxxxxxxxxxxxxxx][sss]
+              [...][ccccccccccccccccccccc][sts]
+            | [...][ccccccccccccccccccccc][tst]    |
+            | [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | Direction
+            P [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | of
+            | [...][ccccccccccccccccccccc][sts]    | clocking
+              [...][ccccccccccccccccccccc][tst]    |
+
+            []     [=====================]
+                   <--------Ser---------
+
+            The extracted array keeps just the leading edge and trails following all charge injection scans and
+            replaces all other values with 0s:
+
+                   [000000000000000000000]
+                   [000000000000000000000]
+              [000][000000000000000000000][000]
+              [000][cc0000000000000000000][st0]
+            | [000][cc0000000000000000000][ts0]    |
+            | [000][000000000000000000000][000]    | Direction
+            P [000][000000000000000000000][000]    | of
+            | [000][cc0000000000000000000][st0]    | clocking
+              [000][cc0000000000000000000][st0]    |
 
-        []     [=====================]
-               <--------Ser---------
+            []     [=====================]
+                   <--------Ser---------
 
-        Parameters
-    ----------
-        array
-        fpr_pixels
-            The column indexes to extract the front edge between (e.g. columns(0, 3) extracts the 1st, 2nd and 3rd rows)
-        trails_pixels
-            The column indexes to extract the trails between (e.g. columns(0, 3) extracts the 1st, 2nd and 3rd rows)
+            Parameters
+        ----------
+            array
+            fpr_pixels
+                The column indexes to extract the front edge between (e.g. columns(0, 3) extracts the 1st, 2nd and 3rd rows)
+            trails_pixels
+                The column indexes to extract the trails between (e.g. columns(0, 3) extracts the 1st, 2nd and 3rd rows)
         """
         new_array = array.native.copy() * 0.0
 
         if fpr_pixels is not None:
-
             new_array = self.serial_fpr.add_to_array(
-                new_array=new_array, array=array, pixels=fpr_pixels
+                new_array=new_array,
+                array=array,
+                settings=SettingsExtract(pixels=fpr_pixels),
             )
 
         if eper_pixels is not None:
-
             new_array = self.serial_eper.add_to_array(
-                new_array=new_array, array=array, pixels=eper_pixels
+                new_array=new_array,
+                array=array,
+                settings=SettingsExtract(pixels=eper_pixels),
             )
 
         return new_array
 
     def serial_overscan_above_eper_array_2d_from(self, array: aa.Array2D) -> aa.Array2D:
         """
         Extract an array of the region above the EPER trails of the serial overscan.
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/parallel/abstract.py` & `autocti-2023.7.7.2/autocti/extract/two_d/serial/abstract.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,128 +1,137 @@
 import numpy as np
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
-
 from autocti.extract.two_d.abstract import Extract2D
+from autocti.extract.settings import SettingsExtract
 
 
-class Extract2DParallel(Extract2D):
+class Extract2DSerial(Extract2D):
     @property
     def binning_axis(self) -> int:
         """
-        The axis over which binning is performed to turn 2D parallel data (e.g. an EPER) into 1D data.
+        The axis over which binning is performed to turn 2D serial data (E.g. an EPER) into 1D data.
 
-        For a parallel extract `axis=1` such that binning is performed over the rows containing the EPER.
+        For a serial extract `axis=0` such that binning is performed over the rows containing the EPER.
         """
-        return 1
+        return 0
+
+    def _value_list_from(
+        self, array: aa.Array2D, value_str: str, settings: SettingsExtract
+    ):
+        median_list = []
+
+        arr_list = [
+            np.ma.array(data=array.native[region.slice], mask=array.mask[region.slice])
+            for region in self.region_list_from(settings=settings)
+        ]
+
+        arr_stack = np.ma.stack(arr_list)
+
+        for row_index in range(arr_list[0].shape[0]):
+            if value_str == "median":
+                median_list.append(float(np.ma.median(arr_stack[:, row_index, :])))
+
+        return median_list
 
     def median_list_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> List[float]:
         """
         Returns the median values of the `Extract2D` object's corresponding region, where the median is taken over
-        all columns of the region(s).
+        all rows of the region(s).
 
         To describe this function we will use the example of estimating the median of the charge lines in charge
-        injection data, by taking the median over every individual column of charge injection (e.g. aligned with the
-        FPR).
-
-        The inner regions of the FPR of each charge injection line informs us of the injected level of charge for
-        that injection.
+        injection data, by taking the median over the rows of charge injection (e.g. each median is anti-aligned with
+        the FPR).
 
         By taking the median of values of the charge injection regions (after accounting for those which have had
-        electrons captured and relocated due to CTI), we can therefore estimate the input charge injection
-        normalization.
+        electrons captured and relocated due to CTI), we can therefore estimate whether there is row-to-row variation
+        in the charge injection.
 
-        This function does this for every column of every charge injection. If multiple charge injections are performed
-        per column, the median of all charge regions is taken.
+        This function does this for every rows of every charge injection. If multiple charge injections are performed,
+        the median of all charge regions is taken.
 
         For example, if there are 3 charge injection regions, this function returns a list where each value
         estimates the charge injection normalization of a given charge injection region. The size of this list
-        is therefore the number of charge injection columns.
+        is therefore the number of charge injection rows.
 
         The function `median_list_of_lists_from` performs the median over each individual charge injection
-        region in each column. It therefore estimates multiple injection normalizations per column. for each individual
+        region in each row. It therefore estimates multiple injection normalizations per row. for each individual
         charge region. Which function one uses depends on the properties of the charge injection on the instrumentation.
 
         Parameters
         ----------
-        array
-            The charge injection image from which the charge injection normalizations are estimated.
-        pixels
-            The row pixel index to extract the FPR between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd
-            FPR rows). To remove the 10 leading pixels which have lost electrons due to CTI, an input such
-            as `pixels=(10, 30)` would be used.
-        """
-        median_list = []
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
+        """
+        return self._value_list_from(
+            array=array,
+            value_str="median",
+            settings=settings,
+        )
+
+    def _value_list_of_lists_from(
+        self, array: aa.Array2D, value_str: str, settings: SettingsExtract
+    ):
+        median_lists = []
 
         arr_list = [
             np.ma.array(data=array.native[region.slice], mask=array.mask[region.slice])
-            for region in self.region_list_from(pixels=pixels)
+            for region in self.region_list_from(settings=settings)
         ]
 
-        arr_stack = np.ma.stack(arr_list)
+        for array_2d in arr_list:
+            value_list = []
 
-        for column_index in range(arr_list[0].shape[1]):
+            for row_index in range(array_2d.shape[0]):
+                value = float(np.ma.median(array_2d[row_index, :]))
 
-            median_list.append(float(np.ma.median(arr_stack[:, :, column_index])))
+                if value_str == "median":
+                    value_list.append(value)
 
-        return median_list
+            median_lists.append(value_list)
+
+        return median_lists
 
     def median_list_of_lists_from(
-        self, array: aa.Array2D, pixels: Tuple[int, int]
+        self, array: aa.Array2D, settings: SettingsExtract
     ) -> List[List]:
         """
         Returns the median values of the `Extract2D` object's corresponding region, where the median is taken over
-        all column(s) of every individual region.
+        all row(s) of every individual region.
 
         To describe this function we will use the example of estimating the median of the charge lines in charge
-        injection data, by taking the median over every individual column of charge injection (e.g. aligned with the
+        injection data, by taking the median over every individual row of charge injection (e.g. aligned with the
         FPR).
 
         The inner regions of the FPR of each charge injection line informs us of the injected level of
         charge for that injection.
 
         By taking the median of values of the charge injection regions (after accounting for those which have had
         electrons captured and relocated due to CTI), we can therefore estimate the input charge injection
         normalization.
 
-        This function does this for every column of every individual charge injection for every charge injection region.
+        This function does this for every row of every individual charge injection for every charge injection region.
 
         For example, if there are 3 charge injection regions, this function returns a list of lists where the outer
         list contains 3 lists each of which give estimates of the charge injection normalization in a given charge
-        injection region. Thd size of the inner list is therefore the number of charge injection columns.
+        injection region. Thd size of the inner list is therefore the number of charge injection rows.
 
         The function `median_list_from` performs the median over all charge injection region in each
-        column and thus estimates a single injection normalization per column. Which function one uses depends on the
+        row and thus estimates a single injection normalization per row. Which function one uses depends on the
         properties of the charge injection on the instrumentation.
 
         Parameters
         ----------
-        array
-            The data from which the median values are estimated.
-        pixels
-            The row pixel index to extract the region between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd
-            rows of the region).
-        """
-        median_lists = []
-
-        arr_list = [
-            np.ma.array(data=array.native[region.slice], mask=array.mask[region.slice])
-            for region in self.region_list_from(pixels=pixels)
-        ]
-
-        for array_2d in arr_list:
-
-            value_list = []
-
-            for column_index in range(array_2d.shape[1]):
-
-                value = float(np.ma.median(array_2d[:, column_index]))
-
-                value_list.append(value)
-
-            median_lists.append(value_list)
-
-        return median_lists
+        settings
+           The settings used to extract the serial region (e.g. the EPERs), which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
+        """
+        return self._value_list_of_lists_from(
+            array=array,
+            value_str="median",
+            settings=settings,
+        )
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/parallel/calibration.py` & `autocti-2023.7.7.2/autocti/extract/two_d/parallel/calibration.py`

 * *Files 18% similar despite different names*

```diff
@@ -202,15 +202,14 @@
         return self.with_extracted_regions(
             layout=layout, extraction_region=extraction_region
         )
 
     def with_extracted_regions(
         self, layout, extraction_region: aa.type.Region2DLike
     ) -> Layout2DCI:
-
         layout = deepcopy(layout)
 
         extracted_region_list = list(
             map(
                 lambda region: aa.util.layout.region_after_extraction(
                     original_region=region, extraction_region=extraction_region
                 ),
@@ -221,62 +220,62 @@
         if not extracted_region_list:
             extracted_region_list = None
 
         layout.region_list = extracted_region_list
         return layout
 
     def imaging_ci_from(
-        self, imaging_ci: ImagingCI, columns: Tuple[int, int]
+        self, dataset: ImagingCI, columns: Tuple[int, int]
     ) -> ImagingCI:
         """
         Returnss a function to extract a parallel section for given columns
         """
 
         from autocti.charge_injection.imaging.imaging import ImagingCI
 
         cosmic_ray_map = (
-            imaging_ci.layout.extract.parallel_calibration.array_2d_from(
-                array=imaging_ci.cosmic_ray_map, columns=columns
+            dataset.layout.extract.parallel_calibration.array_2d_from(
+                array=dataset.cosmic_ray_map, columns=columns
             )
-            if imaging_ci.cosmic_ray_map is not None
+            if dataset.cosmic_ray_map is not None
             else None
         )
 
-        if imaging_ci.noise_scaling_map_dict is not None:
-
+        if dataset.noise_scaling_map_dict is not None:
             noise_scaling_map_dict = {
-                key: imaging_ci.layout.extract.parallel_calibration.array_2d_from(
+                key: dataset.layout.extract.parallel_calibration.array_2d_from(
                     array=noise_scaling_map, columns=columns
                 )
-                for key, noise_scaling_map in imaging_ci.noise_scaling_map_dict.items()
+                for key, noise_scaling_map in dataset.noise_scaling_map_dict.items()
             }
 
         else:
-
             noise_scaling_map_dict = None
 
         extraction_region = (
-            imaging_ci.layout.extract.parallel_calibration.extraction_region_from(
+            dataset.layout.extract.parallel_calibration.extraction_region_from(
                 columns=columns
             )
         )
 
-        mask = self.mask_2d_from(mask=imaging_ci.mask, columns=columns)
+        mask = self.mask_2d_from(mask=dataset.mask, columns=columns)
 
-        imaging_ci = ImagingCI(
-            image=imaging_ci.layout.extract.parallel_calibration.array_2d_from(
-                array=imaging_ci.image, columns=columns
+        dataset = ImagingCI(
+            data=dataset.layout.extract.parallel_calibration.array_2d_from(
+                array=dataset.data, columns=columns
             ),
-            noise_map=imaging_ci.layout.extract.parallel_calibration.array_2d_from(
-                array=imaging_ci.noise_map, columns=columns
+            noise_map=dataset.layout.extract.parallel_calibration.array_2d_from(
+                array=dataset.noise_map, columns=columns
             ),
-            pre_cti_data=imaging_ci.layout.extract.parallel_calibration.array_2d_from(
-                array=imaging_ci.pre_cti_data, columns=columns
+            pre_cti_data=dataset.layout.extract.parallel_calibration.array_2d_from(
+                array=dataset.pre_cti_data, columns=columns
             ),
-            layout=imaging_ci.layout.layout_extracted_from(
+            layout=dataset.layout.layout_extracted_from(
                 extraction_region=extraction_region
             ),
             cosmic_ray_map=cosmic_ray_map,
             noise_scaling_map_dict=noise_scaling_map_dict,
+            fpr_value=dataset.fpr_value,
+            settings_dict=dataset.settings_dict,
         )
 
-        return imaging_ci.apply_mask(mask=mask)
+        return dataset.apply_mask(mask=mask)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/parallel/eper.py` & `autocti-2023.7.7.2/autocti/extract/two_d/parallel/eper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,143 +1,171 @@
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.two_d.parallel.abstract import Extract2DParallel
+from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
 
 class Extract2DParallelEPER(Extract2DParallel):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         """
-          Returns a list of the 2D parallel EPER regions from the `region_list` containing signal  (e.g. the charge
-          injection regions of charge injection data), extracted between two input `pixels` indexes.
+        Returns a list of the 2D parallel EPER regions from the `region_list` containing signal (e.g. the charge
+        injection regions of charge injection data), between two input `pixels` indexes.
 
-          Negative pixel values are supported to the `pixels` tuple, whereby columns in front of the parallel EPERs
-          (e.g. the FPRs) are also extracted.
+        Negative pixel values can be input into the `pixels` tuple, whereby columns in front of the parallel EPERs
+        (e.g. the FPRs) are extracted.
 
-          The diagram below illustrates the extraction for `pixels=(0, 1)`:
-
-          [] = read-out electronics
-          [==========] = read-out register
-          [..........] = serial prescan
-          [pppppppppp] = parallel overscan
-          [ssssssssss] = serial overscan
-          [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-          [tttttttttt] = parallel / serial charge injection region trail
-
-                 [ppppppppppppppppppppp]
-                 [ppppppppppppppppppppp]
-            [...][t1t1t1t1t1t1t1t1t1t1t][sss]
-            [...][c1c1cc1c1cc1cc1ccc1cc][sss]
-          | [...][1c1c1cc1c1cc1ccc1cc1c][sss]     |
-          | [...][t0t0t0t0t0t0t0t0t0t0t][sss]    | Direction
+        The method includes a unique behaviour overide, where if `pixels_from_end=-1` is input the method will return
+        the region lists containg the full parallel EPER regions after each charge injection block (accounting for
+        the possibility that charge injection regions are not spaced uniformly).
+
+        The diagram below illustrates the extraction for `pixels=(0, 1)`:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = parallel / serial charge injection region trail
+
+              [ppppppppppppppppppppp]
+              [ppppppppppppppppppppp]
+         [...][t1t1t1t1t1t1t1t1t1t1t][sss]
+         [...][c1c1cc1c1cc1cc1ccc1cc][sss]
+        | [...][1c1c1cc1c1cc1ccc1cc1c][sss]     |
+        | [...][t0t0t0t0t0t0t0t0t0t0t][sss]    | Direction
         Par [...][0t0t0t0t0t0t0t0t0t0t0][sss]    | of
-          | [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
-         |/ [...][cc0ccc0cccc0cccc0cccc][sss]   \/
+        | [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
+        |/ [...][cc0ccc0cccc0cccc0cccc][sss]   \/
 
-          []     [=====================]
-                 <---------Ser----------
+        []     [=====================]
+              <---------Ser----------
 
-          The extracted regions correspond to the first parallel EPER all charge injection regions:
+        The extracted regions correspond to the first parallel EPER all charge injection regions:
 
-          region_list[0] = [2, 4, 3, 21] (serial prescan is 3 pixels)
-          region_list[1] = [6, 7, 3, 21] (serial prescan is 3 pixels)
+        region_list[0] = [2, 4, 3, 21] (serial prescan is 3 pixels)
+        region_list[1] = [6, 7, 3, 21] (serial prescan is 3 pixels)
 
-          For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
-          parallel EPER of each charge injection region:
+        For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
+        parallel EPER of each charge injection region:
 
-          array_2d_list[0] = [t0t0t0tt0t0t0t0t0t0t0]
-          array_2d_list[1] = [1t1t1t1t1t1t1t1t1t1t1]
+        array_2d_list[0] = [t0t0t0tt0t0t0t0t0t0t0]
+        array_2d_list[1] = [1t1t1t1t1t1t1t1t1t1t1]
 
-          Parameters
-          ----------
-          pixels
-              The row indexes to extract the trails between (e.g. rows(0, 3) extracts the 1st, 2nd and 3rd rows)
+        Parameters
+        ----------
+        settings
+           The settings used to extract the parallel EPERs, which for example include the `pixels` tuple specifying the
+           range of pixel rows they are extracted between.
         """
-        return [
-            region.parallel_trailing_region_from(pixels=pixels)
-            for region in self.region_list
-        ]
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
-        """
-        The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
-        CTI modeling in 1D.
+        pixels = settings.pixels
 
-        This is performed by binning up the data via the `binned_array_1d_from` function.
+        region_list = []
 
-        In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
-        charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
+        if settings.pixels_from_end is not None:
+            parallel_row_spaces = self.parallel_rows_between_regions + [
+                self.parallel_rows_to_array_edge
+            ]
 
-        The function returns the this region if the 1D dataset is extracted from the parallel EPERs. The
-        charge region is only included if there are negative entries in the `pixels` tuple, meaning that pixels
-        before the EPERs (e.g. the FPR) are extracted.
+        for i, region in enumerate(self.region_list):
+            if settings.pixels_from_end is not None:
+                if settings.pixels_from_end == -1:
+                    pixels = (
+                        0,
+                        parallel_row_spaces[i],
+                    )
 
-        Parameters
-        ----------
-        pixels
-            The row pixel index to extract the EPERs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd EPER
-            rows)
-        """
-        return extract_2d_util.binned_region_1d_eper_from(pixels=pixels)
+                else:
+                    pixels = (
+                        parallel_row_spaces[i] - settings.pixels_from_end,
+                        parallel_row_spaces[i],
+                    )
+
+            region_list.append(region.parallel_trailing_region_from(pixels=pixels))
+
+        return region_list
 
     def array_2d_from(self, array: aa.Array2D) -> aa.Array2D:
         """
-         Extract all of the areas of an `Array2D` that contain the parallel EPERs and return them as a new `Array2D`
-         where these extracted regions are included and everything else (e.g. the charge injection regions, serial
-         EPERs) are zeros.
-
-         The dimensions of the input array therefore do not change (unlike other `Layout2DCI` methods).
-
-         Negative pixel values are supported to the `pixels` tuple, whereby rows in front of the parallel EPERs (e.g.
-         the FPR) are also extracted.
-
-         The diagram below illustrates the extraction:
-
-         [] = read-out electronics
-         [==========] = read-out register
-         [..........] = serial prescan
-         [pppppppppp] = parallel overscan
-         [ssssssssss] = serial overscan
-         [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-         [tttttttttt] = parallel / serial charge injection region trail
-
-                [tptpptptptpptpptpptpt]
-                [tptptptpptpttptptptpt]
-           [...][ttttttttttttttttttttt][sss]
-           [...][ccccccccccccccccccccc][sss]
-         | [...][ccccccccccccccccccccc][sss]    |
-         | [...][ttttttttttttttttttttt][sss]    | Direction
+        Extract from an `Array2D` the parallel EPERs and return them as a new `Array2D` where everything else (e.g.
+        the charge injection regions, serial EPERs) are zeros.
+
+        The dimensions of the input array therefore do not change (unlike other ``Extract`` methods).
+
+        Negative pixel values can be input into the `pixels` tuple, whereby rows in front of the parallel EPERs (e.g.
+        the FPR) are extracted.
+
+        The diagram below illustrates the extraction:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = parallel / serial charge injection region trail
+
+             [tptpptptptpptpptpptpt]
+             [tptptptpptpttptptptpt]
+        [...][ttttttttttttttttttttt][sss]
+        [...][ccccccccccccccccccccc][sss]
+        | [...][ccccccccccccccccccccc][sss]    |
+        | [...][ttttttttttttttttttttt][sss]    | Direction
         Par[...][ttttttttttttttttttttt][sss]    | of
-         | [...][ccccccccccccccccccccc][sss]    | clocking
+        | [...][ccccccccccccccccccccc][sss]    | clocking
         |/ [...][ccccccccccccccccccccc][sss]   \/
 
-         []     [=====================]
-                <--------Ser---------
+        []     [=====================]
+             <--------Ser---------
 
-         The extracted array keeps only the parallel EPERs, everything else become 0s:
+        The extracted array keeps only the parallel EPERs, everything else become 0s:
 
-                [tptpptptptpptpptpptpt]
-                [tptptptpptpttptptptpt]
-           [000][ttttttttttttttttttttt][000]
-           [000][000000000000000000000][000]
-         | [000][000000000000000000000][000]    |
-         | [000][ttttttttttttttttttttt][000]    | Direction
+             [tptpptptptpptpptpptpt]
+             [tptptptpptpttptptptpt]
+          [000][ttttttttttttttttttttt][000]
+          [000][000000000000000000000][000]
+        | [000][000000000000000000000][000]    |
+        | [000][ttttttttttttttttttttt][000]    | Direction
         Par[000][ttttttttttttttttttttt][000]    | of
-         | [000][000000000000000000000][000]    | clocking
+        | [000][000000000000000000000][000]    | clocking
         |/ [000][000000000000000000000][000]   \/
 
-         []     [=====================]
-                <--------Ser---------
+        []     [=====================]
+             <--------Ser---------
         """
 
-        parallel_array = array.native.copy()
+        array_2d = array.native.copy()
 
         for region in self.region_list:
-            parallel_array[region.slice] = 0.0
+            array_2d[region.slice] = 0.0
+
+        array_2d.native[self.serial_prescan.slice] = 0.0
+        array_2d.native[self.serial_overscan.slice] = 0.0
+
+        return array_2d
+
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
+        """
+        The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
+        CTI modeling in 1D.
+
+        This is performed by binning up the data via the `binned_array_1d_from` function.
 
-        parallel_array.native[self.serial_prescan.slice] = 0.0
-        parallel_array.native[self.serial_overscan.slice] = 0.0
+        In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
+        charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
 
-        return parallel_array
+        The function returns the this region if the 1D dataset is extracted from the parallel EPERs. The
+        charge region is only included if there are negative entries in the `pixels` tuple, meaning that pixels
+        before the EPERs (e.g. the FPR) are extracted.
+
+        Parameters
+        ----------
+        settings
+           The settings used to extract the parallel EPERs, which for example include the `pixels` tuple specifying the
+           range of pixel rows they are extracted between.
+        """
+        return extract_2d_util.binned_region_1d_eper_from(pixels=settings.pixels)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/parallel/fpr.py` & `autocti-2023.7.7.2/autocti/extract/two_d/parallel/fpr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-from typing import List, Tuple
+from typing import List
 
 import autoarray as aa
 
 from autocti.extract.two_d.parallel.abstract import Extract2DParallel
+from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
 
 class Extract2DParallelFPR(Extract2DParallel):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         """
-         Returns a list of the 2D parallel FPR regions from the `region_list` containing signal  (e.g. the charge
-         injection regions of charge injection data), extracted between two input `pixels` indexes.
+        Returns a list of the 2D parallel FPR regions from the `region_list` containing signal  (e.g. the charge
+        injection regions of charge injection data), between two input `pixels` indexes.
 
-         Negative pixel values are supported to the `pixels` tuple, whereby columns in front of the parallel FPRs
-         are also extracted.
+        Negative pixel values can be input into the `pixels` tuple, whereby columns in front of the parallel FPRs
+        are extracted.
 
-         A 2D region is defined following the convention:
+        A 2D region is defined following the convention:
 
-         (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
-
-         For parallel FPR's the charge spans all columns of the charge injection region, thus the coordinates x0 and x1
-         do not change. y0 and y1 are updated based on the `pixels` input.
-
-         Negative pixel values are supported to the `pixels` tuple, whereby rows in front of the parallel FPRs are
-         also extracted.
-
-         The diagram below illustrates the extraction for `pixels=(0, 1)`:
-
-         [] = read-out electronics
-         [==========] = read-out register
-         [..........] = serial prescan
-         [pppppppppp] = parallel overscan
-         [ssssssssss] = serial overscan
-         [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-         [tttttttttt] = parallel / serial charge injection region trail
-
-                [ppppppppppppppppppppp]
-                [ppppppppppppppppppppp]
-            [...][ttttttttttttttttttttt][sss]
-            [...][c1c1cc1c1cc1cc1ccc1cc][sss]
-         |  [...][1c1c1cc1c1cc1ccc1cc1][sss]    |
-         |  [...][ttttttttttttttttttttt][sss]    | Direction
+        (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
+
+        For parallel FPR's the charge spans all columns of the charge injection region, thus the coordinates x0 and x1
+        do not change. y0 and y1 are updated based on the `pixels` input.
+
+        Negative pixel values can be input into the `pixels` tuple, whereby rows in front of the parallel FPRs are
+        also extracted.
+
+        The diagram below illustrates the extraction for `pixels=(0, 1)`:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = parallel / serial charge injection region trail
+
+               [ppppppppppppppppppppp]
+               [ppppppppppppppppppppp]
+           [...][ttttttttttttttttttttt][sss]
+           [...][c1c1cc1c1cc1cc1ccc1cc][sss]
+        |  [...][1c1c1cc1c1cc1ccc1cc1][sss]    |
+        |  [...][ttttttttttttttttttttt][sss]    | Direction
         Par [...][ttttttttttttttttttttt][sss]    | of
-         |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
+        |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
         |/  [...][cc0ccc0cccc0cccc0cccc][sss]    \/
 
-         []     [=====================]
-                <---------Ser--------
+        []     [=====================]
+               <---------Ser--------
 
-         The extracted regions correspond to the first parallel FPR all charge injection regions:
+        The extracted regions correspond to the first parallel FPR all charge injection regions:
 
-         region_list[0] = [0, 1, 3, 21] (serial prescan is 3 pixels)
-         region_list[1] = [3, 4, 3, 21] (serial prescan is 3 pixels)
+        region_list[0] = [0, 1, 3, 21] (serial prescan is 3 pixels)
+        region_list[1] = [3, 4, 3, 21] (serial prescan is 3 pixels)
 
-         For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
-         parallel FPR of each charge injection region:
+        For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
+        parallel FPR of each charge injection region:
 
-         array_2d_list[0] = [c0c0c0cc0c0c0c0c0c0c0]
-         array_2d_list[1] = [1c1c1c1c1c1c1c1c1c1c1]
+        array_2d_list[0] = [c0c0c0cc0c0c0c0c0c0c0]
+        array_2d_list[1] = [1c1c1c1c1c1c1c1c1c1c1]
 
-         Parameters
-         ----------
-         pixels
-             The row pixel index which determines the region of the FPR (e.g. `pixels=(0, 3)` will compute the region
-             corresponding to the 1st, 2nd and 3rd FPR rows).
+        Parameters
+        ----------
+        settings
+           The settings used to extract the parallel FPRs, which for example include the `pixels` tuple specifying the
+           range of pixel rows they are extracted between.
         """
         return [
-            region.parallel_front_region_from(pixels=pixels)
+            region.parallel_front_region_from(
+                pixels=settings.pixels, pixels_from_end=settings.pixels_from_end
+            )
             for region in self.region_list
         ]
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
         """
         The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
         CTI modeling in 1D.
 
         This is performed by binning up the data via the `binned_array_1d_from` function.
 
         In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
         charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
 
         The function returns the this region if the 1D dataset is extracted from the parallel FPRs. This is
         the full range of the `pixels` tuple, unless negative entries are included, meaning that pixels
-        before the FPRs are also extracted.
+        before the FPRs are extracted.
 
         Parameters
         ----------
-        pixels
-            The row pixel index to extract the FPRs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd FPR
-            rows)
+        settings
+           The settings used to extract the parallel FPR, which for example include the `pixels` tuple specifying the
+           range of pixel rows they are extracted between.
         """
-        return extract_2d_util.binned_region_1d_fpr_from(pixels=pixels)
+        return extract_2d_util.binned_region_1d_fpr_from(pixels=settings.pixels)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/parallel/overscan.py` & `autocti-2023.7.7.2/autocti/extract/two_d/parallel/overscan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.two_d.parallel.abstract import Extract2DParallel
+from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
 
 class Extract2DParallelOverscan(Extract2DParallel):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         """
-         Returns a list containing the 2D parallel overscan region, which is simply the parallel overscan input to the
-         object, extracted between two input `pixels` indexes (this is somewhat redundant information, but mimicks
-         the `Extract` object API across all other `Extract` objects).
-
-         (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
-
-         The parallel overscan spans all columns of the image, thus the coordinates x0 and x1 do not change. y0 and y1
-         are updated based on the `pixels` input.
-
-         Negative pixel values are supported to the `pixels` tuple, whereby rows in front of the parallel overscan are
-         also extracted.
-
-         The diagram below illustrates the extraction for `pixels=(0, 1)`:
-
-         [] = read-out electronics
-         [==========] = read-out register
-         [..........] = serial prescan
-         [pppppppppp] = parallel overscan
-         [ssssssssss] = serial overscan
-         [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-         [tttttttttt] = parallel / serial charge injection region trail
-
-                [ppppppppppppppppppppp]
-                [ppppppppppppppppppppp]
-            [...][ttttttttttttttttttttt][sss]
-            [...][c1c1cc1c1cc1cc1ccc1cc][sss]
-         |  [...][1c1c1cc1c1cc1ccc1cc1][sss]    |
-         |  [...][ttttttttttttttttttttt][sss]    | Direction
+        Returns a list of the 2D parallel overscan region, which is simply the parallel overscan input to the
+        object, between two input `pixels` indexes (this is somewhat redundant information, but mimicks
+        the `Extract` object API across all other `Extract` objects).
+
+        (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
+
+        The parallel overscan spans all columns of the image, thus the coordinates x0 and x1 do not change. y0 and y1
+        are updated based on the `pixels` input.
+
+        Negative pixel values can be input into the `pixels` tuple, whereby rows in front of the parallel overscan are
+        also extracted.
+
+        The diagram below illustrates the extraction for `pixels=(0, 1)`:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = parallel / serial charge injection region trail
+
+               [ppppppppppppppppppppp]
+               [ppppppppppppppppppppp]
+           [...][ttttttttttttttttttttt][sss]
+           [...][c1c1cc1c1cc1cc1ccc1cc][sss]
+        |  [...][1c1c1cc1c1cc1ccc1cc1][sss]    |
+        |  [...][ttttttttttttttttttttt][sss]    | Direction
         Par [...][ttttttttttttttttttttt][sss]    | of
-         |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
+        |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
         |/  [...][cc0ccc0cccc0cccc0cccc][sss]    \/
 
-         []     [=====================]
-                <---------Ser--------
+        []     [=====================]
+               <---------Ser--------
 
-         The extracted regions correspond to the parallel overscan [ppppppppppppppp] regions.
+        The extracted regions correspond to the parallel overscan [ppppppppppppppp] regions.
 
-         For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
-         parallel pixels across the rows of the overscan:
+        For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
+        parallel pixels across the rows of the overscan:
 
-         array_2d_list[0] = [ppppppppppppppppppppp]
+        array_2d_list[0] = [ppppppppppppppppppppp]
 
-         Parameters
-         ----------
-         pixels
-             The row pixel index which determines the region of the overscan (e.g. `pixels=(0, 3)` will compute the
-             region corresponding to the 1st, 2nd and 3rd overscan rows).
+        Parameters
+        ----------
+        settings
+           The settings used to extract the parallel overscan, which for example include the `pixels` tuple specifying the
+           range of pixel rows they are extracted between.
         """
+
+        pixels = settings.pixels
+
+        if settings.pixels_from_end is not None:
+            pixels = (
+                self.parallel_overscan.total_rows - settings.pixels_from_end,
+                self.parallel_overscan.total_rows,
+            )
+
         parallel_overscan_extract = aa.Region2D(
             (
                 self.parallel_overscan.y0 + pixels[0],
                 self.parallel_overscan.y0 + pixels[1],
                 self.parallel_overscan.x0,
                 self.parallel_overscan.x1,
             )
         )
 
         return [parallel_overscan_extract]
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
         """
         The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
         CTI modeling in 1D.
 
         This is performed by binning up the data via the `binned_array_1d_from` function.
 
         In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
@@ -84,12 +94,12 @@
         charge region and therefore FPR. This is the case when science imaging flat field data is used.
 
         The charge region is therefore only included if there are negative entries in the `pixels` tuple, meaning that
         pixels before the overscan (e.g. the FPR) are extracted.
 
         Parameters
         ----------
-        pixels
-            The row pixel index to extract the EPERs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd EPER
-            rows)
+        settings
+           The settings used to extract the parallel overscan, which for example include the `pixels` tuple specifying the
+           range of pixel rows they are extracted between.
         """
-        return extract_2d_util.binned_region_1d_eper_from(pixels=pixels)
+        return extract_2d_util.binned_region_1d_eper_from(pixels=settings.pixels)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/serial/calibration.py` & `autocti-2023.7.7.2/autocti/extract/two_d/serial/calibration.py`

 * *Files 18% similar despite different names*

```diff
@@ -185,15 +185,14 @@
         return aa.Array2D(
             values=new_array,
             mask=mask_2d,
             header=array.header,
         )
 
     def extracted_layout_from(self, layout, new_shape_2d, rows):
-
         serial_prescan = (
             (0, new_shape_2d[0], self.serial_prescan[2], self.serial_prescan[3])
             if self.serial_prescan is not None
             else None
         )
         serial_overscan = (
             (0, new_shape_2d[0], self.serial_overscan[2], self.serial_overscan[3])
@@ -204,71 +203,70 @@
         x0 = self.region_list[0][2]
         x1 = self.region_list[0][3]
         offset = 0
 
         new_pattern_region_list_ci = []
 
         for region in self.region_list:
-
             labelsize = rows[1] - rows[0]
             new_pattern_region_list_ci.append(
                 aa.Region2D(region=(offset, offset + labelsize, x0, x1))
             )
             offset += labelsize
 
         new_layout = deepcopy(layout)
         new_layout.region_list = new_pattern_region_list_ci
         new_layout.serial_prescan = serial_prescan
         new_layout.serial_overscan = serial_overscan
 
         return new_layout
 
-    def imaging_ci_from(self, imaging_ci: ImagingCI, rows) -> ImagingCI:
+    def imaging_ci_from(self, dataset: ImagingCI, rows) -> ImagingCI:
         """
         Returnss a function to extract a serial section for given rows
         """
 
         from autocti.charge_injection.imaging.imaging import ImagingCI
 
         cosmic_ray_map = (
-            imaging_ci.layout.extract.serial_calibration.array_2d_from(
-                array=imaging_ci.cosmic_ray_map, rows=rows
+            dataset.layout.extract.serial_calibration.array_2d_from(
+                array=dataset.cosmic_ray_map, rows=rows
             )
-            if imaging_ci.cosmic_ray_map is not None
+            if dataset.cosmic_ray_map is not None
             else None
         )
 
-        if imaging_ci.noise_scaling_map_dict is not None:
-
+        if dataset.noise_scaling_map_dict is not None:
             noise_scaling_map_dict = {
-                key: imaging_ci.layout.extract.serial_calibration.array_2d_from(
+                key: dataset.layout.extract.serial_calibration.array_2d_from(
                     array=noise_scaling_map, rows=rows
                 )
-                for key, noise_scaling_map in imaging_ci.noise_scaling_map_dict.items()
+                for key, noise_scaling_map in dataset.noise_scaling_map_dict.items()
             }
 
         else:
-
             noise_scaling_map_dict = None
 
-        image = imaging_ci.layout.extract.serial_calibration.array_2d_from(
-            array=imaging_ci.image, rows=rows
+        image = dataset.layout.extract.serial_calibration.array_2d_from(
+            array=dataset.data, rows=rows
         )
 
-        mask = self.mask_2d_from(mask=imaging_ci.mask, rows=rows)
+        mask = self.mask_2d_from(mask=dataset.mask, rows=rows)
 
-        imaging_ci = ImagingCI(
-            image=image,
-            noise_map=imaging_ci.layout.extract.serial_calibration.array_2d_from(
-                array=imaging_ci.noise_map, rows=rows
+        dataset = ImagingCI(
+            data=image,
+            noise_map=dataset.layout.extract.serial_calibration.array_2d_from(
+                array=dataset.noise_map, rows=rows
             ),
-            pre_cti_data=imaging_ci.layout.extract.serial_calibration.array_2d_from(
-                array=imaging_ci.pre_cti_data, rows=rows
+            pre_cti_data=dataset.layout.extract.serial_calibration.array_2d_from(
+                array=dataset.pre_cti_data, rows=rows
             ),
-            layout=imaging_ci.layout.extract.serial_calibration.extracted_layout_from(
-                layout=imaging_ci.layout, new_shape_2d=image.shape, rows=rows
+            layout=dataset.layout.extract.serial_calibration.extracted_layout_from(
+                layout=dataset.layout, new_shape_2d=image.shape, rows=rows
             ),
             cosmic_ray_map=cosmic_ray_map,
             noise_scaling_map_dict=noise_scaling_map_dict,
+            fpr_value=dataset.fpr_value,
+            settings_dict=dataset.settings_dict,
         )
 
-        return imaging_ci.apply_mask(mask=mask)
+        return dataset.apply_mask(mask=mask)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/serial/eper.py` & `autocti-2023.7.7.2/autocti/extract/two_d/serial/eper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import Tuple
+from typing import Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.two_d.serial.abstract import Extract2DSerial
+from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
 
 class Extract2DSerialEPER(Extract2DSerial):
-    def region_list_from(self, pixels: Tuple[int, int]):
+    def region_list_from(self, settings: SettingsExtract):
         """
          Returns a list of the 2D serial EPER regions from the `region_list` containing signal  (e.g. the charge
-         injection regions of charge injection data), extracted between two input `pixels` indexes.
+         injection regions of charge injection data), between two input `pixels` indexes.
 
-         Negative pixel values are supported to the `pixels` tuple, whereby columns in front of the serial EPERs
-         (e.g. the FPRs) are also extracted.
+         Negative pixel values can be input into the `pixels` tuple, whereby columns in front of the serial EPERs
+         (e.g. the FPRs) are extracted.
 
          The diagram below illustrates the extraction for `pixels=(0, 1)`:
 
          [] = read-out electronics
          [==========] = read-out register
          [..........] = serial prescan
          [pppppppppp] = parallel overscan
@@ -48,44 +49,31 @@
          serial EPER of each charge injection region:
 
          array_2d_list[0] = [st0]
          array_2d_list[1] = [st1]
 
          Parameters
          ----------
-         pixels
-             The column indexes to extract the trails between (e.g. columns(0, 3) extracts the 1st, 2nd and 3rd columns)
+        settings
+           The settings used to extract the serial region EPERs from, which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
+
+        pixels = settings.pixels
+
+        if settings.pixels_from_end is not None:
+            pixels = (
+                self.shape_2d[1] - self.region_list[0].x1 - settings.pixels_from_end,
+                self.shape_2d[1] - self.region_list[0].x1,
+            )
         return [
             region.serial_trailing_region_from(pixels=pixels)
             for region in self.region_list
         ]
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
-        """
-        The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
-        CTI modeling in 1D.
-
-        This is performed by binning up the data via the `binned_array_1d_from` function.
-
-        In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
-        charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
-
-        The function returns the this region if the 1D dataset is extracted from theserial EPERs. The
-        charge region is only included if there are negative entries in the `pixels` tuple, meaning that pixels
-        before the EPERs (e.g. the FPR) are extracted.
-
-        Parameters
-        ----------
-        pixels
-            The column pixel index to extract the EPERs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd EPER
-            columns)
-        """
-        return extract_2d_util.binned_region_1d_eper_from(pixels=pixels)
-
     def array_2d_from(self, array: aa.Array2D) -> aa.Array2D:
         """
         Extract an arrays of all of the serial EPERs in the serial overscan region, that are to the side of a
         charge-injection scans from a charge injection array.
 
         The diagram below illustrates the arrays that is extracted from a array:
 
@@ -123,14 +111,36 @@
         | [000][000000000000000000000][tst]    | clocking
           [000][000000000000000000000][sts]    |
 
         []     [=====================]
                <--------Ser---------
         """
 
-        serial_array = array.native.copy() * 0.0
+        array_2d = array.native.copy() * 0.0
 
         return self.add_to_array(
-            new_array=serial_array,
+            new_array=array_2d,
             array=array,
-            pixels=(0, self.serial_overscan.total_columns),
+            settings=SettingsExtract(pixels=(0, self.serial_overscan.total_columns)),
         )
+
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
+        """
+        The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
+        CTI modeling in 1D.
+
+        This is performed by binning up the data via the `binned_array_1d_from` function.
+
+        In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
+        charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
+
+        The function returns the this region if the 1D dataset is extracted from theserial EPERs. The
+        charge region is only included if there are negative entries in the `pixels` tuple, meaning that pixels
+        before the EPERs (e.g. the FPR) are extracted.
+
+        Parameters
+        ----------
+        settings
+           The settings used to extract the serial region EPERs from, which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
+        """
+        return extract_2d_util.binned_region_1d_eper_from(pixels=settings.pixels)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/serial/fpr.py` & `autocti-2023.7.7.2/autocti/extract/two_d/serial/fpr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,87 @@
-from typing import Tuple
+from typing import Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.two_d.serial.abstract import Extract2DSerial
+from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
 
 class Extract2DSerialFPR(Extract2DSerial):
-    def region_list_from(self, pixels: Tuple[int, int]):
+    def region_list_from(self, settings: SettingsExtract):
         """
-         Returns a list of the 2D serial FPR regions from the `region_list` containing signal  (e.g. the charge
-         injection regions of charge injection data), extracted between two input `pixels` indexes.
+        Returns a list of the 2D serial FPR regions from the `region_list` containing signal  (e.g. the charge
+        injection regions of charge injection data), between two input `pixels` indexes.
 
-         Negative pixel values are supported to the `pixels` tuple, whereby columns in front of the serial FPRs (e.g.
-         the serial prescan) are also extracted.
+        Negative pixel values can be input into the `pixels` tuple, whereby columns in front of the serial FPRs (e.g.
+        the serial prescan) are extracted.
 
-         The diagram below illustrates the extraction for `pixels=(0, 1)`:
+        The diagram below illustrates the extraction for `pixels=(0, 1)`:
 
-         [] = read-out electronics
-         [==========] = read-out register
-         [..........] = serial prescan
-         [pppppppppp] = parallel overscan
-         [ssssssssss] = serial overscan
-         [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-         [tttttttttt] = parallel / serial charge injection region trail
-
-                [ppppppppppppppppppppp]
-                [ppppppppppppppppppppp]
-            [...][ttttttttttttttttttttt][sss]
-            [...][c1c1cc1c1cc1cc1ccc1cc][sss]
-         |  [...][1c1c1cc1c1cc1ccc1cc1c][sss]    |
-         |  [...][ttttttttttttttttttttt][sss]    | Direction
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = parallel / serial charge injection region trail
+
+               [ppppppppppppppppppppp]
+               [ppppppppppppppppppppp]
+           [...][ttttttttttttttttttttt][sss]
+           [...][c1c1cc1c1cc1cc1ccc1cc][sss]
+        |  [...][1c1c1cc1c1cc1ccc1cc1c][sss]    |
+        |  [...][ttttttttttttttttttttt][sss]    | Direction
         Par [...][ttttttttttttttttttttt][sss]    | of
-         |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
+        |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
         |/  [...][cc0ccc0cccc0cccc0cccc][sss]    \/
 
-         []     [=====================]
-                <---------Ser--------
+        []     [=====================]
+               <---------Ser--------
 
-         The extracted regions correspond to the first serial FPR all charge injection regions:
+        The extracted regions correspond to the first serial FPR all charge injection regions:
 
-         region_list[0] = [0, 2, 3, 21] (serial prescan is 3 pixels)
-         region_list[1] = [4, 6, 3, 21] (serial prescan is 3 pixels)
+        region_list[0] = [0, 2, 3, 21] (serial prescan is 3 pixels)
+        region_list[1] = [4, 6, 3, 21] (serial prescan is 3 pixels)
 
-         For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
-         serial FPR of each charge injection region:
+        For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
+        serial FPR of each charge injection region:
 
-         array_2d_list[0] =[c0c0]
-         array_2d_list[1] =[1c1c]
+        array_2d_list[0] =[c0c0]
+        array_2d_list[1] =[1c1c]
 
-         Parameters
-         ----------
-         pixels
-             The column indexes to extract the front edge between (e.g. columns(0, 3) extracts the 1st, 2nd and 3rd
-             columns)
+        Parameters
+        ----------
+        settings
+            The settings used to extract the serial region FPRs from, which for example include the `pixels`
+            tuple specifying the range of pixel columns they are extracted between.
         """
         return [
-            region.serial_front_region_from(pixels=pixels)
+            region.serial_front_region_from(
+                pixels=settings.pixels, pixels_from_end=settings.pixels_from_end
+            )
             for region in self.region_list
         ]
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
         """
         The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
         CTI modeling in 1D.
 
         This is performed by binning up the data via the `binned_array_1d_from` function.
 
         In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
         charge regions on the 1D dataset (e.g. where the FPR appears in 1D after binning).
 
         The function returns the this region if the 1D dataset is extracted from the serial FPRs. This is
         the full range of the `pixels` tuple, unless negative entries are included, meaning that pixels
-        before the FPRs are also extracted.
+        before the FPRs are extracted.
 
         Parameters
         ----------
-        pixels
-            The column pixel index to extract the FPRs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd FPR
-            columns)
+        settings
+            The settings used to extract the serial region FPRs from, which for example include the `pixels`
+            tuple specifying the range of pixel columns they are extracted between.
         """
-        return extract_2d_util.binned_region_1d_fpr_from(pixels=pixels)
+        return extract_2d_util.binned_region_1d_fpr_from(pixels=settings.pixels)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/serial/overscan.py` & `autocti-2023.7.7.2/autocti/extract/two_d/serial/overscan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.two_d.serial.abstract import Extract2DSerial
+from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
 
 class Extract2DSerialOverscan(Extract2DSerial):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         """
-         Returns a list containing the 2D serial verscan region, which is simply the parallel overscan input to the
-         object, extracted between two input `pixels` indexes (this is somewhat redundant information, but mimicks
-         the `Extract` object API across all other `Extract` objects).
-
-         (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
-
-         The serial overscan spans all columns of the image, thus the coordinates x0 and x1 do not change. y0 and y1
-         are updated based on the `pixels` input.
-
-         Negative pixel values are supported to the `pixels` tuple, whereby columns in front of the serial overscan are
-         also extracted.
-
-         The diagram below illustrates the extraction for `pixels=(0, 1)`:
-
-         [] = read-out electronics
-         [==========] = read-out register
-         [..........] = serial prescan
-         [pppppppppp] = serial overscan
-         [ssssssssss] = serial overscan
-         [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-         [tttttttttt] = serial / serial charge injection region trail
-
-                [ppppppppppppppppppppp]
-                [ppppppppppppppppppppp]
-            [...][ttttttttttttttttttttt][sss]
-            [...][c1c1cc1c1cc1cc1ccc1cc][sss]
-         |  [...][1c1c1cc1c1cc1ccc1cc1][sss]    |
-         |  [...][ttttttttttttttttttttt][sss]    | Direction
+        Returns a list of the 2D serial overscan region for extraction, which is the serial overscan input to the
+        object, between two input `pixels` indexes (this is somewhat redundant information, but mimicks
+        the `Extract` object API across all other `Extract` objects).
+
+        (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
+
+        The serial overscan spans all columns of the image, thus the coordinates x0 and x1 do not change. y0 and y1
+        are updated based on the `pixels` input.
+
+        Negative pixel values can be input into the `pixels` tuple, whereby columns in front of the serial overscan are
+        also extracted.
+
+        The diagram below illustrates the extraction for `pixels=(0, 1)`:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = serial overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = serial / serial charge injection region trail
+
+               [ppppppppppppppppppppp]
+               [ppppppppppppppppppppp]
+           [...][ttttttttttttttttttttt][sss]
+           [...][c1c1cc1c1cc1cc1ccc1cc][sss]
+        |  [...][1c1c1cc1c1cc1ccc1cc1][sss]    |
+        |  [...][ttttttttttttttttttttt][sss]    | Direction
         Par [...][ttttttttttttttttttttt][sss]    | of
-         |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
+        |  [...][0ccc0cccc0cccc0cccc0c][sss]    | clocking
         |/  [...][cc0ccc0cccc0cccc0cccc][sss]    \/
 
-         []     [=====================]
-                <---------Ser--------
+        []     [=====================]
+               <---------Ser--------
 
-         The extracted regions correspond to the serial overscan [sss] regions.
+        The extracted regions correspond to the serial overscan [sss] regions.
 
-         For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
-         serial pixels across the columns of the overscan:
+        For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
+        serial pixels across the columns of the overscan:
 
-         array_2d_list[0] = [s]
+        array_2d_list[0] = [s]
 
-         Parameters
-         ----------
-         pixels
-             The column pixel index which determines the region of the overscan (e.g. `pixels=(0, 3)` will compute the
-             region corresponding to the 1st, 2nd and 3rd overscan columns).
+        Parameters
+        ----------
+        settings
+            The settings used to extract the serial region overscan from, which for example include the `pixels`
+            tuple specifying the range of pixel columns they are extracted between.
         """
+
+        pixels = settings.pixels
+
+        if settings.pixels_from_end is not None:
+            pixels = (
+                self.serial_overscan.total_columns - settings.pixels_from_end,
+                self.serial_overscan.total_columns,
+            )
+
         serial_overscan_extract = aa.Region2D(
             (
                 self.serial_overscan.y0,
                 self.serial_overscan.y1,
                 self.serial_overscan.x0 + pixels[0],
                 self.serial_overscan.x0 + pixels[1],
             )
         )
 
         return [serial_overscan_extract]
 
-    def binned_region_1d_from(self, pixels: Tuple[int, int]) -> aa.Region1D:
+    def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
         """
         The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
         CTI modeling in 1D.
 
         This is performed by binning up the data via the `binned_array_1d_from` function.
 
         In order to create the 1D dataset a `Layout1D` is required, which requires the `region_list` containing the
@@ -84,12 +94,12 @@
         charge region and therefore FPR. This is the case when science imaging flat field data is used.
 
         The charge region is therefore only included if there are negative entries in the `pixels` tuple, meaning that
         pixels before the overscan (e.g. the FPR) are extracted.
 
         Parameters
         ----------
-        pixels
-            The column pixel index to extract the FPRs between (e.g. `pixels=(0, 3)` extracts the 1st, 2nd and 3rd FPR
-            columns)
+        settings
+            The settings used to extract the serial region overscan from, which for example include the `pixels`
+            tuple specifying the range of pixel columns they are extracted between.
         """
-        return extract_2d_util.binned_region_1d_eper_from(pixels=pixels)
+        return extract_2d_util.binned_region_1d_eper_from(pixels=settings.pixels)
```

### Comparing `autocti-2023.1.15.1/autocti/extract/two_d/serial/prescan.py` & `autocti-2023.7.7.2/autocti/extract/two_d/serial/prescan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,75 @@
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
 from autocti.extract.two_d.serial.abstract import Extract2DSerial
+from autocti.extract.settings import SettingsExtract
 
 
 class Extract2DSerialPrescan(Extract2DSerial):
-    def region_list_from(self, pixels: Tuple[int, int]) -> List[aa.Region2D]:
+    def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         """
-         Returns a list containing the 2D serial prescan region, which is simply the parallel overscan input to the
-         object, extracted between two input `pixels` indexes (this is somewhat redundant information, but mimicks
-         the `Extract` object API across all other `Extract` objects).
-
-         (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
-
-         The serial prescan spans all columns of the image, thus the coordinates x0 and x1 do not change. y0 and y1
-         are updated based on the `pixels` input.
-
-         Negative pixel values are supported to the `pixels` tuple, whereby columns in front of the serial prescan are
-         also extracted.
-
-         The diagram below illustrates the extraction for `pixels=(0, 1)`:
-
-         [] = read-out electronics
-         [==========] = read-out register
-         [..........] = serial prescan
-         [pppppppppp] = parallel overscan
-         [ssssssssss] = serial overscan
-         [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-         [tttttttttt] = serial / serial charge injection region trail
-
-                [ppppppppppppppppppppp]
-                [ppppppppppppppppppppp]
-            [...][ttttttttttttttttttttt][sss]
-            [...][f1f1ff1f1ff1ff1fff1ff][sss]
-         |  [...][1f1f1ff1f1ff1fff1ff1][sss]    |
-         |  [...][ttttttttttttttttttttt][sss]    | Direction
+        Returns a list of the 2D serial prescan region, which is simply the parallel overscan input to the
+        object, between two input `pixels` indexes (this is somewhat redundant information, but mimicks
+        the `Extract` object API across all other `Extract` objects).
+
+        (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
+
+        The serial prescan spans all columns of the image, thus the coordinates x0 and x1 do not change. y0 and y1
+        are updated based on the `pixels` input.
+
+        Negative pixel values can be input into the `pixels` tuple, whereby columns in front of the serial prescan are
+        also extracted.
+
+        The diagram below illustrates the extraction for `pixels=(0, 1)`:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = serial / serial charge injection region trail
+
+               [ppppppppppppppppppppp]
+               [ppppppppppppppppppppp]
+           [...][ttttttttttttttttttttt][sss]
+           [...][f1f1ff1f1ff1ff1fff1ff][sss]
+        |  [...][1f1f1ff1f1ff1fff1ff1][sss]    |
+        |  [...][ttttttttttttttttttttt][sss]    | Direction
         Par [...][ttttttttttttttttttttt][sss]    | of
-         |  [...][0fff0ffff0ffff0ffff0f][sss]    | clocking
+        |  [...][0fff0ffff0ffff0ffff0f][sss]    | clocking
         |/  [...][ff0fff0ffff0ffff0ffff][sss]    \/
 
-         []     [=====================]
-                <---------Ser--------
+        []     [=====================]
+               <---------Ser--------
 
-         The extracted regions correspond to the serial prescan [...] regions.
+        The extracted regions correspond to the serial prescan [...] regions.
 
-         For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
-         serial pixels across the columns of the prescan:
+        For `pixels=(0,1)` the extracted arrays returned via the `array_2d_list_from()` function keep the first
+        serial pixels across the columns of the prescan:
 
-         array_2d_list[0] = [s]
+        array_2d_list[0] = [s]
 
-         Parameters
-         ----------
-         pixels
-             The column pixel index which determines the region of the prescan (e.g. `pixels=(0, 3)` will compute the
-             region corresponding to the 1st, 2nd and 3rd prescan columns).
+        Parameters
+        ----------
+        settings
+           The settings used to extract the serial region overscan from, which for example include the `pixels`
+           tuple specifying the range of pixel columns they are extracted between.
         """
+
+        pixels = settings.pixels
+
+        if settings.pixels_from_end is not None:
+            pixels = (
+                self.serial_prescan.total_columns - settings.pixels_from_end,
+                self.serial_prescan.total_columns,
+            )
+
         serial_prescan_extract = aa.Region2D(
             (
                 self.serial_prescan.y0,
                 self.serial_prescan.y1,
                 self.serial_prescan.x0 + pixels[0],
                 self.serial_prescan.x0 + pixels[1],
             )
```

### Comparing `autocti-2023.1.15.1/autocti/fixtures.py` & `autocti-2023.7.7.2/autocti/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 ### IMAGING ###
 
 
 def make_imaging_7x7_frame():
     return ac.Imaging(
-        image=make_image_7x7_native(),
+        data=make_image_7x7_native(),
         noise_map=make_noise_map_7x7_native(),
         name="mock_imaging_7x7_frame",
     )
 
 
 ### LINE DATASET ###
 
@@ -107,15 +107,14 @@
 
 
 def make_pre_cti_data_7():
     return ac.Array1D.full(fill_value=1.0, shape_native=(7,), pixel_scales=1.0)
 
 
 def make_dataset_1d_7():
-
     return ac.Dataset1D(
         data=make_data_7(),
         noise_map=make_noise_map_7(),
         pre_cti_data=make_pre_cti_data_7(),
         layout=make_layout_7(),
     )
 
@@ -151,39 +150,37 @@
 def make_ci_cosmic_ray_map_7x7():
     cosmic_ray_map = np.zeros(shape=(7, 7))
 
     return ac.Array2D.no_mask(values=cosmic_ray_map, pixel_scales=(1.0, 1.0))
 
 
 def make_ci_noise_scaling_map_dict_7x7():
-
     return {
         "parallel_eper": ac.Array2D.ones(shape_native=(7, 7), pixel_scales=(1.0, 1.0)),
         "serial_eper": ac.Array2D.full(
             shape_native=(7, 7), fill_value=2.0, pixel_scales=(1.0, 1.0)
         ),
     }
 
 
 ### LINE DATASET FITS ###
 
 
-def make_fit_line_7():
+def make_fit_1d_7():
     return ac.FitDataset1D(
         dataset=make_dataset_1d_7(), post_cti_data=make_dataset_1d_7().pre_cti_data + 1
     )
 
 
 ### CHARGE INJECTION IMAGING ###
 
 
 def make_imaging_ci_7x7():
-
     return ac.ImagingCI(
-        image=make_ci_image_7x7(),
+        data=make_ci_image_7x7(),
         noise_map=make_ci_noise_map_7x7(),
         pre_cti_data=make_pre_cti_data_7x7(),
         cosmic_ray_map=make_ci_cosmic_ray_map_7x7(),
         noise_scaling_map_dict=make_ci_noise_scaling_map_dict_7x7(),
         layout=make_layout_ci_7x7(),
     )
 
@@ -206,15 +203,14 @@
     )
 
 
 # ### PHASES ###
 
 
 def make_samples_with_result():
-
     model = af.Collection(
         cti=af.Model(
             ac.CTI2D,
             parallel_trap_list=[ac.TrapInstantCapture],
             parallel_ccd=make_ccd(),
             serial_trap_list=[ac.TrapInstantCapture],
             serial_ccd=make_ccd(),
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/acs/acs_util.py` & `autocti-2023.7.7.2/autocti/instruments/acs/acs_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 
 logging.basicConfig()
 logger = logging.getLogger()
 logger.setLevel("INFO")
 
 
 def fits_hdu_via_quadrant_letter_from(quadrant_letter):
-
     if quadrant_letter == "D" or quadrant_letter == "C":
         return 1
     elif quadrant_letter == "B" or quadrant_letter == "A":
         return 4
     else:
         raise exc.ArrayException("Quadrant letter for FrameACS must be A, B, C or D.")
 
 
 def array_eps_to_counts(array_eps, bscale, bzero):
-
     if bscale is None:
         raise exc.ArrayException(
             "Cannot convert a Frame2D to units COUNTS without a bscale attribute (bscale = None)."
         )
 
     return (array_eps - bzero) / bscale
 
@@ -87,15 +85,14 @@
     quadrant_d,
     header_a=None,
     header_b=None,
     header_c=None,
     header_d=None,
     overwrite: bool = False,
 ):
-
     file_dir = os.path.split(file_path)[0]
 
     if not os.path.exists(file_dir):
         os.makedirs(file_dir)
 
     if overwrite and os.path.exists(file_path):
         os.remove(file_path)
@@ -171,15 +168,14 @@
     hdu_list[4].header = set_header(header_a.header_hdu_obj)
     hdu_list.writeto(file_path)
 
 
 def quadrant_convert_to_original(
     quadrant, roe_corner, header, use_flipud=False, use_calibrated_gain=True
 ):
-
     if header.bias is not None:
         quadrant += header.bias.native
 
     if header.bias_serial_prescan_column is not None:
         quadrant += header.bias_serial_prescan_column
 
     quadrant = header.array_electrons_to_original(
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/acs/array_2d.py` & `autocti-2023.7.7.2/autocti/instruments/acs/array_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,43 +74,39 @@
 
         See the docstring of the `FrameACS` class for a complete description of the HST FPA, quadrants and
         rotations.
 
         Also see https://github.com/spacetelescope/hstcal/blob/main/pkg/acs/calacs/acscte/dopcte-gen2.c#L418
         """
         if quadrant_letter == "A":
-
             array_electrons = array_electrons[0:2068, 0:2072]
             roe_corner = (1, 0)
             use_flipud = True
 
             if bias is not None:
                 bias = bias[0:2068, 0:2072]
 
         elif quadrant_letter == "B":
-
             array_electrons = array_electrons[0:2068, 2072:4144]
             roe_corner = (1, 1)
             use_flipud = True
 
             if bias is not None:
                 bias = bias[0:2068, 2072:4144]
 
         elif quadrant_letter == "C":
-
             array_electrons = array_electrons[0:2068, 0:2072]
 
             roe_corner = (1, 0)
             use_flipud = False
 
             if bias is not None:
                 bias = bias[0:2068, 0:2072]
 
         elif quadrant_letter == "D":
-
             array_electrons = array_electrons[0:2068, 2072:4144]
 
             roe_corner = (1, 1)
             use_flipud = False
 
             if bias is not None:
                 bias = bias[0:2068, 2072:4144]
@@ -153,25 +149,23 @@
             array=array_electrons, roe_corner=roe_corner
         )
 
         if use_flipud:
             array_electrons = np.flipud(array_electrons)
 
         if bias_subtract_via_prescan:
-
             bias_serial_prescan_value = acs_util.prescan_fitted_bias_column(
                 array_electrons[:, 18:24]
             )
 
             array_electrons -= bias_serial_prescan_value
 
             header.bias_serial_prescan_column = bias_serial_prescan_value
 
         if bias is not None:
-
             bias = layout_util.rotate_array_via_roe_corner_from(
                 array=bias, roe_corner=roe_corner
             )
 
             if use_flipud:
                 bias = np.flipud(bias)
 
@@ -198,25 +192,23 @@
         array_electrons = layout_util.rotate_array_via_roe_corner_from(
             array=array_electrons, roe_corner=(1, 1)
         )
 
         array_electrons = np.flipud(array_electrons)
 
         if bias_subtract_via_prescan:
-
             bias_serial_prescan_value = acs_util.prescan_fitted_bias_column(
                 array_electrons[:, 18:24]
             )
 
             array_electrons -= bias_serial_prescan_value
 
             header.bias_serial_prescan_column = bias_serial_prescan_value
 
         if bias is not None:
-
             bias = layout_util.rotate_array_via_roe_corner_from(
                 array=bias, roe_corner=(1, 1)
             )
 
             bias = np.flipud(bias)
 
             array_electrons -= bias
@@ -240,25 +232,23 @@
         """
 
         array_electrons = layout_util.rotate_array_via_roe_corner_from(
             array=array_electrons, roe_corner=(1, 0)
         )
 
         if bias_subtract_via_prescan:
-
             bias_serial_prescan_value = acs_util.prescan_fitted_bias_column(
                 array_electrons[:, 18:24]
             )
 
             array_electrons -= bias_serial_prescan_value
 
             header.bias_serial_prescan_column = bias_serial_prescan_value
 
         if bias is not None:
-
             bias = layout_util.rotate_array_via_roe_corner_from(
                 array=bias, roe_corner=(1, 0)
             )
 
             array_electrons -= bias
 
             header.bias = Array2DACS.no_mask(values=bias, pixel_scales=0.05)
@@ -289,15 +279,14 @@
             )
 
             array_electrons -= bias_serial_prescan_value
 
             header.bias_serial_prescan_column = bias_serial_prescan_value
 
         if bias is not None:
-
             bias = layout_util.rotate_array_via_roe_corner_from(
                 array=bias, roe_corner=(1, 1)
             )
 
             array_electrons -= bias
 
             header.bias = Array2DACS.no_mask(values=bias, pixel_scales=0.05)
@@ -314,19 +303,17 @@
             The path the file is output to, including the filename and the ``.fits`` extension,
             e.g. '/path/to/filename.fits'
         """
 
         new_file_dir = os.path.split(new_file_path)[0]
 
         if not os.path.exists(new_file_dir):
-
             os.makedirs(new_file_dir)
 
         if not os.path.exists(new_file_path):
-
             shutil.copy(original_file_path, new_file_path)
 
         hdulist = fits.open(new_file_path)
 
         hdulist[self.header.hdu].data = self.layout_2d.original_orientation_from(
             array=self
         )
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/acs/header.py` & `autocti-2023.7.7.2/autocti/instruments/acs/header.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         header_sci_obj,
         header_hdu_obj,
         quadrant_letter=None,
         hdu=None,
         bias=None,
         bias_serial_prescan_column=None,
     ):
-
         super().__init__(header_sci_obj=header_sci_obj, header_hdu_obj=header_hdu_obj)
 
         self.bias = bias
         self.bias_serial_prescan_column = bias_serial_prescan_column
         self.quadrant_letter = quadrant_letter
         self.hdu = hdu
 
@@ -39,15 +38,14 @@
 
     @property
     def gain(self):
         return self.header_sci_obj["CCDGAIN"]
 
     @property
     def calibrated_gain(self):
-
         if round(self.gain) == 1:
             calibrated_gain = [0.99989998, 0.97210002, 1.01070000, 1.01800000]
         elif round(self.gain) == 2:
             calibrated_gain = [2.002, 1.945, 2.028, 1.994]
         elif round(self.gain) == 4:
             calibrated_gain = [4.011, 3.902, 4.074, 3.996]
         else:
@@ -74,27 +72,25 @@
 
     def array_eps_to_counts(self, array_eps):
         return acs_util.array_eps_to_counts(
             array_eps=array_eps, bscale=self.bscale, bzero=self.bzero
         )
 
     def array_original_to_electrons(self, array, use_calibrated_gain):
-
         if self.original_units in "COUNTS":
             array = (array * self.bscale) + self.bzero
         elif self.original_units in "CPS":
             array = (array * self.exposure_time * self.bscale) + self.bzero
 
         if use_calibrated_gain:
             return array * self.calibrated_gain
         else:
             return array * self.gain
 
     def array_electrons_to_original(self, array, use_calibrated_gain):
-
         if use_calibrated_gain:
             array /= self.calibrated_gain
         else:
             array /= self.gain
 
         if self.original_units in "COUNTS":
             return (array - self.bzero) / self.bscale
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/acs/image.py` & `autocti-2023.7.7.2/autocti/instruments/acs/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,15 @@
         )
 
         array = header.array_original_to_electrons(
             array=array, use_calibrated_gain=use_calibrated_gain
         )
 
         if bias_subtract_via_bias_file:
-
             if bias_file_path is None:
-
                 file_dir = os.path.split(file_path)[0]
                 bias_file_path = path.join(file_dir, header.bias_file)
 
             bias = array_2d_util.numpy_array_2d_via_fits_from(
                 file_path=bias_file_path, hdu=hdu, do_not_scale_image_data=True
             )
 
@@ -114,21 +112,19 @@
                 header_sci_obj=header_sci_obj,
                 header_hdu_obj=header_hdu_obj,
                 hdu=hdu,
                 quadrant_letter=quadrant_letter,
             )
 
             if bias_header.original_units != "COUNTS":
-
                 raise exc.ArrayException("Cannot use bias frame not in counts.")
 
             bias = bias * bias_header.calibrated_gain
 
         else:
-
             bias = None
 
         return cls.from_ccd(
             array_electrons=array,
             quadrant_letter=quadrant_letter,
             header=header,
             bias_subtract_via_prescan=bias_subtract_via_prescan,
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/acs/layout.py` & `autocti-2023.7.7.2/autocti/instruments/acs/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/instruments/euclid/array_2d.py` & `autocti-2023.7.7.2/autocti/instruments/euclid/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/instruments/euclid/euclid_util.py` & `autocti-2023.7.7.2/autocti/instruments/euclid/euclid_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def roe_corner_from(ccd_id, quadrant_id):
-
     row_index = ccd_id[-1]
 
     if (row_index in "123") and (quadrant_id == "E"):
         return (1, 0)
     elif (row_index in "123") and (quadrant_id == "F"):
         return (1, 1)
     elif (row_index in "123") and (quadrant_id == "G"):
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/euclid/header.py` & `autocti-2023.7.7.2/autocti/instruments/euclid/header.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         header_sci_obj: Dict = None,
         header_hdu_obj: Dict = None,
         original_roe_corner: Tuple[int, int] = None,
         readout_offsets: Optional[Tuple] = None,
         ccd_id: Optional[str] = None,
         quadrant_id: Optional[str] = None,
     ):
-
         super().__init__(
             header_sci_obj=header_sci_obj,
             header_hdu_obj=header_hdu_obj,
             original_roe_corner=original_roe_corner,
             readout_offsets=readout_offsets,
         )
```

### Comparing `autocti-2023.1.15.1/autocti/instruments/euclid/layout.py` & `autocti-2023.7.7.2/autocti/instruments/euclid/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,24 @@
             clocking.
         ccd_id
             The ID of the euclid CCD (1, 2, 3, 4, 5, or 6) indicating which half of the FP the CCD is in.
         quadrant_id
             The ID of the quadrant (E, G, F or H).
         """
         if parallel_overscan_size > 0:
-
             parallel_overscan = Region2D(
                 (
                     0,
                     parallel_overscan_size,
                     serial_prescan_size,
                     serial_size - serial_overscan_size,
                 )
             )
 
         else:
-
             parallel_overscan = None
 
         serial_prescan = Region2D((0, parallel_size, 0, serial_prescan_size))
         serial_overscan = Region2D(
             (
                 0,
                 parallel_size - parallel_overscan_size,
@@ -234,26 +232,24 @@
             The size (number of pixels) of the serial prescan.
         serial_overscan_size
             The size (number of pixels) of the serial overscan.
         parallel_overscan_size
             The size (number of pixels) of the parallel overscan.
         """
         if parallel_overscan_size > 0:
-
             parallel_overscan = Region2D(
                 (
                     0,
                     parallel_overscan_size,
                     serial_overscan_size,
                     serial_size - serial_prescan_size,
                 )
             )
 
         else:
-
             parallel_overscan = None
 
         serial_prescan = Region2D(
             (0, parallel_size, serial_size - serial_prescan_size, serial_size)
         )
         serial_overscan = Region2D(
             (0, parallel_size - parallel_overscan_size, 0, serial_overscan_size)
@@ -308,26 +304,24 @@
             The size (number of pixels) of the serial prescan.
         serial_overscan_size
             The size (number of pixels) of the serial overscan.
         parallel_overscan_size
             The size (number of pixels) of the parallel overscan.
         """
         if parallel_overscan_size > 0:
-
             parallel_overscan = Region2D(
                 (
                     parallel_size - parallel_overscan_size,
                     parallel_size,
                     serial_prescan_size,
                     serial_size - serial_overscan_size,
                 )
             )
 
         else:
-
             parallel_overscan = None
 
         serial_prescan = Region2D((0, parallel_size, 0, serial_prescan_size))
         serial_overscan = Region2D(
             (
                 0,
                 parallel_size - parallel_overscan_size,
@@ -386,26 +380,24 @@
             The size (number of pixels) of the serial prescan.
         serial_overscan_size
             The size (number of pixels) of the serial overscan.
         parallel_overscan_size
             The size (number of pixels) of the parallel overscan.
         """
         if parallel_overscan_size > 0:
-
             parallel_overscan = Region2D(
                 (
                     parallel_size - parallel_overscan_size,
                     parallel_size,
                     serial_overscan_size,
                     serial_size - serial_prescan_size,
                 )
             )
 
         else:
-
             parallel_overscan = None
 
         serial_prescan = Region2D(
             (0, parallel_size, serial_size - serial_prescan_size, serial_size)
         )
         serial_overscan = Region2D(
             (0, parallel_size - parallel_overscan_size, 0, serial_overscan_size)
```

### Comparing `autocti-2023.1.15.1/autocti/layout/one_d.py` & `autocti-2023.7.7.2/autocti/layout/one_d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
-from typing import Tuple
+from typing import Optional, Tuple
 
 import autoarray as aa
 
+from autocti.extract.settings import SettingsExtract
 from autocti import exc
 
 
 class Layout1D(aa.Layout1D):
     def __init__(
         self,
         shape_1d: Tuple[int],
@@ -24,53 +25,57 @@
             A list of the integer coordinates specifying the corners of each charge injection region \
             (top-row, bottom-row, left-column, right-column).
         """
 
         self.region_list = list(map(aa.Region1D, region_list))
 
         for region in self.region_list:
-
             if region.x1 > shape_1d[0]:
                 raise exc.LayoutException(
                     "The charge injection layout_ci regions are bigger than the image image_shape"
                 )
 
         from autocti.extract.one_d.master import Extract1DMaster
 
         self.extract = Extract1DMaster(
-            region_list=region_list, prescan=prescan, overscan=overscan
+            shape_1d=shape_1d,
+            region_list=region_list,
+            prescan=prescan,
+            overscan=overscan,
         )
 
         super().__init__(shape_1d=shape_1d, prescan=prescan, overscan=overscan)
 
     @property
-    def pixels_between_regions(self):
-        return [
-            self.region_list[i + 1].x0 - self.region_list[i].x1
-            for i in range(len(self.region_list) - 1)
-        ]
+    def parallel_rows_between_regions(self):
+        return self.extract.fpr.parallel_rows_between_regions
 
     @property
     def trail_size_to_array_edge(self):
-        return self.shape_1d[0] - np.max([region.x1 for region in self.region_list])
+        return self.extract.fpr.trail_size_to_array_edge
 
     @property
     def smallest_eper_pixels_to_array_edge(self):
-
-        pixels_between_regions = self.pixels_between_regions
-        pixels_between_regions.append(self.trail_size_to_array_edge)
-        return np.min(pixels_between_regions)
-
-    def extract_region_from(self, array: aa.Array1D, region: str):
+        parallel_rows_between_regions = self.parallel_rows_between_regions
+        parallel_rows_between_regions.append(self.trail_size_to_array_edge)
+        return np.min(parallel_rows_between_regions)
+
+    def extract_region_from(self, array: aa.Array1D, region: Optional):
+        if region is None:
+            return array
 
         if region == "fpr":
             return self.extract.fpr.stacked_array_1d_from(
-                array=array, pixels=(0, self.extract.fpr.total_pixels_min)
+                array=array,
+                settings=SettingsExtract(pixels=(0, self.extract.fpr.total_pixels_min)),
             )
         elif region == "eper":
             return self.extract.eper.stacked_array_1d_from(
-                array=array, pixels=(0, self.smallest_eper_pixels_to_array_edge)
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.smallest_eper_pixels_to_array_edge)
+                ),
             )
         else:
             raise exc.PlottingException(
                 "The line region specified for the plotting of a line was invalid"
             )
```

### Comparing `autocti-2023.1.15.1/autocti/layout/two_d.py` & `autocti-2023.7.7.2/autocti/layout/two_d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from copy import deepcopy
 import numpy as np
 from typing import List, Optional, Tuple
 
 import autoarray as aa
 
+from autocti.extract.settings import SettingsExtract
+
 from autocti import exc
 
 
 class Layout2D(aa.Layout2D):
     def __init__(
         self,
         shape_2d: Tuple[int, int],
@@ -45,15 +47,14 @@
         electronics
             The charge injection electronics parameters of the image (e.g. the IG1 and IG2 voltages).
         """
 
         self.region_list = list(map(aa.Region2D, region_list))
 
         for region in self.region_list:
-
             if region.y1 > shape_2d[0] or region.x1 > shape_2d[1]:
                 raise exc.LayoutException(
                     "The charge injection layout_ci regions are bigger than the image image_shape"
                 )
 
         super().__init__(
             shape_2d=shape_2d,
@@ -61,15 +62,14 @@
             parallel_overscan=parallel_overscan,
             serial_prescan=serial_prescan,
             serial_overscan=serial_overscan,
         )
 
     @property
     def extract(self):
-
         from autocti.extract.two_d.master import Extract2DMaster
 
         return Extract2DMaster(
             shape_2d=self.shape_2d,
             region_list=self.region_list,
             parallel_overscan=self.parallel_overscan,
             serial_prescan=self.serial_prescan,
@@ -110,49 +110,63 @@
             region_list=region_list,
             parallel_overscan=layout.parallel_overscan,
             serial_prescan=layout.serial_prescan,
             serial_overscan=layout.serial_overscan,
         )
 
     @property
-    def pixels_between_regions(self) -> List[int]:
+    def parallel_rows_between_regions(self) -> List[int]:
         """
         Returns a list where each entry is the number of pixels a charge injection region and its neighboring
         charge injection region.
         """
-        return [
-            self.region_list[i + 1].y0 - self.region_list[i].y1
-            for i in range(len(self.region_list) - 1)
-        ]
+        return self.extract.parallel_fpr.parallel_rows_between_regions
+
+    @property
+    def parallel_rows_within_regions(self) -> List[int]:
+        """
+        Returns a list where each entry is the number of pixels a charge injection region and its neighboring
+        charge injection region.
+        """
+        return [region.y1 - region.y0 for region in self.region_list]
 
     @property
     def parallel_rows_to_array_edge(self) -> int:
         """
         The number of pixels from the edge of the parallel EPERs to the edge of the array.
 
         This is the number of pixels from the last charge injection FPR edge to the read out register and electronics
         and will include the parallel overscan if the CCD has one.
         """
-        return self.shape_2d[0] - np.max([region.y1 for region in self.region_list])
+        return self.extract.parallel_fpr.parallel_rows_to_array_edge
 
     @property
     def smallest_parallel_rows_between_ci_regions(self) -> int:
         """
         The smallest number of pixels between any two charge injection regions, or the distance of the last
         charge injection region to the edge of the charge injeciton image (e.g. in the direction away from the
         readout register and electronics).
         """
-        pixels_between_regions = self.pixels_between_regions
-        pixels_between_regions.append(self.parallel_rows_to_array_edge)
-        return np.min(pixels_between_regions)
+        parallel_rows_between_regions = self.parallel_rows_between_regions
+        parallel_rows_between_regions.append(self.parallel_rows_to_array_edge)
+        return np.min(parallel_rows_between_regions)
+
+    @property
+    def smallest_parallel_rows_within_ci_regions(self) -> int:
+        """
+        The smallest number of pixels within any of the charge injection regions.
+
+        This can be used to extract the FPR of each charge injection region using a
+        number of pixels which does not exceed the size of any.
+        """
+        return np.min(self.parallel_rows_within_regions)
 
     def with_extracted_regions(
         self, extraction_region: aa.type.Region2DLike
     ) -> "Layout2D":
-
         layout = deepcopy(self)
 
         extracted_region_list = list(
             map(
                 lambda region: aa.util.layout.region_after_extraction(
                     original_region=region, extraction_region=extraction_region
                 ),
@@ -163,28 +177,105 @@
         if not extracted_region_list:
             extracted_region_list = None
 
         layout.region_list = extracted_region_list
         return layout
 
     def extract_region_from(self, array: aa.Array2D, region: str) -> aa.Array1D:
-
         if region == "parallel_fpr":
             return self.extract.parallel_fpr.binned_array_1d_from(
-                array=array, pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                ),
             )
         elif region == "parallel_eper":
             return self.extract.parallel_eper.binned_array_1d_from(
-                array=array, pixels=(0, self.smallest_parallel_rows_between_ci_regions)
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.smallest_parallel_rows_between_ci_regions)
+                ),
             )
-        elif region == "serial_fpr":
+        elif region == "serial_fpr" or region == "fpr_non_uniformity":
             return self.extract.serial_fpr.binned_array_1d_from(
-                array=array, pixels=(0, self.extract.serial_fpr.total_columns_min)
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.serial_fpr.total_columns_min)
+                ),
             )
         elif region == "serial_eper":
             return self.extract.serial_eper.binned_array_1d_from(
-                array=array, pixels=(0, self.serial_eper_pixels)
+                array=array,
+                settings=SettingsExtract(pixels=(0, self.serial_eper_pixels)),
             )
         else:
             raise exc.PlottingException(
                 "The line region specified for the plotting of a line was invalid"
             )
+
+    def extract_region_noise_map_from(
+        self, array: aa.Array2D, region: str
+    ) -> aa.Array1D:
+        if region == "parallel_fpr":
+            binned_noise_map_1d = self.extract.parallel_fpr.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                ),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.parallel_fpr.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(
+                        pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                    ),
+                )
+            )
+        elif region == "parallel_eper":
+            binned_noise_map_1d = self.extract.parallel_eper.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.smallest_parallel_rows_between_ci_regions)
+                ),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.parallel_eper.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(
+                        pixels=(0, self.smallest_parallel_rows_between_ci_regions),
+                    ),
+                )
+            )
+        elif region == "serial_fpr" or region == "fpr_non_uniformity":
+            binned_noise_map_1d = self.extract.serial_fpr.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.serial_fpr.total_columns_min)
+                ),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.serial_fpr.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(
+                        pixels=(0, self.extract.serial_fpr.total_columns_min)
+                    ),
+                )
+            )
+        elif region == "serial_eper":
+            binned_noise_map_1d = self.extract.serial_eper.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(pixels=(0, self.serial_eper_pixels)),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.serial_eper.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(pixels=(0, self.serial_eper_pixels)),
+                )
+            )
+        else:
+            raise exc.PlottingException(
+                "The line region specified for the plotting of a line was invalid"
+            )
+
+        binned_noise_map_1d /= np.sqrt(binned_noise_map_1d_total_pixels)
+
+        return binned_noise_map_1d
```

### Comparing `autocti-2023.1.15.1/autocti/mask/mask_1d.py` & `autocti-2023.7.7.2/autocti/mask/mask_1d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import numpy as np
 from typing import Optional, Tuple
 
 import autoarray as aa
 
 from autocti.layout.one_d import Layout1D
+from autocti.extract.settings import SettingsExtract
 
 
 class SettingsMask1D:
     def __init__(
         self,
         fpr_pixels: Optional[Tuple[int, int]] = None,
         eper_pixels: Optional[Tuple[int, int]] = None,
     ):
-
         self.fpr_pixels = fpr_pixels
         self.eper_pixels = eper_pixels
 
 
 class Mask1D(aa.Mask1D):
     @classmethod
     def masked_fpr_and_eper_from(
         cls,
         mask: "Mask1D",
         layout: Layout1D,
         settings: "SettingsMask1D",
         pixel_scales: aa.type.PixelScales,
     ) -> "Mask1D":
-
         if settings.fpr_pixels is not None:
-
             fpr_mask = cls.masked_fpr_from_layout(
                 layout=layout, settings=settings, pixel_scales=pixel_scales
             )
 
             mask = mask + fpr_mask
 
         if settings.eper_pixels is not None:
-
             eper_mask = cls.masked_eper_from_layout(
                 layout=layout, settings=settings, pixel_scales=pixel_scales
             )
 
             mask = mask + eper_mask
 
         return mask
@@ -49,16 +46,17 @@
     def masked_fpr_from_layout(
         cls,
         layout: Layout1D,
         settings: "SettingsMask1D",
         pixel_scales: aa.type.PixelScales,
         invert: bool = False,
     ) -> "Mask1D":
-
-        fpr_regions = layout.extract.fpr.region_list_from(pixels=settings.fpr_pixels)
+        fpr_regions = layout.extract.fpr.region_list_from(
+            settings=SettingsExtract(pixels=settings.fpr_pixels)
+        )
 
         mask = np.full(layout.shape_1d, False)
 
         for region in fpr_regions:
             mask[region.x0 : region.x1] = True
 
         if invert:
@@ -70,16 +68,17 @@
     def masked_eper_from_layout(
         cls,
         layout: Layout1D,
         settings: "SettingsMask1D",
         pixel_scales: aa.type.PixelScales,
         invert: bool = False,
     ) -> "Mask1D":
-
-        eper_regions = layout.extract.eper.region_list_from(pixels=settings.eper_pixels)
+        eper_regions = layout.extract.eper.region_list_from(
+            settings=SettingsExtract(pixels=settings.eper_pixels)
+        )
 
         mask = np.full(layout.shape_1d, False)
 
         for region in eper_regions:
             mask[region.x0 : region.x1] = True
 
         if invert:
```

### Comparing `autocti-2023.1.15.1/autocti/mask/mask_2d.py` & `autocti-2023.7.7.2/autocti/mask/mask_2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import numpy as np
 from typing import Tuple
 
 import autoarray as aa
 
 from autoarray import exc
 
+from autocti.extract.settings import SettingsExtract
 from autocti.layout.two_d import Layout2D
 
+
 class SettingsMask2D:
     def __init__(
         self,
         parallel_fpr_pixels: Tuple[int, int] = None,
         parallel_eper_pixels: Tuple[int, int] = None,
         serial_fpr_pixels: Tuple[int, int] = None,
         serial_eper_pixels: Tuple[int, int] = None,
         cosmic_ray_parallel_buffer: int = 10,
         cosmic_ray_serial_buffer: int = 10,
         cosmic_ray_diagonal_buffer: int = 3,
     ):
-
         self.parallel_fpr_pixels = parallel_fpr_pixels
         self.parallel_eper_pixels = parallel_eper_pixels
         self.serial_fpr_pixels = serial_fpr_pixels
         self.serial_eper_pixels = serial_eper_pixels
 
         self.cosmic_ray_parallel_buffer = cosmic_ray_parallel_buffer
         self.cosmic_ray_serial_buffer = cosmic_ray_serial_buffer
@@ -93,15 +94,14 @@
             pixel_scales=pixel_scales,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def from_masked_regions(cls, shape_native, pixel_scales, masked_regions):
-
         mask = cls.all_false(shape_native=shape_native, pixel_scales=pixel_scales)
         masked_regions = list(
             map(lambda region: aa.Region2D(region=region), masked_regions)
         )
         for region in masked_regions:
             mask[region.y0 : region.y1, region.x0 : region.x1] = True
 
@@ -129,15 +129,14 @@
         )
 
         cosmic_ray_mask = (cosmic_ray_map.native > 0.0).astype("bool")
 
         for y in range(mask.shape[0]):
             for x in range(mask.shape[1]):
                 if cosmic_ray_mask[y, x]:
-
                     x0 = int(x)
 
                     y0 = y
                     y1 = y + 1 + settings.cosmic_ray_parallel_buffer
 
                     y1 = mask.shape[0] if y1 > mask.shape[0] else y1
 
@@ -198,41 +197,36 @@
     def masked_fpr_and_eper_from(
         cls,
         mask: "Mask2D",
         layout: Layout2D,
         settings: "SettingsMask2D",
         pixel_scales: aa.type.PixelScales,
     ) -> "Mask2D":
-
         if settings.parallel_fpr_pixels is not None:
-
             parallel_fpr_mask = cls.masked_parallel_fpr_from(
                 layout=layout, settings=settings, pixel_scales=pixel_scales
             )
 
             mask = mask + parallel_fpr_mask
 
         if settings.parallel_eper_pixels is not None:
-
             parallel_eper_mask = cls.masked_parallel_eper_from(
                 layout=layout, settings=settings, pixel_scales=pixel_scales
             )
 
             mask = mask + parallel_eper_mask
 
         if settings.serial_fpr_pixels is not None:
-
             serial_fpr_mask = cls.masked_serial_fpr_from(
                 layout=layout, settings=settings, pixel_scales=pixel_scales
             )
 
             mask = mask + serial_fpr_mask
 
         if settings.serial_eper_pixels is not None:
-
             serial_eper_mask = cls.masked_serial_eper_from(
                 layout=layout, settings=settings, pixel_scales=pixel_scales
             )
 
             mask = mask + serial_eper_mask
 
         return mask
@@ -241,17 +235,16 @@
     def masked_parallel_fpr_from(
         cls,
         layout: Layout2D,
         settings: "SettingsMask2D",
         pixel_scales: aa.type.PixelScales,
         invert: bool = False,
     ) -> "Mask2D":
-
         fpr_regions = layout.extract.parallel_fpr.region_list_from(
-            pixels=settings.parallel_fpr_pixels
+            settings=SettingsExtract(pixels=settings.parallel_fpr_pixels)
         )
         mask = np.full(layout.shape_2d, False)
 
         for region in fpr_regions:
             mask[region.y0 : region.y1, region.x0 : region.x1] = True
 
         if invert:
@@ -263,17 +256,16 @@
     def masked_parallel_eper_from(
         cls,
         layout: Layout2D,
         settings: "SettingsMask2D",
         pixel_scales: aa.type.PixelScales,
         invert: bool = False,
     ) -> "Mask2D":
-
         eper_regions = layout.extract.parallel_eper.region_list_from(
-            pixels=settings.parallel_eper_pixels
+            settings=SettingsExtract(pixels=settings.parallel_eper_pixels)
         )
 
         mask = np.full(layout.shape_2d, False)
 
         for region in eper_regions:
             mask[region.y0 : region.y1, region.x0 : region.x1] = True
 
@@ -286,17 +278,16 @@
     def masked_serial_fpr_from(
         cls,
         layout: Layout2D,
         settings: "SettingsMask2D",
         pixel_scales: aa.type.PixelScales,
         invert: bool = False,
     ) -> "Mask2D":
-
         fpr_regions = layout.extract.serial_fpr.region_list_from(
-            pixels=settings.serial_fpr_pixels
+            settings=SettingsExtract(pixels=settings.serial_fpr_pixels)
         )
         mask = np.full(layout.shape_2d, False)
 
         for region in fpr_regions:
             mask[region.y0 : region.y1, region.x0 : region.x1] = True
 
         if invert:
@@ -308,17 +299,16 @@
     def masked_serial_eper_from(
         cls,
         layout: Layout2D,
         settings: "SettingsMask2D",
         pixel_scales: aa.type.PixelScales,
         invert: bool = False,
     ) -> "Mask2D":
-
         eper_regions = layout.extract.serial_eper.region_list_from(
-            pixels=settings.serial_eper_pixels
+            settings=SettingsExtract(pixels=settings.serial_eper_pixels)
         )
         mask = np.full(layout.shape_2d, False)
 
         for region in eper_regions:
             mask[region.y0 : region.y1, region.x0 : region.x1] = True
 
         if invert:
```

### Comparing `autocti-2023.1.15.1/autocti/model/model_util.py` & `autocti-2023.7.7.2/autocti/model/model_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/model/result.py` & `autocti-2023.7.7.2/autocti/model/result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/model/settings.py` & `autocti-2023.7.7.2/autocti/model/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,47 +5,42 @@
 from autocti import exc
 
 
 class AbstractSettingsCTI:
     def check_total_density_within_range_of_traps(
         self, total_density_range: Tuple[float, float], traps: List[TrapInstantCapture]
     ):
-
         if total_density_range is not None:
-
             total_density = sum([trap.density for trap in traps])
 
             if (
                 total_density < total_density_range[0]
                 or total_density > total_density_range[1]
             ):
                 raise exc.PriorException
 
 
 class SettingsCTI1D(AbstractSettingsCTI):
     def __init__(self, total_density_range=None):
         self.total_density_range = total_density_range
 
     def check_total_density_within_range(self, traps):
-
         self.check_total_density_within_range_of_traps(
             total_density_range=self.total_density_range, traps=traps
         )
 
 
 class SettingsCTI2D(AbstractSettingsCTI):
     def __init__(
         self, parallel_total_density_range=None, serial_total_density_range=None
     ):
-
         self.parallel_total_density_range = parallel_total_density_range
         self.serial_total_density_range = serial_total_density_range
 
     def check_total_density_within_range(self, parallel_traps, serial_traps):
-
         self.check_total_density_within_range_of_traps(
             total_density_range=self.parallel_total_density_range, traps=parallel_traps
         )
 
         self.check_total_density_within_range_of_traps(
             total_density_range=self.serial_total_density_range, traps=serial_traps
         )
```

### Comparing `autocti-2023.1.15.1/autocti/model/visualizer.py` & `autocti-2023.7.7.2/autocti/model/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 def plot_setting(section, name):
     return setting(section, name)
 
 
 class Visualizer:
     def __init__(self, visualize_path):
-
         self.visualize_path = visualize_path
 
         self.include_1d = Include1D()
         self.include_2d = Include2D()
 
     def mat_plot_1d_from(self, subfolders, format="png"):
         return MatPlot1D(
```

### Comparing `autocti-2023.1.15.1/autocti/plot/__init__.py` & `autocti-2023.7.7.2/autocti/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/plot/get_visuals/one_d.py` & `autocti-2023.7.7.2/autocti/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/plot/get_visuals/two_d.py` & `autocti-2023.7.7.2/autocti/plot/get_visuals/two_d.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,21 +50,21 @@
         -------
         Visuals2D
             The collection of attributes that are plotted by a `Plotter` object.
         """
         visuals_2d_via_fit = super().via_fit_imaging_from(fit=fit)
 
         parallel_overscan = (
-            self.get("parallel_overscan", fit.imaging_ci.layout.parallel_overscan),
+            self.get("parallel_overscan", fit.dataset.layout.parallel_overscan),
         )
         serial_prescan = (
-            self.get("serial_prescan", fit.imaging_ci.layout.serial_prescan),
+            self.get("serial_prescan", fit.dataset.layout.serial_prescan),
         )
         serial_overscan = (
-            self.get("serial_overscan", fit.imaging_ci.layout.serial_overscan),
+            self.get("serial_overscan", fit.dataset.layout.serial_overscan),
         )
 
         return visuals_2d_via_fit + self.visuals.__class__(
             parallel_overscan=parallel_overscan,
             serial_prescan=serial_prescan,
             serial_overscan=serial_overscan,
         )
```

### Comparing `autocti-2023.1.15.1/autocti/preloads.py` & `autocti-2023.7.7.2/autocti/preloads.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/autocti/util/__init__.py` & `autocti-2023.7.7.2/autocti/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.1.15.1/setup.py` & `autocti-2023.7.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2023.7.7.2")
 requirements.extend(
     [f"autoconf=={version}", f"autofit=={version}", f"autoarray=={version}"]
 )
 
 setup(
     name="autocti",
     version=version,
@@ -34,14 +34,14 @@
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires='>=3.7',
+    python_requires=">=3.7",
     keywords="cli",
     packages=find_packages(exclude=["docs", "test_autocti", "test_autocti*"]),
     install_requires=requirements,
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
 )
```

