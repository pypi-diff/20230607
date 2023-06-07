# Comparing `tmp/autolens-2023.3.27.1.tar.gz` & `tmp/autolens-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autolens-2023.3.27.1.tar", last modified: Mon Mar 27 14:49:20 2023, max compression
+gzip compressed data, was "autolens-2023.7.7.2.tar", last modified: Wed Jun  7 09:59:22 2023, max compression
```

## Comparing `autolens-2023.3.27.1.tar` & `autolens-2023.7.7.2.tar`

### file list

```diff
@@ -1,273 +1,272 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.619319 autolens-2023.3.27.1/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        2 2023-01-29 10:55:28.000000 autolens-2023.3.27.1/.gitattributes
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.150810 autolens-2023.3.27.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.198810 autolens-2023.3.27.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3309 2022-12-19 16:37:24.000000 autolens-2023.3.27.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2022-12-19 11:17:33.000000 autolens-2023.3.27.1/CITATIONS.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18883 2022-12-19 11:17:33.000000 autolens-2023.3.27.1/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/CONTRIBUTING.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2020-11-17 10:41:26.000000 autolens-2023.3.27.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      382 2022-11-28 11:07:42.000000 autolens-2023.3.27.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8683 2023-03-27 14:49:20.619319 autolens-2023.3.27.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7908 2023-01-29 10:51:28.000000 autolens-2023.3.27.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.205810 autolens-2023.3.27.1/autolens/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5784 2023-03-27 14:42:00.000000 autolens-2023.3.27.1/autolens/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.214810 autolens-2023.3.27.1/autolens/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      687 2022-04-18 12:22:28.000000 autolens-2023.3.27.1/autolens/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4648 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/autolens/aggregator/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4496 2022-08-18 12:34:54.000000 autolens-2023.3.27.1/autolens/aggregator/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1501 2022-04-17 17:51:02.000000 autolens-2023.3.27.1/autolens/aggregator/subhalo.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2634 2022-04-18 12:05:11.000000 autolens-2023.3.27.1/autolens/aggregator/tracer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.232810 autolens-2023.3.27.1/autolens/analysis/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/analysis/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18271 2023-03-06 20:55:49.000000 autolens-2023.3.27.1/autolens/analysis/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-04-16 11:29:26.000000 autolens-2023.3.27.1/autolens/analysis/maker.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.236810 autolens-2023.3.27.1/autolens/analysis/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/analysis/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4631 2022-11-25 10:19:22.000000 autolens-2023.3.27.1/autolens/analysis/mock/mock_result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13131 2022-12-20 17:11:01.000000 autolens-2023.3.27.1/autolens/analysis/positions.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14718 2023-03-13 11:43:07.000000 autolens-2023.3.27.1/autolens/analysis/preloads.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15062 2023-02-20 18:27:08.000000 autolens-2023.3.27.1/autolens/analysis/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      450 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/autolens/analysis/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8008 2023-03-06 20:55:49.000000 autolens-2023.3.27.1/autolens/analysis/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12379 2022-05-01 15:05:31.000000 autolens-2023.3.27.1/autolens/analysis/visualizer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        4 2020-11-17 10:41:26.000000 autolens-2023.3.27.1/autolens/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.241810 autolens-2023.3.27.1/autolens/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       52 2023-02-20 16:58:21.000000 autolens-2023.3.27.1/autolens/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1524 2022-12-05 10:32:56.000000 autolens-2023.3.27.1/autolens/config/non_linear.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      517 2022-12-05 10:29:07.000000 autolens-2023.3.27.1/autolens/config/visualize.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2098 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/autolens/exc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4410 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.247810 autolens-2023.3.27.1/autolens/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15136 2023-02-20 17:37:19.000000 autolens-2023.3.27.1/autolens/imaging/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4985 2022-10-28 11:04:48.000000 autolens-2023.3.27.1/autolens/imaging/imaging.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.251810 autolens-2023.3.27.1/autolens/imaging/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/imaging/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      897 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/autolens/imaging/mock/mock_fit_imaging.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.262811 autolens-2023.3.27.1/autolens/imaging/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/imaging/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23976 2023-03-22 15:54:31.000000 autolens-2023.3.27.1/autolens/imaging/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3135 2023-02-20 19:12:23.000000 autolens-2023.3.27.1/autolens/imaging/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4345 2023-02-20 17:33:08.000000 autolens-2023.3.27.1/autolens/imaging/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.266810 autolens-2023.3.27.1/autolens/imaging/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/imaging/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18303 2023-03-03 11:54:07.000000 autolens-2023.3.27.1/autolens/imaging/plot/fit_imaging_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.272810 autolens-2023.3.27.1/autolens/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12878 2022-12-21 17:22:44.000000 autolens-2023.3.27.1/autolens/interferometer/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3713 2022-10-28 11:04:48.000000 autolens-2023.3.27.1/autolens/interferometer/interferometer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.280809 autolens-2023.3.27.1/autolens/interferometer/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/interferometer/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27703 2022-12-21 17:22:44.000000 autolens-2023.3.27.1/autolens/interferometer/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4958 2023-02-20 18:27:08.000000 autolens-2023.3.27.1/autolens/interferometer/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5752 2022-09-28 16:57:53.000000 autolens-2023.3.27.1/autolens/interferometer/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.285810 autolens-2023.3.27.1/autolens/interferometer/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/interferometer/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12859 2023-01-26 17:02:36.000000 autolens-2023.3.27.1/autolens/interferometer/plot/fit_interferometer_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.294810 autolens-2023.3.27.1/autolens/lens/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/autolens/lens/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.300810 autolens-2023.3.27.1/autolens/lens/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/lens/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      490 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/autolens/lens/mock/mock_to_inversion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1704 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/autolens/lens/mock/mock_tracer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.304809 autolens-2023.3.27.1/autolens/lens/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/lens/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14558 2023-01-26 17:02:36.000000 autolens-2023.3.27.1/autolens/lens/plot/ray_tracing_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25603 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/lens/ray_tracing.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6610 2022-07-16 16:37:21.000000 autolens-2023.3.27.1/autolens/lens/ray_tracing_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12221 2023-01-14 17:32:56.000000 autolens-2023.3.27.1/autolens/lens/subhalo.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9314 2022-12-21 13:17:54.000000 autolens-2023.3.27.1/autolens/lens/to_inversion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      459 2022-04-15 18:27:13.000000 autolens-2023.3.27.1/autolens/mock.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.308810 autolens-2023.3.27.1/autolens/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3815 2023-03-21 17:50:46.000000 autolens-2023.3.27.1/autolens/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-11-11 15:50:09.000000 autolens-2023.3.27.1/autolens/plot/abstract_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.314809 autolens-2023.3.27.1/autolens/plot/get_visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:50:09.000000 autolens-2023.3.27.1/autolens/plot/get_visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-11 15:50:09.000000 autolens-2023.3.27.1/autolens/plot/get_visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7342 2023-03-18 15:58:24.000000 autolens-2023.3.27.1/autolens/plot/get_visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.320810 autolens-2023.3.27.1/autolens/point/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/point/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.334810 autolens-2023.3.27.1/autolens/point/fit_point/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/point/fit_point/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4191 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/point/fit_point/fluxes.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3317 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/point/fit_point/max_separation.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2536 2022-07-16 16:37:21.000000 autolens-2023.3.27.1/autolens/point/fit_point/point_dataset.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1524 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/point/fit_point/point_dict.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3683 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/point/fit_point/positions_image.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3421 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/point/fit_point/positions_source.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.337810 autolens-2023.3.27.1/autolens/point/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/point/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      289 2022-03-12 15:33:01.000000 autolens-2023.3.27.1/autolens/point/mock/mock_point_solver.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.343810 autolens-2023.3.27.1/autolens/point/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/point/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3838 2022-11-25 13:51:48.000000 autolens-2023.3.27.1/autolens/point/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      351 2023-02-20 18:27:08.000000 autolens-2023.3.27.1/autolens/point/model/result.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.349812 autolens-2023.3.27.1/autolens/point/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/point/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3598 2023-01-23 15:17:28.000000 autolens-2023.3.27.1/autolens/point/plot/fit_point_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5920 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/point/plot/point_dataset_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6792 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/point/point_dataset.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27225 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/autolens/point/point_solver.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.352810 autolens-2023.3.27.1/autolens/quantity/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/quantity/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1715 2022-10-16 15:04:29.000000 autolens-2023.3.27.1/autolens/quantity/fit_quantity.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.357811 autolens-2023.3.27.1/autolens/quantity/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/autolens/quantity/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7448 2022-12-15 14:06:33.000000 autolens-2023.3.27.1/autolens/quantity/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2383 2023-02-20 18:27:08.000000 autolens-2023.3.27.1/autolens/quantity/model/result.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.359810 autolens-2023.3.27.1/autolens/util/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1344 2022-09-27 20:21:13.000000 autolens-2023.3.27.1/autolens/util/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.618319 autolens-2023.3.27.1/autolens.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7682 2023-03-27 14:49:20.000000 autolens-2023.3.27.1/autolens.egg-info/SOURCES.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.363810 autolens-2023.3.27.1/docs/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.367812 autolens-2023.3.27.1/docs/_templates/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autolens-2023.3.27.1/docs/_templates/custom-class-template.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autolens-2023.3.27.1/docs/_templates/custom_module_template.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.376811 autolens-2023.3.27.1/docs/advanced/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      387 2022-04-17 15:21:49.000000 autolens-2023.3.27.1/docs/advanced/chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6434 2022-11-25 13:51:48.000000 autolens-2023.3.27.1/docs/advanced/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1365 2022-04-18 16:40:35.000000 autolens-2023.3.27.1/docs/advanced/graphical.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      482 2021-02-08 21:32:13.000000 autolens-2023.3.27.1/docs/advanced/hyper_mode.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      502 2023-01-14 16:37:15.000000 autolens-2023.3.27.1/docs/advanced/slam.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.393810 autolens-2023.3.27.1/docs/api/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1627 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/docs/api/data.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      307 2022-12-20 17:31:51.000000 autolens-2023.3.27.1/docs/api/fitting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1119 2022-12-20 17:07:16.000000 autolens-2023.3.27.1/docs/api/galaxy.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-14 14:59:54.000000 autolens-2023.3.27.1/docs/api/light.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1719 2022-12-16 19:28:40.000000 autolens-2023.3.27.1/docs/api/mass.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1350 2022-12-20 17:38:01.000000 autolens-2023.3.27.1/docs/api/modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-14 15:52:09.000000 autolens-2023.3.27.1/docs/api/pixelization.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3173 2022-12-20 18:07:50.000000 autolens-2023.3.27.1/docs/api/plot.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      281 2022-12-14 15:52:09.000000 autolens-2023.3.27.1/docs/api/point.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      744 2022-12-15 16:03:11.000000 autolens-2023.3.27.1/docs/api/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4790 2022-12-24 17:58:25.000000 autolens-2023.3.27.1/docs/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.409810 autolens-2023.3.27.1/docs/general/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2022-12-19 11:17:33.000000 autolens-2023.3.27.1/docs/general/citations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1023 2022-11-27 17:16:09.000000 autolens-2023.3.27.1/docs/general/configs.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1313 2021-08-21 09:36:01.000000 autolens-2023.3.27.1/docs/general/credits.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7996 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/general/demagnified_solutions.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.416810 autolens-2023.3.27.1/docs/general/images/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   294534 2022-07-16 16:37:21.000000 autolens-2023.3.27.1/docs/general/images/maresca_fig1.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   544260 2022-07-16 16:37:21.000000 autolens-2023.3.27.1/docs/general/images/maresca_fig2.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   202096 2022-07-16 16:37:21.000000 autolens-2023.3.27.1/docs/general/images/maresca_fig7.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      979 2022-05-03 11:39:22.000000 autolens-2023.3.27.1/docs/general/likelihood_function.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13040 2023-03-26 14:21:08.000000 autolens-2023.3.27.1/docs/general/model_cookbook.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4512 2023-01-30 09:44:27.000000 autolens-2023.3.27.1/docs/general/papers.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2729 2022-12-05 10:29:07.000000 autolens-2023.3.27.1/docs/general/workspace.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.429810 autolens-2023.3.27.1/docs/howtolens/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2528 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/docs/howtolens/chapter_1_introduction.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2305 2022-08-01 13:03:47.000000 autolens-2023.3.27.1/docs/howtolens/chapter_2_lens_modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1831 2022-04-18 16:40:35.000000 autolens-2023.3.27.1/docs/howtolens/chapter_3_search_chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2110 2023-03-20 16:05:11.000000 autolens-2023.3.27.1/docs/howtolens/chapter_4_pixelizations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1696 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/docs/howtolens/chapter_5_hyper_mode.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      657 2021-08-21 09:36:11.000000 autolens-2023.3.27.1/docs/howtolens/chapter_optional.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4117 2022-05-21 16:51:05.000000 autolens-2023.3.27.1/docs/howtolens/howtolens.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10511 2023-03-26 14:01:04.000000 autolens-2023.3.27.1/docs/index.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.440810 autolens-2023.3.27.1/docs/installation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3972 2022-12-15 09:24:56.000000 autolens-2023.3.27.1/docs/installation/conda.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3525 2022-07-21 10:03:11.000000 autolens-2023.3.27.1/docs/installation/numba.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2466 2022-09-30 11:20:01.000000 autolens-2023.3.27.1/docs/installation/overview.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3410 2022-12-15 09:24:56.000000 autolens-2023.3.27.1/docs/installation/pip.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5007 2022-12-15 09:24:56.000000 autolens-2023.3.27.1/docs/installation/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2840 2023-01-14 16:37:15.000000 autolens-2023.3.27.1/docs/installation/troubleshooting.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.457810 autolens-2023.3.27.1/docs/overview/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.175943 autolens-2023.3.27.1/docs/overview/images/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.459809 autolens-2023.3.27.1/docs/overview/images/clusters/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   318153 2021-08-21 09:36:01.000000 autolens-2023.3.27.1/docs/overview/images/clusters/cluster.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.491810 autolens-2023.3.27.1/docs/overview/images/fitting/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    72357 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/bad_chi_squared_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   111397 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/bad_normalized_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    98136 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/bad_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    91304 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/chi_squared_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    54590 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    61586 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/masked_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    64844 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/model_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    76236 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/noise_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   124025 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/normalized_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30348 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/psf.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113085 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   375168 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/subplot_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57718 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/fitting/tracer_image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.493810 autolens-2023.3.27.1/docs/overview/images/groups/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97053 2021-08-21 09:36:01.000000 autolens-2023.3.27.1/docs/overview/images/groups/image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.521319 autolens-2023.3.27.1/docs/overview/images/interferometry/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41942 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/chi_squared_map_imag.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46412 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/chi_squared_map_real.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140414 2022-04-18 16:53:09.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   123013 2022-04-18 16:53:09.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/dirty_signal_to_noise.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   541388 2022-04-18 16:03:47.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/fit_dirty_images.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97404 2022-04-18 16:55:25.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/image_pre_ft.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45276 2022-04-18 16:03:46.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/model_visibilities.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41124 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/residual_map_imag.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45680 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/residual_map_real.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-04-18 16:53:09.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/uv_wavelengths.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30858 2022-04-18 16:53:09.000000 autolens-2023.3.27.1/docs/overview/images/interferometry/visibilities.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.544321 autolens-2023.3.27.1/docs/overview/images/lensing/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    59062 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/complex_source.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28199 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/grid.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43370 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_convergence.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50440 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_deflections_x.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50354 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_deflections_y.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50181 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_potential.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   400067 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/schematic.jpg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32399 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/sersic_light_profile.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    58721 2020-11-11 17:15:07.000000 autolens-2023.3.27.1/docs/overview/images/lensing/tracer_image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.546319 autolens-2023.3.27.1/docs/overview/images/modeling/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1516307 2021-08-21 09:36:01.000000 autolens-2023.3.27.1/docs/overview/images/modeling/cornerplot.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.556319 autolens-2023.3.27.1/docs/overview/images/multiwavelength/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    88546 2022-04-22 12:33:05.000000 autolens-2023.3.27.1/docs/overview/images/multiwavelength/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49979 2022-04-22 12:34:38.000000 autolens-2023.3.27.1/docs/overview/images/multiwavelength/g_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38512 2022-04-22 12:34:38.000000 autolens-2023.3.27.1/docs/overview/images/multiwavelength/r_image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.572319 autolens-2023.3.27.1/docs/overview/images/pixelizations/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    70438 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/pixelizations/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    66987 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/pixelizations/reconstructed_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   124125 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/pixelizations/rectangular.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   289664 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/pixelizations/voronoi.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   911846 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/pixelizations/voronoi_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   463891 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/pixelizations/voronoi_fit_plane_1.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.575319 autolens-2023.3.27.1/docs/overview/images/point_sources/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36445 2021-08-21 09:36:01.000000 autolens-2023.3.27.1/docs/overview/images/point_sources/image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.592319 autolens-2023.3.27.1/docs/overview/images/simulating/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   196067 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/ao_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35458 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/euclid_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56736 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/hst_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48477 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    70333 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/noise_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30341 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/psf.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33987 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/docs/overview/images/simulating/vro_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5857 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_10_clusters.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9914 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_1_lensing.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5598 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_2_fitting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22996 2023-03-26 13:14:29.000000 autolens-2023.3.27.1/docs/overview/overview_3_modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3112 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_4_simulate.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4256 2022-12-19 12:25:36.000000 autolens-2023.3.27.1/docs/overview/overview_5_pixelizations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8689 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_6_interferometry.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11287 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_7_multi_wavelength.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7667 2023-01-13 16:58:19.000000 autolens-2023.3.27.1/docs/overview/overview_8_point_sources.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4582 2022-12-19 12:25:37.000000 autolens-2023.3.27.1/docs/overview/overview_9_groups.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-12-14 15:52:59.000000 autolens-2023.3.27.1/docs/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2022-04-26 16:24:37.000000 autolens-2023.3.27.1/eden.ini
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.607319 autolens-2023.3.27.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29343 2023-03-03 11:54:07.000000 autolens-2023.3.27.1/files/citations.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1787 2023-01-28 10:33:10.000000 autolens-2023.3.27.1/files/citations.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2398 2023-01-28 10:34:47.000000 autolens-2023.3.27.1/files/citations.tex
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    87075 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/files/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   395739 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/files/imageaxis.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   363152 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/files/imagenoaxis.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75357 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/files/model_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   202826 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/files/reconstruction.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      176 2020-11-17 10:41:27.000000 autolens-2023.3.27.1/libraries.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      109 2022-12-15 09:24:56.000000 autolens-2023.3.27.1/optional_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:49:20.616319 autolens-2023.3.27.1/paper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      188 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/paper/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   395739 2020-11-11 17:15:08.000000 autolens-2023.3.27.1/paper/imageaxis.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75921 2023-03-03 11:54:07.000000 autolens-2023.3.27.1/paper/paper.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      826 2022-02-14 09:21:43.000000 autolens-2023.3.27.1/paper/paper.json
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14346 2022-09-30 11:20:01.000000 autolens-2023.3.27.1/paper/paper.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2022-10-10 12:28:19.000000 autolens-2023.3.27.1/readthedocs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      545 2021-02-12 14:30:10.000000 autolens-2023.3.27.1/release.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-05-03 10:57:57.000000 autolens-2023.3.27.1/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-03-27 14:49:20.620319 autolens-2023.3.27.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2017 2023-03-27 14:45:03.000000 autolens-2023.3.27.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3552 2022-12-08 17:52:44.000000 autolens-2023.3.27.1/to_do_list
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.715563 autolens-2023.7.7.2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        2 2023-01-29 10:55:28.000000 autolens-2023.7.7.2/.gitattributes
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.212536 autolens-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.259528 autolens-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3309 2022-12-19 16:37:24.000000 autolens-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2022-12-19 11:17:33.000000 autolens-2023.7.7.2/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18883 2022-12-19 11:17:33.000000 autolens-2023.7.7.2/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2020-11-17 10:41:26.000000 autolens-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      382 2022-11-28 11:07:42.000000 autolens-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8654 2023-06-07 09:59:22.714568 autolens-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7880 2023-06-04 13:24:21.000000 autolens-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.267527 autolens-2023.7.7.2/autolens/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5693 2023-06-07 09:57:30.000000 autolens-2023.7.7.2/autolens/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.278528 autolens-2023.7.7.2/autolens/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      687 2023-05-11 09:41:21.000000 autolens-2023.7.7.2/autolens/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4387 2023-06-03 09:30:52.000000 autolens-2023.7.7.2/autolens/aggregator/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4396 2023-06-03 09:30:27.000000 autolens-2023.7.7.2/autolens/aggregator/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1501 2023-06-03 09:30:52.000000 autolens-2023.7.7.2/autolens/aggregator/subhalo.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2602 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/autolens/aggregator/tracer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.295528 autolens-2023.7.7.2/autolens/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18281 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/autolens/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-04-16 11:29:26.000000 autolens-2023.7.7.2/autolens/analysis/maker.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.299528 autolens-2023.7.7.2/autolens/analysis/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/analysis/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4143 2023-06-05 20:15:31.000000 autolens-2023.7.7.2/autolens/analysis/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13123 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/analysis/positions.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12889 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/analysis/preloads.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15030 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/analysis/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      448 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/analysis/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1121 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/autolens/analysis/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12590 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/analysis/visualizer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        2 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.302528 autolens-2023.7.7.2/autolens/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       52 2023-02-20 16:58:21.000000 autolens-2023.7.7.2/autolens/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1524 2022-12-05 10:32:56.000000 autolens-2023.7.7.2/autolens/config/non_linear.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.304527 autolens-2023.7.7.2/autolens/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6526 2023-04-29 16:48:45.000000 autolens-2023.7.7.2/autolens/config/visualize/plots.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2099 2023-03-30 11:03:14.000000 autolens-2023.7.7.2/autolens/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4402 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.309527 autolens-2023.7.7.2/autolens/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12978 2023-06-03 08:43:24.000000 autolens-2023.7.7.2/autolens/imaging/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4985 2023-06-03 08:43:51.000000 autolens-2023.7.7.2/autolens/imaging/imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.313526 autolens-2023.7.7.2/autolens/imaging/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/imaging/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      897 2022-08-01 13:03:47.000000 autolens-2023.7.7.2/autolens/imaging/mock/mock_fit_imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.321527 autolens-2023.7.7.2/autolens/imaging/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/imaging/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22133 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/imaging/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3135 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/autolens/imaging/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4431 2023-06-03 08:35:51.000000 autolens-2023.7.7.2/autolens/imaging/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.325527 autolens-2023.7.7.2/autolens/imaging/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/imaging/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21770 2023-06-03 16:20:05.000000 autolens-2023.7.7.2/autolens/imaging/plot/fit_imaging_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.331527 autolens-2023.7.7.2/autolens/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11508 2023-06-05 20:15:31.000000 autolens-2023.7.7.2/autolens/interferometer/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3711 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/interferometer/interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.342528 autolens-2023.7.7.2/autolens/interferometer/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/interferometer/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23148 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/interferometer/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2754 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/interferometer/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5483 2023-06-03 09:05:20.000000 autolens-2023.7.7.2/autolens/interferometer/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.349530 autolens-2023.7.7.2/autolens/interferometer/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/interferometer/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15248 2023-06-03 16:54:40.000000 autolens-2023.7.7.2/autolens/interferometer/plot/fit_interferometer_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.366528 autolens-2023.7.7.2/autolens/lens/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/autolens/lens/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.373527 autolens-2023.7.7.2/autolens/lens/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/lens/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      486 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/lens/mock/mock_to_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1698 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/lens/mock/mock_tracer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.378528 autolens-2023.7.7.2/autolens/lens/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/lens/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14835 2023-04-30 10:34:18.000000 autolens-2023.7.7.2/autolens/lens/plot/ray_tracing_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24526 2023-05-15 18:35:29.000000 autolens-2023.7.7.2/autolens/lens/ray_tracing.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6602 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/lens/ray_tracing_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12096 2023-06-03 09:37:39.000000 autolens-2023.7.7.2/autolens/lens/subhalo.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9280 2023-05-13 12:14:38.000000 autolens-2023.7.7.2/autolens/lens/to_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      459 2022-04-15 18:27:13.000000 autolens-2023.7.7.2/autolens/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.383529 autolens-2023.7.7.2/autolens/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3808 2023-06-03 09:03:18.000000 autolens-2023.7.7.2/autolens/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-11-11 15:50:09.000000 autolens-2023.7.7.2/autolens/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.392528 autolens-2023.7.7.2/autolens/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:50:09.000000 autolens-2023.7.7.2/autolens/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-11 15:50:09.000000 autolens-2023.7.7.2/autolens/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7666 2023-06-03 17:45:21.000000 autolens-2023.7.7.2/autolens/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.399527 autolens-2023.7.7.2/autolens/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/point/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.414528 autolens-2023.7.7.2/autolens/point/fit_point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/point/fit_point/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4187 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/fluxes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3317 2023-01-13 16:58:19.000000 autolens-2023.7.7.2/autolens/point/fit_point/max_separation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2522 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/point_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1522 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/point_dict.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3681 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/positions_image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3415 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/positions_source.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.418528 autolens-2023.7.7.2/autolens/point/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/point/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      287 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/mock/mock_point_solver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.424528 autolens-2023.7.7.2/autolens/point/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/point/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3832 2023-06-03 08:44:08.000000 autolens-2023.7.7.2/autolens/point/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      349 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/model/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.430527 autolens-2023.7.7.2/autolens/point/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/point/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3574 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/plot/fit_point_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5882 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/plot/point_dataset_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6786 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/point_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27183 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/point_solver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.433528 autolens-2023.7.7.2/autolens/quantity/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/quantity/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1715 2022-10-16 15:04:29.000000 autolens-2023.7.7.2/autolens/quantity/fit_quantity.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.439528 autolens-2023.7.7.2/autolens/quantity/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/quantity/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7448 2023-04-06 18:40:49.000000 autolens-2023.7.7.2/autolens/quantity/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2383 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/quantity/model/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.440528 autolens-2023.7.7.2/autolens/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1404 2023-06-04 09:51:02.000000 autolens-2023.7.7.2/autolens/util/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.713551 autolens-2023.7.7.2/autolens.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7619 2023-06-07 09:59:22.000000 autolens-2023.7.7.2/autolens.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.445527 autolens-2023.7.7.2/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.449528 autolens-2023.7.7.2/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autolens-2023.7.7.2/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autolens-2023.7.7.2/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.456527 autolens-2023.7.7.2/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      387 2022-04-17 15:21:49.000000 autolens-2023.7.7.2/docs/advanced/chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6425 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/advanced/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1374 2023-03-29 16:14:17.000000 autolens-2023.7.7.2/docs/advanced/graphical.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      502 2023-01-14 16:37:15.000000 autolens-2023.7.7.2/docs/advanced/slam.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.474527 autolens-2023.7.7.2/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1627 2023-01-13 16:58:19.000000 autolens-2023.7.7.2/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      307 2022-12-20 17:31:51.000000 autolens-2023.7.7.2/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      735 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/docs/api/galaxy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-14 14:59:54.000000 autolens-2023.7.7.2/docs/api/light.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1717 2023-05-31 17:00:51.000000 autolens-2023.7.7.2/docs/api/mass.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1350 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-14 15:52:09.000000 autolens-2023.7.7.2/docs/api/pixelization.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3173 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      281 2022-12-14 15:52:09.000000 autolens-2023.7.7.2/docs/api/point.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      744 2022-12-15 16:03:11.000000 autolens-2023.7.7.2/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4788 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.489528 autolens-2023.7.7.2/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2022-12-19 11:17:33.000000 autolens-2023.7.7.2/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1023 2022-11-27 17:16:09.000000 autolens-2023.7.7.2/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1313 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7996 2023-06-03 08:42:12.000000 autolens-2023.7.7.2/docs/general/demagnified_solutions.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.497528 autolens-2023.7.7.2/docs/general/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   294534 2022-07-16 16:37:21.000000 autolens-2023.7.7.2/docs/general/images/maresca_fig1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   544260 2022-07-16 16:37:21.000000 autolens-2023.7.7.2/docs/general/images/maresca_fig2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   202096 2022-07-16 16:37:21.000000 autolens-2023.7.7.2/docs/general/images/maresca_fig7.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      979 2022-05-03 11:39:22.000000 autolens-2023.7.7.2/docs/general/likelihood_function.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13858 2023-03-29 13:46:46.000000 autolens-2023.7.7.2/docs/general/model_cookbook.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4664 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/docs/general/papers.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2702 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.510527 autolens-2023.7.7.2/docs/howtolens/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2528 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/docs/howtolens/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2305 2022-08-01 13:03:47.000000 autolens-2023.7.7.2/docs/howtolens/chapter_2_lens_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1831 2022-04-18 16:40:35.000000 autolens-2023.7.7.2/docs/howtolens/chapter_3_search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2870 2023-06-01 19:03:35.000000 autolens-2023.7.7.2/docs/howtolens/chapter_4_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      657 2021-08-21 09:36:11.000000 autolens-2023.7.7.2/docs/howtolens/chapter_optional.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3988 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/howtolens/howtolens.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10685 2023-06-04 13:19:09.000000 autolens-2023.7.7.2/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.522527 autolens-2023.7.7.2/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3972 2022-12-15 09:24:56.000000 autolens-2023.7.7.2/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3525 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2443 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3410 2022-12-15 09:24:56.000000 autolens-2023.7.7.2/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4984 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2840 2023-01-14 16:37:15.000000 autolens-2023.7.7.2/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.542528 autolens-2023.7.7.2/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.237527 autolens-2023.7.7.2/docs/overview/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.545758 autolens-2023.7.7.2/docs/overview/images/clusters/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   318153 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/clusters/cluster.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.580527 autolens-2023.7.7.2/docs/overview/images/fitting/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    72357 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/bad_chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   111397 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/bad_normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    98136 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/bad_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    91304 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    54590 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    61586 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/masked_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    64844 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    76236 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   124025 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30348 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113085 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   375168 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/subplot_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57718 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/tracer_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.582528 autolens-2023.7.7.2/docs/overview/images/groups/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97053 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/groups/image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.611043 autolens-2023.7.7.2/docs/overview/images/interferometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41942 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/chi_squared_map_imag.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46412 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/chi_squared_map_real.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140414 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   123013 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/dirty_signal_to_noise.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   541388 2022-04-18 16:03:47.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/fit_dirty_images.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97404 2022-04-18 16:55:25.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/image_pre_ft.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45276 2022-04-18 16:03:46.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/model_visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41124 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/residual_map_imag.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45680 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/residual_map_real.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/uv_wavelengths.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30858 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/visibilities.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.635065 autolens-2023.7.7.2/docs/overview/images/lensing/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    59062 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/complex_source.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28199 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/grid.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43370 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_convergence.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50440 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_deflections_x.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50354 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_deflections_y.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50181 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_potential.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   400067 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/schematic.jpg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32399 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/sersic_light_profile.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    58721 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/tracer_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.637043 autolens-2023.7.7.2/docs/overview/images/modeling/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1516307 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/modeling/cornerplot.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.647551 autolens-2023.7.7.2/docs/overview/images/multiwavelength/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    88546 2022-04-22 12:33:05.000000 autolens-2023.7.7.2/docs/overview/images/multiwavelength/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49979 2022-04-22 12:34:38.000000 autolens-2023.7.7.2/docs/overview/images/multiwavelength/g_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38512 2022-04-22 12:34:38.000000 autolens-2023.7.7.2/docs/overview/images/multiwavelength/r_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.664551 autolens-2023.7.7.2/docs/overview/images/pixelizations/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    70438 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    66987 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/reconstructed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   124125 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/rectangular.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   289664 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   911846 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   463891 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi_fit_plane_1.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.668551 autolens-2023.7.7.2/docs/overview/images/point_sources/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36445 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/point_sources/image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.685567 autolens-2023.7.7.2/docs/overview/images/simulating/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   196067 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/ao_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35458 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/euclid_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56736 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/hst_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48477 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    70333 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30341 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33987 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/vro_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5850 2023-06-03 08:54:22.000000 autolens-2023.7.7.2/docs/overview/overview_10_clusters.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9869 2023-06-03 08:55:28.000000 autolens-2023.7.7.2/docs/overview/overview_1_lensing.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5564 2023-06-03 08:51:27.000000 autolens-2023.7.7.2/docs/overview/overview_2_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23775 2023-06-03 08:58:48.000000 autolens-2023.7.7.2/docs/overview/overview_3_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3100 2023-06-03 09:00:29.000000 autolens-2023.7.7.2/docs/overview/overview_4_simulate.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4256 2023-06-03 08:42:12.000000 autolens-2023.7.7.2/docs/overview/overview_5_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8439 2023-06-03 12:30:35.000000 autolens-2023.7.7.2/docs/overview/overview_6_interferometry.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11468 2023-06-03 09:10:23.000000 autolens-2023.7.7.2/docs/overview/overview_7_multi_wavelength.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7843 2023-06-03 09:10:24.000000 autolens-2023.7.7.2/docs/overview/overview_8_point_sources.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4579 2023-06-03 08:54:21.000000 autolens-2023.7.7.2/docs/overview/overview_9_groups.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-12-14 15:52:59.000000 autolens-2023.7.7.2/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2022-04-26 16:24:37.000000 autolens-2023.7.7.2/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.700551 autolens-2023.7.7.2/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29338 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1787 2023-01-28 10:33:10.000000 autolens-2023.7.7.2/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2398 2023-01-28 10:34:47.000000 autolens-2023.7.7.2/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    87075 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   395739 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/imageaxis.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   363152 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/imagenoaxis.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75357 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   202826 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/reconstruction.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      176 2020-11-17 10:41:27.000000 autolens-2023.7.7.2/libraries.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      111 2023-06-03 19:29:54.000000 autolens-2023.7.7.2/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.711552 autolens-2023.7.7.2/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      188 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   395739 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/paper/imageaxis.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75916 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      826 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14346 2022-09-30 11:20:01.000000 autolens-2023.7.7.2/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2022-10-10 12:28:19.000000 autolens-2023.7.7.2/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      545 2021-02-12 14:30:10.000000 autolens-2023.7.7.2/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-05-03 10:57:57.000000 autolens-2023.7.7.2/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:59:22.715563 autolens-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2014 2023-06-07 09:57:48.000000 autolens-2023.7.7.2/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3552 2022-12-08 17:52:44.000000 autolens-2023.7.7.2/to_do_list
```

### Comparing `autolens-2023.3.27.1/.github/workflows/main.yml` & `autolens-2023.7.7.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/CITATIONS.rst` & `autolens-2023.7.7.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/CODE_OF_CONDUCT.md` & `autolens-2023.7.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/CONTRIBUTING.md` & `autolens-2023.7.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/LICENSE` & `autolens-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/PKG-INFO` & `autolens-2023.7.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autolens
-Version: 2023.3.27.1
+Version: 2023.7.7.2
 Summary: Open-Source Strong Lensing
 Home-page: https://github.com/Jammy2211/PyAutoLens
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -50,19 +50,20 @@
 |binder| |RTD| |Tests| |Build| |code-style| |JOSS| |arXiv|
 
 `Installation Guide <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ |
 `readthedocs <https://pyautolens.readthedocs.io/en/latest/index.html>`_ |
 `Introduction on Binder <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=introduction.ipynb>`_ |
 `HowToLens <https://pyautolens.readthedocs.io/en/latest/howtolens/howtolens.html>`_
 
