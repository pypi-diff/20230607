# Comparing `tmp/autogalaxy-2023.3.27.1.tar.gz` & `tmp/autogalaxy-2023.7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogalaxy-2023.3.27.1.tar", last modified: Mon Mar 27 14:48:38 2023, max compression
+gzip compressed data, was "autogalaxy-2023.7.7.1.tar", last modified: Wed Jun  7 09:47:58 2023, max compression
```

## Comparing `autogalaxy-2023.3.27.1.tar` & `autogalaxy-2023.7.7.1.tar`

### file list

```diff
@@ -1,499 +1,498 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.759038 autogalaxy-2023.3.27.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.869996 autogalaxy-2023.3.27.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.933567 autogalaxy-2023.3.27.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/.github/workflows/draft-pdf.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3327 2022-12-19 16:37:19.000000 autogalaxy-2023.3.27.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1135 2022-12-19 11:17:33.000000 autogalaxy-2023.3.27.1/CITATIONS.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18987 2022-12-20 20:59:49.000000 autogalaxy-2023.3.27.1/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2494 2022-12-20 20:59:49.000000 autogalaxy-2023.3.27.1/CONTRIBUTING.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2020-11-16 19:58:12.000000 autogalaxy-2023.3.27.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8384 2023-03-27 14:48:38.759038 autogalaxy-2023.3.27.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7550 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.942567 autogalaxy-2023.3.27.1/autogalaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5589 2023-03-27 14:42:00.000000 autogalaxy-2023.3.27.1/autogalaxy/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7847 2023-02-20 18:45:51.000000 autogalaxy-2023.3.27.1/autogalaxy/abstract_fit.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.954153 autogalaxy-2023.3.27.1/autogalaxy/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      308 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6998 2022-12-20 16:11:48.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4802 2022-12-20 16:11:48.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4623 2022-12-20 16:11:48.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2747 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2960 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2778 2022-12-20 16:11:48.000000 autogalaxy-2023.3.27.1/autogalaxy/aggregator/plane.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.968258 autogalaxy-2023.3.27.1/autogalaxy/analysis/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-21 09:36:45.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20675 2023-03-18 15:50:23.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6453 2023-03-24 18:01:21.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/clump_model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5035 2023-03-18 15:50:23.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/maker.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.972858 autogalaxy-2023.3.27.1/autogalaxy/analysis/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3240 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/mock/mock_result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26894 2023-03-18 15:50:53.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/model_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11609 2023-02-13 11:16:26.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/preloads.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6646 2023-02-20 18:37:28.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3865 2023-03-16 18:34:52.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19143 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/analysis/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.981752 autogalaxy-2023.3.27.1/autogalaxy/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-11 16:43:14.000000 autogalaxy-2023.3.27.1/autogalaxy/config/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      635 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      266 2023-02-17 17:00:07.000000 autogalaxy-2023.3.27.1/autogalaxy/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1639 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/config/grids.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3247 2023-03-24 12:25:33.000000 autogalaxy-2023.3.27.1/autogalaxy/config/notation.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.991335 autogalaxy-2023.3.27.1/autogalaxy/config/priors/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1607 2022-12-16 19:52:14.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/basis.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      620 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/cosmology.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.997527 autogalaxy-2023.3.27.1/autogalaxy/config/priors/galaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      336 2022-12-21 16:14:34.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/galaxy/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      600 2022-12-21 16:13:37.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/galaxy/hyper.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      204 2022-12-21 16:13:37.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/galaxy/redshift.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      413 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/hyper_data.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.999528 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1012 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.020534 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2105 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/chameleon.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1739 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2097 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/eff.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1733 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2849 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/exponential_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1705 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2061 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/moffat.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2101 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/sersic.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/sersic_core.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.025585 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear_operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear_operated/moffat.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.032583 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/moffat.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1469 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/sersic.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.039583 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1815 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/cartesian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1819 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1807 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/polar.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.060467 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2503 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/chameleon.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2137 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2495 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/eff.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2131 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3241 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/exponential_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2103 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2459 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/moffat.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2499 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/sersic.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3609 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/sersic_core.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.062468 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      639 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.079718 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2457 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/gnfw.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1682 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2077 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3593 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1022 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3402 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.082719 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/multipole/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1295 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/multipole/power_law_m4.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.087375 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/sheets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      389 2023-01-14 17:31:13.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/sheets/external_shear.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      632 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.103376 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2921 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/chameleon.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2545 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2539 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1481 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2907 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/sersic.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4027 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3337 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.117964 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1729 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/isothermal.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/isothermal_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      640 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/point.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/power_law.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2867 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/power_law_broken.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2473 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/power_law_core.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.129373 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      225 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      989 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/delaunay.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/rectangular.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      987 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/voronoi.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      991 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/voronoi_nn.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1536 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/point_sources.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.145587 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      246 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2023-03-24 12:25:33.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      211 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/constant.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      216 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/constant_split.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      434 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/constant_zeroth.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      209 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/zeroth.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.158354 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      144 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/include.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      259 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/mat_wrap_1d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      947 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/mat_wrap_2d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2083 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/config/visualize/plots.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3774 2023-01-14 17:32:38.000000 autogalaxy-2023.3.27.1/autogalaxy/convert.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.164354 autogalaxy-2023.3.27.1/autogalaxy/cosmology/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/cosmology/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13984 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/cosmology/lensing.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      937 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/cosmology/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/cosmology/wrap.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3236 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/exc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7348 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.172142 autogalaxy-2023.3.27.1/autogalaxy/galaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22038 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/galaxy.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6721 2023-01-14 17:32:38.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/hyper.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.176592 autogalaxy-2023.3.27.1/autogalaxy/galaxy/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/mock/mock_galaxy.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.181592 autogalaxy-2023.3.27.1/autogalaxy/galaxy/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40791 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/plot/galaxy_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4525 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/plot/hyper_galaxy_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1002 2022-12-20 17:00:47.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/redshift.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1776 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/galaxy/stellar_dark_decomp.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.187270 autogalaxy-2023.3.27.1/autogalaxy/gui/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/gui/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2049 2023-01-19 10:23:36.000000 autogalaxy-2023.3.27.1/autogalaxy/gui/clicker.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6977 2023-03-25 15:57:41.000000 autogalaxy-2023.3.27.1/autogalaxy/gui/scribbler.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.189270 autogalaxy-2023.3.27.1/autogalaxy/hyper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 16:43:14.000000 autogalaxy-2023.3.27.1/autogalaxy/hyper/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2253 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/hyper/hyper_data.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.194828 autogalaxy-2023.3.27.1/autogalaxy/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16806 2023-03-24 15:47:11.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3868 2022-12-21 17:05:21.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/imaging.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.202828 autogalaxy-2023.3.27.1/autogalaxy/imaging/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18787 2022-12-21 17:29:18.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3595 2023-02-20 18:27:21.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4279 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.206829 autogalaxy-2023.3.27.1/autogalaxy/imaging/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8809 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/imaging/plot/fit_imaging_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.212837 autogalaxy-2023.3.27.1/autogalaxy/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11984 2022-12-21 17:02:54.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3368 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/interferometer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.219835 autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21471 2022-12-21 17:29:34.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5492 2023-02-20 18:27:21.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5105 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.224835 autogalaxy-2023.3.27.1/autogalaxy/interferometer/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6836 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      341 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/mock.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.229835 autogalaxy-2023.3.27.1/autogalaxy/operate/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/operate/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34861 2023-03-22 08:34:29.000000 autogalaxy-2023.3.27.1/autogalaxy/operate/deflections.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20218 2023-03-20 10:09:35.000000 autogalaxy-2023.3.27.1/autogalaxy/operate/image.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.236032 autogalaxy-2023.3.27.1/autogalaxy/plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      686 2020-11-16 19:58:12.000000 autogalaxy-2023.3.27.1/autogalaxy/plane/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18656 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/autogalaxy/plane/plane.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.241032 autogalaxy-2023.3.27.1/autogalaxy/plane/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/plane/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13971 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/plane/plot/plane_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10462 2022-12-21 13:17:53.000000 autogalaxy-2023.3.27.1/autogalaxy/plane/to_inversion.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.249066 autogalaxy-2023.3.27.1/autogalaxy/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3405 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      557 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/abstract_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.255125 autogalaxy-2023.3.27.1/autogalaxy/plot/get_visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/get_visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9938 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/get_visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13327 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/get_visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.262125 autogalaxy-2023.3.27.1/autogalaxy/plot/include/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/include/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1470 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/include/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2660 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/include/two_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4572 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/mass_plotter.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.267124 autogalaxy-2023.3.27.1/autogalaxy/plot/mat_plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/mat_plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6115 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/mat_plot/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10005 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/mat_plot/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.272792 autogalaxy-2023.3.27.1/autogalaxy/plot/visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2129 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4064 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/visuals/two_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      646 2023-03-18 16:31:03.000000 autogalaxy-2023.3.27.1/autogalaxy/plot/wrap.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.280687 autogalaxy-2023.3.27.1/autogalaxy/profiles/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 16:43:14.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13975 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/geometry_profiles.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.289688 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5444 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1284 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/basis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2511 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.312687 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      411 2023-03-25 18:04:40.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6749 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1857 2023-03-25 18:04:40.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/eff.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1831 2023-03-25 18:04:40.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1734 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/exponential_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1755 2023-03-16 18:34:52.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1749 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2219 2023-03-25 18:04:40.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2730 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/sersic_core.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.321689 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear_operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       99 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear_operated/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      209 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear_operated/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      205 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear_operated/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      205 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear_operated/sersic.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.325845 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1038 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/mock/mock_light_profile.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.336898 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      143 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/operated/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       41 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/operated/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      202 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/operated/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      198 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/operated/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      198 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/operated/sersic.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.347867 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      247 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1202 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4264 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/cartesian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4501 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-03-03 11:53:26.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/polar.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.365441 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      371 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4009 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3255 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2581 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2782 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/eff.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2504 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2227 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2736 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2338 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/sersic_core.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.387194 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      490 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5851 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4414 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/eff.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2316 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3188 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/exponential_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4052 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4905 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7640 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5734 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/sersic_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25211 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/light_and_mass_profiles.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.389194 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1008 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.397773 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10362 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7050 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/cse.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8683 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/mge.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.421706 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12403 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13496 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/gnfw.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/gnfw_mcr.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3344 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/mcr_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11551 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2540 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_mcr.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2094 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4412 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_truncated.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1163 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.425813 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      716 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/mock/mock_mass_profile.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.429779 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/multipole/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       46 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/multipole/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8555 2022-12-16 21:22:43.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/multipole/power_law_m4.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.438915 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      127 2022-12-16 18:30:52.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2255 2023-01-14 17:18:56.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/external_shear.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4983 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/input_deflections.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1416 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/mass_sheet.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.459172 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      372 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       35 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8484 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2472 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7635 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16727 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7040 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/sersic_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9615 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.474763 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6348 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/isothermal.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2109 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/isothermal_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1906 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/point.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5182 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/power_law.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6523 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/power_law_broken.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8445 2022-12-16 19:36:21.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/power_law_core.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.479762 autogalaxy-2023.3.27.1/autogalaxy/profiles/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12969 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/plot/light_profile_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14923 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/plot/mass_profile_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      473 2021-08-21 09:36:59.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/point_sources.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1458 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/profiles/scaling_relations.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.484944 autogalaxy-2023.3.27.1/autogalaxy/quantity/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9905 2023-01-14 16:15:50.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/dataset_quantity.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4650 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/fit_quantity.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.492368 autogalaxy-2023.3.27.1/autogalaxy/quantity/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10145 2022-12-21 17:05:21.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1747 2023-02-20 18:27:21.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3537 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.496209 autogalaxy-2023.3.27.1/autogalaxy/quantity/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8176 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/autogalaxy/quantity/plot/fit_quantity_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.502901 autogalaxy-2023.3.27.1/autogalaxy/util/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1331 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/util/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2578 2022-02-14 09:21:43.000000 autogalaxy-2023.3.27.1/autogalaxy/util/error_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.506900 autogalaxy-2023.3.27.1/autogalaxy/util/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/util/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1355 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/autogalaxy/util/mock/mock_cosmology.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5560 2022-12-20 20:45:07.000000 autogalaxy-2023.3.27.1/autogalaxy/util/plane_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3858 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/autogalaxy/util/shear_field.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.758038 autogalaxy-2023.3.27.1/autogalaxy.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16587 2023-03-27 14:48:37.000000 autogalaxy-2023.3.27.1/autogalaxy.egg-info/SOURCES.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.510899 autogalaxy-2023.3.27.1/docs/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.514900 autogalaxy-2023.3.27.1/docs/_templates/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autogalaxy-2023.3.27.1/docs/_templates/custom-class-template.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/_templates/custom_module_template.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.520408 autogalaxy-2023.3.27.1/docs/advanced/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/advanced/chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6363 2022-12-20 22:05:13.000000 autogalaxy-2023.3.27.1/docs/advanced/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1365 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/advanced/graphical.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.534526 autogalaxy-2023.3.27.1/docs/api/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1592 2023-01-13 16:57:54.000000 autogalaxy-2023.3.27.1/docs/api/data.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      330 2022-12-20 17:33:12.000000 autogalaxy-2023.3.27.1/docs/api/fitting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1048 2022-12-20 17:00:47.000000 autogalaxy-2023.3.27.1/docs/api/galaxy.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.909007 autogalaxy-2023.3.27.1/docs/api/images/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.541399 autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41383 2022-12-21 12:27:28.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/data_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34340 2022-12-21 12:27:28.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/grid_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49269 2022-12-21 12:27:49.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/image_plane_mesh.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.548399 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40349 2022-12-21 12:22:21.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/data_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26453 2022-12-21 12:22:21.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48007 2022-12-21 12:28:33.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.555405 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56739 2022-12-21 13:10:07.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/data_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27379 2022-12-21 13:10:07.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    77426 2022-12-21 13:10:07.000000 autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/api/light.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2022-12-20 17:37:15.000000 autogalaxy-2023.3.27.1/docs/api/modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1771 2022-12-21 15:51:37.000000 autogalaxy-2023.3.27.1/docs/api/pixelization.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3184 2022-12-20 17:56:04.000000 autogalaxy-2023.3.27.1/docs/api/plot.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2422 2022-12-16 19:36:25.000000 autogalaxy-2023.3.27.1/docs/api/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4633 2022-12-21 13:26:02.000000 autogalaxy-2023.3.27.1/docs/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.567493 autogalaxy-2023.3.27.1/docs/general/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1593 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/docs/general/citations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1035 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/general/configs.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1315 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/general/credits.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      981 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/general/likelihood_function.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9319 2023-03-26 14:21:08.000000 autogalaxy-2023.3.27.1/docs/general/model_cookbook.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       92 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/general/papers.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2479 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/general/workspace.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.578493 autogalaxy-2023.3.27.1/docs/howtogalaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1827 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_1_introduction.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2244 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_2_modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1038 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_3_search_chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1396 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_4_pixelizations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1462 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_optional.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3491 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/howtogalaxy/howtogalaxy.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10548 2023-03-26 14:14:27.000000 autogalaxy-2023.3.27.1/docs/index.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.589130 autogalaxy-2023.3.27.1/docs/installation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4014 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/installation/conda.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3541 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/installation/numba.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2428 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/installation/overview.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3442 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/installation/pip.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4728 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/installation/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4572 2023-01-14 16:37:15.000000 autogalaxy-2023.3.27.1/docs/installation/troubleshooting.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.612563 autogalaxy-2023.3.27.1/docs/overview/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:37.916007 autogalaxy-2023.3.27.1/docs/overview/images/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.643408 autogalaxy-2023.3.27.1/docs/overview/images/fitting/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37264 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/bad_chi_squared_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63409 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/bad_normalized_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39647 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/bad_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51168 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/chi_squared_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35309 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37035 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/masked_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33220 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/model_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44440 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/noise_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69331 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/normalized_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30136 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/plane_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31550 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/psf.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    65595 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/fitting/residual_map.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.658398 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28953 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/galaxy.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21591 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/grid_2d.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29995 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/merging_galaxies.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29232 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29344 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/sersic_light_profile.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35172 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/galaxies/subplot_galaxies.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.679777 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107396 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113651 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/dirty_signal_to_noise.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   390140 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/fit_dirty_images.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41276 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/image_pre_ft.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46706 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/model_visibilities.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45127 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/reconstruction.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/uv_wavelengths.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30950 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/interferometry/visibilities.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.688783 autogalaxy-2023.3.27.1/docs/overview/images/modeling/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1175623 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/modeling/cornerplot.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39125 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/modeling/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   231702 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/modeling/subplot_fit.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.703515 autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    73817 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75926 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/g_decomposed_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   152814 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/g_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141963 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/r_decomposed_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140328 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/r_image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.708514 autogalaxy-2023.3.27.1/docs/overview/images/pixelizations/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38896 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/pixelizations/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40489 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/pixelizations/rectangular.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.726514 autogalaxy-2023.3.27.1/docs/overview/images/simulating/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   106644 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/ao.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37696 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/euclid.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80336 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/hst.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35633 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43310 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/noise_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33339 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/psf.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49620 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/docs/overview/images/simulating/vro.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8218 2022-12-19 12:25:36.000000 autogalaxy-2023.3.27.1/docs/overview/overview_1_galaxies.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6648 2022-12-19 12:25:36.000000 autogalaxy-2023.3.27.1/docs/overview/overview_2_fitting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20480 2023-03-26 14:14:27.000000 autogalaxy-2023.3.27.1/docs/overview/overview_3_modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2957 2022-12-19 12:25:36.000000 autogalaxy-2023.3.27.1/docs/overview/overview_4_simulate.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3508 2022-12-21 13:35:24.000000 autogalaxy-2023.3.27.1/docs/overview/overview_5_pixelizations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9036 2022-12-19 12:25:37.000000 autogalaxy-2023.3.27.1/docs/overview/overview_6_interferometry.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10667 2022-12-19 12:25:37.000000 autogalaxy-2023.3.27.1/docs/overview/overview_7_multi_wavelength.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/docs/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/eden.ini
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.741515 autogalaxy-2023.3.27.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21260 2023-02-21 10:35:21.000000 autogalaxy-2023.3.27.1/files/citations.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1679 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/files/citations.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2267 2023-02-06 13:53:49.000000 autogalaxy-2023.3.27.1/files/citations.tex
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43549 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/files/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29819 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/files/model_dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    67674 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/files/non_parametric.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   139037 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/files/observed.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/files/parametric.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   223339 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/files/visibilities.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      110 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/optional_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:38.756039 autogalaxy-2023.3.27.1/paper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      190 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/paper/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   399405 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/paper/almacombined.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   342368 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/paper/hstcombined.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   122730 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/paper/observed.pdf
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45539 2023-02-21 10:35:21.000000 autogalaxy-2023.3.27.1/paper/paper.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      830 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/paper/paper.json
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13514 2023-01-25 15:27:13.000000 autogalaxy-2023.3.27.1/paper/paper.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.3.27.1/paper/parametric.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2022-12-19 13:59:53.000000 autogalaxy-2023.3.27.1/readthedocs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       29 2022-12-16 17:06:50.000000 autogalaxy-2023.3.27.1/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-03-27 14:48:38.759038 autogalaxy-2023.3.27.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2019 2023-03-27 14:45:03.000000 autogalaxy-2023.3.27.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3014 2023-03-27 14:42:00.000000 autogalaxy-2023.3.27.1/zenodo.json
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.915660 autogalaxy-2023.7.7.1/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:57.985857 autogalaxy-2023.7.7.1/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.047725 autogalaxy-2023.7.7.1/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/.github/workflows/draft-pdf.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3327 2022-12-19 16:37:19.000000 autogalaxy-2023.7.7.1/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1135 2022-12-19 11:17:33.000000 autogalaxy-2023.7.7.1/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18987 2022-12-20 20:59:49.000000 autogalaxy-2023.7.7.1/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2494 2022-12-20 20:59:49.000000 autogalaxy-2023.7.7.1/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2020-11-16 19:58:12.000000 autogalaxy-2023.7.7.1/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8400 2023-06-07 09:47:58.914628 autogalaxy-2023.7.7.1/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.057726 autogalaxy-2023.7.7.1/autogalaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5518 2023-06-07 09:38:14.000000 autogalaxy-2023.7.7.1/autogalaxy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7805 2023-06-03 11:22:20.000000 autogalaxy-2023.7.7.1/autogalaxy/abstract_fit.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.068740 autogalaxy-2023.7.7.1/autogalaxy/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      308 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7129 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4541 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2653 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2844 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2746 2023-05-11 09:42:09.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/plane.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.087762 autogalaxy-2023.7.7.1/autogalaxy/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-21 09:36:45.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18823 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10497 2023-06-05 13:31:36.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/chaining_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/clump_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5029 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/maker.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.090765 autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3288 2023-06-05 20:15:34.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9953 2023-06-06 14:36:29.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/model_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9842 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/preloads.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6634 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1157 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19568 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.099761 autogalaxy-2023.7.7.1/autogalaxy/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-11 16:43:14.000000 autogalaxy-2023.7.7.1/autogalaxy/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      493 2023-06-06 18:37:09.000000 autogalaxy-2023.7.7.1/autogalaxy/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1677 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/config/grids.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3369 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.108171 autogalaxy-2023.7.7.1/autogalaxy/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1607 2022-12-16 19:52:14.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/basis.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      620 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/cosmology.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.112203 autogalaxy-2023.7.7.1/autogalaxy/config/priors/galaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      253 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/galaxy/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      204 2022-12-21 16:13:37.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/galaxy/redshift.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.115116 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1012 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.138665 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2105 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1739 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2097 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/eff.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1733 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2849 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1705 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2061 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2101 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic_core.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.144647 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/moffat.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.152660 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1469 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/sersic.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.160864 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1815 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/cartesian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1819 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1807 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/polar.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.185674 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2503 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2137 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2495 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/eff.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2131 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3241 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2103 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2459 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2499 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3609 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic_core.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.188655 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      639 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.207151 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2457 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1682 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2077 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3593 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1022 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3402 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.216761 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      640 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/point.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/smbh.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1604 2023-05-17 15:24:31.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/smbh_binary.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.222325 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      389 2023-01-14 17:31:13.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/external_shear.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      632 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.240286 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2921 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2545 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2539 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1481 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2907 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4027 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3337 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.255277 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1729 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2867 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_broken.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2473 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1333 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.267350 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      225 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      989 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/delaunay.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/rectangular.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      987 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      991 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi_nn.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1536 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/point_sources.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.282870 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      246 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2023-03-24 12:25:33.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      211 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/constant.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      216 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/constant_split.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      434 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/constant_zeroth.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      209 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/zeroth.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.294944 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      174 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/include.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      259 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/mat_wrap_1d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      947 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/mat_wrap_2d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5385 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/plots.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3774 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/convert.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.301984 autogalaxy-2023.7.7.1/autogalaxy/cosmology/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13974 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/lensing.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      933 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/wrap.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3232 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7213 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.308879 autogalaxy-2023.7.7.1/autogalaxy/galaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20983 2023-05-15 19:02:02.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/galaxy.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.312879 autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/mock_galaxy.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.317928 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4437 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/adapt_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40501 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/galaxy_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1002 2022-12-20 17:00:47.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/redshift.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1772 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/stellar_dark_decomp.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.322913 autogalaxy-2023.7.7.1/autogalaxy/gui/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/gui/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2041 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/gui/clicker.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6977 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/gui/scribbler.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.327921 autogalaxy-2023.7.7.1/autogalaxy/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12738 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3868 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.335921 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16878 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3215 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4285 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.338924 autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9632 2023-06-03 16:50:56.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/fit_imaging_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.344759 autogalaxy-2023.7.7.1/autogalaxy/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10643 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3368 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.352759 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17326 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2960 2023-06-05 20:15:34.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5378 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.357791 autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8265 2023-06-03 16:50:56.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      341 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.362803 autogalaxy-2023.7.7.1/autogalaxy/operate/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/operate/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36267 2023-06-03 17:45:40.000000 autogalaxy-2023.7.7.1/autogalaxy/operate/deflections.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20198 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/operate/image.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.369913 autogalaxy-2023.7.7.1/autogalaxy/plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      686 2020-11-16 19:58:12.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16202 2023-05-15 18:37:24.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plane.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8439 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plane_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.372907 autogalaxy-2023.7.7.1/autogalaxy/plane/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14120 2023-05-23 09:38:20.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plot/plane_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10432 2023-06-06 10:32:57.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/to_inversion.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.380903 autogalaxy-2023.7.7.1/autogalaxy/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3398 2023-06-03 09:03:18.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      553 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.385903 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9924 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13590 2023-06-03 17:45:40.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.391906 autogalaxy-2023.7.7.1/autogalaxy/plot/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/include/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1470 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/include/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2658 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/include/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4560 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mass_plotter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.397908 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6113 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10005 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.402902 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2123 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4140 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      646 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/wrap.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.410870 autogalaxy-2023.7.7.1/autogalaxy/profiles/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 16:43:14.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13967 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/geometry_profiles.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.419394 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5442 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1883 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/basis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2511 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.454033 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      401 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6951 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1835 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1734 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1755 2023-03-16 18:34:52.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1749 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2223 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2730 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.464044 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       99 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      207 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/sersic.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.468188 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1032 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/mock_light_profile.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.481195 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      143 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      200 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/sersic.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.493270 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      247 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1202 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4264 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/cartesian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4501 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/polar.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.513288 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      371 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4007 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3255 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2581 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2782 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2504 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2227 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2736 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2338 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.537261 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      490 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5851 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4414 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2316 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3188 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4052 2023-04-27 18:43:48.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4905 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7640 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5734 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25207 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light_and_mass_profiles.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.540219 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1020 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.548262 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10340 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7050 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/cse.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8675 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/mge.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.573428 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12379 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13480 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1130 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3352 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/mcr_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11547 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2532 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2090 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4410 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1161 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.577335 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      714 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/mock_mass_profile.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.586402 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       91 2023-05-17 15:24:31.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1902 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/point.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1653 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/smbh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4963 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/smbh_binary.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.596000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      127 2022-12-16 18:30:52.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2611 2023-06-06 12:57:36.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/external_shear.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4977 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/input_deflections.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1416 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/mass_sheet.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.616301 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      372 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8482 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2472 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7629 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16715 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7038 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9613 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.633501 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      337 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6348 2023-06-06 12:20:19.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2109 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5545 2023-06-06 12:57:36.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6460 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_broken.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8476 2023-06-06 12:51:47.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8585 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_multipole.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.639502 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12961 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/light_profile_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14915 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/mass_profile_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      467 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/point_sources.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/scaling_relations.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.645036 autogalaxy-2023.7.7.1/autogalaxy/quantity/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9901 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/dataset_quantity.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4646 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/fit_quantity.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.653791 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10139 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1747 2023-02-20 18:27:21.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3510 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.657797 autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8126 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/fit_quantity_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.663799 autogalaxy-2023.7.7.1/autogalaxy/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1391 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/util/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2572 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/util/error_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.668800 autogalaxy-2023.7.7.1/autogalaxy/util/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/util/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1353 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/util/mock/mock_cosmology.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3858 2023-01-13 16:57:54.000000 autogalaxy-2023.7.7.1/autogalaxy/util/shear_field.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.913466 autogalaxy-2023.7.7.1/autogalaxy.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16633 2023-06-07 09:47:57.000000 autogalaxy-2023.7.7.1/autogalaxy.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.676119 autogalaxy-2023.7.7.1/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.679798 autogalaxy-2023.7.7.1/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autogalaxy-2023.7.7.1/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.686797 autogalaxy-2023.7.7.1/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/advanced/chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6363 2022-12-20 22:05:13.000000 autogalaxy-2023.7.7.1/docs/advanced/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1374 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/advanced/graphical.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.701810 autogalaxy-2023.7.7.1/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1592 2023-01-13 16:57:54.000000 autogalaxy-2023.7.7.1/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      330 2022-12-20 17:33:12.000000 autogalaxy-2023.7.7.1/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      664 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/docs/api/galaxy.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.022475 autogalaxy-2023.7.7.1/docs/api/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.710809 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41383 2022-12-21 12:27:28.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34340 2022-12-21 12:27:28.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49269 2022-12-21 12:27:49.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/image_plane_mesh.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.717924 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40349 2022-12-21 12:22:21.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26453 2022-12-21 12:22:21.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48007 2022-12-21 12:28:33.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.725737 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56739 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27379 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    77426 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/api/light.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1771 2022-12-21 15:51:37.000000 autogalaxy-2023.7.7.1/docs/api/pixelization.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3184 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2420 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4631 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.738737 autogalaxy-2023.7.7.1/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1593 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.1/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1035 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1315 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      981 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/general/likelihood_function.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9728 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/general/model_cookbook.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       92 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/general/papers.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2450 2023-05-12 11:43:15.000000 autogalaxy-2023.7.7.1/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.750173 autogalaxy-2023.7.7.1/docs/howtogalaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1827 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2244 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_2_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1038 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_3_search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1396 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_4_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      960 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_optional.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3447 2023-05-12 10:01:56.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/howtogalaxy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10537 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.761177 autogalaxy-2023.7.7.1/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4014 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3519 2023-05-12 10:01:56.000000 autogalaxy-2023.7.7.1/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2403 2023-05-12 10:10:15.000000 autogalaxy-2023.7.7.1/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3442 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4703 2023-05-12 10:10:15.000000 autogalaxy-2023.7.7.1/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4572 2023-01-14 16:37:15.000000 autogalaxy-2023.7.7.1/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.775209 autogalaxy-2023.7.7.1/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.029699 autogalaxy-2023.7.7.1/docs/overview/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.804669 autogalaxy-2023.7.7.1/docs/overview/images/fitting/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37264 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63409 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39647 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51168 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35309 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37035 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/masked_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33220 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44440 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69331 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30136 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/plane_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31550 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    65595 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/residual_map.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.819713 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28953 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/galaxy.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21591 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/grid_2d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29995 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/merging_galaxies.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29232 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29344 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/sersic_light_profile.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35172 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/subplot_galaxies.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.839804 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107396 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113651 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_signal_to_noise.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   390140 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/fit_dirty_images.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41276 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/image_pre_ft.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46706 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/model_visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45127 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/reconstruction.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/uv_wavelengths.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30950 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/visibilities.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.847859 autogalaxy-2023.7.7.1/docs/overview/images/modeling/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1175623 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/modeling/cornerplot.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39125 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/modeling/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   231702 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/modeling/subplot_fit.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.860859 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    73817 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75926 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_decomposed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   152814 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141963 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_decomposed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140328 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.865883 autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38896 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40489 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/rectangular.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.882894 autogalaxy-2023.7.7.1/docs/overview/images/simulating/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   106644 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/ao.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37696 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/euclid.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80336 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/hst.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35633 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43310 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33339 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49620 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/vro.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8164 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_1_galaxies.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6608 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_2_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20432 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_3_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2948 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_4_simulate.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3483 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_5_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8857 2023-06-03 12:30:36.000000 autogalaxy-2023.7.7.1/docs/overview/overview_6_interferometry.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10664 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_7_multi_wavelength.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.897879 autogalaxy-2023.7.7.1/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21260 2023-02-21 10:35:21.000000 autogalaxy-2023.7.7.1/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1679 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.1/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2267 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.1/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43549 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29819 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/model_dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    67674 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/non_parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   139037 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/observed.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   223339 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      112 2023-06-03 19:29:54.000000 autogalaxy-2023.7.7.1/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.911501 autogalaxy-2023.7.7.1/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      190 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   399405 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/almacombined.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   342368 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/hstcombined.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   122730 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/observed.pdf
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45539 2023-02-21 10:35:21.000000 autogalaxy-2023.7.7.1/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      830 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13514 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2022-12-19 13:59:53.000000 autogalaxy-2023.7.7.1/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       29 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:47:58.915660 autogalaxy-2023.7.7.1/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2016 2023-06-07 09:47:40.000000 autogalaxy-2023.7.7.1/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-06-07 09:38:14.000000 autogalaxy-2023.7.7.1/zenodo.json
```

### Comparing `autogalaxy-2023.3.27.1/.github/workflows/main.yml` & `autogalaxy-2023.7.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/CITATIONS.rst` & `autogalaxy-2023.7.7.1/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/CODE_OF_CONDUCT.md` & `autogalaxy-2023.7.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/CONTRIBUTING.md` & `autogalaxy-2023.7.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/LICENSE` & `autogalaxy-2023.7.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/PKG-INFO` & `autogalaxy-2023.7.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogalaxy
-Version: 2023.3.27.1
+Version: 2023.7.7.1
 Summary: Open-Source Multi Wavelength Galaxy Structure & Morphology
 Home-page: https://github.com/Jammy2211/PyAutoGalaxy
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -145,26 +145,28 @@
     import autogalaxy as ag
 
     import os
 
     """
     Load Imaging data of the strong galaxy from the dataset folder of the workspace.
     """
-    imaging = ag.Imaging.from_fits(
-        image_path="/path/to/dataset/image.fits",
+    dataset = ag.Imaging.from_fits(
+        data_path="/path/to/dataset/image.fits",
         noise_map_path="/path/to/dataset/noise_map.fits",
         psf_path="/path/to/dataset/psf.fits",
         pixel_scales=0.1,
     )
 
     """
     Create a mask for the data, which we setup as a 3.0" circle.
     """
     mask = ag.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+        shape_native=dataset.shape_native,
+        pixel_scales=dataset.pixel_scales,
+        radius=3.0
     )
 
     """
     We model the galaxy using an Sersic LightProfile.
     """
     light_profile = ag.lp.Sersic
 
@@ -180,15 +182,15 @@
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
     
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the galaxy model to the data.
     """
-    analysis = ag.AnalysisImaging(dataset=masked_imaging)
+    analysis = ag.AnalysisImaging(dataset=masked_dataset)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autogalaxy-2023.3.27.1/README.rst` & `autogalaxy-2023.7.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -123,26 +123,28 @@
     import autogalaxy as ag
 
     import os
 
     """
     Load Imaging data of the strong galaxy from the dataset folder of the workspace.
     """
-    imaging = ag.Imaging.from_fits(
-        image_path="/path/to/dataset/image.fits",
+    dataset = ag.Imaging.from_fits(
+        data_path="/path/to/dataset/image.fits",
         noise_map_path="/path/to/dataset/noise_map.fits",
         psf_path="/path/to/dataset/psf.fits",
         pixel_scales=0.1,
     )
 
     """
     Create a mask for the data, which we setup as a 3.0" circle.
     """
     mask = ag.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+        shape_native=dataset.shape_native,
+        pixel_scales=dataset.pixel_scales,
+        radius=3.0
     )
 
     """
     We model the galaxy using an Sersic LightProfile.
     """
     light_profile = ag.lp.Sersic
 
@@ -158,15 +160,15 @@
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
     
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the galaxy model to the data.
     """
-    analysis = ag.AnalysisImaging(dataset=masked_imaging)
+    analysis = ag.AnalysisImaging(dataset=masked_dataset)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/__init__.py` & `autogalaxy-2023.7.7.1/autogalaxy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,17 @@
 from .interferometer.fit_interferometer import FitInterferometer
 from .interferometer.model.analysis import AnalysisInterferometer
 
 from .quantity.fit_quantity import FitQuantity
 from .quantity.model.analysis import AnalysisQuantity
 from .quantity.dataset_quantity import DatasetQuantity
 from .galaxy.galaxy import Galaxy
-from .galaxy.hyper import HyperGalaxy
 from .galaxy.redshift import Redshift
 from .galaxy.stellar_dark_decomp import StellarDarkDecomp
-from .hyper import hyper_data
-from .analysis.setup import SetupHyper
+from .analysis.setup import SetupAdapt
 from .plane.plane import Plane
 from .plane.to_inversion import AbstractToInversion
 from .plane.to_inversion import PlaneToInversion
 from .profiles.geometry_profiles import EllProfile
 from .profiles import (
     point_sources as ps,
     mass as mp,
@@ -107,8 +105,8 @@
 
 from .analysis.clump_model import ClumpModel
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.3.27.1"
+__version__ = "2023.7.7.1"
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/abstract_fit.py` & `autogalaxy-2023.7.7.1/autogalaxy/abstract_fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 import copy
 from typing import TYPE_CHECKING, Dict, Optional
 
+from autofit import ModelInstance
+
 if TYPE_CHECKING:
     from autogalaxy.galaxy.galaxy import Galaxy
 
 import autoarray as aa
 
-from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
+from autogalaxy.profiles.light.basis import Basis
 
 
 class AbstractFitInversion:
     def __init__(self, model_obj, settings_inversion: aa.SettingsInversion):
         """
         An abstract fit object which fits to datasets (e.g. imaging, interferometer) inherit from.
 
@@ -97,19 +99,17 @@
         linear_obj_func_list = self.inversion.cls_list_from(
             cls=aa.AbstractLinearObjFuncList
         )
 
         linear_light_profile_intensity_dict = {}
 
         for linear_obj_func in linear_obj_func_list:
-
             reconstruction = self.inversion.reconstruction_dict[linear_obj_func]
 
             for i, light_profile in enumerate(linear_obj_func.light_profile_list):
-
                 linear_light_profile_intensity_dict[light_profile] = float(
                     reconstruction[i]
                 )
 
         return linear_light_profile_intensity_dict
 
     def galaxy_linear_obj_data_dict_from(
@@ -121,18 +121,18 @@
         objects.
 
         The `model_data` is the `reconstructed_data` solved for in the inversion`.
 
         This is used to create the overall `galaxy_model_image_dict`, which maps every galaxy to its
         overall `model_data` (e.g. including the `model_data` of orindary light profiles too).
 
-        If `use_image=False`, the `reconstructed_data` of the inversion (e.g. an image for imaging data,
+        If `use_image=False`, the `reconstructed_data` of the inversion (e.g. an image for dataset data,
         visibilities for  interferometer data) is input in the dictionary.
 
-        if `use_image=True`, the `reconstructed_image` of the inversion (e.g. the image for imaging data, the
+        if `use_image=True`, the `reconstructed_image` of the inversion (e.g. the image for dataset data, the
         real-space image for interferometer data) is input in the dictionary.
 
         Parameters
         ----------
         use_image
             Whether to put the reconstructed data or images in the dictionary.
 
@@ -143,35 +143,30 @@
         """
         if self.inversion is None:
             return {}
 
         galaxy_linear_obj_image_dict = {}
 
         for linear_obj in self.inversion.linear_obj_list:
-
             galaxy = self.inversion.linear_obj_galaxy_dict[linear_obj]
 
             if not use_image:
-
                 mapped_reconstructed = self.inversion.mapped_reconstructed_data_dict[
                     linear_obj
                 ]
 
             else:
-
                 mapped_reconstructed = self.inversion.mapped_reconstructed_image_dict[
                     linear_obj
                 ]
 
             if galaxy in galaxy_linear_obj_image_dict:
-
                 galaxy_linear_obj_image_dict[galaxy] += mapped_reconstructed
 
             else:
-
                 galaxy_linear_obj_image_dict.update({galaxy: mapped_reconstructed})
 
         return galaxy_linear_obj_image_dict
 
     @property
     def model_obj_linear_light_profiles_to_light_profiles(self):
         """
@@ -187,19 +182,18 @@
         A `model_obj` (E.g. `Plane` or `Tracer`) where the light profile intensity values are set to the results
         of those inferred via the `Inversion`.
         """
 
         if self.linear_light_profile_intensity_dict is None:
             return self.model_obj
 
-        model_obj = copy.copy(self.model_obj)
+        model_instance = ModelInstance(dict(model_obj=self.model_obj))
 
-        for galaxy in model_obj.galaxies:
-            for key, obj in galaxy.__dict__.items():
-                if isinstance(obj, LightProfile):
-                    try:
-                        intensity = self.linear_light_profile_intensity_dict[obj]
-                        galaxy.__dict__[key] = obj.lp_instance_from(intensity=intensity)
-                    except KeyError:
-                        pass
+        for path, instance in model_instance.path_instance_tuples_for_class(
+            (LightProfileLinear, Basis)
+        ):
+            model_instance = model_instance.replacing_for_path(
+                path,
+                instance.lp_instance_from(self.linear_light_profile_intensity_dict),
+            )
 
-        return model_obj
+        return model_instance.model_obj
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/aggregator/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/aggregator/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         ----------
         aggregator
             An PyAutoFit aggregator containing the results of non-linear searches performed by PyAutoFit.
         """
         self.aggregator = aggregator
 
     @abstractmethod
-    def make_object_for_gen(self, fit: af.Fit, galaxies: List[Galaxy]) -> object:
+    def object_via_gen_from(self, fit: af.Fit, galaxies: List[Galaxy]) -> object:
         """
         For example, in the `PlaneAgg` object, this function is overwritten such that it creates a `Plane` from a
         `ModelInstance` that contains the galaxies of a sample from a non-linear search.
 
         Parameters
         ----------
         fit
@@ -51,15 +51,19 @@
 
         For example, in **PyAutoLens**, by overwriting the `make_gen_from` method this returns a generator
         of `Plane` objects from a PyAutoFit aggregator. This generator then generates a list of the maximum log
         likelihood `Plane` objects for all aggregator results.
         """
 
         def func_gen(fit: af.Fit) -> Generator:
-            return self.make_object_for_gen(fit=fit, galaxies=fit.instance.galaxies)
+            galaxies = fit.instance.galaxies
+            if hasattr(fit.instance, "clumps"):
+                galaxies = galaxies + fit.instance.clumps
+
+            return self.object_via_gen_from(fit=fit, galaxies=galaxies)
 
         return self.aggregator.map(func=func_gen)
 
     def weights_above_gen_from(self, minimum_weight: float) -> List:
         """
         Returns a list of all weights above a minimum weight for every result.
 
@@ -67,23 +71,20 @@
         ----------
         minimum_weight
             The minimum weight of a non-linear sample, such that samples with a weight below this value are discarded
             and not included in the generator.
         """
 
         def func_gen(fit: af.Fit, minimum_weight: float) -> List[object]:
-
             samples = fit.value(name="samples")
 
             weight_list = []
 
             for sample in samples.sample_list:
-
                 if sample.weight > minimum_weight:
-
                     weight_list.append(sample.weight)
 
             return weight_list
 
         func = partial(func_gen, minimum_weight=minimum_weight)
 
         return self.aggregator.map(func=func)
@@ -107,26 +108,24 @@
         ----------
         minimum_weight
             The minimum weight of a non-linear sample, such that samples with a weight below this value are discarded
             and not included in the generator.
         """
 
         def func_gen(fit: af.Fit, minimum_weight: float) -> List[object]:
-
             samples = fit.value(name="samples")
 
             all_above_weight_list = []
 
             for sample in samples.sample_list:
-
                 if sample.weight > minimum_weight:
                     instance = sample.instance_for_model(model=samples.model)
 
                     all_above_weight_list.append(
-                        self.make_object_for_gen(fit=fit, galaxies=instance.galaxies)
+                        self.object_via_gen_from(fit=fit, galaxies=instance.galaxies)
                     )
 
             return all_above_weight_list
 
         func = partial(func_gen, minimum_weight=minimum_weight)
 
         return self.aggregator.map(func=func)
@@ -148,19 +147,18 @@
         Parameters
         ----------
         total_samples
             The total number of non-linear search samples that should be randomly drawn from the PDF.
         """
 
         def func_gen(fit: af.Fit, total_samples: int) -> List[object]:
-
             samples = fit.value(name="samples")
 
             return [
-                self.make_object_for_gen(
+                self.object_via_gen_from(
                     fit=fit,
                     galaxies=samples.draw_randomly_via_pdf().galaxies,
                 )
                 for i in range(total_samples)
             ]
 
         func = partial(func_gen, total_samples=total_samples)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/aggregator/fit_imaging.py` & `autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_imaging.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,121 +13,114 @@
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.aggregator.plane import _plane_from
 
 
 def _fit_imaging_from(
     fit: af.Fit,
     galaxies: List[Galaxy],
-    settings_imaging: aa.SettingsImaging = None,
+    settings_dataset: aa.SettingsImaging = None,
     settings_pixelization: aa.SettingsPixelization = None,
     settings_inversion: aa.SettingsInversion = None,
     use_preloaded_grid: bool = True,
-    use_hyper_scaling: bool = True,
 ) -> FItImaging:
     """
     Returns a `FitImaging` object from a PyAutoFit database `Fit` object and an instance of galaxies from a non-linear
     search model-fit.
 
-    This function adds the `hyper_model_image` and `hyper_galaxy_image_path_dict` to the galaxies before performing the
+    This function adds the `adapt_model_image` and `adapt_galaxy_image_path_dict` to the galaxies before performing the
     fit, if they were used.
 
     Parameters
     ----------
     fit
-        A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+        A PyAutoFit database Fit object containing the generators of the results of model-fits.
     galaxies
         A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
     Returns
     -------
     FitImaging
         The fit to the imaging dataset computed via an instance of galaxies.
     """
 
     from autogalaxy.imaging.fit_imaging import FitImaging
 
-    imaging = _imaging_from(fit=fit, settings_imaging=settings_imaging)
+    dataset = _imaging_from(fit=fit, settings_dataset=settings_dataset)
 
     plane = _plane_from(fit=fit, galaxies=galaxies)
 
     settings_pixelization = settings_pixelization or fit.value(
         name="settings_pixelization"
     )
     settings_inversion = settings_inversion or fit.value(name="settings_inversion")
 
     preloads = Preloads(use_w_tilde=False)
 
     if use_preloaded_grid:
-
         sparse_grids_of_planes = fit.value(name="preload_sparse_grids_of_planes")
 
         if sparse_grids_of_planes is not None:
-
             preloads = Preloads(
                 sparse_image_plane_grid_pg_list=sparse_grids_of_planes,
                 use_w_tilde=False,
             )
 
             if len(preloads.sparse_image_plane_grid_pg_list) == 2:
                 if type(preloads.sparse_image_plane_grid_pg_list[1]) != list:
                     preloads.sparse_image_plane_grid_pg_list[1] = [
                         preloads.sparse_image_plane_grid_pg_list[1]
                     ]
 
     return FitImaging(
-        dataset=imaging,
+        dataset=dataset,
         plane=plane,
         settings_pixelization=settings_pixelization,
         settings_inversion=settings_inversion,
         preloads=preloads,
-        use_hyper_scaling=use_hyper_scaling,
     )
 
 
 class FitImagingAgg(AbstractAgg):
     def __init__(
         self,
         aggregator: af.Aggregator,
-        settings_imaging: Optional[aa.SettingsImaging] = None,
+        settings_dataset: Optional[aa.SettingsImaging] = None,
         settings_pixelization: Optional[aa.SettingsPixelization] = None,
         settings_inversion: Optional[aa.SettingsInversion] = None,
         use_preloaded_grid: bool = True,
-        use_hyper_scaling: bool = True,
     ):
         """
         Wraps a PyAutoFit aggregator in order to create generators of fits to imaging data, corresponding to the
         results of a non-linear search model-fit.
         """
         super().__init__(aggregator=aggregator)
 
-        self.settings_imaging = settings_imaging
+        self.settings_dataset = settings_dataset
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
         self.use_preloaded_grid = use_preloaded_grid
-        self.use_hyper_scaling = use_hyper_scaling
 
-    def make_object_for_gen(self, fit, galaxies) -> FItImaging:
+    def object_via_gen_from(self, fit, galaxies) -> FItImaging:
         """
         Creates a `FitImaging` object from a `ModelInstance` that contains the galaxies of a sample from a non-linear
         search.
 
         Parameters
         ----------
         fit
-            A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+            A PyAutoFit database Fit object containing the generators of the results of model-fits.
         galaxies
             A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
         Returns
         -------
         FitImaging
             A fit to imaging data whose galaxies are a sample of a PyAutoFit non-linear search.
         """
         return _fit_imaging_from(
             fit=fit,
             galaxies=galaxies,
-            settings_imaging=self.settings_imaging,
+            settings_dataset=self.settings_dataset,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             use_preloaded_grid=self.use_preloaded_grid,
-            use_hyper_scaling=self.use_hyper_scaling,
         )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/aggregator/fit_interferometer.py` & `autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_interferometer.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,111 +14,109 @@
 from autogalaxy.aggregator.plane import _plane_from
 
 
 def _fit_interferometer_from(
     fit: af.Fit,
     galaxies: List[Galaxy],
     real_space_mask: Optional[aa.Mask2D] = None,
-    settings_interferometer: aa.SettingsInterferometer = None,
+    settings_dataset: aa.SettingsInterferometer = None,
     settings_pixelization: aa.SettingsPixelization = None,
     settings_inversion: aa.SettingsInversion = None,
     use_preloaded_grid: bool = True,
 ) -> FitInterferometer:
     """
     Returns a `FitInterferometer` object from a PyAutoFit database `Fit` object and an instance of galaxies from a non-linear
     search model-fit.
 
-    This function adds the `hyper_model_image` and `hyper_galaxy_image_path_dict` to the galaxies before performing the
+    This function adds the `adapt_model_image` and `adapt_galaxy_image_path_dict` to the galaxies before performing the
     fit, if they were used.
 
     Parameters
     ----------
     fit
-        A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+        A PyAutoFit database Fit object containing the generators of the results of model-fits.
     galaxies
         A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
     Returns
     -------
     FitInterferometer
         The fit to the interferometer dataset computed via an instance of galaxies.
     """
     from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 
-    interferometer = _interferometer_from(
+    dataset = _interferometer_from(
         fit=fit,
         real_space_mask=real_space_mask,
-        settings_interferometer=settings_interferometer,
+        settings_dataset=settings_dataset,
     )
     plane = _plane_from(fit=fit, galaxies=galaxies)
 
     settings_pixelization = settings_pixelization or fit.value(
         name="settings_pixelization"
     )
     settings_inversion = settings_inversion or fit.value(name="settings_inversion")
 
     preloads = None
 
     if use_preloaded_grid:
-
         sparse_grids_of_planes = fit.value(name="preload_sparse_grids_of_planes")
 
         if sparse_grids_of_planes is not None:
-
             preloads = Preloads(sparse_image_plane_grid_pg_list=sparse_grids_of_planes)
 
     return FitInterferometer(
-        dataset=interferometer,
+        dataset=dataset,
         plane=plane,
         settings_pixelization=settings_pixelization,
         settings_inversion=settings_inversion,
         preloads=preloads,
     )
 
 
 class FitInterferometerAgg(AbstractAgg):
     def __init__(
         self,
         aggregator: af.Aggregator,
-        settings_interferometer: Optional[aa.SettingsInterferometer] = None,
+        settings_dataset: Optional[aa.SettingsInterferometer] = None,
         settings_pixelization: Optional[aa.SettingsPixelization] = None,
         settings_inversion: Optional[aa.SettingsInversion] = None,
         use_preloaded_grid: bool = True,
         real_space_mask: Optional[aa.Mask2D] = None,
     ):
         """
         Wraps a PyAutoFit aggregator in order to create generators of fits to interferometer data, corresponding to the
         results of a non-linear search model-fit.
         """
         super().__init__(aggregator=aggregator)
 
-        self.settings_interferometer = settings_interferometer
+        self.settings_dataset = settings_dataset
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
         self.use_preloaded_grid = use_preloaded_grid
         self.real_space_mask = real_space_mask
 
-    def make_object_for_gen(self, fit, galaxies) -> FitInterferometer:
+    def object_via_gen_from(self, fit, galaxies) -> FitInterferometer:
         """
         Creates a `FitInterferometer` object from a `ModelInstance` that contains the galaxies of a sample from a non-linear
         search.
 
         Parameters
         ----------
         fit
-            A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+            A PyAutoFit database Fit object containing the generators of the results of model-fits.
         galaxies
             A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
         Returns
         -------
         FitInterferometer
             A fit to interferometer data whose galaxies are a sample of a PyAutoFit non-linear search.
         """
         return _fit_interferometer_from(
             fit=fit,
             galaxies=galaxies,
-            settings_interferometer=self.settings_interferometer,
+            settings_dataset=self.settings_dataset,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             use_preloaded_grid=self.use_preloaded_grid,
         )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/aggregator/interferometer.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,71 @@
-from functools import partial
-from typing import Optional
+from typing import Tuple
 
-import autofit as af
-import autoarray as aa
+from autogalaxy.profiles.mass.stellar.sersic import Sersic
 
 
-def _interferometer_from(
-    fit: af.Fit,
-    real_space_mask: Optional[aa.Mask2D] = None,
-    settings_interferometer: Optional[aa.SettingsInterferometer] = None,
-):
-    """
-    Returns a `Interferometer` object from an aggregator's `SearchOutput` class, which we call an 'agg_obj' to
-    describe that it acts as the aggregator object for one result in the `Aggregator`. This uses the aggregator's
-    generator outputs such that the function can use the `Aggregator`'s map function to to create a
-    `Interferometer` generator.
-
-    The `Interferometer` is created following the same method as the PyAutoGalaxy `Search` classes, including
-    using the `SettingsInterferometer` instance output by the Search to load inputs of the `Interferometer`
-    (e.g. psf_shape_2d).
-
-    Parameters
-    ----------
-    fit : ImaginSearchOutput
-        A PyAutoFit aggregator's SearchOutput object containing the generators of the results of PyAutoGalaxy
-        model-fits.
-    """
-
-    data = fit.value(name="data")
-    noise_map = fit.value(name="noise_map")
-    uv_wavelengths = fit.value(name="uv_wavelengths")
-    real_space_mask = real_space_mask or fit.value(name="real_space_mask")
-    settings_interferometer = settings_interferometer or fit.value(
-        name="settings_dataset"
-    )
-
-    interferometer = aa.Interferometer(
-        visibilities=data,
-        noise_map=noise_map,
-        uv_wavelengths=uv_wavelengths,
-        real_space_mask=real_space_mask,
-    )
-
-    interferometer = interferometer.apply_settings(settings=settings_interferometer)
-
-    return interferometer
-
+class DevVaucouleurs(Sersic):
+    def __init__(
+        self,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        ell_comps: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 0.1,
+        effective_radius: float = 0.6,
+        mass_to_light_ratio: float = 1.0,
+    ):
+        """
+        The DevVaucouleurs mass profile, the mass profiles of the light profiles that are used to fit and
+        subtract the lens model_galaxy's light.
 
-class InterferometerAgg:
-    def __init__(self, aggregator: af.Aggregator):
+        Parameters
+        ----------
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        ell_comps
+            The first and second ellipticity components of the elliptical coordinate system.
+        intensity
+            Overall flux intensity normalisation in the light profiles (electrons per second).
+        effective_radius
+            The radius containing half the light of this profile.
+        mass_to_light_ratio
+            The mass-to-light ratio of the light profile.
+        """
+        super().__init__(
+            centre=centre,
+            ell_comps=ell_comps,
+            intensity=intensity,
+            effective_radius=effective_radius,
+            sersic_index=4.0,
+            mass_to_light_ratio=mass_to_light_ratio,
+        )
 
-        self.aggregator = aggregator
 
-    def interferometer_gen_from(
+class DevVaucouleursSph(DevVaucouleurs):
+    def __init__(
         self,
-        real_space_mask: Optional[aa.Mask2D] = None,
-        settings_interferometer: Optional[aa.SettingsInterferometer] = None,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 0.1,
+        effective_radius: float = 0.6,
+        mass_to_light_ratio: float = 1.0,
     ):
         """
-        Returns a generator of `Interferometer` objects from an input aggregator, which generates a list of the
-        `Interferometer` objects for every set of results loaded in the aggregator.
-
-        This is performed by mapping the `interferometer_from_agg_obj` with the aggregator, which sets up each
-        interferometer object using only generators ensuring that manipulating the interferometer objects of large
-        sets of results is done in a memory efficient  way.
+        The DevVaucouleurs mass profile, the mass profiles of the light profiles that are used to fit and subtract the
+        lens model_galaxy's light.
 
         Parameters
         ----------
-        aggregator : ImaginAggregator
-            A PyAutoFit aggregator object containing the results of PyAutoGalaxy model-fits."""
-
-        func = partial(
-            _interferometer_from,
-            real_space_mask=real_space_mask,
-            settings_interferometer=settings_interferometer,
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        intensity
+            Overall flux intensity normalisation in the light profiles (electrons per second).
+        effective_radius
+            The circular radius containing half the light of this profile.
+        mass_to_light_ratio
+            The mass-to-light ratio of the light profiles.
+        """
+        super().__init__(
+            centre=centre,
+            ell_comps=(0.0, 0.0),
+            intensity=intensity,
+            effective_radius=effective_radius,
+            mass_to_light_ratio=mass_to_light_ratio,
         )
-
-        return self.aggregator.map(func=func)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/aggregator/plane.py` & `autogalaxy-2023.7.7.1/autogalaxy/aggregator/plane.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,72 +11,70 @@
 
 
 def _plane_from(fit: af.Fit, galaxies: List[Galaxy]) -> Plane:
     """
     Returns a `Plane` object from a PyAutoFit database `Fit` object and an instance of galaxies from a non-linear
     search model-fit.
 
-    This function adds the `hyper_model_image` and `hyper_galaxy_image_path_dict` to the galaxies before constructing
+    This function adds the `adapt_model_image` and `adapt_galaxy_image_path_dict` to the galaxies before constructing
     the `Plane`, if they were used.
 
     Parameters
     ----------
     fit
-        A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+        A PyAutoFit database Fit object containing the generators of the results of model-fits.
     galaxies
         A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
     Returns
     -------
     Plane
         The plane computed via an instance of galaxies.
     """
 
     from autogalaxy.galaxy.galaxy import Galaxy
     from autogalaxy.plane.plane import Plane
 
-    hyper_model_image = fit.value(name="hyper_model_image")
-    hyper_galaxy_image_path_dict = fit.value(name="hyper_galaxy_image_path_dict")
+    adapt_model_image = fit.value(name="adapt_model_image")
+    adapt_galaxy_image_path_dict = fit.value(name="adapt_galaxy_image_path_dict")
 
-    galaxies_with_hyper = []
-
-    if hyper_galaxy_image_path_dict is not None:
+    galaxies_with_adapt = []
 
+    if adapt_galaxy_image_path_dict is not None:
         galaxy_path_list = [
             gal[0] for gal in fit.instance.path_instance_tuples_for_class(Galaxy)
         ]
 
-        for (galaxy_path, galaxy) in zip(galaxy_path_list, galaxies):
-
-            if galaxy_path in hyper_galaxy_image_path_dict:
-                galaxy.hyper_model_image = hyper_model_image
-                galaxy.hyper_galaxy_image = hyper_galaxy_image_path_dict[galaxy_path]
+        for galaxy_path, galaxy in zip(galaxy_path_list, galaxies):
+            if galaxy_path in adapt_galaxy_image_path_dict:
+                galaxy.adapt_model_image = adapt_model_image
+                galaxy.adapt_galaxy_image = adapt_galaxy_image_path_dict[galaxy_path]
 
-            galaxies_with_hyper.append(galaxy)
+            galaxies_with_adapt.append(galaxy)
 
-        return Plane(galaxies=galaxies_with_hyper)
+        return Plane(galaxies=galaxies_with_adapt)
 
     return Plane(galaxies=galaxies)
 
 
 class PlaneAgg(AbstractAgg):
     """
     Wraps a PyAutoFit aggregator in order to create generators of planes corresponding to the results of a non-linear
     search model-fit.
     """
 
-    def make_object_for_gen(self, fit, galaxies) -> Plane:
+    def object_via_gen_from(self, fit, galaxies) -> Plane:
         """
         Creates a `Plane` object from a `ModelInstance` that contains the galaxies of a sample from a non-linear
         search.
 
         Parameters
         ----------
         fit
-            A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+            A PyAutoFit database Fit object containing the generators of the results of model-fits.
         galaxies
             A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
         Returns
         -------
         Plane
             A plane whose galaxies are a sample of a PyAutoFit non-linear search.
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/analysis/analysis.py` & `autogalaxy-2023.7.7.1/autogalaxy/analysis/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import autoarray as aa
 
 from autogalaxy import exc
 from autogalaxy.analysis.maker import FitMaker
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.cosmology.lensing import LensingCosmology
 from autogalaxy.cosmology.wrap import Planck15
-from autogalaxy.hyper.hyper_data import HyperImageSky
-from autogalaxy.hyper.hyper_data import HyperBackgroundNoise
 from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.plane.plane import Plane
 from autogalaxy.analysis.result import ResultDataset
 
 from autogalaxy.analysis import model_util
 
 logger = logging.getLogger(__name__)
@@ -31,15 +29,15 @@
     def __init__(self, cosmology: LensingCosmology = Planck15):
         """
         Analysis classes are used by PyAutoFit to fit a model to a dataset via a non-linear search.
 
         This abstract Analysis class for all model-fits which fit galaxies (or objects containing galaxies like a
         plane), but does not perform a model-fit by itself (and is therefore only inherited from).
 
-        This class stores the Cosmology used for the analysis and hyper datasets used for certain model classes.
+        This class stores the Cosmology used for the analysis and adapt datasets used for certain model classes.
 
         Parameters
         ----------
         cosmology
             The AstroPy Cosmology assumed for this analysis.
         """
         self.cosmology = cosmology
@@ -63,56 +61,54 @@
         return Plane(galaxies=instance.galaxies)
 
 
 class AnalysisDataset(Analysis):
     def __init__(
         self,
         dataset: Union[aa.Imaging, aa.Interferometer],
-        hyper_dataset_result: ResultDataset = None,
+        adapt_result: ResultDataset = None,
         cosmology: LensingCosmology = Planck15(),
         settings_pixelization: aa.SettingsPixelization = None,
         settings_inversion: aa.SettingsInversion = None,
     ):
         """
         Abstract Analysis class for all model-fits which fit galaxies (or objects containing galaxies like a plane)
         to a dataset, like imaging or interferometer data.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. a
-        pixelization or inversion), the Cosmology used for the analysis and hyper datasets used for certain model
+        pixelization or inversion), the Cosmology used for the analysis and adapt datasets used for certain model
         classes.
 
         Parameters
         ----------
         dataset
             The dataset that is the model is fitted too.
-        hyper_dataset_result
-            The hyper-model image and hyper galaxies images of a previous result in a model-fitting pipeline, which are
+        adapt_result
+            The adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
             used by certain classes for adapting the analysis to the properties of the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         settings_pixelization
             settings controlling how a pixelization is fitted during the model-fit, for example if a border is used
             when creating the pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted during the model-fit, for example which linear algebra
             formalism is used.
         """
         super().__init__(cosmology=cosmology)
 
         self.dataset = dataset
-        self.hyper_dataset_result = hyper_dataset_result
+        self.adapt_result = adapt_result
 
-        if self.hyper_dataset_result is not None:
-
-            self.set_hyper_dataset(result=self.hyper_dataset_result)
+        if self.adapt_result is not None:
+            self.set_adapt_dataset(result=self.adapt_result)
 
         else:
-
-            self.hyper_galaxy_image_path_dict = None
-            self.hyper_model_image = None
+            self.adapt_galaxy_image_path_dict = None
+            self.adapt_model_image = None
 
         self.settings_pixelization = settings_pixelization or aa.SettingsPixelization()
         self.settings_inversion = settings_inversion or aa.SettingsInversion()
 
         self.preloads = self.preloads_cls()
 
     def modify_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
@@ -132,42 +128,42 @@
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
             visualization and the pickled objects used by the aggregator output by this function.
         model
             The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
             the imaging data.
         """
 
-        self.check_and_replace_hyper_images(paths=paths)
+        self.check_and_replace_adapt_images(paths=paths)
 
         model_util.set_upper_limit_of_pixelization_pixels_prior(
             model=model, pixels_in_mask=self.dataset.mask.pixels_in_mask
         )
 
-    def set_hyper_dataset(self, result: ResultDataset) -> None:
+    def set_adapt_dataset(self, result: ResultDataset) -> None:
         """
-        Using a the result of a previous model-fit, set the hyper-dataset for this analysis. This is used to adapt
+        Using a the result of a previous model-fit, set the adapt-dataset for this analysis. This is used to adapt
         aspects of the model (e.g. the pixelization, regularization scheme) to the properties of the dataset being
         fitted.
 
-        This passes the hyper model image and hyper galaxy images of the previous fit. These represent where different
+        This passes the adapt image and galaxy images of the previous fit. These represent where different
         galaxies in the dataset are located and thus allows the fit to adapt different aspects of the model to different
         galaxies in the data.
 
         Parameters
         ----------
         result
             The result of a previous model-fit which contains the model image and model galaxy images of a fit to
-            the dataset, which set up the hyper dataset. These are used by certain classes for adapting the analysis
+            the dataset, which set up the adapt dataset. These are used by certain classes for adapting the analysis
             to the properties of the dataset.
         """
-        hyper_galaxy_image_path_dict = result.hyper_galaxy_image_path_dict
-        hyper_model_image = result.hyper_model_image
+        adapt_galaxy_image_path_dict = result.adapt_galaxy_image_path_dict
+        adapt_model_image = result.adapt_model_image
 
-        self.hyper_galaxy_image_path_dict = hyper_galaxy_image_path_dict
-        self.hyper_model_image = hyper_model_image
+        self.adapt_galaxy_image_path_dict = adapt_galaxy_image_path_dict
+        self.adapt_model_image = adapt_model_image
 
     @property
     def preloads_cls(self):
         return Preloads
 
     @property
     def fit_maker_cls(self):
@@ -212,15 +208,14 @@
             self.preloads = self.preloads_cls(failed=True)
         else:
             self.preloads = self.preloads_cls.setup_all_via_fits(
                 fit_0=fit_0, fit_1=fit_1
             )
 
             if conf.instance["general"]["test"]["check_preloads"]:
-
                 self.preloads.check_via_fit(fit=fit_0)
 
         self.preloads.output_info_to_summary(file_path=paths.profile_path)
 
     def modify_after_fit(
         self, paths: af.DirectoryPaths, model: af.AbstractPriorModel, result: af.Result
     ) -> "AnalysisDataset":
@@ -237,67 +232,26 @@
             The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
             the imaging data.
         result
             The result of the model fit that has just been completed.
         """
 
         self.output_or_check_figure_of_merit_sanity(paths=paths, result=result)
-        self.preloads.reset_all()
 
         return self
 
-    def hyper_image_sky_via_instance_from(
-        self, instance: af.ModelInstance
-    ) -> Optional[HyperImageSky]:
-        """
-        If the model instance contains a `HyperImageSky` attribute, which adds a free parameter to the model that
-        scales the background sky, return this attribute. Otherwise a None is returned.
-
-        Parameters
-        ----------
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-
-        Returns
-        -------
-        An instance of the hyper image sky class that scales the sky background.
-        """
-        if hasattr(instance, "hyper_image_sky"):
-            return instance.hyper_image_sky
-
-    def hyper_background_noise_via_instance_from(
-        self, instance: af.ModelInstance
-    ) -> Optional[HyperBackgroundNoise]:
-        """
-        If the model instance contains a `HyperBackgroundNoise` attribute, which adds a free parameter to the model that
-        scales the background noise, return this attribute. Otherwise a None is returned.
-
-        Parameters
-        ----------
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-
-        Returns
-        -------
-        An instance of the hyper background noise class that scales the background noise.
-        """
-        if hasattr(instance, "hyper_background_noise"):
-            return instance.hyper_background_noise
-
-    def instance_with_associated_hyper_images_from(
+    def instance_with_associated_adapt_images_from(
         self, instance: af.ModelInstance
     ) -> af.ModelInstance:
         """
-        Using the model image and galaxy images that were set up as the hyper dataset, associate the galaxy images
+        Using the model image and galaxy images that were set up as the adapt dataset, associate the galaxy images
         of that result with the galaxies in this model fit.
 
         Association is performed based on galaxy names, whereby if the name of a galaxy in this search matches the
-        full-path name of galaxies in the hyper dataset the galaxy image is passed.
+        full-path name of galaxies in the adapt dataset the galaxy image is passed.
 
         If the galaxy collection has a different name then an association is not made.
 
         For example, `galaxies.lens` will match with:
             `galaxies.lens`
         but not with:
             `galaxies.source`
@@ -310,42 +264,40 @@
 
         Returns
         -------
         instance
            The input instance with images associated with galaxies where possible.
         """
 
-        if self.hyper_galaxy_image_path_dict is not None:
-
+        if self.adapt_galaxy_image_path_dict is not None:
             for galaxy_path, galaxy in instance.path_instance_tuples_for_class(Galaxy):
-                if galaxy_path in self.hyper_galaxy_image_path_dict:
+                if galaxy_path in self.adapt_galaxy_image_path_dict:
+                    galaxy.adapt_model_image = self.adapt_model_image
 
-                    galaxy.hyper_model_image = self.hyper_model_image
-
-                    galaxy.hyper_galaxy_image = self.hyper_galaxy_image_path_dict[
+                    galaxy.adapt_galaxy_image = self.adapt_galaxy_image_path_dict[
                         galaxy_path
                     ]
 
         return instance
 
     def save_attributes_for_aggregator(self, paths: af.DirectoryPaths):
         """
         Before the model-fit via the non-linear search begins, this routine saves attributes of the `Analysis` object
-        to the `pickles` folder such that they can be load after the analysis using PyAutoFit's database and aggregator
+        to the `pickles` folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator
         tools.
 
         For this analysis the following are output:
 
         - The dataset's data.
         - The dataset's noise-map.
         - The settings associated with the dataset.
         - The settings associated with the inversion.
         - The settings associated with the pixelization.
         - The Cosmology.
-        - The hyper dataset's model image and galaxy images, if used.
+        - The adapt dataset's model image and galaxy images, if used.
 
         It is common for these attributes to be loaded by many of the template aggregator functions given in the
         `aggregator` modules. For example, when using the database tools to reperform a fit, this will by default
         load the dataset, settings and other attributes necessary to perform a fit using the attributes output by
         this function.
 
         Parameters
@@ -358,53 +310,52 @@
         paths.save_object("noise_map", self.dataset.noise_map)
         paths.save_object("settings_dataset", self.dataset.settings)
         paths.save_object("settings_inversion", self.settings_inversion)
         paths.save_object("settings_pixelization", self.settings_pixelization)
 
         paths.save_object("cosmology", self.cosmology)
 
-        if self.hyper_model_image is not None:
-            paths.save_object("hyper_model_image", self.hyper_model_image)
+        if self.adapt_model_image is not None:
+            paths.save_object("adapt_model_image", self.adapt_model_image)
 
-        if self.hyper_galaxy_image_path_dict is not None:
+        if self.adapt_galaxy_image_path_dict is not None:
             paths.save_object(
-                "hyper_galaxy_image_path_dict", self.hyper_galaxy_image_path_dict
+                "adapt_galaxy_image_path_dict", self.adapt_galaxy_image_path_dict
             )
 
-    def check_and_replace_hyper_images(self, paths: af.DirectoryPaths):
+    def check_and_replace_adapt_images(self, paths: af.DirectoryPaths):
         """
-        Using a the result of a previous model-fit, a hyper-dataset can be set up which adapts aspects of the model
+        Using a the result of a previous model-fit, a adapt-dataset can be set up which adapts aspects of the model
         (e.g. the pixelization, regularization scheme) to the properties of the dataset being fitted.
 
         If the model-fit is being resumed from a previous run, this function checks that the model image and galaxy
-        images used to set up the hyper-dataset are identical to those used previously. If they are not, it replaces
-        them with the previous hyper image. This ensures consistency in the log likelihood function.
+        images used to set up the adapt-dataset are identical to those used previously. If they are not, it replaces
+        them with the previous adapt image. This ensures consistency in the log likelihood function.
 
         Parameters
         ----------
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
             visualization and the pickled objects used by the aggregator output by this function.
         """
         try:
-            hyper_model_image = paths.load_object("hyper_model_image")
-
-            if np.max(abs(hyper_model_image - self.hyper_model_image)) > 1e-8:
+            adapt_model_image = paths.load_object("adapt_model_image")
 
+            if np.max(abs(adapt_model_image - self.adapt_model_image)) > 1e-8:
                 logger.info(
-                    "ANALYSIS - Hyper image loaded from pickle different to that set in Analysis class."
-                    "Overwriting hyper images with values loaded from pickles."
+                    "ANALYSIS - adapt image loaded from pickle different to that set in Analysis class."
+                    "Overwriting adapt images with values loaded from pickles."
                 )
 
-                self.hyper_model_image = hyper_model_image
+                self.adapt_model_image = adapt_model_image
 
-                hyper_galaxy_image_path_dict = paths.load_object(
-                    "hyper_galaxy_image_path_dict"
+                adapt_galaxy_image_path_dict = paths.load_object(
+                    "adapt_galaxy_image_path_dict"
                 )
-                self.hyper_galaxy_image_path_dict = hyper_galaxy_image_path_dict
+                self.adapt_galaxy_image_path_dict = adapt_galaxy_image_path_dict
 
         except (
             FileNotFoundError,
             AttributeError,
             KeyError,
             ModuleNotFoundError,
             TypeError,
@@ -447,27 +398,23 @@
         figure_of_merit = result.max_log_likelihood_fit.figure_of_merit
 
         figure_of_merit_sanity_file = path.join(
             paths.output_path, "figure_of_merit_sanity.json"
         )
 
         if not path.exists(figure_of_merit_sanity_file):
-
             with open(figure_of_merit_sanity_file, "w+") as f:
                 json.dump(figure_of_merit, f)
 
         else:
-
             with open(figure_of_merit_sanity_file) as json_file:
                 figure_of_merit_sanity = json.load(json_file)
 
             if conf.instance["general"]["test"]["check_figure_of_merit_sanity"]:
-
                 if not np.isclose(figure_of_merit, figure_of_merit_sanity):
-
                     raise exc.AnalysisException(
                         "Figure of merit sanity check failed. "
                         ""
                         "This means that the existing results of a model fit used a different "
                         "likelihood function compared to the one implemented now.\n\n"
                         f"Old Figure of Merit = {figure_of_merit_sanity}\n"
                         f"New Figure of Merit = {figure_of_merit}"
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/analysis/clump_model.py` & `autogalaxy-2023.7.7.1/autogalaxy/analysis/clump_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     def __init__(
         self,
         redshift: float,
         centres: aa.Grid2DIrregular,
         light_cls: Optional[Type[LightProfile]] = None,
         mass_cls: Optional[Type[MassProfile]] = None,
         einstein_radius_upper_limit: Optional[float] = None,
+        unfix_centres: bool = False,
     ):
         """
         The clump API allows creates model components which model the light and mass of galaxies that are nearby the
         main galaxy(s) of interest.
 
         The `ClumpModel` object handles the creation of these model components to streamline model composition with
         multiple clumps.
@@ -40,63 +41,87 @@
         light_cls
             The light profile given to all clumps; if omitted all clumps have no light profile.
         mass_cls
             The mass profile given to all clumps; if omitted all clumps have no mass profile.
         einstein_radius_upper_limit
             The upper limit given to any mass model's `einstein_radius` parameter (e.g. if `IsothermalSph` profiles
             are used to model clumps).
+        unfix_centres
+            If required, change the mass and light centres from fixed values to Uniform Prior Models +/- 0.1 around
+            the input centres.
         """
         self.redshift = redshift
         self.centres = centres
 
         self.light_cls = light_cls
         self.mass_cls = mass_cls
 
         self.einstein_radius_upper_limit = einstein_radius_upper_limit
+        self.unfix_centres = unfix_centres
+
+        self.centre_prior_half_width = 0.1
 
     @property
     def total_clumps(self) -> int:
         return len(self.centres.in_list)
 
+    def unfix_centre(obj, centre):
+        obj.centre.centre_0 = af.UniformPrior(
+            lower_limit=new_centre[0] - centre_prior_half_width,
+            upper_limit=new_centre[0] + centre_prior_half_width,
+        )
+        obj.centre.centre_1 = af.UniformPrior(
+            lower_limit=new_centre[1] - centre_prior_half_width,
+            upper_limit=new_centre[1] + centre_prior_half_width,
+        )
+        return obj
+
     @property
     def light_list(self) -> Optional[List[af.Model]]:
         """
         Returns a list of every clump's light model, where the centre of that light model is fixed to its corresponding
-        input clump's centre.
+        input clump's centre, unless specified to be free.
         """
         if self.light_cls is None:
             return None
 
-        return [
-            af.Model(self.light_cls, centre=centre) for centre in self.centres.in_list
-        ]
+        light_list = []
+
+        for centre in self.centres.in_list:
+            if self.unfix_centres:
+                light_list.append(unfix_centre(af.Model(self.light_cls), centre))
+            else:
+                light_list.append(af.Model(self.light_cls, centre=centre))
+
+        return light_list
 
     @property
     def mass_list(self) -> Optional[List[af.Model]]:
         """
         Returns a list of every clump's mass model, where the centre of that mass model is fixed to its corresponding
-        input clump's centre.
+        input clump's centre, unless specified to be free.
         """
         if self.mass_cls is None:
             return None
 
         mass_list = []
 
         for centre in self.centres.in_list:
-
-            mass = af.Model(self.mass_cls, centre=centre)
+            if self.unfix_centres:
+                mass = unfix_centres(af.Model(self.mass_cls), centre)
+            else:
+                mass = af.Model(self.mass_cls, centre=centre)
 
             if (
                 hasattr(mass, "einstein_radius")
                 and self.einstein_radius_upper_limit is not None
             ):
                 mass.einstein_radius = af.UniformPrior(
                     lower_limit=0.0, upper_limit=self.einstein_radius_upper_limit
                 )
-
             mass_list.append(mass)
 
         return mass_list
 
     @property
     def clumps_light_only(self) -> af.Collection:
         """
@@ -105,15 +130,14 @@
 
         All clumps only contain their model mass profiles, which is important for certain pipelines which omit
         the clump mass profiles.
         """
         clumps_light_only = {}
 
         for i in range(self.total_clumps):
-
             light = self.light_list[i] if self.light_cls is not None else None
 
             clumps_light_only[f"clump_{i}"] = af.Model(
                 Galaxy, redshift=self.redshift, light=light
             )
 
         return af.Collection(**clumps_light_only)
@@ -126,15 +150,14 @@
 
         All clumps only contain their model mass profiles, which is important for certain pipelines which omit
         the clump light profiles.
         """
         clumps_mass_only = {}
 
         for i in range(self.total_clumps):
-
             mass = self.mass_list[i] if self.mass_cls is not None else None
 
             clumps_mass_only[f"clump_{i}"] = af.Model(
                 Galaxy, redshift=self.redshift, mass=mass
             )
 
         return af.Collection(**clumps_mass_only)
@@ -150,28 +173,26 @@
         input redshift.
 
         The keys of this dictionary are numerically ordered as `clump_0`, `clump_2` etc.
         """
         clumps = {}
 
         for i in range(self.total_clumps):
-
             light = self.light_list[i] if self.light_cls is not None else None
             mass = self.mass_list[i] if self.mass_cls is not None else None
 
             clumps[f"clump_{i}"] = af.Model(
                 Galaxy, redshift=self.redshift, light=light, mass=mass
             )
 
         return af.Collection(**clumps)
 
 
 class ClumpModelDisabled:
     def __init__(self):
-
         pass
 
     @property
     def clumps_light_only(self):
         return af.Collection()
 
     @property
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/analysis/maker.py` & `autogalaxy-2023.7.7.1/autogalaxy/analysis/maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,26 +111,23 @@
         fit
             A fit object where an instance of the model has been fitted to the data.
         """
 
         preload_attempts = conf.instance["general"]["analysis"]["preload_attempts"]
 
         for i in range(preload_attempts):
-
             try:
-
                 instance = self.model.random_instance(ignore_prior_limits=True)
 
                 # The use_w_tilde here is for speed, incase noise scalin is on.
 
                 fit = self.fit_func(
                     instance=instance,
                     preload_overwrite=self.preloads_cls(use_w_tilde=False),
                 )
 
                 fit.figure_of_merit
 
                 return fit
 
             except Exception as e:
-
                 continue
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/analysis/preloads.py` & `autogalaxy-2023.7.7.1/autogalaxy/analysis/preloads.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,19 +18,17 @@
         use_w_tilde: Optional[bool] = None,
         blurred_image: Optional[aa.Array2D] = None,
         sparse_image_plane_grid_pg_list: Optional[List[List[aa.Grid2D]]] = None,
         relocated_grid: Optional[aa.Grid2D] = None,
         mapper_list: Optional[aa.AbstractMapper] = None,
         mapper_galaxy_dict: Optional[Dict[aa.AbstractMapper, "Galaxy"]] = None,
         linear_func_operated_mapping_matrix_dict=None,
-        linear_func_weighted_mapping_vectors_dict=None,
-        linear_func_curvature_vectors_dict=None,
+        data_linear_func_matrix_dict=None,
+        mapper_operated_mapping_matrix_dict=None,
         operated_mapping_matrix: Optional[np.ndarray] = None,
-        curvature_matrix_preload: Optional[np.ndarray] = None,
-        curvature_matrix_counts: Optional[np.ndarray] = None,
         curvature_matrix: Optional[np.ndarray] = None,
         regularization_matrix: Optional[np.ndarray] = None,
         log_det_regularization_matrix_term: Optional[float] = None,
         traced_sparse_grids_list_of_planes=None,
         sparse_image_plane_grid_list=None,
         failed=False,
     ):
@@ -44,19 +42,19 @@
         via a KMeans algorithm) does not change for the majority of model-fits, because the associated model parameters
         are fixed. Preloading avoids rerruning the KMeans algorithm for every model fitted, by preloading it in memory
         and using this preload in every fit.
 
         Parameters
         ----------
         blurred_image
-            The preloaded array of values containing the blurred image of a lens model fit (e.g. that light profile of
+            The preloaded array of values containing the blurred image of a model fit (e.g. that light profile of
             every galaxy in the model). This can be preloaded when no light profiles in the model vary.
         w_tilde
             A class containing values that enable an inversion's linear algebra to use the w-tilde formalism. This can
-            be preloaded when no component of the model changes the noise map (e.g. hyper galaxies are fixed).
+            be preloaded when no component of the model changes the noise map (e.g. galaxies are fixed).
         use_w_tilde
             Whether to use the w tilde formalism, which superseeds the value in `SettingsInversions` such that w tilde
             will be disabled for model-fits it is not applicable (e.g. because the noise-map changes).
         traced_grids_of_planes_for_inversion
             The two dimensional grids corresponding to the traced grids in a lens fit. This can be preloaded when no
              mass profiles in the model vary.
         sparse_image_plane_grid_pg_list
@@ -68,38 +66,29 @@
             pixelization in a lens fit. This can be preloaded when no mass profiles in the model vary.
         mapper_list
             The mapper of a fit, which preloading avoids recalculation of the mapping matrix and image to source
             pixel mappings. This can be preloaded when no pixelizations in the model vary.
         operated_mapping_matrix
             A matrix containing the mappings between PSF blurred image pixels and source pixels used in the linear
             algebra of an inversion. This can be preloaded when no mass profiles and pixelizations in the model vary.
-        curvature_matrix_preload
-            A matrix containing preloaded value used to construct the curvature matrix from the blurred mapping matrix.
-            This can be preloaded when no mass profiles and pixelizations in the model vary.
-        curvature_matrix_counts
-            A matrix containing the length of values in the curvature matrix preloaded, which are used to construct
-            the curvature matrix from the blurred mapping matrix. This can be preloaded when no mass profiles and
-            pixelizations in the model vary.
 
         Returns
         -------
         The preloads object used to skip certain calculations in the log likelihood function.
         """
         super().__init__(
             w_tilde=w_tilde,
             use_w_tilde=use_w_tilde,
             relocated_grid=relocated_grid,
             sparse_image_plane_grid_pg_list=sparse_image_plane_grid_pg_list,
             mapper_list=mapper_list,
             linear_func_operated_mapping_matrix_dict=linear_func_operated_mapping_matrix_dict,
-            linear_func_weighted_mapping_vectors_dict=linear_func_weighted_mapping_vectors_dict,
-            linear_func_curvature_vectors_dict=linear_func_curvature_vectors_dict,
+            data_linear_func_matrix_dict=data_linear_func_matrix_dict,
+            mapper_operated_mapping_matrix_dict=mapper_operated_mapping_matrix_dict,
             operated_mapping_matrix=operated_mapping_matrix,
-            curvature_matrix_preload=curvature_matrix_preload,
-            curvature_matrix_counts=curvature_matrix_counts,
             curvature_matrix=curvature_matrix,
             regularization_matrix=regularization_matrix,
             log_det_regularization_matrix_term=log_det_regularization_matrix_term,
             traced_sparse_grids_list_of_planes=traced_sparse_grids_list_of_planes,
             sparse_image_plane_grid_list=sparse_image_plane_grid_list,
         )
 
@@ -125,22 +114,20 @@
             Preloads which are set up based on the fit's passed in specific to a lens model.
 
         """
 
         preloads = cls()
 
         if isinstance(fit_0, aa.FitImaging):
-
             preloads.set_w_tilde_imaging(fit_0=fit_0, fit_1=fit_1)
             preloads.set_blurred_image(fit_0=fit_0, fit_1=fit_1)
 
         preloads.set_mapper_list(fit_0=fit_0, fit_1=fit_1)
 
         if preloads.mapper_list is not None:
-
             preloads.mapper_galaxy_dict = fit_0.plane_to_inversion.mapper_galaxy_dict
 
         preloads.set_operated_mapping_matrix_with_preloads(fit_0=fit_0, fit_1=fit_1)
         preloads.set_linear_func_inversion_dicts(fit_0=fit_0, fit_1=fit_1)
         preloads.set_curvature_matrix(fit_0=fit_0, fit_1=fit_1)
         preloads.set_regularization_matrix_and_term(fit_0=fit_0, fit_1=fit_1)
 
@@ -167,62 +154,38 @@
         self.blurred_image = None
 
         precision = 1e-8
 
         if (np.max(abs(fit_0.blurred_image - fit_1.blurred_image)) < precision) and (
             np.sum(fit_0.blurred_image) > precision
         ):
-
             self.blurred_image = fit_0.blurred_image
 
             logger.info(
                 "PRELOADS - Blurred image (e.g. the image of all light profiles) is preloaded for this model-fit."
             )
 
     def output_info_to_summary(self, file_path):
-
         file_preloads = path.join(file_path, "preloads.summary")
 
         if self.failed:
-
             logger.info(
                 "PRELOADS - Preloading failed as models gave too many exceptions, preloading therefore "
                 "not used."
             )
 
             af.formatter.output_list_of_strings_to_file(
                 file=file_preloads, list_of_strings=["FAILED"]
             )
 
         else:
-
             af.formatter.output_list_of_strings_to_file(
                 file=file_preloads, list_of_strings=self.info
             )
 
-    def reset_all(self):
-        """
-        Reset all preloads, typically done at the end of a model-fit to save memory.
-        """
-        self.w_tilde = None
-
-        self.blurred_image = None
-        self.sparse_image_plane_grid_pg_list = None
-        self.relocated_grid = None
-        self.mapper = None
-        self.operated_mapping_matrix = None
-        self.linear_func_operated_mapping_matrix_dict = None
-        self.linear_func_weighted_mapping_vectors_dict = None
-        self.linear_func_curvature_vectors_dict = None
-        self.curvature_matrix_preload = None
-        self.curvature_matrix_counts = None
-        self.curvature_matrix = None
-        self.regularization_matrix = None
-        self.log_det_regularization_matrix_term = None
-
     @property
     def info(self) -> List[str]:
         """
         The information on what has or has not been preloaded, which is written to the file `preloads.summary`.
 
         Returns
         -------
@@ -234,17 +197,14 @@
         line += [f"Mapper = {self.mapper_list is not None}\n"]
         line += [
             f"Blurred Mapping Matrix = {self.operated_mapping_matrix is not None}\n"
         ]
         line += [
             f"Inversion Linear Func (Linear Light Profile) Dicts = {self.linear_func_operated_mapping_matrix_dict is not None}\n"
         ]
-        line += [
-            f"Curvature Matrix Sparse = {self.curvature_matrix_preload is not None}\n"
-        ]
         line += [f"Curvature Matrix = {self.curvature_matrix is not None}\n"]
         line += [
             f"Curvature Matrix Mapper Diag = {self.curvature_matrix_mapper_diag is not None}\n"
         ]
         line += [f"Regularization Matrix = {self.regularization_matrix is not None}\n"]
         line += [
             f"Log Det Regularization Matrix Term = {self.log_det_regularization_matrix_term is not None}\n"
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/analysis/result.py` & `autogalaxy-2023.7.7.1/autogalaxy/analysis/result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import numpy as np
-from typing import Dict, List, Type, Union
+from typing import Dict, List, Tuple, Type, Union
 
 from autoconf import conf
 import autofit as af
 import autoarray as aa
 
 from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.plane.plane import Plane
@@ -20,15 +20,15 @@
 
         - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
           an instance of the maximum log likelihood model).
 
         - The non-linear search used to perform the model fit.
 
         This class contains a number of methods which use the above objects to create the max log likelihood `Plane`,
-        `FitIamging`, hyper-galaxy images,etc.
+        `FitIamging`, adapt-galaxy images,etc.
 
         Parameters
         ----------
         samples
             A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
             run of samples of the nested sampler.
         model
@@ -60,33 +60,32 @@
 
         Returns
         -------
         A deep copy of the instance of the max log likelihood result.
         """
 
         if self.__instance is None:
-
             self.__instance = copy.deepcopy(self.instance)
 
         return self.__instance
 
     @property
     def max_log_likelihood_plane(self) -> Plane:
         """
         An instance of a `Plane` corresponding to the maximum log likelihood model inferred by the non-linear search.
         """
 
-        instance = self.analysis.instance_with_associated_hyper_images_from(
+        instance = self.analysis.instance_with_associated_adapt_images_from(
             instance=self.instance_copy
         )
 
         return self.analysis.plane_via_instance_from(instance=instance)
 
     @property
-    def path_galaxy_tuples(self) -> [(str, Galaxy)]:
+    def path_galaxy_tuples(self) -> List[Tuple[str, Galaxy]]:
         """
         Tuples associating the names of galaxies with instances from the best fit
         """
         return self.instance_copy.path_instance_tuples_for_class(cls=Galaxy)
 
 
 class ResultDataset(Result):
@@ -115,77 +114,76 @@
         """
         The dataset that was fitted by the model-fit.
         """
         return self.max_log_likelihood_fit.dataset
 
     def image_for_galaxy(self, galaxy: Galaxy) -> np.ndarray:
         """
-        Given an instance of a `Galaxy` object, return an image of the galaxy via the the maximum log likelihood fit.
+        Given an instance of a `Galaxy` object, return an image of the galaxy via the maximum log likelihood fit.
 
         This image is extracted via the fit's `galaxy_model_image_dict`, which is necessary to make it straight
-        forward to use the image as hyper-images.
+        forward to use the image as adapt-images.
 
         Parameters
         ----------
         galaxy
             A galaxy used by the model-fit.
 
         Returns
         -------
         ndarray or None
             A numpy arrays giving the model image of that galaxy.
         """
         return self.max_log_likelihood_fit.galaxy_model_image_dict[galaxy]
 
     @property
-    def image_galaxy_dict(self) -> {str: Galaxy}:
+    def image_galaxy_dict(self) -> Dict[str, Galaxy]:
         """
         A dictionary associating galaxy names with model images of those galaxies.
 
-        This is used for creating the hyper-dataset used by Analysis objects to adapt aspects of a model to the dataset
+        This is used for creating the adapt-dataset used by Analysis objects to adapt aspects of a model to the dataset
         being fitted.
         """
         return {
             galaxy_path: self.image_for_galaxy(galaxy)
             for galaxy_path, galaxy in self.path_galaxy_tuples
         }
 
     @property
-    def hyper_galaxy_image_path_dict(self) -> Dict[str, aa.Array2D]:
+    def adapt_galaxy_image_path_dict(self) -> Dict[str, aa.Array2D]:
         """
-        A dictionary associating 1D hyper galaxy images with their names.
+        A dictionary associating 1D galaxy images with their names.
         """
 
-        hyper_minimum_percent = conf.instance["general"]["hyper"][
-            "hyper_minimum_percent"
+        adapt_minimum_percent = conf.instance["general"]["adapt"][
+            "adapt_minimum_percent"
         ]
 
-        hyper_galaxy_image_path_dict = {}
+        adapt_galaxy_image_path_dict = {}
 
         for path, galaxy in self.path_galaxy_tuples:
-
             galaxy_image = self.image_galaxy_dict[path]
 
             if not np.all(galaxy_image == 0):
-                minimum_galaxy_value = hyper_minimum_percent * max(galaxy_image)
+                minimum_galaxy_value = adapt_minimum_percent * max(galaxy_image)
                 galaxy_image[galaxy_image < minimum_galaxy_value] = minimum_galaxy_value
 
-            hyper_galaxy_image_path_dict[path] = galaxy_image
+            adapt_galaxy_image_path_dict[path] = galaxy_image
 
-        return hyper_galaxy_image_path_dict
+        return adapt_galaxy_image_path_dict
 
     @property
-    def hyper_model_image(self) -> aa.Array2D:
+    def adapt_model_image(self) -> aa.Array2D:
         """
-        The hyper model image used by Analysis objects to adapt aspects of a model to the dataset being fitted.
+        The adapt image used by Analysis objects to adapt aspects of a model to the dataset being fitted.
 
-        The hyper model image is the sum of the hyper galaxy image of every individual galaxy.
+        The adapt image is the sum of the galaxy image of every individual galaxy.
         """
-        hyper_model_image = aa.Array2D(
+        adapt_model_image = aa.Array2D(
             values=np.zeros(self.mask.derive_mask.sub_1.pixels_in_mask),
             mask=self.mask.derive_mask.sub_1,
         )
 
         for path, galaxy in self.path_galaxy_tuples:
-            hyper_model_image += self.hyper_galaxy_image_path_dict[path]
+            adapt_model_image += self.adapt_galaxy_image_path_dict[path]
 
-        return hyper_model_image
+        return adapt_model_image
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/analysis/visualizer.py` & `autogalaxy-2023.7.7.1/autogalaxy/analysis/visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import os
 from os import path
-from typing import List, Optional, Union
+from typing import Dict, List, Union
 
 from autoconf import conf
 import autoarray as aa
 import autoarray.plot as aplt
 
 from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.galaxy.plot.galaxy_plotters import GalaxyPlotter
-from autogalaxy.galaxy.plot.hyper_galaxy_plotters import HyperPlotter
+from autogalaxy.galaxy.plot.adapt_plotters import AdaptPlotter
 from autogalaxy.plane.plane import Plane
 from autogalaxy.plane.plot.plane_plotters import PlanePlotter
 
 from autogalaxy.plot.include.two_d import Include2D
 from autogalaxy.plot.mat_plot.one_d import MatPlot1D
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
 
 
 def setting(section: Union[List[str], str], name: str):
     if isinstance(section, str):
         return conf.instance["visualize"]["plots"][section][name]
 
     for sect in reversed(section):
-
         try:
             return conf.instance["visualize"]["plots"][sect][name]
         except KeyError:
             continue
 
     return conf.instance["visualize"]["plots"][section[0]][name]
 
@@ -51,16 +50,14 @@
         Parameters
         ----------
         visualize_path
             The path on the hard-disk to the `image` folder of the non-linear searches results.
         """
         self.visualize_path = visualize_path
 
-        self.plot_fit_no_hyper = plot_setting("hyper", "fit_no_hyper")
-
         self.include_2d = Include2D()
 
         try:
             os.makedirs(visualize_path)
         except FileExistsError:
             pass
 
@@ -108,99 +105,94 @@
         """
         return MatPlot2D(
             output=aplt.Output(
                 path=path.join(self.visualize_path, subfolders), format=format
             )
         )
 
-    def visualize_imaging(self, imaging: aa.Imaging):
+    def visualize_imaging(self, dataset: aa.Imaging):
         """
         Visualizes an `Imaging` dataset object.
 
         Images are output to the `image` folder of the `visualize_path` in a subfolder called `imaging`. When used with
         a non-linear search the `visualize_path` points to the search's results folder.
         `.
         Visualization includes individual images of attributes of the dataset (e.g. the image, noise map, PSF) and a
         subplot of all these attributes on the same figure.
 
         The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
         [dataset] header.
 
         Parameters
         ----------
-        imaging
+        dataset
             The imaging dataset whose attributes are visualized.
         """
 
         def should_plot(name):
             return plot_setting(section=["dataset", "imaging"], name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="imaging")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="dataset")
 
-        imaging_plotter = aplt.ImagingPlotter(
-            imaging=imaging, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+        dataset_plotter = aplt.ImagingPlotter(
+            dataset=dataset, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
-        imaging_plotter.figures_2d(
-            image=should_plot("data"),
+        dataset_plotter.figures_2d(
+            data=should_plot("data"),
             noise_map=should_plot("noise_map"),
             psf=should_plot("psf"),
-            inverse_noise_map=should_plot("inverse_noise_map"),
             signal_to_noise_map=should_plot("signal_to_noise_map"),
-            absolute_signal_to_noise_map=should_plot("absolute_signal_to_noise_map"),
-            potential_chi_squared_map=should_plot("potential_chi_squared_map"),
         )
 
         if should_plot("subplot_dataset"):
+            dataset_plotter.subplot_dataset()
 
-            imaging_plotter.subplot_imaging()
-
-    def visualize_interferometer(self, interferometer: aa.Interferometer):
+    def visualize_interferometer(self, dataset: aa.Interferometer):
         """
         Visualizes an `Interferometer` dataset object.
 
         Images are output to the `image` folder of the `visualize_path` in a subfolder called `interferometer`. When
         used with a non-linear search the `visualize_path` points to the search's results folder.
 
         Visualization includes individual images of attributes of the dataset (e.g. the visibilities, noise map,
         uv-wavelengths) and a subplot of all these attributes on the same figure.
 
         The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
         [dataset] header.
 
         Parameters
         ----------
-        interferometer
+        dataset
             The interferometer dataset whose attributes are visualized.
         """
 
         def should_plot(name):
             return plot_setting(section=["dataset", "interferometer"], name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="interferometer")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="dataset")
 
-        interferometer_plotter = aplt.InterferometerPlotter(
-            interferometer=interferometer,
+        dataset_plotter = aplt.InterferometerPlotter(
+            dataset=dataset,
             include_2d=self.include_2d,
             mat_plot_2d=mat_plot_2d,
         )
 
         if should_plot("subplot_dataset"):
-            interferometer_plotter.subplot_interferometer()
+            dataset_plotter.subplot_dataset()
 
-        interferometer_plotter.figures_2d(
-            visibilities=should_plot("data"),
+        dataset_plotter.figures_2d(
+            data=should_plot("data"),
             u_wavelengths=should_plot("uv_wavelengths"),
             v_wavelengths=should_plot("uv_wavelengths"),
             amplitudes_vs_uv_distances=should_plot("amplitudes_vs_uv_distances"),
             phases_vs_uv_distances=should_plot("phases_vs_uv_distances"),
             dirty_image=should_plot("dirty_image"),
             dirty_noise_map=should_plot("dirty_noise_map"),
             dirty_signal_to_noise_map=should_plot("dirty_signal_to_noise_map"),
-            dirty_inverse_noise_map=should_plot("dirty_inverse_noise_map"),
         )
 
     def visualize_plane(
         self, plane: Plane, grid: aa.type.Grid2DLike, during_analysis: bool
     ):
         """
         Visualizes a `Plane` object.
@@ -225,71 +217,78 @@
         during_analysis
             Whether visualization is performed during a non-linear search or once it is completed.
         """
 
         def should_plot(name):
             return plot_setting(section="plane", name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="plane")
+        subfolders = "plane"
+
+        mat_plot_2d = self.mat_plot_2d_from(subfolders=subfolders)
 
         plane_plotter = PlanePlotter(
             plane=plane, grid=grid, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         if should_plot("subplot_plane"):
-
             plane_plotter.subplot()
 
         if should_plot("subplot_galaxy_images"):
-
             plane_plotter.subplot_galaxy_images()
 
         plane_plotter.figures_2d(
             image=should_plot("image"),
             convergence=should_plot("convergence"),
             potential=should_plot("potential"),
             deflections_y=should_plot("deflections"),
             deflections_x=should_plot("deflections"),
             magnification=should_plot("magnification"),
         )
 
-        if not during_analysis:
-
-            if should_plot("all_at_end_png"):
+        if not during_analysis and should_plot("all_at_end_png"):
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join(subfolders, "end"),
+            )
 
-                plane_plotter.figures_2d(
-                    image=True,
-                    convergence=True,
-                    potential=True,
-                    deflections_y=True,
-                    deflections_x=True,
-                    magnification=True,
-                )
+            plane_plotter = PlanePlotter(
+                plane=plane,
+                grid=grid,
+                mat_plot_2d=mat_plot_2d,
+                include_2d=self.include_2d,
+            )
 
-            if should_plot("all_at_end_fits"):
+            plane_plotter.figures_2d(
+                image=True,
+                convergence=True,
+                potential=True,
+                deflections_y=True,
+                deflections_x=True,
+                magnification=True,
+            )
 
-                fits_mat_plot_2d = self.mat_plot_2d_from(
-                    subfolders=path.join("plane", "fits"), format="fits"
-                )
+        if not during_analysis and should_plot("all_at_end_fits"):
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join(subfolders, "fits"), format="fits"
+            )
 
-                plane_plotter = PlanePlotter(
-                    plane=plane,
-                    grid=grid,
-                    mat_plot_2d=fits_mat_plot_2d,
-                    include_2d=self.include_2d,
-                )
+            plane_plotter = PlanePlotter(
+                plane=plane,
+                grid=grid,
+                mat_plot_2d=mat_plot_2d,
+                include_2d=self.include_2d,
+            )
 
-                plane_plotter.figures_2d(
-                    image=True,
-                    convergence=True,
-                    potential=True,
-                    deflections_y=True,
-                    deflections_x=True,
-                    magnification=True,
-                )
+            plane_plotter.figures_2d(
+                image=True,
+                convergence=True,
+                potential=True,
+                deflections_y=True,
+                deflections_x=True,
+                magnification=True,
+            )
 
     def visualize_galaxies(
         self, galaxies: [List[Galaxy]], grid: aa.type.Grid2DLike, during_analysis: bool
     ):
         """
         Visualizes a list of `Galaxy` objects.
 
@@ -316,15 +315,14 @@
 
         def should_plot(name):
             return plot_setting(section="galaxies", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders="galaxies")
 
         for galaxy in galaxies:
-
             galaxy_plotter = GalaxyPlotter(
                 galaxy=galaxy,
                 grid=grid,
                 mat_plot_1d=mat_plot_1d,
                 include_2d=self.include_2d,
             )
 
@@ -358,130 +356,147 @@
         during_analysis
             Whether visualization is performed during a non-linear search or once it is completed.
         """
 
         def should_plot(name):
             return plot_setting(section="inversion", name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="inversion")
+        subfolders = "inversion"
+
+        mat_plot_2d = self.mat_plot_2d_from(subfolders=subfolders)
 
         inversion_plotter = aplt.InversionPlotter(
             inversion=inversion, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         inversion_plotter.figures_2d(
             reconstructed_image=should_plot("reconstructed_image")
         )
 
         inversion_plotter.figures_2d_of_pixelization(
             pixelization_index=0,
             reconstructed_image=should_plot("reconstructed_image"),
             reconstruction=should_plot("reconstruction"),
             errors=should_plot("errors"),
-            residual_map=should_plot("residual_map"),
-            normalized_residual_map=should_plot("normalized_residual_map"),
-            chi_squared_map=should_plot("chi_squared_map"),
             regularization_weights=should_plot("regularization_weights"),
         )
 
         if should_plot("subplot_inversion"):
-
             mapper_list = inversion.cls_list_from(cls=aa.AbstractMapper)
 
             for mapper_index in range(len(mapper_list)):
                 inversion_plotter.subplot_of_mapper(mapper_index=mapper_index)
 
-        if not during_analysis:
+        if not during_analysis and should_plot("all_at_end_png"):
+            mat_plot_2d = self.mat_plot_2d_from(subfolders=path.join(subfolders, "end"))
 
-            if should_plot("all_at_end_png"):
+            inversion_plotter = aplt.InversionPlotter(
+                inversion=inversion, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+            )
 
-                inversion_plotter.figures_2d(reconstructed_image=True)
+            inversion_plotter.figures_2d(reconstructed_image=True)
 
-                inversion_plotter.figures_2d_of_pixelization(
-                    pixelization_index=0,
-                    reconstructed_image=True,
-                    reconstruction=True,
-                    errors=True,
-                    residual_map=True,
-                    normalized_residual_map=True,
-                    chi_squared_map=True,
-                    regularization_weights=True,
-                )
+            inversion_plotter.figures_2d_of_pixelization(
+                pixelization_index=0,
+                reconstructed_image=True,
+                reconstruction=True,
+                errors=True,
+                regularization_weights=True,
+            )
 
-    def visualize_hyper_images(
+        if not during_analysis and should_plot("all_at_end_fits"):
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join(subfolders, "fits"), format="fits"
+            )
+
+            inversion_plotter = aplt.InversionPlotter(
+                inversion=inversion, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+            )
+
+            inversion_plotter.figures_2d(reconstructed_image=True)
+
+            inversion_plotter.figures_2d_of_pixelization(
+                pixelization_index=0,
+                reconstructed_image=True,
+                reconstruction=True,
+                errors=True,
+                regularization_weights=True,
+                interpolate_to_uniform=True,
+            )
+
+    def visualize_adapt_images(
         self,
-        hyper_galaxy_image_path_dict: {str, aa.Array2D},
-        hyper_model_image: aa.Array2D,
+        adapt_galaxy_image_path_dict: Dict[str, aa.Array2D],
+        adapt_model_image: aa.Array2D,
     ):
         """
-        Visualizes the hyper-images and hyper dataset inferred by a model-fit.
+        Visualizes the adapt-images and adapt dataset inferred by a model-fit.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `hyper`. When
+        Images are output to the `image` folder of the `visualize_path` in a subfolder called `adapt`. When
         used with a non-linear search the `visualize_path` points to the search's results folder.
 
-        Visualization includes individual images of attributes of the hyper dataset (e.g. the hyper model image) and
-        a subplot of all hyper galaxy images on the same figure.
+        Visualization includes individual images of attributes of the adapt dataset (e.g. the adapt image) and
+        a subplot of all galaxy images on the same figure.
 
         The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
-        [hyper] header.
+        [adapt] header.
 
         Parameters
         ----------
-        hyper_galaxy_image_path_dict
-            A dictionary mapping the path to each galaxy (e.g. its name) to its corresponding hyper galaxy image.
-        hyper_model_image
-            The hyper model image which corresponds to the sum of hyper galaxy images.
+        adapt_galaxy_image_path_dict
+            A dictionary mapping the path to each galaxy (e.g. its name) to its corresponding galaxy image.
+        adapt_model_image
+            The adapt image which corresponds to the sum of galaxy images.
         """
 
         def should_plot(name):
-            return plot_setting(section="hyper", name=name)
+            return plot_setting(section="adapt", name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="hyper")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="adapt")
 
-        hyper_plotter = HyperPlotter(
+        adapt_plotter = AdaptPlotter(
             mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         if should_plot("model_image"):
-            hyper_plotter.figure_hyper_model_image(hyper_model_image=hyper_model_image)
+            adapt_plotter.figure_adapt_model_image(adapt_model_image=adapt_model_image)
 
         if should_plot("images_of_galaxies"):
-
-            hyper_plotter.subplot_hyper_images_of_galaxies(
-                hyper_galaxy_image_path_dict=hyper_galaxy_image_path_dict
+            adapt_plotter.subplot_adapt_images_of_galaxies(
+                adapt_galaxy_image_path_dict=adapt_galaxy_image_path_dict
             )
 
     def visualize_contribution_maps(self, plane: Plane):
         """
-        Visualizes the contribution maps that are used for hyper features which adapt a model to the dataset it is
+        Visualizes the contribution maps that are used for adapt features which adapt a model to the dataset it is
         fitting.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `hyper`. When
+        Images are output to the `image` folder of the `visualize_path` in a subfolder called `adapt`. When
         used with a non-linear search the `visualize_path` points to the search's results folder and this function
         visualizes the maximum log likelihood contribution maps inferred by the search so far.
 
-        Visualization includes individual images of attributes of the hyper dataset (e.g. the contribution map of
+        Visualization includes individual images of attributes of the adapt dataset (e.g. the contribution map of
         each galaxy) and a subplot of all contribution maps on the same figure.
 
         The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
-        [hyper] header.
+        [adapt] header.
 
         Parameters
         ----------
         plane
             The maximum log likelihood `Plane` of the non-linear search which is used to plot the contribution maps.
         """
 
         def should_plot(name):
-            return plot_setting(section="hyper", name=name)
+            return plot_setting(section="adapt", name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="hyper")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="adapt")
 
-        hyper_plotter = HyperPlotter(
+        adapt_plotter = AdaptPlotter(
             mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         if hasattr(plane, "contribution_map_list"):
             if should_plot("contribution_map_list"):
-                hyper_plotter.subplot_contribution_map_list(
+                adapt_plotter.subplot_contribution_map_list(
                     contribution_map_list_list=plane.contribution_map_list
                 )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/README.rst` & `autogalaxy-2023.7.7.1/autogalaxy/config/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 The ``config`` folder contains configuration files which customize default **PyAutoLens**.
 
 Folders
 -------
 
-- ``priors``: Configs defining default priors assumed on every lens model component and set of parameters.
+- ``priors``: Configs defining default priors assumed on every model component and set of parameters.
 - ``visualize``: Configs defining what images are output by a lens model fit.
 
 Files
 -----
 
 - ``general.yaml``: Customizes general **PyAutoLens** settings.
 - ``grids.yaml``: Customize default behaviour of grids when used for calculations.
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/grids.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/grids.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Isothermal: 1.0e-08
     IsothermalCore: 1.0e-08
     IsothermalCoreSph: 1.0e-08
     IsothermalSph: 1.0e-08
     MassSheet: 1.0e-08
     Moffat: 1.0e-08
     MoffatSph: 1.0e-08
-    MultipolePowerLawM4: 1.0e-08
+    PowerLawMultipole: 1.0e-08
     NFW: 1.0e-06
     NFWMCRDuffySph: 1.0e-06
     NFWMCRLudlow: 1.0e-06
     NFWMCRLudlowSph: 1.0e-06
     NFWMCRScatterLudlow: 1.0e-06
     NFWMCRScatterLudlowSph: 1.0e-06
     NFWSph: 1.0e-06
@@ -52,8 +52,10 @@
     SersicRadialGradientSph: 1.0e-06
     ShapeletCartesian: 1.0e-8
     ShapeletCartesianEll: 1.0e-8
     ShapeletPolar: 1.0e-8
     ShapeletPolarEll: 1.0e-8
     ShapeletExponential: 1.0e-8
     ShapeletExponentialEll: 1.0e-8
+    SMBH: 1.0e-8
+    SMBHBinary: 1.0e-8
     EllProfile: 1.0e-08
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/notation.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/notation.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 label:
   label:
     sigma: \sigma
     alpha: \alpha
+    angle_binary: \theta
     beta: \beta
     break_radius: \theta_{\rm B}
     centre_0: y
     centre_1: x
     coefficient: \lambda
     contribution_factor: \omega_{\rm 0}
     core_radius: C_{\rm r}
@@ -22,15 +23,18 @@
     gamma_1: \gamma
     gamma_2: \gamma
     inner_coefficient: \lambda_{\rm 1}
     inner_slope: t_{\rm 1}
     intensity: I_{\rm b}
     kappa: \kappa
     kappa_s: \kappa_{\rm s}
+    m: m
+    mass: M
     mass_at_200: M_{\rm 200}
+    mass_ratio: M_{\rm ratio}
     mass_to_light_gradient: \Gamma
     mass_to_light_ratio: \Psi
     noise_factor: \omega_{\rm 1}
     noise_power: \omega{\rm 2}
     noise_scale: \sigma_{\rm 1}
     normalization_scale: n
     outer_coefficient: \lambda_{\rm 2}
@@ -38,14 +42,15 @@
     pixels: N_{\rm pix}
     radius_break: R_{\rm b}
     redshift: z
     redshift_object: z_{\rm obj}
     redshift_source: z_{\rm src}
     scale_radius: R_{\rm s}
     scatter: \sigma
+    separation: s
     sersic_index: n
     shape_0: y_{\rm pix}
     shape_1: x_{\rm pix}
     signal_scale: V
     sky_scale: \sigma_{\rm 0}
     slope: \gamma
     truncation_radius: R_{\rm t}
@@ -53,24 +58,23 @@
     weight_power: W_{\rm p}
     zeroth_coefficient: \lambda_{\rm 0}
     zeroth_signal_scale: V
   superscript:
     ExternalShear: ext
     Mesh: mesh
     Point: point
+    SMBH: smbh
     Redshift: z
     Regularization: reg
-    HyperBackgroundNoise: hyper
-    HyperGalaxy: hyper
-    HyperImageSky: hyper
     InputDeflections: defl
 label_format:
   format:
     sigma: '{:.4f}'
     alpha: '{:.4f}'
+    angle_binary: '{:.4f}'
     angular_diameter_distance_to_earth: '{:.4f}'
     beta: '{:.4f}'
     centre_0: '{:.4f}'
     centre_1: '{:.4f}'
     coefficient: '{:.4f}'
     concentration: '{:.4f}'
     contribution_factor: '{:.4f}'
@@ -89,17 +93,19 @@
     inner_coefficient: '{:.4f}'
     inner_slope: '{:.4f}'
     intensity: '{:.4f}'
     kappa: '{:.4f}'
     kappa_s: '{:.4f}'
     kpc_per_arcsec: '{:.4f}'
     luminosity: '{:.4e}'
+    m: '{:.1f}'
     mass: '{:.4e}'
     mass_at_200: '{:.4e}'
     mass_at_truncation_radius: '{:.4e}'
+    mass_ratio: '{:.4f}'
     mass_to_light_gradient: '{:.4f}'
     mass_to_light_ratio: '{:.4f}'
     n_x: '{:.1d}'
     n_y: '{:.1d}'
     noise_factor: '{:.3f}'
     noise_power: '{:.3f}'
     noise_scale: '{:.3f}'
@@ -110,14 +116,15 @@
     radius: '{:.4f}'
     radius_break: '{:.4f}'
     redshift: '{:.4f}'
     redshift_object: '{:.4f}'
     redshift_source: '{:.4f}'
     rho: '{:.4f}'
     scale_radius: '{:.4f}'
+    separation: '{:.4f}'
     sersic_index: '{:.4f}'
     shape_0: '{:.4f}'
     shape_1: '{:.4f}'
     signal_scale: '{:.4f}'
     sky_scale: '{:.4f}'
     slope: '{:.4f}'
     truncation_radius: '{:.4f}'
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/README.rst` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/cosmology.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/cosmology.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/galaxy/hyper.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-HyperGalaxy:
-  contribution_factor:
-    type: Uniform
-    lower_limit: 0.0
-    upper_limit: 20.0
+MassSheet:
+  centre_0:
+    type: Gaussian
+    mean: 0.0
+    sigma: 0.1
+    lower_limit: -inf
+    upper_limit: inf
     width_modifier:
-      type: Relative
-      value: 0.5
+      type: Absolute
+      value: 0.05
     gaussian_limits:
-      lower: 0.0
+      lower: -inf
       upper: inf
-  noise_factor:
-    type: LogUniform
-    lower_limit: 0.0001
-    upper_limit: 1000.0
+  centre_1:
+    type: Gaussian
+    mean: 0.0
+    sigma: 0.1
+    lower_limit: -inf
+    upper_limit: inf
     width_modifier:
-      type: Relative
-      value: 0.5
+      type: Absolute
+      value: 0.05
     gaussian_limits:
-      lower: 0.0
+      lower: -inf
       upper: inf
-  noise_power:
+  kappa:
     type: Uniform
-    lower_limit: -10.0
-    upper_limit: 10.0
+    lower_limit: -1.0
+    upper_limit: 1.0
     width_modifier:
-      type: Relative
-      value: 0.5
+      type: Absolute
+      value: 0.05
     gaussian_limits:
       lower: -inf
       upper: inf
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/README.rst` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/chameleon.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/eff.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/exponential.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/exponential_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/gaussian.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/moffat.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/sersic.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear/sersic_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear_operated/gaussian.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/linear_operated/moffat.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/gaussian.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/moffat.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/operated/sersic.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/cartesian.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/cartesian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/exponential.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/shapelets/polar.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/polar.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/chameleon.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/eff.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/exponential.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/exponential_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/gaussian.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/moffat.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/sersic.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/light/standard/sersic_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/README.rst` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/gnfw.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/multipole/power_law_m4.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_multipole.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-MultipolePowerLawM4:
+PowerLawMultipole:
+  m:
+    type: Constant
+    value: 4
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.1
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/point_sources.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,85 @@
-MassSheet:
+Point:
   centre_0:
     type: Gaussian
     mean: 0.0
-    sigma: 0.1
+    sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
       type: Absolute
       value: 0.05
     gaussian_limits:
       lower: -inf
       upper: inf
   centre_1:
     type: Gaussian
     mean: 0.0
-    sigma: 0.1
+    sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
       type: Absolute
       value: 0.05
     gaussian_limits:
       lower: -inf
       upper: inf
-  kappa:
-    type: Uniform
-    lower_limit: -1.0
-    upper_limit: 1.0
+PointFlux:
+  centre_0:
+    type: Gaussian
+    mean: 0.0
+    sigma: 0.3
+    lower_limit: -inf
+    upper_limit: inf
+    width_modifier:
+      type: Absolute
+      value: 0.05
+    gaussian_limits:
+      lower: -inf
+      upper: inf
+  centre_1:
+    type: Gaussian
+    mean: 0.0
+    sigma: 0.3
+    lower_limit: -inf
+    upper_limit: inf
+    width_modifier:
+      type: Absolute
+      value: 0.05
+    gaussian_limits:
+      lower: -inf
+      upper: inf
+  flux:
+    type: LogUniform
+    lower_limit: 1.0e-06
+    upper_limit: 1000000.0
+    width_modifier:
+      type: Relative
+      value: 0.5
+    gaussian_limits:
+      lower: 0.0
+      upper: inf
+PointSourceChi:
+  centre_0:
+    type: Gaussian
+    mean: 0.0
+    sigma: 0.3
+    lower_limit: -inf
+    upper_limit: inf
+    width_modifier:
+      type: Absolute
+      value: 0.05
+    gaussian_limits:
+      lower: -inf
+      upper: inf
+  centre_1:
+    type: Gaussian
+    mean: 0.0
+    sigma: 0.3
+    lower_limit: -inf
+    upper_limit: inf
     width_modifier:
       type: Absolute
       value: 0.05
     gaussian_limits:
       lower: -inf
       upper: inf
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/chameleon.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/exponential.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/gaussian.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/sersic.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/sersic_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/isothermal.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/isothermal_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/point.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/point.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/power_law.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/power_law_broken.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_broken.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mass/total/power_law_core.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/delaunay.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/delaunay.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/voronoi.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/mesh/voronoi_nn.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi_nn.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/adaptive_brightness.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/visualize/README.rst` & `autogalaxy-2023.7.7.1/autogalaxy/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/config/visualize/mat_wrap_2d.yaml` & `autogalaxy-2023.7.7.1/autogalaxy/config/visualize/mat_wrap_2d.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/convert.py` & `autogalaxy-2023.7.7.1/autogalaxy/convert.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/cosmology/lensing.py` & `autogalaxy-2023.7.7.1/autogalaxy/cosmology/lensing.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         c = speed of light
         G = Newton's gravity constant
         D_s = angular_diameter_distance_of_source_redshift_to_earth
         D_ls = angular_diameter_distance_of_lens_redshift_to_source_redshift
         D_l = angular_diameter_distance_of_lens_redshift_to_earth
 
         This function returns the critical surface density in units of solar masses, which are convenient units for
-        converting the inferred masses of a lens model from angular units (e.g. dimensionless units inferred from
+        converting the inferred masses of a model from angular units (e.g. dimensionless units inferred from
         data in arcseconds) to solar masses.
 
         Parameters
         ----------
         redshift_0
             The redshift of the first strong lens galaxy (E.g. the lens galaxy) for which the critical surface
             density is calculated.
@@ -173,15 +173,15 @@
         c = speed of light
         G = Newton's gravity constant
         D_s = Angular diameter distance of source redshift to earth
         D_ls = Angular diameter distance of lens redshift to source redshift
         D_l = Angular diameter distance of lens redshift to earth
 
         This function returns the critical surface density in units of solar masses / kpc^2, which are convenient
-        units for converting the inferred masses of a lens model from angular units (e.g. dimensionless units inferred
+        units for converting the inferred masses of a model from angular units (e.g. dimensionless units inferred
         from data in arcseconds) to solar masses.
 
         Parameters
         ----------
         redshift_0
             The redshift of the first strong lens galaxy (E.g. the lens galaxy) for which the critical surface
             density is calculated.
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/cosmology/model.py` & `autogalaxy-2023.7.7.1/autogalaxy/cosmology/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from autogalaxy.cosmology.wrap import FlatLambdaCDM
 from autogalaxy.cosmology.wrap import FlatwCDM
 
 
 class Planck15Om0(FlatLambdaCDM):
     def __init__(self, Om0: float = 0.3075):
-
         planck15 = cosmo.Planck15
 
         super().__init__(
             H0=planck15.H0,
             Om0=Om0,
             Tcmb0=planck15.Tcmb0,
             Neff=planck15.Neff,
@@ -18,15 +17,14 @@
             Ob0=planck15.Ob0,
             name=planck15.name,
         )
 
 
 class Planck15FlatwCDM(FlatwCDM):
     def __init__(self, Om0: float = 0.3075, w0: float = -1.0):
-
         planck15 = cosmo.Planck15
 
         super().__init__(
             H0=planck15.H0,
             Om0=Om0,
             w0=w0,
             Tcmb0=planck15.Tcmb0,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/cosmology/wrap.py` & `autogalaxy-2023.7.7.1/autogalaxy/cosmology/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/exc.py` & `autogalaxy-2023.7.7.1/autogalaxy/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,28 +68,26 @@
     incorrectly.
     """
 
     pass
 
 
 def raise_linear_light_profile_in_unmasked():
-
     raise FitException(
         """
         You cannot compute the unmasked image from a fit which contains linear 
         light profiles or a pixelization, and therefore uses an inversion.
         
         This is because the inversion can only be performed within the masked
         region.
         """
     )
 
 
 def raise_linear_light_profile_in_plot(plotter_type: str, model_obj: str):
-
     raise ProfileException(
         f"""
         A linear light profile (inherits from `LightProfileLinear` class) has 
         been passed to the `{plotter_type}`.
 
         Linear light profiles cannot be plotted, because they do not have an
         intensity value.
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/fixtures.py` & `autogalaxy-2023.7.7.1/autogalaxy/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from autoarray.fixtures import *
 
 import autogalaxy as ag
 import autogalaxy.plot as aplt
 
 
 def make_masked_imaging_7x7():
-
     imaging_7x7 = make_imaging_7x7()
 
     masked_imaging_7x7 = imaging_7x7.apply_mask(mask=make_sub_mask_2d_7x7())
 
     return masked_imaging_7x7.apply_settings(settings=ag.SettingsImaging(sub_size=1))
 
 
 def make_masked_imaging_covariance_7x7():
-
     imaging_7x7 = make_imaging_covariance_7x7()
 
     masked_imaging_7x7 = imaging_7x7.apply_mask(mask=make_sub_mask_2d_7x7())
 
     return masked_imaging_7x7.apply_settings(settings=ag.SettingsImaging(sub_size=1))
 
 
@@ -114,18 +112,14 @@
 
 def make_gal_x1_lp_x1_mp():
     return ag.Galaxy(
         redshift=0.5, light_profile_0=make_lp_0(), mass_profile_0=make_mp_0()
     )
 
 
-def make_hyper_galaxy():
-    return ag.HyperGalaxy(noise_factor=1.0, noise_power=1.0, contribution_factor=1.0)
-
-
 # Plane #
 
 
 def make_plane_7x7():
     return ag.Plane(galaxies=[make_gal_x1_lp_x1_mp()])
 
 
@@ -150,78 +144,74 @@
     return ag.cosmo.Planck15()
 
 
 # QUANTITY DATASET AND FIT #
 
 
 def make_dataset_quantity_7x7_array_2d():
-
     return ag.DatasetQuantity(
         data=aa.Array2D.ones(shape_native=(7, 7), pixel_scales=1.0),
         noise_map=aa.Array2D.full(
             fill_value=2.0, shape_native=(7, 7), pixel_scales=1.0
         ),
     )
 
 
 def make_dataset_quantity_7x7_vector_yx_2d():
-
     return ag.DatasetQuantity(
         data=aa.VectorYX2D.ones(shape_native=(7, 7), pixel_scales=1.0),
         noise_map=aa.VectorYX2D.full(
             fill_value=2.0, shape_native=(7, 7), pixel_scales=1.0
         ),
     )
 
 
 def make_fit_quantity_7x7_array_2d():
-
     return ag.FitQuantity(
         dataset=make_dataset_quantity_7x7_array_2d(),
         light_mass_obj=make_plane_7x7(),
         func_str="convergence_2d_from",
     )
 
 
 def make_fit_quantity_7x7_vector_yx_2d():
-
     return ag.FitQuantity(
         dataset=make_dataset_quantity_7x7_vector_yx_2d(),
         light_mass_obj=make_plane_7x7(),
         func_str="deflections_yx_2d_from",
     )
 
 
-# HYPER galaxies #
+# galaxies #
 
 
-def make_hyper_model_image_7x7():
+def make_adapt_model_image_7x7():
     return ag.Array2D(
         np.full(fill_value=5.0, shape=make_mask_2d_7x7().pixels_in_mask),
         mask=make_mask_2d_7x7(),
     )
 
 
-def make_hyper_galaxy_image_0_7x7():
+def make_adapt_galaxy_image_0_7x7():
     return ag.Array2D(
         np.full(fill_value=2.0, shape=make_mask_2d_7x7().pixels_in_mask),
         mask=make_mask_2d_7x7(),
     )
 
 
-def make_hyper_galaxy_image_path_dict_7x7():
-    hyper_galaxy_image_path_dict = {
-        ("g0",): make_hyper_galaxy_image_0_7x7(),
-        ("g1",): make_hyper_galaxy_image_1_7x7(),
+def make_adapt_galaxy_image_path_dict_7x7():
+    adapt_galaxy_image_path_dict = {
+        ("g0",): make_adapt_galaxy_image_0_7x7(),
+        ("g1",): make_adapt_galaxy_image_1_7x7(),
     }
 
-    return hyper_galaxy_image_path_dict
+    return adapt_galaxy_image_path_dict
 
 
-def make_hyper_galaxy_image_1_7x7():
+def make_adapt_galaxy_image_1_7x7():
     return ag.Array2D(
         np.full(fill_value=3.0, shape=make_mask_2d_7x7().pixels_in_mask),
         mask=make_mask_2d_7x7(),
     )
 
 
 def make_fit_imaging_7x7():
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/galaxy/galaxy.py` & `autogalaxy-2023.7.7.1/autogalaxy/galaxy/galaxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,62 +3,58 @@
 import numpy as np
 
 import autoarray as aa
 import autofit as af
 
 from autoconf.dictable import Dictable
 from autogalaxy import exc
-from autogalaxy.galaxy.hyper import HyperGalaxy
 from autogalaxy.operate.deflections import OperateDeflections
 from autogalaxy.operate.image import OperateImageList
 from autogalaxy.profiles.geometry_profiles import GeometryProfile
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 
 
 class Galaxy(af.ModelObject, OperateImageList, OperateDeflections, Dictable):
     """
     @DynamicAttrs
     """
 
-    def __init__(
-        self, redshift: float, hyper_galaxy: Optional[HyperGalaxy] = None, **kwargs
-    ):
+    def __init__(self, redshift: float, **kwargs):
         """
-        Class representing a galaxy, which is composed of attributes used for fitting hyper_galaxies (e.g. light profiles, \
+        Class representing a galaxy, which is composed of attributes used for fitting galaxies (e.g. light profiles,
         mass profiles, pixelizations, etc.).
-        
+
         All *has_* methods retun `True` if galaxy has that attribute, `False` if not.
 
         Parameters
         ----------
         redshift
             The redshift of the galaxy.
         pixelization
             The pixelization of the galaxy used to reconstruct an observed image using an inversion.
-            
+
         Attributes
         ----------
-        hyper_model_image
+        adapt_model_image
             The best-fit model image to the observed image from a previous analysis
             search. This provides the total light attributed to each image pixel by the
             model.
-        hyper_galaxy_image
+        adapt_galaxy_image
             A model image of the galaxy (from light profiles or an inversion) from a
             previous analysis search.
         """
         super().__init__()
         self.redshift = redshift
 
-        self.hyper_model_image = None
-        self.hyper_galaxy_image = None
+        self.adapt_model_image = None
+        self.adapt_galaxy_image = None
 
         for name, val in kwargs.items():
-
             if isinstance(val, list):
                 raise exc.GalaxyException(
                     "One or more of the input light / mass profiles has been passed to the Galaxy object"
                     "as a list."
                     ""
                     "The Galaxy object cannot accept a list of light / mass profiles. "
                     ""
@@ -67,16 +63,14 @@
                     ""
                     "{bulge : al.lp.Sersic()}"
                     ""
                 )
 
             setattr(self, name, val)
 
-        self.hyper_galaxy = hyper_galaxy
-
     def __hash__(self):
         return int(self.id)
 
     def __repr__(self):
         string = "Redshift: {}".format(self.redshift)
 
         if self.has(cls=LightProfile):
@@ -88,17 +82,14 @@
             string += "\nMass Profiles:\n{}".format(
                 "\n".join(map(str, self.cls_list_from(cls=MassProfile)))
             )
 
         if self.has(cls=aa.Pixelization):
             string += "\nPixelization:\n{}".format(str(self.pixelization))
 
-        if self.hyper_galaxy:
-            string += "\nHyper Galaxy:\n{}".format(str(self.hyper_galaxy))
-
         return string
 
     def __eq__(self, other):
         return self.dict() == other.dict()
 
     @property
     def profile_dict(self) -> Dict:
@@ -164,15 +155,14 @@
             [
                 profile._radial_projected_shape_slim_from(grid=grid)
                 for key, profile in self.profile_dict.items()
             ]
         )
 
     def grid_radial_from(self, grid, centre, angle):
-
         if isinstance(grid, aa.Grid1D) or isinstance(grid, aa.Grid2DIrregular):
             return grid
 
         radial_projected_shape_slim = self._radial_projected_shape_slim_from(grid=grid)
 
         return grid.grid_2d_radial_projected_from(
             centre=centre, angle=angle + 90, shape_slim=radial_projected_shape_slim
@@ -263,21 +253,19 @@
 
         Parameters
         ----------
         grid
             The 1D (x,) coordinates where values of the image are evaluated.
         """
         if self.has(cls=LightProfile):
-
             image_1d_list = []
 
             for light_profile in self.cls_list_from(
                 cls=LightProfile, cls_filtered=LightProfileLinear
             ):
-
                 grid_radial = self.grid_radial_from(
                     grid=grid, centre=light_profile.centre, angle=light_profile.angle
                 )
 
                 image_1d_list.append(light_profile.image_1d_from(grid=grid_radial))
 
             return sum(image_1d_list)
@@ -354,19 +342,17 @@
 
         Parameters
         ----------
         grid
             The 1D (x,) coordinates where values of the convergence are evaluated.
         """
         if self.has(cls=MassProfile):
-
             convergence_1d_list = []
 
             for mass_profile in self.cls_list_from(cls=MassProfile):
-
                 grid_radial = self.grid_radial_from(
                     grid=grid, centre=mass_profile.centre, angle=mass_profile.angle
                 )
 
                 convergence_1d_list.append(
                     mass_profile.convergence_1d_from(grid=grid_radial)
                 )
@@ -416,58 +402,36 @@
 
         Parameters
         ----------
         grid
             The 1D (x,) coordinates where values of the potential are evaluated.
         """
         if self.has(cls=MassProfile):
-
             potential_1d_list = []
 
             for mass_profile in self.cls_list_from(cls=MassProfile):
-
                 grid_radial = self.grid_radial_from(
                     grid=grid, centre=mass_profile.centre, angle=mass_profile.angle
                 )
 
                 potential_1d_list.append(
                     mass_profile.potential_1d_from(grid=grid_radial)
                 )
 
             return sum(potential_1d_list)
 
         return np.zeros((grid.shape[0],))
 
     @property
-    def contribution_map(self) -> aa.Array2D:
-        """
-        Returns the contribution map of a galaxy, which represents the fraction of
-        flux in each pixel that the galaxy is attributed to contain, hyper to the
-        *contribution_factor* hyper_galaxies-parameter.
-
-        This is computed by dividing that galaxy's flux by the total flux in that \
-        pixel and then scaling by the maximum flux such that the contribution map \
-        ranges between 0 and 1.
-
-        Parameters
-        ----------
-
-        """
-        return self.hyper_galaxy.contribution_map_from(
-            hyper_model_image=self.hyper_model_image,
-            hyper_galaxy_image=self.hyper_galaxy_image,
-        )
-
-    @property
     def half_light_radius(self):
         return None
 
     def extract_attribute(self, cls, attr_name):
         """
-        Returns an attribute of a class and its children profiles in the the galaxy as a `ValueIrregular`
+        Returns an attribute of a class and its children profiles in the galaxy as a `ValueIrregular`
         or `Grid2DIrregular` object.
 
         For example, if a galaxy has two light profiles and we want the `LightProfile` axis-ratios, the following:
 
         `galaxy.extract_attribute(cls=LightProfile, name="axis_ratio"`
 
         would return:
@@ -482,15 +446,14 @@
 
         GridIrregular2D(grid=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1), (centre_y_2, centre_x_2)])
 
         This is used for visualization, for example plotting the centres of all light profiles colored by their profile.
         """
 
         def extract(value, name):
-
             try:
                 return getattr(value, name)
             except (AttributeError, IndexError):
                 return None
 
         attributes = [
             extract(value, attr_name)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/galaxy/mock/mock_galaxy.py` & `autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/mock_galaxy.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/galaxy/plot/galaxy_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/galaxy_plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 import math
-from typing import List, Optional
+from typing import TYPE_CHECKING, List, Optional
 
 import autoarray as aa
 import autoarray.plot as aplt
 
 from autogalaxy.plot.abstract_plotters import Plotter
 from autogalaxy.plot.mat_plot.one_d import MatPlot1D
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
@@ -12,16 +13,18 @@
 from autogalaxy.plot.include.one_d import Include1D
 from autogalaxy.plot.include.two_d import Include2D
 from autogalaxy.plot.mass_plotter import MassPlotter
 
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePlotter
-from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePDFPlotter
+
+if TYPE_CHECKING:
+    from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePlotter
+    from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePDFPlotter
 from autogalaxy.profiles.plot.mass_profile_plotters import MassProfilePlotter
 from autogalaxy.profiles.plot.mass_profile_plotters import MassProfilePDFPlotter
 
 from autogalaxy import exc
 from autogalaxy.util import error_util
 
 
@@ -72,15 +75,14 @@
 
         from autogalaxy.profiles.light.linear import (
             LightProfileLinear,
         )
 
         if galaxy is not None:
             if galaxy.has(cls=LightProfileLinear):
-
                 raise exc.raise_linear_light_profile_in_plot(
                     plotter_type=self.__class__.__name__, model_obj="Plane"
                 )
 
         super().__init__(
             mat_plot_2d=mat_plot_2d,
             include_2d=include_2d,
@@ -127,16 +129,17 @@
 
         Returns
         -------
         LightProfilePlotter
             An object that plots the light profiles, often used for plotting attributes of the galaxy.
         """
 
-        if not one_d_only:
+        from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePlotter
 
+        if not one_d_only:
             return LightProfilePlotter(
                 light_profile=light_profile,
                 grid=self.grid,
                 mat_plot_2d=self.mat_plot_2d,
                 visuals_2d=self.get_2d.via_light_obj_from(
                     light_obj=light_profile, grid=self.grid
                 ),
@@ -169,15 +172,14 @@
         Returns
         -------
         MassProfilePlotter
             An object that plots the mass profiles, often used for plotting attributes of the galaxy.
         """
 
         if not one_d_only:
-
             return MassProfilePlotter(
                 mass_profile=mass_profile,
                 grid=self.grid,
                 mat_plot_2d=self.mat_plot_2d,
                 visuals_2d=self.get_2d.via_mass_obj_from(
                     mass_obj=mass_profile, grid=self.grid
                 ),
@@ -197,34 +199,30 @@
                 mass_obj=mass_profile, grid=self.grid
             ),
             include_1d=self.include_1d,
         )
 
     @property
     def decomposed_light_profile_plotter_list(self):
-
         plotter_list = []
 
         for i, light_profile in enumerate(self.galaxy.cls_list_from(cls=LightProfile)):
-
             light_profile_plotter = self.light_profile_plotter_from(
                 light_profile=light_profile, one_d_only=True
             )
 
             plotter_list.append(light_profile_plotter)
 
         return [self] + plotter_list
 
     @property
     def decomposed_mass_profile_plotter_list(self):
-
         plotter_list = []
 
         for i, mass_profile in enumerate(self.galaxy.cls_list_from(cls=MassProfile)):
-
             mass_profile_plotter = self.mass_profile_plotter_from(
                 mass_profile=mass_profile, one_d_only=True
             )
 
             plotter_list.append(mass_profile_plotter)
 
         return [self] + plotter_list
@@ -257,15 +255,14 @@
         """
         if self.mat_plot_1d.yx_plot.plot_axis_type is None:
             plot_axis_type_override = "semilogy"
         else:
             plot_axis_type_override = None
 
         if image:
-
             image_1d = self.galaxy.image_1d_from(grid=self.grid)
 
             self.mat_plot_1d.plot_yx(
                 y=image_1d,
                 x=image_1d.grid_radial,
                 visuals_1d=self.get_visuals_1d_light(),
                 auto_labels=aplt.AutoLabels(
@@ -275,15 +272,14 @@
                     legend=self.galaxy.__class__.__name__,
                     filename="image_1d",
                 ),
                 plot_axis_type_override=plot_axis_type_override,
             )
 
         if convergence:
-
             convergence_1d = self.galaxy.convergence_1d_from(grid=self.grid)
 
             self.mat_plot_1d.plot_yx(
                 y=convergence_1d,
                 x=convergence_1d.grid_radial,
                 visuals_1d=self.get_visuals_1d_mass(),
                 auto_labels=aplt.AutoLabels(
@@ -293,15 +289,14 @@
                     legend=self.galaxy.__class__.__name__,
                     filename="convergence_1d",
                 ),
                 plot_axis_type_override=plot_axis_type_override,
             )
 
         if potential:
-
             potential_1d = self.galaxy.potential_1d_from(grid=self.grid)
 
             self.mat_plot_1d.plot_yx(
                 y=potential_1d,
                 x=potential_1d.grid_radial,
                 visuals_1d=self.get_visuals_1d_mass(),
                 auto_labels=aplt.AutoLabels(
@@ -347,45 +342,41 @@
         potential
             Whether to make a 1D plot (via `imshow`) of the potential.
         legend_labels
             Manually overrides the labels of the plot's legend.
         """
 
         if self.galaxy.has(cls=LightProfile):
-
             multi_plotter = aplt.MultiYX1DPlotter(
                 plotter_list=self.decomposed_light_profile_plotter_list,
                 legend_labels=legend_labels,
             )
             multi_plotter.plotter_list[0].mat_plot_1d.output = self.mat_plot_1d.output
 
             if image:
-
                 change_filename = False
 
                 if multi_plotter.plotter_list[0].mat_plot_1d.output.filename is None:
                     multi_plotter.plotter_list[0].set_filename(
                         filename="image_1d_decomposed"
                     )
                     change_filename = True
 
                 multi_plotter.figure_1d(func_name="figures_1d", figure_name="image")
 
                 if change_filename:
                     multi_plotter.plotter_list[0].set_filename(filename=None)
 
         if self.galaxy.has(cls=MassProfile):
-
             multi_plotter = aplt.MultiYX1DPlotter(
                 plotter_list=self.decomposed_mass_profile_plotter_list,
                 legend_labels=legend_labels,
             )
 
             if convergence:
-
                 change_filename = False
 
                 if multi_plotter.plotter_list[0].mat_plot_1d.output.filename is None:
                     multi_plotter.plotter_list[0].set_filename(
                         filename="convergence_1d_decomposed"
                     )
                     change_filename = True
@@ -394,15 +385,14 @@
                     func_name="figures_1d", figure_name="convergence"
                 )
 
                 if change_filename:
                     multi_plotter.plotter_list[0].set_filename(filename=None)
 
             if potential:
-
                 change_filename = False
 
                 if multi_plotter.plotter_list[0].mat_plot_1d.output.filename is None:
                     multi_plotter.plotter_list[0].set_filename(
                         filename="potential_1d_decomposed"
                     )
                     change_filename = True
@@ -416,15 +406,14 @@
         self,
         image: bool = False,
         convergence: bool = False,
         potential: bool = False,
         deflections_y: bool = False,
         deflections_x: bool = False,
         magnification: bool = False,
-        contribution_map: bool = False,
         title_suffix: str = "",
         filename_suffix: str = "",
     ):
         """
         Plots the individual attributes of the plotter's `Galaxy` object in 2D, which are computed via the plotter's 2D
         grid object.
 
@@ -441,19 +430,16 @@
             Whether to make a 2D plot (via `imshow`) of the potential.
         deflections_y
             Whether to make a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
             Whether to make a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
             Whether to make a 2D plot (via `imshow`) of the magnification.
-        contribution_map
-            Whether to make a 2D plot (via `imshow`) of the contribution map.
         """
         if image:
-
             self.mat_plot_2d.plot_array(
                 array=self.galaxy.image_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Image{title_suffix}", filename=f"image_2d{filename_suffix}"
                 ),
             )
@@ -464,25 +450,14 @@
             deflections_y=deflections_y,
             deflections_x=deflections_x,
             magnification=magnification,
             title_suffix=title_suffix,
             filename_suffix=filename_suffix,
         )
 
-        if contribution_map:
-
-            self.mat_plot_2d.plot_array(
-                array=self.galaxy.contribution_map,
-                visuals_2d=self.get_visuals_2d(),
-                auto_labels=aplt.AutoLabels(
-                    title=f"Contribution Map{title_suffix}",
-                    filename=f"contribution_map_2d{filename_suffix}",
-                ),
-            )
-
     def subplot_of_light_profiles(self, image: bool = False):
         """
         Output a subplot of attributes of every individual light profile in 1D of the `Galaxy` object.
 
         For example, a 1D plot showing how the image (e.g. luminosity) of each component varies radially outwards.
 
         If the plotter has a 1D grid object this is used to evaluate each quantity. If it has a 2D grid, a 1D grid is
@@ -651,14 +626,19 @@
 
         Returns
         -------
         LightProfilePDFPlotter
             An object that plots the average value and errors of a list of light profiles, often used for plotting
             attributes of the galaxy.
         """
+
+        from autogalaxy.profiles.plot.light_profile_plotters import (
+            LightProfilePDFPlotter,
+        )
+
         light_profile_pdf_list = [
             galaxy.cls_list_from(cls=LightProfile)[index]
             for galaxy in self.galaxy_pdf_list
         ]
 
         return LightProfilePDFPlotter(
             light_profile_pdf_list=light_profile_pdf_list,
@@ -751,15 +731,14 @@
         """
         if self.mat_plot_1d.yx_plot.plot_axis_type is None:
             plot_axis_type_override = "semilogy"
         else:
             plot_axis_type_override = None
 
         if image:
-
             image_1d_list = [
                 galaxy.image_1d_from(grid=self.grid) for galaxy in self.galaxy_pdf_list
             ]
 
             min_index = min([image_1d.shape[0] for image_1d in image_1d_list])
             image_1d_list = [image_1d[0:min_index] for image_1d in image_1d_list]
 
@@ -794,15 +773,14 @@
                     legend=self.galaxy_pdf_list[0].__class__.__name__,
                     filename="image_1d",
                 ),
                 plot_axis_type_override=plot_axis_type_override,
             )
 
         if convergence:
-
             convergence_1d_list = [
                 galaxy.convergence_1d_from(grid=self.grid)
                 for galaxy in self.galaxy_pdf_list
             ]
 
             min_index = min(
                 [convergence_1d.shape[0] for convergence_1d in convergence_1d_list]
@@ -844,15 +822,14 @@
                     legend=self.galaxy_pdf_list[0].__class__.__name__,
                     filename="convergence_1d",
                 ),
                 plot_axis_type_override=plot_axis_type_override,
             )
 
         if potential:
-
             potential_1d_list = [
                 galaxy.potential_1d_from(grid=self.grid)
                 for galaxy in self.galaxy_pdf_list
             ]
 
             min_index = min(
                 [potential_1d.shape[0] for potential_1d in potential_1d_list]
@@ -934,15 +911,14 @@
             Whether to make a 1D plot (via `imshow`) of the convergence.
         potential
             Whether to make a 1D plot (via `imshow`) of the potential.
         legend_labels
             Manually overrides the labels of the plot's legend.
         """
         if image:
-
             multi_plotter = aplt.MultiYX1DPlotter(
                 plotter_list=[self] + self.light_profile_pdf_plotter_list,
                 legend_labels=legend_labels,
             )
 
             change_filename = False
 
@@ -955,15 +931,14 @@
 
             multi_plotter.figure_1d(func_name="figures_1d", figure_name="image")
 
             if change_filename:
                 multi_plotter.plotter_list[0].set_filename(filename=None)
 
         if convergence:
-
             multi_plotter = aplt.MultiYX1DPlotter(
                 plotter_list=[self] + self.mass_profile_pdf_plotter_list,
                 legend_labels=legend_labels,
             )
 
             change_filename = False
 
@@ -976,15 +951,14 @@
 
             multi_plotter.figure_1d(func_name="figures_1d", figure_name="convergence")
 
             if change_filename:
                 multi_plotter.plotter_list[0].set_filename(filename=None)
 
         if potential:
-
             multi_plotter = aplt.MultiYX1DPlotter(
                 plotter_list=[self] + self.mass_profile_pdf_plotter_list,
                 legend_labels=legend_labels,
             )
 
             change_filename = False
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/galaxy/plot/hyper_galaxy_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/adapt_plotters.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,114 +6,96 @@
 from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.plot.abstract_plotters import Plotter
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
 from autogalaxy.plot.visuals.two_d import Visuals2D
 from autogalaxy.plot.include.two_d import Include2D
 
 
-class HyperPlotter(Plotter):
+class AdaptPlotter(Plotter):
     def __init__(
         self,
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
     ):
         super().__init__(
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
     def get_visuals_2d(self) -> Visuals2D:
         return self.visuals_2d
 
-    def figure_hyper_model_image(self, hyper_model_image: aa.Array2D):
+    def figure_adapt_model_image(self, adapt_model_image: aa.Array2D):
         """
-        Plot the hyper model image of a hyper galaxy.
+        Plot the adapt image of a galaxy.
 
         Parameters
         ----------
-        hyper_model_image
-            The hyper model image that is plotted.
+        adapt_model_image
+            The adapt image that is plotted.
         """
 
         self.mat_plot_2d.plot_array(
-            array=hyper_model_image,
+            array=adapt_model_image,
             visuals_2d=self.get_visuals_2d(),
             auto_labels=aplt.AutoLabels(
-                title="Hyper Model Image", filename="hyper_model_image"
+                title="adapt image", filename="adapt_model_image"
             ),
         )
 
-    def figure_hyper_galaxy_image(self, galaxy_image: aa.Array2D):
+    def figure_adapt_galaxy_image(self, galaxy_image: aa.Array2D):
         """
-        Plot the hyper galaxy image of a hyper galaxy.
+        Plot the galaxy image of a galaxy.
 
         Parameters
         ----------
         galaxy_image
-            The hyper galaxy image that is plotted.
+            The galaxy image that is plotted.
         """
         self.mat_plot_2d.plot_array(
             array=galaxy_image,
             visuals_2d=self.get_visuals_2d(),
             auto_labels=aplt.AutoLabels(
-                title="Hyper Galaxy Image", filename="hyper_galaxy_image"
+                title="galaxy Image", filename="adapt_galaxy_image"
             ),
         )
 
-    def figure_contribution_map(self, contribution_map: aa.Array2D):
-        """
-        Plot the contribution map of a hyper galaxy.
-
-        Parameters
-        ----------
-        contribution_map
-            The contribution map that is plotted.
-        """
-        self.mat_plot_2d.plot_array(
-            array=contribution_map,
-            visuals_2d=self.get_visuals_2d(),
-            auto_labels=aplt.AutoLabels(
-                title="Contribution Map", filename="contribution_map_2d"
-            ),
-        )
-
-    def subplot_hyper_images_of_galaxies(
-        self, hyper_galaxy_image_path_dict: Dict[Galaxy, aa.Array2D]
+    def subplot_adapt_images_of_galaxies(
+        self, adapt_galaxy_image_path_dict: Dict[Galaxy, aa.Array2D]
     ):
         """
-        Plots a subplot of the hyper galaxy image of all hyper galaxies.
+        Plots a subplot of the galaxy image of all galaxies.
 
-        This uses the `hyper_galaxy_image_path_dict` which is a dictionary mapping each galaxy to its corresponding
-        to hyper galaxy image.
+        This uses the `adapt_galaxy_image_path_dict` which is a dictionary mapping each galaxy to its corresponding
+        to galaxy image.
 
         Parameters
         ----------
-        hyper_galaxy_image_path_dict
-            A dictionary mapping each galaxy to its corresponding to hyper galaxy image.
+        adapt_galaxy_image_path_dict
+            A dictionary mapping each galaxy to its corresponding to galaxy image.
         """
-        if hyper_galaxy_image_path_dict is None:
+        if adapt_galaxy_image_path_dict is None:
             return
 
-        self.open_subplot_figure(number_subplots=len(hyper_galaxy_image_path_dict))
-
-        for path, galaxy_image in hyper_galaxy_image_path_dict.items():
+        self.open_subplot_figure(number_subplots=len(adapt_galaxy_image_path_dict))
 
-            self.figure_hyper_galaxy_image(galaxy_image=galaxy_image)
+        for path, galaxy_image in adapt_galaxy_image_path_dict.items():
+            self.figure_adapt_galaxy_image(galaxy_image=galaxy_image)
 
         self.mat_plot_2d.output.subplot_to_figure(
-            auto_filename="subplot_hyper_images_of_galaxies"
+            auto_filename="subplot_adapt_images_of_galaxies"
         )
 
         self.close_subplot_figure()
 
     def subplot_contribution_map_list(
         self, contribution_map_list_list: List[aa.Array2D]
     ):
         """
-        Plots a subplot of the contribution maps of all hyper galaxies.
+        Plots a subplot of the contribution maps of all galaxies.
 
         This uses the `contribution_map_list` which is a list of each galaxy's corresponding contribution map.
 
         Parameters
         ----------
         contribution_map_list_list
             A list of each galaxy's corresponding contribution map.
@@ -128,15 +110,31 @@
 
         if number_subplots == 0:
             return
 
         self.open_subplot_figure(number_subplots=number_subplots)
 
         for contribution_map_array in contribution_maps:
-
             self.figure_contribution_map(contribution_map=contribution_map_array)
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename="subplot_contribution_map_list"
         )
 
         self.close_subplot_figure()
+
+    def figure_contribution_map(self, contribution_map: aa.Array2D):
+        """
+        Plot the contribution map of a galaxy.
+
+        Parameters
+        ----------
+        contribution_map
+            The contribution map that is plotted.
+        """
+        self.mat_plot_2d.plot_array(
+            array=contribution_map,
+            visuals_2d=self.get_visuals_2d(),
+            auto_labels=aplt.AutoLabels(
+                title="Contribution Map", filename="contribution_map_2d"
+            ),
+        )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/galaxy/redshift.py` & `autogalaxy-2023.7.7.1/autogalaxy/galaxy/redshift.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/galaxy/stellar_dark_decomp.py` & `autogalaxy-2023.7.7.1/autogalaxy/galaxy/stellar_dark_decomp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from autogalaxy import exc
 from autogalaxy.profiles.mass.dark.abstract import DarkProfile
 from autogalaxy.profiles.mass.stellar.abstract import StellarProfile
 
 
 class StellarDarkDecomp:
     def __init__(self, galaxy):
-
         self.galaxy = galaxy
 
     def stellar_mass_angular_within_circle_from(self, radius: float):
         if self.galaxy.has(cls=StellarProfile):
             return sum(
                 [
                     profile.mass_angular_within_circle_from(radius=radius)
@@ -35,12 +34,11 @@
                 "You cannot perform a dark mass-based calculation on a galaxy which does not have a dark mass-profile"
             )
 
     def stellar_fraction_at_radius_from(self, radius):
         return 1.0 - self.dark_fraction_at_radius_from(radius=radius)
 
     def dark_fraction_at_radius_from(self, radius):
-
         stellar_mass = self.stellar_mass_angular_within_circle_from(radius=radius)
         dark_mass = self.dark_mass_angular_within_circle_from(radius=radius)
 
         return dark_mass / (stellar_mass + dark_mass)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/gui/clicker.py` & `autogalaxy-2023.7.7.1/autogalaxy/gui/clicker.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 import autoarray as aa
 
 from autogalaxy import exc
 
 
 class Clicker:
     def __init__(self, image, pixel_scales, search_box_size):
-
         self.image = image
 
         pixel_scales = aa.util.geometry.convert_pixel_scales_2d(
             pixel_scales=pixel_scales
         )
 
         self.pixel_scales = pixel_scales
         self.search_box_size = search_box_size
 
         self.click_list = []
 
     def onclick(self, event):
-
         if event.dblclick:
-
             y_arcsec = (
                 np.rint(event.ydata / self.pixel_scales[0]) * self.pixel_scales[0]
             )
             x_arcsec = (
                 np.rint(event.xdata / self.pixel_scales[1]) * self.pixel_scales[1]
             )
 
@@ -38,15 +35,14 @@
 
             for y in range(
                 y_pixels - self.search_box_size, y_pixels + self.search_box_size
             ):
                 for x in range(
                     x_pixels - self.search_box_size, x_pixels + self.search_box_size
                 ):
-
                     flux_new = self.image.native[y, x]
 
                     if flux_new > flux:
                         flux = flux_new
                         y_pixels_max = y
                         x_pixels_max = x
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/gui/scribbler.py` & `autogalaxy-2023.7.7.1/autogalaxy/gui/scribbler.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/imaging/fit_imaging.py` & `autogalaxy-2023.7.7.1/autogalaxy/plane/plane.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,428 +1,399 @@
+import json
 import numpy as np
-from typing import Dict, List, Optional
-
-from autoconf import conf
-from autoconf import cached_property
+from typing import Dict, List, Optional, Tuple, Type
 
 import autoarray as aa
 
-from autogalaxy.abstract_fit import AbstractFitInversion
-from autogalaxy.analysis.preloads import Preloads
+from autoconf.dictable import Dictable
+
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.hyper.hyper_data import HyperImageSky
-from autogalaxy.hyper.hyper_data import HyperBackgroundNoise
-from autogalaxy.plane.plane import Plane
-from autogalaxy.plane.to_inversion import PlaneToInversion
+from autogalaxy.profiles.light.basis import Basis
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
-from autogalaxy.profiles.light.operated.abstract import LightProfileOperated
+from autogalaxy.profiles.light.snr import LightProfileSNR
+from autogalaxy.operate.image import OperateImageGalaxies
+from autogalaxy.operate.deflections import OperateDeflections
+
+from autogalaxy import exc
+from autogalaxy.plane import plane_util
 
 
-class FitImaging(aa.FitImaging, AbstractFitInversion):
+class Plane(OperateImageGalaxies, OperateDeflections, Dictable):
     def __init__(
         self,
-        dataset: aa.Imaging,
-        plane: Plane,
-        hyper_image_sky: Optional[HyperImageSky] = None,
-        hyper_background_noise: Optional[HyperBackgroundNoise] = None,
-        use_hyper_scaling: bool = True,
-        settings_pixelization: aa.SettingsPixelization = aa.SettingsPixelization(),
-        settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
-        preloads: aa.Preloads = Preloads(),
+        galaxies,
+        redshift: Optional[float] = None,
         profiling_dict: Optional[Dict] = None,
     ):
         """
-        Fits an imaging dataset using a `Plane` object.
-
-        The fit performs the following steps:
-
-        1) Compute the sum of all images of galaxy light profiles in the `Plane`.
-
-        2) Blur this with the imaging PSF to created the `blurred_image`.
-
-        3) Subtract this image from the `data` to create the `profile_subtracted_image`.
-
-        4) If the `Plane` has any linear algebra objects (e.g. linear light profiles, a pixelization / regulariation)
-           fit the `profile_subtracted_image` with these objects via an inversion.
-
-        5) Compute the `model_data` as the sum of the `blurred_image` and `reconstructed_data` of the inversion (if
-           an inversion is not performed the `model_data` is only the `blurred_image`.
-
-        6) Subtract the `model_data` from the data and compute the residuals, chi-squared and likelihood via the
-           noise-map (if an inversion is performed the `log_evidence`, including additional terms describing the linear
-           algebra solution, is computed).
-
-        When performing a `model-fit`via an `AnalysisImaging` object the `figure_of_merit` of this `FitImaging` object
-        is called and returned in the `log_likelihood_function`.
+        A plane of galaxies where all galaxies are at the same redshift.
 
         Parameters
         ----------
-        dataset
-            The imaging dataset which is fitted by the galaxies in the plane.
-        plane
-            The plane of galaxies whose light profile images are used to fit the imaging data.
-        hyper_image_sky
-            If included, accounts for the background sky in the fit.
-        hyper_background_noise
-            If included, adds a noise-scaling term to the background to account for an inaacurate background sky model.
-        use_hyper_scaling
-            If set to False, the hyper scaling functions (e.g. the `hyper_image_sky` / `hyper_background_noise`) are
-            omitted irrespective of their inputs.
-        settings_pixelization
-            Settings controlling how a pixelization is fitted for example if a border is used when creating the
-            pixelization.
-        settings_inversion
-            Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
-        preloads
-            Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
-            the fit.
-        profiling_dict
-            A dictionary which if passed to the fit records how long fucntion calls which have the `profile_func`
-            decorator take to run.
-        """
-
-        self.plane = plane
-        self.preloads = preloads
-
-        super().__init__(
-            dataset=dataset,
-            profiling_dict=profiling_dict,
-        )
-        AbstractFitInversion.__init__(
-            self=self, model_obj=plane, settings_inversion=settings_inversion
-        )
+        redshift or None
+            The redshift of the plane.
+        galaxies : [Galaxy]
+            The list of galaxies in this plane.
+        """
 
-        self.hyper_image_sky = hyper_image_sky
-        self.hyper_background_noise = hyper_background_noise
+        if redshift is None:
+            if not galaxies:
+                raise exc.PlaneException(
+                    "No redshift and no galaxies were input to a Plane. A redshift for the Plane therefore cannot be"
+                    "determined"
+                )
+            elif not all(
+                [galaxies[0].redshift == galaxy.redshift for galaxy in galaxies]
+            ):
+                redshift = np.mean([galaxy.redshift for galaxy in galaxies])
+            else:
+                redshift = galaxies[0].redshift
 
-        self.use_hyper_scaling = use_hyper_scaling
+        self.redshift = redshift
+        self.galaxies = galaxies
 
-        self.settings_pixelization = settings_pixelization
-        self.settings_inversion = settings_inversion
+        self.profiling_dict = profiling_dict
 
-    @property
-    def galaxies(self) -> List[Galaxy]:
-        return self.plane.galaxies
+    def dict(self) -> Dict:
+        plane_dict = super().dict()
+        plane_dict["galaxies"] = [galaxy.dict() for galaxy in self.galaxies]
+        return plane_dict
 
-    @property
-    def grid(self) -> aa.type.Grid2DLike:
-        return self.imaging.grid
+    def output_to_json(self, file_path: str):
+        with open(file_path, "w+") as f:
+            json.dump(self.dict(), f, indent=4)
 
     @property
-    def data(self) -> aa.Array2D:
-        """
-        Returns the imaging data, which may have a hyper scaling performed which rescales the background sky level
-        in order to account for uncertainty in the background sky subtraction.
-        """
-        if self.use_hyper_scaling:
+    def galaxy_redshifts(self) -> List[float]:
+        return [galaxy.redshift for galaxy in self.galaxies]
 
-            return hyper_image_from(
-                image=self.dataset.image, hyper_image_sky=self.hyper_image_sky
-            )
-
-        return self.dataset.data
+    def has(self, cls: Tuple[Type]) -> bool:
+        if self.galaxies is not None:
+            return any(list(map(lambda galaxy: galaxy.has(cls=cls), self.galaxies)))
+        return False
 
-    @property
-    def noise_map(self) -> aa.Array2D:
+    def cls_list_from(self, cls: Type) -> List:
         """
-        Returns the imaging noise-map, which may have a hyper scaling performed which increase the noise in regions of
-        the data that are poorly fitted in order to avoid overfitting.
-        """
-        if self.use_hyper_scaling:
-
-            return hyper_noise_map_from(
-                noise_map=self.dataset.noise_map,
-                model_obj=self.plane,
-                hyper_background_noise=self.hyper_background_noise,
-            )
+        Returns a list of objects in the plane which are an instance of the input `cls`.
 
-        return self.dataset.noise_map
+        For example:
 
-    @property
-    def blurred_image(self) -> aa.Array2D:
-        """
-        Returns the image of the light profiles of all galaxies in the fit's plane, convolved with the
-        imaging dataset's PSF.
+        - If the input is `cls=ag.LightProfile`, a list containing all light profiles in the plane is returned.
 
-        If the plane does not have any light profiles, the image is computed bypassing the convolution routine
-        altogether.
+        Returns
+        -------
+            The list of objects in the plane that inherit from input `cls`.
         """
+        cls_list = []
 
-        if len(self.plane.cls_list_from(cls=LightProfile)) == len(self.plane.cls_list_from(cls=LightProfileOperated)):
+        for galaxy in self.galaxies:
+            if galaxy.has(cls=cls):
+                for cls_galaxy in galaxy.cls_list_from(cls=cls):
+                    cls_list.append(cls_galaxy)
 
-            return self.plane.image_2d_from(
-                grid=self.dataset.grid,
-            )
+        return cls_list
 
-        return self.plane.blurred_image_2d_from(
-            grid=self.dataset.grid,
-            convolver=self.dataset.convolver,
-            blurring_grid=self.dataset.blurring_grid,
-        )
+    def galaxies_with_cls_list_from(self, cls: Type) -> List[Galaxy]:
+        return list(filter(lambda galaxy: galaxy.has(cls=cls), self.galaxies))
 
     @property
-    def profile_subtracted_image(self) -> aa.Array2D:
-        """
-        Returns the dataset's image data with all blurred light profile images in the fit's plane subtracted.
-        """
-        return self.image - self.blurred_image
+    def adapt_galaxies_with_pixelization_image_list(self) -> List[aa.Array2D]:
+        return [
+            galaxy.adapt_galaxy_image
+            for galaxy in self.galaxies_with_cls_list_from(cls=aa.Pixelization)
+        ]
 
-    @property
-    def model_data(self) -> aa.Array2D:
+    @aa.grid_dec.grid_2d_to_structure
+    def image_2d_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> aa.Array2D:
         """
-        Returns the model-image that is used to fit the data.
+        Returns the profile-image plane image of the list of galaxies of the plane's sub-grid, by summing the
+        individual images of each galaxy's light profile.
 
-        If the plane does not have any linear objects and therefore omits an inversion, the model data is the
-        sum of all light profile images blurred with the PSF.
+        If the `operated_only` input is included, the function omits light profiles which are parents of
+        the `LightProfileOperated` object, which signifies that the light profile represents emission that has
+        already had the instrument operations (e.g. PSF convolution, a Fourier transform) applied to it.
 
-        If a inversion is included it is the sum of this image and the inversion's reconstruction of the image.
-        """
-        return self.blurred_image
+        If the plane has no galaxies (or no galaxies have mass profiles) an arrays of all zeros the shape of the plane's
+        sub-grid is returned.
 
-    @property
-    def plane_to_inversion(self) -> PlaneToInversion:
-        return PlaneToInversion(
-            plane=self.plane,
-            dataset=self.dataset,
-            data=self.profile_subtracted_image,
-            noise_map=self.noise_map,
-            w_tilde=self.w_tilde,
-            settings_pixelization=self.settings_pixelization,
-            settings_inversion=self.settings_inversion,
-            preloads=self.preloads,
-        )
+        Parameters
+        ----------
+        grid
+            The 2D (y, x) coordinates where values of the image are evaluated.
+        operated_only
+            By default, the image is the sum of light profile images (irrespective of whether they have been operatd on
+            or not). If this input is included as a bool, only images which are or are not already operated are summed
+            and returned.
+        """
+        if self.galaxies:
+            return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
+        return np.zeros((grid.shape[0],))
+
+    def image_2d_list_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> List[aa.Array2D]:
+        return [
+            galaxy.image_2d_from(grid=grid, operated_only=operated_only)
+            for galaxy in self.galaxies
+        ]
+
+    def galaxy_image_2d_dict_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> {Galaxy: np.ndarray}:
+        """
+        Returns a dictionary associating every `Galaxy` object in the `Plane` with its corresponding 2D image, using
+        the instance of each galaxy as the dictionary keys.
+
+        This object is used for adapt features, which use the image of each galaxy in a model-fit in order to
+        adapt quantities like a pixelization or regularization scheme to the surface brightness of the galaxies being
+        fitted.
+
+        By inheriting from `OperateImageGalaxies` functions which apply operations of this dictionary are accessible,
+        for example convolving every image with a PSF or applying a Fourier transform to create a galaxy-visibilities
+        dictionary.
 
-    @cached_property
-    def inversion(self) -> Optional[aa.AbstractInversion]:
-        """
-        If the plane has linear objects which are used to fit the data (e.g. a linear light profile / pixelization)
-        this function returns a linear inversion, where the flux values of these objects (e.g. the `intensity`
-        of linear light profiles) are computed via linear matrix algebra.
+        Parameters
+        ----------
+        grid
+            The 2D (y,x) coordinates of the (masked) grid, in its original geometric reference frame.
 
-        The data passed to this function is the dataset's image with all light profile images of the plane subtracted,
-        ensuring that the inversion only fits the data with ordinary light profiles subtracted.
+        Returns
+        -------
+        A dictionary associated every galaxy in the plane with its corresponding 2D image.
         """
 
-        if self.perform_inversion:
-            return self.plane_to_inversion.inversion
-
-    @property
-    def model_data(self) -> aa.Array2D:
-        """
-        Returns the model-image that is used to fit the data.
+        galaxy_image_2d_dict = dict()
 
-        If the plane does not have any linear objects and therefore omits an inversion, the model data is the
-        sum of all light profile images blurred with the PSF.
+        image_2d_list = self.image_2d_list_from(grid=grid, operated_only=operated_only)
 
-        If a inversion is included it is the sum of this image and the inversion's reconstruction of the image.
-        """
+        for galaxy_index, galaxy in enumerate(self.galaxies):
+            galaxy_image_2d_dict[galaxy] = image_2d_list[galaxy_index]
 
-        if self.perform_inversion:
+        return galaxy_image_2d_dict
 
-            return self.blurred_image + self.inversion.mapped_reconstructed_data
+    def plane_image_2d_from(
+        self, grid: aa.type.Grid2DLike, zoom_to_brightest: bool = True
+    ) -> aa.Array2D:
+        return plane_util.plane_image_from(
+            galaxies=self.galaxies,
+            grid=grid.mask.derive_grid.all_false_sub_1,
+            zoom_to_brightest=zoom_to_brightest,
+        )
 
-        return self.blurred_image
+    @aa.grid_dec.grid_2d_to_vector_yx
+    @aa.grid_dec.grid_2d_to_structure
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+        if self.galaxies:
+            return sum(
+                map(lambda g: g.deflections_yx_2d_from(grid=grid), self.galaxies)
+            )
+        return np.zeros(shape=(grid.shape[0], 2))
 
-    @property
-    def galaxy_model_image_dict(self) -> Dict[Galaxy, np.ndarray]:
+    @aa.grid_dec.grid_2d_to_structure
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
         """
-        A dictionary which associates every galaxy in the plane with its `model_image`.
+        Returns the convergence of the list of galaxies of the plane's sub-grid, by summing the individual convergences \
+        of each galaxy's mass profile.
 
-        This image is the image of the sum of:
+        The convergence is calculated on the sub-grid and binned-up to the original grid by taking the mean
+        value of every set of sub-pixels, provided the *returned_binned_sub_grid* bool is `True`.
 
-        - The images of all ordinary light profiles in that plane summed and convolved with the imaging data's PSF.
-        - The images of all linear objects (e.g. linear light profiles / pixelizations), where the images are solved
-          for first via the inversion.
+        If the plane has no galaxies (or no galaxies have mass profiles) an arrays of all zeros the shape of the plane's
+        sub-grid is returned.
 
-        For modeling, this dictionary is used to set up the `hyper_images` that adapt certain pixelizations to the
-        data being fitted.
-        """
+        Internally data structures are treated as ndarrays, however the decorator `grid_2d_to_structure` converts
+        the output to an `Array2D` using the input `grid`'s attributes.
 
-        galaxy_blurred_image_2d_dict = self.plane.galaxy_blurred_image_2d_dict_from(
-            grid=self.grid,
-            convolver=self.imaging.convolver,
-            blurring_grid=self.imaging.blurring_grid,
-        )
+        Parameters
+        ----------
+        grid : Grid2D
+            The grid (or sub) of (y,x) arc-second coordinates at the centre of every unmasked pixel which the \
+            potential is calculated on.
+        galaxies : [Galaxy]
+            The galaxies whose mass profiles are used to compute the surface densities.
+        """
+        if self.galaxies:
+            return sum(map(lambda g: g.convergence_2d_from(grid=grid), self.galaxies))
+        return np.zeros((grid.shape[0],))
+
+    @aa.grid_dec.grid_2d_to_structure
+    def potential_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+        """
+        Returns the potential of the list of galaxies of the plane's sub-grid, by summing the individual potentials \
+        of each galaxy's mass profile.
 
-        galaxy_linear_obj_image_dict = self.galaxy_linear_obj_data_dict_from(
-            use_image=True
-        )
+        The potential is calculated on the sub-grid and binned-up to the original grid by taking the mean
+        value of every set of sub-pixels, provided the *returned_binned_sub_grid* bool is `True`.
 
-        return {**galaxy_blurred_image_2d_dict, **galaxy_linear_obj_image_dict}
+        If the plane has no galaxies (or no galaxies have mass profiles) an arrays of all zeros the shape of the plane's
+        sub-grid is returned.
 
-    @property
-    def model_images_of_galaxies_list(self) -> List:
+        Internally data structures are treated as ndarrays, however the decorator `grid_2d_to_structure` converts
+        the output to an `Array2D` using the input `grid`'s attributes.
+
+        Parameters
+        ----------
+        grid : Grid2D
+            The grid (or sub) of (y,x) arc-second coordinates at the centre of every unmasked pixel which the \
+            potential is calculated on.
+        galaxies : [Galaxy]
+            The galaxies whose mass profiles are used to compute the surface densities.
+        """
+        if self.galaxies:
+            return sum(map(lambda g: g.potential_2d_from(grid=grid), self.galaxies))
+        return np.zeros((grid.shape[0],))
+
+    @aa.grid_dec.grid_2d_to_structure
+    def traced_grid_from(self, grid: aa.type.Grid2DLike) -> aa.type.Grid2DLike:
         """
-        A list of the model images of each galaxy in the plane.
+        Trace this plane's grid_stacks to the next plane, using its deflection angles.
         """
-        return list(self.galaxy_model_image_dict.values())
+        return grid - self.deflections_yx_2d_from(grid=grid)
 
     @property
-    def subtracted_images_of_galaxies_list(self) -> List[aa.Array2D]:
+    def perform_inversion(self) -> bool:
         """
-        A list of the subtracted image of every galaxy.
+        Returns a bool specifying whether this fit object performs an inversion.
 
-        A subtracted image of a galaxy is the data where all other galaxy images are subtracted from it, therefore
-        showing how a galaxy appears in the data in the absence of all other galaxies.
+        This is based on whether any of the galaxies in the `model_obj` have a `Pixelization` or `LightProfileLinear`
+        object, in which case an inversion is performed.
 
-        This is used to visualize the contribution of each galaxy in the data.
+        Returns
+        -------
+            A bool which is True if an inversion is performed.
         """
+        if self.has(cls=(aa.Pixelization, LightProfileLinear)):
+            return True
+        elif self.has(cls=Basis):
+            basis_list = self.cls_list_from(cls=Basis)
+            for basis in basis_list:
+                for light_profile in basis.light_profile_list:
+                    if isinstance(light_profile, LightProfileLinear):
+                        return True
 
-        subtracted_images_of_galaxies_list = []
+        return False
 
-        model_images_of_galaxies_list = self.model_images_of_galaxies_list
+    def extract_attribute(self, cls, attr_name):
+        """
+        Returns an attribute of a class in `Plane` as a `ValueIrregular` or `Grid2DIrregular` object.
 
-        for galaxy_index in range(len(self.galaxies)):
+        For example, if a plane has a galaxy which two light profiles and we want its axis-ratios, the following:
 
-            other_galaxies_model_images = [
-                model_image
-                for i, model_image in enumerate(model_images_of_galaxies_list)
-                if i != galaxy_index
-            ]
+        `plane.extract_attribute(cls=LightProfile, name="axis_ratio")`
 
-            subtracted_image = self.image - sum(other_galaxies_model_images)
+        would return:
 
-            subtracted_images_of_galaxies_list.append(subtracted_image)
+        ArrayIrregular(values=[axis_ratio_0, axis_ratio_1])
 
-        return subtracted_images_of_galaxies_list
+        If a galaxy has three mass profiles and we want their centres, the following:
 
-    @property
-    def unmasked_blurred_image(self) -> aa.Array2D:
-        """
-        The blurred image of the overall fit that would be evaluated without a mask being used.
+        `plane.extract_attribute(cls=MassProfile, name="centres")`
 
-        Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
-        image cannot be computed.
-        """
-        if self.plane.has(cls=LightProfileLinear):
-            exc.raise_linear_light_profile_in_unmasked()
+        would return:
 
-        return self.plane.unmasked_blurred_image_2d_from(
-            grid=self.grid, psf=self.imaging.psf
-        )
+        GridIrregular2D(grid=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1), (centre_y_2, centre_x_2)])
 
-    @property
-    def unmasked_blurred_image_of_galaxies_list(self) -> List[aa.Array2D]:
+        This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
         """
-        The blurred image of every galaxy int he plane used in this fit, that would be evaluated without a mask being
-        used.
 
-        Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
-        image cannot be computed.
-        """
-        if self.plane.has(cls=LightProfileLinear):
-            exc.raise_linear_light_profile_in_unmasked()
+        def extract(value, name):
+            try:
+                return getattr(value, name)
+            except (AttributeError, IndexError):
+                return None
 
-        return self.plane.unmasked_blurred_image_2d_list_from(
-            grid=self.grid, psf=self.imaging.psf
-        )
+        attributes = [
+            extract(value, attr_name)
+            for galaxy in self.galaxies
+            for value in galaxy.__dict__.values()
+            if isinstance(value, cls)
+        ]
 
-    @property
-    def plane_linear_light_profiles_to_light_profiles(self) -> Plane:
-        """
-        The `Plane` where all linear light profiles have been converted to ordinary light profiles, where their
-        `intensity` values are set to the values inferred by this fit.
+        if attributes == []:
+            return None
+        elif isinstance(attributes[0], float):
+            return aa.ArrayIrregular(values=attributes)
+        elif isinstance(attributes[0], tuple):
+            return aa.Grid2DIrregular(values=attributes)
 
-        This is typically used for visualization, because linear light profiles cannot be used in `LightProfilePlotter`
-        or `GalaxyPlotter` objects.
+    def extract_attributes_of_galaxies(self, cls, attr_name, filter_nones=False):
         """
-        return self.model_obj_linear_light_profiles_to_light_profiles
+        Returns an attribute of a class in the plane as a list of `ValueIrregular` or `Grid2DIrregular` objects,
+        where the list indexes correspond to each galaxy in the plane..
 
-    def refit_with_new_preloads(
-        self,
-        preloads: Preloads,
-        settings_inversion: Optional[aa.SettingsInversion] = None,
-    ) -> "FitImaging":
-        """
-        Returns a new fit which uses the dataset, plane and other objects of this fit, but uses a different set of
-        preloads input into this function.
+        For example, if a plane has two galaxies which each have a light profile the following:
 
-        This is used when setting up the preloads objects, to concisely test how using different preloads objects
-        changes the attributes of the fit.
+        `plane.extract_attributes_of_galaxies(cls=LightProfile, name="axis_ratio")`
 
-        Parameters
-        ----------
-        preloads
-            The new preloads which are used to refit the data using the
-        settings_inversion
-            Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
+        would return:
 
-        Returns
-        -------
-        A new fit which has used new preloads input into this function but the same dataset, plane and other settings.
-        """
-        profiling_dict = {} if self.profiling_dict is not None else None
+        [ArrayIrregular(values=[axis_ratio_0]), ArrayIrregular(values=[axis_ratio_1])]
 
-        settings_inversion = (
-            self.settings_inversion
-            if settings_inversion is None
-            else settings_inversion
-        )
+        If a plane has two galaxies, the first with a mass profile and the second with two mass profiles ,the following:
 
-        return FitImaging(
-            dataset=self.imaging,
-            plane=self.plane,
-            hyper_image_sky=self.hyper_image_sky,
-            hyper_background_noise=self.hyper_background_noise,
-            use_hyper_scaling=self.use_hyper_scaling,
-            settings_pixelization=self.settings_pixelization,
-            settings_inversion=settings_inversion,
-            preloads=preloads,
-            profiling_dict=profiling_dict,
-        )
+        `plane.extract_attributes_of_galaxies(cls=MassProfile, name="centres")`
 
+        would return:
+        [
+            Grid2DIrregular(values=[(centre_y_0, centre_x_0)]),
+            Grid2DIrregular(values=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1)])
+        ]
 
-def hyper_image_from(image: aa.Array2D, hyper_image_sky: HyperImageSky) -> aa.Array2D:
-    """
-    Returns a `hyper_image` from the input data's `image` used in a fit.
-
-    The `hyper_image` is the image with its background sky subtraction changed based on the `hyper_image_sky` object,
-    which scales the sky level using a `sky_scale` parameter.
-
-    Parameters
-    ----------
-    image
-        The image of the data whose background sky is changed.
-    hyper_image_sky
-        The model image describing how much the background sky level is scaled.
-
-    Returns
-    -------
-    The image whose background sky is scaled.
-    """
-    if hyper_image_sky is not None:
-        return hyper_image_sky.hyper_image_from(image=image)
-    return image
-
-
-def hyper_noise_map_from(
-    noise_map: aa.Array2D, model_obj, hyper_background_noise: HyperBackgroundNoise
-) -> aa.Array2D:
-    """
-    Returns a `hyper_noise_map` from the input data's `noise_map` used in a fit.
-
-    The `hyper_noise_map` is the noise-map with a background value added or subtracted from it, based on
-    the `hyper_background_noise` object, which scales the noise level using a `noise_scale` parameter.
-
-    Parameters
-    ----------
-    image
-        The image of the data whose background sky is changed.
-    hyper_image_sky
-        The model image describing how much the background sky level is scaled.
-
-    Returns
-    -------
-    The image whose background sky is scaled.
-    """
-    hyper_noise_map = model_obj.hyper_noise_map_from(noise_map=noise_map)
-
-    if hyper_background_noise is not None:
-        noise_map = hyper_background_noise.hyper_noise_map_from(noise_map=noise_map)
-
-    if hyper_noise_map is not None:
-        noise_map = noise_map + hyper_noise_map
-        noise_map_limit = conf.instance["general"]["hyper"]["hyper_noise_limit"]
-        noise_map[noise_map > noise_map_limit] = noise_map_limit
+        If a Profile does not have a certain entry, it is replaced with a None. Nones can be removed by
+        setting `filter_nones=True`.
 
-    return noise_map
+        This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
+        """
+        if filter_nones:
+            return [
+                galaxy.extract_attribute(cls=cls, attr_name=attr_name)
+                for galaxy in self.galaxies
+                if galaxy.extract_attribute(cls=cls, attr_name=attr_name) is not None
+            ]
+
+        else:
+            return [
+                galaxy.extract_attribute(cls=cls, attr_name=attr_name)
+                for galaxy in self.galaxies
+            ]
+
+    def set_snr_of_snr_light_profiles(
+        self,
+        grid: aa.type.Grid2DLike,
+        exposure_time: float,
+        background_sky_level: float = 0.0,
+        psf: Optional[aa.Kernel2D] = None,
+    ):
+        """
+        Iterate over every `LightProfileSNR` in the plane and set their `intensity` values to values which give
+        their input `signal_to_noise_ratio` value, which is performed as follows:
+
+        - Evaluate the image of each light profile on the input grid.
+        - Blur this image with a PSF, if included.
+        - Take the value of the brightest pixel.
+        - Use an input `exposure_time` and `background_sky` (e.g. from the `SimulatorImaging` object) to determine
+          what value of `intensity` gives the desired signal to noise ratio for the image.
+
+        Parameters
+        ----------
+        grid
+            The (y, x) coordinates in the original reference frame of the grid.
+        exposure_time
+            The exposure time of the simulated imaging.
+        background_sky_level
+            The level of the background sky of the simulated imaging.
+        psf
+            The psf of the simulated imaging which can change the S/N of the light profile due to spreading out
+            the emission.
+        """
+        for galaxy in self.galaxies:
+            for light_profile in galaxy.cls_list_from(cls=LightProfile):
+                if isinstance(light_profile, LightProfileSNR):
+                    light_profile.set_intensity_from(
+                        grid=grid,
+                        exposure_time=exposure_time,
+                        background_sky_level=background_sky_level,
+                        psf=psf,
+                    )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/imaging/imaging.py` & `autogalaxy-2023.7.7.1/autogalaxy/imaging/imaging.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,17 @@
             psf=self.psf,
         )
 
         image = plane.padded_image_2d_from(
             grid=grid, psf_shape_2d=self.psf.shape_native
         )
 
-        imaging = self.via_image_from(image=image.binned)
+        dataset = self.via_image_from(image=image.binned)
 
-        return imaging.trimmed_after_convolution_from(
+        return dataset.trimmed_after_convolution_from(
             kernel_shape=self.psf.shape_native
         )
 
     def via_galaxies_from(self, galaxies, grid):
         """
         Simulate imaging data for this data, as follows:
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/imaging/model/analysis.py` & `autogalaxy-2023.7.7.1/autogalaxy/imaging/model/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 from autoarray.exc import PixelizationException
 
 from autogalaxy.analysis.analysis import AnalysisDataset
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.cosmology.lensing import LensingCosmology
 from autogalaxy.cosmology.wrap import Planck15
 from autogalaxy.imaging.model.visualizer import VisualizerImaging
-from autogalaxy.hyper.hyper_data import HyperImageSky
-from autogalaxy.hyper.hyper_data import HyperBackgroundNoise
 from autogalaxy.imaging.model.result import ResultImaging
 from autogalaxy.imaging.fit_imaging import FitImaging
 from autogalaxy.plane.plane import Plane
 
 from autogalaxy import exc
 
 
 class AnalysisImaging(AnalysisDataset):
     def __init__(
         self,
         dataset: aa.Imaging,
-        hyper_dataset_result: ResultImaging = None,
+        adapt_result: ResultImaging = None,
         cosmology: LensingCosmology = Planck15(),
         settings_pixelization: aa.SettingsPixelization = None,
         settings_inversion: aa.SettingsInversion = None,
     ):
         """
         Analysis classes are used by PyAutoFit to fit a model to a dataset via a non-linear search.
 
@@ -38,50 +36,50 @@
         such as visualization, outputting results to hard-disk and storing results in a format that can be loaded after
         the model-fit is complete using PyAutoFit's database tools.
 
         This Analysis class is used for model-fits which fit galaxies (or objects containing galaxies like a `Plane`)
         to an imaging dataset.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. a
-        pixelization or inversion), the Cosmology used for the analysis and hyper datasets used for certain model
+        pixelization or inversion), the Cosmology used for the analysis and adapt datasets used for certain model
         classes.
 
         Parameters
         ----------
         dataset
             The `Imaging` dataset that the model is fitted too.
-        hyper_dataset_result
-            The hyper-model image and hyper galaxies images of a previous result in a model-fitting pipeline, which are
+        adapt_result
+            The adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
             used by certain classes for adapting the analysis to the properties of the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         settings_pixelization
             Settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         """
         super().__init__(
             dataset=dataset,
-            hyper_dataset_result=hyper_dataset_result,
+            adapt_result=adapt_result,
             cosmology=cosmology,
             settings_pixelization=settings_pixelization,
             settings_inversion=settings_inversion,
         )
 
     @property
     def imaging(self):
         return self.dataset
 
     def modify_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
         """
         PyAutoFit calls this function immediately before the non-linear search begins, therefore it can be used to
         perform tasks using the final model parameterization.
 
-        This function checks that the hyper-dataset is consistent with previous hyper-datasets if the model-fit is
+        This function checks that the adapt-dataset is consistent with previous adapt-datasets if the model-fit is
         being resumed from a previous run, and it visualizes objects which do not change throughout the model fit
         like the dataset.
 
         Parameters
         ----------
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
@@ -90,40 +88,28 @@
             The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
             the imaging data.
         """
 
         super().modify_before_fit(paths=paths, model=model)
 
         if not paths.is_complete:
-
-            if not os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-
-                visualizer = VisualizerImaging(visualize_path=paths.image_path)
-
-                visualizer.visualize_imaging(imaging=self.imaging)
-
-                visualizer.visualize_hyper_images(
-                    hyper_galaxy_image_path_dict=self.hyper_galaxy_image_path_dict,
-                    hyper_model_image=self.hyper_model_image,
-                )
-
             self.set_preloads(paths=paths, model=model)
 
         return self
 
     def log_likelihood_function(self, instance: af.ModelInstance) -> float:
         """
         Given an instance of the model, where the model parameters are set via a non-linear search, fit the model
         instance to the imaging dataset.
 
         This function returns a log likelihood which is used by the non-linear search to guide the model-fit.
 
         For this analysis class, this function performs the following steps:
 
-        1) If the analysis has a hyper dataset, associated the model galaxy images of this dataset to the galaxies in
+        1) If the analysis has a adapt dataset, associated the model galaxy images of this dataset to the galaxies in
            the model instance.
 
         2) Extract attributes which model aspects of the data reductions, like the scaling the background sky
            and background noise.
 
         3) Extracts all galaxies from the model instance and set up a `Plane`.
 
@@ -160,87 +146,64 @@
             OverflowError,
         ) as e:
             raise exc.FitException from e
 
     def fit_imaging_via_instance_from(
         self,
         instance: af.ModelInstance,
-        use_hyper_scaling: bool = True,
         preload_overwrite: Optional[Preloads] = None,
         profiling_dict: Optional[Dict] = None,
     ) -> FitImaging:
         """
         Given a model instance create a `FitImaging` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
         Parameters
         ----------
         instance
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
-        use_hyper_scaling
-            If false, the scaling of the background sky and noise are not performed irrespective of the model components
-            themselves.
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitImaging
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
-        instance = self.instance_with_associated_hyper_images_from(instance=instance)
-
-        hyper_image_sky = self.hyper_image_sky_via_instance_from(instance=instance)
-
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
+        instance = self.instance_with_associated_adapt_images_from(instance=instance)
 
         plane = self.plane_via_instance_from(instance=instance)
 
         return self.fit_imaging_via_plane_from(
             plane=plane,
-            hyper_image_sky=hyper_image_sky,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
             preload_overwrite=preload_overwrite,
             profiling_dict=profiling_dict,
         )
 
     def fit_imaging_via_plane_from(
         self,
         plane: Plane,
-        hyper_image_sky: Optional[HyperImageSky],
-        hyper_background_noise: Optional[HyperBackgroundNoise],
-        use_hyper_scaling: bool = True,
         preload_overwrite: Optional[Preloads] = None,
         profiling_dict: Optional[Dict] = None,
     ) -> FitImaging:
         """
         Given a `Plane`, which the analysis constructs from a model instance, create a `FitImaging` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
         Parameters
         ----------
         plane
             The plane of galaxies whose model images are used to fit the imaging data.
-        hyper_image_sky
-            A model component which scales the background sky level of the data before computing the log likelihood.
-        hyper_background_noise
-            A model component which scales the background noise level of the data before computing the log likelihood.
-        use_hyper_scaling
-            If false, the scaling of the background sky and noise are not performed irrespective of the model components
-            themselves.
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
@@ -249,27 +212,51 @@
         """
 
         preloads = self.preloads if preload_overwrite is None else preload_overwrite
 
         return FitImaging(
             dataset=self.dataset,
             plane=plane,
-            hyper_image_sky=hyper_image_sky,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     @property
     def fit_func(self):
         return self.fit_imaging_via_instance_from
 
+    def visualize_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
+        """
+        PyAutoFit calls this function immediately before the non-linear search begins.
+
+        It visualizes objects which do not change throughout the model fit like the dataset.
+
+        Parameters
+        ----------
+        paths
+            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
+            visualization and the pickled objects used by the aggregator output by this function.
+        model
+            The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
+            the imaging data.
+        """
+        if not self.should_visualize(paths=paths):
+            return
+
+        visualizer = VisualizerImaging(visualize_path=paths.image_path)
+
+        visualizer.visualize_imaging(dataset=self.dataset)
+
+        visualizer.visualize_adapt_images(
+            adapt_galaxy_image_path_dict=self.adapt_galaxy_image_path_dict,
+            adapt_model_image=self.adapt_model_image,
+        )
+
     def visualize(
         self,
         paths: af.DirectoryPaths,
         instance: af.ModelInstance,
         during_analysis: bool,
     ):
         """
@@ -280,20 +267,17 @@
         The visualization performed by this function includes:
 
         - Images of the best-fit `Plane`, including the images of each of its galaxies.
 
         - Images of the best-fit `FitImaging`, including the model-image, residuals and chi-squared of its fit to
           the imaging data.
 
-        - The hyper-images of the model-fit showing how the hyper galaxies are used to represent different galaxies in
+        - The adapt-images of the model-fit showing how the galaxies are used to represent different galaxies in
           the dataset.
 
-        - If hyper features are used to scale the noise or background sky, a `FitImaging` with these features turned
-          off may be output, to indicate how much these features are altering the dataset.
-
         The images output by this function are customized using the file `config/visualize/plots.ini`.
 
         Parameters
         ----------
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
             visualization, and the pickled objects used by the aggregator output by this function.
@@ -301,33 +285,26 @@
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
         during_analysis
             If True the visualization is being performed midway through the non-linear search before it is finished,
             which may change which images are output.
         """
 
-        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+        if not self.should_visualize(paths=paths):
             return
 
-        instance = self.instance_with_associated_hyper_images_from(instance=instance)
+        instance = self.instance_with_associated_adapt_images_from(instance=instance)
         plane = self.plane_via_instance_from(instance=instance)
 
-        hyper_image_sky = self.hyper_image_sky_via_instance_from(instance=instance)
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
-
         fit = self.fit_imaging_via_plane_from(
             plane=plane,
-            hyper_image_sky=hyper_image_sky,
-            hyper_background_noise=hyper_background_noise,
         )
 
         visualizer = VisualizerImaging(visualize_path=paths.image_path)
-        visualizer.visualize_imaging(imaging=self.imaging)
+        visualizer.visualize_imaging(dataset=self.dataset)
 
         try:
             visualizer.visualize_fit_imaging(fit=fit, during_analysis=during_analysis)
         except exc.InversionException:
             pass
 
         plane = fit.plane_linear_light_profiles_to_light_profiles
@@ -339,35 +316,19 @@
             galaxies=plane.galaxies, grid=fit.grid, during_analysis=during_analysis
         )
         if fit.inversion is not None:
             visualizer.visualize_inversion(
                 inversion=fit.inversion, during_analysis=during_analysis
             )
 
-        visualizer.visualize_hyper_images(
-            hyper_galaxy_image_path_dict=self.hyper_galaxy_image_path_dict,
-            hyper_model_image=self.hyper_model_image,
+        visualizer.visualize_adapt_images(
+            adapt_galaxy_image_path_dict=self.adapt_galaxy_image_path_dict,
+            adapt_model_image=self.adapt_model_image,
         )
 
-        if visualizer.plot_fit_no_hyper:
-
-            fit = self.fit_imaging_via_plane_from(
-                plane=plane,
-                hyper_image_sky=None,
-                hyper_background_noise=None,
-                use_hyper_scaling=False,
-            )
-
-            try:
-                visualizer.visualize_fit_imaging(
-                    fit=fit, during_analysis=during_analysis, subfolders="fit_no_hyper"
-                )
-            except (exc.InversionException, np.linalg.LinAlgError):
-                pass
-
     def make_result(
         self,
         samples: af.SamplesPDF,
         model: af.Collection,
         sigma=1.0,
         use_errors=True,
         use_widths=False,
@@ -380,15 +341,15 @@
 
         - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
           an instance of the maximum log likelihood model).
 
         - The non-linear search used to perform the model fit.
 
         The `ResultImaging` object contains a number of methods which use the above objects to create the max
-        log likelihood `Plane`, `FitImaging`, hyper-galaxy images,etc.
+        log likelihood `Plane`, `FitImaging`, adapt-galaxy images,etc.
 
         Parameters
         ----------
         samples
             A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
             run of samples of the nested sampler.
         model
@@ -403,25 +364,25 @@
             The result of fitting the model to the imaging dataset, via a non-linear search.
         """
         return ResultImaging(samples=samples, model=model, analysis=self)
 
     def save_attributes_for_aggregator(self, paths: af.DirectoryPaths):
         """
          Before the non-linear search begins, this routine saves attributes of the `Analysis` object to the `pickles`
-         folder such that they can be load after the analysis using PyAutoFit's database and aggregator tools.
+         folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
          For this analysis, it uses the `AnalysisDataset` object's method to output the following:
 
          - The dataset's data.
          - The dataset's noise-map.
          - The settings associated with the dataset.
          - The settings associated with the inversion.
          - The settings associated with the pixelization.
          - The Cosmology.
-         - The hyper dataset's model image and galaxy images, if used.
+         - The adapt dataset's model image and galaxy images, if used.
 
          This function also outputs attributes specific to an imaging dataset:
 
         - Its PSF.
         - Its mask.
 
          It is common for these attributes to be loaded by many of the template aggregator functions given in the
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/imaging/model/result.py` & `autogalaxy-2023.7.7.1/autogalaxy/imaging/model/result.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
     an instance of the maximum log likelihood model).
 
     - The non-linear search used to perform the model fit.
 
     This class contains a number of methods which use the above objects to create the max log likelihood `Plane`,
-    `FitImaging`, hyper-galaxy images,etc.
+    `FitImaging`, adapt-galaxy images,etc.
 
     Parameters
     ----------
     samples
         A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
         run of samples of the nested sampler.
     model
@@ -42,32 +42,22 @@
 
     @property
     def max_log_likelihood_fit(self) -> FitImaging:
         """
         An instance of a `FitImaging` corresponding to the maximum log likelihood model inferred by the non-linear
         search.
         """
-        hyper_image_sky = self.analysis.hyper_image_sky_via_instance_from(
-            instance=self.instance_copy
-        )
-
-        hyper_background_noise = self.analysis.hyper_background_noise_via_instance_from(
-            instance=self.instance_copy
-        )
-
-        instance = self.analysis.instance_with_associated_hyper_images_from(
+        instance = self.analysis.instance_with_associated_adapt_images_from(
             instance=self.instance_copy
         )
 
         plane = self.analysis.plane_via_instance_from(instance=instance)
 
         return self.analysis.fit_imaging_via_plane_from(
             plane=plane,
-            hyper_image_sky=hyper_image_sky,
-            hyper_background_noise=hyper_background_noise,
         )
 
     @property
     def max_log_likelihood_plane(self) -> Plane:
         """
         An instance of a `Plane` corresponding to the maximum log likelihood model inferred by the non-linear search.
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/imaging/model/visualizer.py` & `autogalaxy-2023.7.7.1/autogalaxy/imaging/model/visualizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from autogalaxy.analysis.visualizer import Visualizer
 
 from autogalaxy.analysis.visualizer import plot_setting
 
 
 class VisualizerImaging(Visualizer):
     def visualize_fit_imaging(
-        self, fit: FitImaging, during_analysis: bool, subfolders: str = "fit_imaging"
+        self, fit: FitImaging, during_analysis: bool, subfolders: str = "fit_dataset"
     ):
         """
         Visualizes a `FitImaging` object, which fits an imaging dataset.
 
         Images are output to the `image` folder of the `visualize_path` in a subfolder called `fit`. When
         used with a non-linear search the `visualize_path` points to the search's results folder and this function
         visualizes the maximum log likelihood `FitImaging` inferred by the search so far.
@@ -36,73 +36,74 @@
         """
 
         def should_plot(name):
             return plot_setting(section=["fit", "fit_imaging"], name=name)
 
         mat_plot_2d = self.mat_plot_2d_from(subfolders=subfolders)
 
-        fit_imaging_plotter = FitImagingPlotter(
+        fit_plotter = FitImagingPlotter(
             fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
-        fit_imaging_plotter.figures_2d(
-            image=should_plot("data"),
+        fit_plotter.figures_2d(
+            data=should_plot("data"),
             noise_map=should_plot("noise_map"),
             signal_to_noise_map=should_plot("signal_to_noise_map"),
             model_image=should_plot("model_data"),
             residual_map=should_plot("residual_map"),
             normalized_residual_map=should_plot("normalized_residual_map"),
             chi_squared_map=should_plot("chi_squared_map"),
         )
 
-        fit_imaging_plotter.figures_2d_of_galaxies(
+        fit_plotter.figures_2d_of_galaxies(
             subtracted_image=should_plot("subtracted_images_of_galaxies"),
             model_image=should_plot("model_images_of_galaxies"),
         )
 
         if should_plot("subplot_fit"):
-            fit_imaging_plotter.subplot_fit_imaging()
+            fit_plotter.subplot_fit()
 
         if should_plot("subplot_of_galaxies"):
-            fit_imaging_plotter.subplot_of_galaxies()
+            fit_plotter.subplot_of_galaxies()
 
-        if not during_analysis:
+        if not during_analysis and should_plot("all_at_end_png"):
+            mat_plot_2d = self.mat_plot_2d_from(subfolders=path.join(subfolders, "end"))
 
-            if should_plot("all_at_end_png"):
-
-                fit_imaging_plotter.figures_2d(
-                    image=True,
-                    noise_map=True,
-                    signal_to_noise_map=True,
-                    model_image=True,
-                    residual_map=True,
-                    normalized_residual_map=True,
-                    chi_squared_map=True,
-                )
-
-                fit_imaging_plotter.figures_2d_of_galaxies(
-                    subtracted_image=True, model_image=True
-                )
-
-            if should_plot("all_at_end_fits"):
-
-                mat_plot_2d = self.mat_plot_2d_from(
-                    subfolders=path.join("fit_imaging", "fits"), format="fits"
-                )
-
-                fit_imaging_plotter = FitImagingPlotter(
-                    fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
-                )
-
-                fit_imaging_plotter.figures_2d(
-                    image=True,
-                    noise_map=True,
-                    signal_to_noise_map=True,
-                    model_image=True,
-                    residual_map=True,
-                    normalized_residual_map=True,
-                    chi_squared_map=True,
-                )
-
-                fit_imaging_plotter.figures_2d_of_galaxies(
-                    subtracted_image=True, model_image=True
-                )
+            fit_plotter = FitImagingPlotter(
+                fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+            )
+
+            fit_plotter.figures_2d(
+                data=True,
+                noise_map=True,
+                signal_to_noise_map=True,
+                model_image=True,
+                residual_map=True,
+                normalized_residual_map=True,
+                chi_squared_map=True,
+            )
+
+            fit_plotter.figures_2d_of_galaxies(subtracted_image=True, model_image=True)
+
+        if not during_analysis and should_plot("all_at_end_fits"):
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join(subfolders, "fits"), format="fits"
+            )
+
+            fit_plotter = FitImagingPlotter(
+                fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+            )
+
+            fit_plotter.figures_2d(
+                data=True,
+                noise_map=True,
+                signal_to_noise_map=True,
+                model_image=True,
+                residual_map=True,
+                normalized_residual_map=True,
+                chi_squared_map=True,
+            )
+
+            fit_plotter.figures_2d_of_galaxies(
+                subtracted_image=True,
+                model_image=True,
+            )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/imaging/plot/fit_imaging_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/fit_imaging_plotters.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,14 @@
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
             residuals_symmetric_cmap=residuals_symmetric_cmap,
         )
 
         self.figures_2d = self._fit_imaging_meta_plotter.figures_2d
         self.subplot = self._fit_imaging_meta_plotter.subplot
-        self.subplot_fit_imaging = self._fit_imaging_meta_plotter.subplot_fit_imaging
 
     def get_visuals_2d(self) -> Visuals2D:
         return self.get_2d.via_fit_imaging_from(fit=self.fit)
 
     @property
     def inversion_plotter(self) -> aplt.InversionPlotter:
         """
@@ -141,17 +140,15 @@
         """
         if galaxy_index is None:
             galaxy_indices = self.galaxy_indices
         else:
             galaxy_indices = [galaxy_index]
 
         for galaxy_index in galaxy_indices:
-
             if subtracted_image:
-
                 self.mat_plot_2d.cmap.kwargs["vmin"] = np.max(
                     self.fit.model_images_of_galaxies_list[galaxy_index]
                 )
                 self.mat_plot_2d.cmap.kwargs["vmin"] = np.min(
                     self.fit.model_images_of_galaxies_list[galaxy_index]
                 )
 
@@ -161,24 +158,51 @@
                     auto_labels=aplt.AutoLabels(
                         title=f"Subtracted Image of Galaxy {galaxy_index}",
                         filename=f"subtracted_image_of_galaxy_{galaxy_index}",
                     ),
                 )
 
             if model_image:
-
                 self.mat_plot_2d.plot_array(
                     array=self.fit.model_images_of_galaxies_list[galaxy_index],
                     visuals_2d=self.get_visuals_2d(),
                     auto_labels=aplt.AutoLabels(
                         title=f"Model Image of Galaxy {galaxy_index}",
                         filename=f"model_image_of_galaxy_{galaxy_index}",
                     ),
                 )
 
+    def subplot_fit(self):
+        """
+        Standard subplot of the attributes of the plotter's `FitImaging` object.
+        """
+
+        self.open_subplot_figure(number_subplots=6)
+
+        self.figures_2d(data=True)
+
+        self.figures_2d(signal_to_noise_map=True)
+        self.figures_2d(model_image=True)
+        self.figures_2d(normalized_residual_map=True)
+
+        self.mat_plot_2d.cmap.kwargs["vmin"] = -1.0
+        self.mat_plot_2d.cmap.kwargs["vmax"] = 1.0
+
+        self.set_title(label="Normalized Residual Map (1 sigma)")
+        self.figures_2d(normalized_residual_map=True)
+        self.set_title(label=None)
+
+        self.mat_plot_2d.cmap.kwargs.pop("vmin")
+        self.mat_plot_2d.cmap.kwargs.pop("vmax")
+
+        self.figures_2d(chi_squared_map=True)
+
+        self.mat_plot_2d.output.subplot_to_figure(auto_filename="subplot_fit")
+        self.close_subplot_figure()
+
     def subplot_of_galaxies(self, galaxy_index: Optional[int] = None):
         """
         Plots images representing each individual `Galaxy` in the plotter's `Plane` in 2D on a subplot, which are
         computed via the plotter's 2D grid object.
 
         These images subtract or omit the contribution of other galaxies in the plane, such that plots showing
         each individual galaxy are made.
@@ -194,18 +218,17 @@
 
         if galaxy_index is None:
             galaxy_indices = self.galaxy_indices
         else:
             galaxy_indices = [galaxy_index]
 
         for galaxy_index in galaxy_indices:
-
             self.open_subplot_figure(number_subplots=4)
 
-            self.figures_2d(image=True)
+            self.figures_2d(data=True)
             self.figures_2d_of_galaxies(
                 galaxy_index=galaxy_index, subtracted_image=True
             )
             self.figures_2d_of_galaxies(galaxy_index=galaxy_index, model_image=True)
 
             if self.plane.has(cls=aa.Pixelization):
                 self.inversion_plotter.figures_2d_of_pixelization(
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/interferometer/fit_interferometer.py` & `autogalaxy-2023.7.7.1/autogalaxy/imaging/fit_imaging.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,241 +4,275 @@
 from autoconf import cached_property
 
 import autoarray as aa
 
 from autogalaxy.abstract_fit import AbstractFitInversion
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.hyper.hyper_data import HyperBackgroundNoise
 from autogalaxy.plane.plane import Plane
 from autogalaxy.plane.to_inversion import PlaneToInversion
+from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
+from autogalaxy.profiles.light.operated.abstract import LightProfileOperated
 
+from autogalaxy import exc
 
-class FitInterferometer(aa.FitInterferometer, AbstractFitInversion):
+
+class FitImaging(aa.FitImaging, AbstractFitInversion):
     def __init__(
         self,
-        dataset: aa.Interferometer,
+        dataset: aa.Imaging,
         plane: Plane,
-        hyper_background_noise: HyperBackgroundNoise = None,
-        use_hyper_scaling: bool = True,
         settings_pixelization: aa.SettingsPixelization = aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: aa.Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ):
         """
-        Fits an interferometer dataset using a `Plane` object.
+        Fits an imaging dataset using a `Plane` object.
 
         The fit performs the following steps:
 
         1) Compute the sum of all images of galaxy light profiles in the `Plane`.
 
-        2) Fourier transform this image with the transformer object and `uv_wavelengths` to create
-           the `profile_visibilities`.
+        2) Blur this with the imaging PSF to created the `blurred_image`.
 
-        3) Subtract these visibilities from the `data` to create the `profile_subtracted_visibilities`.
+        3) Subtract this image from the `data` to create the `profile_subtracted_image`.
 
         4) If the `Plane` has any linear algebra objects (e.g. linear light profiles, a pixelization / regulariation)
-           fit the `profile_subtracted_visibilities` with these objects via an inversion.
+           fit the `profile_subtracted_image` with these objects via an inversion.
 
-        5) Compute the `model_data` as the sum of the `profile_visibilities` and `reconstructed_data` of the inversion
-           (if an inversion is not performed the `model_data` is only the `profile_visibilities`.
+        5) Compute the `model_data` as the sum of the `blurred_image` and `reconstructed_data` of the inversion (if
+           an inversion is not performed the `model_data` is only the `blurred_image`.
 
         6) Subtract the `model_data` from the data and compute the residuals, chi-squared and likelihood via the
-           noise-map (if an inversion is performed the `log_evidence`, including addition terms describing the linear
+           noise-map (if an inversion is performed the `log_evidence`, including additional terms describing the linear
            algebra solution, is computed).
 
-        When performing a model-fit` via ` AnalysisInterferometer` object the `figure_of_merit` of
-        this `FitInterferometer` object is called and returned in the `log_likelihood_function`.
+        When performing a `model-fit`via an `AnalysisImaging` object the `figure_of_merit` of this `FitImaging` object
+        is called and returned in the `log_likelihood_function`.
 
         Parameters
         ----------
         dataset
-            The interfometer dataset which is fitted by the galaxies in the plane.
+            The imaging dataset which is fitted by the galaxies in the plane.
         plane
-            The plane of galaxies whose light profile images are used to fit the interferometer data.
-        hyper_background_noise
-            If included, adds a noise-scaling term to the background noise.
-        use_hyper_scaling
-            If set to False, the hyper scaling functions (e.g. the `hyper_background_noise`) are
-            omitted irrespective of their inputs.
+            The plane of galaxies whose light profile images are used to fit the imaging data.
         settings_pixelization
             Settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
             the fit.
         profiling_dict
             A dictionary which if passed to the fit records how long fucntion calls which have the `profile_func`
             decorator take to run.
         """
 
-        try:
-            from autoarray.inversion.inversion import inversion_util_secret
-        except ImportError:
-            settings_inversion.use_w_tilde = False
+        self.plane = plane
+        self.preloads = preloads
 
         super().__init__(
-            dataset=dataset, use_mask_in_fit=False, profiling_dict=profiling_dict
+            dataset=dataset,
+            profiling_dict=profiling_dict,
         )
         AbstractFitInversion.__init__(
             self=self, model_obj=plane, settings_inversion=settings_inversion
         )
 
-        self.plane = plane
-
-        self.hyper_background_noise = hyper_background_noise
-
-        self.use_hyper_scaling = use_hyper_scaling
-
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
 
-        self.preloads = preloads
+    @property
+    def galaxies(self) -> List[Galaxy]:
+        return self.plane.galaxies
+
+    @property
+    def grid(self) -> aa.type.Grid2DLike:
+        return self.dataset.grid
 
     @property
-    def noise_map(self) -> aa.VisibilitiesNoiseMap:
+    def blurred_image(self) -> aa.Array2D:
         """
-        Returns the interferometer's noise-map, which may have a hyper scaling performed which increase the noise in
-        regions of the data that are poorly fitted in order to avoid overfitting.
+        Returns the image of the light profiles of all galaxies in the fit's plane, convolved with the
+        imaging dataset's PSF.
+
+        If the plane does not have any light profiles, the image is computed bypassing the convolution routine
+        altogether.
         """
-        if self.use_hyper_scaling and self.hyper_background_noise is not None:
 
-            return self.hyper_background_noise.hyper_noise_map_complex_from(
-                noise_map=self.dataset.noise_map
+        if len(self.plane.cls_list_from(cls=LightProfile)) == len(
+            self.plane.cls_list_from(cls=LightProfileOperated)
+        ):
+            return self.plane.image_2d_from(
+                grid=self.dataset.grid,
             )
 
-        return self.dataset.noise_map
+        return self.plane.blurred_image_2d_from(
+            grid=self.dataset.grid,
+            convolver=self.dataset.convolver,
+            blurring_grid=self.dataset.blurring_grid,
+        )
 
     @property
-    def profile_visibilities(self) -> aa.Visibilities:
+    def profile_subtracted_image(self) -> aa.Array2D:
         """
-        Returns the visibilities of every light profile of every galaxy in the plane, which are computed by performing
-        a Fourier transform to the sum of light profile images.
+        Returns the dataset's image data with all blurred light profile images in the fit's plane subtracted.
         """
-        return self.plane.visibilities_from(
-            grid=self.dataset.grid, transformer=self.dataset.transformer
-        )
+        return self.image - self.blurred_image
 
     @property
-    def profile_subtracted_visibilities(self) -> aa.Visibilities:
+    def model_data(self) -> aa.Array2D:
         """
-        Returns the interferometer dataset's visibilities with all transformed light profile images in the fit's
-        plane subtracted.
+        Returns the model-image that is used to fit the data.
+
+        If the plane does not have any linear objects and therefore omits an inversion, the model data is the
+        sum of all light profile images blurred with the PSF.
+
+        If a inversion is included it is the sum of this image and the inversion's reconstruction of the image.
         """
-        return self.visibilities - self.profile_visibilities
+        return self.blurred_image
 
     @property
     def plane_to_inversion(self) -> PlaneToInversion:
         return PlaneToInversion(
             plane=self.plane,
             dataset=self.dataset,
-            data=self.profile_subtracted_visibilities,
+            data=self.profile_subtracted_image,
             noise_map=self.noise_map,
             w_tilde=self.w_tilde,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=self.preloads,
         )
 
     @cached_property
     def inversion(self) -> Optional[aa.AbstractInversion]:
         """
         If the plane has linear objects which are used to fit the data (e.g. a linear light profile / pixelization)
         this function returns a linear inversion, where the flux values of these objects (e.g. the `intensity`
         of linear light profiles) are computed via linear matrix algebra.
 
-        The data passed to this function is the dataset's visibilities with all light profile visibilities of the
-        plane subtracted.
+        The data passed to this function is the dataset's image with all light profile images of the plane subtracted,
+        ensuring that the inversion only fits the data with ordinary light profiles subtracted.
         """
-        if self.perform_inversion:
 
+        if self.perform_inversion:
             return self.plane_to_inversion.inversion
 
     @property
-    def model_data(self) -> aa.Visibilities:
+    def model_data(self) -> aa.Array2D:
         """
-        Returns the model data that is used to fit the data.
+        Returns the model-image that is used to fit the data.
 
         If the plane does not have any linear objects and therefore omits an inversion, the model data is the
-        sum of all light profile images Fourier transformed to visibilities.
+        sum of all light profile images blurred with the PSF.
 
-        If a inversion is included it is the sum of these visibilities and the inversion's reconstructed visibilities.
+        If a inversion is included it is the sum of this image and the inversion's reconstruction of the image.
         """
 
         if self.perform_inversion:
+            return self.blurred_image + self.inversion.mapped_reconstructed_data
 
-            return self.profile_visibilities + self.inversion.mapped_reconstructed_data
-
-        return self.profile_visibilities
-
-    @property
-    def grid(self) -> aa.Grid2D:
-        return self.interferometer.grid
-
-    @property
-    def galaxies(self) -> List[Galaxy]:
-        return self.plane.galaxies
+        return self.blurred_image
 
     @property
     def galaxy_model_image_dict(self) -> Dict[Galaxy, np.ndarray]:
         """
-        A dictionary which associates every galaxy in the plane with its `image`.
+        A dictionary which associates every galaxy in the plane with its `model_image`.
 
         This image is the image of the sum of:
 
-        - The images of all ordinary light profiles in that plane summed.
+        - The images of all ordinary light profiles in that plane summed and convolved with the imaging data's PSF.
         - The images of all linear objects (e.g. linear light profiles / pixelizations), where the images are solved
           for first via the inversion.
 
-        For modeling, this dictionary is used to set up the `hyper_images` that adapt certain pixelizations to the
+        For modeling, this dictionary is used to set up the `adapt_images` that adapt certain pixelizations to the
         data being fitted.
         """
-        galaxy_model_image_dict = self.plane.galaxy_image_2d_dict_from(grid=self.grid)
+
+        galaxy_blurred_image_2d_dict = self.plane.galaxy_blurred_image_2d_dict_from(
+            grid=self.grid,
+            convolver=self.dataset.convolver,
+            blurring_grid=self.dataset.blurring_grid,
+        )
 
         galaxy_linear_obj_image_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=True
         )
 
-        return {**galaxy_model_image_dict, **galaxy_linear_obj_image_dict}
+        return {**galaxy_blurred_image_2d_dict, **galaxy_linear_obj_image_dict}
 
     @property
-    def galaxy_model_visibilities_dict(self) -> Dict[Galaxy, np.ndarray]:
+    def model_images_of_galaxies_list(self) -> List:
         """
-        A dictionary which associates every galaxy in the plane with its model visibilities.
+        A list of the model images of each galaxy in the plane.
+        """
+        return list(self.galaxy_model_image_dict.values())
 
-        These visibilities are the sum of:
+    @property
+    def subtracted_images_of_galaxies_list(self) -> List[aa.Array2D]:
+        """
+        A list of the subtracted image of every galaxy.
 
-        - The visibilities of all ordinary light profiles in that plane summed and Fourier transformed to visibilities
-          space.
-        - The visibilities of all linear objects (e.g. linear light profiles / pixelizations), where the visibilities
-          are solved for first via the inversion.
+        A subtracted image of a galaxy is the data where all other galaxy images are subtracted from it, therefore
+        showing how a galaxy appears in the data in the absence of all other galaxies.
 
-        For modeling, this dictionary is used to set up the `hyper_visibilities` that adapt certain pixelizations to the
-        data being fitted.
+        This is used to visualize the contribution of each galaxy in the data.
         """
-        galaxy_model_visibilities_dict = self.plane.galaxy_visibilities_dict_from(
-            grid=self.interferometer.grid, transformer=self.interferometer.transformer
-        )
 
-        galaxy_linear_obj_data_dict = self.galaxy_linear_obj_data_dict_from(
-            use_image=False
-        )
+        subtracted_images_of_galaxies_list = []
+
+        model_images_of_galaxies_list = self.model_images_of_galaxies_list
+
+        for galaxy_index in range(len(self.galaxies)):
+            other_galaxies_model_images = [
+                model_image
+                for i, model_image in enumerate(model_images_of_galaxies_list)
+                if i != galaxy_index
+            ]
+
+            subtracted_image = self.image - sum(other_galaxies_model_images)
 
-        return {**galaxy_model_visibilities_dict, **galaxy_linear_obj_data_dict}
+            subtracted_images_of_galaxies_list.append(subtracted_image)
+
+        return subtracted_images_of_galaxies_list
 
     @property
-    def model_visibilities_of_galaxies_list(self) -> List:
+    def unmasked_blurred_image(self) -> aa.Array2D:
         """
-        A list of the model visibilities of each galaxy in the plane.
+        The blurred image of the overall fit that would be evaluated without a mask being used.
+
+        Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
+        image cannot be computed.
         """
-        return list(self.galaxy_model_visibilities_dict.values())
+        if self.plane.has(cls=LightProfileLinear):
+            exc.raise_linear_light_profile_in_unmasked()
+
+        return self.plane.unmasked_blurred_image_2d_from(
+            grid=self.grid, psf=self.dataset.psf
+        )
+
+    @property
+    def unmasked_blurred_image_of_galaxies_list(self) -> List[aa.Array2D]:
+        """
+        The blurred image of every galaxy int he plane used in this fit, that would be evaluated without a mask being
+        used.
+
+        Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
+        image cannot be computed.
+        """
+        if self.plane.has(cls=LightProfileLinear):
+            exc.raise_linear_light_profile_in_unmasked()
+
+        return self.plane.unmasked_blurred_image_2d_list_from(
+            grid=self.grid, psf=self.dataset.psf
+        )
 
     @property
     def plane_linear_light_profiles_to_light_profiles(self) -> Plane:
         """
         The `Plane` where all linear light profiles have been converted to ordinary light profiles, where their
         `intensity` values are set to the values inferred by this fit.
 
@@ -247,15 +281,15 @@
         """
         return self.model_obj_linear_light_profiles_to_light_profiles
 
     def refit_with_new_preloads(
         self,
         preloads: Preloads,
         settings_inversion: Optional[aa.SettingsInversion] = None,
-    ) -> "FitInterferometer":
+    ) -> "FitImaging":
         """
         Returns a new fit which uses the dataset, plane and other objects of this fit, but uses a different set of
         preloads input into this function.
 
         This is used when setting up the preloads objects, to concisely test how using different preloads objects
         changes the attributes of the fit.
 
@@ -266,25 +300,23 @@
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
 
         Returns
         -------
         A new fit which has used new preloads input into this function but the same dataset, plane and other settings.
         """
-        if self.profiling_dict is not None:
-            profiling_dict = {}
-        else:
-            profiling_dict = None
+        profiling_dict = {} if self.profiling_dict is not None else None
 
-        if settings_inversion is None:
-            settings_inversion = self.settings_inversion
+        settings_inversion = (
+            self.settings_inversion
+            if settings_inversion is None
+            else settings_inversion
+        )
 
-        return FitInterferometer(
-            dataset=self.interferometer,
+        return FitImaging(
+            dataset=self.dataset,
             plane=self.plane,
-            hyper_background_noise=self.hyper_background_noise,
-            use_hyper_scaling=self.use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=settings_inversion,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/interferometer/interferometer.py` & `autogalaxy-2023.7.7.1/autogalaxy/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/analysis.py` & `autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,29 +12,28 @@
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.cosmology.lensing import LensingCosmology
 from autogalaxy.cosmology.wrap import Planck15
 from autogalaxy.interferometer.model.result import ResultInterferometer
 from autogalaxy.interferometer.model.visualizer import VisualizerInterferometer
 from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.hyper.hyper_data import HyperBackgroundNoise
 from autogalaxy.plane.plane import Plane
 
 from autogalaxy import exc
 
 logger = logging.getLogger(__name__)
 
 logger.setLevel(level="INFO")
 
 
 class AnalysisInterferometer(AnalysisDataset):
     def __init__(
         self,
         dataset: aa.Interferometer,
-        hyper_dataset_result: ResultInterferometer = None,
+        adapt_result: ResultInterferometer = None,
         cosmology: LensingCosmology = Planck15(),
         settings_pixelization: aa.SettingsPixelization = None,
         settings_inversion: aa.SettingsInversion = None,
     ):
         """
         Analysis classes are used by PyAutoFit to fit a model to a dataset via a non-linear search.
 
@@ -43,123 +42,50 @@
         such as visualization, outputting results to hard-disk and storing results in a format that can be loaded after
         the model-fit is complete using PyAutoFit's database tools.
 
         This Analysis class is used for all model-fits which fit galaxies (or objects containing galaxies like a
         `Plane`) to an interferometer dataset.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. a
-        pixelization or inversion), the Cosmology used for the analysis and hyper datasets used for certain model
+        pixelization or inversion), the Cosmology used for the analysis and adapt datasets used for certain model
         classes.
 
         Parameters
         ----------
         dataset
             The interferometer dataset that the model is fitted too.
-        hyper_dataset_result
-            The hyper-model image and hyper galaxies images of a previous result in a model-fitting pipeline, which are
+        adapt_result
+            The adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
             used by certain classes for adapting the analysis to the properties of the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         settings_pixelization
             settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted, for example which linear algebra formalism is used.
         """
         super().__init__(
             dataset=dataset,
-            hyper_dataset_result=hyper_dataset_result,
+            adapt_result=adapt_result,
             cosmology=cosmology,
             settings_pixelization=settings_pixelization,
             settings_inversion=settings_inversion,
         )
 
-        if self.hyper_dataset_result is not None:
-
-            self.set_hyper_dataset(result=self.hyper_dataset_result)
-
-        else:
-
-            self.hyper_galaxy_visibilities_path_dict = None
-            self.hyper_model_visibilities = None
-
     @property
     def interferometer(self):
         return self.dataset
 
-    def set_hyper_dataset(self, result):
-        """
-        Using a the result of a previous model-fit, set the hyper-dataset for this analysis. This is used to adapt
-        aspects of the model (e.g. the pixelization, regularization scheme) to the properties of the dataset being
-        fitted.
-
-        This passes the hyper model image and hyper galaxy images of the previous fit. These represent where different
-        galaxies in the dataset are located and thus allows the fit to adapt different aspects of the model to different
-        galaxies in the data.
-
-        It also passes hyper visibilities, which are used to scale the noise of a visibility dataset.
-
-        Parameters
-        ----------
-        result
-            The result of a previous model-fit which contains the model image and model galaxy images of a fit to
-            the dataset, which set up the hyper dataset. These are used by certain classes for adapting the analysis
-            to the properties of the dataset.
-        """
-        super().set_hyper_dataset(result=result)
-
-        self.hyper_model_visibilities = result.hyper_model_visibilities
-        self.hyper_galaxy_visibilities_path_dict = (
-            result.hyper_galaxy_visibilities_path_dict
-        )
-
-    def instance_with_associated_hyper_visibilities_from(
-        self, instance: af.ModelInstance
-    ) -> af.ModelInstance:
-        """
-        Using the model visibilities that were set up as the hyper dataset, associate the galaxy images of that result
-        with the galaxies in this model fit.
-
-        Association is performed based on galaxy names, whereby if the name of a galaxy in this search matches the
-        full-path name of galaxies in the hyper dataset the galaxy image is passed.
-
-        If the galaxy collection has a different name then an association is not made.
-
-        For example, `galaxies.lens` will match with:
-            `galaxies.lens`
-        but not with:
-            `galaxies.source`
-
-        Parameters
-        ----------
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search), which has 0 or more galaxies in its tree.
-
-        Returns
-        -------
-        instance
-           The input instance with visibilities associated with galaxies where possible.
-        """
-        if self.hyper_galaxy_visibilities_path_dict is not None:
-            for galaxy_path, galaxy in instance.path_instance_tuples_for_class(Galaxy):
-                if galaxy_path in self.hyper_galaxy_visibilities_path_dict:
-                    galaxy.hyper_model_visibilities = self.hyper_model_visibilities
-                    galaxy.hyper_galaxy_visibilities = (
-                        self.hyper_galaxy_visibilities_path_dict[galaxy_path]
-                    )
-
-        return instance
-
     def modify_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
         """
         PyAutoFit calls this function immediately before the non-linear search begins, therefore it can be used to
         perform tasks using the final model parameterization.
 
-        This function checks that the hyper-dataset is consistent with previous hyper-datasets if the model-fit is
+        This function checks that the adapt-dataset is consistent with previous adapt-datasets if the model-fit is
         being resumed from a previous run, and it visualizes objects which do not change throughout the model fit
         like the dataset.
 
         Parameters
         ----------
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
@@ -168,26 +94,14 @@
             The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
             the imaging data.
         """
 
         super().modify_before_fit(paths=paths, model=model)
 
         if not paths.is_complete:
-
-            if not os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-
-                visualizer = VisualizerInterferometer(visualize_path=paths.image_path)
-
-                visualizer.visualize_interferometer(interferometer=self.interferometer)
-
-                visualizer.visualize_hyper_images(
-                    hyper_galaxy_image_path_dict=self.hyper_galaxy_image_path_dict,
-                    hyper_model_image=self.hyper_model_image,
-                )
-
             logger.info(
                 "PRELOADS - Setting up preloads, may take a few minutes for fits using an inversion."
             )
 
             self.set_preloads(paths=paths, model=model)
 
         return self
@@ -197,15 +111,15 @@
         Given an instance of the model, where the model parameters are set via a non-linear search, fit the model
         instance to the interferometer dataset.
 
         This function returns a log likelihood which is used by the non-linear search to guide the model-fit.
 
         For this analysis class, this function performs the following steps:
 
-        1) If the analysis has a hyper dataset, associated the model galaxy images of this dataset to the galaxies in
+        1) If the analysis has a adapt dataset, associated the model galaxy images of this dataset to the galaxies in
            the model instance.
 
         2) Extract attributes which model aspects of the data reductions, like scaling the background background noise.
 
         3) Extracts all galaxies from the model instance and set up a `Plane`.
 
         4) Use the `Plane` and other attributes to create a `FitInterferometer` object, which performs steps such as
@@ -243,117 +157,126 @@
             OverflowError,
         ) as e:
             raise exc.FitException from e
 
     def fit_interferometer_via_instance_from(
         self,
         instance: af.ModelInstance,
-        use_hyper_scaling: bool = True,
         preload_overwrite: Optional[Preloads] = None,
     ) -> FitInterferometer:
         """
         Given a model instance create a `FitInterferometer` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the interferometer data and compute
         the log likelihood.
 
         Parameters
         ----------
         instance
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
-        use_hyper_scaling
-            If false, the scaling of the background sky and noise are not performed irrespective of the model components
-            themselves.
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitInterferometer
             The fit of the plane to the interferometer dataset, which includes the log likelihood.
         """
-        instance = self.instance_with_associated_hyper_images_from(instance=instance)
-
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
+        instance = self.instance_with_associated_adapt_images_from(instance=instance)
 
         plane = self.plane_via_instance_from(instance=instance)
 
         return self.fit_interferometer_via_plane_from(
             plane=plane,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
         )
 
     def fit_interferometer_via_plane_from(
         self,
         plane: Plane,
-        hyper_background_noise: Optional[HyperBackgroundNoise],
-        use_hyper_scaling: bool = True,
         preload_overwrite: Optional[Preloads] = None,
     ) -> FitInterferometer:
         """
         Given a `Plane`, which the analysis constructs from a model instance, create a `FitInterferometer` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the interferometer data and compute
         the log likelihood.
 
         Parameters
         ----------
         plane
             The plane of galaxies whose model images are used to fit the interferometer data.
-        hyper_background_noise
-            A model component which scales the background noise level of the data before computing the log likelihood.
-        use_hyper_scaling
-            If false, the scaling of the background noise is not performed irrespective of the model components
-            themselves.
 
         Returns
         -------
         FitInterferometer
             The fit of the plane to the interferometer dataset, which includes the log likelihood.
         """
 
         preloads = self.preloads if preload_overwrite is None else preload_overwrite
 
         return FitInterferometer(
             dataset=self.dataset,
             plane=plane,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
         )
 
     @property
     def fit_func(self):
         return self.fit_interferometer_via_instance_from
 
+    def visualize_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
+        """
+        PyAutoFit calls this function immediately before the non-linear search begins.
+
+        It visualizes objects which do not change throughout the model fit like the dataset.
+
+        Parameters
+        ----------
+        paths
+            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
+            visualization and the pickled objects used by the aggregator output by this function.
+        model
+            The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
+            the imaging data.
+        """
+
+        if not self.should_visualize(paths=paths):
+            return
+
+        visualizer = VisualizerInterferometer(visualize_path=paths.image_path)
+
+        visualizer.visualize_interferometer(dataset=self.interferometer)
+
+        visualizer.visualize_adapt_images(
+            adapt_galaxy_image_path_dict=self.adapt_galaxy_image_path_dict,
+            adapt_model_image=self.adapt_model_image,
+        )
+
     def visualize(self, paths: af.DirectoryPaths, instance, during_analysis):
         """
         Outputs images of the maximum log likelihood model inferred by the model-fit. This function is called
         throughout the non-linear search at input intervals, and therefore provides on-the-fly visualization of how
         well the model-fit is going.
 
         The visualization performed by this function includes:
 
         - Images of the best-fit `Plane`, including the images of each of its galaxies.
 
         - Images of the best-fit `FitInterferometer`, including the model-image, residuals and chi-squared of its fit
           to the imaging data.
 
-        - The hyper-images of the model-fit showing how the hyper galaxies are used to represent different galaxies in
+        - The adapt-images of the model-fit showing how the galaxies are used to represent different galaxies in
           the dataset.
 
-        - If hyper features are used to scale the noise, a `FitInterferometer` with these features turned off may be
+        - If adapt features are used to scale the noise, a `FitInterferometer` with these features turned off may be
           output, to indicate how much these features are altering the dataset.
 
         The images output by this function are customized using the file `config/visualize/plots.ini`.
 
         Parameters
         ----------
         paths
@@ -363,29 +286,26 @@
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
         during_analysis
             If True the visualization is being performed midway through the non-linear search before it is finished,
             which may change which images are output.
         """
 
-        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+        if not self.should_visualize(paths=paths):
             return
 
-        instance = self.instance_with_associated_hyper_images_from(instance=instance)
+        instance = self.instance_with_associated_adapt_images_from(instance=instance)
         plane = self.plane_via_instance_from(instance=instance)
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
 
         fit = self.fit_interferometer_via_plane_from(
-            plane=plane, hyper_background_noise=hyper_background_noise
+            plane=plane,
         )
 
         visualizer = VisualizerInterferometer(visualize_path=paths.image_path)
-        visualizer.visualize_interferometer(interferometer=self.interferometer)
+        visualizer.visualize_interferometer(dataset=self.interferometer)
 
         plane = fit.plane_linear_light_profiles_to_light_profiles
 
         visualizer.visualize_plane(
             plane=plane, grid=fit.grid, during_analysis=during_analysis
         )
         visualizer.visualize_galaxies(
@@ -403,28 +323,19 @@
             try:
                 visualizer.visualize_inversion(
                     inversion=fit.inversion, during_analysis=during_analysis
                 )
             except IndexError:
                 pass
 
-        visualizer.visualize_hyper_images(
-            hyper_galaxy_image_path_dict=self.hyper_galaxy_image_path_dict,
-            hyper_model_image=self.hyper_model_image,
+        visualizer.visualize_adapt_images(
+            adapt_galaxy_image_path_dict=self.adapt_galaxy_image_path_dict,
+            adapt_model_image=self.adapt_model_image,
         )
 
-        if visualizer.plot_fit_no_hyper:
-            fit = self.fit_interferometer_via_plane_from(
-                plane=plane, hyper_background_noise=None, use_hyper_scaling=False
-            )
-
-            visualizer.visualize_fit_interferometer(
-                fit=fit, during_analysis=during_analysis, subfolders="fit_no_hyper"
-            )
-
     def make_result(
         self,
         samples: af.SamplesPDF,
         model: af.Collection,
         sigma=1.0,
         use_errors=True,
         use_widths=False,
@@ -437,15 +348,15 @@
 
         - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
           an instance of the maximum log likelihood model).
 
         - The non-linear search used to perform the model fit.
 
         The `ResultInterferometer` object contains a number of methods which use the above objects to create the max
-        log likelihood `Plane`, `FitInterferometer`, hyper-galaxy images,etc.
+        log likelihood `Plane`, `FitInterferometer`, adapt-galaxy images,etc.
 
         Parameters
         ----------
         samples
             A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
             run of samples of the nested sampler.
         model
@@ -460,25 +371,25 @@
             The result of fitting the model to the interferometer dataset, via a non-linear search.
         """
         return ResultInterferometer(samples=samples, model=model, analysis=self)
 
     def save_attributes_for_aggregator(self, paths: af.DirectoryPaths):
         """
          Before the model-fit begins, this routine saves attributes of the `Analysis` object to the `pickles` folder
-         such that they can be load after the analysis using PyAutoFit's database and aggregator tools.
+         such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
          For this analysis, it uses the `AnalysisDataset` object's method to output the following:
 
          - The dataset's data.
          - The dataset's noise-map.
          - The settings associated with the dataset.
          - The settings associated with the inversion.
          - The settings associated with the pixelization.
          - The Cosmology.
-         - The hyper dataset's model image and galaxy images, if used.
+         - The adapt dataset's model image and galaxy images, if used.
 
          This function also outputs attributes specific to an interferometer dataset:
 
         - Its uv-wavelengths
         - Its real space mask.
 
          It is common for these attributes to be loaded by many of the template aggregator functions given in the
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/result.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,137 @@
+import numpy as np
+from scipy.integrate import quad
+from typing import Optional, Tuple
+
 import autoarray as aa
 
-from autogalaxy.analysis.result import ResultDataset
-from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.plane.plane import Plane
-from autogalaxy.interferometer.fit_interferometer import FitInterferometer
-
-
-class ResultInterferometer(ResultDataset):
-    """
-    After the non-linear search of a fit to an interferometer dataset is complete it creates
-    this `ResultInterferometer` object, which includes:
-
-    - The samples of the non-linear search (E.g. MCMC chains, nested sampling samples) which are used to compute
-    the maximum likelihood model, posteriors and other properties.
-
-    - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
-    an instance of the maximum log likelihood model).
-
-    - The non-linear search used to perform the model fit.
-
-    This class contains a number of methods which use the above objects to create the max log likelihood `Plane`,
-    `FitInterferometer`, hyper-galaxy images,etc.
-
-    Parameters
-    ----------
-    samples
-        A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
-        run of samples of the nested sampler.
-    model
-        The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
-        the interferometer data.
-    search
-        The non-linear search used to perform this model-fit.
-
-    Returns
-    -------
-    ResultInterferometer
-        The result of fitting the model to the interferometer dataset, via a non-linear search.
-    """
+from autogalaxy.operate.image import OperateImage
+from autogalaxy.profiles.geometry_profiles import EllProfile
 
-    @property
-    def max_log_likelihood_fit(self) -> FitInterferometer:
-        """
-        An instance of a `FitInterferometer` corresponding to the maximum log likelihood model inferred by the
-        non-linear search.
+
+class LightProfile(EllProfile, OperateImage):
+    def __init__(
+        self,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        ell_comps: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 0.1,
+    ):
         """
-        hyper_background_noise = self.analysis.hyper_background_noise_via_instance_from(
-            instance=self.instance_copy
-        )
+        Abstract base class for an elliptical light-profile.
 
-        instance = self.analysis.instance_with_associated_hyper_images_from(
-            instance=self.instance_copy
-        )
+        Each light profile has an analytic equation associated with it that describes its 1D surface brightness.
 
-        plane = self.analysis.plane_via_instance_from(instance=instance)
+        Given an input grid of 1D or 2D (y,x) coordinates the light profile can be used to evaluate its surface
+        brightness in 1D or as a 2D image.
 
-        return self.analysis.fit_interferometer_via_plane_from(
-            plane=plane, hyper_background_noise=hyper_background_noise
-        )
+        Associated with a light profile is a spherical or elliptical geometry, which describes its `centre` of
+        emission and ellipticity. Geometric transformations are performed by decorators linked to the **PyAutoArray**
+        `geometry` package.
 
-    @property
-    def max_log_likelihood_plane(self) -> Plane:
+        Parameters
+        ----------
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        ell_comps
+            The first and second ellipticity components of the elliptical coordinate system (see the module
+            `autogalaxy -> convert.py` for the convention).
+        """
+        super().__init__(centre=centre, ell_comps=ell_comps)
+        self.intensity = intensity
+
+    def image_2d_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> aa.Array2D:
         """
-        An instance of a `Plane` corresponding to the maximum log likelihood model inferred by the non-linear search.
+        Returns the light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates, which may have been
+        transformed using the light profile's geometry.
+
+        If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
+        profile `centre`), this is performed automatically.
 
-        The `Plane` is computed from the `max_log_likelihood_fit`, as this ensures that all linear light profiles
-        are converted to normal light profiles with their `intensity` values updated.
+        Parameters
+        ----------
+        grid
+            The 2D (y, x) coordinates in the original reference frame of the grid.
+
+        Returns
+        -------
+        image
+            The image of the `LightProfile` evaluated at every (y,x) coordinate on the transformed grid.
         """
-        return (
-            self.max_log_likelihood_fit.model_obj_linear_light_profiles_to_light_profiles
-        )
+        raise NotImplementedError()
 
-    @property
-    def real_space_mask(self) -> aa.Mask2D:
+    def image_2d_via_radii_from(self, grid_radii: np.ndarray) -> np.ndarray:
         """
-        The real space mask used by this model-fit.
+        Returns the light profile's 2D image from a 1D grid of coordinates which are the radial distance of each
+        coordinate from the light profile `centre`.
+
+        Parameters
+        ----------
+        grid_radii
+            The radial distances from the centre of the profile, for each coordinate on the grid.
         """
-        return self.max_log_likelihood_fit.interferometer.real_space_mask
+        raise NotImplementedError()
 
-    def visibilities_for_galaxy(self, galaxy: Galaxy) -> aa.Visibilities:
+    @aa.grid_dec.grid_1d_to_structure
+    def image_1d_from(self, grid: aa.type.Grid1D2DLike) -> aa.type.Grid1D2DLike:
         """
-        Given an instance of a `Galaxy` object, return an image of the galaxy via the the maximum log likelihood fit.
+        Returns the light profile's 1D image from a grid of Cartesian coordinates, which may have been
+        transformed using the light profile's geometry.
+
+        If a 1D grid is input the image is evaluated every coordinate on the grid. If a 2D grid is input, this is
+        converted to a 1D grid by aligning with the major-axis of the light profile's elliptical geometry.
 
-        This image is extracted via the fit's `galaxy_model_image_dict`, which is necessary to make it straight
-        forward to use the image as hyper-images.
+        Internally, this function uses a 2D grid to compute the image, which is mapped to a 1D data structure on return
+        via the `grid_1d_to_structure` decorator. This avoids code repetition by ensuring that light profiles only use
+        their `image_2d_from()`  function to evaluate their image.
 
         Parameters
         ----------
-        galaxy
-            A galaxy used by the model-fit.
+        grid
+            A 1D or 2D grid of coordinates which are used to evaluate the light profile in 1D.
 
         Returns
         -------
-        ndarray or None
-            A numpy arrays giving the model image of that galaxy.
+        image
+            The 1D image of the light profile evaluated at every (x,) coordinate on the 1D transformed grid.
         """
-        return self.max_log_likelihood_fit.galaxy_model_visibilities_dict[galaxy]
+        return self.image_2d_from(grid=grid)
 
-    @property
-    def visibilities_galaxy_dict(self) -> {str: Galaxy}:
-        """
-        A dictionary associating galaxy names with model visibilities of those galaxies.
+    def luminosity_within_circle_from(self, radius: float) -> float:
         """
-        return {
-            galaxy_path: self.visibilities_for_galaxy(galaxy)
-            for galaxy_path, galaxy in self.path_galaxy_tuples
-        }
+        Integrate the light profile to compute the total luminosity within a circle of specified radius. This is
+        centred on the light profile's `centre`.
 
-    @property
-    def hyper_galaxy_visibilities_path_dict(self):
-        """
-        A dictionary associating 1D hyper_galaxies galaxy visibilities with their names.
+        The `intensity` of a light profile is in dimension units, which are given physical meaning when the light
+        profile is compared to data with physical units. The luminosity output by this function therefore is also
+        dimensionless until compared to data.
 
-        This is used for creating the hyper-dataset used by Analysis objects to adapt aspects of a model to the dataset
-        being fitted.
+        Parameters
+        ----------
+        radius
+            The radius of the circle to compute the dimensionless luminosity within.
         """
 
-        hyper_galaxy_visibilities_path_dict = {}
+        return quad(func=self.luminosity_integral, a=0.0, b=radius)[0]
 
-        for path, galaxy in self.path_galaxy_tuples:
-            hyper_galaxy_visibilities_path_dict[path] = self.visibilities_galaxy_dict[
-                path
-            ]
-
-        return hyper_galaxy_visibilities_path_dict
-
-    @property
-    def hyper_model_visibilities(self) -> aa.Visibilities:
+    def luminosity_integral(self, x: np.ndarray) -> np.ndarray:
         """
-        The hyper model visibilities used by AnalysisInterferometer objects to adapt aspects of a model to the dataset
-        being fitted.
+        Routine to integrate the luminosity of an elliptical light profile.
+
+        The axis ratio is set to 1.0 for computing the luminosity within a circle
 
-        The hyper model visibilities are the sum of the hyper galaxy visibilities of every individual galaxy.
+        Parameters
+        ----------
+        x
+            The 1D (x) radial coordinates where the luminosity integral is evaluated.
         """
-        hyper_model_visibilities = aa.Visibilities.zeros(
-            shape_slim=(self.max_log_likelihood_fit.visibilities.shape_slim,)
-        )
+        return 2 * np.pi * x * self.image_2d_via_radii_from(x)
 
-        for path, galaxy in self.path_galaxy_tuples:
-            hyper_model_visibilities += self.hyper_galaxy_visibilities_path_dict[path]
+    @property
+    def half_light_radius(self) -> float:
+        if hasattr(self, "effective_radius"):
+            return self.effective_radius
 
-        return hyper_model_visibilities
+    @property
+    def _intensity(self):
+        return self.intensity
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/interferometer/model/visualizer.py` & `autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/visualizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class VisualizerInterferometer(Visualizer):
     def visualize_fit_interferometer(
         self,
         fit: FitInterferometer,
         during_analysis: bool,
-        subfolders: str = "fit_interferometer",
+        subfolders: str = "fit_dataset",
     ):
         """
         Visualizes a `FitInterferometer` object, which fits an interferometer dataset.
 
         Images are output to the `image` folder of the `visualize_path` in a subfolder called `fit`. When
         used with a non-linear search the `visualize_path` points to the search's results folder and this function
         visualizes the maximum log likelihood `FitInterferometer` inferred by the search so far.
@@ -42,76 +42,86 @@
 
         def should_plot(name):
             return plot_setting(section=["fit", "fit_interferometer"], name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=subfolders)
         mat_plot_2d = self.mat_plot_2d_from(subfolders=subfolders)
 
-        fit_interferometer_plotter = FitInterferometerPlotter(
+        fit_plotter = FitInterferometerPlotter(
             fit=fit,
             include_2d=self.include_2d,
             mat_plot_1d=mat_plot_1d,
             mat_plot_2d=mat_plot_2d,
         )
 
         if should_plot("subplot_fit"):
-            fit_interferometer_plotter.subplot_fit_interferometer()
-            fit_interferometer_plotter.subplot_fit_real_space()
+            fit_plotter.subplot_fit()
 
-        fit_interferometer_plotter.figures_2d(
-            visibilities=should_plot("data"),
+        if should_plot("subplot_fit_real_space"):
+            fit_plotter.subplot_fit_real_space()
+
+        fit_plotter.figures_2d(
+            data=should_plot("data"),
             noise_map=should_plot("noise_map"),
             signal_to_noise_map=should_plot("signal_to_noise_map"),
-            model_visibilities=should_plot("model_data"),
+            model_data=should_plot("model_data"),
             residual_map_real=should_plot("residual_map"),
             residual_map_imag=should_plot("residual_map"),
             chi_squared_map_real=should_plot("chi_squared_map"),
             chi_squared_map_imag=should_plot("chi_squared_map"),
             normalized_residual_map_real=should_plot("normalized_residual_map"),
             normalized_residual_map_imag=should_plot("normalized_residual_map"),
             dirty_image=should_plot("dirty_image"),
             dirty_noise_map=should_plot("dirty_noise_map"),
             dirty_signal_to_noise_map=should_plot("dirty_signal_to_noise_map"),
             dirty_residual_map=should_plot("residual_map"),
             dirty_normalized_residual_map=should_plot("normalized_residual_map"),
             dirty_chi_squared_map=should_plot("chi_squared_map"),
         )
 
-        if not during_analysis:
-
-            if should_plot("all_at_end_png"):
-
-                fit_interferometer_plotter.figures_2d(
-                    visibilities=True,
-                    noise_map=True,
-                    signal_to_noise_map=True,
-                    model_visibilities=True,
-                    residual_map_real=True,
-                    residual_map_imag=True,
-                    chi_squared_map_real=True,
-                    chi_squared_map_imag=True,
-                    normalized_residual_map_real=True,
-                    normalized_residual_map_imag=True,
-                )
-
-            if should_plot("all_at_end_fits"):
-
-                mat_plot_2d = self.mat_plot_2d_from(
-                    subfolders=path.join("fit_interferometer", "fits"), format="fits"
-                )
-
-                fit_interferometer_plotter = FitInterferometerPlotter(
-                    fit=fit, include_2d=self.include_2d, mat_plot_2d=mat_plot_2d
-                )
-
-                fit_interferometer_plotter.figures_2d(
-                    visibilities=True,
-                    noise_map=True,
-                    signal_to_noise_map=True,
-                    model_visibilities=True,
-                    residual_map_real=True,
-                    residual_map_imag=True,
-                    chi_squared_map_real=True,
-                    chi_squared_map_imag=True,
-                    normalized_residual_map_real=True,
-                    normalized_residual_map_imag=True,
-                )
+        if not during_analysis and should_plot("all_at_end_png"):
+            mat_plot_1d = self.mat_plot_1d_from(subfolders=path.join(subfolders, "end"))
+            mat_plot_2d = self.mat_plot_2d_from(subfolders=path.join(subfolders, "end"))
+
+            fit_plotter = FitInterferometerPlotter(
+                fit=fit,
+                include_2d=self.include_2d,
+                mat_plot_1d=mat_plot_1d,
+                mat_plot_2d=mat_plot_2d,
+            )
+
+            fit_plotter.figures_2d(
+                data=True,
+                noise_map=True,
+                signal_to_noise_map=True,
+                model_data=True,
+                residual_map_real=True,
+                residual_map_imag=True,
+                chi_squared_map_real=True,
+                chi_squared_map_imag=True,
+                normalized_residual_map_real=True,
+                normalized_residual_map_imag=True,
+                dirty_image=True,
+                dirty_noise_map=True,
+                dirty_signal_to_noise_map=True,
+                dirty_residual_map=True,
+                dirty_normalized_residual_map=True,
+                dirty_chi_squared_map=True,
+            )
+
+        if not during_analysis and should_plot("all_at_end_fits"):
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join("fit_dataset", "fits"), format="fits"
+            )
+
+            fit_plotter = FitInterferometerPlotter(
+                fit=fit, include_2d=self.include_2d, mat_plot_2d=mat_plot_2d
+            )
+
+            fit_plotter.figures_2d(
+                dirty_image=True,
+                dirty_noise_map=True,
+                dirty_signal_to_noise_map=True,
+                dirty_residual_map=True,
+                dirty_normalized_residual_map=True,
+                dirty_chi_squared_map=True,
+            )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/interferometer/plot/fit_interferometer_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/fit_interferometer_plotters.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,23 +81,21 @@
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
             residuals_symmetric_cmap=residuals_symmetric_cmap,
         )
 
         self.figures_2d = self._fit_interferometer_meta_plotter.figures_2d
         self.subplot = self._fit_interferometer_meta_plotter.subplot
-        self.subplot_fit_interferometer = (
-            self._fit_interferometer_meta_plotter.subplot_fit_interferometer
-        )
+        #  self.subplot_fit = self._fit_interferometer_meta_plotter.subplot_fit
         self.subplot_fit_dirty_images = (
             self._fit_interferometer_meta_plotter.subplot_fit_dirty_images
         )
 
     def get_visuals_2d_real_space(self) -> Visuals2D:
-        return self.get_2d.via_mask_from(mask=self.fit.interferometer.real_space_mask)
+        return self.get_2d.via_mask_from(mask=self.fit.dataset.real_space_mask)
 
     @property
     def plane(self) -> Plane:
         return self.fit.plane_linear_light_profiles_to_light_profiles
 
     def plane_plotter_from(self, plane: Plane) -> PlanePlotter:
         """
@@ -106,15 +104,15 @@
         Returns
         -------
         plane
             The plane used to make the `PlanePlotter`.
         """
         return PlanePlotter(
             plane=plane,
-            grid=self.fit.interferometer.grid,
+            grid=self.fit.dataset.grid,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.get_visuals_2d_real_space(),
             include_2d=self.include_2d,
         )
 
     @property
     def inversion_plotter(self) -> aplt.InversionPlotter:
@@ -129,31 +127,75 @@
         return aplt.InversionPlotter(
             inversion=self.fit.inversion,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.get_visuals_2d_real_space(),
             include_2d=self.include_2d,
         )
 
+    def subplot_fit(self):
+        """
+        Standard subplot of the attributes of the plotter's `FitImaging` object.
+        """
+
+        self.open_subplot_figure(number_subplots=9)
+
+        self.figures_2d(amplitudes_vs_uv_distances=True)
+
+        self.mat_plot_1d.subplot_index = 2
+        self.mat_plot_2d.subplot_index = 2
+
+        self.figures_2d(dirty_image=True)
+        self.figures_2d(dirty_signal_to_noise_map=True)
+
+        self.mat_plot_1d.subplot_index = 4
+        self.mat_plot_2d.subplot_index = 4
+
+        self.figures_2d(dirty_model_image=True)
+
+        self.mat_plot_1d.subplot_index = 5
+        self.mat_plot_2d.subplot_index = 5
+
+        self.figures_2d(normalized_residual_map_real=True)
+        self.figures_2d(normalized_residual_map_imag=True)
+
+        self.mat_plot_1d.subplot_index = 7
+        self.mat_plot_2d.subplot_index = 7
+
+        self.figures_2d(dirty_normalized_residual_map=True)
+
+        self.mat_plot_2d.cmap.kwargs["vmin"] = -1.0
+        self.mat_plot_2d.cmap.kwargs["vmax"] = 1.0
+
+        self.set_title(label="Normalized Residual Map (1 sigma)")
+        self.figures_2d(dirty_normalized_residual_map=True)
+        self.set_title(label=None)
+
+        self.mat_plot_2d.cmap.kwargs.pop("vmin")
+        self.mat_plot_2d.cmap.kwargs.pop("vmax")
+
+        self.figures_2d(dirty_chi_squared_map=True)
+
+        self.mat_plot_2d.output.subplot_to_figure(auto_filename="subplot_fit")
+        self.close_subplot_figure()
+
     def subplot_fit_real_space(self):
         """
         Standard subplot of the real-space attributes of the plotter's `FitInterferometer` object.
 
         Depending on whether `LightProfile`'s or an `Inversion` are used to represent galaxies in the `Plane`, different
         methods are called to create these real-space images.
         """
         if self.fit.inversion is None:
-
             plane_plotter = self.plane_plotter_from(plane=self.plane)
 
             plane_plotter.subplot(
                 image=True, plane_image=True, auto_filename="subplot_fit_real_space"
             )
 
         elif self.fit.inversion is not None:
-
             self.open_subplot_figure(number_subplots=6)
 
             mapper_index = 0
 
             self.inversion_plotter.figures_2d_of_pixelization(
                 pixelization_index=mapper_index, reconstructed_image=True
             )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/operate/deflections.py` & `autogalaxy-2023.7.7.1/autogalaxy/operate/deflections.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 def grid_scaled_2d_for_marching_squares_from(
     grid_pixels_2d: aa.Grid2D,
     shape_native: Tuple[int, int],
     mask: aa.Mask2D,
 ) -> aa.Grid2DIrregular:
-
     pixel_scales = mask.pixel_scales
     sub_size = mask.sub_size
     origin = mask.origin
 
     grid_scaled_1d = aa.util.geometry.grid_scaled_2d_slim_from(
         grid_pixels_2d_slim=grid_pixels_2d,
         shape_native=shape_native,
@@ -53,15 +52,14 @@
 
 
 def evaluation_grid(func):
     @wraps(func)
     def wrapper(
         lensing_obj, grid, pixel_scale: Union[Tuple[float, float], float] = 0.05
     ):
-
         if hasattr(grid, "is_evaluation_grid"):
             if grid.is_evaluation_grid:
                 return func(lensing_obj, grid, pixel_scale)
 
         pixel_scale_ratio = grid.pixel_scale / pixel_scale
 
         zoom_shape_native = grid.mask.zoom_shape_native
@@ -164,15 +162,15 @@
 
         det_jacobian = jacobian[0][0] * jacobian[1][1] - jacobian[0][1] * jacobian[1][0]
 
         return aa.Array2D(values=1 / det_jacobian, mask=grid.mask)
 
     def hessian_from(self, grid, buffer: float = 0.01, deflections_func=None) -> Tuple:
         """
-        Returns the Hessian of the lensing object, where the Hessian is the second partial derivatives of the the
+        Returns the Hessian of the lensing object, where the Hessian is the second partial derivatives of the
         potential (see equation 55 https://www.tau.ac.il/~lab3/MICROLENSING/JeruLect.pdf):
 
         `hessian_{i,j} = d^2 / dtheta_i dtheta_j`
 
         The Hessian is computed by evaluating the 2D deflection angles around every (y,x) coordinate on the input 2D
         grid map in four directions (positive y, negative y, positive x, negative x), exploiting how the deflection
         angles are the derivative of the potential.
@@ -345,15 +343,14 @@
 
         if len(tangential_critical_curve_indices_list) == 0:
             return []
 
         tangential_critical_curve_list = []
 
         for tangential_critical_curve_indices in tangential_critical_curve_indices_list:
-
             curve = grid_scaled_2d_for_marching_squares_from(
                 grid_pixels_2d=tangential_critical_curve_indices,
                 shape_native=tangential_eigen_values.sub_shape_native,
                 mask=grid.mask,
             )
 
             tangential_critical_curve_list.append(curve)
@@ -390,15 +387,14 @@
 
         if len(radial_critical_curve_indices_list) == 0:
             return []
 
         radial_critical_curve_list = []
 
         for radial_critical_curve_indices in radial_critical_curve_indices_list:
-
             curve = grid_scaled_2d_for_marching_squares_from(
                 grid_pixels_2d=radial_critical_curve_indices,
                 shape_native=radial_eigen_values.sub_shape_native,
                 mask=grid.mask,
             )
 
             radial_critical_curve_list.append(curve)
@@ -433,15 +429,14 @@
         tangential_critical_curve_list = self.tangential_critical_curve_list_from(
             grid=grid, pixel_scale=pixel_scale
         )
 
         tangential_caustic_list = []
 
         for tangential_critical_curve in tangential_critical_curve_list:
-
             deflections_critical_curve = self.deflections_yx_2d_from(
                 grid=tangential_critical_curve
             )
 
             tangential_caustic_list.append(
                 tangential_critical_curve - deflections_critical_curve
             )
@@ -476,27 +471,55 @@
         radial_critical_curve_list = self.radial_critical_curve_list_from(
             grid=grid, pixel_scale=pixel_scale
         )
 
         radial_caustic_list = []
 
         for radial_critical_curve in radial_critical_curve_list:
-
             deflections_critical_curve = self.deflections_yx_2d_from(
                 grid=radial_critical_curve
             )
 
             radial_caustic_list.append(
                 radial_critical_curve - deflections_critical_curve
             )
 
         return radial_caustic_list
 
     @evaluation_grid
-    def area_within_tangential_critical_curve_list_from(
+    def radial_critical_curve_area_list_from(
+        self, grid, pixel_scale: Union[Tuple[float, float], float]
+    ) -> List[float]:
+        """
+        Returns the surface area within each radial critical curve as a list, the calculation of which is described in
+        the function `radial_critical_curve_list_from()`.
+
+        The area is computed via a line integral.
+
+        Due to the use of a marching squares algorithm to estimate the critical curve, this function can only use the
+        Jacobian and a uniform 2D grid.
+
+
+        Parameters
+        ----------
+        grid
+            The 2D grid of (y,x) arc-second coordinates the deflection angles used to calculate the radial critical
+            curve are computed on.
+        pixel_scale
+            If input, the `evaluation_grid` decorator creates the 2D grid at this resolution, therefore enabling the
+            caustic to be computed more accurately using a higher resolution grid.
+        """
+        radial_critical_curve_list = self.radial_critical_curve_list_from(
+            grid=grid, pixel_scale=pixel_scale
+        )
+
+        return self.area_within_curve_list_from(curve_list=radial_critical_curve_list)
+
+    @evaluation_grid
+    def tangential_critical_curve_area_list_from(
         self, grid, pixel_scale: Union[Tuple[float, float], float] = 0.05
     ) -> List[float]:
         """
         Returns the surface area within each tangential critical curve as a list, the calculation of which is
         described in the function `tangential_critical_curve_list_from()`.
 
         The area is computed via a line integral.
@@ -513,18 +536,24 @@
             If input, the `evaluation_grid` decorator creates the 2D grid at this resolution, therefore enabling the
             caustic to be computed more accurately using a higher resolution grid.
         """
         tangential_critical_curve_list = self.tangential_critical_curve_list_from(
             grid=grid, pixel_scale=pixel_scale
         )
 
-        area_within_each_curve_list = []
+        return self.area_within_curve_list_from(
+            curve_list=tangential_critical_curve_list
+        )
 
-        for curve in tangential_critical_curve_list:
+    def area_within_curve_list_from(
+        self, curve_list: List[aa.Grid2DIrregular]
+    ) -> List[float]:
+        area_within_each_curve_list = []
 
+        for curve in curve_list:
             x, y = curve[:, 0], curve[:, 1]
             area = np.abs(0.5 * np.sum(y[:-1] * np.diff(x) - x[:-1] * np.diff(y)))
             area_within_each_curve_list.append(area)
 
         return area_within_each_curve_list
 
     @evaluation_grid
@@ -537,30 +566,30 @@
         Each Einstein radius is defined as the radius of the circle which contains the same area as the area within
         each tangential critical curve.
 
         This definition is sometimes referred to as the "effective Einstein radius" in the literature and is commonly
         adopted in studies, for example the SLACS series of papers.
 
         The calculation of the tangential critical curves and their areas is described in the functions
-         `tangential_critical_curve_list_from()` and `area_within_tangential_critical_curve_list_from()`.
+         `tangential_critical_curve_list_from()` and `tangential_critical_curve_area_list_from()`.
 
         Due to the use of a marching squares algorithm to estimate the critical curve, this function can only use the
         Jacobian and a uniform 2D grid.
 
         Parameters
         ----------
         grid
             The 2D grid of (y,x) arc-second coordinates the deflection angles used to calculate the tangential critical
             curve are computed on.
         pixel_scale
             If input, the `evaluation_grid` decorator creates the 2D grid at this resolution, therefore enabling the
             caustic to be computed more accurately using a higher resolution grid.
         """
         try:
-            area_list = self.area_within_tangential_critical_curve_list_from(
+            area_list = self.tangential_critical_curve_area_list_from(
                 grid=grid, pixel_scale=pixel_scale
             )
             return [np.sqrt(area / np.pi) for area in area_list]
         except TypeError:
             raise TypeError("The grid input was unable to estimate the Einstein Radius")
 
     @evaluation_grid
@@ -576,15 +605,15 @@
         This definition is sometimes referred to as the "effective Einstein radius" in the literature and is commonly
         adopted in studies, for example the SLACS series of papers.
 
         If there are multiple tangential critical curves (e.g. because the mass distribution is complex) this function
         raises an error, and the function `einstein_radius_list_from()` should be used instead.
 
         The calculation of the tangential critical curves and their areas is described in the functions
-         `tangential_critical_curve_list_from()` and `area_within_tangential_critical_curve_list_from()`.
+         `tangential_critical_curve_list_from()` and `tangential_critical_curve_area_list_from()`.
 
         Due to the use of a marching squares algorithm to estimate the critical curve, this function can only use the
         Jacobian and a uniform 2D grid.
 
         Parameters
         ----------
         grid
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/operate/image.py` & `autogalaxy-2023.7.7.1/autogalaxy/operate/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,30 +32,26 @@
     def _blurred_image_2d_from(
         self,
         image_2d: aa.Array2D,
         blurring_image_2d: aa.Array2D,
         psf: Optional[aa.Kernel2D],
         convolver: aa.Convolver,
     ) -> aa.Array2D:
-
         if psf is not None:
-
             return psf.convolved_array_with_mask_from(
                 array=image_2d.binned.native + blurring_image_2d.binned.native,
                 mask=image_2d.mask,
             )
 
         elif convolver is not None:
-
             return convolver.convolve_image(
                 image=image_2d, blurring_image=blurring_image_2d
             )
 
         else:
-
             raise exc.OperateException(
                 "A PSF or Convolver was not passed to the `blurred_image_2d_list_from()` function."
             )
 
     def blurred_image_2d_from(
         self,
         grid: aa.Grid2D,
@@ -258,15 +254,14 @@
         blurring_image_2d_not_operated_list = self.image_2d_list_from(
             grid=blurring_grid, operated_only=False
         )
 
         blurred_image_2d_list = []
 
         for i in range(len(image_2d_operated_list)):
-
             image_2d_not_operated = image_2d_not_operated_list[i]
             blurring_image_2d_not_operated = blurring_image_2d_not_operated_list[i]
 
             blurred_image_2d = self._blurred_image_2d_from(
                 image_2d=image_2d_not_operated,
                 blurring_image_2d=blurring_image_2d_not_operated,
                 psf=psf,
@@ -306,15 +301,14 @@
         padded_grid = grid.padded_grid_from(kernel_shape_native=psf.shape_native)
 
         padded_image_1d_list = self.image_2d_list_from(grid=padded_grid)
 
         unmasked_blurred_image_list = []
 
         for padded_image_1d in padded_image_1d_list:
-
             unmasked_blurred_array_2d = padded_grid.mask.unmasked_blurred_array_from(
                 padded_array=padded_image_1d, psf=psf, image_shape=grid.mask.shape
             )
 
             unmasked_blurred_image_list.append(unmasked_blurred_array_2d)
 
         return unmasked_blurred_image_list
@@ -346,15 +340,14 @@
             in the uv-plane.
         """
         image_2d_list = self.image_2d_list_from(grid=grid)
 
         visibilities_list = []
 
         for image_2d in image_2d_list:
-
             if not np.any(image_2d):
                 visibilities = aa.Visibilities.zeros(
                     shape_slim=(transformer.uv_wavelengths.shape[0],)
                 )
             else:
                 visibilities = transformer.visibilities_from(image=image_2d.binned)
 
@@ -414,15 +407,14 @@
         galaxy_image_2d_operated_dict = self.galaxy_image_2d_dict_from(
             grid=grid, operated_only=True
         )
 
         galaxy_blurred_image_2d_dict = {}
 
         for galaxy_key in galaxy_image_2d_not_operated_dict.keys():
-
             image_2d_not_operated = galaxy_image_2d_not_operated_dict[galaxy_key]
             blurring_image_2d_not_operated = galaxy_blurring_image_2d_not_operated_dict[
                 galaxy_key
             ]
 
             blurred_image_2d = convolver.convolve_image(
                 image=image_2d_not_operated.binned,
@@ -465,22 +457,20 @@
         """
 
         galaxy_image_2d_dict = self.galaxy_image_2d_dict_from(grid=grid)
 
         galaxy_visibilities_dict = {}
 
         for galaxy_key in galaxy_image_2d_dict.keys():
-
             image_2d = galaxy_image_2d_dict[galaxy_key]
 
             if not np.any(image_2d):
                 visibilities = aa.Visibilities.zeros(
                     shape_slim=(transformer.uv_wavelengths.shape[0],)
                 )
 
             else:
-
                 visibilities = transformer.visibilities_from(image=image_2d.binned)
 
             galaxy_visibilities_dict[galaxy_key] = visibilities
 
         return galaxy_visibilities_dict
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plane/__init__.py` & `autogalaxy-2023.7.7.1/autogalaxy/plane/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plane/plot/plane_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/plane/plot/plane_plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         """
 
         from autogalaxy.profiles.light.linear import (
             LightProfileLinear,
         )
 
         if plane.has(cls=LightProfileLinear):
-
             raise exc.raise_linear_light_profile_in_plot(
                 plotter_type=self.__class__.__name__, model_obj="Plane"
             )
 
         super().__init__(
             mat_plot_2d=mat_plot_2d,
             include_2d=include_2d,
@@ -127,15 +126,15 @@
         plane_image: bool = False,
         plane_grid: bool = False,
         convergence: bool = False,
         potential: bool = False,
         deflections_y: bool = False,
         deflections_x: bool = False,
         magnification: bool = False,
-        contribution_map: bool = False,
+        zoom_to_brightest: bool = True,
         title_suffix: str = "",
         filename_suffix: str = "",
     ):
         """
         Plots the individual attributes of the plotter's `Plane` object in 2D, which are computed via the plotter's 2D
         grid object.
 
@@ -156,44 +155,57 @@
             Whether to make a 2D plot (via `imshow`) of the potential.
         deflections_y
             Whether to make a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
             Whether to make a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
             Whether to make a 2D plot (via `imshow`) of the magnification.
-        contribution_map
-            Whether to make a 2D plot (via `imshow`) of the contribution map.
+        zoom_to_brightest
+            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
+            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
         title_suffix
             Add a suffix to the end of the matplotlib title label.
         filename_suffix
             Add a suffix to the end of the filename the plot is saved to hard-disk using.
         """
         if image:
-
             self.mat_plot_2d.plot_array(
                 array=self.plane.image_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Image{title_suffix}", filename=f"image_2d{filename_suffix}"
                 ),
             )
 
         if plane_image:
+            import numpy as np
+
+            # print(self.plane.galaxies[0].bulge)
+            # print(self.plane.galaxies[0].bulge.intensity)
+            #
+            # print(self.plane.plane_image_2d_from(
+            #         grid=self.grid, zoom_to_brightest=zoom_to_brightest
+            #     ))
+            # print(np.max(self.plane.plane_image_2d_from(
+            #         grid=self.grid, zoom_to_brightest=zoom_to_brightest
+            #     )))
+            # www
 
             self.mat_plot_2d.plot_array(
-                array=self.plane.plane_image_2d_from(grid=self.grid).array,
+                array=self.plane.plane_image_2d_from(
+                    grid=self.grid, zoom_to_brightest=zoom_to_brightest
+                ),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Plane Image{title_suffix}",
                     filename=f"plane_image{filename_suffix}",
                 ),
             )
 
         if plane_grid:
-
             self.mat_plot_2d.plot_grid(
                 grid=self.grid,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Plane Grid2D{title_suffix}",
                     filename=f"plane_grid{filename_suffix}",
                 ),
@@ -203,24 +215,14 @@
             convergence=convergence,
             potential=potential,
             deflections_y=deflections_y,
             deflections_x=deflections_x,
             magnification=magnification,
         )
 
-        if contribution_map:
-
-            self.mat_plot_2d.plot_array(
-                array=self.plane.contribution_map,
-                visuals_2d=self.get_visuals_2d(),
-                auto_labels=aplt.AutoLabels(
-                    title="Contribution Map", filename="contribution_map_2d"
-                ),
-            )
-
     def galaxy_indexes_from(self, galaxy_index: Optional[int]) -> List[int]:
         """
         Returns a list of all indexes of the galaxys in the fit, which is iterated over in figures that plot
         individual figures of each galaxy in a plane.
 
         Parameters
         ----------
@@ -253,19 +255,17 @@
             unlensed light).
         galaxy_index
             If input, plots for only a single galaxy based on its index in the plane are created.
         """
         galaxy_indexes = self.galaxy_indexes_from(galaxy_index=galaxy_index)
 
         for galaxy_index in galaxy_indexes:
-
             galaxy_plotter = self.galaxy_plotter_from(galaxy_index=galaxy_index)
 
             if image:
-
                 galaxy_plotter.figures_2d(
                     image=True,
                     title_suffix=f" Of Galaxy {galaxy_index}",
                     filename_suffix=f"_of_galaxy_{galaxy_index}",
                 )
 
     def subplot(
@@ -274,15 +274,14 @@
         plane_image: bool = False,
         plane_grid: bool = False,
         convergence: bool = False,
         potential: bool = False,
         deflections_y: bool = False,
         deflections_x: bool = False,
         magnification: bool = False,
-        contribution_map: bool = False,
         auto_filename: str = "subplot_plane",
     ):
         """
         Plots the individual attributes of the plotter's `Plane` object in 2D on a subplot, which are computed via the
         plotter's 2D grid object.
 
         The API is such that every plottable attribute of the `Plane` object is an input parameter of type bool of
@@ -302,29 +301,26 @@
             Whether or not to  include a 2D plot (via `imshow`) of the potential.
         deflections_y
             Whether or not to  include a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
             Whether or not to  include a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
             Whether or not to  include a 2D plot (via `imshow`) of the magnification.
-        contribution_map
-            Whether or not to  include a 2D plot (via `imshow`) of the contribution map.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
         self._subplot_custom_plot(
             image=image,
             plane_image=plane_image,
             plane_grid=plane_grid,
             convergence=convergence,
             potential=potential,
             deflections_y=deflections_y,
             deflections_x=deflections_x,
             magnification=magnification,
-            contribution_map=contribution_map,
             auto_labels=aplt.AutoLabels(filename=auto_filename),
         )
 
     def subplot_plane(self):
         """
         Standard subplot of the attributes of the plotter's `Plane` object.
         """
@@ -343,15 +339,14 @@
         For example, for a 2 galaxy `Plane`, this creates a subplot with 2 panels, one for each galaxy.
         """
         number_subplots = len(self.plane.galaxies)
 
         self.open_subplot_figure(number_subplots=number_subplots)
 
         for galaxy_index in range(0, len(self.plane.galaxies)):
-
             galaxy_plotter = self.galaxy_plotter_from(galaxy_index=galaxy_index)
             galaxy_plotter.figures_2d(
                 image=True, title_suffix=f" Of Plane {galaxy_index}"
             )
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename=f"subplot_galaxy_images"
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plane/to_inversion.py` & `autogalaxy-2023.7.7.1/autogalaxy/plane/to_inversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,16 @@
         noise_map: Optional[Union[aa.Array2D, aa.VisibilitiesNoiseMap]] = None,
         w_tilde: Optional[Union[aa.WTildeImaging, aa.WTildeInterferometer]] = None,
         settings_pixelization=aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads=Preloads(),
         profiling_dict: Optional[Dict] = None,
     ):
-
         if dataset is not None:
-
             if dataset.noise_covariance_matrix is not None:
-
                 raise aa.exc.InversionException(
                     """
                     You cannot perform an inversion (e.g. use a linear light profile or pixelization) 
                     if the dataset has a `noise_covariance_matrix`.
                     
                     This is because the linear algebra implementation is only valid under the assumption 
                     of independent gaussian noise.
@@ -62,26 +59,24 @@
     ) -> Dict[LightProfileLinearObjFuncList, Galaxy]:
         raise NotImplementedError
 
     @cached_property
     def lp_linear_func_list_galaxy_dict(
         self,
     ) -> Dict[LightProfileLinearObjFuncList, Galaxy]:
-
         raise NotImplementedError
 
     @cached_property
     def mapper_galaxy_dict(self):
         raise NotImplementedError
 
     @cached_property
     def linear_obj_galaxy_dict(
         self,
     ) -> Dict[Union[LightProfileLinearObjFuncList, aa.AbstractMapper], Galaxy]:
-
         lp_linear_func_galaxy_dict = self.lp_linear_func_list_galaxy_dict
 
         mapper_galaxy_dict = self.mapper_galaxy_dict
 
         return {**lp_linear_func_galaxy_dict, **mapper_galaxy_dict}
 
     @cached_property
@@ -105,15 +100,14 @@
         blurring_grid: Optional[aa.type.Grid2DLike] = None,
         grid_pixelization: Optional[aa.type.Grid2DLike] = None,
         settings_pixelization=aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads=aa.Preloads(),
         profiling_dict: Optional[Dict] = None,
     ):
-
         self.plane = plane
 
         super().__init__(
             dataset=dataset,
             data=data,
             noise_map=noise_map,
             w_tilde=w_tilde,
@@ -143,36 +137,33 @@
             self.grid_pixelization = dataset.grid_pixelization
         else:
             self.grid_pixelization = None
 
     def cls_light_profile_func_list_galaxy_dict_from(
         self, cls: Type
     ) -> Dict[LightProfileLinearObjFuncList, Galaxy]:
-
         if not self.plane.has(cls=cls):
             return {}
 
         lp_linear_func_galaxy_dict = {}
 
         for galaxy in self.plane.galaxies:
             if galaxy.has(cls=cls):
                 for light_profile in galaxy.cls_list_from(cls=cls):
-
                     if isinstance(light_profile, LightProfileLinear):
                         light_profile_list = [light_profile]
                     else:
                         light_profile_list = light_profile.light_profile_list
                         light_profile_list = [
                             light_profile
                             for light_profile in light_profile_list
                             if isinstance(light_profile, LightProfileLinear)
                         ]
 
                     if len(light_profile_list) > 0:
-
                         lp_linear_func = LightProfileLinearObjFuncList(
                             grid=self.grid,
                             blurring_grid=self.blurring_grid,
                             convolver=self.dataset.convolver,
                             light_profile_list=light_profile_list,
                             regularization=light_profile.regularization,
                         )
@@ -181,15 +172,14 @@
 
         return lp_linear_func_galaxy_dict
 
     @cached_property
     def lp_linear_func_list_galaxy_dict(
         self,
     ) -> Dict[LightProfileLinearObjFuncList, Galaxy]:
-
         lp_linear_light_profile_func_list_galaxy_dict = (
             self.cls_light_profile_func_list_galaxy_dict_from(cls=LightProfileLinear)
         )
 
         lp_basis_func_list_galaxy_dict = (
             self.cls_light_profile_func_list_galaxy_dict_from(cls=Basis)
         )
@@ -199,86 +189,81 @@
             **lp_basis_func_list_galaxy_dict,
         }
 
     @cached_property
     def sparse_image_plane_grid_list(
         self,
     ) -> Optional[List[aa.Grid2DSparse]]:
-
         if not self.plane.has(cls=aa.Pixelization):
             return None
 
         return [
             pixelization.mesh.image_plane_mesh_grid_from(
                 image_plane_data_grid=self.grid_pixelization,
-                hyper_data=hyper_galaxy_image,
+                adapt_data=adapt_galaxy_image,
                 settings=self.settings_pixelization,
             )
-            for pixelization, hyper_galaxy_image in zip(
+            for pixelization, adapt_galaxy_image in zip(
                 self.plane.cls_list_from(cls=aa.Pixelization),
-                self.plane.hyper_galaxies_with_pixelization_image_list,
+                self.plane.adapt_galaxies_with_pixelization_image_list,
             )
         ]
 
     def mapper_from(
         self,
         mesh: aa.AbstractMesh,
         regularization: aa.AbstractRegularization,
         source_plane_mesh_grid: aa.Grid2DSparse,
-        hyper_galaxy_image: aa.Array2D,
+        adapt_galaxy_image: aa.Array2D,
         image_plane_mesh_grid: aa.Grid2DSparse = None,
     ) -> aa.AbstractMapper:
-
         mapper_grids = mesh.mapper_grids_from(
             source_plane_data_grid=self.grid_pixelization,
             source_plane_mesh_grid=source_plane_mesh_grid,
             image_plane_mesh_grid=image_plane_mesh_grid,
-            hyper_data=hyper_galaxy_image,
+            adapt_data=adapt_galaxy_image,
             settings=self.settings_pixelization,
             preloads=self.preloads,
             profiling_dict=self.plane.profiling_dict,
         )
 
         return mapper_from(mapper_grids=mapper_grids, regularization=regularization)
 
     @cached_property
     def mapper_galaxy_dict(self) -> Dict[aa.AbstractMapper, Galaxy]:
-
         if not self.plane.has(cls=aa.Pixelization):
             return {}
 
         sparse_grid_list = self.sparse_image_plane_grid_list
 
         mapper_galaxy_dict = {}
 
         pixelization_list = self.plane.cls_list_from(cls=aa.Pixelization)
         galaxies_with_pixelization_list = self.plane.galaxies_with_cls_list_from(
             cls=aa.Pixelization
         )
-        hyper_galaxy_image_list = self.plane.hyper_galaxies_with_pixelization_image_list
+        adapt_galaxy_image_list = self.plane.adapt_galaxies_with_pixelization_image_list
 
         for mapper_index in range(len(sparse_grid_list)):
-
             mapper = self.mapper_from(
                 mesh=pixelization_list[mapper_index].mesh,
                 regularization=pixelization_list[mapper_index].regularization,
                 source_plane_mesh_grid=sparse_grid_list[mapper_index],
-                hyper_galaxy_image=hyper_galaxy_image_list[mapper_index],
+                adapt_galaxy_image=adapt_galaxy_image_list[mapper_index],
                 image_plane_mesh_grid=sparse_grid_list[mapper_index],
             )
 
             galaxy = galaxies_with_pixelization_list[mapper_index]
 
             mapper_galaxy_dict[mapper] = galaxy
 
         return mapper_galaxy_dict
 
     @property
     def inversion(self) -> aa.AbstractInversion:
-
         inversion = inversion_unpacked_from(
             dataset=self.dataset,
             data=self.data,
             noise_map=self.noise_map,
             w_tilde=self.w_tilde,
             linear_obj_list=self.linear_obj_list,
             settings=self.settings_inversion,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/__init__.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 from autogalaxy.galaxy.plot.galaxy_plotters import GalaxyPDFPlotter
 from autogalaxy.quantity.plot.fit_quantity_plotters import FitQuantityPlotter
 from autogalaxy.imaging.plot.fit_imaging_plotters import FitImagingPlotter
 from autogalaxy.interferometer.plot.fit_interferometer_plotters import (
     FitInterferometerPlotter,
 )
 from autogalaxy.plane.plot.plane_plotters import PlanePlotter
-from autogalaxy.galaxy.plot.hyper_galaxy_plotters import HyperPlotter
+from autogalaxy.galaxy.plot.adapt_plotters import AdaptPlotter
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/abstract_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/abstract_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 from autoarray.plot.abstract_plotters import AbstractPlotter
 
 
 class Plotter(AbstractPlotter):
     @property
     def get_1d(self):
-
         from autogalaxy.plot.get_visuals.one_d import GetVisuals1D
 
         return GetVisuals1D(visuals=self.visuals_1d, include=self.include_1d)
 
     @property
     def get_2d(self):
-
         from autogalaxy.plot.get_visuals.two_d import GetVisuals2D
 
         return GetVisuals2D(visuals=self.visuals_2d, include=self.include_2d)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/get_visuals/one_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/one_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,35 +99,31 @@
         Returns
         -------
         Visuals1D
             The mean value and errors of each attribute that are plotted in 1D by a `Plotter` object.
         """
 
         if self.include.half_light_radius:
-
             half_light_radius_list = [
                 light_profile.half_light_radius for light_profile in light_obj_list
             ]
 
             if None in half_light_radius_list:
-
                 half_light_radius = None
                 half_light_radius_errors = None
 
             else:
-
                 (
                     half_light_radius,
                     half_light_radius_errors,
                 ) = error_util.value_median_and_error_region_via_quantile(
                     value_list=half_light_radius_list, low_limit=low_limit
                 )
 
         else:
-
             half_light_radius = None
             half_light_radius_errors = None
 
         half_light_radius = self.get("half_light_radius", value=half_light_radius)
         half_light_radius_errors = self.get(
             "half_light_radius", value=half_light_radius_errors
         )
@@ -210,19 +206,17 @@
         Returns
         -------
         Visuals1D
             The mean value and errors of each attribute that are plotted in 1D by a `Plotter` object.
         """
 
         if self.include.einstein_radius:
-
             einstein_radius_list = []
 
             for mass_obj in mass_obj_list:
-
                 try:
                     einstein_radius_list.append(
                         mass_obj.einstein_radius_from(grid=grid)
                     )
                 except TypeError:
                     einstein_radius_list.append(None)
 
@@ -232,15 +226,14 @@
                 einstein_radius,
                 einstein_radius_errors,
             ) = error_util.value_median_and_error_region_via_quantile(
                 value_list=einstein_radius_list, low_limit=low_limit
             )
 
         else:
-
             einstein_radius = None
             einstein_radius_errors = None
 
         einstein_radius = self.get("einstein_radius", value=einstein_radius)
         einstein_radius_errors = self.get(
             "einstein_radius", value=einstein_radius_errors
         )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/get_visuals/two_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/two_d.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,21 +63,19 @@
         vis.Visuals2D
             The collection of attributes that can be plotted by a `Plotter` object.
         """
 
         visuals_via_mask = self.via_mask_from(mask=grid.mask)
 
         if isinstance(light_obj, LightProfile):
-
             light_profile_centres = self.get(
                 "light_profile_centres", aa.Grid2DIrregular(values=[light_obj.centre])
             )
 
         else:
-
             light_profile_centres = self.get(
                 "light_profile_centres",
                 light_obj.extract_attribute(cls=LightProfile, attr_name="centre"),
             )
 
         return (
             self.visuals
@@ -115,38 +113,43 @@
         vis.Visuals2D
             The collection of attributes that can be plotted by a `Plotter` object.
         """
 
         visuals_via_mask = self.via_mask_from(mask=grid.mask)
 
         if isinstance(mass_obj, MassProfile):
-
             mass_profile_centres = self.get(
                 "mass_profile_centres", aa.Grid2DIrregular(values=[mass_obj.centre])
             )
 
         else:
-
             mass_profile_centres = self.get(
                 "mass_profile_centres",
                 mass_obj.extract_attribute(cls=MassProfile, attr_name="centre"),
             )
 
         tangential_critical_curves = self.get(
             "tangential_critical_curves",
             mass_obj.tangential_critical_curve_list_from(grid=grid),
             "tangential_critical_curves",
         )
 
-        radial_critical_curves = self.get(
-            "radial_critical_curves",
-            mass_obj.radial_critical_curve_list_from(grid=grid),
-            "radial_critical_curves",
+        radial_critical_curves = None
+
+        radial_critical_curve_area_list = mass_obj.radial_critical_curve_area_list_from(
+            grid=grid
         )
 
+        if any([area > grid.pixel_scale for area in radial_critical_curve_area_list]):
+            radial_critical_curves = self.get(
+                "radial_critical_curves",
+                mass_obj.radial_critical_curve_list_from(grid=grid),
+                "radial_critical_curves",
+            )
+
         return (
             self.visuals
             + visuals_via_mask
             + self.visuals.__class__(
                 mass_profile_centres=mass_profile_centres,
                 tangential_critical_curves=tangential_critical_curves,
                 radial_critical_curves=radial_critical_curves,
@@ -242,25 +245,23 @@
             "mass_profile_centres",
             plane.galaxies[galaxy_index].extract_attribute(
                 cls=MassProfile, attr_name="centre"
             ),
         )
 
         if galaxy_index == 0:
-
             tangential_critical_curves = self.get(
                 "tangential_critical_curves",
                 plane.tangential_critical_curve_list_from(grid=grid),
                 "tangential_critical_curves",
             )
         else:
             tangential_critical_curves = None
 
         if galaxy_index == 0:
-
             radial_critical_curves = self.get(
                 "radial_critical_curves",
                 plane.radial_critical_curve_list_from(grid=grid),
                 "radial_critical_curves",
             )
         else:
             radial_critical_curves = None
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/include/one_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/include/two_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/include/two_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         tangential_caustics=None,
         radial_caustics=None,
         multiple_images=None,
         mapper_source_plane_mesh_grid: Optional[bool] = None,
         mapper_source_plane_data_grid: Optional[bool] = None,
         mapper_image_plane_mesh_grid=None,
     ):
-
         super().__init__(
             origin=origin,
             mask=mask,
             border=border,
             grid=grid,
             mapper_source_plane_mesh_grid=mapper_source_plane_mesh_grid,
             mapper_source_plane_data_grid=mapper_source_plane_data_grid,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/mass_plotter.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/mass_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         mass_obj,
         grid: aa.type.Grid2DLike,
         get_visuals_2d: Callable,
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
     ):
-
         super().__init__(
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
         self.mass_obj = mass_obj
         self.grid = grid
         self._get_visuals_2d = get_visuals_2d
@@ -61,37 +60,34 @@
             Whether to make a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
             Whether to make a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
             Whether to make a 2D plot (via `imshow`) of the magnification.
         """
         if convergence:
-
             self.mat_plot_2d.plot_array(
                 array=self.mass_obj.convergence_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Convergence{title_suffix}",
                     filename=f"convergence_2d{filename_suffix}",
                 ),
             )
 
         if potential:
-
             self.mat_plot_2d.plot_array(
                 array=self.mass_obj.potential_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Potential{title_suffix}",
                     filename=f"potential_2d{filename_suffix}",
                 ),
             )
 
         if deflections_y:
-
             deflections = self.mass_obj.deflections_yx_2d_from(grid=self.grid)
             deflections_y = aa.Array2D(
                 values=deflections.slim[:, 0], mask=self.grid.mask
             )
 
             self.mat_plot_2d.plot_array(
                 array=deflections_y,
@@ -99,15 +95,14 @@
                 auto_labels=aplt.AutoLabels(
                     title=f"Deflections Y{title_suffix}",
                     filename=f"deflections_y_2d{filename_suffix}",
                 ),
             )
 
         if deflections_x:
-
             deflections = self.mass_obj.deflections_yx_2d_from(grid=self.grid)
             deflections_x = aa.Array2D(
                 values=deflections.slim[:, 1], mask=self.grid.mask
             )
 
             self.mat_plot_2d.plot_array(
                 array=deflections_x,
@@ -115,15 +110,14 @@
                 auto_labels=aplt.AutoLabels(
                     title=f"deflections X{title_suffix}",
                     filename=f"deflections_x_2d{filename_suffix}",
                 ),
             )
 
         if magnification:
-
             self.mat_plot_2d.plot_array(
                 array=self.mass_obj.magnification_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Magnification{title_suffix}",
                     filename=f"magnification_2d{filename_suffix}",
                 ),
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/mat_plot/one_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/one_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         )
 
     def set_for_multi_plot(self, is_for_multi_plot: bool, color: str):
         """
         Sets the `is_for_subplot` attribute for every `MatWrap` object in this `MatPlot` object by updating
         the `is_for_subplot`. By changing this tag:
 
-            - The [subplot] section of the config file of every `MatWrap` object is used instead of [figure].
+            - The subplot: section of the config file of every `MatWrap` object is used instead of figure:.
             - Calls which output or close the matplotlib figure are over-ridden so that the subplot is not removed.
 
         Parameters
         ----------
         is_for_subplot
             The entry the `is_for_subplot` attribute of every `MatWrap` object is set too.
         """
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/mat_plot/two_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/visuals/one_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/one_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         shaded_region: Optional[List[Union[List, aa.Array1D, np.ndarray]]] = None,
         half_light_radius: Optional[float] = None,
         half_light_radius_errors: Optional[List[float]] = None,
         einstein_radius: Optional[float] = None,
         einstein_radius_errors: Optional[List[float]] = None,
         model_fluxes: Optional[aa.Grid1D] = None,
     ):
-
         super().__init__(
             origin=origin,
             mask=mask,
             points=points,
             vertical_line=vertical_line,
             shaded_region=shaded_region,
         )
@@ -31,15 +30,14 @@
         self.half_light_radius = half_light_radius
         self.half_light_radius_errors = half_light_radius_errors
         self.einstein_radius = einstein_radius
         self.einstein_radius_errors = einstein_radius_errors
         self.model_fluxes = model_fluxes
 
     def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None):
-
         super().plot_via_plotter(plotter=plotter)
 
         if self.half_light_radius is not None:
             plotter.half_light_radius_axvline.axvline_vertical_line(
                 vertical_line=self.half_light_radius,
                 vertical_errors=self.half_light_radius_errors,
                 label="Half-light Radius",
@@ -49,11 +47,10 @@
             plotter.einstein_radius_axvline.axvline_vertical_line(
                 vertical_line=self.einstein_radius,
                 vertical_errors=self.einstein_radius_errors,
                 label="Einstein Radius",
             )
 
         if self.model_fluxes is not None:
-
             plotter.model_fluxes_yx_scatter.scatter_yx(
                 y=self.model_fluxes, x=np.arange(len(self.model_fluxes))
             )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/visuals/two_d.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/two_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         ] = None,
         parallel_overscan=None,
         serial_prescan=None,
         serial_overscan=None,
         indexes: Union[List[int], List[List[int]]] = None,
         pix_indexes: Union[List[int], List[List[int]]] = None,
     ):
-
         super().__init__(
             mask=mask,
             positions=positions,
             grid=grid,
             mesh_grid=mesh_grid,
             vectors=vectors,
             patches=patches,
@@ -61,15 +60,14 @@
         self.multiple_images = multiple_images
         self.tangential_critical_curves = tangential_critical_curves
         self.radial_critical_curves = radial_critical_curves
         self.tangential_caustics = tangential_caustics
         self.radial_caustics = radial_caustics
 
     def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None):
-
         super().plot_via_plotter(
             plotter=plotter, grid_indexes=grid_indexes, mapper=mapper
         )
 
         if self.light_profile_centres is not None:
             plotter.light_profile_centres_scatter.scatter_grid(
                 grid=self.light_profile_centres
@@ -89,21 +87,25 @@
                     grid=self.tangential_critical_curves
                 )
             except TypeError:
                 pass
 
         if self.radial_critical_curves is not None:
             try:
-                plotter.radial_critical_curves_plot.plot_grid(grid=self.radial_critical_curves)
+                plotter.radial_critical_curves_plot.plot_grid(
+                    grid=self.radial_critical_curves
+                )
             except TypeError:
                 pass
 
         if self.tangential_caustics is not None:
             try:
-                plotter.tangential_caustics_plot.plot_grid(grid=self.tangential_caustics)
+                plotter.tangential_caustics_plot.plot_grid(
+                    grid=self.tangential_caustics
+                )
             except TypeError:
                 pass
 
         if self.radial_caustics is not None:
             try:
                 plotter.radial_caustics_plot.plot_grid(grid=self.radial_caustics)
             except TypeError:
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/plot/wrap.py` & `autogalaxy-2023.7.7.1/autogalaxy/plot/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/geometry_profiles.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/geometry_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     Parameters
     ----------
     centre
         The (y,x) arc-second coordinates of the profile centre.
     """
 
     def __init__(self, centre: Tuple[float, float] = (0.0, 0.0)):
-
         self.centre = centre
 
     def __hash__(self):
         return id(self)
 
     def __repr__(self):
         return "{}\n{}".format(
@@ -76,15 +75,14 @@
     Parameters
     ----------
     centre
         The (y,x) arc-second coordinates of the profile centre.
     """
 
     def __init__(self, centre: Tuple[float, float] = (0.0, 0.0)):
-
         super().__init__(centre=centre)
 
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     def radial_grid_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
         """
         Convert a grid of (y, x) coordinates, to their radial distances from the profile
@@ -266,15 +264,15 @@
 
     @aa.grid_dec.grid_2d_to_structure
     def rotated_grid_from_reference_frame_from(self, grid):
         """
         Rotate a grid of (y,x) coordinates which have been transformed to the elliptical reference frame of a profile
         back to the original unrotated coordinate grid reference frame.
 
-        Note that unlike the method `transformed_from_reference_frame_grid_from` the the coordinates are not
+        Note that unlike the method `transformed_from_reference_frame_grid_from` the coordinates are not
         translated back to the profile's original centre.
 
         This routine is used after computing deflection angles in the reference frame of the profile, so that the
         deflection angles can be re-rotated to the frame of the original coordinates before performing ray-tracing.
 
         Parameters
         ----------
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/eff.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,121 @@
 import numpy as np
-from scipy.integrate import quad
 from typing import Optional, Tuple
 
 import autoarray as aa
 
-from autogalaxy.operate.image import OperateImage
-from autogalaxy.profiles.geometry_profiles import EllProfile
+from autogalaxy.profiles.light.abstract import LightProfile
+from autogalaxy.profiles.light.decorators import (
+    check_operated_only,
+)
 
 
-class LightProfile(EllProfile, OperateImage):
+class ElsonFreeFall(LightProfile):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
+        effective_radius: float = 0.6,
+        eta: float = 1.5,
     ):
         """
-        Abstract base class for an elliptical light-profile.
-
-        Each light profile has an analytic equation associated with it that describes its 1D surface brightness.
-
-        Given an input grid of 1D or 2D (y,x) coordinates the light profile can be used to evaluate its surface
-        brightness in 1D or as a 2D image.
-
-        Associated with a light profile is a spherical or elliptical geometry, which describes its `centre` of
-        emission and ellipticity. Geometric transformations are performed by decorators linked to the **PyAutoArray**
-        `geometry` package.
+        The elliptical Elson, Fall and Freeman (EFF) light profile, which is commonly used to represent the clumps of
+        Lyman-alpha emitter galaxies (see https://arxiv.org/abs/1708.08854).
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
         ell_comps
-            The first and second ellipticity components of the elliptical coordinate system (see the module
-            `autogalaxy -> convert.py` for the convention).
-        """
-        super().__init__(centre=centre, ell_comps=ell_comps)
-        self.intensity = intensity
-
-    def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
-    ) -> aa.Array2D:
+            The first and second ellipticity components of the elliptical coordinate system.
+        intensity
+            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
+            the light profile's image is compared too, which is expected to be electrons per second).
+        effective_radius
+            The circular radius containing half the light of this profile.
+        eta
+            Scales the intensity gradient of the profile.
         """
-        Returns the light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates, which may have been
-        transformed using the light profile's geometry.
-
-        If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
-        profile `centre`), this is performed automatically.
 
-        Parameters
-        ----------
-        grid
-            The 2D (y, x) coordinates in the original reference frame of the grid.
+        super().__init__(centre=centre, ell_comps=ell_comps, intensity=intensity)
 
-        Returns
-        -------
-        image
-            The image of the `LightProfile` evaluated at every (y,x) coordinate on the transformed grid.
-        """
-        raise NotImplementedError()
+        self.effective_radius = effective_radius
+        self.eta = eta
 
     def image_2d_via_radii_from(self, grid_radii: np.ndarray) -> np.ndarray:
         """
-        Returns the light profile's 2D image from a 1D grid of coordinates which are the radial distance of each
-        coordinate from the light profile `centre`.
+        Returns the 2D image of the Sersic light profile from a grid of coordinates which are the radial distances of
+        each coordinate from the its `centre`.
 
         Parameters
         ----------
         grid_radii
             The radial distances from the centre of the profile, for each coordinate on the grid.
         """
-        raise NotImplementedError()
-
-    @aa.grid_dec.grid_1d_to_structure
-    def image_1d_from(self, grid: aa.type.Grid1D2DLike) -> aa.type.Grid1D2DLike:
+        np.seterr(all="ignore")
+        return self._intensity * (1 + (grid_radii / self.effective_radius) ** 2) ** (
+            -self.eta
+        )
+
+    @aa.grid_dec.grid_2d_to_structure
+    @check_operated_only
+    @aa.grid_dec.transform
+    @aa.grid_dec.relocate_to_radial_minimum
+    def image_2d_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> np.ndarray:
         """
-        Returns the light profile's 1D image from a grid of Cartesian coordinates, which may have been
-        transformed using the light profile's geometry.
+        Returns the Eff light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
-        If a 1D grid is input the image is evaluated every coordinate on the grid. If a 2D grid is input, this is
-        converted to a 1D grid by aligning with the major-axis of the light profile's elliptical geometry.
-
-        Internally, this function uses a 2D grid to compute the image, which is mapped to a 1D data structure on return
-        via the `grid_1d_to_structure` decorator. This avoids code repetition by ensuring that light profiles only use
-        their `image_2d_from()`  function to evaluate their image.
+        If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
+        profile `centre`), this is performed automatically.
 
         Parameters
         ----------
         grid
-            A 1D or 2D grid of coordinates which are used to evaluate the light profile in 1D.
+            The 2D (y, x) coordinates in the original reference frame of the grid.
 
         Returns
         -------
         image
-            The 1D image of the light profile evaluated at every (x,) coordinate on the 1D transformed grid.
-        """
-        return self.image_2d_from(grid=grid)
-
-    def luminosity_within_circle_from(self, radius: float) -> float:
+            The image of the Eff evaluated at every (y,x) coordinate on the transformed grid.
         """
-        Integrate the light profile to compute the total luminosity within a circle of specified radius. This is
-        centred on the light profile's `centre`.
+        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
 
-        The `intensity` of a light profile is in dimension units, which are given physical meaning when the light
-        profile is compared to data with physical units. The luminosity output by this function therefore is also
-        dimensionless until compared to data.
-
-        Parameters
-        ----------
-        radius
-            The radius of the circle to compute the dimensionless luminosity within.
-        """
+    @property
+    def half_light_radius(self) -> float:
+        return self.effective_radius * np.sqrt(0.5 ** (1.0 / (1.0 - self.eta)) - 1.0)
 
-        return quad(func=self.luminosity_integral, a=0.0, b=radius)[0]
 
-    def luminosity_integral(self, x: np.ndarray) -> np.ndarray:
+class ElsonFreeFallSph(ElsonFreeFall):
+    def __init__(
+        self,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 0.1,
+        effective_radius: float = 0.6,
+        eta: float = 1.5,
+    ):
         """
-        Routine to integrate the luminosity of an elliptical light profile.
-
-        The axis ratio is set to 1.0 for computing the luminosity within a circle
+        The spherical Elson, Fall and Freeman (EFF) light profile, which is commonly used to represent the clumps of
+        Lyman-alpha emitter galaxies (see https://arxiv.org/abs/1708.08854).
 
         Parameters
         ----------
-        x
-            The 1D (x) radial coordinates where the luminosity integral is evaluated.
-        """
-        return 2 * np.pi * x * self.image_2d_via_radii_from(x)
-
-    @property
-    def half_light_radius(self) -> float:
-
-        if hasattr(self, "effective_radius"):
-            return self.effective_radius
-
-    @property
-    def _intensity(self):
-        return self.intensity
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        intensity
+            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
+            the light profile's image is compared too, which is expected to be electrons per second).
+        effective_radius
+            The circular radius containing half the light of this profile.
+        eta
+            Scales the intensity gradient of the profile.
+        """
+
+        super().__init__(
+            centre=centre,
+            ell_comps=(0.0, 0.0),
+            intensity=intensity,
+            effective_radius=effective_radius,
+            eta=eta,
+        )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/decorators.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/decorators.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,46 +52,52 @@
         args.remove("self")
 
         parameters_dict = {key: parameters_dict[key] for key in args}
         parameters_dict["intensity"] = intensity
 
         return parameters_dict
 
-    def lp_instance_from(self, intensity: float) -> LightProfile:
+    def lp_instance_from(
+        self, linear_light_profile_intensity_dict: Dict
+    ) -> LightProfile:
         """
         Creates an instance of a linear light profile using its parent normal light profile (e.g. the non linear
         variant which has an `intensity` parameter).
 
         The `intensity` value of the profile created is passed into this function and used.
 
         Parameters
         ----------
         intensity
             Overall intensity normalisation of the not linear light profile that is created (units are dimensionless
             and derived from the data the light profile's image is compared too, which is expected to be electrons
             per second).
         """
+        intensity = linear_light_profile_intensity_dict[self]
         parameters_dict = self.parameters_dict_from(intensity=intensity)
 
         return self.lp_cls(**parameters_dict)
 
-    def lmp_model_from(self, intensity: float) -> af.Model(lmp.LightMassProfile):
+    def lmp_model_from(
+        self, linear_light_profile_intensity_dict: Dict
+    ) -> af.Model(lmp.LightMassProfile):
         """
         Creates an instance of a linear light profile using its parent light and mass profile (e.g. the non linear
         variant which has `mass_to_light_ratio` and `intensity` parameters).
 
         The `intensity` value of the profile created is passed into this function and used.
 
         Parameters
         ----------
         intensity
             Overall intensity normalisation of the not linear light profile that is created (units are dimensionless
             and derived from the data the light profile's image is compared too, which is expected to be electrons
             per second).
         """
+        intensity = linear_light_profile_intensity_dict[self]
         parameters_dict = self.parameters_dict_from(intensity=intensity)
 
         return af.Model(self.lmp_cls, **parameters_dict)
 
 
 class LightProfileLinearObjFuncList(aa.AbstractLinearObjFuncList):
     def __init__(
@@ -99,17 +105,15 @@
         grid: aa.type.Grid1D2DLike,
         blurring_grid: aa.type.Grid1D2DLike,
         convolver: Optional[aa.Convolver],
         light_profile_list: List[LightProfileLinear],
         regularization=aa.reg.Regularization,
         profiling_dict: Optional[Dict] = None,
     ):
-
         for light_profile in light_profile_list:
-
             if not isinstance(light_profile, LightProfileLinear):
                 raise exc.ProfileException(
                     """
                     A light profile that is not a LightProfileLinear object has been input into the
                     LightProfileLinearObjFuncList object.
 
                     Only children of the LightProfileLinear class can be used in a linear inversion.
@@ -126,15 +130,14 @@
 
     @property
     def params(self):
         return len(self.light_profile_list)
 
     @property
     def mapping_matrix(self) -> np.ndarray:
-
         mapping_matrix = np.zeros(shape=(self.grid.mask.pixels_in_mask, self.params))
 
         for pixel, light_profile in enumerate(self.light_profile_list):
             image_2d = light_profile.image_2d_from(grid=self.grid).binned.slim
 
             mapping_matrix[:, pixel] = image_2d
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/dev_vaucouleurs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
         effective_radius
             The circular radius containing half the light of this profile.
         """
         super().__init__(
             centre=centre,
             ell_comps=(0.0, 0.0),
             effective_radius=effective_radius,
-        )
+        )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/exponential.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     def lp_cls(self):
         return lp.Exponential
 
     @property
     def lmp_cls(self):
         return lmp.Exponential
 
+
 class ExponentialSph(Exponential):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         effective_radius: float = 0.6,
     ):
         """
@@ -56,8 +57,8 @@
         effective_radius
             The circular radius containing half the light of this profile.
         """
         super().__init__(
             centre=centre,
             ell_comps=(0.0, 0.0),
             effective_radius=effective_radius,
-        )
+        )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/exponential_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/gaussian.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/moffat.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/sersic.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     def lp_cls(self):
         return lp.Sersic
 
     @property
     def lmp_cls(self):
         return lmp.Sersic
 
+
 class SersicSph(Sersic):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         effective_radius: float = 0.6,
         sersic_index: float = 4.0,
     ):
@@ -66,8 +67,8 @@
         """
 
         super().__init__(
             centre=centre,
             ell_comps=(0.0, 0.0),
             effective_radius=effective_radius,
             sersic_index=sersic_index,
-        )
+        )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/linear/sersic_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/mock/mock_light_profile.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/mock_light_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,28 @@
         self,
         image_2d=None,
         image_2d_value=None,
         image_2d_first_value=None,
         value=None,
         value1=None,
     ):
-
         super().__init__()
 
         self.image_2d = image_2d
         self.image_2d_value = image_2d_value
         self.image_2d_first_value = image_2d_first_value
 
         self.value = value
         self.value1 = value1
 
     @aa.grid_dec.grid_2d_to_structure
     @check_operated_only
     def image_2d_from(self, grid, operated_only: Optional[bool] = None):
-
         if self.image_2d is not None:
             return self.image_2d
 
         image_2d = np.ones(shape=(grid.shape[0]))
 
         if self.image_2d_first_value is not None:
-
             image_2d[0] = self.image_2d_first_value
 
         return image_2d
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/cartesian.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/cartesian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/exponential.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/shapelets/polar.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/polar.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         image_2d = self.image_2d_from(grid=grid)
         if psf is not None:
             image_2d = psf.convolved_array_from(array=image_2d)
 
         brightest_value = np.max(image_2d)
 
         def func(intensity_factor):
-
             signal = intensity_factor * brightest_value * exposure_time
             noise = np.sqrt(signal + background_sky_level_counts)
 
             signal_to_noise_ratio = signal / noise
 
             return signal_to_noise_ratio - self.signal_to_noise_ratio
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/chameleon.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/eff.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/eff.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/exponential.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/gaussian.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/sersic.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/snr/sersic_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/chameleon.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/eff.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/gaussian.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,117 +5,111 @@
 
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.decorators import (
     check_operated_only,
 )
 
 
-class ElsonFreeFall(LightProfile):
+class Gaussian(LightProfile):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
-        effective_radius: float = 0.6,
-        eta: float = 1.5,
+        sigma: float = 1.0,
     ):
         """
-        The elliptical Elson, Fall and Freeman (EFF) light profile, which is commonly used to represent the clumps of
-        Lyman-alpha emitter galaxies (see https://arxiv.org/abs/1708.08854).
+        The elliptical Gaussian light profile.
+
+        The intensity distribution of the profile is given by:
+
+        .. math:: I(\\xi) = I \exp (-0.5 \\xi / (\sigma / q^{0.5}))^2
+
+        Where \\xi are elliptical coordinates calculated according to :class: SphProfile.
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
         intensity
             Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
             the light profile's image is compared too, which is expected to be electrons per second).
-        effective_radius
-            The circular radius containing half the light of this profile.
-        eta
-            Scales the intensity gradient of the profile.
+        sigma
+            The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
         """
-
         super().__init__(centre=centre, ell_comps=ell_comps, intensity=intensity)
-
-        self.effective_radius = effective_radius
-        self.eta = eta
+        self.sigma = sigma
 
     def image_2d_via_radii_from(self, grid_radii: np.ndarray) -> np.ndarray:
         """
-        Returns the 2D image of the Sersic light profile from a grid of coordinates which are the radial distances of
+        Returns the 2D image of the Gaussian light profile from a grid of coordinates which are the radial distance of
         each coordinate from the its `centre`.
 
+        Note: sigma is divided by sqrt(q) here.
+
         Parameters
         ----------
         grid_radii
             The radial distances from the centre of the profile, for each coordinate on the grid.
         """
-        np.seterr(all="ignore")
-        return self._intensity * (1 + (grid_radii / self.effective_radius) ** 2) ** (
-            -self.eta
+        return np.multiply(
+            self._intensity,
+            np.exp(
+                -0.5
+                * np.square(
+                    np.divide(grid_radii, self.sigma / np.sqrt(self.axis_ratio))
+                )
+            ),
         )
 
     @aa.grid_dec.grid_2d_to_structure
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> np.ndarray:
         """
-        Returns the Eff light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
+        Returns the Gaussian light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
         Parameters
         ----------
         grid
             The 2D (y, x) coordinates in the original reference frame of the grid.
 
         Returns
         -------
         image
-            The image of the Eff evaluated at every (y,x) coordinate on the transformed grid.
+            The image of the Gaussian evaluated at every (y,x) coordinate on the transformed grid.
         """
-        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
 
-    @property
-    def half_light_radius(self) -> float:
-        return self.effective_radius * np.sqrt(0.5 ** (1.0 / (1.0 - self.eta)) - 1.0)
+        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
 
 
-class ElsonFreeFallSph(ElsonFreeFall):
+class GaussianSph(Gaussian):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
-        effective_radius: float = 0.6,
-        eta: float = 1.5,
+        sigma: float = 1.0,
     ):
         """
-        The spherical Elson, Fall and Freeman (EFF) light profile, which is commonly used to represent the clumps of
-        Lyman-alpha emitter galaxies (see https://arxiv.org/abs/1708.08854).
+        The spherical Gaussian light profile.
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
         intensity
             Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
             the light profile's image is compared too, which is expected to be electrons per second).
-        effective_radius
-            The circular radius containing half the light of this profile.
-        eta
-            Scales the intensity gradient of the profile.
+        sigma
+            The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
         """
-
         super().__init__(
-            centre=centre,
-            ell_comps=(0.0, 0.0),
-            intensity=intensity,
-            effective_radius=effective_radius,
-            eta=eta,
+            centre=centre, ell_comps=(0.0, 0.0), intensity=intensity, sigma=sigma
         )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/exponential.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/exponential_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/moffat.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/sersic.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light/standard/sersic_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/light_and_mass_profiles.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/light_and_mass_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,14 @@
         sersic_index: float = 4.0,
         radius_break: float = 0.01,
         intensity: float = 0.05,
         gamma: float = 0.25,
         alpha: float = 3.0,
         mass_to_light_ratio: float = 1.0,
     ):
-
         lp.SersicCore.__init__(
             self,
             centre=centre,
             ell_comps=ell_comps,
             effective_radius=effective_radius,
             sersic_index=sersic_index,
             radius_break=radius_break,
@@ -624,15 +623,14 @@
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
         core_radius_0: float = 0.01,
         core_radius_1: float = 0.005,
         mass_to_light_ratio: float = 1.0,
     ):
-
         lp.Chameleon.__init__(
             self,
             centre=centre,
             ell_comps=ell_comps,
             intensity=intensity,
             core_radius_0=core_radius_0,
             core_radius_1=core_radius_1,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/__init__.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .abstract.abstract import MassProfile
+from .point import PointMass, SMBH, SMBHBinary
 from .total import (
-    PointMass,
     PowerLawCore,
     PowerLawCoreSph,
     PowerLawBroken,
     PowerLawBrokenSph,
+    PowerLawMultipole,
     IsothermalCore,
     IsothermalCoreSph,
     PowerLaw,
     PowerLawSph,
     Isothermal,
     IsothermalSph,
 )
@@ -39,9 +40,8 @@
     SersicCore,
     SersicCoreSph,
     SersicRadialGradient,
     SersicRadialGradientSph,
     Chameleon,
     ChameleonSph,
 )
-from .multipole import MultipolePowerLawM4
 from .sheets import ExternalShear, MassSheet, InputDeflections
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         """
         super().__init__(centre=centre, ell_comps=ell_comps)
 
     def deflections_yx_2d_from(self, grid):
         raise NotImplementedError
 
     def deflections_2d_via_potential_2d_from(self, grid):
-
         potential = self.potential_2d_from(grid=grid)
 
         deflections_y_2d = np.gradient(potential.native, grid.native[:, 0, 0], axis=0)
         deflections_x_2d = np.gradient(potential.native, grid.native[0, :, 1], axis=1)
 
         return aa.Grid2D(
             values=np.stack((deflections_y_2d, deflections_x_2d), axis=-1),
@@ -120,37 +119,34 @@
         rescaled into a circle using the axis ratio.
 
         This radius corresponds to the Einstein radius of the mass profile, and is a property of a number of \
         mass profiles below.
         """
 
         def func(radius):
-
             return (
                 self.mass_angular_within_circle_from(radius=radius)
                 - np.pi * radius**2.0
             )
 
         return self.ellipticity_rescale * root_scalar(func, bracket=[1e-4, 1e4]).root
 
     def mass_angular_via_normalization_from(self, normalization, radius):
-
         mass_profile = self.with_new_normalization(normalization=normalization)
 
         return mass_profile.mass_angular_within_circle_from(radius=radius)
 
     def normalization_via_mass_angular_from(
         self,
         mass_angular,
         radius,
         normalization_min=1e-15,
         normalization_max=1e15,
         bins=200,
     ):
-
         normalization_list = np.logspace(
             np.log10(normalization_min), np.log10(normalization_max), bins
         )
 
         mass_angulars = [
             self.mass_angular_via_normalization_from(
                 normalization=normalization, radius=radius
@@ -175,15 +171,14 @@
                 ""
                 "The input einstein_radius may be too small or large to feasibly be computed by integrating the "
                 "convergence. Alternative the normalization range or number of bins may need to be changed to "
                 "capture the true einstein_radius value."
             )
 
         def func(normalization, mass_angular_root, radius):
-
             mass_angular = self.mass_angular_via_normalization_from(
                 normalization=normalization, radius=radius
             )
 
             return mass_angular - mass_angular_root
 
         return root_scalar(
@@ -192,26 +187,24 @@
             args=(mass_angular, radius),
         ).root
 
     def with_new_normalization(self, normalization):
         raise NotImplementedError()
 
     def einstein_radius_via_normalization_from(self, normalization):
-
         mass_profile = self.with_new_normalization(normalization=normalization)
 
         try:
             return mass_profile.average_convergence_of_1_radius
         except ValueError:
             return None
 
     def normalization_via_einstein_radius_from(
         self, einstein_radius, normalization_min=1e-9, normalization_max=1e9, bins=100
     ):
-
         normalization_list = np.logspace(
             np.log10(normalization_min), np.log10(normalization_max), bins
         )
 
         einstein_radii = [
             self.einstein_radius_via_normalization_from(normalization=normalization)
             for normalization in normalization_list
@@ -234,30 +227,29 @@
                 ""
                 "The input einstein_radius may be too small or large to feasibly be computed by integrating the "
                 "convergence. Alternative the normalization range or number of bins may need to be changed to "
                 "capture the true einstein_radius value."
             )
 
         def func(normalization, einstein_radius_root):
-
             einstein_radius = self.einstein_radius_via_normalization_from(
                 normalization=normalization
             )
 
             return einstein_radius - einstein_radius_root
 
         return root_scalar(
             func,
             bracket=[normalization_list[0], normalization_list[-1]],
             args=(einstein_radius,),
         ).root
 
     def extract_attribute(self, cls, attr_name):
         """
-        Returns an attribute of a class and its children profiles in the the galaxy as a `ValueIrregular`
+        Returns an attribute of a class and its children profiles in the galaxy as a `ValueIrregular`
         or `Grid2DIrregular` object.
 
         For example, if a galaxy has two light profiles and we want the `LightProfile` axis-ratios, the following:
 
         `galaxy.extract_attribute(cls=LightProfile, name="axis_ratio"`
 
         would return:
@@ -273,14 +265,13 @@
         GridIrregular2D(grid=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1), (centre_y_2, centre_x_2)])
 
         This is used for visualization, for example plotting the centres of all light profiles colored by their profile.
         """
 
         if isinstance(self, cls):
             if hasattr(self, attr_name):
-
                 attribute = getattr(self, attr_name)
 
                 if isinstance(attribute, float):
                     return aa.ArrayIrregular(values=[attribute])
                 if isinstance(attribute, tuple):
                     return aa.Grid2DIrregular(values=[attribute])
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/cse.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/cse.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/abstract/mge.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/mge.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,25 +97,23 @@
     This class speeds up deflection angle calculations of certain mass profiles by decompositing them into many
     Gaussians.
 
     This follows the method of Shajib 2019 - https://academic.oup.com/mnras/article/488/1/1387/5526256
     """
 
     def __init__(self):
-
         self.count = 0
         self.sigma_calc = 0
         self.z = 0
         self.zq = 0
         self.expv = 0
 
     @staticmethod
     #  @aa.util.numba.jit()
     def zeta_from(grid, amps, sigmas, axis_ratio):
-
         """
         The key part to compute the deflection angle of each Gaussian.
         Because of my optimization, there are blocks looking weird and indirect. What I'm doing here
         is trying to avoid big matrix operation to save time.
         I think there are still spaces we can optimize.
 
         It seems when using w_f_approx, it gives some errors if y < 0. So when computing for places
@@ -135,15 +133,14 @@
         ys[ys_minus] *= -1
         z = xs + 1j * ys
         zq = axis_ratio * xs + 1j * ys / axis_ratio
 
         expv = -(xs**2.0) * (1.0 - q2) - ys**2.0 * (1.0 / q2 - 1.0)
 
         for i in range(len(sigmas)):
-
             if i > 0:
                 z /= sigmas[i] / sigmas[i - 1]
                 zq /= sigmas[i] / sigmas[i - 1]
                 expv /= (sigmas[i] / sigmas[i - 1]) ** 2.0
 
             output_grid = -1j * (w_f_approx(z) - np.exp(expv) * w_f_approx(zq))
 
@@ -260,15 +257,14 @@
 
     def convergence_func_gaussian(self, grid_radii, sigma, intensity):
         return np.multiply(
             intensity, np.exp(-0.5 * np.square(np.divide(grid_radii, sigma)))
         )
 
     def _deflections_2d_via_mge_from(self, grid, sigmas_factor=1.0):
-
         axis_ratio = self.axis_ratio
 
         if axis_ratio > 0.9999:
             axis_ratio = 0.9999
 
         amps, sigmas = self.decompose_convergence_via_mge()
         sigmas *= sigmas_factor
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/abstract.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     MassProfileMGE,
 )
 
 from autogalaxy import exc
 
 
 class DarkProfile:
-
     pass
 
 
 class AbstractgNFW(MassProfile, DarkProfile, MassProfileMGE):
     epsrel = 1.49e-5
 
     def __init__(
@@ -108,15 +107,14 @@
         minimum_log_eta = np.log10(eta_min)
         maximum_log_eta = np.log10(eta_max)
         bin_size = (maximum_log_eta - minimum_log_eta) / (tabulate_bins - 1)
 
         return eta_min, eta_max, minimum_log_eta, maximum_log_eta, bin_size
 
     def decompose_convergence_via_mge(self):
-
         rho_at_scale_radius = (
             self.kappa_s / self.scale_radius
         )  # density parameter of 3D gNFW
 
         radii_min = self.scale_radius / 2000.0
         radii_max = self.scale_radius * 30.0
 
@@ -142,32 +140,29 @@
             )
         else:
             return self.coord_func_f_float_jit(grid_radius=grid_radius)
 
     @staticmethod
     @aa.util.numba.jit()
     def coord_func_f_jit(grid_radius, f):
-
         for index in range(f.shape[0]):
-
             if np.real(grid_radius[index]) > 1.0:
                 f[index] = (
                     1.0 / np.sqrt(np.square(grid_radius[index]) - 1.0)
                 ) * np.arccos(np.divide(1.0, grid_radius[index]))
             elif np.real(grid_radius[index]) < 1.0:
                 f[index] = (
                     1.0 / np.sqrt(1.0 - np.square(grid_radius[index]))
                 ) * np.arccosh(np.divide(1.0, grid_radius[index]))
 
         return f
 
     @staticmethod
     @aa.util.numba.jit()
     def coord_func_f_float_jit(grid_radius):
-
         if np.real(grid_radius) > 1.0:
             return (1.0 / np.sqrt(np.square(grid_radius) - 1.0)) * np.arccos(
                 np.divide(1.0, grid_radius)
             )
         elif np.real(grid_radius) < 1.0:
             return (1.0 / np.sqrt(1.0 - np.square(grid_radius))) * np.arccosh(
                 np.divide(1.0, grid_radius)
@@ -186,29 +181,27 @@
             )
         else:
             return self.coord_func_g_float_jit(grid_radius=grid_radius, f_r=f_r)
 
     @staticmethod
     @aa.util.numba.jit()
     def coord_func_g_jit(grid_radius, f_r, g):
-
         for index in range(f_r.shape[0]):
             if np.real(grid_radius[index]) > 1.0:
                 g[index] = (1.0 - f_r[index]) / (np.square(grid_radius[index]) - 1.0)
             elif np.real(grid_radius[index]) < 1.0:
                 g[index] = (f_r[index] - 1.0) / (1.0 - np.square(grid_radius[index]))
             else:
                 g[index] = 1.0 / 3.0
 
         return g
 
     @staticmethod
     @aa.util.numba.jit()
     def coord_func_g_float_jit(grid_radius, f_r):
-
         if np.real(grid_radius) > 1.0:
             return (1.0 - f_r) / (np.square(grid_radius) - 1.0)
         elif np.real(grid_radius) < 1.0:
             return (f_r - 1.0) / (1.0 - np.square(grid_radius))
         else:
             return 1.0 / 3.0
 
@@ -236,15 +229,14 @@
     def delta_concentration(
         self,
         redshift_object,
         redshift_source,
         redshift_of_cosmic_average_density="profile",
         cosmology: LensingCosmology = Planck15(),
     ):
-
         if redshift_of_cosmic_average_density == "profile":
             redshift_calc = redshift_object
         elif redshift_of_cosmic_average_density == "local":
             redshift_calc = 0.0
         else:
             raise exc.UnitsException(
                 "The redshift of the cosmic average density haas been specified as an invalid "
@@ -268,15 +260,14 @@
     def concentration(
         self,
         redshift_profile,
         redshift_source,
         redshift_of_cosmic_average_density="profile",
         cosmology: LensingCosmology = Planck15(),
     ):
-
         delta_concentration = self.delta_concentration(
             redshift_object=redshift_profile,
             redshift_source=redshift_source,
             redshift_of_cosmic_average_density=redshift_of_cosmic_average_density,
             cosmology=cosmology,
         )
 
@@ -301,15 +292,14 @@
     def radius_at_200(
         self,
         redshift_object,
         redshift_source,
         redshift_of_cosmic_average_density="profile",
         cosmology: LensingCosmology = Planck15(),
     ):
-
         concentration = self.concentration(
             redshift_profile=redshift_object,
             redshift_source=redshift_source,
             redshift_of_cosmic_average_density=redshift_of_cosmic_average_density,
             cosmology=cosmology,
         )
 
@@ -318,15 +308,14 @@
     def mass_at_200_solar_masses(
         self,
         redshift_object,
         redshift_source,
         redshift_of_cosmic_average_density="profile",
         cosmology: LensingCosmology = Planck15(),
     ):
-
         if redshift_of_cosmic_average_density == "profile":
             redshift_calc = redshift_object
         elif redshift_of_cosmic_average_density == "local":
             redshift_calc = 0.0
         else:
             raise exc.UnitsException(
                 "The redshift of the cosmic average density haas been specified as an invalid "
@@ -358,11 +347,10 @@
         )
 
     @property
     def ellipticity_rescale(self):
         return 1.0 - ((1.0 - self.axis_ratio) / 2.0)
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.kappa_s = normalization
         return mass_profile
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/gnfw.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import autoarray as aa
 
 from autogalaxy.profiles.mass.dark.abstract import AbstractgNFW
 
 
 def jit_integrand(integrand_function):
-
     from numba import cfunc
     from numba.types import intc, CPointer, float64
 
     jitted_function = aa.util.numba.jit(nopython=True, cache=True)(integrand_function)
     no_args = len(inspect.getfullargspec(integrand_function).args)
 
     wrapped = None
@@ -81,22 +80,20 @@
     cf = cfunc(float64(intc, CPointer(float64)))
 
     return LowLevelCallable(cf(wrapped).ctypes)
 
 
 class gNFW(AbstractgNFW):
     def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-
         return self.deflections_2d_via_mge_from(grid=grid)
 
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_2d_via_mge_from(self, grid: aa.type.Grid2DLike):
-
         return self._deflections_2d_via_mge_from(
             grid=grid, sigmas_factor=self.axis_ratio
         )
 
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
@@ -120,19 +117,17 @@
             return (
                 (3 - inner_slope)
                 * (x + kappa_radius / scale_radius) ** (inner_slope - 4)
                 * (1 - np.sqrt(1 - x * x))
             )
 
         def calculate_deflection_component(npow, yx_index):
-
             deflection_grid = np.zeros(grid.shape[0])
 
             for i in range(grid.shape[0]):
-
                 deflection_grid[i] = (
                     2.0
                     * self.kappa_s
                     * self.axis_ratio
                     * grid[i, yx_index]
                     * quad(
                         self.deflection_func,
@@ -194,15 +189,14 @@
         npow,
         axis_ratio,
         minimum_log_eta,
         maximum_log_eta,
         tabulate_bins,
         surface_density_integral,
     ):
-
         _eta_u = np.sqrt((u * ((x**2) + (y**2 / (1 - (1 - axis_ratio**2) * u)))))
         bin_size = (maximum_log_eta - minimum_log_eta) / (tabulate_bins - 1)
         i = 1 + int((np.log10(_eta_u) - minimum_log_eta) / bin_size)
         r1 = 10.0 ** (minimum_log_eta + (i - 1) * bin_size)
         r2 = r1 * 10.0**bin_size
         kap = surface_density_integral[i] + (
             surface_density_integral[i + 1] - surface_density_integral[i]
@@ -212,15 +206,14 @@
     def convergence_func(self, grid_radius: float) -> float:
         def integral_y(y, eta):
             return (y + eta) ** (self.inner_slope - 4) * (1 - np.sqrt(1 - y**2))
 
         grid_radius = (1.0 / self.scale_radius) * grid_radius
 
         for index in range(grid_radius.shape[0]):
-
             integral_y_value = quad(
                 integral_y,
                 a=0.0,
                 b=1.0,
                 args=grid_radius[index],
                 epsrel=gNFW.epsrel,
             )[0]
@@ -292,15 +285,14 @@
                     4 - self.inner_slope,
                     -(eta / self.scale_radius),
                 )
                 + integral
             )
 
         for i in range(grid.shape[0]):
-
             potential_grid[i] = (2.0 * self.kappa_s * self.axis_ratio) * quad(
                 self.potential_func,
                 a=0.0,
                 b=1.0,
                 args=(
                     grid[i, 0],
                     grid[i, 1],
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/gnfw_mcr.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw_mcr.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
         inner_slope: float = 1.0,
     ):
-
         self.mass_at_200 = mass_at_200
         self.redshift_object = redshift_object
         self.redshift_source = redshift_source
 
         (
             kappa_s,
             scale_radius,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/mcr_util.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/mcr_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from astropy import units
-from colossus.cosmology import cosmology as col_cosmology
-from colossus.halo.concentration import concentration as col_concentration
+
 import numpy as np
 import warnings
 
 from autogalaxy.cosmology.wrap import Planck15
 
 
 def kappa_s_and_scale_radius_for_duffy(mass_at_200, redshift_object, redshift_source):
-
     cosmology = Planck15()
 
     cosmic_average_density = (
         cosmology.critical_density(redshift_object).to(units.solMass / units.kpc**3)
     ).value
 
     critical_surface_density = (
@@ -50,14 +48,16 @@
 
     return kappa_s, scale_radius, radius_at_200
 
 
 def kappa_s_and_scale_radius_for_ludlow(
     mass_at_200, scatter_sigma, redshift_object, redshift_source
 ):
+    from colossus.cosmology import cosmology as col_cosmology
+    from colossus.halo.concentration import concentration as col_concentration
 
     warnings.filterwarnings("ignore")
 
     cosmology = Planck15()
 
     col_cosmo = col_cosmology.setCosmology("planck15")
     m_input = mass_at_200 * col_cosmo.h
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
         """
 
         def calculate_deflection_component(npow, index):
             deflection_grid = self.axis_ratio * grid[:, index]
 
             for i in range(grid.shape[0]):
-
                 deflection_grid[i] *= (
                     self.kappa_s
                     * quad(
                         self.deflection_func,
                         a=0.0,
                         b=1.0,
                         args=(
@@ -158,15 +157,14 @@
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
 
         """
 
         potential_grid = np.zeros(grid.shape[0])
 
         for i in range(grid.shape[0]):
-
             potential_grid[i] = quad(
                 self.potential_func,
                 a=0.0,
                 b=1.0,
                 args=(
                     grid[i, 0],
                     grid[i, 1],
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_mcr.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
     ):
-
         self.mass_at_200 = mass_at_200
         self.redshift_object = redshift_object
         self.redshift_source = redshift_source
 
         (
             kappa_s,
             scale_radius,
@@ -31,28 +30,26 @@
             redshift_object=redshift_object,
             redshift_source=redshift_source,
         )
 
         super().__init__(centre=centre, kappa_s=kappa_s, scale_radius=scale_radius)
 
     def with_new_normalization(self, normalization):
-
         raise NotImplementedError()
 
 
 class NFWMCRLudlow(NFW):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
     ):
-
         self.mass_at_200 = mass_at_200
         self.redshift_object = redshift_object
         self.redshift_source = redshift_source
 
         (
             kappa_s,
             scale_radius,
@@ -76,15 +73,14 @@
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
     ):
-
         super().__init__(
             centre=centre,
             mass_at_200=mass_at_200,
             scatter_sigma=0.0,
             redshift_object=redshift_object,
             redshift_source=redshift_source,
         )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         scatter_sigma: float = 0.0,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
     ):
-
         self.mass_at_200 = mass_at_200
         self.scatter_sigma = scatter_sigma
         self.redshift_object = redshift_object
         self.redshift_source = redshift_source
 
         (
             kappa_s,
@@ -41,15 +40,14 @@
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         scatter_sigma: float = 0.0,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
     ):
-
         self.mass_at_200 = mass_at_200
         self.scatter_sigma = scatter_sigma
         self.redshift_object = redshift_object
         self.redshift_source = redshift_source
 
         (
             kappa_s,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_truncated.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
             np.divide(
                 grid_radius,
                 np.sqrt(np.square(grid_radius) + np.square(self.tau)) + self.tau,
             )
         )
 
     def coord_func_l(self, grid_radius):
-
         f_r = self.coord_func_f(grid_radius=grid_radius)
         g_r = self.coord_func_g(grid_radius=grid_radius)
         k_r = self.coord_func_k(grid_radius=grid_radius)
 
         return np.divide(self.tau**2.0, (self.tau**2.0 + 1.0) ** 2.0) * (
             ((self.tau**2.0 + 1.0) * g_r)
             + (2 * f_r)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         mass_at_200: float = 1e9,
         scatter_sigma: float = 0.0,
         redshift_object: float = 0.5,
         redshift_source: float = 1.0,
     ):
-
         self.mass_at_200 = mass_at_200
         self.scatter_sigma = scatter_sigma
         self.redshift_object = redshift_object
         self.redshift_source = redshift_source
 
         (
             kappa_s,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/mock/mock_mass_profile.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/mock_mass_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
         self,
         convergence_2d=None,
         potential_2d=None,
         deflections_yx_2d=None,
         value=None,
         value1=None,
     ):
-
         super().__init__()
 
         self.convergence_2d = convergence_2d
         self.potential_2d = potential_2d
         self.deflections_2d = deflections_yx_2d
 
         self.value = value
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/multipole/power_law_m4.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_multipole.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,24 +62,25 @@
     )
     k_m = np.sqrt(ell_comps_multipole[1] ** 2 + ell_comps_multipole[0] ** 2)
     if angle_m < 0.0:
         return k_m, angle_m + 90.0
     return k_m, angle_m
 
 
-class MultipolePowerLawM4(MassProfile):
+class PowerLawMultipole(MassProfile):
     def __init__(
         self,
+        m: int,
         centre: Tuple[float, float] = (0.0, 0.0),
         einstein_radius: float = 1.0,
         slope: float = 2.0,
         ell_comps_multipole: Tuple[float, float] = (0.0, 0.0),
     ):
         r"""
-        A multipole extension with multipole order M=4 to the power-law total mass distribution.
+        A multipole extension with multipole order M to the power-law total mass distribution.
 
         Quantities computed from this profile (e.g. deflections, convergence) are of only the multipole, and not the
         power-law mass distribution itself.
 
         The typical use case is therefore for the multipoles to be combined with a `PowerLaw` mass profile with the
         same parameters (see example below).
 
@@ -117,15 +118,15 @@
         mass = al.mp.PowerLaw(
             centre=(0.0, 0.0),
             ell_comps=(-0.1, 0.2),
             einstein_radius=1.0,
             slope=2.2
         )
 
-        multipole = al.mp.MultipolePowerLawM4(
+        multipole = al.mp.PowerLawMultipole(
             centre=(0.0, 0.0),
             einstein_radius=1.0,
             slope=2.2,
             ell_comps_multipole=(0.3, 0.2)
         )
 
         galaxy = al.Galaxy(
@@ -138,15 +139,15 @@
 
         deflections = galaxy.deflections_yx_2d_from(
             grid=grid
         )
         """
         super().__init__(centre=centre, ell_comps=(0.0, 0.0))
 
-        self.m = 4
+        self.m = int(m)
 
         self.einstein_radius = einstein_radius
         self.slope = slope
 
         self.ell_comps_multipole = ell_comps_multipole
         self.k_m, self.angle_m = multipole_parameters_from(
             ell_comps_multipole=ell_comps_multipole
@@ -219,15 +220,15 @@
         )
 
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def convergence_2d_from(self, grid: aa.type.Grid1D2DLike) -> np.ndarray:
         """
-        Calculate the projected convergence on a grid of (y,x) arc-second coordinates.
+        Returns the two dimensional projected convergence on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
         r, angle = radial_and_angle_grid_from(grid=grid)
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/external_shear.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/external_shear.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,23 @@
 
     @aa.grid_dec.grid_2d_to_structure
     def convergence_2d_from(self, grid: aa.type.Grid2DLike):
         return np.zeros(shape=grid.shape[0])
 
     @aa.grid_dec.grid_2d_to_structure
     def potential_2d_from(self, grid: aa.type.Grid2DLike):
-        return np.zeros(shape=grid.shape[0])
+        shear_angle = (
+            self.angle - 90
+        )  ##to be onsistent with autolens deflection angle calculation
+        phig = np.deg2rad(shear_angle)
+        shear_amp = self.magnitude
+        phicoord = np.arctan2(grid[:, 0], grid[:, 1])
+        rcoord = np.sqrt(grid[:, 0] ** 2.0 + grid[:, 1] ** 2.0)
+
+        return -0.5 * shear_amp * rcoord**2 * np.cos(2 * (phicoord - phig))
 
     @aa.grid_dec.grid_2d_to_vector_yx
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
         """
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/input_deflections.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/input_deflections.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,29 +75,26 @@
     @aa.grid_dec.grid_2d_to_structure
     def potential_2d_from(self, grid: aa.type.Grid2DLike):
         return np.zeros(shape=grid.shape[0])
 
     @aa.grid_dec.grid_2d_to_vector_yx
     @aa.grid_dec.grid_2d_to_structure
     def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-
         if self.preload_grid is not None and self.preload_deflections is not None:
-
             try:
                 if grid.sub_shape_slim == self.preload_grid.sub_shape_slim:
                     if np.allclose(grid, self.preload_grid, 1e-8):
                         return self.normalization_scale * self.preload_deflections
             except AttributeError:
                 pass
 
         if (
             self.preload_blurring_grid is not None
             and self.preload_blurring_deflections is not None
         ):
-
             try:
                 if grid.sub_shape_slim == self.preload_blurring_grid.sub_shape_slim:
                     if np.allclose(grid, self.preload_blurring_grid, 1e-8):
                         return (
                             self.normalization_scale * self.preload_blurring_deflections
                         )
             except AttributeError:
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/sheets/mass_sheet.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/mass_sheet.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/chameleon.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/chameleon.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,14 @@
 
     @property
     def axis_ratio(self):
         axis_ratio = super().axis_ratio
         return axis_ratio if axis_ratio < 0.99999 else 0.99999
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.mass_to_light_ratio = normalization
         return mass_profile
 
 
 class ChameleonSph(Chameleon):
     def __init__(
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/exponential.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 from typing import Tuple
 
 from autogalaxy.profiles.mass.stellar.sersic import Sersic
 
 
-class DevVaucouleurs(Sersic):
+class Exponential(Sersic):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
         effective_radius: float = 0.6,
         mass_to_light_ratio: float = 1.0,
     ):
         """
-        The DevVaucouleurs mass profile, the mass profiles of the light profiles that are used to fit and
+        The Exponential mass profile, the mass profiles of the light profiles that are used to fit and
         subtract the lens model_galaxy's light.
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
         intensity
             Overall flux intensity normalisation in the light profiles (electrons per second).
         effective_radius
-            The radius containing half the light of this profile.
+            The circular radius containing half the light of this profile.
         mass_to_light_ratio
-            The mass-to-light ratio of the light profile.
+            The mass-to-light ratio of the light profiles
         """
         super().__init__(
             centre=centre,
             ell_comps=ell_comps,
             intensity=intensity,
             effective_radius=effective_radius,
-            sersic_index=4.0,
+            sersic_index=1.0,
             mass_to_light_ratio=mass_to_light_ratio,
         )
 
 
-class DevVaucouleursSph(DevVaucouleurs):
+class ExponentialSph(Exponential):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
         effective_radius: float = 0.6,
         mass_to_light_ratio: float = 1.0,
     ):
         """
-        The DevVaucouleurs mass profile, the mass profiles of the light profiles that are used to fit and subtract the
-        lens model_galaxy's light.
+        The Exponential mass profile, the mass profiles of the light profiles that are used to fit and subtract the lens
+        model_galaxy's light.
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
         intensity
             Overall flux intensity normalisation in the light profiles (electrons per second).
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/gaussian.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,19 +94,17 @@
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
 
         Note: sigma is divided by sqrt(q) here.
 
         """
 
         def calculate_deflection_component(npow, index):
-
             deflection_grid = self.axis_ratio * grid[:, index]
 
             for i in range(grid.shape[0]):
-
                 deflection_grid[i] *= (
                     self.intensity
                     * self.mass_to_light_ratio
                     * quad(
                         self.deflection_func,
                         a=0.0,
                         b=1.0,
@@ -211,11 +209,10 @@
                 * wofz(self.axis_ratio * xs_1 + 1j * ys_1 / self.axis_ratio)
             )
         )
 
         return output_grid
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.mass_to_light_ratio = normalization
         return mass_profile
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/sersic.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,16 @@
 )
 from autogalaxy.profiles.mass.stellar.abstract import StellarProfile
 
 
 def cse_settings_from(
     effective_radius, sersic_index, sersic_constant, mass_to_light_gradient
 ):
-
     if mass_to_light_gradient > 0.5:
-
         if effective_radius > 0.2:
-
             lower_dex = 6.0
             upper_dex = np.min(
                 [np.log10((18.0 / sersic_constant) ** sersic_index), 1.1]
             )
 
             if sersic_index <= 1.2:
                 total_cses = 50
@@ -53,15 +50,14 @@
                 upper_dex = 1.5
             else:
                 upper_dex = 1.1
                 lower_dex = 6.0
                 total_cses = 30
                 sample_points = 50
     else:
-
         upper_dex = np.min(
             [
                 np.log10((23.0 / sersic_constant) ** sersic_index),
                 0.85 - np.log10(effective_radius),
             ]
         )
 
@@ -348,15 +344,14 @@
 
         The elliptical effective radius instead describes the major-axis radius of the ellipse containing \
         half the light, and may be more appropriate for highly flattened systems like disk galaxies.
         """
         return self.effective_radius / np.sqrt(self.axis_ratio)
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.mass_to_light_ratio = normalization
         return mass_profile
 
 
 class Sersic(AbstractSersic, MassProfileMGE, MassProfileCSE):
     @aa.grid_dec.grid_2d_to_structure
@@ -375,15 +370,14 @@
 
         def calculate_deflection_component(npow, index):
             sersic_constant = self.sersic_constant
 
             deflection_grid = self.axis_ratio * grid[:, index]
 
             for i in range(grid.shape[0]):
-
                 deflection_grid[i] *= (
                     self.intensity
                     * self.mass_to_light_ratio
                     * quad(
                         self.deflection_func,
                         a=0.0,
                         b=1.0,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/sersic_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
                         )
                     ),
                 )
             ),
         )
 
     def decompose_convergence_via_mge(self):
-
         radii_min = self.effective_radius / 50.0
         radii_max = self.effective_radius * 20.0
 
         def core_sersic_2D(r):
             return (
                 self.mass_to_light_ratio
                 * self.intensity_prime
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 
         def calculate_deflection_component(npow, index):
             sersic_constant = self.sersic_constant
 
             deflection_grid = self.axis_ratio * grid[:, index]
 
             for i in range(grid.shape[0]):
-
                 deflection_grid[i] *= (
                     self.intensity
                     * self.mass_to_light_ratio
                     * quad(
                         self.deflection_func,
                         a=0.0,
                         b=1.0,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/isothermal.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/isothermal_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/point.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/point.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         einstein_radius
             The arc-second Einstein radius of the point-mass.
         """
         super().__init__(centre=centre, ell_comps=(0.0, 0.0))
         self.einstein_radius = einstein_radius
 
     def convergence_2d_from(self, grid: aa.type.Grid2DLike):
-
         squared_distances = np.square(grid[:, 0] - self.centre[0]) + np.square(
             grid[:, 1] - self.centre[1]
         )
         central_pixel = np.argmin(squared_distances)
 
         convergence = np.zeros(shape=grid.shape[0])
         #    convergence[central_pixel] = np.pi * self.einstein_radius ** 2.0
@@ -50,11 +49,10 @@
         )
 
     @property
     def is_point_mass(self):
         return True
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.einstein_radius = normalization
         return mass_profile
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/power_law.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,26 @@
             centre=centre,
             ell_comps=ell_comps,
             einstein_radius=einstein_radius,
             slope=slope,
             core_radius=0.0,
         )
 
+    @aa.grid_dec.grid_2d_to_structure
+    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+        alpha = self.deflections_yx_2d_from(grid)
+
+        alpha_x = alpha[:, 1]
+        alpha_y = alpha[:, 0]
+
+        x = grid[:, 1] - self.centre[1]
+        y = grid[:, 0] - self.centre[0]
+
+        return (x * alpha_x + y * alpha_y) / (3 - self.slope)
+
     @aa.grid_dec.grid_2d_to_vector_yx
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
@@ -140,15 +152,14 @@
         )
 
     @aa.grid_dec.grid_2d_to_vector_yx
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-
         eta = self.radial_grid_from(grid)
         deflection_r = (
             2.0
             * self.einstein_radius_rescaled
             * np.divide(
                 np.power(eta, (3.0 - self.slope)), np.multiply((3.0 - self.slope), eta)
             )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/power_law_broken.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_broken.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import copy
 import numpy as np
-from scipy.integrate import quad
-from scipy import special
 from typing import Tuple
 
 import autoarray as aa
 
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 
 
@@ -155,15 +153,14 @@
         for n in range(max_terms):
             F += a_n * (u**n)
             a_n *= ((2 * n) + 4 - (2 * t)) / ((2 * n) + 4 - t)
 
         return F
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.einstein_radius_elliptical = normalization
         return mass_profile
 
 
 class PowerLawBrokenSph(PowerLawBroken):
     def __init__(
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/mass/total/power_law_core.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         )
 
     @aa.grid_dec.grid_2d_to_structure
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def convergence_2d_from(self, grid: aa.type.Grid2DLike):
         """
-        Calculate the projected convergence on a grid of (y,x) arc-second coordinates.
+        Returns the two dimensional projected convergence on a grid of (y,x) arc-second coordinates.
 
         The `grid_2d_to_structure` decorator reshapes the ndarrays the convergence is outputted on. See
         *aa.grid_2d_to_structure* for a description of the output.
 
         Parameters
         ----------
         grid
@@ -83,18 +83,19 @@
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
 
+        print(grid)
+
         potential_grid = np.zeros(grid.shape[0])
 
         for i in range(grid.shape[0]):
-
             potential_grid[i] = quad(
                 self.potential_func,
                 a=0.0,
                 b=1.0,
                 args=(
                     grid[i, 0],
                     grid[i, 1],
@@ -123,15 +124,14 @@
 
         def calculate_deflection_component(npow, index):
             einstein_radius_rescaled = self.einstein_radius_rescaled
 
             deflection_grid = self.axis_ratio * grid[:, index]
 
             for i in range(grid.shape[0]):
-
                 deflection_grid[i] *= (
                     einstein_radius_rescaled
                     * quad(
                         self.deflection_func,
                         a=0.0,
                         b=1.0,
                         args=(
@@ -184,15 +184,14 @@
         return (1.0 + self.axis_ratio) / 2.0
 
     @property
     def unit_mass(self):
         return "angular"
 
     def with_new_normalization(self, normalization):
-
         mass_profile = copy.copy(self)
         mass_profile.einstein_radius = normalization
         return mass_profile
 
 
 class PowerLawCoreSph(PowerLawCore):
     def __init__(
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/plot/light_profile_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/light_profile_plotters.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         """
 
         from autogalaxy.profiles.light.linear import (
             LightProfileLinear,
         )
 
         if isinstance(light_profile, LightProfileLinear):
-
             raise exc.raise_linear_light_profile_in_plot(
                 plotter_type=self.__class__.__name__, model_obj="Plane"
             )
 
         self.light_profile = light_profile
         self.grid = grid
 
@@ -112,15 +111,14 @@
         """
         if self.mat_plot_1d.yx_plot.plot_axis_type is None:
             plot_axis_type_override = "semilogy"
         else:
             plot_axis_type_override = None
 
         if image:
-
             image_1d = self.light_profile.image_1d_from(grid=self.grid)
 
             self.mat_plot_1d.plot_yx(
                 y=image_1d,
                 x=image_1d.grid_radial,
                 visuals_1d=self.get_visuals_1d(),
                 auto_labels=aplt.AutoLabels(
@@ -143,15 +141,14 @@
 
         Parameters
         ----------
         image
             Whether to make a 2D plot (via `imshow`) of the image.
         """
         if image:
-
             self.mat_plot_2d.plot_array(
                 array=self.light_profile.image_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(title="Image", filename="image_2d"),
             )
 
 
@@ -250,15 +247,14 @@
         """
         if self.mat_plot_1d.yx_plot.plot_axis_type is None:
             plot_axis_type_override = "semilogy"
         else:
             plot_axis_type_override = None
 
         if image:
-
             image_1d_list = [
                 light_profile.image_1d_from(grid=self.grid)
                 for light_profile in self.light_profile_pdf_list
             ]
 
             min_index = min([image_1d.shape[0] for image_1d in image_1d_list])
             image_1d_list = [image_1d[0:min_index] for image_1d in image_1d_list]
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/plot/mass_profile_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/mass_profile_plotters.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
         """
         if self.mat_plot_1d.yx_plot.plot_axis_type is None:
             plot_axis_type_override = "semilogy"
         else:
             plot_axis_type_override = None
 
         if convergence:
-
             convergence_1d = self.mass_profile.convergence_1d_from(grid=self.grid)
 
             self.mat_plot_1d.plot_yx(
                 y=convergence_1d,
                 x=convergence_1d.grid_radial,
                 visuals_1d=self.get_visuals_1d(),
                 auto_labels=aplt.AutoLabels(
@@ -129,15 +128,14 @@
                     legend=self.mass_profile.__class__.__name__,
                     filename="convergence_1d",
                 ),
                 plot_axis_type_override=plot_axis_type_override,
             )
 
         if potential:
-
             potential_1d = self.mass_profile.potential_1d_from(grid=self.grid)
 
             self.mat_plot_1d.plot_yx(
                 y=potential_1d,
                 x=potential_1d.grid_radial,
                 visuals_1d=self.get_visuals_1d(),
                 auto_labels=aplt.AutoLabels(
@@ -244,15 +242,14 @@
         """
         if self.mat_plot_1d.yx_plot.plot_axis_type is None:
             plot_axis_type_override = "semilogy"
         else:
             plot_axis_type_override = None
 
         if convergence:
-
             convergence_1d_list = [
                 mass_profile.convergence_1d_from(grid=self.grid)
                 for mass_profile in self.mass_profile_pdf_list
             ]
 
             min_index = min(
                 [convergence_1d.shape[0] for convergence_1d in convergence_1d_list]
@@ -290,15 +287,14 @@
                     legend=self.mass_profile_pdf_list[0].__class__.__name__,
                     filename="convergence_1d",
                 ),
                 plot_axis_type_override=plot_axis_type_override,
             )
 
         if potential:
-
             potential_1d_list = [
                 mass_profile.potential_1d_from(grid=self.grid)
                 for mass_profile in self.mass_profile_pdf_list
             ]
 
             min_index = min(
                 [potential_1d.shape[0] for potential_1d in potential_1d_list]
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/profiles/scaling_relations.py` & `autogalaxy-2023.7.7.1/autogalaxy/profiles/scaling_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from typing import Tuple
 
 from autogalaxy.profiles import mass as mp
 
 
 class MassLightRelation:
     def __init__(self, gradient=1.0, denominator=1.0, power=0.5):
-
         self.gradient = gradient
         self.denominator = denominator
         self.power = power
 
     def einstein_radius_from(self, luminosity):
-
         return self.gradient * ((luminosity / self.denominator) ** self.power)
 
 
 class IsothermalSphMLR(mp.IsothermalSph):
     def __init__(
         self,
         relation: MassLightRelation = MassLightRelation(),
         luminosity: float = 1.0,
         centre: Tuple[float, float] = (0.0, 0.0),
     ):
-
         self.luminosity = luminosity
         self.relation = relation
 
         einstein_radius = relation.einstein_radius_from(luminosity=luminosity)
 
         super().__init__(centre=centre, einstein_radius=einstein_radius)
 
@@ -35,15 +32,14 @@
     def __init__(
         self,
         relation: MassLightRelation = MassLightRelation(),
         luminosity: float = 1.0,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
     ):
-
         self.luminosity = luminosity
         self.relation = relation
 
         einstein_radius = relation.einstein_radius_from(luminosity=luminosity)
 
         super().__init__(
             centre=centre,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/quantity/dataset_quantity.py` & `autogalaxy-2023.7.7.1/autogalaxy/quantity/dataset_quantity.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,15 @@
         noise_map
             The 2D noise map of the quantity's data, which is often chosen in an arbitrary way.
         settings
             Controls settings of how the dataset is set up (e.g. the types of grids used to perform calculations).
         """
 
         if data.shape != noise_map.shape:
-
             if data.shape[0:-1] == noise_map.shape[0:]:
-
                 noise_map = aa.VectorYX2D.no_mask(
                     values=np.stack((noise_map, noise_map), axis=-1),
                     pixel_scales=data.pixel_scales,
                     shape_native=data.shape_native,
                     sub_size=data.sub_size,
                     origin=data.origin,
                 )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/quantity/fit_quantity.py` & `autogalaxy-2023.7.7.1/autogalaxy/quantity/fit_quantity.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,15 @@
         self.func_str = func_str
         self.model_data_manual = model_data_manual
 
         super().__init__(dataset=dataset, use_mask_in_fit=False)
 
     @property
     def model_data(self):
-
         if self.model_data_manual is None:
-
             func = getattr(self.light_mass_obj, self.func_str)
             return func(grid=self.dataset.grid)
 
         return self.model_data_manual
 
     @property
     def y(self) -> "FitQuantity":
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/quantity/model/analysis.py` & `autogalaxy-2023.7.7.1/autogalaxy/quantity/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         )
 
     def visualize(
         self,
         paths: af.DirectoryPaths,
         instance: af.ModelInstance,
         during_analysis: bool,
-    ) -> None:
+    ):
         """
         Output images of the maximum log likelihood model inferred by the model-fit. This function is called throughout
         the non-linear search at regular intervals, and therefore provides on-the-fly visualization of how well the
         model-fit is going.
 
         The visualization performed by this function includes:
 
@@ -197,15 +197,15 @@
             The result of fitting the model to the imaging dataset, via a non-linear search.
         """
         return ResultQuantity(samples=samples, model=model, analysis=self)
 
     def save_attributes_for_aggregator(self, paths: af.DirectoryPaths):
         """
         Before the non-linear search begins, this routine saves attributes of the `Analysis` object to the `pickles`
-        folder such that they can be load after the analysis using PyAutoFit's database and aggregator tools.
+        folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
         For this analysis, it uses the `AnalysisDataset` object's method to output the following:
 
         - The dataset's data.
         - The dataset's noise-map.
         - The settings associated with the dataset.
         - The Cosmology.
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/quantity/model/result.py` & `autogalaxy-2023.7.7.1/autogalaxy/quantity/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/quantity/model/visualizer.py` & `autogalaxy-2023.7.7.1/autogalaxy/quantity/model/visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             fit=fit,
             mat_plot_2d=mat_plot_2d,
             visuals_2d=visuals_2d,
             include_2d=self.include_2d,
         )
 
         if should_plot("subplot_fit"):
-            fit_quantity_plotter.subplot_fit_quantity()
+            fit_quantity_plotter.subplot_fit()
 
         mat_plot_2d = self.mat_plot_2d_from(subfolders="fit_quantity")
 
         fit_quantity_plotter = FitQuantityPlotter(
             fit=fit,
             mat_plot_2d=mat_plot_2d,
             visuals_2d=visuals_2d,
@@ -65,24 +65,23 @@
             model_image=should_plot("model_image"),
             residual_map=should_plot("residual_map"),
             normalized_residual_map=should_plot("normalized_residual_map"),
             chi_squared_map=should_plot("chi_squared_map"),
         )
 
         if should_plot("all_at_end_fits"):
-
             mat_plot_2d = self.mat_plot_2d_from(
                 subfolders="fit_quantity/fits", format="fits"
             )
 
-            fit_imaging_plotter = FitQuantityPlotter(
+            fit_plotter = FitQuantityPlotter(
                 fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
             )
 
-            fit_imaging_plotter.figures_2d(
+            fit_plotter.figures_2d(
                 image=True,
                 noise_map=True,
                 signal_to_noise_map=True,
                 model_image=True,
                 residual_map=True,
                 normalized_residual_map=True,
                 chi_squared_map=True,
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/quantity/plot/fit_quantity_plotters.py` & `autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/fit_quantity_plotters.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,45 +91,43 @@
         normalized_residual_map
             Whether to make a 2D plot (via `imshow`) of the normalized residual map.
         chi_squared_map
             Whether to make a 2D plot (via `imshow`) of the chi-squared map.
         """
 
         if isinstance(self.fit.dataset.data, aa.Array2D):
-
             fit_plotter = FitImagingPlotterMeta(
                 fit=self.fit,
                 get_visuals_2d=self.get_visuals_2d,
                 mat_plot_2d=self.mat_plot_2d,
                 include_2d=self.include_2d,
                 visuals_2d=self.visuals_2d,
             )
 
             fit_plotter.figures_2d(
-                image=image,
+                data=image,
                 noise_map=noise_map,
                 signal_to_noise_map=signal_to_noise_map,
                 model_image=model_image,
                 residual_map=residual_map,
                 normalized_residual_map=normalized_residual_map,
                 chi_squared_map=chi_squared_map,
             )
 
         else:
-
             fit_plotter_y = FitImagingPlotterMeta(
                 fit=self.fit.y,
                 get_visuals_2d=self.get_visuals_2d_y,
                 mat_plot_2d=self.mat_plot_2d,
                 include_2d=self.include_2d,
                 visuals_2d=self.visuals_2d,
             )
 
             fit_plotter_y.figures_2d(
-                image=image,
+                data=image,
                 noise_map=noise_map,
                 signal_to_noise_map=signal_to_noise_map,
                 model_image=model_image,
                 residual_map=residual_map,
                 normalized_residual_map=normalized_residual_map,
                 chi_squared_map=chi_squared_map,
                 suffix="_y",
@@ -140,79 +138,77 @@
                 get_visuals_2d=self.get_visuals_2d_x,
                 mat_plot_2d=self.mat_plot_2d,
                 include_2d=self.include_2d,
                 visuals_2d=self.visuals_2d,
             )
 
             fit_plotter_x.figures_2d(
-                image=image,
+                data=image,
                 noise_map=noise_map,
                 signal_to_noise_map=signal_to_noise_map,
                 model_image=model_image,
                 residual_map=residual_map,
                 normalized_residual_map=normalized_residual_map,
                 chi_squared_map=chi_squared_map,
                 suffix="_x",
             )
 
-    def subplot_fit_quantity(self):
+    def subplot_fit(self):
         """
         Standard subplot of the attributes of the plotter's `FitQuantity` object.
         """
 
         if isinstance(self.fit.dataset.data, aa.Array2D):
-
             fit_plotter = FitImagingPlotterMeta(
                 fit=self.fit,
                 get_visuals_2d=self.get_visuals_2d,
                 mat_plot_2d=self.mat_plot_2d,
                 include_2d=self.include_2d,
                 visuals_2d=self.visuals_2d,
             )
 
             fit_plotter.subplot(
-                image=True,
+                data=True,
                 signal_to_noise_map=True,
                 model_image=True,
                 residual_map=True,
                 normalized_residual_map=True,
                 chi_squared_map=True,
-                auto_filename="subplot_fit_quantity",
+                auto_filename="subplot_fit",
             )
 
         else:
-
             fit_plotter_y = FitImagingPlotterMeta(
                 fit=self.fit.y,
                 get_visuals_2d=self.get_visuals_2d_y,
                 mat_plot_2d=self.mat_plot_2d,
                 include_2d=self.include_2d,
                 visuals_2d=self.visuals_2d,
             )
 
             fit_plotter_y.subplot(
-                image=True,
+                data=True,
                 signal_to_noise_map=True,
                 model_image=True,
                 residual_map=True,
                 normalized_residual_map=True,
                 chi_squared_map=True,
-                auto_filename="subplot_fit_quantity_y",
+                auto_filename="subplot_fit_y",
             )
 
             fit_plotter_x = FitImagingPlotterMeta(
                 fit=self.fit.x,
                 get_visuals_2d=self.get_visuals_2d_x,
                 mat_plot_2d=self.mat_plot_2d,
                 include_2d=self.include_2d,
                 visuals_2d=self.visuals_2d,
             )
 
             fit_plotter_x.subplot(
-                image=True,
+                data=True,
                 signal_to_noise_map=True,
                 model_image=True,
                 residual_map=True,
                 normalized_residual_map=True,
                 chi_squared_map=True,
-                auto_filename="subplot_fit_quantity_x",
+                auto_filename="subplot_fit_x",
             )
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/util/__init__.py` & `autogalaxy-2023.7.7.1/autogalaxy/util/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,11 +15,12 @@
     inversion_imaging_util as inversion_imaging,
 )
 from autoarray.inversion.inversion.interferometer import (
     inversion_interferometer_util as inversion_interferometer,
 )
 from autoarray.operators import transformer_util as transformer
 from autoarray.util import misc_util as misc
-from autogalaxy.analysis import model_util as model
 
+from autogalaxy.analysis import model_util as model
 from autogalaxy.util import error_util as error
-from autogalaxy.util import plane_util as plane
+from autogalaxy.plane import plane_util as plane
+from autogalaxy.analysis import chaining_util as chaining
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/util/error_util.py` & `autogalaxy-2023.7.7.1/autogalaxy/util/error_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import numpy as np
 
 from autofit.non_linear.samples.pdf import quantile
 
 
 def value_median_and_error_region_via_quantile(value_list, low_limit):
-
     median_profile_1d = quantile(x=value_list, q=0.5)
     lower_profile_1d = quantile(x=value_list, q=low_limit)
     upper_profile_1d = quantile(x=value_list, q=1 - low_limit)
 
     return median_profile_1d, [lower_profile_1d, upper_profile_1d]
 
 
 def profile_1d_median_and_error_region_via_quantile(profile_1d_list, low_limit):
-
     median_profile_1d = quantile_profile_1d(profile_1d_list=profile_1d_list, q=0.5)
     lower_profile_1d = quantile_profile_1d(profile_1d_list=profile_1d_list, q=low_limit)
     upper_profile_1d = quantile_profile_1d(
         profile_1d_list=profile_1d_list, q=1 - low_limit
     )
 
     return median_profile_1d, [lower_profile_1d, upper_profile_1d]
@@ -59,13 +57,12 @@
     ValueError
         For invalid quantiles; ``q`` not in ``[0, 1]`` or dimension mismatch between ``x`` and ``weight_list``.
     """
 
     radial_quantile = np.zeros(shape=profile_1d_list[0].shape[0])
 
     for radial_index in range(profile_1d_list[0].shape[0]):
-
         radial_list = [profile_1d[radial_index] for profile_1d in profile_1d_list]
 
         radial_quantile[radial_index] = quantile(x=radial_list, q=q, weights=weights)[0]
 
     return radial_quantile
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/util/mock/mock_cosmology.py` & `autogalaxy-2023.7.7.1/autogalaxy/util/mock/mock_cosmology.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     def __init__(
         self,
         arcsec_per_kpc=0.5,
         kpc_per_arcsec=2.0,
         critical_surface_density=2.0,
         cosmic_average_density=2.0,
     ):
-
         super().__init__()
 
         self.arcsec_per_kpc = arcsec_per_kpc
         self.kpc_per_arcsec = kpc_per_arcsec
         self.critical_surface_density = critical_surface_density
         self.cosmic_average_density = cosmic_average_density
```

### Comparing `autogalaxy-2023.3.27.1/autogalaxy/util/shear_field.py` & `autogalaxy-2023.7.7.1/autogalaxy/util/shear_field.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/autogalaxy.egg-info/SOURCES.txt` & `autogalaxy-2023.7.7.1/autogalaxy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 autogalaxy/aggregator/fit_imaging.py
 autogalaxy/aggregator/fit_interferometer.py
 autogalaxy/aggregator/imaging.py
 autogalaxy/aggregator/interferometer.py
 autogalaxy/aggregator/plane.py
 autogalaxy/analysis/__init__.py
 autogalaxy/analysis/analysis.py
+autogalaxy/analysis/chaining_util.py
 autogalaxy/analysis/clump_model.py
 autogalaxy/analysis/maker.py
 autogalaxy/analysis/model_util.py
 autogalaxy/analysis/preloads.py
 autogalaxy/analysis/result.py
 autogalaxy/analysis/setup.py
 autogalaxy/analysis/visualizer.py
@@ -40,18 +41,16 @@
 autogalaxy/config/README.rst
 autogalaxy/config/general.yaml
 autogalaxy/config/grids.yaml
 autogalaxy/config/notation.yaml
 autogalaxy/config/priors/README.rst
 autogalaxy/config/priors/basis.yaml
 autogalaxy/config/priors/cosmology.yaml
-autogalaxy/config/priors/hyper_data.yaml
 autogalaxy/config/priors/point_sources.yaml
 autogalaxy/config/priors/galaxy/README.rst
-autogalaxy/config/priors/galaxy/hyper.yaml
 autogalaxy/config/priors/galaxy/redshift.yaml
 autogalaxy/config/priors/light/README.rst
 autogalaxy/config/priors/light/linear/chameleon.yaml
 autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
 autogalaxy/config/priors/light/linear/eff.yaml
 autogalaxy/config/priors/light/linear/exponential.yaml
 autogalaxy/config/priors/light/linear/exponential_core.yaml
@@ -80,30 +79,32 @@
 autogalaxy/config/priors/mass/dark/gnfw.yaml
 autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
 autogalaxy/config/priors/mass/dark/nfw.yaml
 autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
 autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
 autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
 autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
-autogalaxy/config/priors/mass/multipole/power_law_m4.yaml
+autogalaxy/config/priors/mass/point/point.yaml
+autogalaxy/config/priors/mass/point/smbh.yaml
+autogalaxy/config/priors/mass/point/smbh_binary.yaml
 autogalaxy/config/priors/mass/sheets/external_shear.yaml
 autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
 autogalaxy/config/priors/mass/stellar/chameleon.yaml
 autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
 autogalaxy/config/priors/mass/stellar/exponential.yaml
 autogalaxy/config/priors/mass/stellar/gaussian.yaml
 autogalaxy/config/priors/mass/stellar/sersic.yaml
 autogalaxy/config/priors/mass/stellar/sersic_core.yaml
 autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
 autogalaxy/config/priors/mass/total/isothermal.yaml
 autogalaxy/config/priors/mass/total/isothermal_core.yaml
-autogalaxy/config/priors/mass/total/point.yaml
 autogalaxy/config/priors/mass/total/power_law.yaml
 autogalaxy/config/priors/mass/total/power_law_broken.yaml
 autogalaxy/config/priors/mass/total/power_law_core.yaml
+autogalaxy/config/priors/mass/total/power_law_multipole.yaml
 autogalaxy/config/priors/mesh/README.rst
 autogalaxy/config/priors/mesh/delaunay.yaml
 autogalaxy/config/priors/mesh/rectangular.yaml
 autogalaxy/config/priors/mesh/voronoi.yaml
 autogalaxy/config/priors/mesh/voronoi_nn.yaml
 autogalaxy/config/priors/regularization/README.rst
 autogalaxy/config/priors/regularization/adaptive_brightness.yaml
@@ -120,27 +121,24 @@
 autogalaxy/config/visualize/plots.yaml
 autogalaxy/cosmology/__init__.py
 autogalaxy/cosmology/lensing.py
 autogalaxy/cosmology/model.py
 autogalaxy/cosmology/wrap.py
 autogalaxy/galaxy/__init__.py
 autogalaxy/galaxy/galaxy.py
-autogalaxy/galaxy/hyper.py
 autogalaxy/galaxy/redshift.py
 autogalaxy/galaxy/stellar_dark_decomp.py
 autogalaxy/galaxy/mock/__init__.py
 autogalaxy/galaxy/mock/mock_galaxy.py
 autogalaxy/galaxy/plot/__init__.py
+autogalaxy/galaxy/plot/adapt_plotters.py
 autogalaxy/galaxy/plot/galaxy_plotters.py
-autogalaxy/galaxy/plot/hyper_galaxy_plotters.py
 autogalaxy/gui/__init__.py
 autogalaxy/gui/clicker.py
 autogalaxy/gui/scribbler.py
-autogalaxy/hyper/__init__.py
-autogalaxy/hyper/hyper_data.py
 autogalaxy/imaging/__init__.py
 autogalaxy/imaging/fit_imaging.py
 autogalaxy/imaging/imaging.py
 autogalaxy/imaging/model/__init__.py
 autogalaxy/imaging/model/analysis.py
 autogalaxy/imaging/model/result.py
 autogalaxy/imaging/model/visualizer.py
@@ -156,14 +154,15 @@
 autogalaxy/interferometer/plot/__init__.py
 autogalaxy/interferometer/plot/fit_interferometer_plotters.py
 autogalaxy/operate/__init__.py
 autogalaxy/operate/deflections.py
 autogalaxy/operate/image.py
 autogalaxy/plane/__init__.py
 autogalaxy/plane/plane.py
+autogalaxy/plane/plane_util.py
 autogalaxy/plane/to_inversion.py
 autogalaxy/plane/plot/__init__.py
 autogalaxy/plane/plot/plane_plotters.py
 autogalaxy/plot/__init__.py
 autogalaxy/plot/abstract_plotters.py
 autogalaxy/plot/mass_plotter.py
 autogalaxy/plot/wrap.py
@@ -248,16 +247,18 @@
 autogalaxy/profiles/mass/dark/nfw_mcr.py
 autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
 autogalaxy/profiles/mass/dark/nfw_truncated.py
 autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
 autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
 autogalaxy/profiles/mass/mock/__init__.py
 autogalaxy/profiles/mass/mock/mock_mass_profile.py
-autogalaxy/profiles/mass/multipole/__init__.py
-autogalaxy/profiles/mass/multipole/power_law_m4.py
+autogalaxy/profiles/mass/point/__init__.py
+autogalaxy/profiles/mass/point/point.py
+autogalaxy/profiles/mass/point/smbh.py
+autogalaxy/profiles/mass/point/smbh_binary.py
 autogalaxy/profiles/mass/sheets/__init__.py
 autogalaxy/profiles/mass/sheets/external_shear.py
 autogalaxy/profiles/mass/sheets/input_deflections.py
 autogalaxy/profiles/mass/sheets/mass_sheet.py
 autogalaxy/profiles/mass/stellar/__init__.py
 autogalaxy/profiles/mass/stellar/abstract.py
 autogalaxy/profiles/mass/stellar/chameleon.py
@@ -266,33 +267,32 @@
 autogalaxy/profiles/mass/stellar/gaussian.py
 autogalaxy/profiles/mass/stellar/sersic.py
 autogalaxy/profiles/mass/stellar/sersic_core.py
 autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
 autogalaxy/profiles/mass/total/__init__.py
 autogalaxy/profiles/mass/total/isothermal.py
 autogalaxy/profiles/mass/total/isothermal_core.py
-autogalaxy/profiles/mass/total/point.py
 autogalaxy/profiles/mass/total/power_law.py
 autogalaxy/profiles/mass/total/power_law_broken.py
 autogalaxy/profiles/mass/total/power_law_core.py
+autogalaxy/profiles/mass/total/power_law_multipole.py
 autogalaxy/profiles/plot/__init__.py
 autogalaxy/profiles/plot/light_profile_plotters.py
 autogalaxy/profiles/plot/mass_profile_plotters.py
 autogalaxy/quantity/__init__.py
 autogalaxy/quantity/dataset_quantity.py
 autogalaxy/quantity/fit_quantity.py
 autogalaxy/quantity/model/__init__.py
 autogalaxy/quantity/model/analysis.py
 autogalaxy/quantity/model/result.py
 autogalaxy/quantity/model/visualizer.py
 autogalaxy/quantity/plot/__init__.py
 autogalaxy/quantity/plot/fit_quantity_plotters.py
 autogalaxy/util/__init__.py
 autogalaxy/util/error_util.py
-autogalaxy/util/plane_util.py
 autogalaxy/util/shear_field.py
 autogalaxy/util/mock/__init__.py
 autogalaxy/util/mock/mock_cosmology.py
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/_templates/custom-class-template.rst
```

### Comparing `autogalaxy-2023.3.27.1/docs/_templates/custom-class-template.rst` & `autogalaxy-2023.7.7.1/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/_templates/custom_module_template.rst` & `autogalaxy-2023.7.7.1/docs/_templates/custom_module_template.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/advanced/database.rst` & `autogalaxy-2023.7.7.1/docs/advanced/database.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/advanced/graphical.rst` & `autogalaxy-2023.7.7.1/docs/advanced/graphical.rst`

 * *Files 9% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 distribution (e.g. a Gaussian). It is the parameters of this parent distribution that are shared
 across the dataset, and these are the parameters we ultimately wish to infer to understand the global behaviour of the
 model.
 
 An example of such a model might be determining the parent distribution from which the Sersic index's of galaxies are
 drawn.
 
-A full description of graphical and hierarchical models can be found `in the graphical package of the autogalaxy_workspace <https://github.com/Jammy2211/autogalaxy_workspace/tree/release/notebooks/imaging/graphical>`_.
+A full description of graphical and hierarchical models can be found `in the graphical package of the autogalaxy_workspace <https://github.com/Jammy2211/autogalaxy_workspace/tree/release/notebooks/imaging/advanced/graphical>`_.
```

### Comparing `autogalaxy-2023.3.27.1/docs/api/data.rst` & `autogalaxy-2023.7.7.1/docs/api/data.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/galaxy.rst` & `autogalaxy-2023.7.7.1/docs/api/galaxy.rst`

 * *Files 19% similar despite different names*

```diff
@@ -23,21 +23,8 @@
 The ``Redshift`` object does not need to be used for general **PyAutoGalaxy** use.
 
 .. autosummary::
    :toctree: _autosummary
    :template: custom-class-template.rst
    :recursive:
 
-    Redshift
-
-By using a ``HyperGalaxy``, the noise-map value in the regions of the image that the galaxy is located
-are increased.
-
-This prevents over-fitting regions of the data where the model does not provide a good fit
-(e.g. where a high chi-squared is inferred).
-
-.. autosummary::
-   :toctree: _autosummary
-   :template: custom-class-template.rst
-   :recursive:
-
-   HyperGalaxy
+    Redshift
```

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/data_image_plane.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/data_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/grid_image_plane.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/grid_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_image_plane/image_plane_mesh.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/image_plane_mesh.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/data_image_plane.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/data_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/data_image_plane.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/data_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png` & `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/light.rst` & `autogalaxy-2023.7.7.1/docs/api/light.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/modeling.rst` & `autogalaxy-2023.7.7.1/docs/api/modeling.rst`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
    :recursive:
 
    UniformPrior
    GaussianPrior
    LogUniformPrior
    LogGaussianPrior
 
-Hyper
+Adapt
 -----
 
 .. currentmodule:: autogalaxy
 
 .. autosummary::
    :toctree: generated/
 
-   SetupHyper
+   SetupAdapt
```

### Comparing `autogalaxy-2023.3.27.1/docs/api/pixelization.rst` & `autogalaxy-2023.7.7.1/docs/api/pixelization.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/api/plot.rst` & `autogalaxy-2023.7.7.1/docs/api/plot.rst`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     InterferometerPlotter
     LightProfilePlotter
     LightProfilePDFPlotter
     GalaxyPlotter
     FitImagingPlotter
     FitInterferometerPlotter
     PlanePlotter
-    HyperPlotter
+    AdaptPlotter
     FitImagingPlotter
     FitInterferometerPlotter
     MultiFigurePlotter
     MultiYX1DPlotter
 
 Non-linear Search Plotters [aplt]
 ---------------------------------
```

### Comparing `autogalaxy-2023.3.27.1/docs/api/source.rst` & `autogalaxy-2023.7.7.1/docs/api/source.rst`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 .. currentmodule:: autogalaxy.profiles.mass
 
 .. autosummary::
    :toctree: _autosummary
    :template: custom-class-template.rst
    :recursive:
 
-   MultipolePowerLawM4
+   PowerLawMultipole
 
 Stellar [ag.mp]
 ---------------
 
 .. currentmodule:: autogalaxy.profiles.mass
 
 .. autosummary::
```

### Comparing `autogalaxy-2023.3.27.1/docs/conf.py` & `autogalaxy-2023.7.7.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath("."))
 
 
 def clone_repo(name: str, url: str):
-
     clone = f"git clone {url}/{name}"
     os.system(clone)
     os.system(f"pip install -r {name}/requirements.txt")
     os.system(f"rm -rf {name}/docs")
     sys.path.insert(
         0,
         os.path.abspath(f"{clone_path}/{name}"),
```

### Comparing `autogalaxy-2023.3.27.1/docs/general/citations.rst` & `autogalaxy-2023.7.7.1/docs/general/citations.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/general/configs.rst` & `autogalaxy-2023.7.7.1/docs/general/configs.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/general/credits.rst` & `autogalaxy-2023.7.7.1/docs/general/credits.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/general/likelihood_function.rst` & `autogalaxy-2023.7.7.1/docs/general/likelihood_function.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/general/model_cookbook.rst` & `autogalaxy-2023.7.7.1/docs/general/model_cookbook.rst`

 * *Files 5% similar despite different names*

```diff
@@ -184,14 +184,24 @@
     # (Assertions can only be added at the end of model composition, after all components
     # have been bright together in a `Collection`.
     model.add_assertion(model.galaxies.bulge.effective_radius > model.galaxies.disk.effective_radius)
 
     # Assert that the bulge effetive radius is below 3.0":
     model.add_assertion(model.galaxies.bulge.effective_radius < 3.0)
 
+Available Model Components
+--------------------------
+
+The light profiles, mass profiles and other components that can be used for galaxy modeling are given at the following
+API documentation pages:
+
+ - https://pyautogalaxy.readthedocs.io/en/latest/api/light.html
+ - https://pyautogalaxy.readthedocs.io/en/latest/api/mass.html
+ - https://pyautogalaxy.readthedocs.io/en/latest/api/pixelization.html
+
 JSon Outputs
 ------------
 
 After a model is composed, it can easily be output to a .json file on hard-disk in a readable structure:
 
 .. code-block:: python
```

### Comparing `autogalaxy-2023.3.27.1/docs/general/workspace.rst` & `autogalaxy-2023.7.7.1/docs/general/workspace.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 A full description of the scripts available is given on
 the `autogalaxy workspace GitHub page <https://github.com/Jammy2211/autogalaxy_workspace>`_.
 
 Config
 ------
 
-Here, you'll find the configuration files used by **PyAutoGalaxy** which customize:
+Here, you'll find the configuration files which customize:
 
     - The default settings used by every non-linear search.
     - Visualization, including the backend used by *matplotlib*.
     - The priors and notation configs associated with the light and mass profiles used for lens modeling.
     - The behaviour of different (y,x) Cartesian grids used to perform lens calculations.
     - The generaltrue config which customizes other aspects of **PyAutoGalaxy**.
 
@@ -51,8 +51,8 @@
 
 Contains the dataset's used to perform lens modeling. Example datasets using simulators included with the workspace
 are included here by default.
 
 Output
 ------
 
-The folder where lens modeling results are stored.
+The folder where  modeling results are stored.
```

### Comparing `autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_1_introduction.rst` & `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_1_introduction.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_2_modeling.rst` & `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_2_modeling.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_3_search_chaining.rst` & `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_3_search_chaining.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_4_pixelizations.rst` & `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_4_pixelizations.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/howtogalaxy/chapter_optional.rst` & `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_optional.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 Chapter: Optional
 =================
 
 This chapter contains optional tutorials expanding on different aspects of how **PyAutoGalaxy** work.
 
 The chapter contains the following tutorials:
 
-`Tutorial: Background Sky  <https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/release?filepath=notebooks/howtogalaxy/chapter_optional/tutorial_background_sky.ipynb>`_
-- Including the background sky subtraction in the model.
-
 `Tutorial: Mass Profiles  <https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/release?filepath=notebooks/howtogalaxy/chapter_optional/tutorial_mass_profiles.ipynb>`_
 - A description of mass profiles implemented in PyAutoGalaxy, which are currently only used by its child project PyAutoLens.
 
-`Tutorial: Noise-Map Scaling  <https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/release?filepath=notebooks/howtogalaxy/chapter_optional/tutorial_noise_map_scaling.ipynb>`_
-- Scaling the noise-map during a model-fit to overcome fitting complex galaxies.
-
 `Tutorial: Sub-grids  <https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/release?filepath=notebooks/howtogalaxy/chapter_optional/tutorial_sub_grids.ipynb>`_
 - Use sub-grids to perform more accurate and precise calculations.
 
 `Tutorial: Searches  <https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/release?filepath=notebooks/howtogalaxy/chapter_optional/tutorial_searches.ipynb>`_
 - Alternative non-linear searches to sample parameter space.
```

### Comparing `autogalaxy-2023.3.27.1/docs/howtogalaxy/howtogalaxy.rst` & `autogalaxy-2023.7.7.1/docs/howtogalaxy/howtogalaxy.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 - **Search Chaining** - How to fit complex lens models using non-linear search chaining.
 - **Pixelizations** - How to perform pixelized reconstructions of a galaxy.
 
 How to Tackle HowToGalaxy
 -------------------------
 
 The **HowToGalaxy** lecture series current sits at 4 chapters, and each will take a day or so to go through
-properly. You probably want to be modeling galaxies with **PyAutoGalaxy** faster than that! Furthermore, the concepts
-in the later chapters are pretty challenging, and familiarity with **PyAutoGalaxy** and modeling is desirable before
+properly. You probably want to be modeling galaxies faster than that! Furthermore, the concepts
+in the later chapters are pretty challenging, and familiarity and modeling is desirable before
 you tackle them.
 
 Therefore, we recommend that you complete chapters 1 & 2 and then apply what you've learnt to the modeling of simulated
 and real galaxy data, using the scripts found in the 'autogalaxy_workspace'. Once you're happy
 with the results and confident with your use of **PyAutoGalaxy**, you can then begin to cover the advanced functionality
 covered in chapters 3 & 4.
```

### Comparing `autogalaxy-2023.3.27.1/docs/index.rst` & `autogalaxy-2023.7.7.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 **PyAutoGalaxy** also fits interferometer data from observatories such as ALMA:
 
 |pic2|
 
 .. |pic2| image:: https://github.com/Jammy2211/PyAutoGalaxy/blob/main/paper/almacombined.png?raw=true
 
 Core features include fully automated Bayesian model-fitting of galaxy two-dimensional surface brightness profiles,
-support for imaging and interferometer datasets and comprehensive tools for simulating galaxy images. The software
+support for dataset and interferometer datasets and comprehensive tools for simulating galaxy images. The software
 places a focus on **big data** analysis, including support for hierarchical models that simultaneously fit thousands of
 galaxies, massively parallel model-fitting and an SQLite3 database that allows large suites of modeling results to be
 loaded, queried and analysed.
 
 The software comes distributed with the **HowToGalaxy** Jupyter notebook lectures, which are written assuming no
-previous knowledge about galaxy structure and teach a new user the theory and statistics required to analyse
+previous knowledge about galaxy structure and teach a new user theory and statistics required to analyse
 galaxy data. Checkout `the howtogalaxy section of
 the readthedocs <https://pyautogalaxy.readthedocs.io/en/latest/howtogalaxy/howtogalaxy.html>`_.
 
 An overview of **PyAutoGalaxy**'s core features can be found in
 the `overview section of the readthedocs <https://pyautogalaxy.readthedocs.io/en/latest/overview/lensing.html>`_.
 
 Galaxy Morphology & Structure
@@ -75,15 +75,15 @@
     import autogalaxy as ag
     import autogalaxy.plot as aplt
 
     """
     To describe the galaxy emission two-dimensional grids of (y,x) Cartesian
     coordinates are used.
     """
-    grid_2d = ag.Grid2D.uniform(
+    grid = ag.Grid2D.uniform(
         shape_native=(50, 50),
         pixel_scales=0.05,  # <- Conversion from pixel units to arc-seconds.
     )
 
     """
     The galaxy has an elliptical sersic light profile representing its bulge.
     """
@@ -118,15 +118,15 @@
         galaxies=[galaxy],
     )
 
     """
     We can use the Grid2D and Plane to perform many calculations, for example
     plotting the image of the lensed source.
     """
-    plane_plotter = aplt.PlanePlotter(plane=plane, grid=grid_2d)
+    plane_plotter = aplt.PlanePlotter(plane=plane, grid=grid)
     plane_plotter.figures_2d(image=True)
 
 
 To perform model-fitting, `PyAutoGalaxy` adopts the probabilistic programming
 language `PyAutoFit` (https://github.com/rhayes777/PyAutoFit). `PyAutoFit` allows users to compose a
 model from `LightProfile` and `Galaxy` objects, customize the model parameterization and fit it to data via a
 non-linear search (e.g., `dynesty` [@dynesty], `emcee` [@emcee], `PySwarms` [@pyswarms]). By composing a model with
@@ -139,26 +139,26 @@
     import autogalaxy as ag
 
     import os
 
     """
     Load Imaging data of the galaxy from the dataset folder of the workspace.
     """
-    imaging = ag.Imaging.from_fits(
-        image_path="/path/to/dataset/image.fits",
+    dataset = ag.Imaging.from_fits(
+        data_path="/path/to/dataset/image.fits",
         noise_map_path="/path/to/dataset/noise_map.fits",
         psf_path="/path/to/dataset/psf.fits",
         pixel_scales=0.1,
     )
 
     """
     Create a mask for the data, which we setup as a 3.0" circle.
     """
     mask = ag.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+        shape_native=dataset.shape_native, pixel_scales=dataset.pixel_scales, radius=3.0
     )
 
     """
     We model the galaxy using an Sersic LightProfile.
     """
     light_profile = ag.lp.Sersic
 
@@ -174,15 +174,15 @@
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
 
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the lens model to the data.
     """
-    analysis = ag.AnalysisImaging(dataset=masked_imaging)
+    analysis = ag.AnalysisImaging(dataset=masked_dataset)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autogalaxy-2023.3.27.1/docs/installation/conda.rst` & `autogalaxy-2023.7.7.1/docs/installation/conda.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/installation/numba.rst` & `autogalaxy-2023.7.7.1/docs/installation/numba.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Certain functionality (pixelized source reconstructions, linear light profiles) is disabled without numba installed
 because it will have too slow run-times.
 
 However, some users have experienced difficulties installing numba, meaning they have been unable to try out
 **PyAutoGalaxy** and determine if it the right software for them, before committing more time to installing numba
 successfully.
 
-For this reason, numba is an optional installation, so that users can easily experiment with **PyAutoGalaxy** and learn
+For this reason, numba is an optional installation, so that users can easily experiment and learn
 the basic API.
 
 If you do not have numba installed, you can do so via pip as follows:
 
 .. code-block:: bash
 
     pip install numba
```

### Comparing `autogalaxy-2023.3.27.1/docs/installation/overview.rst` & `autogalaxy-2023.7.7.1/docs/installation/overview.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ========
 
 **PyAutoGalaxy** requires Python 3.8+ and support the Linux, MacOS and Windows operating systems.
 
 **PyAutoGalaxy** can be installed via the Python distribution `Anaconda <https://www.anaconda.com/>`_ or using
 `PyPI <https://pypi.org/>`_ to ``pip install`` **PyAutoGalaxy** into your Python distribution.
 
-We recommend Anaconda as it manages the installation of many major libraries used by **PyAutoGalaxy** (e.g. numpy, scipy,
+We recommend Anaconda as it manages the installation of many major libraries (e.g. numpy, scipy,
 matplotlib, etc.) making installation more straight forward. Windows users must use Anaconda.
 
 The installation guide for both approaches can be found at:
 
 - `Anaconda installation guide <https://pyautogalaxy.readthedocs.io/en/latest/installation/conda.html>`_
 
 - `PyPI installation guide <https://pyautogalaxy.readthedocs.io/en/latest/installation/pip.html>`_
```

### Comparing `autogalaxy-2023.3.27.1/docs/installation/pip.rst` & `autogalaxy-2023.7.7.1/docs/installation/pip.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/installation/source.rst` & `autogalaxy-2023.7.7.1/docs/installation/source.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 A large amount of **PyAutoGalaxy** functionality is contained in its parent projects:
 
 **PyAutoFit** https://github.com/rhayes777/PyAutoFit
 
 **PyAutoArray** https://github.com/Jammy2211/PyAutoArray
 
-If you wish to build from source all code used by **PyAutoGalaxy** you may need to build from source these 3 additional
+If you wish to build from source all code you may need to build from source these 3 additional
 projects. We include below instructions for building just **PyAutoGalaxy** from source or building all projects.
 
 Building Only PyAutoGalaxy
 --------------------------
 
 We upgrade pip to ensure certain libraries install:
```

### Comparing `autogalaxy-2023.3.27.1/docs/installation/troubleshooting.rst` & `autogalaxy-2023.7.7.1/docs/installation/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/bad_chi_squared_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_chi_squared_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/bad_normalized_residual_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_normalized_residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/bad_residual_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/chi_squared_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/chi_squared_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/masked_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/masked_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/model_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/model_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/noise_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/noise_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/normalized_residual_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/normalized_residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/plane_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/plane_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/psf.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/psf.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/fitting/residual_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/fitting/residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/galaxies/galaxy.png` & `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/galaxy.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/galaxies/grid_2d.png` & `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/grid_2d.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/galaxies/merging_galaxies.png` & `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/merging_galaxies.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/galaxies/plane.png` & `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/galaxies/sersic_light_profile.png` & `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/sersic_light_profile.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/galaxies/subplot_galaxies.png` & `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/subplot_galaxies.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/dirty_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/dirty_signal_to_noise.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_signal_to_noise.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/fit_dirty_images.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/fit_dirty_images.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/image_pre_ft.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/image_pre_ft.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/model_visibilities.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/model_visibilities.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/reconstruction.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/reconstruction.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/uv_wavelengths.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/uv_wavelengths.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/interferometry/visibilities.png` & `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/visibilities.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/modeling/cornerplot.png` & `autogalaxy-2023.7.7.1/docs/overview/images/modeling/cornerplot.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/modeling/image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/modeling/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/modeling/subplot_fit.png` & `autogalaxy-2023.7.7.1/docs/overview/images/modeling/subplot_fit.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/dirty_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/g_decomposed_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_decomposed_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/g_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/r_decomposed_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_decomposed_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/multiwavelength/r_image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/pixelizations/image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/pixelizations/rectangular.png` & `autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/rectangular.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/ao.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/ao.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/euclid.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/euclid.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/hst.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/hst.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/image.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/noise_map.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/noise_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/psf.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/psf.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/images/simulating/vro.png` & `autogalaxy-2023.7.7.1/docs/overview/images/simulating/vro.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_1_galaxies.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_1_galaxies.rst`

 * *Files 5% similar despite different names*

```diff
@@ -25,38 +25,38 @@
 two-dimensional Cartesian grids of (y,x) coordinates.
 
 Below, we make and plot a uniform Cartesian grid (the ``pixel_scales`` describes the conversion from pixel
 units to arc-seconds):
 
 .. code:: python
 
-    grid_2d = ag.Grid2D.uniform(
+    grid = ag.Grid2D.uniform(
         shape_native=(100, 100),
         pixel_scales=0.1,
     )
 
-    grid_2d_plotter = aplt.Grid2DPlotter(grid=grid_2d)
-    grid_2d_plotter.figure_2d()
+    grid_plotter = aplt.Grid2DPlotter(grid=grid)
+    grid_plotter.figure_2d()
 
 .. sourcecode:: python
 
     import autogalaxy as ag
 
 
-    grid_2d = ag.Grid2D.uniform(
+    grid = ag.Grid2D.uniform(
         shape_native=(100, 100),
         pixel_scales=0.1,
     )
 
-    grid_2d_plotter = aplt.Grid2DPlotter(grid=grid_2d)
-    grid_2d_plotter.figure_2d()
+    grid_plotter = aplt.Grid2DPlotter(grid=grid)
+    grid_plotter.figure_2d()
 
 This is what our ``Grid2D`` looks like:
 
-.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/galaxies/grid_2d.png
+.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/galaxies/grid.png
   :width: 400
   :alt: Alternative text
 
 Light Profiles
 --------------
 
 We will use this `Grid2D`'s coordinates to evaluate the galaxy's morphology. We therefore need analytic
@@ -76,23 +76,23 @@
     )
 
 By passing this profile a `Grid2D`, we evaluate the light at every (y,x) coordinate on the `Grid2D` and create an
 image of the `LightProfile`.
 
 .. code-block:: python
 
-    image_2d = sersic_light_profile.image_2d_from(grid=grid_2d)
+    image = sersic_light_profile.image_2d_from(grid=grid)
 
 The PyAutoGalaxy plot module provides methods for plotting objects and their properties, like
 the `LightProfile`'s image.
 
 .. code-block:: python
 
     light_profile_plotter = aplt.LightProfilePlotter(
-        light_profile=sersic_light_profile, grid=grid_2d
+        light_profile=sersic_light_profile, grid=grid
     )
     light_profile_plotter.figures_2d(image=True)
 
 The light profile's image appears as shown below:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/galaxies/sersic_light_profile.png
   :width: 400
@@ -124,23 +124,23 @@
 
     galaxy = ag.Galaxy(redshift=0.5, bulge=bulge, disk=disk)
 
 We can create an image the galaxy by passing it the 2D grid above.
 
 .. code-block:: python
 
-    image_2d = galaxy.image_2d_from(grid=grid_2d)
+    image = galaxy.image_2d_from(grid=grid)
 
 The **PyAutoGalaxy** plot module provides methods for plotting galaxies.
 
 Below, we plot its image, which is the sum of the bulge and disk components.
 
 .. code-block:: python
 
-    galaxy_plotter = aplt.GalaxyPlotter(galaxy=galaxy, grid=grid_2d)
+    galaxy_plotter = aplt.GalaxyPlotter(galaxy=galaxy, grid=grid)
     galaxy_plotter.figures_2d(image=True)
 
 The galaxy, with both a bulge and disk, appears as follows
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/galaxies/galaxy.png
   :width: 400
   :alt: Alternative text
@@ -180,17 +180,17 @@
 
 The image of the plane consists of all galaxies.
 
 **PyAutoGalaxy** plot tools allow us to plot this image or a subplot containing images of each individual galaxy.
 
 .. code-block:: python
 
-    image_2d = plane.image_2d_from(grid=grid_2d)
+    image = plane.image_2d_from(grid=grid)
 
-    plane_plotter = aplt.PlanePlotter(plane=plane, grid=grid_2d)
+    plane_plotter = aplt.PlanePlotter(plane=plane, grid=grid)
     plane_plotter.figures_2d(image=True)
     plane_plotter.subplot_galaxy_images()
 
 The plane image shows both galaxies:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/galaxies/plane.png
   :width: 400
```

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_2_fitting.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_2_fitting.rst`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 demonstrate fitting.
 
 .. code:: python
 
     dataset_name = "light_sersic"
     dataset_path = path.join("dataset", "imaging", dataset_name)
 
-    imaging = ag.Imaging.from_fits(
-        image_path=path.join(dataset_path, "image.fits"),
+    dataset = ag.Imaging.from_fits(
+        data_path=path.join(dataset_path, "data.fits"),
         psf_path=path.join(dataset_path, "psf.fits"),
         noise_map_path=path.join(dataset_path, "noise_map.fits"),
         pixel_scales=0.1,
     )
 
-    imaging_plotter = aplt.ImagingPlotter(imaging=imaging)
-    imaging_plotter.figures_2d(image=True, noise_map=True, psf=True)
+    dataset_plotter = aplt.ImagingPlotter(dataset=dataset)
+    dataset_plotter.figures_2d(image=True, noise_map=True, psf=True)
 
 Here's what our ``image``, ``noise_map`` and ``psf`` (point-spread function) look like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/fitting/image.png
   :width: 400
   :alt: Alternative text
 
@@ -47,22 +47,22 @@
 
 We next mask the data, so that regions where there is no signal (e.g. the edges) are omitted from the fit.
 
 To do this we can use a ``Mask2D`` object, which for this example we'll create as a 3.0" circle.
 
 .. code-block:: python
 
-    mask_2d = ag.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+    mask = ag.Mask2D.circular(
+        shape_native=dataset.shape_native, pixel_scales=dataset.pixel_scales, radius=3.0
     )
 
-    imaging = imaging.apply_mask(mask=mask_2d)
+    dataset = dataset.apply_mask(mask=mask)
 
-    imaging_plotter = aplt.ImagingPlotter(imaging=imaging)
-    imaging_plotter.figures_2d(image=True)
+    dataset_plotter = aplt.ImagingPlotter(dataset=dataset)
+    dataset_plotter.figures_2d(image=True)
 
 Here is what our image looks like with the mask applied, where **PyAutoGalaxy** has automatically zoomed around the
 ``Mask2D`` to make the lensed source appear bigger:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/fitting/masked_image.png
   :width: 400
   :alt: Alternative text
@@ -97,18 +97,18 @@
 
 The fit performs the necessary tasks to create the `model_image` we fit the data with, such as blurring the plane`s
 image with the `Imaging` Point Spread Function (PSF). We can see this by comparing the plane`s image (which isn't PSF
 convolved) and the fit`s model image (which is).
 
 .. code-block:: python
 
-    fit = ag.FitImaging(dataset=imaging, plane=plane)
+    fit = ag.FitImaging(dataset=dataset, plane=plane)
 
-    fit_imaging_plotter = aplt.FitImagingPlotter(fit=fit)
-    fit_imaging_plotter.figures_2d(model_image=True)
+    fit_plotter = aplt.FitImagingPlotter(fit=fit)
+    fit_plotter.figures_2d(model_image=True)
 
 Here is how the ``Plane``'s image of the galaxy and the ``FitImaging``'s model-image look.
 
 Note how the model-image has been blurred with the PSF of our dataset:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/fitting/plane_image.png
   :width: 400
@@ -124,17 +124,17 @@
  - The `normalized_residual_map`: The `residual_map `divided by the observed dataset's `noise_map`.
  - The `chi_squared_map`: The `normalized_residual_map` squared.
 
 We can plot all three of these quantities
 
 .. code-block:: python
 
-    fit_imaging_plotter = aplt.FitImagingPlotter(fit=fit)
+    fit_plotter = aplt.FitImagingPlotter(fit=fit)
 
-    fit_imaging_plotter.figures_2d(
+    fit_plotter.figures_2d(
         residual_map=True,
         normalized_residual_map=True,
         chi_squared_map=True
     )
 
 For a good model where the model image and plane are representative of the galaxy system the
 residuals, normalized residuals and chi-squared are minimized:
```

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_3_modeling.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_3_modeling.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   :alt: Alternative text
 
 The task of finding these ``LightProfiles``'is called *modeling*.
 
 PyAutoFit
 ---------
 
-Modeling with **PyAutoGalaxy** uses the probabilistic programming language
+Modeling uses the probabilistic programming language
 `PyAutoFit <https://github.com/rhayes777/PyAutoFit>`_, an open-source Python framework that allows complex model
 fitting techniques to be straightforwardly integrated into scientific modeling software. Check it out if you
 are interested in developing your own software to perform advanced model-fitting!
 
 We import it separately to **PyAutoGalaxy**
 
 .. code-block:: python
@@ -114,15 +114,15 @@
 --------
 
 We next create an ``AnalysisImaging`` object, which contains the ``log likelihood function`` that the non-linear
 search calls to fit the lens model to the data.
 
 .. code-block:: python
 
-    analysis = ag.AnalysisImaging(dataset=imaging)
+    analysis = ag.AnalysisImaging(dataset=dataset)
 
 Model-Fit
 ---------
 
 To perform the model-fit we pass the model and analysis to the search's fit method. This will output results (e.g.,
 dynesty samples, model parameters, visualization) to hard-disk.
 
@@ -273,16 +273,16 @@
     print()
 
 **PyAutoGalaxy** includes many visualization tools for plotting the results of a non-linear search, for example we can
 make a corner plot of the probability density function (PDF):
 
 .. code-block:: python
 
-    dynesty_plotter = aplt.DynestyPlotter(samples=result.samples)
-    dynesty_plotter.cornerplot()
+    search_plotter = aplt.DynestyPlotter(samples=result.samples)
+    search_plotter.cornerplot()
 
 Here is an example of how a PDF estimated for a model appears:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/modeling/cornerplot.png
   :width: 600
   :alt: Alternative text
 
@@ -290,16 +290,16 @@
 plotted.
 
 .. code-block:: python
 
     plane_plotter = aplt.PlanePlotter(plane=result.max_log_likelihood_plane, grid=mask.derive_grid.masked)
     plane_plotter.subplot_plane()
 
-    fit_imaging_plotter = aplt.FitImagingPlotter(fit=result.max_log_likelihood_fit)
-    fit_imaging_plotter.subplot_fit_imaging()
+    fit_plotter = aplt.FitImagingPlotter(fit=result.max_log_likelihood_fit)
+    fit_plotter.subplot_fit()
 
 Here's what the model-fit of the model which maximizes the log likelihood looks like, providing good residuals and
 low chi-squared values:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/modeling/subplot_fit.png
   :width: 600
   :alt: Alternative text
```

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_4_simulate.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_4_simulate.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 Simulating galaxy images uses a `SimulatorImaging` object, which models the process that an instrument like the
 Hubble Space Telescope goes through to observe a galaxy. This includes accounting for the exposure time to
 determine the signal-to-noise of the data, blurring the observed light of the galaxy with the telescope optics
 and accounting for the background sky in the exposure which adds Poisson noise.
 
 .. code-block:: python
 
-    psf_2d = ag.Kernel2D.from_gaussian(shape_native=(11, 11), sigma=0.1, pixel_scales=0.05)
+    psf = ag.Kernel2D.from_gaussian(shape_native=(11, 11), sigma=0.1, pixel_scales=0.05)
 
     simulator = ag.SimulatorImaging(
-        exposure_time=300.0, background_sky_level=1.0, psf=psf_2d, add_poisson_noise=True
+        exposure_time=300.0, background_sky_level=1.0, psf=psf, add_poisson_noise=True
     )
 
 Once we have a simulator, we can use it to create an imaging dataset which consists of an image, noise-map and
 Point Spread Function (PSF) by passing it a plane and grid.
 
 .. code-block:: python
 
-    imaging = simulator.via_plane_from(plane=plane, grid=grid_2d)
+    dataset = simulator.via_plane_from(plane=plane, grid=grid)
 
 Here is what our dataset looks like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/simulating/image.png
   :width: 400
   :alt: Alternative text
```

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_5_pixelizations.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_5_pixelizations.rst`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 -------------------
 
 To fit this image with an ``Inversion``, we first mask the ``Imaging`` object:
 
 .. code-block:: python
 
    mask = al.Mask2D.circular(
-      shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+      shape_native=dataset.shape_native, pixel_scales=dataset.pixel_scales, radius=3.0
     )
 
-   imaging = imaging.apply_mask(mask=mask_2d)
+   dataset = dataset.apply_mask(mask=mask)
 
 To reconstruct the galaxy on a pixel-grid, called a mesh, we simply pass it the ``Mesh`` class we want to reconstruct its
 light on.
 
 We also pass a ``Regularization`` scheme which applies a smoothness prior on the source reconstruction.
 
 Below, we use a ``Rectangular`` pixelization with resolution 50 x 50 and a ``Constant`` regularization scheme:
@@ -46,15 +46,15 @@
 same way as before, by simply passing the galaxy to a `Plane` and using this `Plane` to create a `FitImaging`
 object.
 
 .. code-block:: python
 
     plane = ag.Plane(galaxies=[galaxy])
 
-    fit = ag.FitImaging(dataset=imaging, plane=plane)
+    fit = ag.FitImaging(dataset=dataset, plane=plane)
 
 Here is what our reconstructed galaxy looks like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/pixelizations/rectangular.png
   :width: 400
   :alt: Alternative text
 
@@ -77,15 +77,15 @@
 with the inversion so as to ensure they do not impact the fit.
 
 The workspace contains examples of how to do this, as well as other uses for pixelizations.
 
 Wrap-Up
 -------
 
-This was a brief overview of ``Inverion``'s with **PyAutoGalaxy**.
+This was a brief overview of ``Inverion``'s.
 
 There is a lot more to using ``Inverion``'s then presented here, which is covered in chapters 4 of the **HowToGalaxy**,
 specifically:
 
  - How the inversion's reconstruction determines the flux-values of the galaxy it reconstructs.
  - The Bayesian framework employed to choose the appropriate level of `Regularization` and avoid overfitting noise.
  - Unphysical model solutions that often arise when using an `Inversion`.
```

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_6_interferometry.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_6_interferometry.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 
 To begin, we define a real-space mask. Although interferometer analysis is performed in the uv-plane and
 therefore Fourier space, we still need to define the grid of coordinates in real-space from which the galaxy's
 images are computed. It is this image that is mapped to Fourier space to compare to the uv-plane data.
 
 .. code-block:: python
 
-    real_space_mask_2d = ag.Mask2D.circular(
+    real_space_mask = ag.Mask2D.circular(
         shape_native=(400, 400), pixel_scales=0.025, radius=3.0
     )
 
 Interferometer Data
 -------------------
 
 We next load an ``Interferometer`` dataset from fits files, which follows the same API that we have seen
 for an ``Imaging`` object.
 
 .. code-block:: python
 
     dataset_path = "/path/to/dataset/folder"
 
-    interferometer = ag.Interferometer.from_fits(
-        visibilities_path=path.join(dataset_path, "visibilities.fits"),
+    dataset = ag.Interferometer.from_fits(
+        data_path=path.join(dataset_path, "data.fits"),
         noise_map_path=path.join(dataset_path, "noise_map.fits"),
         uv_wavelengths_path=path.join(dataset_path, "uv_wavelengths.fits"),
-        real_space_mask=real_space_mask_2d,
+        real_space_mask=real_space_mask,
     )
 
-    interferometer_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
-    interferometer_plotter.figures_2d(visibilities=True, uv_wavelengths=True)
+    dataset_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
+    dataset_plotter.figures_2d(visibilities=True, uv_wavelengths=True)
 
 Here is what the interferometer visibilities and uv wavelength (which represent the interferometer's baselines) looks
 like.
 
-.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/visibilities.png
+.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/data.png
   :width: 400
   :alt: Alternative text
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/uv_wavelengths.png
   :width: 400
   :alt: Alternative text
 
@@ -58,16 +58,16 @@
 
 We discuss below how **PyAutoGalaxy** can scale up to large visibilities datasets from an instrument like ALMA.
 
 This can also plot the dataset in real-space, using the fast Fourier transforms described below.
 
 .. code-block:: python
 
-    interferometer_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
-    interferometer_plotter.figures_2d(dirty_image=True, dirty_signal_to_noise_map=True)
+    dataset_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
+    dataset_plotter.figures_2d(dirty_image=True, dirty_signal_to_noise_map=True)
 
 Here is what the image and signal-to-noise map look like in real space:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/dirty_image.png
   :width: 400
   :alt: Alternative text
 
@@ -99,15 +99,15 @@
     transformer_class = ag.TransformerNUFFT
 
 To perform a fit, we follow the same process we did for imaging. We do not need to mask an interferometer dataset,
 but we will apply the settings above:
 
 .. code-block:: python
 
-    interferometer = interferometer.apply_settings(
+    dataset = dataset.apply_settings(
         settings=ag.SettingsInterferometer(transformer_class=transformer_class)
     )
 
 Fitting
 -------
 
 Visualization of the fit can be performed in the uv-plane or in real-space.
@@ -116,28 +116,28 @@
 
 .. code-block:: python
 
     fit = ag.FitInterferometer(
         interferometer=interferometer, tracer=tracer
     )
 
-    fit_interferometer_plotter = aplt.FitInterferometerPlotter(fit=fit)
-    fit_interferometer_plotter.subplot_fit_interferometer()
-    fit_interferometer_plotter.subplot_fit_dirty_images()
-    fit_interferometer_plotter.subplot_fit_real_space()
+    fit_plotter = aplt.FitInterferometerPlotter(fit=fit)
+    fit_plotter.subplot_fit()
+    fit_plotter.subplot_fit_dirty_images()
+    fit_plotter.subplot_fit_real_space()
 
 Here is what the image of the galaxy looks like before it is Fourier transformed to the uv-plane:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/image_pre_ft.png
   :width: 400
   :alt: Alternative text
 
 And here is what the Fourier transformed model visibilities look like:
 
-.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/model_visibilities.png
+.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/model_data.png
   :width: 400
   :alt: Alternative text
 
 Here is what the fit of the galaxy looks like in real space (which is computed via a FFT from the uv-plane):
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoGalaxy/main/docs/overview/images/interferometry/fit_dirty_images.png
   :width: 400
@@ -186,39 +186,39 @@
     galaxy = af.Model(ag.Galaxy, redshift=0.5, bulge=ag.lp.Sersic)
 
     galaxies = af.Collection(galaxy=galaxy)
     model = af.Collection(galaxies=galaxies)
 
     search = af.DynestyStatic(name="overview_interferometer")
 
-    analysis = ag.AnalysisInterferometer(dataset=interferometer)
+    analysis = ag.AnalysisInterferometer(dataset=dataset)
 
     result = search.fit(model=model, analysis=analysis)
 
 Simulations
 -----------
 
 Simulated interferometer datasets can be generated using the ``SimulatorInterferometer`` object, which includes adding
 Gaussian noise to the visibilities:
 
 .. code-block:: python
 
-    real_space_grid_2d = ag.Grid2D.uniform(
+    real_space_grid = ag.Grid2D.uniform(
         shape_native=real_space_mask.shape_native,
         pixel_scales=real_space_mask.pixel_scales
     )
 
     simulator = ag.SimulatorInterferometer(
         uv_wavelengths=uv_wavelengths,
         exposure_time=300.0,
         background_sky_level=1.0,
         noise_sigma=0.01,
     )
 
-    interferometer = simulator.via_plane_from(plane=plane, grid=real_space_grid)
+    dataset = simulator.via_plane_from(plane=plane, grid=real_space_grid)
 
 Wrap-Up
 -------
 
 The `interferometer <https://github.com/Jammy2211/autogalaxy_workspace/tree/release/notebooks/interferometer>`_ package
 of the `autogalaxy_workspace <https://github.com/Jammy2211/autogalaxy_workspace>`_ contains numerous example scripts for performing
 interferometer modeling and simulating galaxy interferometer datasets.
```

### Comparing `autogalaxy-2023.3.27.1/docs/overview/overview_7_multi_wavelength.rst` & `autogalaxy-2023.7.7.1/docs/overview/overview_7_multi_wavelength.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 Multi-wavelength imaging datasets do not use any new objects or class in **PyAutoGalaxy**.
 
 We simply use lists of the classes we are now familiar with, for example the `Imaging` class.
 
 .. code-block:: python
 
-    imaging_list = [
+    dataset_list = [
         al.Imaging.from_fits(
             image_path=path.join(dataset_path, f"{color}_image.fits"),
             psf_path=path.join(dataset_path, f"{color}_psf.fits"),
             noise_map_path=path.join(dataset_path, f"{color}_noise_map.fits"),
             pixel_scales=pixel_scales,
         )
         for color, pixel_scales in zip(color_list, pixel_scales_list)
@@ -64,29 +64,29 @@
 define and use to set up the `Imaging` object that the galaxy model fits.
 
 For multi-wavelength galaxy modeling, we use the same mask for every dataset whenever possible. This is not absolutely
 necessary, but provides a more reliable analysis.
 
 .. code-block:: python
 
-    mask_2d_list = [
+    mask_list = [
         al.Mask2D.circular(
-            shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+            shape_native=dataset.shape_native, pixel_scales=dataset.pixel_scales, radius=3.0
         )
-        for imaging in imaging_list
+        for dataset in dataset_list
     ]
 
 Analysis
 --------
 
 We create a list of ``AnalysisImaging`` objects for every dataset.
 
 .. code-block:: python
 
-    analysis_list = [al.AnalysisImaging(dataset=imaging) for imaging in imaging_list]
+    analysis_list = [al.AnalysisImaging(dataset=dataset) for dataset in dataset_list]
 
 We now introduce the key new aspect to the **PyAutoGalaxy** multi-dataset API, which is critical to fitting multiple
 datasets simultaneously.
 
 We sum the list of analysis objects to create an overall `CombinedAnalysis` object, which we can use to fit the
 multi-wavelength imaging data, where:
 
@@ -199,20 +199,20 @@
     wavelength_list = [464, 658, 806]
 
     analysis_list = []
 
     bulge_m = af.UniformPrior(lower_limit=-0.1, upper_limit=0.1)
     bulge_c = af.UniformPrior(lower_limit=-10.0, upper_limit=10.0)
 
-    for wavelength, imaging in zip(wavelength_list, imaging_list):
+    for wavelength, imaging in zip(wavelength_list, dataset_list):
 
         bulge_intensity = (wavelength * bulge_m) + bulge_c
 
         analysis_list.append(
-            ag.AnalysisImaging(dataset=imaging).with_model(
+            ag.AnalysisImaging(dataset=dataset).with_model(
                 model.replacing(
                     {
                         model.galaxies.galaxy.bulge.intensity: bulge_intensity,
                     }
                 )
             )
         )
```

### Comparing `autogalaxy-2023.3.27.1/files/citations.bib` & `autogalaxy-2023.7.7.1/files/citations.bib`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/citations.md` & `autogalaxy-2023.7.7.1/files/citations.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/citations.tex` & `autogalaxy-2023.7.7.1/files/citations.tex`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/dirty_image.png` & `autogalaxy-2023.7.7.1/files/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/model_dirty_image.png` & `autogalaxy-2023.7.7.1/files/model_dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/non_parametric.png` & `autogalaxy-2023.7.7.1/files/non_parametric.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/observed.png` & `autogalaxy-2023.7.7.1/files/observed.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/parametric.png` & `autogalaxy-2023.7.7.1/files/parametric.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/files/visibilities.png` & `autogalaxy-2023.7.7.1/files/visibilities.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/paper/almacombined.png` & `autogalaxy-2023.7.7.1/paper/almacombined.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/paper/hstcombined.png` & `autogalaxy-2023.7.7.1/paper/hstcombined.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/paper/observed.pdf` & `autogalaxy-2023.7.7.1/paper/observed.pdf`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/paper/paper.bib` & `autogalaxy-2023.7.7.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/paper/paper.json` & `autogalaxy-2023.7.7.1/paper/paper.json`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/paper/paper.md` & `autogalaxy-2023.7.7.1/paper/paper.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 # Summary
 
 Nearly a century ago, Edwin Hubble famously classified galaxies into three distinct groups: ellipticals, spirals and 
 irregulars [@Hubble1926]. Today, by analysing millions of galaxies with advanced image processing techniques Astronomers have 
 expanded on this picture and revealed the rich diversity of galaxy morphology in both the nearby and distant 
 Universe [@Kormendy2015a; @Vulcani2014; @VanDerWel2012]. `PyAutoGalaxy` is an open-source Python 3.8+ package 
 for analysing the morphologies and structures of large multiwavelength galaxy samples, with core features including 
-fully automated Bayesian model-fitting of galaxy two-dimensional surface brightness profiles, support for imaging and 
+fully automated Bayesian model-fitting of galaxy two-dimensional surface brightness profiles, support for dataset and 
 interferometer datasets and comprehensive tools for simulating galaxy images. The software places a focus 
 on big data analysis, including support for hierarchical models that simultaneously fit thousands of galaxies, 
 massively parallel model-fitting and an SQLite3 database that allows large suites of modeling results to be loaded, 
 queried and analysed. Accompanying `PyAutoGalaxy` is the [autogalaxy workspace](https://github.com/Jammy2211/autogalaxy_workspace), 
 which includes example scripts, datasets and the `HowToGalaxy` lectures in Jupyter notebook format which introduce 
 non-experts to studies of galaxy morphology using `PyAutoGalaxy`. Readers can try `PyAutoGalaxy` right now by going 
 to [the introduction Jupyter notebook on Binder](https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/release) or
```

### Comparing `autogalaxy-2023.3.27.1/paper/parametric.png` & `autogalaxy-2023.7.7.1/paper/parametric.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.3.27.1/setup.py` & `autogalaxy-2023.7.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.3.27.1")
+version = environ.get("VERSION", "2023.7.7.1")
 requirements.extend(
     [f"autoconf=={version}", f"autoarray=={version}", f"autofit=={version}"]
 )
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
-    for (path, directories, filenames) in os.walk(directory):
+    for path, directories, filenames in os.walk(directory):
         for directory in directories:
             paths.append(f"{path}/{directory}".replace("/", "."))
     return paths
 
 
 setup(
     name="autogalaxy",
```

### Comparing `autogalaxy-2023.3.27.1/zenodo.json` & `autogalaxy-2023.7.7.1/zenodo.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9398148148148149%*

 * *Differences: {"'related_identifiers'": "{0: {'identifier': "*

 * *                          "'https://github.com/Jammy2211/PyAutoGalaxy/tree/2023.7.7.1'}}",*

 * * "'version'": "'2023.7.7.1'"}*

```diff
@@ -55,21 +55,21 @@
         }
     ],
     "description": "Release which is tied to the publication of PyAutoGalaxy in the Journal of Open Source software (JOSS).",
     "license": "other-open",
     "publication_date": "2023-01-19",
     "related_identifiers": [
         {
-            "identifier": "https://github.com/Jammy2211/PyAutoGalaxy/tree/2023.3.27.1",
+            "identifier": "https://github.com/Jammy2211/PyAutoGalaxy/tree/2023.7.7.1",
             "relation": "isSupplementTo",
             "scheme": "url"
         },
         {
             "identifier": "10.5281/zenodo.7546914",
             "relation": "isVersionOf",
             "scheme": "doi"
         }
     ],
     "title": "PyAutoGalaxy: Open-Source Multiwavelength Galaxy Structure & Morphology",
     "upload_type": "software",
-    "version": "2023.3.27.1"
+    "version": "2023.7.7.1"
 }
```