+.. image:: https://github.com/Jammy2211/PyAutoLogo/blob/main/gifs/pyautolens.gif?raw=true
+  :width: 900
+
 When two or more galaxies are aligned perfectly down our line-of-sight, the background galaxy appears multiple times.
-This is called strong gravitational lensing and **PyAutoLens** makes it simple to model strong gravitational lenses,
-like this one:
 
-.. image:: https://github.com/Jammy2211/PyAutoLens/blob/main/files/imageaxis.png?raw=true
+This is called strong gravitational lensing and **PyAutoLens** makes it simple to model strong gravitational lenses.
 
 Getting Started
 ---------------
 
 The following links are useful for new starters:
 
 - `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoLens** in a web browser (without installation).
@@ -116,76 +117,84 @@
     source_galaxy = al.Galaxy(redshift=1.0, disk=disk)
 
     """
     We create the strong lens using a Tracer, which uses the galaxies, their redshifts
     and an input cosmology to determine how light is deflected on its path to Earth.
     """
     tracer = al.Tracer.from_galaxies(
-        galaxies=[lens_galaxy, source_galaxy], cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15()
+        galaxies=[lens_galaxy, source_galaxy], 
+        cosmology = al.cosmo.Planck15()
     )
 
     """
     We can use the Grid2D and Tracer to perform many lensing calculations, for example
     plotting the image of the lensed source.
     """
     tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid)
     tracer_plotter.figures_2d(image=True)
 
 With **PyAutoLens**, you can begin modeling a lens in minutes. The example below demonstrates a simple analysis which
-fits the lens galaxy's mass with an ``Isothermal`` and the source galaxy's light with an ``Sersic``.
+fits the lens galaxy's mass with an ``Isothermal`` and the source galaxy's light with a ``Sersic``.
 
 .. code-block:: python
 
     import autofit as af
     import autolens as al
     import autolens.plot as aplt
 
     """
     Load Imaging data of the strong lens from the dataset folder of the workspace.
     """
-    imaging = al.Imaging.from_fits(
-        image_path="/path/to/dataset/image.fits",
+    dataset = al.Imaging.from_fits(
+        data_path="/path/to/dataset/image.fits",
         noise_map_path="/path/to/dataset/noise_map.fits",
         psf_path="/path/to/dataset/psf.fits",
         pixel_scales=0.1,
     )
 
     """
     Create a mask for the imaging data, which we setup as a 3.0" circle, and apply it.
     """
     mask = al.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+        shape_native=dataset.shape_native,
+        pixel_scales=dataset.pixel_scales,
+        radius=3.0
     )
-    imaging = imaging.apply_mask(mask=mask)
+    dataset = dataset.apply_mask(mask=mask)
 
     """
     We model the lens galaxy using an elliptical isothermal mass profile and
     the source galaxy using an elliptical sersic light profile.
-    """
-    lens_mass_profile = al.mp.Isothermal
-    source_light_profile = al.lp.Sersic
 
-    """
     To setup these profiles as model components whose parameters are free & fitted for
-    we set up each Galaxy as a Model and define the model as a Collection of all galaxies.
+    we set up each Galaxy as a `Model` and define the model as a `Collection` of all galaxies.
     """
-    lens_galaxy_model = af.Model(al.Galaxy, redshift=0.5, mass=lens_mass_profile)
-    source_galaxy_model = af.Model(al.Galaxy, redshift=1.0, disk=source_light_profile)
-    model = af.Collection(galaxies=af.Collection(lens=lens_galaxy_model, source=source_galaxy_model))
+    # Lens:
+
+    mass = af.Model(al.mp.Isothermal)
+    lens = af.Model(al.Galaxy, redshift=0.5, mass=lens_mass_profile)
+
+    # Source:
+
+    disk = af.Model(al.lp.Sersic)
+    source = af.Model(al.Galaxy, redshift=1.0, disk=disk)
+
+    # Overall Lens Model:
+    model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
     """
     We define the non-linear search used to fit the model to the data (in this case, Dynesty).
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
 
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the lens model to the data.
     """
-    analysis = al.AnalysisImaging(dataset=imaging)
+    analysis = al.AnalysisImaging(dataset=dataset)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autolens-2023.3.27.1/README.rst` & `autolens-2023.7.7.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 |binder| |RTD| |Tests| |Build| |code-style| |JOSS| |arXiv|
 
 `Installation Guide <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ |
 `readthedocs <https://pyautolens.readthedocs.io/en/latest/index.html>`_ |
 `Introduction on Binder <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=introduction.ipynb>`_ |
 `HowToLens <https://pyautolens.readthedocs.io/en/latest/howtolens/howtolens.html>`_
 
+.. image:: https://github.com/Jammy2211/PyAutoLogo/blob/main/gifs/pyautolens.gif?raw=true
+  :width: 900
+
 When two or more galaxies are aligned perfectly down our line-of-sight, the background galaxy appears multiple times.
-This is called strong gravitational lensing and **PyAutoLens** makes it simple to model strong gravitational lenses,
-like this one:
 
-.. image:: https://github.com/Jammy2211/PyAutoLens/blob/main/files/imageaxis.png?raw=true
+This is called strong gravitational lensing and **PyAutoLens** makes it simple to model strong gravitational lenses.
 
 Getting Started
 ---------------
 
 The following links are useful for new starters:
 
 - `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoLens** in a web browser (without installation).
@@ -95,76 +96,84 @@
     source_galaxy = al.Galaxy(redshift=1.0, disk=disk)
 
     """
     We create the strong lens using a Tracer, which uses the galaxies, their redshifts
     and an input cosmology to determine how light is deflected on its path to Earth.
     """
     tracer = al.Tracer.from_galaxies(
-        galaxies=[lens_galaxy, source_galaxy], cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15()
+        galaxies=[lens_galaxy, source_galaxy], 
+        cosmology = al.cosmo.Planck15()
     )
 
     """
     We can use the Grid2D and Tracer to perform many lensing calculations, for example
     plotting the image of the lensed source.
     """
     tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid)
     tracer_plotter.figures_2d(image=True)
 
 With **PyAutoLens**, you can begin modeling a lens in minutes. The example below demonstrates a simple analysis which
-fits the lens galaxy's mass with an ``Isothermal`` and the source galaxy's light with an ``Sersic``.
+fits the lens galaxy's mass with an ``Isothermal`` and the source galaxy's light with a ``Sersic``.
 
 .. code-block:: python
 
     import autofit as af
     import autolens as al
     import autolens.plot as aplt
 
     """
     Load Imaging data of the strong lens from the dataset folder of the workspace.
     """
-    imaging = al.Imaging.from_fits(
-        image_path="/path/to/dataset/image.fits",
+    dataset = al.Imaging.from_fits(
+        data_path="/path/to/dataset/image.fits",
         noise_map_path="/path/to/dataset/noise_map.fits",
         psf_path="/path/to/dataset/psf.fits",
         pixel_scales=0.1,
     )
 
     """
     Create a mask for the imaging data, which we setup as a 3.0" circle, and apply it.
     """
     mask = al.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+        shape_native=dataset.shape_native,
+        pixel_scales=dataset.pixel_scales,
+        radius=3.0
     )
-    imaging = imaging.apply_mask(mask=mask)
+    dataset = dataset.apply_mask(mask=mask)
 
     """
     We model the lens galaxy using an elliptical isothermal mass profile and
     the source galaxy using an elliptical sersic light profile.
-    """
-    lens_mass_profile = al.mp.Isothermal
-    source_light_profile = al.lp.Sersic
 
-    """
     To setup these profiles as model components whose parameters are free & fitted for
-    we set up each Galaxy as a Model and define the model as a Collection of all galaxies.
+    we set up each Galaxy as a `Model` and define the model as a `Collection` of all galaxies.
     """
-    lens_galaxy_model = af.Model(al.Galaxy, redshift=0.5, mass=lens_mass_profile)
-    source_galaxy_model = af.Model(al.Galaxy, redshift=1.0, disk=source_light_profile)
-    model = af.Collection(galaxies=af.Collection(lens=lens_galaxy_model, source=source_galaxy_model))
+    # Lens:
+
+    mass = af.Model(al.mp.Isothermal)
+    lens = af.Model(al.Galaxy, redshift=0.5, mass=lens_mass_profile)
+
+    # Source:
+
+    disk = af.Model(al.lp.Sersic)
+    source = af.Model(al.Galaxy, redshift=1.0, disk=disk)
+
+    # Overall Lens Model:
+    model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
     """
     We define the non-linear search used to fit the model to the data (in this case, Dynesty).
     """
     search = af.DynestyStatic(name="search[example]", nlive=50)
 
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the lens model to the data.
     """
-    analysis = al.AnalysisImaging(dataset=imaging)
+    analysis = al.AnalysisImaging(dataset=dataset)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
```

### Comparing `autolens-2023.3.27.1/autolens/__init__.py` & `autolens-2023.7.7.2/autolens/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,20 @@
 from autoarray.structures.visibilities import Visibilities
 from autoarray.structures.visibilities import VisibilitiesNoiseMap
 
 from autogalaxy import cosmology as cosmo
 from autogalaxy.gui.clicker import Clicker
 from autogalaxy.gui.scribbler import Scribbler
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.galaxy.hyper import HyperGalaxy
 from autogalaxy.galaxy.redshift import Redshift
 from autogalaxy.analysis.clump_model import ClumpModel
 from autogalaxy.analysis.clump_model import ClumpModelDisabled
 
 from autogalaxy.quantity.dataset_quantity import DatasetQuantity
 from autogalaxy.quantity.dataset_quantity import SettingsQuantity
-from autogalaxy.hyper import hyper_data
 from autogalaxy.plane.plane import Plane
 from autogalaxy.profiles.geometry_profiles import EllProfile
 from autogalaxy.profiles import (
     point_sources as ps,
     mass as mp,
     light_and_mass_profiles as lmp,
     scaling_relations as sr,
@@ -85,15 +83,15 @@
 from .lens import subhalo
 from .analysis.settings import SettingsLens
 from .lens.ray_tracing import Tracer
 from .lens.to_inversion import TracerToInversion
 from .analysis.positions import PositionsLHResample
 from .analysis.positions import PositionsLHPenalty
 from .analysis.preloads import Preloads
-from .analysis.setup import SetupHyper
+from .analysis.setup import SetupAdapt
 from .imaging.imaging import SimulatorImaging
 from .imaging.fit_imaging import FitImaging
 from .imaging.model.analysis import AnalysisImaging
 from .interferometer.interferometer import SimulatorInterferometer
 from .interferometer.fit_interferometer import FitInterferometer
 from .interferometer.model.analysis import AnalysisInterferometer
 from .point.point_dataset import PointDataset
@@ -112,8 +110,8 @@
 from . import mock as m
 from . import util
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.3.27.1"
+__version__ = "2023.7.7.2"
```

### Comparing `autolens-2023.3.27.1/autolens/aggregator/__init__.py` & `autolens-2023.7.7.2/autolens/aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/aggregator/fit_imaging.py` & `autolens-2023.7.7.2/autolens/aggregator/fit_interferometer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,119 @@
 from typing import Optional, List
 
 import autofit as af
 import autoarray as aa
 import autogalaxy as ag
 
-from autogalaxy.aggregator.imaging import _imaging_from
+from autogalaxy.aggregator.interferometer import _interferometer_from
 from autogalaxy.aggregator.abstract import AbstractAgg
 
-from autolens.imaging.fit_imaging import FitImaging
+from autolens.interferometer.fit_interferometer import FitInterferometer
 from autolens.analysis.preloads import Preloads
+
 from autolens.aggregator.tracer import _tracer_from
 
 
-def _fit_imaging_from(
+def _fit_interferometer_from(
     fit: af.Fit,
     galaxies: List[ag.Galaxy],
-    settings_imaging: aa.SettingsImaging = None,
+    real_space_mask: Optional[aa.Mask2D] = None,
+    settings_dataset: aa.SettingsInterferometer = None,
     settings_pixelization: aa.SettingsPixelization = None,
     settings_inversion: aa.SettingsInversion = None,
     use_preloaded_grid: bool = True,
-    use_hyper_scaling: bool = True,
-) -> FitImaging:
+) -> FitInterferometer:
     """
-    Returns a `FitImaging` object from a PyAutoFit database `Fit` object and an instance of galaxies from a non-linear
+    Returns a `FitInterferometer` object from a PyAutoFit database `Fit` object and an instance of galaxies from a non-linear
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
-    FitImaging
-        The fit to the imaging dataset computed via an instance of galaxies.
+    FitInterferometer
+        The fit to the interferometer dataset computed via an instance of galaxies.
     """
-
-    imaging = _imaging_from(fit=fit, settings_imaging=settings_imaging)
-
+    dataset = _interferometer_from(
+        fit=fit,
+        real_space_mask=real_space_mask,
+        settings_dataset=settings_dataset,
+    )
     tracer = _tracer_from(fit=fit, galaxies=galaxies)
 
     settings_pixelization = settings_pixelization or fit.value(
         name="settings_pixelization"
     )
     settings_inversion = settings_inversion or fit.value(name="settings_inversion")
 
-    preloads = Preloads(use_w_tilde=False)
+    preloads = Preloads(use_w_tilde=settings_inversion.use_w_tilde)
 
     if use_preloaded_grid:
-
         sparse_grids_of_planes = fit.value(name="preload_sparse_grids_of_planes")
 
         if sparse_grids_of_planes is not None:
+            preloads = Preloads(sparse_image_plane_grid_pg_list=sparse_grids_of_planes)
 
-            preloads = Preloads(
-                sparse_image_plane_grid_pg_list=sparse_grids_of_planes,
-                use_w_tilde=False,
-            )
-
-            if len(preloads.sparse_image_plane_grid_pg_list) == 2:
-                if type(preloads.sparse_image_plane_grid_pg_list[1]) != list:
-                    preloads.sparse_image_plane_grid_pg_list[1] = [
-                        preloads.sparse_image_plane_grid_pg_list[1]
-                    ]
-
-    return FitImaging(
-        dataset=imaging,
+    return FitInterferometer(
+        dataset=dataset,
         tracer=tracer,
         settings_pixelization=settings_pixelization,
         settings_inversion=settings_inversion,
         preloads=preloads,
-        use_hyper_scaling=use_hyper_scaling,
     )
 
 
-class FitImagingAgg(AbstractAgg):
+class FitInterferometerAgg(AbstractAgg):
     def __init__(
         self,
         aggregator: af.Aggregator,
-        settings_imaging: Optional[aa.SettingsImaging] = None,
+        settings_dataset: Optional[aa.SettingsInterferometer] = None,
         settings_pixelization: Optional[aa.SettingsPixelization] = None,
         settings_inversion: Optional[aa.SettingsInversion] = None,
         use_preloaded_grid: bool = True,
-        use_hyper_scaling: bool = True,
+        real_space_mask: Optional[aa.Mask2D] = None,
     ):
         """
-        Wraps a PyAutoFit aggregator in order to create generators of fits to imaging data, corresponding to the
+        Wraps a PyAutoFit aggregator in order to create generators of fits to interferometer data, corresponding to the
         results of a non-linear search model-fit.
         """
         super().__init__(aggregator=aggregator)
 
-        self.settings_imaging = settings_imaging
+        self.settings_dataset = settings_dataset
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
         self.use_preloaded_grid = use_preloaded_grid
-        self.use_hyper_scaling = use_hyper_scaling
+        self.real_space_mask = real_space_mask
 
-    def make_object_for_gen(self, fit, galaxies) -> FitImaging:
+    def object_via_gen_from(self, fit, galaxies) -> FitInterferometer:
         """
-        Creates a `FitImaging` object from a `ModelInstance` that contains the galaxies of a sample from a non-linear
-        search.
+        Creates a `FitInterferometer` object from a `ModelInstance` that contains the galaxies of a sample from a
+        non-linear search.
 
         Parameters
         ----------
         fit
-            A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+            A PyAutoFit database Fit object containing the generators of the results of model-fits.
         galaxies
             A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
         Returns
         -------
-        FitImaging
-            A fit to imaging data whose galaxies are a sample of a PyAutoFit non-linear search.
+        FitInterferometer
+            A fit to interferometer data whose galaxies are a sample of a PyAutoFit non-linear search.
         """
-
-        return _fit_imaging_from(
+        return _fit_interferometer_from(
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

### Comparing `autolens-2023.3.27.1/autolens/aggregator/subhalo.py` & `autolens-2023.7.7.2/autolens/aggregator/subhalo.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from autolens import exc
 
 
 class SubhaloAgg:
     def __init__(
         self,
         aggregator_grid_search: af.GridSearchAggregator,
-        settings_imaging: Optional[aa.SettingsImaging] = None,
+        settings_dataset: Optional[aa.SettingsImaging] = None,
         settings_pixelization: Optional[aa.SettingsPixelization] = None,
         settings_inversion: Optional[aa.SettingsInversion] = None,
         use_preloaded_grid: bool = True,
     ):
         """
         Wraps a PyAutoFit aggregator in order to create generators of fits to imaging data, corresponding to the
         results of a non-linear search model-fit.
         """
 
         self.aggregator_grid_search = aggregator_grid_search
-        self.settings_imaging = settings_imaging
+        self.settings_dataset = settings_dataset
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
         self.use_preloaded_grid = use_preloaded_grid
 
         if len(aggregator_grid_search) == 0:
             raise exc.AggregatorException(
                 "There is no grid search of results in the aggregator."
```

### Comparing `autolens-2023.3.27.1/autolens/aggregator/tracer.py` & `autolens-2023.7.7.2/autolens/aggregator/tracer.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,69 +8,67 @@
 
 
 def _tracer_from(fit: af.Fit, galaxies: List[ag.Galaxy]) -> Tracer:
     """
     Returns a `Tracer` object from a PyAutoFit database `Fit` object and an instance of galaxies from a non-linear
     search model-fit.
 
-    This function adds the `hyper_model_image` and `hyper_galaxy_image_path_dict` to the galaxies before constructing
+    This function adds the `adapt_model_image` and `adapt_galaxy_image_path_dict` to the galaxies before constructing
     the `Tracer`, if they were used.
 
     Parameters
     ----------
     fit
-        A PyAutoFit database Fit object containing the generators of the results of PyAutoGalaxy model-fits.
+        A PyAutoFit database Fit object containing the generators of the results of model-fits.
     galaxies
         A list of galaxies corresponding to a sample of a non-linear search and model-fit.
 
     Returns
     -------
     Tracer
         The tracer computed via an instance of galaxies.
     """
 
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
             gal[0] for gal in fit.instance.path_instance_tuples_for_class(ag.Galaxy)
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
 
-        return Tracer.from_galaxies(galaxies=galaxies_with_hyper)
+        return Tracer.from_galaxies(galaxies=galaxies_with_adapt)
 
     return Tracer.from_galaxies(galaxies=galaxies)
 
 
 class TracerAgg(AbstractAgg):
     """
     Wraps a PyAutoFit aggregator in order to create generators of tracers corresponding to the results of a non-linear
     search model-fit.
     """
 
-    def make_object_for_gen(self, fit, galaxies) -> Tracer:
+    def object_via_gen_from(self, fit, galaxies) -> Tracer:
         """
         Creates a `Tracer` object from a `ModelInstance` that contains the galaxies of a sample from a non-linear
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
         Tracer
             A tracer whose galaxies are a sample of a PyAutoFit non-linear search.
```

### Comparing `autolens-2023.3.27.1/autolens/analysis/analysis.py` & `autolens-2023.7.7.2/autolens/analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,18 @@
             The Cosmology assumed for this analysis.
         """
         self.cosmology = cosmology
         self.settings_lens = settings_lens or SettingsLens()
         self.positions_likelihood = positions_likelihood
 
     def tracer_via_instance_from(
-        self, instance: af.ModelInstance, profiling_dict: Optional[Dict] = None
+        self,
+        instance: af.ModelInstance,
+        profiling_dict: Optional[Dict] = None,
+        tracer_cls=Tracer,
     ) -> Tracer:
         """
         Create a `Tracer` from the galaxies contained in a model instance.
 
         If PyAutoFit's profiling tools are used with the analsyis class, this function may receive a `profiling_dict`
         which times how long each set of the model-fit takes to perform.
 
@@ -87,38 +90,36 @@
         if hasattr(instance, "perturbation"):
             instance.galaxies.subhalo = instance.perturbation
 
         # TODO : Need to think about how we do this without building it into the model attribute names.
         # TODO : A Subhalo class that extends the Galaxy class maybe?
 
         if hasattr(instance.galaxies, "subhalo"):
-
             subhalo_centre = ray_tracing_util.grid_2d_at_redshift_from(
                 galaxies=instance.galaxies,
                 redshift=instance.galaxies.subhalo.redshift,
                 grid=aa.Grid2DIrregular(values=[instance.galaxies.subhalo.mass.centre]),
                 cosmology=self.cosmology,
             )
 
             instance.galaxies.subhalo.mass.centre = tuple(subhalo_centre.in_list[0])
 
         if hasattr(instance, "clumps"):
-
             return Tracer.from_galaxies(
                 galaxies=instance.galaxies + instance.clumps,
                 cosmology=self.cosmology,
                 profiling_dict=profiling_dict,
             )
 
         if hasattr(instance, "cosmology"):
             cosmology = instance.cosmology
         else:
             cosmology = self.cosmology
 
-        return Tracer.from_galaxies(
+        return tracer_cls.from_galaxies(
             galaxies=instance.galaxies,
             cosmology=cosmology,
             profiling_dict=profiling_dict,
         )
 
     def log_likelihood_positions_overwrite_from(
         self, instance: af.ModelInstance
@@ -139,15 +140,14 @@
 
         Returns
         -------
         The penalty value of the positions log likelihood, if the positions do not trace close in the source plane,
         else a None is returned to indicate there is no penalty.
         """
         if self.positions_likelihood is not None:
-
             try:
                 return self.positions_likelihood.log_likelihood_function_positions_overwrite(
                     instance=instance, analysis=self
                 )
             except (ValueError, np.linalg.LinAlgError) as e:
                 raise exc.FitException from e
 
@@ -155,15 +155,15 @@
 class AnalysisDataset(AgAnalysisDataset, AnalysisLensing):
     def __init__(
         self,
         dataset,
         positions_likelihood: Optional[
             Union[PositionsLHResample, PositionsLHPenalty]
         ] = None,
-        hyper_dataset_result=None,
+        adapt_result=None,
         cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15(),
         settings_pixelization: aa.SettingsPixelization = None,
         settings_inversion: aa.SettingsInversion = None,
         settings_lens: SettingsLens = None,
         raise_inversion_positions_likelihood_exception: bool = True,
     ):
         """
@@ -199,15 +199,15 @@
             be inferred, in which case an Exception is raised before the model-fit begins to inform the user
             of this. This exception is not raised if this input is False, allowing the user to perform the model-fit
             anyway.
         """
 
         super().__init__(
             dataset=dataset,
-            hyper_dataset_result=hyper_dataset_result,
+            adapt_result=adapt_result,
             cosmology=cosmology,
             settings_pixelization=settings_pixelization,
             settings_inversion=settings_inversion,
         )
 
         AnalysisLensing.__init__(
             self=self,
@@ -221,25 +221,24 @@
         self.preloads = self.preloads_cls()
 
         self.raise_inversion_positions_likelihood_exception = (
             raise_inversion_positions_likelihood_exception
         )
 
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-
             self.raise_inversion_positions_likelihood_exception = False
 
     def modify_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
         """
         PyAutoFit calls this function immediately before the non-linear search begins, therefore it can be used to
         perform tasks using the final model parameterization.
 
         This function:
 
-        - Checks that the hyper-dataset is consistent with previous hyper-datasets if the model-fit is being
+        - Checks that the adapt-dataset is consistent with previous adapt-datasets if the model-fit is being
           resumed from a previous run.
 
         - Checks the model and raises exceptions if certain critieria are not met.
 
         Once inherited from it also visualizes objects which do not change throughout the model fit like the dataset.
 
         Parameters
@@ -253,15 +252,14 @@
         """
 
         super().modify_before_fit(paths=paths, model=model)
 
         self.raise_exceptions(model=model)
 
     def raise_exceptions(self, model):
-
         if ag.util.model.has_pixelization_from(model=model):
             if (
                 self.positions_likelihood is None
                 and self.raise_inversion_positions_likelihood_exception
                 and not conf.instance["general"]["test"][
                     "disable_positions_lh_inversion_check"
                 ]
@@ -342,27 +340,26 @@
 
         Parameters
         ----------
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
             visualization and the pickled objects used by the aggregator output by this function.
         result
-            The result of a lens model fit, including the non-linear search, samples and maximum likelihood tracer.
+            The result of a model fit, including the non-linear search, samples and maximum likelihood tracer.
         """
 
         mesh_list = ag.util.model.mesh_list_from(model=result.model)
 
         if len(mesh_list) > 0:
-
             paths.save_object(
                 "preload_sparse_grids_of_planes",
                 result.max_log_likelihood_fit.tracer_to_inversion.sparse_image_plane_grid_pg_list,
             )
 
-        if conf.instance["general"]["hyper"]["stochastic_outputs"]:
+        if conf.instance["general"]["adapt"]["stochastic_outputs"]:
             if len(mesh_list) > 0:
                 for mesh in mesh_list:
                     if mesh.is_stochastic:
                         self.save_stochastic_outputs(
                             paths=paths, samples=result.samples
                         )
```

### Comparing `autolens-2023.3.27.1/autolens/analysis/mock/mock_result.py` & `autolens-2023.7.7.2/autolens/analysis/mock/mock_result.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,42 +10,37 @@
         analysis=None,
         search=None,
         mask=None,
         model_image=None,
         max_log_likelihood_tracer=None,
         max_log_likelihood_fit=None,
         max_log_likelihood_mesh_grids_of_planes=None,
-        hyper_galaxy_image_path_dict=None,
-        hyper_model_image=None,
-        hyper_galaxy_visibilities_path_dict=None,
-        hyper_model_visibilities=None,
+        adapt_galaxy_image_path_dict=None,
+        adapt_model_image=None,
         pixelization=None,
         positions=None,
         updated_positions=None,
         updated_positions_threshold=None,
         stochastic_log_likelihoods=None,
     ):
-
         super().__init__(
             samples=samples,
             instance=instance,
             model=model,
             analysis=analysis,
             search=search,
         )
 
         self._model = model
         self.gaussian_tuples = None
         self.mask = None
         self.positions = None
         self.mask = mask
-        self.hyper_galaxy_image_path_dict = hyper_galaxy_image_path_dict
-        self.hyper_model_image = hyper_model_image
-        self.hyper_galaxy_visibilities_path_dict = hyper_galaxy_visibilities_path_dict
-        self.hyper_model_visibilities = hyper_model_visibilities
+        self.adapt_galaxy_image_path_dict = adapt_galaxy_image_path_dict
+        self.adapt_model_image = adapt_model_image
         self.model_image = model_image
         self.unmasked_model_image = model_image
         self.max_log_likelihood_tracer = max_log_likelihood_tracer
         self.max_log_likelihood_fit = max_log_likelihood_fit
         self.max_log_likelihood_mesh_grids_of_planes = (
             max_log_likelihood_mesh_grids_of_planes
         )
@@ -72,18 +67,16 @@
         instance=None,
         model=None,
         analysis=None,
         search=None,
         mask=None,
         model_image=None,
         max_log_likelihood_tracer=None,
-        hyper_galaxy_image_path_dict=None,
-        hyper_model_image=None,
-        hyper_galaxy_visibilities_path_dict=None,
-        hyper_model_visibilities=None,
+        adapt_galaxy_image_path_dict=None,
+        adapt_model_image=None,
         pixelization=None,
         positions=None,
         updated_positions=None,
         updated_positions_threshold=None,
         stochastic_log_likelihoods=None,
     ):
         """
@@ -98,18 +91,16 @@
             instance=instance,
             model=model,
             analysis=analysis,
             search=search,
             mask=mask,
             model_image=model_image,
             max_log_likelihood_tracer=max_log_likelihood_tracer,
-            hyper_galaxy_image_path_dict=hyper_galaxy_image_path_dict,
-            hyper_model_image=hyper_model_image,
-            hyper_galaxy_visibilities_path_dict=hyper_galaxy_visibilities_path_dict,
-            hyper_model_visibilities=hyper_model_visibilities,
+            adapt_galaxy_image_path_dict=adapt_galaxy_image_path_dict,
+            adapt_model_image=adapt_model_image,
             pixelization=pixelization,
             positions=positions,
             updated_positions=updated_positions,
             updated_positions_threshold=updated_positions_threshold,
             stochastic_log_likelihoods=stochastic_log_likelihoods,
         )
```

### Comparing `autolens-2023.3.27.1/autolens/analysis/positions.py` & `autolens-2023.7.7.2/autolens/analysis/positions.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,14 @@
             return
 
         positions_fit = FitPositionsSourceMaxSeparation(
             positions=self.positions, noise_map=None, tracer=tracer
         )
 
         if not positions_fit.max_separation_within_threshold(self.threshold):
-
             if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
                 return
 
             raise exc.RayTracingException
 
 
 class PositionsLHPenalty(AbstractPositionsLH):
@@ -214,27 +213,25 @@
         """
 
         residual_map = aa.util.fit.residual_map_from(
             data=dataset.data, model_data=np.zeros(dataset.data.shape)
         )
 
         if isinstance(dataset, aa.Imaging):
-
             chi_squared_map = aa.util.fit.chi_squared_map_from(
                 residual_map=residual_map, noise_map=dataset.noise_map
             )
 
             chi_squared = aa.util.fit.chi_squared_from(chi_squared_map=chi_squared_map)
 
             noise_normalization = aa.util.fit.noise_normalization_from(
                 noise_map=dataset.noise_map
             )
 
         else:
-
             chi_squared_map = aa.util.fit.chi_squared_map_complex_from(
                 residual_map=residual_map, noise_map=dataset.noise_map
             )
 
             chi_squared = aa.util.fit.chi_squared_complex_from(
                 chi_squared_map=chi_squared_map
             )
@@ -265,15 +262,14 @@
             return
 
         positions_fit = FitPositionsSourceMaxSeparation(
             positions=self.positions, noise_map=None, tracer=tracer
         )
 
         if not positions_fit.max_separation_within_threshold(self.threshold):
-
             return self.log_likelihood_penalty_factor * (
                 positions_fit.max_separation_of_source_plane_positions - self.threshold
             )
 
     def log_likelihood_function_positions_overwrite(
         self, instance: af.ModelInstance, analysis: AnalysisDataset
     ) -> Optional[float]:
```

### Comparing `autolens-2023.3.27.1/autolens/analysis/preloads.py` & `autolens-2023.7.7.2/autolens/analysis/preloads.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,18 +19,16 @@
         traced_grids_of_planes_for_inversion: Optional[aa.Grid2D] = None,
         sparse_image_plane_grid_pg_list: Optional[List[List[aa.Grid2D]]] = None,
         relocated_grid: Optional[aa.Grid2D] = None,
         mapper_list: Optional[aa.AbstractMapper] = None,
         mapper_galaxy_dict: Optional[Dict[aa.AbstractMapper, ag.Galaxy]] = None,
         operated_mapping_matrix: Optional[np.ndarray] = None,
         linear_func_operated_mapping_matrix_dict=None,
-        linear_func_weighted_mapping_vectors_dict=None,
-        linear_func_curvature_vectors_dict=None,
-        curvature_matrix_preload: Optional[np.ndarray] = None,
-        curvature_matrix_counts: Optional[np.ndarray] = None,
+        data_linear_func_matrix_dict=None,
+        mapper_operated_mapping_matrix_dict=None,
         regularization_matrix: Optional[np.ndarray] = None,
         log_det_regularization_matrix_term: Optional[float] = None,
         traced_sparse_grids_list_of_planes=None,
         sparse_image_plane_grid_list=None,
         failed=False,
     ):
         """
@@ -43,19 +41,19 @@
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
@@ -67,21 +65,14 @@
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
         Preloads
             The preloads object used to skip certain calculations in the log likelihood function.
         """
         super().__init__(
@@ -90,18 +81,16 @@
             blurred_image=blurred_image,
             relocated_grid=relocated_grid,
             sparse_image_plane_grid_pg_list=sparse_image_plane_grid_pg_list,
             mapper_list=mapper_list,
             mapper_galaxy_dict=mapper_galaxy_dict,
             operated_mapping_matrix=operated_mapping_matrix,
             linear_func_operated_mapping_matrix_dict=linear_func_operated_mapping_matrix_dict,
-            linear_func_weighted_mapping_vectors_dict=linear_func_weighted_mapping_vectors_dict,
-            linear_func_curvature_vectors_dict=linear_func_curvature_vectors_dict,
-            curvature_matrix_preload=curvature_matrix_preload,
-            curvature_matrix_counts=curvature_matrix_counts,
+            data_linear_func_matrix_dict=data_linear_func_matrix_dict,
+            mapper_operated_mapping_matrix_dict=mapper_operated_mapping_matrix_dict,
             regularization_matrix=regularization_matrix,
             log_det_regularization_matrix_term=log_det_regularization_matrix_term,
             traced_sparse_grids_list_of_planes=traced_sparse_grids_list_of_planes,
             sparse_image_plane_grid_list=sparse_image_plane_grid_list,
         )
 
         self.traced_grids_of_planes_for_inversion = traced_grids_of_planes_for_inversion
@@ -134,15 +123,14 @@
 
         preloads.set_traced_grids_of_planes_for_inversion(fit_0=fit_0, fit_1=fit_1)
         preloads.set_sparse_image_plane_grid_pg_list(fit_0=fit_0, fit_1=fit_1)
         preloads.set_relocated_grid(fit_0=fit_0, fit_1=fit_1)
         preloads.set_mapper_list(fit_0=fit_0, fit_1=fit_1)
 
         if preloads.mapper_list is not None:
-
             preloads.mapper_galaxy_dict = fit_0.tracer_to_inversion.mapper_galaxy_dict
 
         preloads.set_operated_mapping_matrix_with_preloads(fit_0=fit_0, fit_1=fit_1)
         preloads.set_linear_func_inversion_dicts(fit_0=fit_0, fit_1=fit_1)
         preloads.set_curvature_matrix(fit_0=fit_0, fit_1=fit_1)
         preloads.set_regularization_matrix_and_term(fit_0=fit_0, fit_1=fit_1)
 
@@ -153,15 +141,15 @@
         If the `MassProfiles`'s in a model are fixed their deflection angles and therefore corresponding traced grids
         do not change during the model-fit and can therefore be preloaded.
 
         This function compares the traced grids of two fit's corresponding to two model instances, and preloads the
         traced grids if the grids of both fits are the same. This preloaded grid is only used when constructing an
         inversion, because the `blurred_image` preload accounts for light profiles.
 
-        The preload is typically used in hyper searches, where the mass model is fixed and the hyper-parameters are
+        The preload is typically used in adapt searches, where the mass model is fixed and the adapt-parameters are
         varied.
 
         Parameters
         ----------
         fit_0
             The first fit corresponding to a model with a specific set of unit-values.
         fit_1
@@ -175,27 +163,24 @@
         )
 
         traced_grids_of_planes_1 = fit_1.tracer.traced_grid_2d_list_from(
             grid=fit_1.dataset.grid_pixelization
         )
 
         if traced_grids_of_planes_0[-1] is not None:
-
             if (
                 traced_grids_of_planes_0[-1].shape[0]
                 == traced_grids_of_planes_1[-1].shape[0]
             ):
-
                 if (
                     np.max(
                         abs(traced_grids_of_planes_0[-1] - traced_grids_of_planes_1[-1])
                     )
                     < 1e-8
                 ):
-
                     self.traced_grids_of_planes_for_inversion = traced_grids_of_planes_0
 
                     logger.info(
                         "PRELOADS - Traced grid of planes (for inversion) preloaded for this model-fit."
                     )
 
     def set_sparse_image_plane_grid_pg_list(self, fit_0, fit_1):
@@ -204,15 +189,15 @@
         that are ray-traced to construct the source-plane pixelization) do not change during the model=fit and
         can therefore be preloaded.
 
         This function compares the image plane sparse grid of two fit's corresponding to two model instances, and p
         reloads the grid if the grids of both fits are the same.
 
         The preload is typically used thoughout search chaining pipelines which use inversions, as it is common to
-        for the pixelization's parameters to only vary in the hyper-searches.
+        for the pixelization's parameters to only vary in the adapt-searches.
 
         Parameters
         ----------
         fit_0
             The first fit corresponding to a model with a specific set of unit-values.
         fit_1
             The second fit corresponding to a model with a different set of unit-values.
@@ -225,61 +210,36 @@
         )
 
         sparse_image_plane_grid_pg_list_1 = (
             fit_1.tracer_to_inversion.sparse_image_plane_grid_pg_list
         )
 
         if sparse_image_plane_grid_pg_list_0[-1] is not None:
-
             if sparse_image_plane_grid_pg_list_0[-1][0] is not None:
-
                 if (
                     sparse_image_plane_grid_pg_list_0[-1][0].shape[0]
                     == sparse_image_plane_grid_pg_list_1[-1][0].shape[0]
                 ):
-
                     if (
                         np.max(
                             abs(
                                 sparse_image_plane_grid_pg_list_0[-1][0]
                                 - sparse_image_plane_grid_pg_list_1[-1][0]
                             )
                         )
                         < 1e-8
                     ):
-
                         self.sparse_image_plane_grid_pg_list = (
                             sparse_image_plane_grid_pg_list_0
                         )
 
                         logger.info(
                             "PRELOADS - Sparse image-plane grids of planes is preloaded for this model-fit."
                         )
 
-    def reset_all(self):
-        """
-        Reset all preloads, typically done at the end of a model-fit to save memory.
-        """
-        self.w_tilde = None
-
-        self.blurred_image = None
-        self.traced_grids_of_planes_for_inversion = None
-        self.sparse_image_plane_grid_pg_list = None
-        self.relocated_grid = None
-        self.mapper = None
-        self.blurred_mapping_matrix = None
-        self.curvature_matrix = None
-        self.linear_func_operated_mapping_matrix_dict = None
-        self.linear_func_weighted_mapping_vectors_dict = None
-        self.linear_func_curvature_vectors_dict = None
-        self.curvature_matrix_preload = None
-        self.curvature_matrix_counts = None
-        self.regularization_matrix = None
-        self.log_det_regularization_matrix_term = None
-
     @property
     def info(self) -> List[str]:
         """
         The information on what has or has not been preloaded, which is written to the file `preloads.summary`.
 
         Returns
         -------
@@ -296,18 +256,15 @@
         ]
         line += [f"Relocated Grid = {self.relocated_grid is not None}\n"]
         line += [f"Mapper = {self.mapper_list is not None}\n"]
         line += [
             f"Blurred Mapping Matrix = {self.operated_mapping_matrix is not None}\n"
         ]
         line += [
-            f"Inversion Linear Func (Linear Light Profile) Dicts = {self.linear_func_weighted_mapping_vectors_dict is not None}\n"
-        ]
-        line += [
-            f"Curvature Matrix Sparse = {self.curvature_matrix_preload is not None}\n"
+            f"Inversion Linear Func (Linear Light Profile) Dicts = {self.linear_func_operated_mapping_matrix_dict is not None}\n"
         ]
         line += [f"Curvature Matrix = {self.curvature_matrix is not None}\n"]
         line += [
             f"Curvature Matrix Mapper Diag = {self.curvature_matrix_mapper_diag is not None}\n"
         ]
         line += [f"Regularization Matrix = {self.regularization_matrix is not None}\n"]
         line += [
```

### Comparing `autolens-2023.3.27.1/autolens/analysis/result.py` & `autolens-2023.7.7.2/autolens/analysis/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,15 +165,14 @@
     def positions_likelihood_from(
         self,
         factor=1.0,
         minimum_threshold=None,
         use_resample=False,
         positions: Optional[aa.Grid2DIrregular] = None,
     ) -> Union[PositionsLHPenalty, PositionsLHResample]:
-
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
             return None
 
         positions = (
             self.image_plane_multiple_image_positions
             if positions is None
             else positions
@@ -196,17 +195,17 @@
 
 class ResultDataset(Result):
     @property
     def max_log_likelihood_tracer(self) -> Tracer:
         """
         An instance of a `Tracer` corresponding to the maximum log likelihood model inferred by the non-linear search.
 
-        If a dataset is fitted the hyper images of the hyper dataset must first be associated with each galaxy.
+        If a dataset is fitted the adapt images of the adapt dataset must first be associated with each galaxy.
         """
-        instance = self.analysis.instance_with_associated_hyper_images_from(
+        instance = self.analysis.instance_with_associated_adapt_images_from(
             instance=self.instance_copy
         )
 
         return self.analysis.tracer_via_instance_from(instance=instance)
 
     @property
     def max_log_likelihood_fit(self):
@@ -263,18 +262,18 @@
             if self.max_log_likelihood_fit.inversion.has(cls=aa.AbstractMapper):
                 return self.max_log_likelihood_fit.inversion.brightest_reconstruction_pixel_centre_list[
                     0
                 ]
 
     def image_for_galaxy(self, galaxy: ag.Galaxy) -> np.ndarray:
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
@@ -285,62 +284,61 @@
         return self.max_log_likelihood_fit.galaxy_model_image_dict[galaxy]
 
     @property
     def image_galaxy_dict(self) -> {str: ag.Galaxy}:
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
 
     def stochastic_log_likelihoods_from(self, paths: AbstractPaths) -> np.ndarray:
         """
         Certain `Inversion`'s have stochasticity in their log likelihood estimate.
 
         For example, the `VoronoiBrightnessImage` pixelization, which changes the likelihood depending on how different
         KMeans seeds change the pixel-grid.
```

### Comparing `autolens-2023.3.27.1/autolens/analysis/visualizer.py` & `autolens-2023.7.7.2/autolens/analysis/visualizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.stats import norm
 from os import path
 import os
+from typing import Dict
 
 import autoarray as aa
 import autogalaxy.plot as aplt
 
 from autogalaxy.analysis.visualizer import plot_setting
 
 from autogalaxy.analysis.visualizer import Visualizer as AgVisualizer
@@ -66,67 +67,72 @@
             tracer=tracer,
             grid=grid,
             mat_plot_2d=mat_plot_2d,
             include_2d=self.include_2d,
         )
 
         if should_plot("subplot_ray_tracing"):
-
             tracer_plotter.subplot_tracer()
 
         if should_plot("subplot_plane_images"):
-
             tracer_plotter.subplot_plane_images()
 
         tracer_plotter.figures_2d(
             image=should_plot("image"),
             source_plane=should_plot("source_plane_image"),
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
+                subfolders=path.join("ray_tracing", "end"),
+            )
 
-                tracer_plotter.figures_2d(
-                    image=True,
-                    source_plane=True,
-                    convergence=True,
-                    potential=True,
-                    deflections_y=True,
-                    deflections_x=True,
-                    magnification=True,
-                )
+            tracer_plotter = TracerPlotter(
+                tracer=tracer,
+                grid=grid,
+                mat_plot_2d=mat_plot_2d,
+                include_2d=self.include_2d,
+            )
 
-            if should_plot("all_at_end_fits"):
+            tracer_plotter.figures_2d(
+                image=True,
+                source_plane=True,
+                convergence=True,
+                potential=True,
+                deflections_y=True,
+                deflections_x=True,
+                magnification=True,
+            )
 
-                fits_mat_plot_2d = self.mat_plot_2d_from(
-                    subfolders=path.join("ray_tracing", "fits"), format="fits"
-                )
+        if not during_analysis and should_plot("all_at_end_fits"):
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join("ray_tracing", "fits"), format="fits"
+            )
 
-                tracer_plotter = TracerPlotter(
-                    tracer=tracer,
-                    grid=grid,
-                    mat_plot_2d=fits_mat_plot_2d,
-                    include_2d=self.include_2d,
-                )
+            tracer_plotter = TracerPlotter(
+                tracer=tracer,
+                grid=grid,
+                mat_plot_2d=mat_plot_2d,
+                include_2d=self.include_2d,
+            )
 
-                tracer_plotter.figures_2d(
-                    image=True,
-                    source_plane=True,
-                    convergence=True,
-                    potential=True,
-                    deflections_y=True,
-                    deflections_x=True,
-                    magnification=True,
-                )
+            tracer_plotter.figures_2d(
+                image=True,
+                source_plane=True,
+                convergence=True,
+                potential=True,
+                deflections_y=True,
+                deflections_x=True,
+                magnification=True,
+            )
 
     def visualize_image_with_positions(
         self, image: aa.Array2D, positions: aa.Grid2DIrregular
     ):
         """
         Visualizes the positions of a model-fit, where these positions are used to resample lens models where
         the positions to do trace within an input threshold of one another in the source-plane.
@@ -161,90 +167,89 @@
                 include_2d=self.include_2d,
                 visuals_2d=visuals_2d,
             )
             image_plotter.set_filename("image_with_positions")
             if should_plot("image_with_positions"):
                 image_plotter.figure_2d()
 
-    def visualize_hyper_images(
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
 
-        hyper_plotter = aplt.HyperPlotter(
+        adapt_plotter = aplt.AdaptPlotter(
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
 
     def visualize_contribution_maps(self, tracer: Tracer):
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
         tracer
             The maximum log likelihood `Tracer` of the non-linear search which is used to plot the contribution maps.
         """
 
         def should_plot(name):
-            return plot_setting(section="hyper", name=name)
+            return plot_setting(section="adapt", name=name)
 
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="hyper")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="adapt")
 
-        hyper_plotter = aplt.HyperPlotter(
+        adapt_plotter = aplt.AdaptPlotter(
             mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         if hasattr(tracer, "contribution_map_list"):
             if should_plot("contribution_map_list"):
-                hyper_plotter.subplot_contribution_map_list(
+                adapt_plotter.subplot_contribution_map_list(
                     contribution_map_list_list=tracer.contribution_map_list
                 )
 
     def visualize_stochastic_histogram(
         self,
         stochastic_log_likelihoods: np.ndarray,
         max_log_evidence: float,
@@ -280,15 +285,14 @@
             A log likelihood cap which is applied in a stochastic model-fit to give improved error and posterior
             estimates.
         """
         if stochastic_log_likelihoods is None:
             return
 
         if plot_setting("other", "stochastic_histogram"):
-
             file_path = path.join(self.visualize_path, "other")
 
             try:
                 os.makedirs(file_path)
             except FileExistsError or IsADirectoryError:
                 pass
```

### Comparing `autolens-2023.3.27.1/autolens/config/non_linear.yaml` & `autolens-2023.7.7.2/autolens/config/non_linear.yaml`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/exc.py` & `autolens-2023.7.7.2/autolens/exc.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
 
     pass
 
 
 class PointExtractionException(Exception):
     """
-    Raises exceptions associated with the extraction of quantites in the  `point` module, where the name of a
+    Raises exceptions associated with the extraction of quantities in the  `point` module, where the name of a
     `PointSource` profile often relates to a model-component.
 
     For example if one tries to extract a profile `point_1` but there is no corresponding `PointSource` profile
     named `point_1`.
     """
 
     pass
```

### Comparing `autolens-2023.3.27.1/autolens/fixtures.py` & `autolens-2023.7.7.2/autolens/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,50 +39,46 @@
 
 
 def make_tracer_x1_plane_7x7():
     return al.Tracer.from_galaxies(galaxies=[make_gal_x1_lp()])
 
 
 def make_tracer_x2_plane_7x7():
-
     source_gal_x1_lp = al.Galaxy(redshift=1.0, light_profile_0=make_lp_0())
 
     return al.Tracer.from_galaxies(
         galaxies=[make_gal_x1_mp(), make_gal_x1_lp(), source_gal_x1_lp]
     )
 
 
 def make_tracer_x2_plane_inversion_7x7():
-
     pixelization = al.Pixelization(
         mesh=al.mesh.Rectangular(), regularization=al.reg.Constant()
     )
 
     source_gal_inversion = al.Galaxy(redshift=1.0, pixelization=pixelization)
 
     return al.Tracer.from_galaxies(
         galaxies=[make_gal_x1_mp(), make_gal_x1_lp(), source_gal_inversion]
     )
 
 
 def make_tracer_x2_plane_voronoi_7x7():
-
     pixelization = al.Pixelization(
         mesh=al.mesh.VoronoiMagnification(), regularization=al.reg.Constant()
     )
 
     source_gal_inversion = al.Galaxy(redshift=1.0, pixelization=pixelization)
 
     return al.Tracer.from_galaxies(
         galaxies=[make_gal_x1_mp(), make_gal_x1_lp(), source_gal_inversion]
     )
 
 
 def make_tracer_x2_plane_point():
-
     source_gal_x1_lp = al.Galaxy(redshift=1.0, point_0=al.ps.PointFlux())
 
     return al.Tracer.from_galaxies(
         galaxies=[make_gal_x1_mp(), make_gal_x1_lp(), source_gal_x1_lp]
     )
```

### Comparing `autolens-2023.3.27.1/autolens/imaging/fit_imaging.py` & `autolens-2023.7.7.2/autolens/imaging/fit_imaging.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,32 +4,26 @@
 from autoconf import cached_property
 
 import autoarray as aa
 import autogalaxy as ag
 
 from autogalaxy.abstract_fit import AbstractFitInversion
 
-from autogalaxy.imaging.fit_imaging import hyper_image_from
-from autogalaxy.imaging.fit_imaging import hyper_noise_map_from
-
 from autolens.analysis.preloads import Preloads
 from autolens.lens.ray_tracing import Tracer
 from autolens.lens.to_inversion import TracerToInversion
 
 from autolens import exc
 
 
 class FitImaging(aa.FitImaging, AbstractFitInversion):
     def __init__(
         self,
         dataset: aa.Imaging,
         tracer: Tracer,
-        hyper_image_sky: Optional[ag.hyper_data.HyperImageSky] = None,
-        hyper_background_noise: Optional[ag.hyper_data.HyperBackgroundNoise] = None,
-        use_hyper_scaling: bool = True,
         settings_pixelization: aa.SettingsPixelization = aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ):
         """
         Fits an imaging dataset using a `Tracer` object.
@@ -57,21 +51,14 @@
 
         Parameters
         ----------
         dataset
             The imaging dataset which is fitted by the galaxies in the tracer.
         tracer
             The tracer of galaxies whose light profile images are used to fit the imaging data.
-        hyper_image_sky
-            If included, accounts for the background sky in the fit.
-        hyper_background_noise
-            If included, adds a noise-scaling term to the background to account for an inaacurate background sky model.
-        use_hyper_scaling
-            If set to False, the hyper scaling functions (e.g. the `hyper_image_sky` / `hyper_background_noise`) are
-            omitted irrespective of their inputs.
         settings_pixelization
             Settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
@@ -84,54 +71,20 @@
         super().__init__(dataset=dataset, profiling_dict=profiling_dict)
         AbstractFitInversion.__init__(
             self=self, model_obj=tracer, settings_inversion=settings_inversion
         )
 
         self.tracer = tracer
 
-        self.hyper_image_sky = hyper_image_sky
-        self.hyper_background_noise = hyper_background_noise
-        self.use_hyper_scaling = use_hyper_scaling
-
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
 
         self.preloads = preloads
 
     @property
-    def data(self) -> aa.Array2D:
-        """
-        Returns the imaging data, which may have a hyper scaling performed which rescales the background sky level
-        in order to account for uncertainty in the background sky subtraction.
-        """
-        if self.use_hyper_scaling:
-
-            return hyper_image_from(
-                image=self.dataset.image, hyper_image_sky=self.hyper_image_sky
-            )
-
-        return self.dataset.data
-
-    @property
-    def noise_map(self) -> aa.Array2D:
-        """
-        Returns the imaging noise-map, which may have a hyper scaling performed which increase the noise in regions of
-        the data that are poorly fitted in order to avoid overfitting.
-        """
-        if self.use_hyper_scaling:
-
-            return hyper_noise_map_from(
-                noise_map=self.dataset.noise_map,
-                model_obj=self.tracer,
-                hyper_background_noise=self.hyper_background_noise,
-            )
-
-        return self.dataset.noise_map
-
-    @property
     def blurred_image(self) -> aa.Array2D:
         """
         Returns the image of all light profiles in the fit's tracer convolved with the imaging dataset's PSF.
 
         For certain lens models the blurred image does not change (for example when all light profiles in the tracer
         are fixed in the lens model). For faster run-times the blurred image can be preloaded.
         """
@@ -195,34 +148,34 @@
 
             return self.blurred_image + self.inversion.mapped_reconstructed_data
 
         return self.blurred_image
 
     @property
     def grid(self) -> aa.type.Grid2DLike:
-        return self.imaging.grid
+        return self.dataset.grid
 
     @property
     def galaxy_model_image_dict(self) -> Dict[ag.Galaxy, np.ndarray]:
         """
         A dictionary which associates every galaxy in the tracer with its `model_image`.
 
         This image is the image of the sum of:
 
         - The images of all ordinary light profiles in that plane summed and convolved with the imaging data's PSF.
         - The images of all linear objects (e.g. linear light profiles / pixelizations), where the images are solved
           for first via the inversion.
 
-        For modeling, this dictionary is used to set up the `hyper_images` that adaptmodel_images_of_planes_list certain pixelizations to the
-        data being fitted.
+        For modeling, this dictionary is used to set up the `adapt_images` that adaptmodel_images_of_planes_list
+        certain pixelizations to the data being fitted.
         """
         galaxy_blurred_image_2d_dict = self.tracer.galaxy_blurred_image_2d_dict_from(
             grid=self.grid,
-            convolver=self.imaging.convolver,
-            blurring_grid=self.imaging.blurring_grid,
+            convolver=self.dataset.convolver,
+            blurring_grid=self.dataset.blurring_grid,
         )
 
         galaxy_linear_obj_image_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=True
         )
 
         return {**galaxy_blurred_image_2d_dict, **galaxy_linear_obj_image_dict}
@@ -297,15 +250,15 @@
         Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
         image cannot be computed.
         """
         if self.tracer.has(cls=ag.lp_linear.LightProfileLinear):
             exc.raise_linear_light_profile_in_unmasked()
 
         return self.tracer.unmasked_blurred_image_2d_from(
-            grid=self.grid, psf=self.imaging.psf
+            grid=self.grid, psf=self.dataset.psf
         )
 
     @property
     def unmasked_blurred_image_of_planes_list(self) -> List[aa.Array2D]:
         """
         The blurred image of every galaxy in the tracer used in this fit, that would be evaluated without a mask being
         used.
@@ -313,15 +266,15 @@
         Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
         image cannot be computed.
         """
         if self.tracer.has(cls=ag.lp_linear.LightProfileLinear):
             exc.raise_linear_light_profile_in_unmasked()
 
         return self.tracer.unmasked_blurred_image_2d_list_from(
-            grid=self.grid, psf=self.imaging.psf
+            grid=self.grid, psf=self.dataset.psf
         )
 
     @property
     def tracer_linear_light_profiles_to_light_profiles(self) -> Tracer:
         """
         The `Tracer` where all linear light profiles have been converted to ordinary light profiles, where their
         `intensity` values are set to the values inferred by this fit.
@@ -359,17 +312,14 @@
         settings_inversion = (
             self.settings_inversion
             if settings_inversion is None
             else settings_inversion
         )
 
         return FitImaging(
-            dataset=self.imaging,
+            dataset=self.dataset,
             tracer=self.tracer,
-            hyper_image_sky=self.hyper_image_sky,
-            hyper_background_noise=self.hyper_background_noise,
-            use_hyper_scaling=self.use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=settings_inversion,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
```

### Comparing `autolens-2023.3.27.1/autolens/imaging/imaging.py` & `autolens-2023.7.7.2/autolens/imaging/imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
             background_sky_level=self.background_sky_level,
         )
 
         image = tracer.padded_image_2d_from(
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

### Comparing `autolens-2023.3.27.1/autolens/imaging/mock/mock_fit_imaging.py` & `autolens-2023.7.7.2/autolens/imaging/mock/mock_fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/imaging/model/analysis.py` & `autolens-2023.7.7.2/autolens/imaging/model/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def modify_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
         """
         PyAutoFit calls this function immediately before the non-linear search begins, therefore it can be used to
         perform tasks using the final model parameterization.
 
         This function:
 
-        - Checks that the hyper-dataset is consistent with previous hyper-datasets if the model-fit is being
+        - Checks that the adapt-dataset is consistent with previous adapt-datasets if the model-fit is being
           resumed from a previous run.
 
         - Checks the model and raises exceptions if certain critieria are not met.
 
         Once inherited from it also visualizes objects which do not change throughout the model fit like the dataset.
 
         Parameters
@@ -54,45 +54,28 @@
             The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
             the imaging data.
         """
         super().modify_before_fit(paths=paths, model=model)
 
         if not paths.is_complete:
 
-            if not os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-
-                visualizer = VisualizerImaging(visualize_path=paths.image_path)
-
-                visualizer.visualize_imaging(imaging=self.imaging)
-
-                if self.positions_likelihood is not None:
-                    visualizer.visualize_image_with_positions(
-                        image=self.imaging.image,
-                        positions=self.positions_likelihood.positions,
-                    )
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
 
         3) Extracts all galaxies from the model instance and set up a `Tracer`, which includes ordering the galaxies
            by redshift to set up each `Plane`.
@@ -144,109 +127,83 @@
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
         check_positions
             Whether the multiple image positions of the lensed source should be checked, i.e. whether they trace
             within the position threshold of one another in the source plane.
         profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitImaging
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
-        self.instance_with_associated_hyper_images_from(instance=instance)
+        self.instance_with_associated_adapt_images_from(instance=instance)
         tracer = self.tracer_via_instance_from(
             instance=instance, profiling_dict=profiling_dict
         )
 
-        hyper_image_sky = self.hyper_image_sky_via_instance_from(instance=instance)
-
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
-
         return self.fit_imaging_via_tracer_from(
             tracer=tracer,
-            hyper_image_sky=hyper_image_sky,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
             preload_overwrite=preload_overwrite,
             profiling_dict=profiling_dict,
         )
 
     def fit_imaging_via_tracer_from(
         self,
         tracer: Tracer,
-        hyper_image_sky: Optional[ag.hyper_data.HyperImageSky],
-        hyper_background_noise: Optional[ag.hyper_data.HyperBackgroundNoise],
-        use_hyper_scaling: bool = True,
         preload_overwrite: Optional[Preloads] = None,
         profiling_dict: Optional[Dict] = None,
     ) -> FitImaging:
         """
         Given a `Tracer`, which the analysis constructs from a model instance, create a `FitImaging` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
         Parameters
         ----------
         tracer
             The tracer of galaxies whose ray-traced model images are used to fit the imaging data.
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
         FitImaging
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
-        preloads = self.preloads if preload_overwrite is None else preload_overwrite
+        preloads = preload_overwrite or self.preloads
 
         return FitImaging(
             dataset=self.dataset,
             tracer=tracer,
-            hyper_image_sky=hyper_image_sky,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     @property
@@ -299,18 +256,18 @@
         info_dict["fit_time"] = fit_time
 
         fit = self.fit_imaging_via_instance_from(
             instance=instance, profiling_dict=profiling_dict
         )
         fit.figure_of_merit
 
-        info_dict["image_pixels"] = self.imaging.grid.sub_shape_slim
-        info_dict["sub_size_light_profiles"] = self.imaging.grid.sub_size
-        info_dict["sub_size_pixelization"] = self.imaging.grid_pixelization.sub_size
-        info_dict["psf_shape_2d"] = self.imaging.psf.shape_native
+        info_dict["image_pixels"] = self.dataset.grid.sub_shape_slim
+        info_dict["sub_size_light_profiles"] = self.dataset.grid.sub_size
+        info_dict["sub_size_pixelization"] = self.dataset.grid_pixelization.sub_size
+        info_dict["psf_shape_2d"] = self.dataset.psf.shape_native
 
         if fit.inversion is not None:
             info_dict["source_pixels"] = len(fit.inversion.reconstruction)
 
         if hasattr(fit.inversion, "w_tilde"):
             info_dict[
                 "w_tilde_curvature_preload_size"
@@ -352,46 +309,38 @@
 
         Returns
         -------
         float
             A log likelihood cap which is applied in a stochastic model-fit to give improved error and posterior
             estimates.
         """
-        instance = self.instance_with_associated_hyper_images_from(instance=instance)
+        instance = self.instance_with_associated_adapt_images_from(instance=instance)
         tracer = self.tracer_via_instance_from(instance=instance)
 
         if not tracer.has(cls=ag.Pixelization):
             return
 
         if not any(
             pix.mesh.is_stochastic for pix in tracer.cls_list_from(cls=ag.Pixelization)
         ):
             return
 
-        hyper_image_sky = self.hyper_image_sky_via_instance_from(instance=instance)
-
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
-
         settings_pixelization = (
             self.settings_pixelization.settings_with_is_stochastic_true()
         )
 
         log_evidences = []
 
         for i in range(self.settings_lens.stochastic_samples):
 
             try:
 
                 log_evidence = FitImaging(
                     dataset=self.dataset,
                     tracer=tracer,
-                    hyper_image_sky=hyper_image_sky,
-                    hyper_background_noise=hyper_background_noise,
                     settings_pixelization=settings_pixelization,
                     settings_inversion=self.settings_inversion,
                     preloads=self.preloads,
                 ).log_evidence
             except (
                 PixelizationException,
                 exc.PixelizationException,
@@ -402,14 +351,47 @@
                 log_evidence = None
 
             if log_evidence is not None:
                 log_evidences.append(log_evidence)
 
         return log_evidences
 
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
+        if self.positions_likelihood is not None:
+            visualizer.visualize_image_with_positions(
+                image=self.dataset.image,
+                positions=self.positions_likelihood.positions,
+            )
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
@@ -420,20 +402,17 @@
         The visualization performed by this function includes:
 
         - Images of the best-fit `Tracer`, including the images of each of its galaxies.
 
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
@@ -441,18 +420,18 @@
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
 
         fit = self.fit_imaging_via_instance_from(instance=instance)
 
         if self.positions_likelihood is not None:
             self.positions_likelihood.output_positions_info(
                 output_path=paths.output_path, tracer=fit.tracer
             )
@@ -475,36 +454,21 @@
         visualizer.visualize_tracer(
             tracer=tracer, grid=fit.grid, during_analysis=during_analysis
         )
         visualizer.visualize_galaxies(
             galaxies=tracer.galaxies, grid=fit.grid, during_analysis=during_analysis
         )
         if fit.inversion is not None:
-            visualizer.visualize_inversion(
-                inversion=fit.inversion, during_analysis=during_analysis
-            )
+            if fit.inversion.has(cls=ag.AbstractMapper):
+                visualizer.visualize_inversion(
+                    inversion=fit.inversion, during_analysis=during_analysis
+                )
 
         visualizer.visualize_contribution_maps(tracer=fit.tracer)
 
-        if visualizer.plot_fit_no_hyper:
-            fit = self.fit_imaging_via_tracer_from(
-                tracer=fit.tracer,
-                hyper_image_sky=None,
-                hyper_background_noise=None,
-                use_hyper_scaling=False,
-                preload_overwrite=Preloads(use_w_tilde=False),
-            )
-
-            try:
-                visualizer.visualize_fit_imaging(
-                    fit=fit, during_analysis=during_analysis, subfolders="fit_no_hyper"
-                )
-            except exc.InversionException:
-                pass
-
     def make_result(
         self,
         samples: af.SamplesPDF,
         model: af.Collection,
         sigma=1.0,
         use_errors=True,
         use_widths=False,
@@ -517,15 +481,15 @@
 
         - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
           an instance of the maximum log likelihood model).
 
         - The non-linear search used to perform the model fit.
 
         The `ResultImaging` object contains a number of methods which use the above objects to create the max
-        log likelihood `Tracer`, `FitImaging`, hyper-galaxy images,etc.
+        log likelihood `Tracer`, `FitImaging`, adapt-galaxy images,etc.
 
         Parameters
         ----------
         samples
             A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
             run of samples of the nested sampler.
         model
@@ -538,25 +502,25 @@
             The result of fitting the model to the imaging dataset, via a non-linear search.
         """
         return ResultImaging(samples=samples, model=model, analysis=self)
 
     def save_attributes_for_aggregator(self, paths: af.DirectoryPaths):
         """
         Before the non-linear search begins, this routine saves attributes of the `Analysis` object to the `pickles`
-        folder such that they can be load after the analysis using PyAutoFit's database and aggregator tools.
+        folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
         For this analysis, it uses the `AnalysisDataset` object's method to output the following:
 
         - The dataset's data.
         - The dataset's noise-map.
         - The settings associated with the dataset.
         - The settings associated with the inversion.
         - The settings associated with the pixelization.
         - The Cosmology.
-        - The hyper dataset's model image and galaxy images, if used.
+        - The adapt dataset's model image and galaxy images, if used.
 
         This function also outputs attributes specific to an imaging dataset:
 
         - Its PSF.
         - Its mask.
         - The positions of the brightest pixels in the lensed source which are used to discard mass models.
         - The preloaded image-plane source plane pixelization if used by the analysis. This ensures that differences in
```

### Comparing `autolens-2023.3.27.1/autolens/imaging/model/result.py` & `autolens-2023.7.7.2/autolens/imaging/model/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
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
```

### Comparing `autolens-2023.3.27.1/autolens/imaging/model/visualizer.py` & `autolens-2023.7.7.2/autolens/imaging/model/visualizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from autolens.imaging.plot.fit_imaging_plotters import FitImagingPlotter
 
 from autolens.analysis.visualizer import plot_setting
 
 
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
@@ -36,74 +36,80 @@
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
             chi_squared_map=should_plot("chi_squared_map"),
             normalized_residual_map=should_plot("normalized_residual_map"),
         )
 
-        fit_imaging_plotter.figures_2d_of_planes(
+        fit_plotter.figures_2d_of_planes(
             subtracted_image=should_plot("subtracted_images_of_planes"),
             model_image=should_plot("model_images_of_planes"),
             plane_image=should_plot("plane_images_of_planes"),
         )
 
         if should_plot("subplot_fit"):
-            fit_imaging_plotter.subplot_fit_imaging()
+            fit_plotter.subplot_fit()
 
-        if should_plot("subplots_of_planes_fits"):
-            fit_imaging_plotter.subplot_of_planes()
+        if should_plot("subplot_of_planes"):
+            fit_plotter.subplot_of_planes()
 
-        if not during_analysis:
+        if not during_analysis and should_plot("all_at_end_png"):
 
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
-                fit_imaging_plotter.figures_2d_of_planes(
-                    subtracted_image=True, model_image=True, plane_image=True
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
-                fit_imaging_plotter.figures_2d_of_planes(
-                    subtracted_image=True, model_image=True
-                )
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join("fit_dataset", "end"),
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
+            fit_plotter.figures_2d_of_planes(
+                subtracted_image=True, model_image=True, plane_image=True
+            )
+
+        if not during_analysis and should_plot("all_at_end_fits"):
+
+            mat_plot_2d = self.mat_plot_2d_from(
+                subfolders=path.join("fit_dataset", "fits"), format="fits"
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
+            fit_plotter.figures_2d_of_planes(
+                subtracted_image=True, model_image=True, interpolate_to_uniform=True
+            )
```

### Comparing `autolens-2023.3.27.1/autolens/imaging/plot/fit_imaging_plotters.py` & `autolens-2023.7.7.2/autolens/imaging/plot/fit_imaging_plotters.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,18 +60,14 @@
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
             residuals_symmetric_cmap=residuals_symmetric_cmap
         )
 
         self.residuals_symmetric_cmap = residuals_symmetric_cmap
 
-        # self.figures_2d = self._fit_imaging_meta_plotter.figures_2d
-        # self.subplot = self._fit_imaging_meta_plotter.subplot
-        # self.subplot_fit_imaging = self._fit_imaging_meta_plotter.subplot_fit_imaging
-
     def get_visuals_2d(self) -> aplt.Visuals2D:
         return self.get_2d.via_fit_imaging_from(fit=self.fit)
 
     @property
     def tracer(self):
         return self.fit.tracer_linear_light_profiles_to_light_profiles
 
@@ -135,14 +131,17 @@
 
     def figures_2d_of_planes(
         self,
         plane_index: Optional[int] = None,
         subtracted_image: bool = False,
         model_image: bool = False,
         plane_image: bool = False,
+        use_source_vmax: bool = False,
+        zoom_to_brightest: bool = True,
+        interpolate_to_uniform: bool = False,
     ):
         """
         Plots images representing each individual `Plane` in the fit's `Tracer` in 2D, which are computed via the
         plotter's 2D grid object.
 
         These images subtract or omit the contribution of other planes in the plane, such that plots showing
         each individual plane are made.
@@ -161,57 +160,51 @@
         model_image
             Whether to make a 2D plot (via `imshow`) of the model image of a plane, where this image is the
             model image of one plane, thereby showing how much it contributes to the overall model image.
         plane_image
             Whether to make a 2D plot (via `imshow`) of the image of a plane in its source-plane (e.g. unlensed).
             Depending on how the fit is performed, this could either be an image of light profiles of the reconstruction
             of an `Inversion`.
+        use_source_vmax
+            If `True`, the maximum value of the lensed source (e.g. in the image-plane) is used to set the `vmax` of
+            certain plots (e.g. the `data`) in order to ensure the lensed source is visible compared to the lens.
+        zoom_to_brightest
+            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
+            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
+        interpolate_to_uniform
+            If `True`, the mapper's reconstruction is interpolated to a uniform grid before plotting, for example
+            meaning that an irregular Delaunay grid can be plotted as a uniform grid.
         """
 
         visuals_2d = self.get_visuals_2d()
 
         visuals_2d_no_critical_caustic = self.get_visuals_2d()
-        visuals_2d_no_critical_caustic.critical_curves = None
-        visuals_2d_no_critical_caustic.caustics = None
+        visuals_2d_no_critical_caustic.tangential_critical_curves = None
+        visuals_2d_no_critical_caustic.radial_critical_curves = None
+        visuals_2d_no_critical_caustic.tangential_caustics = None
+        visuals_2d_no_critical_caustic.radial_caustics = None
 
         plane_indexes = self.plane_indexes_from(plane_index=plane_index)
 
+        if use_source_vmax:
+            self.mat_plot_2d.cmap.kwargs["vmax"] = np.max(self.fit.model_images_of_planes_list[-1])
+
         for plane_index in plane_indexes:
 
             if subtracted_image:
 
-                if "vmin" in self.mat_plot_2d.cmap.kwargs:
-                    vmin_stored = True
-                else:
-                    self.mat_plot_2d.cmap.kwargs["vmin"] = 0.0
-                    vmin_stored = False
-
-                if "vmax" in self.mat_plot_2d.cmap.kwargs:
-                    vmax_stored = True
-                else:
-                    self.mat_plot_2d.cmap.kwargs["vmax"] = np.max(
-                        self.fit.model_images_of_planes_list[plane_index]
-                    )
-                    vmax_stored = False
-
                 self.mat_plot_2d.plot_array(
                     array=self.fit.subtracted_images_of_planes_list[plane_index],
                     visuals_2d=visuals_2d_no_critical_caustic,
                     auto_labels=aplt.AutoLabels(
                         title=f"Subtracted Image of Plane {plane_index}",
                         filename=f"subtracted_image_of_plane_{plane_index}",
                     ),
                 )
 
-                if not vmin_stored:
-                    self.mat_plot_2d.cmap.kwargs.pop("vmin")
-
-                if not vmax_stored:
-                    self.mat_plot_2d.cmap.kwargs.pop("vmax")
-
             if model_image:
 
                 if self.tracer.planes[plane_index].has(cls=aa.Pixelization):
 
                     # Overwrite plane_index=0 so that model image uses critical curves -- improve via config cutomization
 
                     visuals_2d_model_image = self.inversion_plotter_of_plane(plane_index=0).get_visuals_2d_for_data()
@@ -230,26 +223,34 @@
                 )
 
             if plane_image:
 
                 if not self.tracer.planes[plane_index].has(cls=aa.Pixelization):
 
                     self.tracer_plotter.figures_2d_of_planes(
-                        plane_image=True, plane_index=plane_index
+                        plane_image=True,
+                        plane_index=plane_index,
+                        zoom_to_brightest=zoom_to_brightest
                     )
 
                 elif self.tracer.planes[plane_index].has(cls=aa.Pixelization):
 
                     inversion_plotter = self.inversion_plotter_of_plane(
                         plane_index=plane_index
                     )
                     inversion_plotter.figures_2d_of_pixelization(
-                        pixelization_index=0, reconstruction=True
+                        pixelization_index=0,
+                        reconstruction=True,
+                        zoom_to_brightest=zoom_to_brightest,
+                        interpolate_to_uniform=interpolate_to_uniform
                     )
 
+        if use_source_vmax:
+            self.mat_plot_2d.cmap.kwargs.pop("vmax")
+
     def subplot_of_planes(self, plane_index: Optional[int] = None):
         """
         Plots images representing each individual `Plane` in the plotter's `Tracer` in 2D on a subplot, which are
         computed via the plotter's 2D grid object.
 
         These images subtract or omit the contribution of other planes in the plane, such that plots showing
         each individual plane are made.
@@ -265,138 +266,209 @@
 
         plane_indexes = self.plane_indexes_from(plane_index=plane_index)
 
         for plane_index in plane_indexes:
 
             self.open_subplot_figure(number_subplots=4)
 
-            self.figures_2d(image=True)
+            self.figures_2d(data=True)
+
             self.figures_2d_of_planes(subtracted_image=True, plane_index=plane_index)
             self.figures_2d_of_planes(model_image=True, plane_index=plane_index)
             self.figures_2d_of_planes(plane_image=True, plane_index=plane_index)
 
             self.mat_plot_2d.output.subplot_to_figure(
                 auto_filename=f"subplot_of_plane_{plane_index}"
             )
             self.close_subplot_figure()
 
     def subplot(
         self,
-        image: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
-        model_image: bool = False,
+        model_data: bool = False,
         residual_map: bool = False,
         normalized_residual_map: bool = False,
         chi_squared_map: bool = False,
-        auto_filename: str = "subplot_fit_imaging",
+        auto_filename: str = "subplot_fit",
     ):
         """
         Plots the individual attributes of the plotter's `FitImaging` object in 2D on a subplot.
 
         The API is such that every plottable attribute of the `FitImaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
-        image
-            Whether or not to include a 2D plot (via `imshow`) of the image data.
+        data
+            Whether to include a 2D plot (via `imshow`) of the image data.
         noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the noise map.
+            Whether to include a 2D plot (via `imshow`) of the noise map.
         psf
-            Whether or not to include a 2D plot (via `imshow`) of the psf.
+            Whether to include a 2D plot (via `imshow`) of the psf.
         signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the signal-to-noise map.
-        model_image
-            Whether or not to include a 2D plot (via `imshow`) of the model image.
+            Whether to include a 2D plot (via `imshow`) of the signal-to-noise map.
+        model_data
+            Whether to include a 2D plot (via `imshow`) of the model image.
         residual_map
-            Whether or not to include a 2D plot (via `imshow`) of the residual map.
+            Whether to include a 2D plot (via `imshow`) of the residual map.
         normalized_residual_map
-            Whether or not to include a 2D plot (via `imshow`) of the normalized residual map.
+            Whether to include a 2D plot (via `imshow`) of the normalized residual map.
         chi_squared_map
-            Whether or not to include a 2D plot (via `imshow`) of the chi-squared map.
+            Whether to include a 2D plot (via `imshow`) of the chi-squared map.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
         self._subplot_custom_plot(
-            image=image,
+            data=data,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
-            model_image=model_image,
+            model_image=model_data,
             residual_map=residual_map,
             normalized_residual_map=normalized_residual_map,
             chi_squared_map=chi_squared_map,
             auto_labels=AutoLabels(filename=auto_filename),
         )
 
-    def subplot_fit_imaging(self):
+    def subplot_fit(self):
         """
         Standard subplot of the attributes of the plotter's `FitImaging` object.
         """
-        return self.subplot(
-            image=True,
-            signal_to_noise_map=True,
-            model_image=True,
-            residual_map=True,
-            normalized_residual_map=True,
-            chi_squared_map=True,
+
+        self.open_subplot_figure(number_subplots=12)
+
+        self.figures_2d(data=True)
+
+        self.set_title(label="Data (Source Scale)")
+        self.figures_2d(data=True, use_source_vmax=True)
+        self.set_title(label=None)
+
+        self.figures_2d(signal_to_noise_map=True)
+        self.figures_2d(model_image=True)
+
+        self.set_title(label="Lens Light Model Image")
+        self.figures_2d_of_planes(plane_index=0, model_image=True)
+
+        # If the lens light is not included the subplot index does not increase, so we must manually set it to 4
+        self.mat_plot_2d.subplot_index = 6
+
+        final_plane_index = len(self.fit.tracer.planes) - 1
+
+        self.mat_plot_2d.cmap.kwargs["vmin"] = 0.0
+
+        self.set_title(label="Lens Light Subtracted Image")
+        self.figures_2d_of_planes(plane_index=final_plane_index, subtracted_image=True, use_source_vmax=True)
+
+        self.set_title(label="Source Model Image (Image Plane)")
+        self.figures_2d_of_planes(plane_index=final_plane_index, model_image=True, use_source_vmax=True)
+
+        self.mat_plot_2d.cmap.kwargs.pop("vmin")
+
+        self.set_title(label="Source Plane (Zoomed)")
+        self.figures_2d_of_planes(plane_index=final_plane_index, plane_image=True, use_source_vmax=True)
+
+
+        self.set_title(label=None)
+
+        self.mat_plot_2d.subplot_index = 9
+
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
+        self.set_title(label="Source Plane (No Zoom)")
+        self.figures_2d_of_planes(
+            plane_index=final_plane_index,
+            plane_image=True,
+            zoom_to_brightest=False,
+            use_source_vmax=True
+        )
+
+        self.set_title(label=None)
+
+        self.mat_plot_2d.output.subplot_to_figure(
+            auto_filename="subplot_fit"
         )
+        self.close_subplot_figure()
 
     def figures_2d(
         self,
-        image: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         model_image: bool = False,
         residual_map: bool = False,
         normalized_residual_map: bool = False,
         chi_squared_map: bool = False,
+        use_source_vmax : bool = False,
         suffix: str = "",
     ):
         """
         Plots the individual attributes of the plotter's `FitImaging` object in 2D.
 
         The API is such that every plottable attribute of the `FitImaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
-        image
+        data
             Whether to make a 2D plot (via `imshow`) of the image data.
         noise_map
             Whether to make a 2D plot (via `imshow`) of the noise map.
         signal_to_noise_map
             Whether to make a 2D plot (via `imshow`) of the signal-to-noise map.
         model_image
             Whether to make a 2D plot (via `imshow`) of the model image.
         residual_map
             Whether to make a 2D plot (via `imshow`) of the residual map.
         normalized_residual_map
             Whether to make a 2D plot (via `imshow`) of the normalized residual map.
         chi_squared_map
             Whether to make a 2D plot (via `imshow`) of the chi-squared map.
+        use_source_vmax
+            If `True`, the maximum value of the lensed source (e.g. in the image-plane) is used to set the `vmax` of
+            certain plots (e.g. the `data`) in order to ensure the lensed source is visible compared to the lens.
         """
 
         visuals_2d = self.get_visuals_2d()
 
         visuals_2d_no_critical_caustic = self.get_visuals_2d()
-        visuals_2d_no_critical_caustic.critical_curves = None
-        visuals_2d_no_critical_caustic.caustics = None
+        visuals_2d_no_critical_caustic.tangential_critical_curves = None
+        visuals_2d_no_critical_caustic.radial_critical_curves = None
+        visuals_2d_no_critical_caustic.tangential_caustics = None
+        visuals_2d_no_critical_caustic.radial_caustics = None
         visuals_2d_no_critical_caustic.origin = None
         visuals_2d_no_critical_caustic.light_profile_centres = None
         visuals_2d_no_critical_caustic.mass_profile_centres = None
 
-        if image:
+        if data:
+
+            if use_source_vmax:
+                self.mat_plot_2d.cmap.kwargs["vmax"] = np.max(self.fit.model_images_of_planes_list[-1])
 
             self.mat_plot_2d.plot_array(
                 array=self.fit.data,
                 visuals_2d=visuals_2d_no_critical_caustic,
-                auto_labels=AutoLabels(title="Image", filename=f"image_2d{suffix}"),
+                auto_labels=AutoLabels(title="Image", filename=f"data{suffix}"),
             )
 
+            if use_source_vmax:
+                self.mat_plot_2d.cmap.kwargs.pop("vmax")
+
         if noise_map:
 
             self.mat_plot_2d.plot_array(
                 array=self.fit.noise_map,
                 visuals_2d=visuals_2d_no_critical_caustic,
                 auto_labels=AutoLabels(
                     title="Noise-Map", filename=f"noise_map{suffix}"
@@ -405,28 +477,34 @@
 
         if signal_to_noise_map:
 
             self.mat_plot_2d.plot_array(
                 array=self.fit.signal_to_noise_map,
                 visuals_2d=visuals_2d_no_critical_caustic,
                 auto_labels=AutoLabels(
-                    title="Signal-To-Noise Map", filename=f"signal_to_noise_map{suffix}"
+                    title="Signal-To-Noise Map", cb_unit=" S/N", filename=f"signal_to_noise_map{suffix}"
                 ),
             )
 
         if model_image:
 
+            if use_source_vmax:
+                self.mat_plot_2d.cmap.kwargs["vmax"] = np.max(self.fit.model_images_of_planes_list[-1])
+
             self.mat_plot_2d.plot_array(
                 array=self.fit.model_data,
                 visuals_2d=visuals_2d,
                 auto_labels=AutoLabels(
                     title="Model Image", filename=f"model_image{suffix}"
                 ),
             )
 
+            if use_source_vmax:
+                self.mat_plot_2d.cmap.kwargs.pop("vmax")
+
         cmap_original = self.mat_plot_2d.cmap
 
         if self.residuals_symmetric_cmap:
 
             self.mat_plot_2d.cmap = self.mat_plot_2d.cmap.symmetric
 
         if residual_map:
@@ -442,22 +520,23 @@
         if normalized_residual_map:
 
             self.mat_plot_2d.plot_array(
                 array=self.fit.normalized_residual_map,
                 visuals_2d=visuals_2d_no_critical_caustic,
                 auto_labels=AutoLabels(
                     title="Normalized Residual Map",
+                    cb_unit=r" $\sigma$",
                     filename=f"normalized_residual_map{suffix}",
                 ),
             )
 
         self.mat_plot_2d.cmap = cmap_original
 
         if chi_squared_map:
 
             self.mat_plot_2d.plot_array(
                 array=self.fit.chi_squared_map,
                 visuals_2d=visuals_2d_no_critical_caustic,
                 auto_labels=AutoLabels(
-                    title="Chi-Squared Map", filename=f"chi_squared_map{suffix}"
+                    title="Chi-Squared Map", cb_unit=r" $\chi^2$",  filename=f"chi_squared_map{suffix}"
                 ),
             )
```

### Comparing `autolens-2023.3.27.1/autolens/interferometer/fit_interferometer.py` & `autolens-2023.7.7.2/autolens/interferometer/fit_interferometer.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 
 class FitInterferometer(aa.FitInterferometer, AbstractFitInversion):
     def __init__(
         self,
         dataset: aa.Interferometer,
         tracer: Tracer,
-        hyper_background_noise: ag.hyper_data.HyperBackgroundNoise = None,
-        use_hyper_scaling: bool = True,
         settings_pixelization: aa.SettingsPixelization = aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ):
         """
         Fits an interferometer dataset using a `Tracer` object.
@@ -52,19 +50,14 @@
 
         Parameters
         ----------
         dataset
             The interforometer dataset which is fitted by the galaxies in the tracer.
         tracer
             The tracer of galaxies whose light profile images are used to fit the interferometer data.
-        hyper_background_noise
-            If included, adds a noise-scaling term to the background noise.
-        use_hyper_scaling
-            If set to False, the hyper scaling functions (e.g. the `hyper_background_noise`) are
-            omitted irrespective of their inputs.
         settings_pixelization
             Settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
@@ -77,44 +70,27 @@
         try:
             from autoarray.inversion.inversion import inversion_util_secret
         except ImportError:
             settings_inversion.use_w_tilde = False
 
         self.tracer = tracer
 
-        self.hyper_background_noise = hyper_background_noise
-        self.use_hyper_scaling = use_hyper_scaling
-
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
 
         self.preloads = preloads
 
         self.profiling_dict = profiling_dict
 
         super().__init__(dataset=dataset, profiling_dict=profiling_dict)
         AbstractFitInversion.__init__(
             self=self, model_obj=tracer, settings_inversion=settings_inversion
         )
 
     @property
-    def noise_map(self) -> aa.Visibilities:
-        """
-        Returns the interferometer's noise-map, which may have a hyper scaling performed which increase the noise in
-        regions of the data that are poorly fitted in order to avoid overfitting.
-        """
-        if self.use_hyper_scaling and self.hyper_background_noise is not None:
-
-            return self.hyper_background_noise.hyper_noise_map_complex_from(
-                noise_map=self.dataset.noise_map
-            )
-
-        return self.dataset.noise_map
-
-    @property
     def profile_visibilities(self) -> aa.Visibilities:
         """
         Returns the visibilities of every light profile in the tracer, which are computed by performing a Fourier
         transform to the sum of light profile images.
         """
         return self.tracer.visibilities_from(
             grid=self.dataset.grid, transformer=self.dataset.transformer
@@ -126,15 +102,14 @@
         Returns the interferometer dataset's visibilities with all transformed light profile images in the fit's
         tracer subtracted.
         """
         return self.visibilities - self.profile_visibilities
 
     @property
     def tracer_to_inversion(self) -> TracerToInversion:
-
         return TracerToInversion(
             tracer=self.tracer,
             dataset=self.dataset,
             data=self.profile_subtracted_visibilities,
             noise_map=self.noise_map,
             w_tilde=self.w_tilde,
             settings_pixelization=self.settings_pixelization,
@@ -163,35 +138,34 @@
         If the tracer does not have any linear objects and therefore omits an inversion, the model data is the
         sum of all light profile images Fourier transformed to visibilities.
 
         If a inversion is included it is the sum of these visibilities and the inversion's reconstructed visibilities.
         """
 
         if self.perform_inversion:
-
             return self.profile_visibilities + self.inversion.mapped_reconstructed_data
 
         return self.profile_visibilities
 
     @property
     def grid(self) -> aa.type.Grid2DLike:
-        return self.interferometer.grid
+        return self.dataset.grid
 
     @property
     def galaxy_model_image_dict(self) -> Dict[ag.Galaxy, np.ndarray]:
         """
         A dictionary which associates every galaxy in the tracer with its `image`.
 
         This image is the image of the sum of:
 
         - The images of all ordinary light profiles in that tracer summed.
         - The images of all linear objects (e.g. linear light profiles / pixelizations), where the images are solved
           for first via the inversion.
 
-        For modeling, this dictionary is used to set up the `hyper_images` that adapt certain pixelizations to the
+        For modeling, this dictionary is used to set up the `adapt_images` that adapt certain pixelizations to the
         data being fitted.
         """
         galaxy_model_image_dict = self.tracer.galaxy_image_2d_dict_from(grid=self.grid)
 
         galaxy_linear_obj_image_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=True
         )
@@ -205,20 +179,17 @@
 
         These visibilities are the sum of:
 
         - The visibilities of all ordinary light profiles in that tracer summed and Fourier transformed to visibilities
           space.
         - The visibilities of all linear objects (e.g. linear light profiles / pixelizations), where the visibilities
           are solved for first via the inversion.
-
-        For modeling, this dictionary is used to set up the `hyper_visibilities` that adapt certain pixelizations to the
-        data being fitted.
         """
         galaxy_model_visibilities_dict = self.tracer.galaxy_visibilities_dict_from(
-            grid=self.interferometer.grid, transformer=self.interferometer.transformer
+            grid=self.dataset.grid, transformer=self.dataset.transformer
         )
 
         galaxy_linear_obj_visibilities_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=False
         )
 
         return {**galaxy_model_visibilities_dict, **galaxy_linear_obj_visibilities_dict}
@@ -293,14 +264,12 @@
 
         if settings_inversion is None:
             settings_inversion = self.settings_inversion
 
         return FitInterferometer(
             dataset=self.interferometer,
             tracer=self.tracer,
-            hyper_background_noise=self.hyper_background_noise,
-            use_hyper_scaling=self.use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=settings_inversion,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
```

### Comparing `autolens-2023.3.27.1/autolens/interferometer/interferometer.py` & `autolens-2023.7.7.2/autolens/interferometer/interferometer.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
            imaging data instance."""
 
         tracer = Tracer.from_galaxies(galaxies=galaxies)
 
         return self.via_tracer_from(tracer=tracer, grid=grid)
 
     def via_deflections_and_galaxies_from(self, deflections, galaxies):
-
         grid = aa.Grid2D.uniform(
             shape_native=deflections.shape_native,
             pixel_scales=deflections.pixel_scales,
             sub_size=1,
         )
 
         deflected_grid = grid - deflections.binned
```

### Comparing `autolens-2023.3.27.1/autolens/interferometer/model/analysis.py` & `autolens-2023.7.7.2/autolens/interferometer/model/analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class AnalysisInterferometer(AnalysisDataset):
     def __init__(
         self,
         dataset,
         positions_likelihood: Optional[
             Union[PositionsLHResample, PositionsLHPenalty]
         ] = None,
-        hyper_dataset_result=None,
+        adapt_result=None,
         cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15(),
         settings_pixelization: aa.SettingsPixelization = None,
         settings_inversion: aa.SettingsInversion = None,
         settings_lens: SettingsLens = None,
         raise_inversion_positions_likelihood_exception: bool = True,
     ):
         """
@@ -48,27 +48,27 @@
         such as visualization, outputting results to hard-disk and storing results in a format that can be loaded after
         the model-fit is complete using PyAutoFit's database tools.
 
         This Analysis class is used for all model-fits which fit galaxies (or objects containing galaxies like a
         `Tracer`) to an interferometer dataset.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. a
-        pixelization or inversion), the Cosmology used for the analysis and hyper datasets used for certain model
+        pixelization or inversion), the Cosmology used for the analysis and adapt datasets used for certain model
         classes.
 
         Parameters
         ----------
         dataset
             The interferometer dataset that the model is fitted too.
         positions_likelihood
             An object which alters the likelihood function to include a term which accounts for whether
             image-pixel coordinates in arc-seconds corresponding to the multiple images of the lensed source galaxy
             trace close to one another in the source-plane.
-        hyper_dataset_result
-            The hyper-model image and hyper galaxies images of a previous result in a model-fitting pipeline, which are
+        adapt_result
+            Theadapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
             used by certain classes for adapting the analysis to the properties of the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         settings_pixelization
             settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
@@ -81,41 +81,32 @@
             be inferred, in which case an Exception is raised before the model-fit begins to inform the user
             of this. This exception is not raised if this input is False, allowing the user to perform the model-fit
             anyway.
         """
         super().__init__(
             dataset=dataset,
             positions_likelihood=positions_likelihood,
-            hyper_dataset_result=hyper_dataset_result,
+            adapt_result=adapt_result,
             cosmology=cosmology,
             settings_pixelization=settings_pixelization,
             settings_inversion=settings_inversion,
             settings_lens=settings_lens,
             raise_inversion_positions_likelihood_exception=raise_inversion_positions_likelihood_exception,
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
@@ -123,116 +114,32 @@
         model
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
-                if self.positions_likelihood is not None:
-                    visualizer.visualize_image_with_positions(
-                        image=self.interferometer.dirty_image,
-                        positions=self.positions_likelihood.positions,
-                    )
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
 
-    def set_hyper_dataset(self, result):
-        """
-        Using a the result of a previous model-fit, set the hyper-dataset for this analysis. This is used to adapt
-        aspects of the model (e.g. the pixelization, regularization scheme) to the properties of the dataset being
-        fitted.
-
-        This passes the hyper model image and hyper galaxy images of the previous fit. These represent where different
-        galaxies in the dataset are located and thus allows the fit to adapt different aspects of the model to
-        different galaxies in the data.
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
-            for galaxy_path, galaxy in instance.path_instance_tuples_for_class(
-                ag.Galaxy
-            ):
-                if galaxy_path in self.hyper_galaxy_visibilities_path_dict:
-                    galaxy.hyper_model_visibilities = self.hyper_model_visibilities
-                    galaxy.hyper_galaxy_visibilities = (
-                        self.hyper_galaxy_visibilities_path_dict[galaxy_path]
-                    )
-
-        return instance
-
     def log_likelihood_function(self, instance):
         """
         Given an instance of the model, where the model parameters are set via a non-linear search, fit the model
         instance to the interferometer dataset.
 
         This function returns a log likelihood which is used by the non-linear search to guide the model-fit.
 
         For this analysis class, this function performs the following steps:
 
-        1) If the analysis has a hyper dataset, associated the model galaxy images of this dataset to the galaxies in
+        1) If the analysis has a adapt dataset, associated the model galaxy images of this dataset to the galaxies in
            the model instance.
 
         2) Extract attributes which model aspects of the data reductions, like the scaling the background sky
            and background noise.
 
         3) Extracts all galaxies from the model instance and set up a `Tracer`, which includes ordering the galaxies
            by redshift to set up each `Plane`.
@@ -282,81 +189,62 @@
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
         check_positions
             Whether the multiple image positions of the lensed source should be checked, i.e. whether they trace
             within the position threshold of one another in the source plane.
         profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitInterferometer
             The fit of the plane to the interferometer dataset, which includes the log likelihood.
         """
-        self.instance_with_associated_hyper_images_from(instance=instance)
+        self.instance_with_associated_adapt_images_from(instance=instance)
         tracer = self.tracer_via_instance_from(instance=instance)
 
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
-
         return self.fit_interferometer_via_tracer_from(
             tracer=tracer,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
         )
 
     def fit_interferometer_via_tracer_from(
         self,
         tracer: Tracer,
-        hyper_background_noise: Optional[ag.hyper_data.HyperBackgroundNoise],
-        use_hyper_scaling: bool = True,
         preload_overwrite: Optional[Preloads] = None,
     ):
         """
         Given a `Tracer`, which the analysis constructs from a model instance, create a `FitInterferometer` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
         Parameters
         ----------
         tracer
             The tracer of galaxies whose ray-traced model images are used to fit the imaging data.
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
@@ -364,16 +252,14 @@
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
         preloads = self.preloads if preload_overwrite is None else preload_overwrite
 
         return FitInterferometer(
             dataset=self.dataset,
             tracer=tracer,
-            hyper_background_noise=hyper_background_noise,
-            use_hyper_scaling=use_hyper_scaling,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
         )
 
     @property
     def fit_func(self):
@@ -400,45 +286,39 @@
 
          Returns
          -------
          float
              A log likelihood cap which is applied in a stochastic model-fit to give improved error and posterior
              estimates.
         """
-        instance = self.instance_with_associated_hyper_images_from(instance=instance)
+        instance = self.instance_with_associated_adapt_images_from(instance=instance)
         tracer = self.tracer_via_instance_from(instance=instance)
 
         if not tracer.has(cls=aa.Pixelization):
             return None
 
         if not any(
             [
                 pix.mesh.is_stochastic
                 for pix in tracer.cls_list_from(cls=ag.Pixelization)
             ]
         ):
             return
 
-        hyper_background_noise = self.hyper_background_noise_via_instance_from(
-            instance=instance
-        )
-
         settings_pixelization = (
             self.settings_pixelization.settings_with_is_stochastic_true()
         )
 
         log_evidences = []
 
         for i in range(self.settings_lens.stochastic_samples):
-
             try:
                 log_evidence = FitInterferometer(
                     dataset=self.dataset,
                     tracer=tracer,
-                    hyper_background_noise=hyper_background_noise,
                     settings_pixelization=settings_pixelization,
                     settings_inversion=self.settings_inversion,
                     preloads=self.preloads,
                 ).log_evidence
             except (
                 PixelizationException,
                 exc.PixelizationException,
@@ -449,31 +329,64 @@
                 log_evidence = None
 
             if log_evidence is not None:
                 log_evidences.append(log_evidence)
 
         return log_evidences
 
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
+        visualizer = VisualizerInterferometer(visualize_path=paths.image_path)
+
+        visualizer.visualize_interferometer(dataset=self.interferometer)
+
+        if self.positions_likelihood is not None:
+            visualizer.visualize_image_with_positions(
+                image=self.dataset.dirty_image,
+                positions=self.positions_likelihood.positions,
+            )
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
 
         - Images of the best-fit `Tracer`, including the images of each of its galaxies.
 
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
@@ -483,18 +396,18 @@
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
 
         fit = self.fit_interferometer_via_instance_from(instance=instance)
 
         if self.positions_likelihood is not None:
             self.positions_likelihood.output_positions_info(
                 output_path=paths.output_path, tracer=fit.tracer
             )
@@ -528,29 +441,14 @@
                     inversion=fit.inversion, during_analysis=during_analysis
                 )
             except IndexError:
                 pass
 
         visualizer.visualize_contribution_maps(tracer=fit.tracer)
 
-        if visualizer.plot_fit_no_hyper:
-            fit = self.fit_interferometer_via_tracer_from(
-                tracer=fit.tracer,
-                hyper_background_noise=None,
-                use_hyper_scaling=False,
-                preload_overwrite=Preloads(use_w_tilde=False),
-            )
-
-            try:
-                visualizer.visualize_fit_interferometer(
-                    fit=fit, during_analysis=during_analysis, subfolders="fit_no_hyper"
-                )
-            except exc.InversionException:
-                pass
-
     def make_result(
         self,
         samples: af.SamplesPDF,
         model: af.Collection,
         sigma=1.0,
         use_errors=True,
         use_widths=False,
@@ -563,15 +461,15 @@
 
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
@@ -584,25 +482,25 @@
             The result of fitting the model to the imaging dataset, via a non-linear search.
         """
         return ResultInterferometer(samples=samples, model=model, analysis=self)
 
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
 
         - Its uv-wavelengths
         - Its real space mask.
         - The positions of the brightest pixels in the lensed source which are used to discard mass models.
         - The preloaded image-plane source plane pixelization if used by the analysis. This ensures that differences in
```

### Comparing `autolens-2023.3.27.1/autolens/interferometer/model/visualizer.py` & `autolens-2023.7.7.2/autolens/interferometer/model/visualizer.py`

 * *Files 23% similar despite different names*

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
         used with a non-linear search the `visualize_path` points to the search's results folder.
 
@@ -41,31 +41,35 @@
 
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
-            fit_interferometer_plotter.subplot_fit_dirty_images()
-            fit_interferometer_plotter.subplot_fit_real_space()
+            fit_plotter.subplot_fit()
 
-        fit_interferometer_plotter.figures_2d(
-            visibilities=should_plot("data"),
+        if should_plot("subplot_fit_dirty_images"):
+            fit_plotter.subplot_fit_dirty_images()
+
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
             chi_squared_map_real=should_plot("chi_squared_map"),
             normalized_residual_map_real=should_plot("normalized_residual_map"),
             residual_map_imag=should_plot("residual_map"),
             chi_squared_map_imag=should_plot("chi_squared_map"),
             normalized_residual_map_imag=should_plot("normalized_residual_map"),
             dirty_image=should_plot("data"),
@@ -73,60 +77,56 @@
             dirty_signal_to_noise_map=should_plot("signal_to_noise_map"),
             dirty_model_image=should_plot("model_data"),
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
-                    chi_squared_map_real=True,
-                    normalized_residual_map_real=True,
-                    residual_map_imag=True,
-                    chi_squared_map_imag=True,
-                    normalized_residual_map_imag=True,
-                    dirty_image=True,
-                    dirty_noise_map=True,
-                    dirty_signal_to_noise_map=True,
-                    dirty_model_image=True,
-                    dirty_residual_map=True,
-                    dirty_normalized_residual_map=True,
-                    dirty_chi_squared_map=True,
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
-                    chi_squared_map_real=True,
-                    normalized_residual_map_real=True,
-                    residual_map_imag=True,
-                    chi_squared_map_imag=True,
-                    normalized_residual_map_imag=True,
-                    dirty_image=True,
-                    dirty_noise_map=True,
-                    dirty_signal_to_noise_map=True,
-                    dirty_model_image=True,
-                    dirty_residual_map=True,
-                    dirty_normalized_residual_map=True,
-                    dirty_chi_squared_map=True,
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
+                chi_squared_map_real=True,
+                normalized_residual_map_real=True,
+                residual_map_imag=True,
+                chi_squared_map_imag=True,
+                normalized_residual_map_imag=True,
+                dirty_image=True,
+                dirty_noise_map=True,
+                dirty_signal_to_noise_map=True,
+                dirty_model_image=True,
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
+                dirty_model_image=True,
+                dirty_residual_map=True,
+                dirty_normalized_residual_map=True,
+                dirty_chi_squared_map=True,
+            )
```

### Comparing `autolens-2023.3.27.1/autolens/interferometer/plot/fit_interferometer_plotters.py` & `autolens-2023.7.7.2/autolens/interferometer/plot/fit_interferometer_plotters.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,36 +77,34 @@
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
             residuals_symmetric_cmap=residuals_symmetric_cmap,
         )
 
         self.subplot = self._fit_interferometer_meta_plotter.subplot
-        self.subplot_fit_interferometer = (
-            self._fit_interferometer_meta_plotter.subplot_fit_interferometer
-        )
+        #   self.subplot_fit = self._fit_interferometer_meta_plotter.subplot_fit
         self.subplot_fit_dirty_images = (
             self._fit_interferometer_meta_plotter.subplot_fit_dirty_images
         )
 
     def get_visuals_2d_real_space(self) -> aplt.Visuals2D:
-        return self.get_2d.via_mask_from(mask=self.fit.interferometer.real_space_mask)
+        return self.get_2d.via_mask_from(mask=self.fit.dataset.real_space_mask)
 
     @property
     def tracer(self) -> Tracer:
         return self.fit.tracer_linear_light_profiles_to_light_profiles
 
     @property
     def tracer_plotter(self) -> TracerPlotter:
         """
         Returns an `TracerPlotter` corresponding to the `Tracer` in the `FitImaging`.
         """
         return TracerPlotter(
             tracer=self.tracer,
-            grid=self.fit.interferometer.grid,
+            grid=self.fit.dataset.grid,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.visuals_2d,
             include_2d=self.include_2d,
         )
 
     def inversion_plotter_of_plane(self, plane_index: int) -> aplt.InversionPlotter:
         """
@@ -128,20 +126,79 @@
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.tracer_plotter.get_visuals_2d_of_plane(
                 plane_index=plane_index
             ),
             include_2d=self.include_2d,
         )
 
+    def subplot_fit(self):
+        """
+        Standard subplot of the attributes of the plotter's `FitImaging` object.
+        """
+
+        self.open_subplot_figure(number_subplots=12)
+
+        self.figures_2d(amplitudes_vs_uv_distances=True)
+
+        self.mat_plot_1d.subplot_index = 2
+        self.mat_plot_2d.subplot_index = 2
+
+        self.figures_2d(dirty_image=True)
+        self.figures_2d(dirty_signal_to_noise_map=True)
+        self.figures_2d(dirty_model_image=True)
+        self.figures_2d(image=True)
+
+        self.mat_plot_1d.subplot_index = 6
+        self.mat_plot_2d.subplot_index = 6
+
+        self.figures_2d(normalized_residual_map_real=True)
+        self.figures_2d(normalized_residual_map_imag=True)
+
+        self.mat_plot_1d.subplot_index = 8
+        self.mat_plot_2d.subplot_index = 8
+
+        final_plane_index = len(self.fit.tracer.planes) - 1
+
+        self.set_title(label="Source Plane (Zoomed)")
+        self.figures_2d_of_planes(plane_index=final_plane_index, plane_image=True)
+        self.set_title(label=None)
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
+        self.set_title(label="Source Plane (No Zoom)")
+        self.figures_2d_of_planes(
+            plane_index=final_plane_index,
+            plane_image=True,
+            zoom_to_brightest=False,
+        )
+
+        self.set_title(label=None)
+
+        self.mat_plot_2d.output.subplot_to_figure(auto_filename="subplot_fit")
+        self.close_subplot_figure()
+
     def figures_2d(
         self,
-        visibilities: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
-        model_visibilities: bool = False,
+        amplitudes_vs_uv_distances: bool = False,
+        model_data: bool = False,
         residual_map_real: bool = False,
         residual_map_imag: bool = False,
         normalized_residual_map_real: bool = False,
         normalized_residual_map_imag: bool = False,
         chi_squared_map_real: bool = False,
         chi_squared_map_imag: bool = False,
         image: bool = False,
@@ -157,21 +214,21 @@
         Plots the individual attributes of the plotter's `FitInterferometer` object in 1D and 2D.
 
         The API is such that every plottable attribute of the `Interferometer` object is an input parameter of type
         bool of the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
-        visibilities
+        data
             Whether to make a 2D plot (via `scatter`) of the visibility data.
         noise_map
             Whether to make a 2D plot (via `scatter`) of the noise-map.
         signal_to_noise_map
             Whether to make a 2D plot (via `scatter`) of the signal-to-noise-map.
-        model_visibilities
+        model_data
             Whether to make a 2D plot (via `scatter`) of the model visibility data.
         residual_map_real
             Whether to make a 1D plot (via `plot`) of the real component of the residual map.
         residual_map_imag
             Whether to make a 1D plot (via `plot`) of the imaginary component of the residual map.
         normalized_residual_map_real
             Whether to make a 1D plot (via `plot`) of the real component of the normalized residual map.
@@ -193,18 +250,19 @@
             Whether to make a 2D plot (via `imshow`) of the dirty residual map.
         dirty_normalized_residual_map
             Whether to make a 2D plot (via `imshow`) of the dirty normalized residual map.
         dirty_chi_squared_map
             Whether to make a 2D plot (via `imshow`) of the dirty chi-squared map.
         """
         self._fit_interferometer_meta_plotter.figures_2d(
-            visibilities=visibilities,
+            data=data,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
-            model_visibilities=model_visibilities,
+            amplitudes_vs_uv_distances=amplitudes_vs_uv_distances,
+            model_data=model_data,
             residual_map_real=residual_map_real,
             residual_map_imag=residual_map_imag,
             normalized_residual_map_real=normalized_residual_map_real,
             normalized_residual_map_imag=normalized_residual_map_imag,
             chi_squared_map_real=chi_squared_map_real,
             chi_squared_map_imag=chi_squared_map_imag,
             dirty_image=dirty_image,
@@ -213,23 +271,25 @@
             dirty_model_image=dirty_model_image,
             dirty_residual_map=dirty_residual_map,
             dirty_normalized_residual_map=dirty_normalized_residual_map,
             dirty_chi_squared_map=dirty_chi_squared_map,
         )
 
         if image:
-
             if self.fit.inversion is None:
                 self.tracer_plotter.figures_2d(image=True)
             else:
                 inversion_plotter = self.inversion_plotter_of_plane(plane_index=1)
                 inversion_plotter.figures_2d(reconstructed_image=True)
 
     def figures_2d_of_planes(
-        self, plane_index: Optional[int] = None, plane_image: bool = False
+        self,
+        plane_index: Optional[int] = None,
+        plane_image: bool = False,
+        zoom_to_brightest: bool = True,
     ):
         """
         Plots images representing each individual `Plane` in the fit's `Tracer` in 2D, which are computed via the
         plotter's 2D grid object.
 
         These images subtract or omit the contribution of other planes in the plane, such that plots showing
         each individual plane are made.
@@ -241,45 +301,47 @@
         ----------
         plane_index
             The index of the plane which figures are plotted for.
         plane_image
             Whether to make a 2D plot (via `imshow`) of the image of a plane in its source-plane (e.g. unlensed).
             Depending on how the fit is performed, this could either be an image of light profiles of the reconstruction
             of an `Inversion`.
+        zoom_to_brightest
+            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
+            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
         """
         if plane_image:
-
             if not self.tracer.planes[plane_index].has(cls=aa.Pixelization):
-
                 self.tracer_plotter.figures_2d_of_planes(
-                    plane_image=True, plane_index=plane_index
+                    plane_image=True,
+                    plane_index=plane_index,
+                    zoom_to_brightest=zoom_to_brightest,
                 )
 
             elif self.tracer.planes[plane_index].has(cls=aa.Pixelization):
-
                 inversion_plotter = self.inversion_plotter_of_plane(plane_index=1)
                 inversion_plotter.figures_2d_of_pixelization(
-                    pixelization_index=0, reconstruction=True
+                    pixelization_index=0,
+                    reconstruction=True,
+                    zoom_to_brightest=zoom_to_brightest,
                 )
 
     def subplot_fit_real_space(self):
         """
         Standard subplot of the real-space attributes of the plotter's `FitInterferometer` object.
 
         Depending on whether `LightProfile`'s or an `Inversion` are used to represent galaxies in the `Tracer`,
         different methods are called to create these real-space images.
         """
         if self.fit.inversion is None:
-
             self.tracer_plotter.subplot(
                 image=True, source_plane=True, auto_filename="subplot_fit_real_space"
             )
 
         elif self.fit.inversion is not None:
-
             self.open_subplot_figure(number_subplots=2)
 
             inversion_plotter = self.inversion_plotter_of_plane(plane_index=1)
 
             inversion_plotter.figures_2d_of_pixelization(
                 pixelization_index=0, reconstructed_image=True
             )
```

### Comparing `autolens-2023.3.27.1/autolens/lens/mock/mock_tracer.py` & `autolens-2023.7.7.2/autolens/lens/mock/mock_tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 class MockTracer:
     def __init__(
         self, traced_grid_2d_list_from=None, sparse_image_plane_grid_pg_list=None
     ):
-
         self.sparse_image_plane_grid_pg_list = sparse_image_plane_grid_pg_list
         self._traced_grid_2d_list_from = traced_grid_2d_list_from
 
     def traced_grid_2d_list_from(self, grid):
-
         return self._traced_grid_2d_list_from
 
 
 class MockTracerPoint(MockTracer):
     def __init__(
         self,
         sparse_image_plane_grid_pg_list=None,
         traced_grid=None,
         attribute=None,
         profile=None,
         magnification=None,
         einstein_radius=None,
         einstein_mass=None,
     ):
-
         super().__init__(
             sparse_image_plane_grid_pg_list=sparse_image_plane_grid_pg_list
         )
 
         self.positions = traced_grid
 
         self.attribute = attribute
```

### Comparing `autolens-2023.3.27.1/autolens/lens/plot/ray_tracing_plotters.py` & `autolens-2023.7.7.2/autolens/lens/plot/ray_tracing_plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         """
 
         from autogalaxy.profiles.light.linear import (
             LightProfileLinear,
         )
 
         if tracer.has(cls=LightProfileLinear):
-
             raise exc.raise_linear_light_profile_in_plot(
                 plotter_type=self.__class__.__name__, model_obj="Plane"
             )
 
         super().__init__(
             mat_plot_1d=mat_plot_1d,
             visuals_1d=visuals_1d,
@@ -152,15 +151,14 @@
         magnification
             Whether to make a 2D plot (via `imshow`) of the magnification.
         contribution_map
             Whether to make a 2D plot (via `imshow`) of the contribution map.
         """
 
         if image:
-
             self.mat_plot_2d.plot_array(
                 array=self.tracer.image_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(title="Image", filename="image_2d"),
             )
 
         if source_plane:
@@ -173,15 +171,14 @@
             potential=potential,
             deflections_y=deflections_y,
             deflections_x=deflections_x,
             magnification=magnification,
         )
 
         if contribution_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.tracer.contribution_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title="Contribution Map", filename="contribution_map_2d"
                 ),
             )
@@ -206,14 +203,15 @@
         return [plane_index]
 
     def figures_2d_of_planes(
         self,
         plane_image: bool = False,
         plane_grid: bool = False,
         plane_index: Optional[int] = None,
+        zoom_to_brightest: bool = True,
     ):
         """
         Plots source-plane images (e.g. the unlensed light) each individual `Plane` in the plotter's `Tracer` in 2D,
         which are computed via the plotter's 2D grid object.
 
         The API is such that every plottable attribute of the `Plane` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
@@ -224,31 +222,32 @@
             Whether to make a 2D plot (via `imshow`) of the image of the plane in the soure-plane (e.g. its
             unlensed light).
         plane_grid
             Whether to make a 2D plot (via `scatter`) of the lensed (y,x) coordinates of the plane in the
             source-plane.
         plane_index
             If input, plots for only a single plane based on its index in the tracer are created.
+        zoom_to_brightest
+            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
+            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
         """
         plane_indexes = self.plane_indexes_from(plane_index=plane_index)
 
         for plane_index in plane_indexes:
-
             plane_plotter = self.plane_plotter_from(plane_index=plane_index)
 
             if plane_image:
-
                 plane_plotter.figures_2d(
                     plane_image=True,
+                    zoom_to_brightest=zoom_to_brightest,
                     title_suffix=f" Of Plane {plane_index}",
                     filename_suffix=f"_of_plane_{plane_index}",
                 )
 
             if plane_grid:
-
                 plane_plotter.figures_2d(
                     plane_grid=True,
                     title_suffix=f" Of Plane {plane_index}",
                     filename_suffix=f"_of_plane_{plane_index}",
                 )
 
     def subplot(
@@ -269,31 +268,31 @@
 
         The API is such that every plottable attribute of the `Tracer` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
         image
-            Whether or not to include a 2D plot (via `imshow`) of the image of tracer in its image-plane (e.g. after
+            Whether to include a 2D plot (via `imshow`) of the image of tracer in its image-plane (e.g. after
             lensing).
         source_plane
-            Whether or not to include a 2D plot (via `imshow`) of the image of the tracer in the source-plane (e.g. its
+            Whether to include a 2D plot (via `imshow`) of the image of the tracer in the source-plane (e.g. its
             unlensed light).
         convergence
-            Whether or not to include a 2D plot (via `imshow`) of the convergence.
+            Whether to include a 2D plot (via `imshow`) of the convergence.
         potential
-            Whether or not to include a 2D plot (via `imshow`) of the potential.
+            Whether to include a 2D plot (via `imshow`) of the potential.
         deflections_y
-            Whether or not to include a 2D plot (via `imshow`) of the y component of the deflection angles.
+            Whether to include a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
-            Whether or not to include a 2D plot (via `imshow`) of the x component of the deflection angles.
+            Whether to include a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
-            Whether or not to include a 2D plot (via `imshow`) of the magnification.
+            Whether to include a 2D plot (via `imshow`) of the magnification.
         contribution_map
-            Whether or not to include a 2D plot (via `imshow`) of the contribution map.
+            Whether to include a 2D plot (via `imshow`) of the contribution map.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
 
         self._subplot_custom_plot(
             image=image,
             source_plane=source_plane,
@@ -328,15 +327,14 @@
         images at each plane.
         """
         number_subplots = self.tracer.total_planes
 
         self.open_subplot_figure(number_subplots=number_subplots)
 
         for plane_index in range(0, self.tracer.total_planes):
-
             plane_plotter = self.plane_plotter_from(plane_index=plane_index)
             plane_plotter.figures_2d(
                 image=True, title_suffix=f" Of Plane {plane_index}"
             )
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename=f"subplot_lensed_images"
@@ -357,15 +355,14 @@
 
         plane_plotter = self.plane_plotter_from(plane_index=0)
         plane_plotter.figures_2d(image=True, title_suffix=" Of Plane 0")
 
         self.mat_plot_2d.subplot_index += 1
 
         for plane_index in range(1, self.tracer.total_planes):
-
             plane_plotter = self.plane_plotter_from(plane_index=plane_index)
             plane_plotter.figures_2d(
                 image=True, title_suffix=f" Of Plane {plane_index}"
             )
             plane_plotter.figures_2d(
                 plane_image=True, title_suffix=f" Of Plane {plane_index}"
             )
```

### Comparing `autolens-2023.3.27.1/autolens/lens/ray_tracing.py` & `autolens-2023.7.7.2/autolens/lens/ray_tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,31 +53,29 @@
     @classmethod
     def from_galaxies(
         cls,
         galaxies,
         cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15(),
         profiling_dict: Optional[Dict] = None,
     ):
-
         planes = ag.util.plane.planes_via_galaxies_from(
             galaxies=galaxies, profiling_dict=profiling_dict
         )
 
-        return Tracer(planes=planes, cosmology=cosmology, profiling_dict=profiling_dict)
+        return cls(planes=planes, cosmology=cosmology, profiling_dict=profiling_dict)
 
     @classmethod
     def sliced_tracer_from(
         cls,
         lens_galaxies,
         line_of_sight_galaxies,
         source_galaxies,
         planes_between_lenses,
         cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15(),
     ):
-
         """Ray-tracer for a lens system with any number of planes.
 
         The redshift of these planes are specified by the input parameters *lens_redshifts* and \
          *slices_between_main_planes*. Every galaxy is placed in its closest plane in redshift-space.
 
         To perform multi-plane ray-tracing, a cosmology must be supplied so that deflection-angles can be rescaled \
         according to the lens-geometry of the multi-plane system. All galaxies input to the tracer must therefore \
@@ -248,22 +246,20 @@
         )
 
     @aa.grid_dec.grid_2d_to_structure
     @aa.profile_func
     def image_2d_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> aa.Array2D:
-
         return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
 
     @aa.grid_dec.grid_2d_to_structure_list
     def image_2d_list_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> List[aa.Array2D]:
-
         traced_grid_list = self.traced_grid_2d_list_from(
             grid=grid, plane_index_limit=self.upper_plane_index_with_light_profile
         )
 
         image_2d_list = [
             self.planes[plane_index].image_2d_from(
                 grid=traced_grid_list[plane_index], operated_only=operated_only
@@ -282,15 +278,15 @@
     def galaxy_image_2d_dict_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> Dict[ag.Galaxy, np.ndarray]:
         """
         Returns a dictionary associating every `Galaxy` object in the `Tracer` with its corresponding 2D image, using
         the instance of each galaxy as the dictionary keys.
 
-        This object is used for hyper-features, which use the image of each galaxy in a model-fit in order to
+        This object is used for adaptive-features, which use the image of each galaxy in a model-fit in order to
         adapt quantities like a pixelization or regularization scheme to the surface brightness of the galaxies being
         fitted.
 
         By inheriting from `OperateImageGalaxies` functions which apply operations of this dictionary are accessible,
         for example convolving every image with a PSF or applying a Fourier transform to create a galaxy-visibilities
         dictionary.
 
@@ -304,21 +300,20 @@
         A dictionary associated every galaxy in the tracer with its corresponding 2D image.
         """
 
         galaxy_image_2d_dict = dict()
 
         traced_grid_list = self.traced_grid_2d_list_from(grid=grid)
 
-        for (plane_index, plane) in enumerate(self.planes):
+        for plane_index, plane in enumerate(self.planes):
             image_2d_list = plane.image_2d_list_from(
                 grid=traced_grid_list[plane_index], operated_only=operated_only
             )
 
-            for (galaxy_index, galaxy) in enumerate(plane.galaxies):
-
+            for galaxy_index, galaxy in enumerate(plane.galaxies):
                 galaxy_image_2d_dict[galaxy] = image_2d_list[galaxy_index]
 
         return galaxy_image_2d_dict
 
     @aa.grid_dec.grid_2d_to_vector_yx
     @aa.grid_dec.grid_2d_to_structure
     def deflections_yx_2d_from(
@@ -336,15 +331,14 @@
         return sum([plane.deflections_yx_2d_from(grid=grid) for plane in self.planes])
 
     @aa.grid_dec.grid_2d_to_vector_yx
     @aa.grid_dec.grid_2d_to_structure
     def deflections_between_planes_from(
         self, grid: aa.type.Grid2DLike, plane_i=0, plane_j=-1
     ) -> Union[aa.VectorYX2D, aa.VectorYX2DIrregular]:
-
         traced_grids_list = self.traced_grid_2d_list_from(grid=grid)
 
         return traced_grids_list[plane_i] - traced_grids_list[plane_j]
 
     @aa.grid_dec.grid_2d_to_structure
     def convergence_2d_from(self, grid: aa.type.Grid2DLike) -> aa.Array2D:
         return sum([plane.convergence_2d_from(grid=grid) for plane in self.planes])
@@ -370,49 +364,14 @@
         ]
         return [
             plane_index
             for plane_index in plane_indexes_with_inversions
             if plane_index is not None
         ]
 
-    def hyper_noise_map_from(self, noise_map: aa.Array2D) -> aa.Array2D:
-        return sum(self.hyper_noise_map_list_from(noise_map=noise_map))
-
-    def hyper_noise_map_list_from(self, noise_map: aa.Array2D) -> List[aa.Array2D]:
-        return [
-            plane.hyper_noise_map_from(noise_map=noise_map) for plane in self.planes
-        ]
-
-    @property
-    def contribution_map(self) -> Optional[aa.Array2D]:
-
-        contribution_map_list = self.contribution_map_list
-
-        contribution_map_list = [i for i in contribution_map_list if i is not None]
-
-        if contribution_map_list:
-            return sum(contribution_map_list)
-
-    @property
-    def contribution_map_list(self) -> List[aa.Array2D]:
-
-        contribution_map_list = []
-
-        for plane in self.planes:
-
-            if plane.contribution_map is not None:
-
-                contribution_map_list.append(plane.contribution_map)
-
-            else:
-
-                contribution_map_list.append(None)
-
-        return contribution_map_list
-
     @property
     def perform_inversion(self) -> bool:
         """
         Returns a bool specifying whether this fit object performs an inversion.
 
         This is based on whether any of the galaxies in the `model_obj` have a `Pixelization` or `LightProfileLinear`
         object, in which case an inversion is performed.
@@ -444,15 +403,14 @@
 
         GridIrregular2D(grid=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1), (centre_y_2, centre_x_2)])
 
         This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
         """
 
         def extract(value, name):
-
             try:
                 return getattr(value, name)
             except (AttributeError, IndexError):
                 return None
 
         attributes = [
             extract(value, attr_name)
@@ -496,23 +454,21 @@
 
         If a Profile does not have a certain entry, it is replaced with a None, although the nones can be removed
         by setting `filter_nones=True`.
 
         This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
         """
         if filter_nones:
-
             return [
                 plane.extract_attribute(cls=cls, attr_name=attr_name)
                 for plane in self.planes
                 if plane.extract_attribute(cls=cls, attr_name=attr_name) is not None
             ]
 
         else:
-
             return [
                 plane.extract_attribute(cls=cls, attr_name=attr_name)
                 for plane in self.planes
             ]
 
     def extract_attributes_of_galaxies(self, cls, attr_name, filter_nones=False):
         """
@@ -553,23 +509,21 @@
 
         If a Profile does not have a certain entry, it is replaced with a None, although the nones can be removed
         by setting `filter_nones=True`.
 
         This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
         """
         if filter_nones:
-
             return [
                 galaxy.extract_attribute(cls=cls, attr_name=attr_name)
                 for galaxy in self.galaxies
                 if galaxy.extract_attribute(cls=cls, attr_name=attr_name) is not None
             ]
 
         else:
-
             return [
                 galaxy.extract_attribute(cls=cls, attr_name=attr_name)
                 for galaxy in self.galaxies
             ]
 
     def extract_profile(self, profile_name):
         """
@@ -652,9 +606,8 @@
                             exposure_time=exposure_time,
                             background_sky_level=background_sky_level,
                             psf=psf,
                         )
 
     @aa.profile_func
     def convolve_via_convolver(self, image, blurring_image, convolver):
-
         return convolver.convolve_image(image=image, blurring_image=blurring_image)
```

### Comparing `autolens-2023.3.27.1/autolens/lens/ray_tracing_util.py` & `autolens-2023.7.7.2/autolens/lens/ray_tracing_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     """
 
     traced_grid_list = []
     traced_deflection_list = []
 
     plane_redshifts = [plane.redshift for plane in planes]
 
-    for (plane_index, plane) in enumerate(planes):
-
+    for plane_index, plane in enumerate(planes):
         scaled_grid = grid.copy()
 
         if plane_index > 0:
             for previous_plane_index in range(plane_index):
                 scaling_factor = cosmology.scaling_factor_between_redshifts_from(
                     redshift_0=plane_redshifts[previous_plane_index],
                     redshift_1=plane.redshift,
@@ -129,23 +128,21 @@
     plane_index_with_redshift = [
         plane_index
         for plane_index, plane in enumerate(planes)
         if plane.redshift == redshift
     ]
 
     if plane_index_with_redshift:
-
         traced_grid_list = traced_grid_2d_list_from(
             planes=planes, grid=grid, cosmology=cosmology
         )
 
         return traced_grid_list[plane_index_with_redshift[0]]
 
     for plane_index, plane_redshift in enumerate(plane_redshifts):
-
         if redshift < plane_redshift:
             plane_index_insert = plane_index
 
     planes.insert(plane_index_insert, ag.Plane(redshift=redshift, galaxies=[]))
 
     traced_grid_list = traced_grid_2d_list_from(
         planes=planes, grid=grid, cosmology=cosmology
```

### Comparing `autolens-2023.3.27.1/autolens/lens/subhalo.py` & `autolens-2023.7.7.2/autolens/lens/subhalo.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from autolens.aggregator.fit_imaging import _fit_imaging_from
 
 
 class SubhaloResult:
     def __init__(
         self, grid_search_result, result_no_subhalo, stochastic_log_likelihoods=None
     ):
-
         self.grid_search_result = grid_search_result
         self.result_no_subhalo = result_no_subhalo
         self.stochastic_log_likelihoods = stochastic_log_likelihoods
 
     @property
     def fit_imaging_before(self):
         try:
@@ -28,15 +27,14 @@
                 fit=self.result_no_subhalo,
                 galaxies=self.result_no_subhalo.instance.galaxies,
             )
         except AttributeError:
             return self.result_no_subhalo.max_log_likelihood_fit
 
     def _subhalo_array_from(self, values_native) -> aa.Array2D:
-
         values_reshaped = [value for values in values_native for value in values]
 
         return aa.Array2D.from_yx_and_values(
             y=[centre[0] for centre in self.grid_search_result.physical_centres_lists],
             x=[centre[1] for centre in self.grid_search_result.physical_centres_lists],
             values=values_reshaped,
             pixel_scales=self.grid_search_result.physical_step_sizes,
@@ -45,40 +43,36 @@
 
     def subhalo_detection_array_from(
         self,
         use_log_evidences: bool = True,
         use_stochastic_log_likelihoods: bool = False,
         relative_to_no_subhalo: bool = True,
     ) -> aa.Array2D:
-
         try:
             samples_no_subhalo = self.result_no_subhalo["samples"]
         except TypeError:
             samples_no_subhalo = self.result_no_subhalo.samples
 
         if (not use_log_evidences) and (not use_stochastic_log_likelihoods):
-
             values_native = self.grid_search_result.log_likelihoods_native
             values_native[values_native == None] = np.nan
 
             if relative_to_no_subhalo:
                 values_native -= (
                     samples_no_subhalo.max_log_likelihood_sample.log_likelihood
                 )
 
         elif use_log_evidences and not use_stochastic_log_likelihoods:
-
             values_native = self.grid_search_result.log_evidences_native
             values_native[values_native == None] = np.nan
 
             if relative_to_no_subhalo:
                 values_native -= samples_no_subhalo.log_evidence
 
         else:
-
             values_native = self.stochastic_log_evidences_native
             values_native[values_native == None] = np.nan
 
             if relative_to_no_subhalo:
                 values_native -= np.median(
                     self.result_no_subhalo["stochastic_log_likelihoods"]
                 )
@@ -86,42 +80,39 @@
         return self._subhalo_array_from(values_native=values_native)
 
     def subhalo_mass_array_from(self):
         return self._subhalo_array_from(values_native=self.masses_native)
 
     @property
     def stochastic_log_evidences_native(self) -> List[float]:
-
         return self.grid_search_result._list_to_native(
             lst=self.stochastic_log_likelihoods
         )
 
     def instance_list_via_results_from(self, results):
         return [
             None if result.samples.median_pdf() is None else result.samples.median_pdf()
             for result in results
         ]
 
     @property
     def masses_native(self) -> List[float]:
-
         instance_list = self.instance_list_via_results_from(
             results=self.grid_search_result.results
         )
 
         return self.grid_search_result._list_to_native(
             [
                 None if instance is None else instance.galaxies.subhalo.mass.mass_at_200
                 for instance in instance_list
             ]
         )
 
     @property
     def centres_native(self) -> aa.Grid2D:
-
         instance_list = self.instance_list_via_results_from(
             results=self.grid_search_result.results
         )
 
         centres_native = np.zeros(
             (self.grid_search_result.shape[0], self.grid_search_result.shape[1], 2)
         )
@@ -188,87 +179,78 @@
             fit=self.fit_imaging_detect,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=visuals_2d,
             include_2d=self.include_2d,
         )
 
     def detection_array_from(self, remove_zeros: bool = False):
-
         detection_array = self.subhalo_result.subhalo_detection_array_from(
             use_log_evidences=self.use_log_evidences,
             use_stochastic_log_likelihoods=self.use_stochastic_log_likelihoods,
             relative_to_no_subhalo=True,
         )
 
         if remove_zeros:
-
             detection_array[detection_array < 0.0] = 0.0
 
         return detection_array
 
     def figure_with_detection_overlay(
         self,
         image: bool = False,
         remove_zeros: bool = False,
         show_median: bool = True,
         overwrite_title=False,
         transpose_array=False,
     ):
-
         array_overlay = self.detection_array_from(remove_zeros=remove_zeros)
 
         median_detection = np.round(np.nanmedian(array_overlay), 2)
 
         # Due to bug with flipped subhalo inv, can remove one day
 
         if transpose_array:
             array_overlay = np.fliplr(np.fliplr(array_overlay.native).T)
 
         visuals_2d = self.visuals_2d + self.visuals_2d.__class__(
             array_overlay=array_overlay,
             mass_profile_centres=self.subhalo_result.centres_native,
         )
 
-        fit_imaging_plotter = self.fit_imaging_detect_plotter_from(
-            visuals_2d=visuals_2d
-        )
+        fit_plotter = self.fit_imaging_detect_plotter_from(visuals_2d=visuals_2d)
 
         if show_median:
             if overwrite_title:
-                fit_imaging_plotter.set_title(label=f"Image {median_detection}")
+                fit_plotter.set_title(label=f"Image {median_detection}")
 
-        #   fit_imaging_plotter.figures_2d(image=image)
-        fit_imaging_plotter.figures_2d_of_planes(plane_index=-1, subtracted_image=True)
+        #   fit_plotter.figures_2d(image=image)
+        fit_plotter.figures_2d_of_planes(plane_index=-1, subtracted_image=True)
 
     def figure_with_mass_overlay(self, image: bool = False, transpose_array=False):
-
         array_overlay = self.subhalo_result.subhalo_mass_array_from()
 
         # Due to bug with flipped subhalo inv, can remove one day
 
         if transpose_array:
             array_overlay = np.fliplr(np.fliplr(array_overlay.native).T)
 
         visuals_2d = self.visuals_2d + self.visuals_2d.__class__(
             array_overlay=array_overlay,
             mass_profile_centres=self.subhalo_result.centres_native,
         )
 
-        fit_imaging_plotter = self.fit_imaging_detect_plotter_from(
-            visuals_2d=visuals_2d
-        )
+        fit_plotter = self.fit_imaging_detect_plotter_from(visuals_2d=visuals_2d)
 
-        fit_imaging_plotter.figures_2d_of_planes(plane_index=-1, subtracted_image=True)
+        fit_plotter.figures_2d_of_planes(plane_index=-1, subtracted_image=True)
 
     def subplot_detection_imaging(self, remove_zeros: bool = False):
-
         self.open_subplot_figure(number_subplots=4)
 
         self.set_title("Image")
-        self.fit_imaging_detect_plotter.figures_2d(image=True)
+        self.fit_imaging_detect_plotter.figures_2d(data=True)
 
         self.set_title("Signal-To-Noise Map")
         self.fit_imaging_detect_plotter.figures_2d(signal_to_noise_map=True)
         self.set_title(None)
 
         self.mat_plot_2d.plot_array(
             array=self.detection_array_from(remove_zeros=remove_zeros),
```

### Comparing `autolens-2023.3.27.1/autolens/lens/to_inversion.py` & `autolens-2023.7.7.2/autolens/lens/to_inversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         noise_map: Optional[Union[aa.Array2D, aa.VisibilitiesNoiseMap]] = None,
         w_tilde: Optional[Union[aa.WTildeImaging, aa.WTildeInterferometer]] = None,
         settings_pixelization=aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads=Preloads(),
         profiling_dict: Optional[Dict] = None,
     ):
-
         self.tracer = tracer
 
         super().__init__(
             dataset=dataset,
             data=data,
             noise_map=noise_map,
             w_tilde=w_tilde,
@@ -46,15 +45,14 @@
     def traced_grid_2d_list_of_inversion(self) -> List[aa.type.Grid2DLike]:
         return self.tracer.traced_grid_2d_list_from(grid=self.dataset.grid_pixelization)
 
     @cached_property
     def lp_linear_func_list_galaxy_dict(
         self,
     ) -> Dict[ag.LightProfileLinearObjFuncList, ag.Galaxy]:
-
         if not self.tracer.perform_inversion:
             return {}
 
         lp_linear_galaxy_dict_list = {}
 
         traced_grids_of_planes_list = self.tracer.traced_grid_2d_list_from(
             grid=self.dataset.grid
@@ -65,16 +63,15 @@
                 grid=self.dataset.blurring_grid
             )
         else:
             traced_blurring_grids_of_planes_list = [None] * len(
                 traced_grids_of_planes_list
             )
 
-        for (plane_index, plane) in enumerate(self.planes):
-
+        for plane_index, plane in enumerate(self.planes):
             plane_to_inversion = ag.PlaneToInversion(
                 plane=plane,
                 dataset=self.dataset,
                 grid=traced_grids_of_planes_list[plane_index],
                 blurring_grid=traced_blurring_grids_of_planes_list[plane_index],
             )
 
@@ -89,32 +86,31 @@
 
         return lp_linear_galaxy_dict_list
 
     def cls_pg_list_from(self, cls: Type) -> List:
         return [plane.cls_list_from(cls=cls) for plane in self.planes]
 
     @cached_property
-    def hyper_galaxy_image_pg_list(self) -> List:
+    def adapt_galaxy_image_pg_list(self) -> List:
         return [
-            plane.hyper_galaxies_with_pixelization_image_list for plane in self.planes
+            plane.adapt_galaxies_with_pixelization_image_list for plane in self.planes
         ]
 
     @cached_property
     @aa.profile_func
     def sparse_image_plane_grid_pg_list(self) -> List[List]:
         """
         Specific pixelizations, like the `VoronoiMagnification`, begin by determining what will become its the
         source-pixel centres by calculating them  in the image-plane. The `VoronoiBrightnessImage` pixelization
         performs a KMeans clustering.
         """
 
         sparse_image_plane_grid_list_of_planes = []
 
         for plane in self.planes:
-
             plane_to_inversion = ag.PlaneToInversion(
                 plane=plane,
                 grid_pixelization=self.dataset.grid,
                 settings_pixelization=self.settings_pixelization,
             )
 
             sparse_image_plane_grid_list = (
@@ -132,37 +128,32 @@
         angles at (y,x) coordinate on the grid from the galaxy mass profiles and then ray-trace them from the
         image-plane to the source plane.
         """
         if (
             self.preloads.sparse_image_plane_grid_pg_list is None
             or self.settings_pixelization.is_stochastic
         ):
-
             sparse_image_plane_grid_pg_list = self.sparse_image_plane_grid_pg_list
 
         else:
-
             sparse_image_plane_grid_pg_list = (
                 self.preloads.sparse_image_plane_grid_pg_list
             )
 
         traced_sparse_grid_pg_list = []
 
-        for (plane_index, plane) in enumerate(self.planes):
-
+        for plane_index, plane in enumerate(self.planes):
             if sparse_image_plane_grid_pg_list[plane_index] is None:
                 traced_sparse_grid_pg_list.append(None)
             else:
-
                 traced_sparse_grids_list = []
 
                 for sparse_image_plane_grid in sparse_image_plane_grid_pg_list[
                     plane_index
                 ]:
-
                     try:
                         traced_sparse_grids_list.append(
                             self.tracer.traced_grid_2d_list_from(
                                 grid=sparse_image_plane_grid
                             )[plane_index]
                         )
                     except AttributeError:
@@ -170,15 +161,14 @@
 
                 traced_sparse_grid_pg_list.append(traced_sparse_grids_list)
 
         return traced_sparse_grid_pg_list, sparse_image_plane_grid_pg_list
 
     @cached_property
     def mapper_galaxy_dict(self) -> Dict[aa.AbstractMapper, ag.Galaxy]:
-
         mapper_galaxy_dict = {}
 
         if self.preloads.traced_grids_of_planes_for_inversion is None:
             traced_grids_of_planes_list = self.traced_grid_2d_list_of_inversion
         else:
             traced_grids_of_planes_list = (
                 self.preloads.traced_grids_of_planes_for_inversion
@@ -191,60 +181,56 @@
             ) = self.traced_sparse_grid_pg_list
         else:
             traced_sparse_grids_list_of_planes = (
                 self.preloads.traced_sparse_grids_list_of_planes
             )
             sparse_image_plane_grid_list = self.preloads.sparse_image_plane_grid_list
 
-        for (plane_index, plane) in enumerate(self.planes):
-
+        for plane_index, plane in enumerate(self.planes):
             if plane.has(cls=aa.Pixelization):
-
                 plane_to_inversion = ag.PlaneToInversion(
                     plane=plane,
                     grid_pixelization=traced_grids_of_planes_list[plane_index],
                     settings_pixelization=self.settings_pixelization,
                     preloads=self.preloads,
                 )
 
                 galaxies_with_pixelization_list = plane.galaxies_with_cls_list_from(
                     cls=aa.Pixelization
                 )
 
                 for mapper_index in range(
                     len(traced_sparse_grids_list_of_planes[plane_index])
                 ):
-
                     pixelization_list = self.cls_pg_list_from(cls=aa.Pixelization)
 
                     mapper = plane_to_inversion.mapper_from(
                         mesh=pixelization_list[plane_index][mapper_index].mesh,
                         regularization=pixelization_list[plane_index][
                             mapper_index
                         ].regularization,
                         source_plane_mesh_grid=traced_sparse_grids_list_of_planes[
                             plane_index
                         ][mapper_index],
                         image_plane_mesh_grid=sparse_image_plane_grid_list[plane_index][
                             mapper_index
                         ],
-                        hyper_galaxy_image=self.hyper_galaxy_image_pg_list[plane_index][
+                        adapt_galaxy_image=self.adapt_galaxy_image_pg_list[plane_index][
                             mapper_index
                         ],
                     )
 
                     galaxy = galaxies_with_pixelization_list[mapper_index]
 
                     mapper_galaxy_dict[mapper] = galaxy
 
         return mapper_galaxy_dict
 
     @cached_property
     def inversion(self):
-
         inversion = inversion_unpacked_from(
             dataset=self.dataset,
             data=self.data,
             noise_map=self.noise_map,
             w_tilde=self.w_tilde,
             linear_obj_list=self.linear_obj_list,
             settings=self.settings_inversion,
```

### Comparing `autolens-2023.3.27.1/autolens/plot/__init__.py` & `autolens-2023.7.7.2/autolens/plot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 from autogalaxy.quantity.plot.fit_quantity_plotters import FitQuantityPlotter
 
 from autogalaxy.imaging.plot.fit_imaging_plotters import FitImagingPlotter
 from autogalaxy.interferometer.plot.fit_interferometer_plotters import (
     FitInterferometerPlotter,
 )
 from autogalaxy.plane.plot.plane_plotters import PlanePlotter
-from autogalaxy.galaxy.plot.hyper_galaxy_plotters import HyperPlotter
+from autogalaxy.galaxy.plot.adapt_plotters import AdaptPlotter
 
 from autolens.point.plot.point_dataset_plotters import PointDatasetPlotter
 from autolens.point.plot.point_dataset_plotters import PointDictPlotter
 from autolens.imaging.plot.fit_imaging_plotters import FitImagingPlotter
 from autolens.interferometer.plot.fit_interferometer_plotters import (
     FitInterferometerPlotter,
 )
```

### Comparing `autolens-2023.3.27.1/autolens/plot/abstract_plotters.py` & `autolens-2023.7.7.2/autolens/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/plot/get_visuals/one_d.py` & `autolens-2023.7.7.2/autolens/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/plot/get_visuals/two_d.py` & `autolens-2023.7.7.2/autolens/plot/get_visuals/two_d.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,28 +94,36 @@
 
         tangential_critical_curves = None
         radial_critical_curves = None
         tangential_caustics = None
         radial_caustics = None
 
         if plane_index == 0:
-
             tangential_critical_curves = self.get(
                 "tangential_critical_curves",
                 tracer.tangential_critical_curve_list_from(grid=grid),
                 "tangential_critical_curves",
             )
 
-            radial_critical_curves = self.get(
-                "radial_critical_curves",
-                tracer.radial_critical_curve_list_from(grid=grid),
-                "radial_critical_curves",
+            radial_critical_curves = None
+
+            radial_critical_curve_area_list = (
+                tracer.radial_critical_curve_area_list_from(grid=grid)
             )
 
-        if plane_index == 1:
+            if any(
+                [area > grid.pixel_scale for area in radial_critical_curve_area_list]
+            ):
+                radial_critical_curves = self.get(
+                    "radial_critical_curves",
+                    tracer.radial_critical_curve_list_from(grid=grid),
+                    "radial_critical_curves",
+                )
+
+        if plane_index > 0:
             tangential_caustics = self.get(
                 "tangential_caustics",
                 tracer.tangential_caustic_list_from(grid=grid),
                 "tangential_caustics",
             )
 
             radial_caustics = self.get(
```

### Comparing `autolens-2023.3.27.1/autolens/point/fit_point/fluxes.py` & `autolens-2023.7.7.2/autolens/point/fit_point/fluxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         name: str,
         fluxes: aa.ArrayIrregular,
         noise_map: aa.ArrayIrregular,
         positions: aa.Grid2DIrregular,
         tracer: Tracer,
         point_profile: Optional[ag.ps.Point] = None,
     ):
-
         super().__init__(dataset=fluxes)
 
         self.tracer = tracer
 
         self._noise_map = noise_map
 
         self.name = name
@@ -67,15 +66,14 @@
 
         For multi-plane ray-tracing with more than 2 planes, the deflection function determines the index of the
         plane with the last mass profile such that the deflection function does not perform unecessary computations
         beyond this plane.
         """
 
         if len(self.tracer.planes) > 2:
-
             upper_plane_index = self.tracer.extract_plane_index_of_profile(
                 profile_name=self.name
             )
 
             return partial(
                 self.tracer.deflections_between_planes_from,
                 plane_i=0,
```

### Comparing `autolens-2023.3.27.1/autolens/point/fit_point/max_separation.py` & `autolens-2023.7.7.2/autolens/point/fit_point/max_separation.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/point/fit_point/point_dataset.py` & `autolens-2023.7.7.2/autolens/point/fit_point/point_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,33 +17,29 @@
     NumbaException = AttributeError
 
 
 class FitPointDataset:
     def __init__(
         self, point_dataset: PointDataset, tracer: Tracer, point_solver: PointSolver
     ):
-
         self.point_dataset = point_dataset
 
         point_profile = tracer.extract_profile(profile_name=point_dataset.name)
 
         try:
-
             if isinstance(point_profile, ag.ps.PointSourceChi):
-
                 self.positions = FitPositionsSource(
                     name=point_dataset.name,
                     positions=point_dataset.positions,
                     noise_map=point_dataset.positions_noise_map,
                     tracer=tracer,
                     point_profile=point_profile,
                 )
 
             else:
-
                 self.positions = FitPositionsImage(
                     name=point_dataset.name,
                     positions=point_dataset.positions,
                     noise_map=point_dataset.positions_noise_map,
                     point_solver=point_solver,
                     tracer=tracer,
                     point_profile=point_profile,
@@ -51,29 +47,26 @@
 
         except exc.PointExtractionException:
             self.positions = None
         except (AttributeError, NumbaException) as e:
             raise exc.FitException from e
 
         try:
-
             self.flux = FitFluxes(
                 name=point_dataset.name,
                 fluxes=point_dataset.fluxes,
                 noise_map=point_dataset.fluxes_noise_map,
                 positions=point_dataset.positions,
                 tracer=tracer,
             )
 
         except exc.PointExtractionException:
-
             self.flux = None
 
     @property
     def log_likelihood(self) -> float:
-
         log_likelihood_positions = (
             self.positions.log_likelihood if self.positions is not None else 0.0
         )
         log_likelihood_flux = self.flux.log_likelihood if self.flux is not None else 0.0
 
         return log_likelihood_positions + log_likelihood_flux
```

### Comparing `autolens-2023.3.27.1/autolens/point/fit_point/point_dict.py` & `autolens-2023.7.7.2/autolens/point/fit_point/point_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         """
 
         self.tracer = tracer
 
         super().__init__()
 
         for key, point_dataset in point_dict.items():
-
             self[key] = FitPointDataset(
                 point_dataset=point_dataset, tracer=tracer, point_solver=point_solver
             )
 
     @property
     def log_likelihood(self) -> float:
         return sum(fit.log_likelihood for fit in self.values())
```

### Comparing `autolens-2023.3.27.1/autolens/point/fit_point/positions_image.py` & `autolens-2023.7.7.2/autolens/point/fit_point/positions_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
     @property
     def model_positions(self) -> aa.Grid2DIrregular:
         return self.model_data
 
     @property
     def residual_map(self) -> aa.ArrayIrregular:
-
         residual_positions = self.positions - self.model_positions
 
         return residual_positions.distances_to_coordinate_from(coordinate=(0.0, 0.0))
 
     @property
     def chi_squared(self) -> float:
         """
```

### Comparing `autolens-2023.3.27.1/autolens/point/fit_point/positions_source.py` & `autolens-2023.7.7.2/autolens/point/fit_point/positions_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,17 @@
         """
         Returns the model positions, which are computed via the point solver.
 
         It if common for many more image-plane positions to be computed than actual positions in the dataset. In this
         case, each data point is paired with its closest model position.
         """
         if len(self.tracer.planes) <= 2:
-
             deflections = self.tracer.deflections_yx_2d_from(grid=self.positions)
 
         else:
-
             upper_plane_index = self.tracer.extract_plane_index_of_profile(
                 profile_name=self.name
             )
 
             deflections = self.tracer.deflections_between_planes_from(
                 grid=self.positions, plane_i=0, plane_j=upper_plane_index
             )
@@ -89,15 +87,14 @@
 
     @property
     def model_positions(self) -> aa.Grid2DIrregular:
         return self.model_data
 
     @property
     def residual_map(self) -> aa.ArrayIrregular:
-
         return self.model_positions.distances_to_coordinate_from(
             coordinate=self.source_plane_coordinate
         )
 
     @property
     def chi_squared(self) -> float:
         """
```

### Comparing `autolens-2023.3.27.1/autolens/point/model/analysis.py` & `autolens-2023.7.7.2/autolens/point/model/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,46 +57,44 @@
         AnalysisLensing.__init__(
             self=self, settings_lens=settings_lens, cosmology=cosmology
         )
 
         self.point_dict = point_dict
 
         self.solver = solver
-        self.imaging = imaging
+        self.dataset = imaging
 
     def log_likelihood_function(self, instance):
         """
         Determine the fit of the strong lens system of lens galaxies and source galaxies to the point source data.
 
         Parameters
         ----------
         instance
             A model instance with attributes
 
         Returns
         -------
         fit : Fit
-            A fractional value indicating how well this model fit and the model masked_imaging itself
+            A fractional value indicating how well this model fit and the model masked_dataset itself
         """
         try:
             fit = self.fit_positions_for(instance=instance)
             return fit.log_likelihood
         except (AttributeError, ValueError, TypeError, NumbaException) as e:
             raise exc.FitException from e
 
     def fit_positions_for(self, instance):
-
         tracer = self.tracer_via_instance_from(instance=instance)
 
         return FitPointDict(
             point_dict=self.point_dict, tracer=tracer, point_solver=self.solver
         )
 
     def visualize(self, paths, instance, during_analysis):
-
         tracer = self.tracer_via_instance_from(instance=instance)
 
         visualizer = Visualizer(visualize_path=paths.image_path)
 
     def make_result(
         self,
         samples: af.SamplesPDF,
@@ -104,9 +102,8 @@
         sigma=1.0,
         use_errors=True,
         use_widths=False,
     ):
         return ResultPoint(samples=samples, model=model, analysis=self)
 
     def save_attributes_for_aggregator(self, paths: af.DirectoryPaths):
-
         paths.save_object("dataset", self.point_dict)
```

### Comparing `autolens-2023.3.27.1/autolens/point/plot/fit_point_plotters.py` & `autolens-2023.7.7.2/autolens/point/plot/fit_point_plotters.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,15 @@
     def get_visuals_1d(self) -> aplt.Visuals1D:
         return self.visuals_1d
 
     def get_visuals_2d(self) -> aplt.Visuals2D:
         return self.visuals_2d
 
     def figures_2d(self, positions: bool = False, fluxes: bool = False):
-
         if positions:
-
             visuals_2d = self.get_visuals_2d()
 
             visuals_2d += visuals_2d.__class__(
                 positions=self.fit.positions.model_positions
             )
 
             self.mat_plot_2d.plot_grid(
@@ -58,23 +56,20 @@
         # nasty hack to ensure subplot index between 2d and 1d plots are syncs. Need a refactor that mvoes subplot
         # functionality out of mat_plot and into plotter.
 
         if (
             self.mat_plot_1d.subplot_index is not None
             and self.mat_plot_2d.subplot_index is not None
         ):
-
             self.mat_plot_1d.subplot_index = max(
                 self.mat_plot_1d.subplot_index, self.mat_plot_2d.subplot_index
             )
 
         if fluxes:
-
             if self.fit.point_dataset.fluxes is not None:
-
                 visuals_1d = self.get_visuals_1d()
 
                 visuals_1d += visuals_1d.__class__(
                     model_fluxes=self.fit.flux.model_fluxes
                 )
 
                 self.mat_plot_1d.plot_yx(
@@ -89,18 +84,17 @@
                     plot_axis_type_override="errorbar",
                 )
 
     def subplot(
         self,
         positions: bool = False,
         fluxes: bool = False,
-        auto_filename: str = "subplot_fit_point",
+        auto_filename: str = "subplot_fit",
     ):
-
         self._subplot_custom_plot(
             positions=positions,
             fluxes=fluxes,
             auto_labels=aplt.AutoLabels(filename=auto_filename),
         )
 
-    def subplot_fit_point(self):
+    def subplot_fit(self):
         self.subplot(positions=True, fluxes=True)
```

### Comparing `autolens-2023.3.27.1/autolens/point/plot/point_dataset_plotters.py` & `autolens-2023.7.7.2/autolens/point/plot/point_dataset_plotters.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,61 +30,54 @@
     def get_visuals_1d(self) -> aplt.Visuals1D:
         return self.visuals_1d
 
     def get_visuals_2d(self) -> aplt.Visuals2D:
         return self.visuals_2d
 
     def point_dataset_plotter_from(self, name):
-
         return PointDatasetPlotter(
             point_dataset=self.point_dict[name],
             mat_plot_1d=self.mat_plot_1d,
             include_1d=self.include_1d,
             visuals_1d=self.visuals_1d,
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
         )
 
     def subplot(self):
-
         self.open_subplot_figure(number_subplots=len(self.point_dict))
 
         for name in self.point_dict.keys():
-
             point_dataset_plotter = self.point_dataset_plotter_from(name=name)
 
             point_dataset_plotter.figures_2d(positions=True, fluxes=True)
 
         self.mat_plot_2d.output.subplot_to_figure(auto_filename="subplot_point_dict")
 
         self.close_subplot_figure()
 
     def subplot_positions(self):
-
         self.open_subplot_figure(number_subplots=len(self.point_dict))
 
         for name in self.point_dict.keys():
-
             point_dataset_plotter = self.point_dataset_plotter_from(name=name)
 
             point_dataset_plotter.figures_2d(positions=True)
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename="subplot_point_dict_positions"
         )
 
         self.close_subplot_figure()
 
     def subplot_fluxes(self):
-
         self.open_subplot_figure(number_subplots=len(self.point_dict))
 
         for name in self.point_dict.keys():
-
             point_dataset_plotter = self.point_dataset_plotter_from(name=name)
 
             point_dataset_plotter.figures_2d(fluxes=True)
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename="subplot_point_dict_fluxes"
         )
@@ -117,17 +110,15 @@
     def get_visuals_1d(self) -> aplt.Visuals1D:
         return self.visuals_1d
 
     def get_visuals_2d(self) -> aplt.Visuals2D:
         return self.visuals_2d
 
     def figures_2d(self, positions: bool = False, fluxes: bool = False):
-
         if positions:
-
             self.mat_plot_2d.plot_grid(
                 grid=self.point_dataset.positions,
                 y_errors=self.point_dataset.positions_noise_map,
                 x_errors=self.point_dataset.positions_noise_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"{self.point_dataset.name} Positions",
@@ -139,23 +130,20 @@
         # nasty hack to ensure subplot index between 2d and 1d plots are syncs. Need a refactor that mvoes subplot
         # functionality out of mat_plot and into plotter.
 
         if (
             self.mat_plot_1d.subplot_index is not None
             and self.mat_plot_2d.subplot_index is not None
         ):
-
             self.mat_plot_1d.subplot_index = max(
                 self.mat_plot_1d.subplot_index, self.mat_plot_2d.subplot_index
             )
 
         if fluxes:
-
             if self.point_dataset.fluxes is not None:
-
                 self.mat_plot_1d.plot_yx(
                     y=self.point_dataset.fluxes,
                     y_errors=self.point_dataset.fluxes_noise_map,
                     visuals_1d=self.get_visuals_1d(),
                     auto_labels=aplt.AutoLabels(
                         title=f" {self.point_dataset.name} Fluxes",
                         filename="point_dataset_fluxes",
@@ -164,18 +152,17 @@
                     plot_axis_type_override="errorbar",
                 )
 
     def subplot(
         self,
         positions: bool = False,
         fluxes: bool = False,
-        auto_filename="subplot_point_dataset",
+        auto_filename="subplot_dataset",
     ):
-
         self._subplot_custom_plot(
             positions=positions,
             fluxes=fluxes,
             auto_labels=aplt.AutoLabels(filename=auto_filename),
         )
 
-    def subplot_point_dataset(self):
+    def subplot_dataset(self):
         self.subplot(positions=True, fluxes=True)
```

### Comparing `autolens-2023.3.27.1/autolens/point/point_dataset.py` & `autolens-2023.7.7.2/autolens/point/point_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
             A dictionary where the keys are the `name` entries of each `PointDataset` and the values are
             the corresponding instance of the `PointDataset` class.
         """
 
         super().__init__()
 
         for point_dataset in point_dataset_list:
-
             self[point_dataset.name] = point_dataset
 
     @property
     def positions_list(self):
         return [point_dataset.positions for keys, point_dataset in self.items()]
 
     @property
@@ -163,22 +162,20 @@
         -------
         A collection of point source datasets.
         """
         return cls(map(PointDataset.from_dict, dicts))
 
     @classmethod
     def from_json(cls, file_path):
-
         with open(file_path) as infile:
             dicts = json.load(infile)
 
         return cls.from_dicts(dicts=dicts)
 
     def output_to_json(self, file_path, overwrite=False):
-
         file_dir = os.path.split(file_path)[0]
 
         if not path.exists(file_dir):
             os.makedirs(file_dir)
 
         if overwrite and path.exists(file_path):
             os.remove(file_path)
```

### Comparing `autolens-2023.3.27.1/autolens/point/point_solver.py` & `autolens-2023.7.7.2/autolens/point/point_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,23 @@
         self,
         use_upscaling=True,
         upscale_factor=2,
         magnification_threshold=0.1,
         distance_to_source_centre=None,
         distance_to_mass_profile_centre=None,
     ):
-
         self.use_upscaling = use_upscaling
         self.upscale_factor = upscale_factor
         self.magnification_threshold = magnification_threshold
         self.distance_to_source_centre = distance_to_source_centre
         self.distance_to_mass_profile_centre = distance_to_mass_profile_centre
 
     def grid_with_points_below_magnification_threshold_removed(
         self, lensing_obj, deflections_func, grid
     ):
-
         magnifications = np.abs(
             lensing_obj.magnification_2d_via_hessian_from(
                 grid=grid, buffer=grid.pixel_scale, deflections_func=deflections_func
             )
         )
 
         grid_mag = []
@@ -60,23 +58,21 @@
             An object which has a `deflection_2d_from` method for performing lensing calculations, for example a
             `MassProfile`, _Galaxy_, `Plane` or `Tracer`.
         grid : autoarray.Grid2DIrregularUniform or ndarray
             A gridd of (y,x) Cartesian coordinates for which their distances to the mass profile centres are computed,
             with points within the threshold removed.
         """
         if self.distance_to_mass_profile_centre is not None:
-
             pixel_scales = grid.pixel_scales
 
             centres = lensing_obj.extract_attribute(
                 cls=ag.mp.MassProfile, attr_name="centre"
             )
 
             for centre in centres.in_list:
-
                 distances_1d = np.sqrt(
                     np.square(grid[:, 0] - centre[0])
                     + np.square(grid[:, 1] - centre[1])
                 )
 
                 grid = grid_outside_distance_mask_from(
                     distances_1d=distances_1d,
@@ -332,15 +328,14 @@
 
         if len(grid) == 0:
             return None
         else:
             return [tuple(coordinate) for coordinate in grid]
 
     def solve(self, lensing_obj, source_plane_coordinate, upper_plane_index=None):
-
         if upper_plane_index is None:
             deflections_func = lensing_obj.deflections_yx_2d_from
         else:
             deflections_func = partial(
                 lensing_obj.deflections_between_planes_from,
                 plane_i=0,
                 plane_j=upper_plane_index,
@@ -361,34 +356,31 @@
         coordinates_list = self.grid_with_points_below_magnification_threshold_removed(
             lensing_obj=lensing_obj,
             deflections_func=deflections_func,
             grid=coordinates_list,
         )
 
         if not self.use_upscaling:
-
             coordinates_list = self.grid_within_distance_of_source_plane_centre(
                 deflection_func=deflections_func,
                 grid=aa.Grid2DIrregularUniform(
                     values=coordinates_list, pixel_scales=self.grid.pixel_scales
                 ),
                 source_plane_coordinate=source_plane_coordinate,
                 distance=self.distance_to_source_centre,
             )
 
             return aa.Grid2DIrregular(values=coordinates_list)
 
         pixel_scale = self.grid.pixel_scale
 
         while pixel_scale > self.pixel_scale_precision:
-
             refined_coordinates_list = []
 
             for coordinate in coordinates_list:
-
                 refined_coordinates = self.refined_coordinates_from(
                     deflections_func=deflections_func,
                     coordinate=coordinate,
                     pixel_scale=pixel_scale,
                     source_plane_coordinate=source_plane_coordinate,
                 )
 
@@ -419,36 +411,32 @@
         )
 
         return aa.Grid2DIrregular(values=coordinates_list)
 
 
 @aa.util.numba.jit()
 def grid_remove_duplicates(grid):
-
     tolerance = 1e-8
 
     grid_no_duplicates = []
 
     separations = np.zeros((grid.shape[0], grid.shape[0]))
 
     for i in range(grid.shape[0]):
         for j in range(grid.shape[0]):
             separations[i, j] = np.sqrt(
                 np.square(grid[i, 0] - grid[j, 0]) + np.square(grid[i, 1] - grid[j, 1])
             )
             separations[i, i] = tolerance * 2
 
     for i in range(grid.shape[0]):
-
         is_duplicate = False
 
         for j in range(grid.shape[0]):
-
             if separations[i, j] < tolerance:
-
                 is_duplicate = True
                 separations[i, j] = tolerance * 2
                 separations[j, i] = tolerance * 2
 
         if not is_duplicate:
             grid_no_duplicates.append((grid[i, 0], grid[i, 1]))
 
@@ -499,15 +487,14 @@
         edge_start = -int(edge / 2)
         edge_end = int(edge / 2)
         y_odd_pixel_scale = 0.0
         x_odd_pixel_scale = 0.0
 
     for y in range(edge_start, edge_end):
         for x in range(edge_start, edge_end):
-
             grid_slim[grid_index, 0] = (
                 coordinate[0]
                 - y * pixel_scales_upscaled[0]
                 - y_upscale_half
                 + y_odd_pixel_scale
             )
             grid_slim[grid_index, 1] = (
@@ -519,15 +506,14 @@
             grid_index += 1
 
     return grid_slim
 
 
 @aa.util.numba.jit()
 def pair_coordinate_to_closest_pixel_on_grid(coordinate, grid_slim):
-
     squared_distances = np.square(grid_slim[:, 0] - coordinate[0]) + np.square(
         grid_slim[:, 1] - coordinate[1]
     )
 
     return np.argmin(squared_distances)
 
 
@@ -574,17 +560,15 @@
     has_neighbors = np.full(shape=shape_slim, fill_value=False)
     neighbors_1d = np.full(shape=(shape_slim, 8), fill_value=-1.0)
 
     index = 0
 
     for y in range(shape_of_edge):
         for x in range(shape_of_edge):
-
             if y > 0 and x > 0 and y < shape_of_edge - 1 and x < shape_of_edge - 1:
-
                 neighbors_1d[index, 0] = index - shape_of_edge - 1
                 neighbors_1d[index, 1] = index - shape_of_edge
                 neighbors_1d[index, 2] = index - shape_of_edge + 1
                 neighbors_1d[index, 3] = index - 1
                 neighbors_1d[index, 4] = index + 1
                 neighbors_1d[index, 5] = index + shape_of_edge - 1
                 neighbors_1d[index, 6] = index + shape_of_edge
@@ -616,51 +600,46 @@
     has_neighbors
         An array of bools, where `True` means a pixel has 8 neighbors and `False` means it has less than 8 and is not
         compared to the source distance.
     """
     peaks_list = []
 
     for grid_index in range(grid_slim.shape[0]):
-
         if has_neighbors[grid_index]:
-
             distance = distance_1d[grid_index]
 
             if (
                 distance <= distance_1d[neighbors[grid_index, 0]]
                 and distance <= distance_1d[neighbors[grid_index, 1]]
                 and distance <= distance_1d[neighbors[grid_index, 2]]
                 and distance <= distance_1d[neighbors[grid_index, 3]]
                 and distance <= distance_1d[neighbors[grid_index, 4]]
                 and distance <= distance_1d[neighbors[grid_index, 5]]
                 and distance <= distance_1d[neighbors[grid_index, 6]]
                 and distance <= distance_1d[neighbors[grid_index, 7]]
             ):
-
                 peaks_list.append(grid_slim[grid_index])
 
     return peaks_list
 
 
 @aa.util.numba.jit()
 def grid_within_distance(distances_1d, grid_slim, within_distance):
-
     grid_within_size = 0
 
     for grid_index in range(grid_slim.shape[0]):
         if distances_1d[grid_index] < within_distance:
             grid_within_size += 1
 
     grid_within = np.zeros(shape=(grid_within_size, 2))
 
     grid_within_index = 0
 
     for grid_index in range(grid_slim.shape[0]):
         if distances_1d[grid_index] < within_distance:
-
             grid_within[grid_within_index, :] = grid_slim[grid_index, :]
             grid_within_index += 1
 
     return grid_within
 
 
 @aa.util.numba.jit()
```

### Comparing `autolens-2023.3.27.1/autolens/quantity/fit_quantity.py` & `autolens-2023.7.7.2/autolens/quantity/fit_quantity.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/quantity/model/analysis.py` & `autolens-2023.7.7.2/autolens/quantity/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/autolens/quantity/model/result.py` & `autolens-2023.7.7.2/autolens/quantity/model/result.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return self.analysis.dataset.grid
 
     @property
     def max_log_likelihood_tracer(self) -> Tracer:
         """
         An instance of a `Tracer` corresponding to the maximum log likelihood model inferred by the non-linear search.
 
-        If a dataset is fitted the hyper images of the hyper dataset must first be associated with each galaxy.
+        If a dataset is fitted the adapt images of the adapt dataset must first be associated with each galaxy.
         """
         return self.analysis.tracer_via_instance_from(instance=self.instance_copy)
 
     @property
     def max_log_likelihood_fit(self) -> ag.FitQuantity:
         """
         An instance of a `FitQuantity` corresponding to the maximum log likelihood model inferred by the non-linear
```

### Comparing `autolens-2023.3.27.1/autolens/util/__init__.py` & `autolens-2023.7.7.2/autolens/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 )
 from autoarray.inversion.inversion.interferometer import (
     inversion_interferometer_util as inversion_interferometer,
 )
 from autoarray.operators import transformer_util as transformer
 from autogalaxy.analysis import model_util as model
 from autogalaxy.util import error_util as error
-from autogalaxy.util import plane_util as plane
+from autogalaxy.plane import plane_util as plane
+from autogalaxy.analysis import chaining_util as chaining
 
 from autolens.lens import ray_tracing_util as ray_tracing
```

### Comparing `autolens-2023.3.27.1/autolens.egg-info/SOURCES.txt` & `autolens-2023.7.7.2/autolens.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 autolens/analysis/settings.py
 autolens/analysis/setup.py
 autolens/analysis/visualizer.py
 autolens/analysis/mock/__init__.py
 autolens/analysis/mock/mock_result.py
 autolens/config/general.yaml
 autolens/config/non_linear.yaml
-autolens/config/visualize.yaml
+autolens/config/visualize/plots.yaml
 autolens/imaging/__init__.py
 autolens/imaging/fit_imaging.py
 autolens/imaging/imaging.py
 autolens/imaging/mock/__init__.py
 autolens/imaging/mock/mock_fit_imaging.py
 autolens/imaging/model/__init__.py
 autolens/imaging/model/analysis.py
@@ -101,15 +101,14 @@
 docs/index.rst
 docs/requirements.txt
 docs/_templates/custom-class-template.rst
 docs/_templates/custom_module_template.rst
 docs/advanced/chaining.rst
 docs/advanced/database.rst
 docs/advanced/graphical.rst
-docs/advanced/hyper_mode.rst
 docs/advanced/slam.rst
 docs/api/data.rst
 docs/api/fitting.rst
 docs/api/galaxy.rst
 docs/api/light.rst
 docs/api/mass.rst
 docs/api/modeling.rst
@@ -128,15 +127,14 @@
 docs/general/images/maresca_fig1.png
 docs/general/images/maresca_fig2.png
 docs/general/images/maresca_fig7.png
 docs/howtolens/chapter_1_introduction.rst
 docs/howtolens/chapter_2_lens_modeling.rst
 docs/howtolens/chapter_3_search_chaining.rst
 docs/howtolens/chapter_4_pixelizations.rst
-docs/howtolens/chapter_5_hyper_mode.rst
 docs/howtolens/chapter_optional.rst
 docs/howtolens/howtolens.rst
 docs/installation/conda.rst
 docs/installation/numba.rst
 docs/installation/overview.rst
 docs/installation/pip.rst
 docs/installation/source.rst
```

### Comparing `autolens-2023.3.27.1/docs/_templates/custom-class-template.rst` & `autolens-2023.7.7.2/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/_templates/custom_module_template.rst` & `autolens-2023.7.7.2/docs/_templates/custom_module_template.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/advanced/database.rst` & `autolens-2023.7.7.2/docs/advanced/database.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _database:
 
 Database
 --------
 
 The default behaviour of **PyAutoLens** is for model-fitting results to be output to hard-disc in folders, which are
-straight forward to navigate and manually check the lens modeling results. For small samples of lenses this is
+straight forward to navigate and manually check the  modeling results. For small samples of lenses this is
 sufficient, however many users have a need to perform many model fits to large lens datasets, making the manual
 inspection of results time consuming.
 
 **PyAutoLens**'s database feature outputs all model-fitting results as a sqlite3 (https://docs.python.org/3/library/sqlite3.html)
 relational database, such that all results can be efficiently loaded into a Jupyter notebook or Python script for
 inspection, analysis and interpretation. This database supports advanced querying, so that specific
 model-fits (e.g., which fit a certain lens model or dataset) can be loaded.
@@ -62,15 +62,15 @@
 
         print(max(samples.log_likelihood))
 
 This object (and all objects loaded by the ``Aggregator``) are returned as a generator (as opposed to a list,
 dictionary or other Python type). This is because generators do not store large arrays or classes in memory until they
 are used, ensuring that when we are manipulating large sets of results we do not run out of memory!
 
-We can iterate over the samples to print the maximum log likelihood lens model of every fit:
+We can iterate over the samples to print the maximum log likelihood model of every fit:
 
 .. code-block:: python
 
     for samps in agg.values("samples"):
 
         instance = samps.max_log_likelihood()
```

### Comparing `autolens-2023.3.27.1/docs/advanced/graphical.rst` & `autolens-2023.7.7.2/docs/advanced/graphical.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 distribution (e.g. a Gaussian). It is the parameters of this parent distribution that are shared
 across the dataset, and these are the parameters we ultimately wish to infer to understand the global behaviour of the
 model.
 
 An example of such a model might be determining the parent distribution from which the density slope of strong lens
 galaxies are drawn.
 
-A full description of graphical and hierarchical models can be found `in the graphical package of the autolens_workspace <https://github.com/Jammy2211/autolens_workspace/tree/release/notebooks/imaging/graphical>`_.
+A full description of graphical and hierarchical models can be found `in the graphical package of the autolens_workspace <https://github.com/Jammy2211/autolens_workspace/tree/release/notebooks/imaging/advanced/graphical>`_.
```

### Comparing `autolens-2023.3.27.1/docs/api/data.rst` & `autolens-2023.7.7.2/docs/api/data.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/api/galaxy.rst` & `autolens-2023.7.7.2/docs/api/galaxy.rst`

 * *Files 26% similar despite different names*

```diff
@@ -25,21 +25,8 @@
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

### Comparing `autolens-2023.3.27.1/docs/api/light.rst` & `autolens-2023.7.7.2/docs/api/light.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/api/mass.rst` & `autolens-2023.7.7.2/docs/api/mass.rst`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
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

### Comparing `autolens-2023.3.27.1/docs/api/pixelization.rst` & `autolens-2023.7.7.2/docs/api/pixelization.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/api/plot.rst` & `autolens-2023.7.7.2/docs/api/plot.rst`

 * *Files 1% similar despite different names*

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

### Comparing `autolens-2023.3.27.1/docs/api/source.rst` & `autolens-2023.7.7.2/docs/api/source.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/conf.py` & `autolens-2023.7.7.2/docs/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `autolens-2023.3.27.1/docs/general/citations.rst` & `autolens-2023.7.7.2/docs/general/citations.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/configs.rst` & `autolens-2023.7.7.2/docs/general/configs.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/credits.rst` & `autolens-2023.7.7.2/docs/general/credits.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/demagnified_solutions.rst` & `autolens-2023.7.7.2/docs/general/demagnified_solutions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 The penalty term is created and passed to an ``Analysis`` object as follows:
 
 .. code-block:: python
 
     positions_likelihood = al.PositionsLHPenalty(positions=positions, threshold=0.3)
 
     analysis = al.AnalysisImaging(
-        dataset=imaging, positions_likelihood=positions_likelihood
+        dataset=dataset, positions_likelihood=positions_likelihood
     )
 
 The threshold of 0.5" is large. For an accurate lens model we would anticipate the positions trace within < 0.01" of
 one another. However, we only want the threshold to aid the non-linear with the choice of mass model in the intial fit
 and remove demagnified solutions.
 
 Resampling
@@ -108,15 +108,15 @@
 guessing and rejecting mass models.
 
 .. code-block:: python
 
     positions_likelihood = al.PositionsLHResample(positions=positions, threshold=0.3)
 
     analysis = al.AnalysisImaging(
-        dataset=imaging, positions_likelihood=positions_likelihood
+        dataset=dataset, positions_likelihood=positions_likelihood
     )
 
 Auto Position Updates
 ---------------------
 
 There are a number of downsides to having to input the mulitple images positions manually:
 
@@ -164,12 +164,12 @@
         )
 
 This is often used to set up new ``Analysis`` objects with a positions penalty concisely:
 
 .. code-block:: python
 
     analysis_2 = al.AnalysisImaging(
-        dataset=imaging,
+        dataset=dataset,
         positions_likelihood=result_1.positions_likelihood_from(
             factor=3.0, minimum_threshold=0.2
         ),
     )
```

### Comparing `autolens-2023.3.27.1/docs/general/images/maresca_fig1.png` & `autolens-2023.7.7.2/docs/general/images/maresca_fig1.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/images/maresca_fig2.png` & `autolens-2023.7.7.2/docs/general/images/maresca_fig2.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/images/maresca_fig7.png` & `autolens-2023.7.7.2/docs/general/images/maresca_fig7.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/likelihood_function.rst` & `autolens-2023.7.7.2/docs/general/likelihood_function.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/general/model_cookbook.rst` & `autolens-2023.7.7.2/docs/general/model_cookbook.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,34 @@
 -----------------
 
 A simple lens model we can compose has a lens galaxy with a Sersic light profile, Isothermal mass profile and
 source galaxy with a Sersic light profile:
 
 .. code-block:: python
 
+    # Lens:
+
     bulge = af.Model(al.lp.Sersic)
     mass = af.Model(al.mp.Isothermal)
 
     lens = af.Model(
         al.Galaxy,
         redshift=0.5,
         bulge=bulge,
         mass=mass,
     )
 
+    # Source:
+
     bulge = af.Model(al.lp.Sersic)
 
     source = af.Model(al.Galaxy, redshift=1.0, bulge=bulge)
 
+    # Overall Lens Model:
+
     model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
 The redshifts in the above model are used to determine which galaxy is the lens and which is the source.
 
 The model ``prior_count`` tells us the total number of free parameters (which are fitted for via a non-linear search),
 which in this case is 19 (7 from the lens Sersic, 5 from the lens Isothermal and 7 from the source Sersic).
 
@@ -87,14 +93,16 @@
 More Complex Lens Models
 ------------------------
 
 The API above can be easily extended to compose lens models where each galaxy has multiple light or mass profiles:
 
 .. code-block:: python
 
+    # Lens:
+
     bulge = af.Model(al.lp.Sersic)
     disk = af.Model(al.lp.Exponential)
 
     mass = af.Model(al.mp.Isothermal)
     shear = af.Model(al.mp.ExternalShear)
 
     lens = af.Model(
@@ -102,19 +110,23 @@
         redshift=0.5,
         bulge=bulge,
         disk=disk,
         mass=mass,
         shear=shear,
     )
 
+    # Source:
+
     bulge = af.Model(al.lp.Sersic)
     disk = af.Model(al.lp.Exponential)
 
     source = af.Model(al.Galaxy, redshift=1.0, bulge=bulge, disk=disk)
 
+    # Overall Lens Model:
+
     model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
 The use of the words `bulge`, `disk`, `mass` and `shear` above are arbitrary. They can be replaced with any name you
 like, e.g. `bulge_0`, `bulge_1`, `mass_0`, `mass_1`, and the model will still behave in the same way.
 
 The API can also be extended to compose lens models where there are multiple galaxies:
 
@@ -136,22 +148,28 @@
     lens_1 = af.Model(
         al.Galaxy,
         redshift=0.5,
         bulge=bulge,
         mass=mass,
     )
 
+    # Source 0:
+
     bulge = af.Model(al.lp.Sersic)
 
     source_0 = af.Model(al.Galaxy, redshift=1.0, bulge=bulge)
 
+    # Source 1 :
+
     bulge = af.Model(al.lp.Sersic)
 
     source_1 = af.Model(al.Galaxy, redshift=1.0, bulge=bulge)
 
+    # Overall Lens Model:
+
     model = af.Collection(
         galaxies=af.Collection(
             lens_0=lens_0,
             lens_1=lens_1, 
             source_0=source_0,
             source_1=source_1
         )
@@ -165,15 +183,16 @@
 
 Concise API
 -----------
 
 If a light or mass profile is passed directly to the `af.Model` of a galaxy, it is automatically assigned to be a
 `af.Model` component of the galaxy.
 
-This means we can write the model above comprising multiple light and mass profiles more concisely as follows:
+This means we can write the model above comprising multiple light and mass profiles more concisely as follows (also
+removing the comments reading Lens / Source / Overall Lens Model to make the code more readable):
 
 .. code-block:: python
 
     lens = af.Model(
         al.Galaxy,
         redshift=0.5,
         bulge=al.lp.Sersic,
@@ -187,21 +206,24 @@
         redshift=1.0,
         bulge=al.lp.Sersic,
         disk=al.lp.Exponential
     )
 
     model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
+
 Prior Customization
 -------------------
 
 We can customize the priors of the lens model component individual parameters as follows:
 
 .. code-block:: python
 
+    # Lens:
+
     bulge = af.Model(al.lp.Sersic)
     bulge.intensity = af.LogUniformPrior(lower_limit=1e-4, upper_limit=1e4)
     bulge.sersic_index = af.GaussianPrior(mean=4.0, sigma=1.0, lower_limit=1.0, upper_limit=8.0)
 
     mass = af.Model(al.mp.Isothermal)
     mass.centre.centre_0 = af.GaussianPrior(mean=0.0, sigma=0.1, lower_limit=-0.5, upper_limit=0.5)
     mass.centre.centre_1 = af.GaussianPrior(mean=0.0, sigma=0.1, lower_limit=-0.5, upper_limit=0.5)
@@ -212,26 +234,32 @@
         redshift=0.5,
         bulge=bulge,
         mass=mass,
     )
 
     bulge = af.Model(al.lp.Sersic)
 
+    # Source
+
     source = af.Model(al.Galaxy, redshift=1.0, bulge=bulge)
     source.effective_radius = af.GaussianPrior(mean=0.1, sigma=0.05, lower_limit=0.0, upper_limit=1.0)
 
+    # Overall Lens Model:
+
     model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
 Model Customization
 -------------------
 
 We can customize the lens model parameters in a number of different ways, as shown below:
 
 .. code-block:: python
 
+    # Lens:
+
     bulge = af.Model(al.lp.Sersic)
     disk = af.Model(al.lp.Exponential)
 
     # Parameter Pairing: Pair the centre of the bulge and disk together, reducing
     # the complexity of non-linear parameter space by N = 2
 
     bulge.centre = disk.centre
@@ -256,29 +284,43 @@
         redshift=0.5,
         bulge=bulge,
         disk=disk,
         mass=mass,
         shear=shear,
     )
 
+    # Source:
+
     bulge = af.Model(al.lp.Sersic)
     disk = af.Model(al.lp.Exponential)
 
     source = af.Model(al.Galaxy, redshift=1.0, bulge=bulge, disk=disk)
 
+    # Overall Lens Model:
+
     model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
     # Assert that the effective radius of the bulge is larger than that of the disk.
     # (Assertions can only be added at the end of model composition, after all components
     # have been bright together in a `Collection`.
     model.add_assertion(model.galaxies.bulge.effective_radius > model.galaxies.disk.effective_radius)
 
     # Assert that the Einstein Radius is below 3.0":
     model.add_assertion(model.galaxies.mass.einstein_radius < 3.0)
 
+Available Model Components
+--------------------------
+
+The light profiles, mass profiles and other components that can be used for lens modeling are given at the following
+API documentation pages:
+
+ - https://pyautolens.readthedocs.io/en/latest/api/light.html
+ - https://pyautolens.readthedocs.io/en/latest/api/mass.html
+ - https://pyautolens.readthedocs.io/en/latest/api/pixelization.html
+
 JSon Outputs
 ------------
 
 After a model is composed, it can easily be output to a .json file on hard-disk in a readable structure:
 
 .. code-block:: python
```

### Comparing `autolens-2023.3.27.1/docs/general/papers.rst` & `autolens-2023.7.7.2/docs/general/papers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 
 `Modelling high-resolution ALMA observations of strongly lensed dusty star forming galaxies detected by Herschel <https://arxiv.org/abs/2111.09680>`_
 
 `ALMA resolves the first strongly-lensed Optical/NIR-dark galaxy <https://arxiv.org/abs/2207.00466>`_
 
 `The Two 𝑧 ∼ 13 Galaxy Candidates HD1 and HD2 Are Likely Not Lensed <https://arxiv.org/abs/2209.06830>`_
 
+`The Way of Water: ALMA resolves H2O emission lines in a strongly lensed dusty star-forming galaxy at z ∼ 3.1 <https://arxiv.org/abs/2304.08563>`_
+
 **Surveys**
 
 `When Spectral Modeling Meets Convolutional Networks: A Method for Discovering Reionization-era Lensed Quasars in Multi-band Imaging Data <https://arxiv.org/abs/2211.14543>`_
 
 `Modeling Strong Lenses from Wide-Field Ground-Based Observations in KiDS and GAMA <https://arxiv.org/abs/2301.05320>`_
 
 `MNELLS: The MUSE Nearby Early-Type Galaxy Lens Locator Survey <https://arxiv.org/abs/2002.07191>`_
```

### Comparing `autolens-2023.3.27.1/docs/general/workspace.rst` & `autolens-2023.7.7.2/docs/general/workspace.rst`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 Descriptions of every configuration file and their input parameters are provided in the ``README.rst`` in
 the `config directory of the workspace <https://github.com/Jammy2211/autolens_workspace/tree/release/config>`_
 
 Config
 ------
 
-Here, you'll find the configuration files used by **PyAutoLens** which customize:
+Here, you'll find the configuration files which customize:
 
     - The default settings used by every non-linear search.
     - Visualization, including the backend used by *matplotlib*.
     - The priors and notation configs associated with the light and mass profiles used for lens modeling.
     - The behaviour of different (y,x) Cartesian grids used to perform lens calculations.
     - The general.yaml config which customizes other aspects of **PyAutoLens**.
 
@@ -51,15 +51,15 @@
 
 Contains the dataset's used to perform lens modeling. Example datasets using simulators included with the workspace
 are included here by default.
 
 Output
 ------
 
-The folder where lens modeling results are stored.
+The folder where  modeling results are stored.
 
 SLaM
 ----
 
 Advanced lens modeling pipelines that use the Source, Light and Mass (SLaM) approach to lens modeling.
 
 See `here <https://pyautolens.readthedocs.io/en/latest/advanced/slam.html>`_ for an overview.
```

### Comparing `autolens-2023.3.27.1/docs/howtolens/chapter_1_introduction.rst` & `autolens-2023.7.7.2/docs/howtolens/chapter_1_introduction.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/howtolens/chapter_2_lens_modeling.rst` & `autolens-2023.7.7.2/docs/howtolens/chapter_2_lens_modeling.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/howtolens/chapter_3_search_chaining.rst` & `autolens-2023.7.7.2/docs/howtolens/chapter_3_search_chaining.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/howtolens/chapter_4_pixelizations.rst` & `autolens-2023.7.7.2/docs/howtolens/chapter_4_pixelizations.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Chapter 4: Inversions
-=====================
+Chapter 4: Pixelizations
+========================
 
 In chapter 4, we use **Pixelizations** to reconstruct complex source galaxies on pixelized grids.
 
 The chapter contains the following tutorials:
 
 `Tutorial 1: Pixelizations <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_1_pixelizations.ipynb>`_
 - Creating a pixel-grid in the source-plane.
@@ -23,8 +23,17 @@
 `Tutorial 6: Lens Modeling  <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_6_lens_modeling.ipynb>`_
 - How to use inversions to fit a lens model.
 
 `Tutorial 7: Adaptive Pixelization <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_7_adaptive_pixelization.ipynb>`_
 - A Voronoi mesh which adapts to the mass model's magnification.
 
 `Tutorial 8: Model Fit <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_8_model_fit.ipynb>`_
-- An example lens modeling pipeline which uses an inversion.
+- An example lens modeling pipeline which uses an inversion.
+
+`Tutorial 9: Fit Problems <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_9_fit_problems.ipynb>`_
+- The shortcomings of our lens models and inversions.
+
+`Tutorial 10: Brightness Adaption <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_10_brightness_adaption.ipynb>`_
+- Adapting the pixelization to the source's morphology.
+
+`Tutorial 11: Adaptive Regularization <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=notebooks/howtolens/chapter_4_pixelizations/tutorial_11_adaptive_regularization.py.ipynb>`_
+- Adapting the regularization to the source's morphology.
```

### Comparing `autolens-2023.3.27.1/docs/howtolens/chapter_optional.rst` & `autolens-2023.7.7.2/docs/howtolens/chapter_optional.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/howtolens/howtolens.rst` & `autolens-2023.7.7.2/docs/howtolens/howtolens.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 The lectures are provided as Jupyter notebooks (and Python scripts), and they are linked to via this readthedocs. The
 lectures are composed of five chapters
 
 - **Introduction** - An introduction to strong gravitational lensing and **PyAutolens**.
 - **Lens Modeling** - How to model strong lenses, including a primer on Bayesian non-linear analysis.
 - **Search Chaining** - How to fit complex lens models using non-linear search chaining.
 - **Pixelizations** - How to perform pixelized reconstructions of the source-galaxy.
-- **Hyper-Mode** - How to use **PyAutoLens** advanced modeling features that adapt the model to the strong lens being analysed.
 
 How to Tackle HowToLens
 -----------------------
 
 The HowToLens lecture series currently sits at 5 chapters, and each will take around 3-6 hours to go through thoroughly. 
-You probably want to be modeling lenses with **PyAutoLens** faster than that! Furthermore, the concepts in the
-later chapters are pretty challenging, and familiarity with **PyAutoLens** and lens modeling is desirable before you
+You probably want to be modeling lensestick_maker.min_value faster than that! Furthermore, the concepts in the
+later chapters are pretty challenging, and familiaritytick_maker.min_value and lens modeling is desirable before you
 tackle them.
 
 Therefore, we recommend that you complete chapters 1 & 2 and then apply what you've learnt to the modeling of simulated
 and real strong lenses imaging, using the scripts found in the 'autolens_workspace' `modeling` packages. Once you're
 confident with your use of **PyAutoLens**, you can then begin to cover the advanced functionality covered in chapters
 3, 4 & 5.
```

### Comparing `autolens-2023.3.27.1/docs/index.rst` & `autolens-2023.7.7.2/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+.. image:: https://github.com/Jammy2211/PyAutoLogo/blob/main/gifs/pyautolens.gif?raw=true
+  :width: 900
+
+
 What is PyAutoLens?
 ===================
 
 **PyAutoLens** is open source software for the analysis and modeling of strong gravitational lenses, with its target
 audience anyone with an interest in astronomy and cosmology.
 
 The software comes distributed with the **HowToLens** Jupyter notebook lectures, which are written assuming no
-previous knowledge about what gravitational lensing is and teach a new user the theory and statistics required to analyse
+previous knowledge about what gravitational lensing is and teach a new user theory and statistics required to analyse
 strong lens data. Checkout `the howtolens section of
 the readthedocs <https://pyautolens.readthedocs.io/en/latest/howtolens/howtolens.html>`_.
 
-
 An overview of **PyAutoLens**'s core features can be found in
 the `overview section of the readthedocs <https://pyautolens.readthedocs.io/en/latest/overview/lensing.html>`_.
 
 Strong Gravitational Lensing
 ============================
 
 When two galaxies are aligned down the line-of-sight to Earth, light rays from the background galaxy are deflected by the
@@ -51,63 +54,63 @@
 objects are extensible, making it straightforward to compose highly customized lensing system. The example code
 below shows this in action:
 
 .. code-block:: python
 
     import autolens as al
     import autolens.plot as aplt
+    from astropy import cosmology as cosmo
 
     """
     To describe the deflection of light by mass, two-dimensional grids of (y,x) Cartesian
     coordinates are used.
     """
-
-    grid_2d = al.Grid2D.uniform(
+    grid = al.Grid2D.uniform(
         shape_native=(50, 50),
         pixel_scales=0.05,  # <- Conversion from pixel units to arc-seconds.
     )
 
     """
     The lens galaxy has an elliptical isothermal mass profile and is at redshift 0.5.
     """
-
-    sie = al.mp.Isothermal(
-        centre=(0.0, 0.0), ell_comps=(0.1, 0.05), einstein_radius=1.6
+    mass = al.mp.Isothermal(
+        centre=(0.0, 0.0),
+        ell_comps=(0.1, 0.05),
+        einstein_radius=1.6
     )
 
-    lens_galaxy = al.Galaxy(redshift=0.5, mass=sie)
+    lens_galaxy = al.Galaxy(redshift=0.5, mass=mass)
 
     """
     The source galaxy has an elliptical exponential light profile and is at redshift 1.0.
     """
-
-    exponential = al.lp.Exponential(
+    disk = al.lp.Exponential(
         centre=(0.3, 0.2),
         ell_comps=(0.05, 0.25),
         intensity=0.05,
         effective_radius=0.5,
     )
 
-    source_galaxy = al.Galaxy(redshift=1.0, light=exponential)
+    source_galaxy = al.Galaxy(redshift=1.0, disk=disk)
 
     """
     We create the strong lens using a Tracer, which uses the galaxies, their redshifts
     and an input cosmology to determine how light is deflected on its path to Earth.
     """
-
     tracer = al.Tracer.from_galaxies(
-        galaxies=[lens_galaxy, source_galaxy], cosmology=al.cosmo.Planck15()
+        galaxies=[lens_galaxy, source_galaxy],
+        cosmology = al.cosmo.Planck15()
     )
 
     """
     We can use the Grid2D and Tracer to perform many lensing calculations, for example
     plotting the image of the lensed source.
     """
-
-    aplt.Tracer.image(tracer=tracer, grid=grid_2d)
+    tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid)
+    tracer_plotter.figures_2d(image=True)
 
 To perform lens modeling, **PyAutoLens** adopts the probabilistic programming
 language `PyAutoFit <https://github.com/rhayes777/PyAutoFit>`_. **PyAutoFit** allows users to compose a
 lens model from ``LightProfile``, ``MassProfile`` and ``Galaxy`` objects, customize the model parameterization and
 fit it to data via a non-linear search (e.g. `dynesty <https://github.com/joshspeagle/dynesty>`_,
 `emcee <https://github.com/dfm/emcee>`_ or `PySwarms <https://pyswarms.readthedocs.io/en/latest/>`_). The example
 code below shows how to setup and fit a lens model to a dataset:
@@ -118,54 +121,61 @@
     import autofit as af
     import autolens as al
     import autolens.plot as aplt
 
     """
     Load Imaging data of the strong lens from the dataset folder of the workspace.
     """
-    imaging = al.Imaging.from_fits(
-        image_path="/path/to/dataset/image.fits",
+    dataset = al.Imaging.from_fits(
+        data_path="/path/to/dataset/image.fits",
         noise_map_path="/path/to/dataset/noise_map.fits",
         psf_path="/path/to/dataset/psf.fits",
         pixel_scales=0.1,
     )
 
     """
-    Create a mask for the data, which we setup as a 3.0" circle.
+    Create a mask for the imaging data, which we setup as a 3.0" circle, and apply it.
     """
     mask = al.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.0
+        shape_native=dataset.shape_native,
+        pixel_scales=dataset.pixel_scales,
+        radius=3.0
     )
-    imaging = imaging.apply_mask(mask=mask_2d)
+    dataset = dataset.apply_mask(mask=mask)
 
     """
     We model the lens galaxy using an elliptical isothermal mass profile and
     the source galaxy using an elliptical sersic light profile.
-    """
-    lens_mass_profile = al.mp.Isothermal
-    source_light_profile = al.lp.Sersic
 
-    """
     To setup these profiles as model components whose parameters are free & fitted for
-    we set up each Galaxy as a Model and define the model as a Collection of all galaxies.
+    we set up each Galaxy as a `Model` and define the model as a `Collection` of all galaxies.
     """
-    lens_galaxy_model = af.Model(al.Galaxy, redshift=0.5, mass=lens_mass_profile)
-    source_galaxy_model = af.Model(al.Galaxy, redshift=1.0, disk=source_light_profile)
-    model = af.Collection(lens=lens_galaxy_model, source=source_galaxy_model)
+    # Lens:
+
+    mass = af.Model(al.mp.Isothermal)
+    lens = af.Model(al.Galaxy, redshift=0.5, mass=lens_mass_profile)
+
+    # Source:
+
+    disk = af.Model(al.lp.Sersic)
+    source = af.Model(al.Galaxy, redshift=1.0, disk=disk)
+
+    # Overall Lens Model:
+    model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
     """
     We define the non-linear search used to fit the model to the data (in this case, Dynesty).
     """
-    search = af.DynestyStatic(name="search[example]", n_live_points=50)
+    search = af.DynestyStatic(name="search[example]", nlive=50)
 
     """
     We next set up the `Analysis`, which contains the `log likelihood function` that the
     non-linear search calls to fit the lens model to the data.
     """
-    analysis = al.AnalysisImaging(dataset=imaging)
+    analysis = al.AnalysisImaging(dataset=dataset)
 
     """
     To perform the model-fit we pass the model and analysis to the search's fit method. This will
     output results (e.g., dynesty samples, model parameters, visualization) to hard-disk.
     """
     result = search.fit(model=model, analysis=analysis)
 
@@ -184,15 +194,15 @@
 datasets.
 
 For new **PyAutoLens** users, we recommend they start by
 `installing PyAutoLens <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ (if you haven't
 already!), read through the ``introduction.ipynb`` notebook on
 the `autolens_workspace <https://github.com/Jammy2211/autolens_workspace>`_ and take the
 `HowToLens Jupyter notebook lecture series <https://pyautolens.readthedocs.io/en/latest/howtolens/howtolens.html>`_ on
-strong gravitational lensing with **PyAutoLens**.
+strong gravitational lensingtick_maker.min_value.
 
 .. toctree::
    :caption: Overview:
    :maxdepth: 1
    :hidden:
 
    overview/overview_1_lensing
@@ -237,15 +247,14 @@
    :hidden:
 
    howtolens/howtolens
    howtolens/chapter_1_introduction
    howtolens/chapter_2_lens_modeling
    howtolens/chapter_3_search_chaining
    howtolens/chapter_4_pixelizations
-   howtolens/chapter_5_hyper_mode
    howtolens/chapter_optional
 
 .. toctree::
    :caption: API Reference:
    :maxdepth: 1
    :hidden:
 
@@ -265,8 +274,7 @@
    :maxdepth: 1
    :hidden:
 
    advanced/database
    advanced/chaining
    advanced/slam
    advanced/graphical
-   advanced/hyper_mode
```

### Comparing `autolens-2023.3.27.1/docs/installation/conda.rst` & `autolens-2023.7.7.2/docs/installation/conda.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/installation/numba.rst` & `autolens-2023.7.7.2/docs/installation/numba.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Certain functionality (pixelized source reconstructions, linear light profiles) is disabled without numba installed
 because it will have too slow run-times.
 
 However, some users have experienced difficulties installing numba, meaning they have been unable to try out
 PyAutoLens and determine if it the right software for them, before committing more time to installing numba
 successfully.
 
-For this reason, numba is an optional installation, so that users can easily experiment with **PyAutoLens** and learn
+For this reason, numba is an optional installation, so that users can easily experimenttick_maker.min_value and learn
 the basic API.
 
 If you do not have numba installed, you can do so via pip as follows:
 
 .. code-block:: bash
 
     pip install numba
```

### Comparing `autolens-2023.3.27.1/docs/installation/overview.rst` & `autolens-2023.7.7.2/docs/installation/overview.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ========
 
 **PyAutoLens** requires Python 3.8+ and support the Linux, MacOS and Windows operating systems.
 
 **PyAutoLens** can be installed via the Python distribution `Anaconda <https://www.anaconda.com/>`_ or using
 `Pypi <https://pypi.org/>`_ to ``pip install`` **PyAutoLens** into your Python distribution.
 
-We recommend Anaconda as it manages the installation of many major libraries used by **PyAutoLens** (e.g. numpy, scipy,
+We recommend Anaconda as it manages the installation of many major libraries (e.g. numpy, scipy,
 matplotlib, etc.) making installation more straight forward. Windows users must use Anaconda.
 
 The installation guide for both approaches can be found at:
 
 - `Anaconda installation guide <https://pyautolens.readthedocs.io/en/latest/installation/conda.html>`_
 
 - `PyPI installation guide <https://pyautolens.readthedocs.io/en/latest/installation/pip.html>`_
```

### Comparing `autolens-2023.3.27.1/docs/installation/pip.rst` & `autolens-2023.7.7.2/docs/installation/pip.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/installation/source.rst` & `autolens-2023.7.7.2/docs/installation/source.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 **PyAutoFit** https://github.com/rhayes777/PyAutoFit
 
 **PyAutoArray** https://github.com/Jammy2211/PyAutoArray
 
 **PyAutoGalaxy** https://github.com/Jammy2211/PyAutoGalaxy
 
-If you wish to build from source all code used by **PyAutoLens** you may need to build from source these 3 additional
+If you wish to build from source all code you may need to build from source these 3 additional
 projects. We include below instructions for building just **PyAutoLens** from source or building all projects.
 
 Building Only PyAutoLens
 ------------------------
 
 We upgrade pip to ensure certain libraries install:
```

### Comparing `autolens-2023.3.27.1/docs/installation/troubleshooting.rst` & `autolens-2023.7.7.2/docs/installation/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/clusters/cluster.png` & `autolens-2023.7.7.2/docs/overview/images/clusters/cluster.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/bad_chi_squared_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/bad_chi_squared_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/bad_normalized_residual_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/bad_normalized_residual_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/bad_residual_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/bad_residual_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/chi_squared_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/chi_squared_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/image.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/masked_image.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/masked_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/model_image.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/model_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/noise_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/noise_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/normalized_residual_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/normalized_residual_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/psf.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/psf.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/residual_map.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/residual_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/subplot_fit.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/subplot_fit.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/fitting/tracer_image.png` & `autolens-2023.7.7.2/docs/overview/images/fitting/tracer_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/groups/image.png` & `autolens-2023.7.7.2/docs/overview/images/groups/image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/chi_squared_map_imag.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/chi_squared_map_imag.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/chi_squared_map_real.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/chi_squared_map_real.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/dirty_image.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/dirty_signal_to_noise.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/dirty_signal_to_noise.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/fit_dirty_images.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/fit_dirty_images.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/image_pre_ft.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/image_pre_ft.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/model_visibilities.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/model_visibilities.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/residual_map_imag.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/residual_map_imag.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/residual_map_real.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/residual_map_real.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/uv_wavelengths.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/uv_wavelengths.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/interferometry/visibilities.png` & `autolens-2023.7.7.2/docs/overview/images/interferometry/visibilities.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/complex_source.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/complex_source.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/grid.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/grid.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_convergence.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_convergence.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_deflections_x.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_deflections_x.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_deflections_y.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_deflections_y.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/isothermal_mass_profile_potential.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_potential.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/schematic.jpg` & `autolens-2023.7.7.2/docs/overview/images/lensing/schematic.jpg`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/sersic_light_profile.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/sersic_light_profile.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/lensing/tracer_image.png` & `autolens-2023.7.7.2/docs/overview/images/lensing/tracer_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/modeling/cornerplot.png` & `autolens-2023.7.7.2/docs/overview/images/modeling/cornerplot.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/multiwavelength/dirty_image.png` & `autolens-2023.7.7.2/docs/overview/images/multiwavelength/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/multiwavelength/g_image.png` & `autolens-2023.7.7.2/docs/overview/images/multiwavelength/g_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/multiwavelength/r_image.png` & `autolens-2023.7.7.2/docs/overview/images/multiwavelength/r_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/pixelizations/image.png` & `autolens-2023.7.7.2/docs/overview/images/pixelizations/image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/pixelizations/reconstructed_image.png` & `autolens-2023.7.7.2/docs/overview/images/pixelizations/reconstructed_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/pixelizations/rectangular.png` & `autolens-2023.7.7.2/docs/overview/images/pixelizations/rectangular.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/pixelizations/voronoi.png` & `autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/pixelizations/voronoi_fit.png` & `autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi_fit.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/pixelizations/voronoi_fit_plane_1.png` & `autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi_fit_plane_1.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/point_sources/image.png` & `autolens-2023.7.7.2/docs/overview/images/point_sources/image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/ao_image.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/ao_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/euclid_image.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/euclid_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/hst_image.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/hst_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/image.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/noise_map.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/noise_map.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/psf.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/psf.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/images/simulating/vro_image.png` & `autolens-2023.7.7.2/docs/overview/images/simulating/vro_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/docs/overview/overview_10_clusters.rst` & `autolens-2023.7.7.2/docs/overview/overview_10_clusters.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 To model a cluster, we assume that every source galaxy is a ``PointSrcChi`` model, which means the goodness-of-fit is
 evaluated in the source-plane. This removes the need to iteratively solve the lens equation. However, we still define
 a ``PointSolver``, incase we wish to perform image-plane fits.
 
 .. code-block:: python
 
-    point_solver = al.PointSolver(grid=grid_2d, pixel_scale_precision=0.025)
+    point_solver = al.PointSolver(grid=grid, pixel_scale_precision=0.025)
 
 Lens Model
 ----------
 
 A cluster scale strong lens model is typically composed of the following:
 
  - One or more brightest cluster galaxies (BCG), which are sufficiently large that we model them individually.
@@ -75,15 +75,15 @@
 SExtractor Catalogues
 ---------------------
 
 Composing the lens model for cluster scale objects requires care, given there are could be hundreds of lenses and
 sources galaxies. Manually writing the model in a Python script, in the way we do for galaxy-scale lenses, is therefore
 not feasible.
 
-For this cluster, we therefore composed the the model by interfacing with Source Extractor
+For this cluster, we therefore composed the model by interfacing with Source Extractor
 (https://sextract.readthedocs.io/) catalogue files. A full illustration of how to make the lens and source models
 from catalogue files is given at the following links:
 
  `lenses <https://github.com/Jammy2211/autolens_workspace/blob/main/scripts/cluster/model_maker/example__lenses.py>`_
  `sources <https://github.com/Jammy2211/autolens_workspace/blob/main/scripts/cluster/model_maker/example__sources.py>`_
 
 These files can be easily altered to compose a cluster model suited to your lens
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_1_lensing.rst` & `autolens-2023.7.7.2/docs/overview/overview_1_lensing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 are two-dimensional Cartesian grids of (y,x) coordinates.
 
 Below, we create and plot a uniform Cartesian ``Grid2D`` (the ``pixel_scales`` describes the conversion from pixel
 units to arc-seconds):
 
 .. code-block:: python
 
-    grid_2d = al.Grid2D.uniform(
+    grid = al.Grid2D.uniform(
         shape_native=(50, 50), pixel_scales=0.05
     )
-    grid_2d_plotter = aplt.Grid2DPlotter(grid=grid_2d)
-    grid_2d_plotter.figure_2d()
+    grid_plotter = aplt.Grid2DPlotter(grid=grid)
+    grid_plotter.figure_2d()
 
 This is what our ``Grid2D`` looks like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/lensing/grid.png
   :width: 400
   :alt: Alternative text
 
@@ -67,22 +67,22 @@
     )
 
 By passing this ``Profile`` a ``Grid2D``, we can evaluate the light at every coordinate on that ``Grid2D``, creating an
 image of the ``LightProfile``:
 
 .. code-block:: python
 
-    image_2d = sersic_light_profile.image_2d_from(grid=grid_2d)
+    image = sersic_light_profile.image_2d_from(grid=grid)
 
 The **PyAutoLens** plot module provides methods for plotting objects and their properties, like the ``LightProfile``'s image.
 
 .. code-block:: python
 
     light_profile_plotter = aplt.LightProfilePlotter(
-        light_profile=sersic_light_profile, grid=grid_2d
+        light_profile=sersic_light_profile, grid=grid
     )
     light_profile_plotter.figures_2d(image=True)
 
 The light profile's image appears as shown below:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/lensing/sersic_light_profile.png
   :width: 400
@@ -101,20 +101,20 @@
 
     isothermal_mass_profile = al.mp.Isothermal(
         centre=(0.0, 0.0),
         ell_comps=(0.1, 0.1),
         einstein_radius=1.6,
     )
 
-    convergence = isothermal_mass_profile.convergence_2d_from(grid=grid_2d)
-    potential = isothermal_mass_profile.potential_2d_from(grid=grid_2d)
-    deflections = isothermal_mass_profile.deflections_yx_2d_from(grid=grid_2d)
+    convergence = isothermal_mass_profile.convergence_2d_from(grid=grid)
+    potential = isothermal_mass_profile.potential_2d_from(grid=grid)
+    deflections = isothermal_mass_profile.deflections_yx_2d_from(grid=grid)
 
     mass_profile_plotter = aplt.MassProfilePlotter(
-        mass_profile=isothermal_mass_profile, grid=grid_2d
+        mass_profile=isothermal_mass_profile, grid=grid
     )
     mass_profile_plotter.figures_2d(
         convergence=True, potential=True, deflections_y=True, deflections_x=True
     )
 
 Here is how the convergence, potential and deflection angles appear:
 
@@ -171,17 +171,17 @@
 
 When calculating this image, the ``Tracer`` performs all ray-tracing for the strong lens system. This includes using
 the lens galaxy's total mass distribution to deflect the light-rays that are traced to the source galaxy. As a result,
 the source appears as a multiply imaged and strongly lensed Einstein ring.
 
 .. code-block:: python
 
-    image_2d = tracer.image_2d_from(grid=grid_2d)
+    image = tracer.image_2d_from(grid=grid)
 
-    tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid_2d)
+    tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid)
     tracer_plotter.figures_2d(image=True)
 
 This makes the image below, where the source's light appears as a multiply imaged and strongly lensed Einstein ring.
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/lensing/tracer_image.png
   :width: 400
   :alt: Alternative text
@@ -240,15 +240,15 @@
             effective_radius=0.1,
             sersic_index=1.5,
         ),
     )
 
     tracer = al.Tracer.from_galaxies(galaxies=[lens_galaxy_0, lens_galaxy_1, source_galaxy])
 
-    tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid_2d)
+    tracer_plotter = aplt.TracerPlotter(tracer=tracer, grid=grid)
     tracer_plotter.figures_2d(image=True)
 
 This is what the lens looks like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/lensing/complex_source.png
   :width: 400
   :alt: Alternative text
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_2_fitting.rst` & `autolens-2023.7.7.2/docs/overview/overview_2_fitting.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 We are now going to use a ``Tracer`` to fit imaging data of a strong lens, which we begin by loading
 from .fits files as an ``Imaging`` object:
 
 .. code-block:: python
 
     dataset_path = "/path/to/dataset/folder"
 
-    imaging = al.Imaging.from_fits(
-        image_path=path.join(dataset_path, "image.fits"),
+    dataset = al.Imaging.from_fits(
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
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/fitting/image.png
   :width: 400
   :alt: Alternative text
 
@@ -45,21 +45,21 @@
 
 We now need to mask the data, so that regions where there is no signal (e.g. the edges) are omitted from the fit. To do
 this we can use a ``Mask2D`` object, which for this example we'll create as a 3.0" circle.
 
 .. code-block:: python
 
     mask = al.Mask2D.circular(
-        shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, sub_size=1, radius=3.0
+        shape_native=dataset.shape_native, pixel_scales=dataset.pixel_scales, sub_size=1, radius=3.0
     )
 
-    imaging = imaging.apply_mask(mask=mask_2d)
+    dataset = dataset.apply_mask(mask=mask_2d)
 
-    imaging_plotter = aplt.ImagingPlotter(imaging=imaging)
-    imaging_plotter.figures_2d(image=True)
+    dataset_plotter = aplt.ImagingPlotter(dataset=dataset)
+    dataset_plotter.figures_2d(image=True)
 
 Here is what our image looks like with the mask applied, where **PyAutoLens** has automatically zoomed around the
 ``Mask2D`` to make the lensed source appear bigger:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/fitting/masked_image.png
   :width: 400
   :alt: Alternative text
@@ -72,18 +72,18 @@
 
 By passing a ``Tracer`` and ``Imaging`` object to a ``FitImaging`` object, we create a model-image from the ``Tracer``.
 The model-image is the image of the ``Tracer`` blurred with the ``Imaging`` dataset's PSF, ensuring our fit to the data
 provides a like-with-like comparison.
 
 .. code-block:: python
 
-    fit = al.FitImaging(dataset=masked_imaging, tracer=tracer)
+    fit = al.FitImaging(dataset=masked_dataset, tracer=tracer)
 
-    fit_imaging_plotter = aplt.FitImagingPlotter(fit=fit)
-    fit_imaging_plotter.figures_2d(model_image=True)
+    fit_plotter = aplt.FitImagingPlotter(fit=fit)
+    fit_plotter.figures_2d(model_image=True)
 
 Here is how the ``Tracer``'s image and the ``FitImaging``'s model-image look, note how the model-image has been blurred
 with the PSF of our dataset:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/fitting/tracer_image.png
   :width: 400
   :alt: Alternative text
@@ -94,17 +94,17 @@
 
 The ``FitImaging`` object does a lot more than just create the model-image, it also subtracts this image from
 the data to produce a residual-map and combines this with the noise-map to compute a chi-squared-map, both of which
 we can plot:
 
 .. code-block:: python
 
-    fit_imaging_plotter = aplt.FitImagingPlotter(fit=fit)
+    fit_plotter = aplt.FitImagingPlotter(fit=fit)
 
-    fit_imaging_plotter.figures_2d(
+    fit_plotter.figures_2d(
         residual_map=True,
         chi_squared_map=True
     )
 
 For a good lens model where the ``Tracer``'s model image is representative of the strong lens system the residuals and
 chi-squared values minimized:
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_3_modeling.rst` & `autolens-2023.7.7.2/docs/overview/overview_3_modeling.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   :alt: Alternative text
 
 The task of finding these ``LightProfiles``'s and ``MassProfiles``'s is called *lens modeling*.
 
 PyAutoFit
 ---------
 
-Lens modeling with **PyAutoLens** uses the probabilistic programming language
+Lens modelingtick_maker.min_value uses the probabilistic programming language
 `PyAutoFit <https://github.com/rhayes777/PyAutoFit>`_, an open-source Python framework that allows complex model
 fitting techniques to be straightforwardly integrated into scientific modeling software. Check it out if you
 are interested in developing your own software to perform advanced model-fitting!
 
 We import it separately to **PyAutoLens**
 
 .. code-block:: python
@@ -34,43 +34,55 @@
 
 We compose the lens model that we fit to the data using a ``Model`` object, which behaves analogously to the ``Galaxy``,
 ``LightProfile`` and ``MassProfile`` used previously, however their parameters are not specified and are instead
 determined by a fitting procedure.
 
 .. code-block:: python
 
-    lens_galaxy_model = af.Model(
+    # Lens:
+
+    bulge = af.Model(al.lp.DevVaucouleurs)
+    mass = af.Model(al.mp.Isothermal)
+
+    lens = af.Model(
         al.Galaxy,
         redshift=0.5,
-        bulge=al.lp.DevVaucouleurs,
-        mass=al.mp.Isothermal
+        bulge=bulge,
+        mass=mass
     )
-    source_galaxy_model = af.Model(al.Galaxy, redshift=1.0, disk=al.lp.Exponential)
+
+    # Source:
+
+    disk = af.Model(al.lp.Exponential)
+
+    source = af.Model(al.Galaxy, redshift=1.0, disk=disk)
 
 We combine the lens and source model galaxies above into a ``Collection``, which is the model we will fit. Note how
 we could easily extend this object to compose highly complex models containing many galaxies.
 
 The reason we create separate ``Collection``'s for the ``galaxies`` and ``model`` is because the `model`
 can be extended to include other components than just galaxies.
 
 
 In this example, we therefore fit our strong lens data with two galaxies:
 
-    - A lens galaxy with a elliptisl Dev Vaucouleurs ``LightProfile`` representing a bulge and
+    - A lens galaxy with a elliptical Dev Vaucouleurs ``LightProfile`` representing a bulge and
       elliptical isothermal ``MassProfile`` representing its mass.
     - A source galaxy with an elliptical exponential ``LightProfile`` representing a disk.
 
 The redshifts of the lens (z=0.5) and source(z=1.0) are fixed.
 
 Printing the ``info`` attribute of the model shows us this is the model we are fitting, and shows us the free parameters and
 their priors:
 
 .. code-block:: python
 
-    galaxies = af.Collection(lens=lens_galaxy_model, source=source_galaxy_model)
+    # Overall Lens Model:
+
+    galaxies = af.Collection(lens=lens, source=source)
     model = af.Collection(galaxies=galaxies)
 
 .. code-block:: python
 
     print(model.info)
 
 This gives the following output:
@@ -131,15 +143,15 @@
 --------
 
 We next create an ``AnalysisImaging`` object, which contains the ``log likelihood function`` that the non-linear
 search calls to fit the lens model to the data.
 
 .. code-block:: python
 
-    analysis = al.AnalysisImaging(dataset=imaging)
+    analysis = al.AnalysisImaging(dataset=dataset)
 
 Model-Fit
 ---------
 
 To perform the model-fit we pass the model and analysis to the search's fit method. This will output results (e.g.,
 dynesty samples, model parameters, visualization) to hard-disk.
 
@@ -315,16 +327,16 @@
 parameter samples, log likelihood values and tools to compute the errors on the lens model.
 
 **PyAutoLens** includes many visualization tools for plotting the results of a non-linear search, for example we can
 make a corner plot of the probability density function (PDF):
 
 .. code-block:: python
 
-    dynesty_plotter = aplt.DynestyPlotter(samples=result.samples)
-    dynesty_plotter.cornerplot()
+    search_plotter = aplt.DynestyPlotter(samples=result.samples)
+    search_plotter.cornerplot()
 
 Here is an example of how a PDF estimated for a lens model appears:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/modeling/cornerplot.png
   :width: 600
   :alt: Alternative text
 
@@ -332,16 +344,16 @@
 plotted.
 
 .. code-block:: python
 
     tracer_plotter = aplt.TracerPlotter(tracer=result.max_log_likelihood_tracer, grid=mask.derive_grid.masked)
     tracer_plotter.subplot_tracer()
 
-    fit_imaging_plotter = aplt.FitImagingPlotter(fit=result.max_log_likelihood_fit)
-    fit_imaging_plotter.subplot_fit_imaging()
+    fit_plotter = aplt.FitImagingPlotter(fit=result.max_log_likelihood_fit)
+    fit_plotter.subplot_fit()
 
 Here's what the model-fit of the model which maximizes the log likelihood looks like, providing good residuals and
 low chi-squared values:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/fitting/subplot_fit.png
   :width: 600
   :alt: Alternative text
@@ -353,37 +365,44 @@
 -------------------
 
 The ``Model`` can be fully customized, making it simple to parameterize and fit many different lens models
 using any combination of ``LightProfile``'s and ``MassProfile``'s:
 
 .. code-block:: python
 
-    lens_galaxy_model = af.Model(
-        al.Galaxy,
-        redshift=0.5,
-        bulge=al.lp.DevVaucouleurs,
-        mass=al.mp.Isothermal
-    )
+    # Lens:
+
+    bulge = af.Model(al.lp.DevVaucouleurs)
+    mass = af.Model(al.mp.Isothermal)
 
     """
     This aligns the light and mass profile centres in the model, reducing the
     number of free parameter fitted for by Dynesty by 2.
     """
-    lens_galaxy_model.bulge.centre = lens_galaxy_model.mass.centre
+    bulge.centre = mass.centre
 
     """
     This fixes the lens galaxy light profile's effective radius to a value of
     0.8 arc-seconds, removing another free parameter.
     """
-    lens_galaxy_model.bulge.effective_radius = 0.8
+    bulge.effective_radius = 0.8
 
     """
     This forces the mass profile's einstein radius to be above 1.0 arc-seconds.
     """
-    lens_galaxy_model.mass.add_assertion(lens_galaxy_model.mass.einstein_radius > 1.0)
+    mass.add_assertion(lens.mass.einstein_radius > 1.0)
+
+    lens = af.Model(
+        al.Galaxy,
+        redshift=0.5,
+        bulge=bulge,
+        mass=mass
+    )
+
+
 
 The above fit used the non-linear search ``dynesty``, but **PyAutoLens** supports many other methods and their
 setting can be easily customized:
 
 Linear Light Profiles
 ---------------------
 
@@ -398,56 +417,87 @@
 parameters (e.g. ``effective_radius``, ``sersic_index``).
 
 For complex models, linear light profiles are a powerful way to simplify the parameter space to ensure the best-fit
 model is inferred.
 
 .. code-block:: python
 
-    sersic_linear = al.lp_linear.Sersic()
+    # Lens:
+
+    bulge = af.Model(al.lp_linear.DevVaucouleurs)
+    disk = af.Model(al.lp_linear.Sersic)
     
-    lens_model_linear = af.Model(
+    lens = af.Model(
         al.Galaxy,
         redshift=0.5,
-        bulge=ag.lp_linear.DevVaucouleurs,
-        disk=ag.lp_linear.Sersic,
+        bulge=bulge,
+        disk=disk
     )
-    
-    source_model_linear = af.Model(al.Galaxy, redshift=1.0, disk=al.lp_linear.Exponential)
 
-Basis Functions
----------------
+    # Source:
+
+    disk = af.Model(al.lp_linear.Exponential)
+
+    source = af.Model(al.Galaxy, redshift=1.0, disk=disk)
+
+Multi Gaussian Expansion
+------------------------
 
 A natural extension of linear light profiles are basis functions, which group many linear light profiles together in
 order to capture complex and irregular structures in a galaxy's emission.
 
 Using a clever model parameterization a basis can be composed which corresponds to just N = 5-10 parameters, making
 model-fitting efficient and robust.
 
-Below, we compose a basis of 10 Gaussians which all share the same `centre` and `ell_comps`. Their `sigma`
-values are set via the relation `y = a + (log10(i+1) + b)`, where `i` is the  Gaussian index and `a` and `b` are free
-parameters. This basis is could be used to represent the lens galaxy's light.
+Below, we compose a basis of 30 Gaussians which all share the same `centre` and `ell_comps`. Their `sigma`
+values are set in growing log10 bins in steps from 0.01 to 3.0 arc-seconds, which is the radius of the mask.
 
-Because `a` and `b` are free parameters (as opposed to `sigma` which can assume many values), we are able to
-compose and fit `Basis` objects which can capture very complex light distributions with just N = 5-10 non-linear
-parameters!
+The `Basis` objects below can capture very complex light distributions with just N = 4 non-linear parameters!
 
 .. code-block:: python
 
-    bulge_a = af.UniformPrior(lower_limit=0.0, upper_limit=0.2)
-    bulge_b = af.UniformPrior(lower_limit=0.0, upper_limit=10.0)
+    total_gaussians = 30
+
+    # The sigma values of the Gaussians will be fixed to values spanning 0.01 to the mask radius, 3.0".
+    log10_sigma_list = np.linspace(-2, np.log10(3.0), total_gaussians)
+
+    # By defining the centre here, it creates two free parameters that are assigned below to all Gaussians.
+
+    centre_0 = af.UniformPrior(lower_limit=-0.1, upper_limit=0.1)
+    centre_1 = af.UniformPrior(lower_limit=-0.1, upper_limit=0.1)
+
+    # A list of Gaussian model components whose parameters are customized belows.
+
+    gaussian_list = af.Collection(
+        af.Model(al.lp_linear.Gaussian) for _ in range(total_gaussians)
+    )
+
+    # Iterate over every Gaussian and customize its parameters.
+
+    for i, gaussian in enumerate(gaussian_list):
 
-    gaussians_lens = af.Collection(af.Model(al.lp_linear.Gaussian) for _ in range(10))
+        # All Gaussians have same y and x centre.
 
-    for i, gaussian in enumerate(gaussians_lens):
+        gaussian.centre.centre_0 = centre_0
+        gaussian.centre.centre_1 = centre_1
 
-        gaussian.centre = gaussians_lens[0].centre
-        gaussian.ell_comps = gaussians_lens[0].ell_comps
-        gaussian.sigma = bulge_a + (bulge_b * np.log10(i+1))
+        # All Gaussians have same elliptical components.
 
-    bulge = af.Model(al.lp_basis.Basis, light_profile_list=gaussians_lens)
+        gaussian.ell_comps = gaussian_list[0].ell_comps
+
+        # All Gaussian sigmas are fixed to values above.
+
+        gaussian.sigma = 10 ** log10_sigma_list[i]
+
+    # The Basis object groups many light profiles together into a single model component.
+
+    bulge = af.Model(
+        al.lp_basis.Basis,
+        light_profile_list=gaussian_list,
+    )
 
 The bulge's ``info`` attribute describes the basis model composition:
 
 .. code-block:: python
 
     print(bulge.info)
 
@@ -497,20 +547,26 @@
                     bulge_b                                                         UniformPrior, lower_limit = 0.0, upper_limit = 10.0
                     other                                                           0.3010299956639812
         2
         ...
         trimmed for conciseness
         ...
 
+Shapelets
+---------
+
 **PyAutoLens** also supports Shapelet basis functions, which are appropriate for capturing exponential / disk-like
 features in a galaxy, and therefore may make a good model for most lensed source galaxies.
 
 This is illustrated in full on the ``autogalaxy_workspace`` in the example
 script autolens_workspace/scripts/imaging/modeling/advanced/shapelets.py .
 
+Regularization
+--------------
+
 **PyAutoLens** can also apply Bayesian regularization to Basis functions, which smooths the linear light profiles
 (e.g. the Gaussians) in order to prevent over-fitting noise.
 
 .. code-block:: python
 
     bulge = af.Model(
         al.lp_basis.Basis, light_profile_list=gaussians_lens, regularization=al.reg.Constant
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_4_simulate.rst` & `autolens-2023.7.7.2/docs/overview/overview_4_simulate.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 Simulating strong lens images uses a *SimulatorImaging* object, which models the process that an instrument like the
 Hubble Space Telescope goes through observe a strong lens. This includes accounting for the exposure time to
 determine the signal-to-noise of the data, blurring the observed light of the strong lens with the telescope optics
 and accounting for the background sky in the exposure which adds Poisson noise:
 
 .. code-block:: python
 
-    psf_2d = ag.Kernel2D.from_gaussian(
-        shape_native=(11, 11), sigma=0.1, pixel_scales=grid_2d.pixel_scales
+    psf = ag.Kernel2D.from_gaussian(
+        shape_native=(11, 11), sigma=0.1, pixel_scales=grid.pixel_scales
     )
 
     simulator = al.SimulatorImaging(
         exposure_time=300.0,
         background_sky_level=1.0,
-        psf=psf_2d,
+        psf=psf,
         add_poisson_noise=True,
     )
 
 Once we have a simulator, we can use it to create an imaging dataset which consists of an image, noise-map and
 Point Spread Function (PSF) by passing it a tracer and grid:
 
 .. code-block:: python
 
-    imaging = simulator.from_tracer_and_grid(tracer=tracer, grid=grid_2d)
+    dataset = simulator.from_tracer_and_grid(tracer=tracer, grid=grid)
 
 Here is what our dataset looks like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/simulating/image.png
   :width: 400
   :alt: Alternative text
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_5_pixelizations.rst` & `autolens-2023.7.7.2/docs/overview/overview_5_pixelizations.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 -------------------
 
 To fit this image with an ``Inversion``, we first mask the ``Imaging`` object:
 
 .. code-block:: python
 
    mask = al.Mask2D.circular(
-      shape_native=imaging.shape_native, pixel_scales=imaging.pixel_scales, radius=3.6
+      shape_native=dataset.shape_native, pixel_scales=dataset.pixel_scales, radius=3.6
     )
 
-   imaging = imaging.apply_mask(mask=mask_2d)
+   dataset = dataset.apply_mask(mask=mask_2d)
 
 To reconstruct the source on a pixel-grid, called a mesh, we simply pass it the ``Mesh`` class we want to reconstruct its
 light on.
 
 We also pass a ``Regularization`` scheme which applies a smoothness prior on the source reconstruction.
 
 Below, we use a ``Rectangular`` mesh with resolution 40 x 40 and a ``Constant`` regularization scheme:
@@ -49,15 +49,15 @@
 ``FitImaging`` object will automatically use the source galaxy's ``Pixelization`` and ``Regularization`` to reconstruct
 the lensed source's light using the ``Inversion``:
 
 .. code-block:: python
 
     tracer = al.Tracer.from_galaxies(galaxies=[lens_galaxy, source_galaxy])
 
-    fit = al.FitImaging(dataset=imaging, tracer=tracer)
+    fit = al.FitImaging(dataset=dataset, tracer=tracer)
 
 Here is what our reconstructed source galaxy looks like:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/pixelizations/rectangular.png
   :width: 400
   :alt: Alternative text
 
@@ -89,15 +89,15 @@
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/pixelizations/voronoi_fit.png
   :width: 600
   :alt: Alternative text
 
 Wrap-Up
 -------
 
-This was a brief overview of ``Inverion``'s with **PyAutoLens**.
+This was a brief overview of ``Inverion``'stick_maker.min_value.
 
 There is a lot more to using ``Inverion``'s then presented here, which is covered in chapters 4 and 5 of
 the **HowToLens**, specifically:
 
     - How the source reconstruction calculates the flux-values of the source pixels when it performs the reconsturction.
     - What exactly regularization is and why it is necessary.
     - The Bayesian framework employed to choose an appropriate level of smoothing and avoid overfitting noise.
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_6_interferometry.rst` & `autolens-2023.7.7.2/docs/overview/overview_6_interferometry.rst`

 * *Files 6% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 We next load an ``Interferometer`` dataset from fits files, which follows the same API that we have seen
 for an ``Imaging`` object.
 
 .. code-block:: python
 
     dataset_path = "/path/to/dataset/folder"
 
-    interferometer = al.Interferometer.from_fits(
-        visibilities_path=path.join(dataset_path, "visibilities.fits"),
+    dataset = al.Interferometer.from_fits(
+        data_path=path.join(dataset_path, "data.fits"),
         noise_map_path=path.join(dataset_path, "noise_map.fits"),
         uv_wavelengths_path=path.join(dataset_path, "uv_wavelengths.fits"),
         real_space_mask=real_space_mask_2d
     )
 
-    interferometer_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
-    interferometer_plotter.figures_2d(visibilities=True, uv_wavelengths=True)
+    dataset_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
+    dataset_plotter.figures_2d(visibilities=True, uv_wavelengths=True)
 
 Here is what the interferometer visibilities and uv wavelength (which represent the interferometer's baselines):
 
-.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/visibilities.png
+.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/data.png
   :width: 400
   :alt: Alternative text
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/uv_wavelengths.png
   :width: 400
   :alt: Alternative text
 
@@ -57,16 +57,16 @@
 
 We discuss below how **PyAutoLens** can scale up to large visibilities datasets from an instrument like ALMA.
 
 This can also plot the dataset in real-space, using the fast Fourier transforms described below.
 
 .. code-block:: python
 
-    interferometer_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
-    interferometer_plotter.figures_2d(dirty_image=True, dirty_signal_to_noise_map=True)
+    dataset_plotter = aplt.InterferometerPlotter(interferometer=interferometer)
+    dataset_plotter.figures_2d(dirty_image=True, dirty_signal_to_noise_map=True)
 
 Here is what the image and signal-to-noise map look like in real space:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/dirty_image.png
   :width: 400
   :alt: Alternative text
 
@@ -99,42 +99,42 @@
     transformer_class = al.TransformerNUFFT
 
 To perform a fit, we follow the same process we did for imaging. We do not need to mask an interferometer dataset,
 but we will apply the settings above:
 
 .. code-block:: python
 
-    interferometer = interferometer.apply_settings(
+    dataset = dataset.apply_settings(
         settings=al.SettingsInterferometer(transformer_class=transformer_class)
     )
 
 Fitting
 -------
 
 The interferometer can now be passed to a ``FitInterferometer`` object to fit it to a data-set:
 
 .. code-block:: python
 
     fit = al.FitInterferometer(
         interferometer=interferometer, tracer=tracer
     )
 
-    fit_interferometer_plotter = aplt.FitInterferometerPlotter(fit=fit)
-    fit_interferometer_plotter.subplot_fit_interferometer()
-    fit_interferometer_plotter.subplot_fit_real_space()
+    fit_plotter = aplt.FitInterferometerPlotter(fit=fit)
+    fit_plotter.subplot_fit()
+    fit_plotter.subplot_fit_real_space()
 
 Here is what the image of the tracer looks like before it is Fourier transformed to the uv-plane:
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/image_pre_ft.png
   :width: 400
   :alt: Alternative text
 
 And here is what the Fourier transformed model visibilities look like:
 
-.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/model_visibilities.png
+.. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/model_data.png
   :width: 400
   :alt: Alternative text
 
 Here is what the fit of the galaxy looks like in real space (which is computed via a FFT from the uv-plane):
 
 .. image:: https://raw.githubusercontent.com/Jammy2211/PyAutoLens/main/docs/overview/images/interferometry/fit_dirty_images.png
   :width: 400
@@ -170,46 +170,51 @@
 
 Whereas we previously used an ``AnalysisImaging`` object, we instead use an ``AnalysisInterferometer`` object which fits
 the lens model in the correct way for an interferometer dataset. This includes mapping the lens model from real-space
 to the uv-plane via the Fourier transform discussed above:
 
 .. code-block:: python
 
-    lens_galaxy_model = af.Model(al.Galaxy, redshift=0.5, mass=al.mp.Isothermal)
-    source_galaxy_model = af.Model(al.Galaxy, redshift=1.0, disk=al.lp.Exponential)
+    # Lens:
 
-    model = af.Collection(lens=lens_galaxy_model, source=source_galaxy_model)
+    mass = af.Model(al.mp.Isothermal)
 
-    search = af.DynestyStatic(name="overview_interferometer")
+    lens = af.Model(al.Galaxy, redshift=0.5, mass=mass)
 
-    analysis = al.AnalysisInterferometer(dataset=interferometer)
+    # Source:
 
-    result = search.fit(model=model, analysis=analysis)
+    disk = af.Model(al.lp.Exponential)
+
+    source = af.Model(al.Galaxy, redshift=1.0, disk=disk)
+
+    # Overall Lens Model:
+
+    model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
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
 
     simulator = al.SimulatorInterferometer(
         uv_wavelengths=uv_wavelengths,
         exposure_time=300.0,
         background_sky_level=1.0,
         noise_sigma=0.01,
     )
 
-    interferometer = simulator.via_tracer_from(tracer=tracer, grid=real_space_grid)
+    dataset = simulator.via_tracer_from(tracer=tracer, grid=real_space_grid)
 
 Wrap-Up
 -------
 
 The `interferometer <https://github.com/Jammy2211/autolens_workspace/tree/release/notebooks/interferometer>`_ package
 of the `autolens_workspace <https://github.com/Jammy2211/autolens_workspace>`_ contains numerous example scripts for performing
 interferometer modeling and simulating strong lens interferometer datasets.
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_7_multi_wavelength.rst` & `autolens-2023.7.7.2/docs/overview/overview_7_multi_wavelength.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 Multi-wavelength imaging datasets do not use any new objects or class in **PyAutoLens**.
 
 We simply use lists of the classes we are now familiar with, for example the ``Imaging`` class.
 
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
@@ -71,27 +71,27 @@
 For multi-wavelength lens modeling, we use the same mask for every dataset whenever possible. This is not absolutely
 necessary, but provides a more reliable analysis.
 
 .. code-block:: python
 
     mask_2d_list = [
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
 
 We now introduce the key new aspect to the **PyAutoLens** multi-dataset API, which is critical to fitting multiple
 datasets simultaneously.
 
 We sum the list of analysis objects to create an overall ``CombinedAnalysis`` object, which we can use to fit the
 multi-wavelength imaging data, where:
 
@@ -114,22 +114,35 @@
 Model
 -----
 
 We compose an initial lens model as per usual.
 
 .. code-block:: python
 
+    # Lens:
+
+    bulge = af.Model(al.lp.Sersic)
+    mass = af.Model(al.mp.Isothermal)
+    shear = af.Model(al.mp.ExternalShear)
+
     lens = af.Model(
         al.Galaxy,
         redshift=0.5,
-        bulge=al.lp.Sersic,
-        mass=al.mp.Isothermal,
-        shear=al.mp.ExternalShear,
+        bulge=bulge,
+        mass=mass,
+        shear=shear,
     )
-    source = af.Model(al.Galaxy, redshift=1.0, bulge=al.lp.Sersic)
+
+    # Source:
+
+    bulge = af.Model(al.lp.Sersic)
+
+    source = af.Model(al.Galaxy, redshift=1.0, bulge=bulge)
+
+    # Overall Lens Model:
 
     model = af.Collection(galaxies=af.Collection(lens=lens, source=source))
 
 However, there is a problem for multi-wavelength datasets. Should the light profiles of the lens's bulge and
 source's bulge have the same parameters for each wavelength image?
 
 The answer is no. At different wavelengths, different stars appear brighter or fainter, meaning that the overall
@@ -214,21 +227,21 @@
     lens_c = af.UniformPrior(lower_limit=-10.0, upper_limit=10.0)
 
     source_m = af.UniformPrior(lower_limit=-0.1, upper_limit=0.1)
     source_c = af.UniformPrior(lower_limit=-10.0, upper_limit=10.0)
 
     analysis_list = []
 
-    for wavelength, imaging in zip(wavelength_list, imaging_list):
+    for wavelength, imaging in zip(wavelength_list, dataset_list):
 
         lens_intensity = (wavelength * lens_m) + lens_c
         source_intensity = (wavelength * source_m) + source_c
 
         analysis_list.append(
-            al.AnalysisImaging(dataset=imaging).with_model(
+            al.AnalysisImaging(dataset=dataset).with_model(
                 model.replacing(
                     {
                         model.galaxies.lens.bulge.intensity: lens_intensity,
                         model.galaxies.source.bulge.intensity: source_intensity,
                     }
                 )
             )
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_8_point_sources.rst` & `autolens-2023.7.7.2/docs/overview/overview_8_point_sources.rst`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 There are many options that can be passed to a ``PositionsSovler``, below we only specify the precision we want the
 image-plane coordinates to be calculated too, which is 0.001", much lower than the resolution fo the data we observed
 the point-sources on!
 
 .. code-block:: python
 
     solver = al.PointSolver(
-        grid=grid_2d,
+        grid=grid,
         pixel_scale_precision=0.001,
     )
 
     positions = solver.solve(lensing_obj=tracer, source_plane_coordinate=(0.07, 0.07))
 
 Here is what the solved positions look like, compared to the observe data. In this example, the data was simulated
 with the mass-model we used above, so the match is good:
@@ -138,29 +138,45 @@
     print(fit["point_0"].positions.residual_map)
     print(fit["point_0"].positions.chi_squared_map)
     print(fit["point_0"].positions.log_likelihood)
 
 Lens Modeling
 -------------
 
-It is straight forward to fit a lens model to a point source dataset, using the same API that we saw for imaging and
+It is straight forward to fit a lens model to a point source dataset, using the same API that we saw for dataset and
 interferometer datasets.
 
 This uses an ``AnalysisPoint`` object which fits the lens model in the correct way for a point source dataset.
 This includes mapping the ``name``'s of each dataset in the ``PointDict`` to the names of the point sources in
 the lens model.
 
 .. code-block:: python
 
-    lens_galaxy_model = af.Model(al.Galaxy, redshift=0.5, mass=al.mp.Isothermal)
-    source_galaxy_model = af.Model(al.Galaxy, redshift=1.0, point_0=al.ps.Point)
+    # Lens:
 
-    galaxies = af.Collection(lens=lens_galaxy_model, source=source_galaxy_model)
+    bulge = af.Model(al.lp.Sersic)
+    mass = af.Model(al.mp.Isothermal)
+
+    lens = af.Model(
+        al.Galaxy, redshift=0.5, bulge=bulge, mass=mass
+    )
+
+    # Source:
+
+    point_0 = af.Model(al.ps.Point)
+
+    source = af.Model(al.Galaxy, redshift=1.0, point_0=point_0)
+
+    # Overall Lens Model:
+
+    galaxies = af.Collection(lens=lens, source=source)
     model = af.Collection(galaxies=galaxies)
 
+    # Search + Analysis + Model-Fit
+
     search = af.DynestyStatic(name="overview_point_source")
 
     analysis = al.AnalysisPoint(point_dict=point_dict, solver=solver)
 
     result = search.fit(model=model, analysis=analysis)
 
 Wrap-Up
```

### Comparing `autolens-2023.3.27.1/docs/overview/overview_9_groups.rst` & `autolens-2023.7.7.2/docs/overview/overview_9_groups.rst`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 .. code-block:: python
 
     point_dict = al.PointDict.from_json(
         file_path=path.join(dataset_path, "point_dict.json")
     )
 
-    point_solver = al.PointSolver(grid=grid_2d, pixel_scale_precision=0.025)
+    point_solver = al.PointSolver(grid=grid, pixel_scale_precision=0.025)
 
 Model via JSON
 --------------
 
 We now compose the lens model. For groups there could be many hundreds of galaxies in the model. Whereas previous
 examples explicitly wrote the model out via Python code, for group modeling we opt to write the model in .json files,
 which is loaded as follows:
```

### Comparing `autolens-2023.3.27.1/files/citations.bib` & `autolens-2023.7.7.2/files/citations.bib`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     author={Minas Karamanis and Florian Beutler},
     year={2020},
     eprint={2002.06212},
     archivePrefix={arXiv},
     primaryClass={stat.ML}
 }
 @article{Nightingale2015,
-abstract = {We present a new pixelized method for the inversion of gravitationally lensed extended source images which we term adaptive semi-linear inversion (SLI). At the heart of the method is an h-means clustering algorithm which is used to derive a source plane pixelization that adapts to the lens model magnification. The distinguishing feature of adaptive SLI is that every pixelization is derived from a random initialization, ensuring that data discretization is performed in a completely different and unique way for every lens model parameter set. We compare standard SLI on a fixed source pixel grid with the new method and demonstrate the shortcomings of the former when modelling singular power-law ellipsoid (SPLE) lens profiles. In particular, we demonstrate the superior reliability and efficiency of adaptive SLI which, by design, fixes the number of degrees of freedom (NDOF) of the optimization and thereby removes biases present with other methods that allow the NDOF to vary. In addition, we highlight the importance of data discretization in pixel-based inversion methods, showing that adaptive SLI averages over significant systematics that are present when a fixed source pixel grid is used. In the case of the SPLE lens profile, we show how the method successfully samples its highly degenerate posterior probability distribution function with a single nonlinear search. The robustness of adaptive SLI provides a firm foundation for the development of a strong lens modelling pipeline, which will become necessary in the short-term future to cope with the increasing rate of discovery of new strong lens systems.},
+abstract = {We present a new pixelized method for the inversion of gravitationally lensed extended source images which we term adaptive semi-linear inversion (SLI). At the heart of the method is an h-means clustering algorithm which is used to derive a source plane pixelization that adapts to the lens model magnification. The distinguishing feature of adaptive SLI is that every pixelization is derived from a random initialization, ensuring that data discretization is performed in a completely different and unique way for every model parameter set. We compare standard SLI on a fixed source pixel grid with the new method and demonstrate the shortcomings of the former when modelling singular power-law ellipsoid (SPLE) lens profiles. In particular, we demonstrate the superior reliability and efficiency of adaptive SLI which, by design, fixes the number of degrees of freedom (NDOF) of the optimization and thereby removes biases present with other methods that allow the NDOF to vary. In addition, we highlight the importance of data discretization in pixel-based inversion methods, showing that adaptive SLI averages over significant systematics that are present when a fixed source pixel grid is used. In the case of the SPLE lens profile, we show how the method successfully samples its highly degenerate posterior probability distribution function with a single nonlinear search. The robustness of adaptive SLI provides a firm foundation for the development of a strong lens modelling pipeline, which will become necessary in the short-term future to cope with the increasing rate of discovery of new strong lens systems.},
 archivePrefix = {arXiv},
 arxivId = {1412.7436},
 author = {Nightingale, J. W. and Dye, S.},
 doi = {10.1093/mnras/stv1455},
 eprint = {1412.7436},
 issn = {13652966},
 journal = {MNRAS},
```

### Comparing `autolens-2023.3.27.1/files/citations.md` & `autolens-2023.7.7.2/files/citations.md`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/files/citations.tex` & `autolens-2023.7.7.2/files/citations.tex`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/files/image.png` & `autolens-2023.7.7.2/files/image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/files/imageaxis.png` & `autolens-2023.7.7.2/files/imageaxis.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/files/imagenoaxis.png` & `autolens-2023.7.7.2/files/imagenoaxis.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/files/model_image.png` & `autolens-2023.7.7.2/files/model_image.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/files/reconstruction.png` & `autolens-2023.7.7.2/files/reconstruction.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/paper/imageaxis.png` & `autolens-2023.7.7.2/paper/imageaxis.png`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/paper/paper.bib` & `autolens-2023.7.7.2/paper/paper.bib`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
 pages = {1999--2012},
 title = {{Herschel *-ATLAS: Deep HST/WFC3 imaging of strongly lensed submillimetre galaxies}},
 url = {http://arxiv.org/abs/1311.5898},
 volume = {440},
 year = {2014}
 }
 @article{Nightingale2015,
-abstract = {We present a new pixelized method for the inversion of gravitationally lensed extended source images which we term adaptive semi-linear inversion (SLI). At the heart of the method is an h-means clustering algorithm which is used to derive a source plane pixelization that adapts to the lens model magnification. The distinguishing feature of adaptive SLI is that every pixelization is derived from a random initialization, ensuring that data discretization is performed in a completely different and unique way for every lens model parameter set. We compare standard SLI on a fixed source pixel grid with the new method and demonstrate the shortcomings of the former when modelling singular power-law ellipsoid (SPLE) lens profiles. In particular, we demonstrate the superior reliability and efficiency of adaptive SLI which, by design, fixes the number of degrees of freedom (NDOF) of the optimization and thereby removes biases present with other methods that allow the NDOF to vary. In addition, we highlight the importance of data discretization in pixel-based inversion methods, showing that adaptive SLI averages over significant systematics that are present when a fixed source pixel grid is used. In the case of the SPLE lens profile, we show how the method successfully samples its highly degenerate posterior probability distribution function with a single nonlinear search. The robustness of adaptive SLI provides a firm foundation for the development of a strong lens modelling pipeline, which will become necessary in the short-term future to cope with the increasing rate of discovery of new strong lens systems.},
+abstract = {We present a new pixelized method for the inversion of gravitationally lensed extended source images which we term adaptive semi-linear inversion (SLI). At the heart of the method is an h-means clustering algorithm which is used to derive a source plane pixelization that adapts to the lens model magnification. The distinguishing feature of adaptive SLI is that every pixelization is derived from a random initialization, ensuring that data discretization is performed in a completely different and unique way for every model parameter set. We compare standard SLI on a fixed source pixel grid with the new method and demonstrate the shortcomings of the former when modelling singular power-law ellipsoid (SPLE) lens profiles. In particular, we demonstrate the superior reliability and efficiency of adaptive SLI which, by design, fixes the number of degrees of freedom (NDOF) of the optimization and thereby removes biases present with other methods that allow the NDOF to vary. In addition, we highlight the importance of data discretization in pixel-based inversion methods, showing that adaptive SLI averages over significant systematics that are present when a fixed source pixel grid is used. In the case of the SPLE lens profile, we show how the method successfully samples its highly degenerate posterior probability distribution function with a single nonlinear search. The robustness of adaptive SLI provides a firm foundation for the development of a strong lens modelling pipeline, which will become necessary in the short-term future to cope with the increasing rate of discovery of new strong lens systems.},
 archivePrefix = {arXiv},
 arxivId = {1412.7436},
 author = {Nightingale, J. W. and Dye, S.},
 doi = {10.1093/mnras/stv1455},
 eprint = {1412.7436},
 issn = {13652966},
 journal = {MNRAS},
```

### Comparing `autolens-2023.3.27.1/paper/paper.json` & `autolens-2023.7.7.2/paper/paper.json`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/paper/paper.md` & `autolens-2023.7.7.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/release.sh` & `autolens-2023.7.7.2/release.sh`

 * *Files identical despite different names*

### Comparing `autolens-2023.3.27.1/setup.py` & `autolens-2023.7.7.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.3.27.1")
+version = environ.get("VERSION", "2023.7.7.2")
 requirements.extend(
     [
         f"autoarray=={version}",
         f"autoconf=={version}",
         f"autofit=={version}",
         f"autogalaxy=={version}",
     ]
 )
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
-    for (path, directories, filenames) in os.walk(directory):
+    for path, directories, filenames in os.walk(directory):
         for directory in directories:
             paths.append(f"{path}/{directory}".replace("/", "."))
     return paths
 
 
 setup(
     name="autolens",
```

### Comparing `autolens-2023.3.27.1/to_do_list` & `autolens-2023.7.7.2/to_do_list`

 * *Files identical despite different names*

