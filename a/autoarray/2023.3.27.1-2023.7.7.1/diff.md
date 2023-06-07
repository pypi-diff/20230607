# Comparing `tmp/autoarray-2023.3.27.1.tar.gz` & `tmp/autoarray-2023.7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoarray-2023.3.27.1.tar", last modified: Mon Mar 27 14:48:07 2023, max compression
+gzip compressed data, was "autoarray-2023.7.7.1.tar", last modified: Wed Jun  7 09:44:45 2023, max compression
```

## Comparing `autoarray-2023.3.27.1.tar` & `autoarray-2023.7.7.1.tar`

### file list

```diff
@@ -1,423 +1,425 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.290477 autoarray-2023.3.27.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.245547 autoarray-2023.3.27.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.297787 autoarray-2023.3.27.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3065 2022-12-19 16:37:07.000000 autoarray-2023.3.27.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-02 11:50:15.000000 autoarray-2023.3.27.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1007 2023-03-27 14:48:07.289467 autoarray-2023.3.27.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2022-05-03 18:33:14.000000 autoarray-2023.3.27.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.309787 autoarray-2023.3.27.1/autoarray/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4722 2023-03-27 14:42:00.000000 autoarray-2023.3.27.1/autoarray/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1660 2022-12-19 16:33:57.000000 autoarray-2023.3.27.1/autoarray/abstract_ndarray.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.318826 autoarray-2023.3.27.1/autoarray/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/autoarray/config/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      635 2022-12-02 11:50:15.000000 autoarray-2023.3.27.1/autoarray/config/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      699 2023-03-24 11:58:38.000000 autoarray-2023.3.27.1/autoarray/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       57 2022-11-29 17:43:26.000000 autoarray-2023.3.27.1/autoarray/config/grids.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      416 2021-06-17 13:08:16.000000 autoarray-2023.3.27.1/autoarray/config/logging.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.334824 autoarray-2023.3.27.1/autoarray/config/visualize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-02 11:50:15.000000 autoarray-2023.3.27.1/autoarray/config/visualize/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      749 2023-03-24 12:02:35.000000 autoarray-2023.3.27.1/autoarray/config/visualize/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1412 2022-12-21 13:17:54.000000 autoarray-2023.3.27.1/autoarray/config/visualize/include.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3272 2023-02-12 10:45:24.000000 autoarray-2023.3.27.1/autoarray/config/visualize/mat_wrap.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1209 2022-12-02 11:50:15.000000 autoarray-2023.3.27.1/autoarray/config/visualize/mat_wrap_1d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3987 2023-01-15 20:42:59.000000 autoarray-2023.3.27.1/autoarray/config/visualize/mat_wrap_2d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2412 2022-12-02 18:02:42.000000 autoarray-2023.3.27.1/autoarray/config/visualize/plots.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.339707 autoarray-2023.3.27.1/autoarray/dataset/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/autoarray/dataset/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.347746 autoarray-2023.3.27.1/autoarray/dataset/abstract/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/abstract/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6037 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/dataset/abstract/dataset.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4675 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/abstract/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1752 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/abstract/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.359863 autoarray-2023.3.27.1/autoarray/dataset/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/dataset/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12746 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/dataset/imaging/imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3269 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/imaging/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4574 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/dataset/imaging/simulator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2023-02-06 13:53:42.000000 autoarray-2023.3.27.1/autoarray/dataset/imaging/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.372255 autoarray-2023.3.27.1/autoarray/dataset/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8166 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/dataset/interferometer/interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2471 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/interferometer/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3708 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/interferometer/simulator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2043 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/dataset/interferometer/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.376287 autoarray-2023.3.27.1/autoarray/dataset/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/dataset/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      194 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/dataset/mock/mock_dataset.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.381305 autoarray-2023.3.27.1/autoarray/dataset/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/dataset/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10557 2023-01-26 17:02:36.000000 autoarray-2023.3.27.1/autoarray/dataset/plot/imaging_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13311 2023-01-26 17:02:35.000000 autoarray-2023.3.27.1/autoarray/dataset/plot/interferometer_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20442 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/dataset/preprocess.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3138 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/exc.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.391326 autoarray-2023.3.27.1/autoarray/fit/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/autoarray/fit/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12284 2023-02-20 16:46:54.000000 autoarray-2023.3.27.1/autoarray/fit/fit_dataset.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2592 2022-12-13 16:21:24.000000 autoarray-2023.3.27.1/autoarray/fit/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6255 2022-12-13 16:21:23.000000 autoarray-2023.3.27.1/autoarray/fit/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18328 2022-12-20 20:45:06.000000 autoarray-2023.3.27.1/autoarray/fit/fit_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.396344 autoarray-2023.3.27.1/autoarray/fit/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/fit/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1306 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/fit/mock/mock_fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      896 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/fit/mock/mock_fit_interferometer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.406356 autoarray-2023.3.27.1/autoarray/fit/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/fit/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11170 2023-01-26 17:02:35.000000 autoarray-2023.3.27.1/autoarray/fit/plot/fit_imaging_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22678 2023-01-26 17:02:36.000000 autoarray-2023.3.27.1/autoarray/fit/plot/fit_interferometer_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10539 2023-01-26 17:02:35.000000 autoarray-2023.3.27.1/autoarray/fit/plot/fit_vector_yx_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13678 2023-03-13 19:36:52.000000 autoarray-2023.3.27.1/autoarray/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.416388 autoarray-2023.3.27.1/autoarray/geometry/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/autoarray/geometry/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1065 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/geometry/abstract_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2768 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/geometry/geometry_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12385 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/geometry/geometry_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1687 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/geometry/geometry_2d_irregular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26638 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/geometry/geometry_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.418389 autoarray-2023.3.27.1/autoarray/inversion/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-19 14:59:34.000000 autoarray-2023.3.27.1/autoarray/inversion/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.434661 autoarray-2023.3.27.1/autoarray/inversion/inversion/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:42.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35085 2023-03-24 12:05:37.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15515 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/factory.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.445660 autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10134 2023-03-13 21:49:37.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28017 2023-03-13 20:55:52.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10622 2023-03-13 19:00:36.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/mapping.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23943 2023-03-18 17:02:31.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.459749 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6130 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5655 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5333 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/lop.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8272 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/mapping.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9538 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/w_tilde.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21125 2023-03-24 12:05:37.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/inversion_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42651 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/inversion_util_secret.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38767 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/inversion_util_secret_clean.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3410 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/inversion/settings.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.469746 autoarray-2023.3.27.1/autoarray/inversion/linear_obj/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/linear_obj/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4924 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/inversion/linear_obj/func_list.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7269 2023-03-20 16:41:33.000000 autoarray-2023.3.27.1/autoarray/inversion/linear_obj/linear_obj.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2022-12-21 17:08:33.000000 autoarray-2023.3.27.1/autoarray/inversion/linear_obj/neighbors.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1701 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/linear_obj/unique_mappings.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.492033 autoarray-2023.3.27.1/autoarray/inversion/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6765 2023-02-12 10:43:58.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_inversion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4231 2023-02-12 10:43:58.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_inversion_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1134 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_inversion_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      890 2023-02-06 13:53:42.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_linear_obj.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      611 2023-02-06 13:53:42.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_linear_obj_func_list.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2272 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_mapper.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1681 2022-12-21 13:25:52.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_mesh.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1027 2022-12-21 13:25:52.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_pixelization.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      512 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/mock/mock_regularization.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.500228 autoarray-2023.3.27.1/autoarray/inversion/pixelization/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.519550 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20017 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10119 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/delaunay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3243 2022-12-21 13:16:25.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/factory.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3665 2022-12-21 15:37:32.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/mapper_grids.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27399 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/mapper_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6780 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/rectangular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12734 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/voronoi.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.539197 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5490 2022-12-21 13:25:52.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13091 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/delaunay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24451 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/mesh_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7143 2022-12-21 17:08:33.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/rectangular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4715 2022-12-21 17:08:33.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/triangulation.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13162 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/voronoi.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5281 2022-12-22 08:54:23.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/voronoi_nn.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7683 2022-12-21 15:48:54.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/pixelization.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1451 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/pixelization/settings.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.545208 autoarray-2023.3.27.1/autoarray/inversion/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/inversion/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11617 2023-01-26 17:02:34.000000 autoarray-2023.3.27.1/autoarray/inversion/plot/inversion_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6193 2023-02-08 10:34:55.000000 autoarray-2023.3.27.1/autoarray/inversion/plot/mapper_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.567607 autoarray-2023.3.27.1/autoarray/inversion/regularization/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      455 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8960 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4728 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/adaptive_brightness.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4508 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/adaptive_brightness_split.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5208 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3391 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/brightness_zeroth.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2964 2023-02-06 13:53:42.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/constant.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3226 2022-12-19 16:33:57.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/constant_split.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2189 2023-02-06 13:53:42.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/constant_zeroth.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15379 2023-03-22 15:47:12.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/regularization_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3030 2023-02-06 13:53:42.000000 autoarray-2023.3.27.1/autoarray/inversion/regularization/zeroth.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.575656 autoarray-2023.3.27.1/autoarray/layout/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-06-17 13:08:16.000000 autoarray-2023.3.27.1/autoarray/layout/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11376 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/layout/layout.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7323 2022-12-19 16:33:57.000000 autoarray-2023.3.27.1/autoarray/layout/layout_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14070 2023-02-12 10:43:58.000000 autoarray-2023.3.27.1/autoarray/layout/region.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.586117 autoarray-2023.3.27.1/autoarray/mask/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/autoarray/mask/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5226 2022-12-19 16:20:31.000000 autoarray-2023.3.27.1/autoarray/mask/abstract_mask.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.597364 autoarray-2023.3.27.1/autoarray/mask/derive/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/mask/derive/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3485 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/mask/derive/grid_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16580 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/mask/derive/grid_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21875 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/mask/derive/indexes_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5317 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/mask/derive/mask_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21304 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/mask/derive/mask_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6016 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/mask/mask_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3661 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/mask/mask_1d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35878 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/mask/mask_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48977 2023-03-21 18:17:34.000000 autoarray-2023.3.27.1/autoarray/mask/mask_2d_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.601364 autoarray-2023.3.27.1/autoarray/mask/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/mask/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/mask/mock/mock_mask.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1556 2023-02-12 10:43:58.000000 autoarray-2023.3.27.1/autoarray/mock.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4786 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/numba_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.608368 autoarray-2023.3.27.1/autoarray/operators/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/autoarray/operators/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22076 2023-03-13 21:20:30.000000 autoarray-2023.3.27.1/autoarray/operators/convolver.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.612367 autoarray-2023.3.27.1/autoarray/operators/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/operators/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      244 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/operators/mock/mock_convolver.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11057 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/operators/transformer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7743 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/operators/transformer_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.619529 autoarray-2023.3.27.1/autoarray/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3668 2023-02-12 10:45:24.000000 autoarray-2023.3.27.1/autoarray/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7181 2022-12-13 16:21:22.000000 autoarray-2023.3.27.1/autoarray/plot/abstract_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      280 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/auto_labels.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.626759 autoarray-2023.3.27.1/autoarray/plot/get_visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/get_visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2662 2022-12-21 17:08:33.000000 autoarray-2023.3.27.1/autoarray/plot/get_visuals/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2394 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/get_visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9159 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/plot/get_visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.633758 autoarray-2023.3.27.1/autoarray/plot/include/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/include/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1718 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/include/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1263 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/include/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4182 2022-12-21 13:25:52.000000 autoarray-2023.3.27.1/autoarray/plot/include/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.643761 autoarray-2023.3.27.1/autoarray/plot/mat_plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/mat_plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9906 2023-02-12 16:45:35.000000 autoarray-2023.3.27.1/autoarray/plot/mat_plot/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9618 2023-02-12 10:45:24.000000 autoarray-2023.3.27.1/autoarray/plot/mat_plot/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26172 2023-02-12 16:45:29.000000 autoarray-2023.3.27.1/autoarray/plot/mat_plot/two_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2106 2022-11-10 18:26:59.000000 autoarray-2023.3.27.1/autoarray/plot/multi_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.652071 autoarray-2023.3.27.1/autoarray/plot/visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2690 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/plot/visuals/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1270 2022-11-11 15:49:33.000000 autoarray-2023.3.27.1/autoarray/plot/visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3402 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/plot/visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.657055 autoarray-2023.3.27.1/autoarray/plot/wrap/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2250 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.699259 autoarray-2023.3.27.1/autoarray/plot/wrap/base/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      469 2023-02-12 10:45:24.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3878 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      546 2023-02-12 10:45:24.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/annotate.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1904 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/axis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4007 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/cmap.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3716 2023-03-18 17:02:31.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/colorbar.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      448 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/colorbar_tickparams.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3046 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/figure.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4223 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/label.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/legend.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5984 2023-02-17 16:36:56.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/output.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      527 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/text.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      542 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/tickparams.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7713 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/ticks.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      912 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/title.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2420 2022-12-02 11:50:15.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/base/units.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.718582 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      133 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1963 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/avxline.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1828 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/fill_between.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2738 2023-01-26 17:35:30.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/yx_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/yx_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44375 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/segmentdata.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.784746 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      791 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      780 2023-02-12 16:45:53.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/array_overlay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      324 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/border_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4685 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/grid_errorbar.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3735 2023-03-18 16:26:42.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/grid_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6745 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/grid_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      316 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/index_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4420 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/mask_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      288 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      310 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/origin_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/patch_overlay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      321 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/positions_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/serial_overscan_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      273 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/serial_prescan_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1222 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/vector_yx_quiver.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3138 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/voronoi_drawer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23168 2023-03-21 18:19:52.000000 autoarray-2023.3.27.1/autoarray/preloads.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.795969 autoarray-2023.3.27.1/autoarray/structures/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-13 18:02:25.000000 autoarray-2023.3.27.1/autoarray/structures/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2961 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/abstract_structure.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.813302 autoarray-2023.3.27.1/autoarray/structures/arrays/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:40:14.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9231 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/array_1d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31360 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/array_2d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4905 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/irregular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18873 2023-03-21 18:18:00.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/kernel_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11031 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/uniform_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42411 2023-01-27 18:12:01.000000 autoarray-2023.3.27.1/autoarray/structures/arrays/uniform_2d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.842746 autoarray-2023.3.27.1/autoarray/structures/grids/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:32:21.000000 autoarray-2023.3.27.1/autoarray/structures/grids/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9420 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/structures/grids/grid_1d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32885 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/structures/grids/grid_2d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18582 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/grids/irregular_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41151 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/structures/grids/iterate_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8542 2023-01-14 20:55:19.000000 autoarray-2023.3.27.1/autoarray/structures/grids/sparse_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5502 2023-03-13 18:37:33.000000 autoarray-2023.3.27.1/autoarray/structures/grids/sparse_2d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      258 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/grids/transformed_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18089 2023-01-17 18:33:57.000000 autoarray-2023.3.27.1/autoarray/structures/grids/uniform_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48031 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/structures/grids/uniform_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1581 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/structures/header.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.857951 autoarray-2023.3.27.1/autoarray/structures/mesh/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/structures/mesh/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/mesh/abstract_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3544 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/structures/mesh/delaunay_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7848 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/structures/mesh/rectangular_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10542 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/structures/mesh/triangulation_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3649 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/structures/mesh/voronoi_2d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.866039 autoarray-2023.3.27.1/autoarray/structures/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/structures/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2683 2022-12-29 16:03:57.000000 autoarray-2023.3.27.1/autoarray/structures/mock/mock_grid.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10879 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/mock/mock_structure_decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.870600 autoarray-2023.3.27.1/autoarray/structures/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/structures/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7227 2022-11-11 15:49:29.000000 autoarray-2023.3.27.1/autoarray/structures/plot/structure_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22133 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/structure_decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.882193 autoarray-2023.3.27.1/autoarray/structures/vectors/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/structures/vectors/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1030 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/vectors/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5749 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/vectors/irregular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21676 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/structures/vectors/uniform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9558 2023-03-13 19:00:38.000000 autoarray-2023.3.27.1/autoarray/structures/visibilities.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1692 2023-01-13 16:54:26.000000 autoarray-2023.3.27.1/autoarray/type.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.887215 autoarray-2023.3.27.1/autoarray/util/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2603 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/misc_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.892371 autoarray-2023.3.27.1/autoarray/util/nn/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1731 2023-03-21 17:41:19.000000 autoarray-2023.3.27.1/autoarray/util/nn/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3899 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/nn_py.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:06.896889 autoarray-2023.3.27.1/autoarray/util/nn/src/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1248 2022-12-20 22:03:05.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/README.md
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.077648 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      558 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/.indent.pro
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5420 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/CHANGELOG
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/CUSTOMISE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      166 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/config.h.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141175 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/configure
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2745 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/configure.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19071 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/delaunay.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1261 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/delaunay.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2408 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/delaunay_internal.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3877 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/distribute.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      717 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/distribute.h
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.081767 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.102166 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      233 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/generate.awk
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       64 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/suptitle.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1430 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/viewexample.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.145475 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1258 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   240932 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      835 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/mpitest.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/suptitle.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      760 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      997 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/viewdata.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1229 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2958 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/viewinterp.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.172594 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1300 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/generate-data.awk
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      235 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/generate-points.awk
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       46 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/test.sh
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.206841 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      556 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132840 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       56 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      999 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/viewdata.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1244 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2966 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/viewinterp.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.246092 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      456 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1407289 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       54 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      461 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      536 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2981 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/viewinterp.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2614 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/viewinterp2.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.275236 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      613 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   165065 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       45 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       34 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2979 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/viewinterp.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      655 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22150 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/hash.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2040 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/hash.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4772 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/install-sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1398 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/istack.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      767 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/istack.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      600 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/istack_internal.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4154 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/lpi.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3271 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/makefile.example
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/makefile.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3145 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/makefile_autolens
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36312 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/minell.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      920 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/minell.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/mkinstalldirs
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      891 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nan.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10955 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nn.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      949 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nn_internal.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11021 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnai.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30764 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnbathy.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2344 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nncommon-vulnerable.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14340 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nncommon.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      390 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nncommon.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnconfig.h.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2220 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnhpi_customized.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40728 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnpi.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      183 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnpi.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4699 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/preader.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/preader.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2326 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/sample.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   652743 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/triangle.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21562 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/triangle.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/autoarray/util/nn/src/nn/version.c
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.288433 autoarray-2023.3.27.1/autoarray.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14065 2023-03-27 14:48:06.000000 autoarray-2023.3.27.1/autoarray.egg-info/SOURCES.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.282368 autoarray-2023.3.27.1/docs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/docs/Makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3628 2021-06-17 13:08:16.000000 autoarray-2023.3.27.1/docs/conf.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       26 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/docs/index.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/docs/make.bat
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/eden.ini
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:48:07.287414 autoarray-2023.3.27.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2021-06-17 13:08:16.000000 autoarray-2023.3.27.1/files/eden.ini
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      546 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/files/release.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      626 2021-04-02 09:27:57.000000 autoarray-2023.3.27.1/files/to_do_list
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2022-12-02 11:50:15.000000 autoarray-2023.3.27.1/optional_requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-11-04 15:14:02.000000 autoarray-2023.3.27.1/readthedocs.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      141 2023-03-21 17:41:15.000000 autoarray-2023.3.27.1/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-03-27 14:48:07.290477 autoarray-2023.3.27.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2039 2023-03-27 14:45:03.000000 autoarray-2023.3.27.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1578 2023-03-08 13:36:03.000000 autoarray-2023.3.27.1/to_do_list
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.047043 autoarray-2023.7.7.1/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.601516 autoarray-2023.7.7.1/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.666601 autoarray-2023.7.7.1/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3065 2022-12-19 16:37:07.000000 autoarray-2023.7.7.1/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-02 11:50:15.000000 autoarray-2023.7.7.1/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1006 2023-06-07 09:44:45.046043 autoarray-2023.7.7.1/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2022-05-03 18:33:14.000000 autoarray-2023.7.7.1/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.685670 autoarray-2023.7.7.1/autoarray/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4721 2023-06-07 09:38:14.000000 autoarray-2023.7.7.1/autoarray/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1656 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/abstract_ndarray.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.698728 autoarray-2023.7.7.1/autoarray/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2023-06-06 18:37:08.000000 autoarray-2023.7.7.1/autoarray/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       57 2022-11-29 17:43:26.000000 autoarray-2023.7.7.1/autoarray/config/grids.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      416 2021-06-17 13:08:16.000000 autoarray-2023.7.7.1/autoarray/config/logging.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.722473 autoarray-2023.7.7.1/autoarray/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-02 11:50:15.000000 autoarray-2023.7.7.1/autoarray/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2775 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1412 2022-12-21 13:17:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/include.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4233 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1209 2022-12-02 11:50:15.000000 autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_1d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3987 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_2d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3208 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/plots.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.728474 autoarray-2023.7.7.1/autoarray/dataset/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/dataset/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.740728 autoarray-2023.7.7.1/autoarray/dataset/abstract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4826 2023-06-03 08:48:54.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4663 2023-05-17 16:06:23.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.755774 autoarray-2023.7.7.1/autoarray/dataset/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12906 2023-06-03 08:47:07.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3269 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4573 2023-06-03 08:45:47.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2023-02-06 13:53:42.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.770787 autoarray-2023.7.7.1/autoarray/dataset/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7830 2023-06-03 09:02:33.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2471 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3700 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2043 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.776787 autoarray-2023.7.7.1/autoarray/dataset/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/dataset/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      192 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/dataset/mock/mock_dataset.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.784805 autoarray-2023.7.7.1/autoarray/dataset/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/dataset/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8157 2023-06-03 08:56:57.000000 autoarray-2023.7.7.1/autoarray/dataset/plot/imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12160 2023-06-03 16:54:06.000000 autoarray-2023.7.7.1/autoarray/dataset/plot/interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20436 2023-06-03 09:10:24.000000 autoarray-2023.7.7.1/autoarray/dataset/preprocess.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3138 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.799861 autoarray-2023.7.7.1/autoarray/fit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/fit/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11912 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/fit_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2592 2023-06-03 08:43:24.000000 autoarray-2023.7.7.1/autoarray/fit/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6016 2023-06-03 09:34:51.000000 autoarray-2023.7.7.1/autoarray/fit/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18328 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/fit_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.807893 autoarray-2023.7.7.1/autoarray/fit/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/fit/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1304 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      894 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.821117 autoarray-2023.7.7.1/autoarray/fit/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/fit/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11054 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/plot/fit_imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22589 2023-06-03 16:41:28.000000 autoarray-2023.7.7.1/autoarray/fit/plot/fit_interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10437 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/plot/fit_vector_yx_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13605 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.838408 autoarray-2023.7.7.1/autoarray/geometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/geometry/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1065 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/abstract_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2768 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12385 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1687 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_2d_irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27690 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.841405 autoarray-2023.7.7.1/autoarray/inversion/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-19 14:59:34.000000 autoarray-2023.7.7.1/autoarray/inversion/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.864525 autoarray-2023.7.7.1/autoarray/inversion/inversion/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:42.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35991 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15443 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/factory.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.882596 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11938 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34720 2023-06-03 09:10:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12033 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/mapping.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27386 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.904699 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6128 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5655 2023-03-13 18:37:33.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5331 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/lop.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8257 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/mapping.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9532 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/w_tilde.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12793 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42583 2023-04-24 16:16:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38687 2023-04-24 16:16:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret_clean.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4733 2023-06-03 09:10:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.920745 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4922 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/func_list.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7267 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/linear_obj.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2022-12-21 17:08:33.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/neighbors.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1701 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/unique_mappings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.953848 autoarray-2023.7.7.1/autoarray/inversion/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6792 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3080 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      888 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      912 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj_func_list.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2270 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1675 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mesh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1023 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_pixelization.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      508 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_regularization.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.963927 autoarray-2023.7.7.1/autoarray/inversion/pixelization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.992150 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21230 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10119 2023-03-13 19:00:38.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/delaunay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3235 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/factory.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3665 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_grids.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27357 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6780 2023-03-13 19:00:38.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/rectangular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12734 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/voronoi.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.021248 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5486 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13091 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/delaunay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24438 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/mesh_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7143 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/rectangular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4713 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/triangulation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13162 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5281 2022-12-22 08:54:23.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi_nn.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7677 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/pixelization.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1451 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.030452 autoarray-2023.7.7.1/autoarray/inversion/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10447 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/plot/inversion_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6803 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/plot/mapper_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.065747 autoarray-2023.7.7.1/autoarray/inversion/regularization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      455 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8894 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4728 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4508 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5208 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3391 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/brightness_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2964 2023-02-06 13:53:42.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/constant.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3226 2022-12-19 16:33:57.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_split.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2187 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15369 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/regularization_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3030 2023-02-06 13:53:42.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/zeroth.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.075741 autoarray-2023.7.7.1/autoarray/layout/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-06-17 13:08:16.000000 autoarray-2023.7.7.1/autoarray/layout/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11370 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/layout/layout.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7309 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/layout/layout_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14064 2023-05-25 17:19:43.000000 autoarray-2023.7.7.1/autoarray/layout/region.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.093025 autoarray-2023.7.7.1/autoarray/mask/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/mask/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5222 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/abstract_mask.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.113102 autoarray-2023.7.7.1/autoarray/mask/derive/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-29 16:03:57.000000 autoarray-2023.7.7.1/autoarray/mask/derive/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3485 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/grid_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16580 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/grid_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21875 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/derive/indexes_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5317 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21304 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5990 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3659 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35868 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48943 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_2d_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.119100 autoarray-2023.7.7.1/autoarray/mask/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/mask/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mock/mock_mask.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1556 2023-02-12 10:43:58.000000 autoarray-2023.7.7.1/autoarray/mock.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4767 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/numba_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.130113 autoarray-2023.7.7.1/autoarray/operators/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/operators/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22050 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/operators/convolver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.136164 autoarray-2023.7.7.1/autoarray/operators/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/operators/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      244 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/operators/mock/mock_convolver.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11017 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/operators/transformer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7717 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/operators/transformer_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.148178 autoarray-2023.7.7.1/autoarray/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3668 2023-06-03 09:03:18.000000 autoarray-2023.7.7.1/autoarray/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7455 2023-06-03 10:15:39.000000 autoarray-2023.7.7.1/autoarray/plot/abstract_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      477 2023-06-03 16:38:13.000000 autoarray-2023.7.7.1/autoarray/plot/auto_labels.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.159197 autoarray-2023.7.7.1/autoarray/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2662 2022-12-21 17:08:33.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2394 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9159 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.171054 autoarray-2023.7.7.1/autoarray/plot/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/include/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1718 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/include/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1263 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/include/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4182 2022-12-21 13:25:52.000000 autoarray-2023.7.7.1/autoarray/plot/include/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.183088 autoarray-2023.7.7.1/autoarray/plot/mat_plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10623 2023-06-03 16:30:58.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10971 2023-06-03 09:24:37.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26131 2023-06-04 12:43:35.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2319 2023-05-15 17:44:36.000000 autoarray-2023.7.7.1/autoarray/plot/multi_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.195184 autoarray-2023.7.7.1/autoarray/plot/visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2690 2023-05-12 10:15:02.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1262 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3396 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.201183 autoarray-2023.7.7.1/autoarray/plot/wrap/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2250 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.256874 autoarray-2023.7.7.1/autoarray/plot/wrap/base/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      469 2023-02-12 10:45:24.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3900 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/annotate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1900 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/axis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3736 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/cmap.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6309 2023-05-15 17:44:36.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/colorbar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      446 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/colorbar_tickparams.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/figure.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2865 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/label.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      789 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/legend.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6068 2023-06-05 13:02:24.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      525 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/text.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      542 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/tickparams.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13250 2023-06-05 13:24:35.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/ticks.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/title.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2166 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/units.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.277894 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      133 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1961 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/avxline.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1826 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/fill_between.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2802 2023-06-03 16:54:27.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44375 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/segmentdata.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.343403 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      791 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      778 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/array_overlay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      324 2022-12-29 16:03:57.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/border_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4685 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_errorbar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3733 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6735 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      316 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/index_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4542 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2022-12-29 16:03:57.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/mask_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      288 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      310 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/origin_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/patch_overlay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      321 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/positions_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/serial_overscan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      273 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/serial_prescan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1222 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/vector_yx_quiver.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3220 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/voronoi_drawer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22159 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/preloads.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.356530 autoarray-2023.7.7.1/autoarray/structures/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-13 18:02:25.000000 autoarray-2023.7.7.1/autoarray/structures/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2955 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/abstract_structure.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.378549 autoarray-2023.7.7.1/autoarray/structures/arrays/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:40:14.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9227 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/array_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31344 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/array_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4901 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18861 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/kernel_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11029 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42401 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_2d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.408648 autoarray-2023.7.7.1/autoarray/structures/grids/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:32:21.000000 autoarray-2023.7.7.1/autoarray/structures/grids/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9412 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/grid_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32851 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/grid_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18547 2023-05-12 10:10:35.000000 autoarray-2023.7.7.1/autoarray/structures/grids/irregular_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41103 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/iterate_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8537 2023-05-11 09:40:23.000000 autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5498 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      256 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/transformed_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18087 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/uniform_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48025 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/structures/grids/uniform_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1579 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/header.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.427747 autoarray-2023.7.7.1/autoarray/structures/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/abstract_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3544 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/delaunay_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7848 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/rectangular_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10536 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/triangulation_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3645 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/voronoi_2d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.436747 autoarray-2023.7.7.1/autoarray/structures/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2679 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/structures/mock/mock_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10875 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mock/mock_structure_decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.442765 autoarray-2023.7.7.1/autoarray/structures/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7227 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/structures/plot/structure_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22127 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/structure_decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.453799 autoarray-2023.7.7.1/autoarray/structures/vectors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5747 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21670 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9550 2023-06-05 19:59:54.000000 autoarray-2023.7.7.1/autoarray/structures/visibilities.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1692 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/type.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.465209 autoarray-2023.7.7.1/autoarray/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2642 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/util/cholesky_funcs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5284 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/util/fnnls.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2603 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/misc_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.470223 autoarray-2023.7.7.1/autoarray/util/nn/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1731 2023-03-21 17:41:19.000000 autoarray-2023.7.7.1/autoarray/util/nn/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3897 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/util/nn/nn_py.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.474239 autoarray-2023.7.7.1/autoarray/util/nn/src/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1248 2022-12-20 22:03:05.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/README.md
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.645016 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      558 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/.indent.pro
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5420 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CHANGELOG
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CUSTOMISE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      166 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/config.h.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141175 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2745 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19071 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1261 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2408 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3877 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      717 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.h
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.650014 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.857596 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      233 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/generate.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       64 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/suptitle.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1430 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/viewexample.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.901234 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1258 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   240932 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      835 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/mpitest.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/suptitle.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      760 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      997 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewdata.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1229 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2958 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewinterp.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.924294 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1300 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/generate-data.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      235 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/generate-points.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       46 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/test.sh
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.957326 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      556 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132840 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       56 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      999 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewdata.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1244 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2966 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewinterp.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.994531 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      456 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1407289 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       54 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      461 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      536 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2981 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2614 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp2.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.023399 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      613 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   165065 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       45 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       34 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2979 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/viewinterp.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      655 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22150 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2040 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4772 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/install-sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1398 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      767 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      600 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4154 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/lpi.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3271 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.example
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3145 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile_autolens
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36312 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      920 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/mkinstalldirs
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      891 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nan.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10955 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      949 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11021 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnai.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30764 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnbathy.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2344 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon-vulnerable.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14340 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      390 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnconfig.h.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2220 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnhpi_customized.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40728 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnpi.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      183 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnpi.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4699 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2326 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/sample.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   652743 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21562 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/version.c
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.044044 autoarray-2023.7.7.1/autoarray.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14122 2023-06-07 09:44:43.000000 autoarray-2023.7.7.1/autoarray.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.034416 autoarray-2023.7.7.1/docs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/docs/Makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3624 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/docs/conf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       26 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/docs/index.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/docs/make.bat
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.042048 autoarray-2023.7.7.1/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2021-06-17 13:08:16.000000 autoarray-2023.7.7.1/files/eden.ini
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      546 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/files/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      626 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/files/to_do_list
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/optional_requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/readthedocs.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      141 2023-03-21 17:41:15.000000 autoarray-2023.7.7.1/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:44:45.047043 autoarray-2023.7.7.1/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2036 2023-06-07 09:44:29.000000 autoarray-2023.7.7.1/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1572 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/to_do_list
```

### Comparing `autoarray-2023.3.27.1/.github/workflows/main.yml` & `autoarray-2023.7.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/LICENSE` & `autoarray-2023.7.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/PKG-INFO` & `autoarray-2023.7.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoarray
-Version: 2023.3.27.1
+Version: 2023.7.7.1
 Summary: PyAuto Data Structures
 Home-page: https://github.com/Jammy2211/PyAutoArray
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autoarray-2023.3.27.1/autoarray/__init__.py` & `autoarray-2023.7.7.1/autoarray/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 from .structures.visibilities import Visibilities
 from .structures.visibilities import VisibilitiesNoiseMap
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.3.27.1"
+__version__ = "2023.7.7.1"
```

### Comparing `autoarray-2023.3.27.1/autoarray/abstract_ndarray.py` & `autoarray-2023.7.7.1/autoarray/abstract_ndarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,25 @@
     from autoarray.structures.abstract_structure import Structure
 
 from autoarray.structures.arrays import array_2d_util
 
 
 class AbstractNDArray(np.ndarray, ABC):
     def __reduce__(self):
-
         pickled_state = super().__reduce__()
 
         class_dict = {}
         for key, value in self.__dict__.items():
             class_dict[key] = value
         new_state = pickled_state[2] + (class_dict,)
 
         return pickled_state[0], pickled_state[1], new_state
 
     # noinspection PyMethodOverriding
     def __setstate__(self, state):
-
         for key, value in state[-1].items():
             setattr(self, key, value)
         super().__setstate__(state[0:-1])
 
     @property
     @abstractmethod
     def native(self) -> Structure:
```

### Comparing `autoarray-2023.3.27.1/autoarray/config/README.rst` & `autoarray-2023.7.7.1/autoarray/config/README.rst`

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

### Comparing `autoarray-2023.3.27.1/autoarray/config/visualize/README.rst` & `autoarray-2023.7.7.1/autoarray/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/config/visualize/include.yaml` & `autoarray-2023.7.7.1/autoarray/config/visualize/include.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/config/visualize/mat_wrap_1d.yaml` & `autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_1d.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/config/visualize/mat_wrap_2d.yaml` & `autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_2d.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -102,19 +102,19 @@
   subplot:
     edgecolor: c
     facecolor: null
 PositionsScatter:    # wrapper for `plt.scatter()`: customize the appearance of positions input via `Visuals2d.positions`.
   figure:
     c: k,m,y,b,r,g
     marker: .
-    s: 16
+    s: 32
   subplot:
     c: k,m,y,b,r,g
     marker: .
-    s: 16
+    s: 32
 VectorYXQuiver:      # wrapper for `plt.quiver()`: customize (y,x) vectors appearances (e.g. a shear field).
   figure:
     alpha: 1.0
     angles: xy
     headlength: 0
     headwidth: 1
     linewidth: 5
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/abstract/dataset.py` & `autoarray-2023.7.7.1/autoarray/dataset/abstract/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,17 +43,15 @@
         self.settings = settings
 
         mask = self.mask
 
         self.noise_covariance_matrix = noise_covariance_matrix
 
         if noise_map is None:
-
             try:
-
                 noise_map = Array2D.no_mask(
                     values=np.diag(noise_covariance_matrix),
                     shape_native=data.shape_native,
                     pixel_scales=data.shape_native,
                 )
 
                 logger.info(
@@ -63,25 +61,23 @@
                     Using the diagonal of the `noise_covariance_matrix` to create the `noise_map`. 
     
                     This `noise-map` is used only for visualization where it is not appropriate to plot covariance.
                     """
                 )
 
             except ValueError as e:
-
                 raise exc.DatasetException(
                     """
                     No noise map or noise_covariance_matrix was passed to the Imaging object.
                     """
                 ) from e
 
         self.noise_map = noise_map
 
         if conf.instance["general"]["structures"]["use_dataset_grids"]:
-
             mask_grid = mask.mask_new_sub_size_from(
                 mask=mask, sub_size=settings.sub_size
             )
             self.grid = settings.grid_from(mask=mask_grid)
 
             mask_inversion = mask.mask_new_sub_size_from(
                 mask=mask, sub_size=settings.sub_size_pixelization
@@ -104,18 +100,14 @@
         return self.mask.pixel_scales
 
     @property
     def mask(self) -> Union[Mask1D, Mask2D]:
         return self.data.mask
 
     @property
-    def inverse_noise_map(self) -> Structure:
-        return 1.0 / self.noise_map
-
-    @property
     def signal_to_noise_map(self) -> Structure:
         """
         The estimated signal-to-noise_maps mappers of the image.
 
         Warnings airse when masked native noise-maps are used, whose masked entries are given values of 0.0. We
         uses the warnings module to surpress these RunTimeWarnings.
         """
@@ -128,56 +120,26 @@
     @property
     def signal_to_noise_max(self) -> float:
         """
         The maximum value of signal-to-noise_maps in an image pixel in the image's signal-to-noise_maps mappers.
         """
         return np.max(self.signal_to_noise_map)
 
-    @property
-    def absolute_signal_to_noise_map(self) -> Structure:
-        """
-        The estimated absolute_signal-to-noise_maps mappers of the image.
-        """
-        return np.divide(np.abs(self.data), self.noise_map)
-
-    @property
-    def absolute_signal_to_noise_max(self) -> float:
-        """
-        The maximum value of absolute signal-to-noise_map in an image pixel in the image's signal-to-noise_maps mappers.
-        """
-        return np.max(self.absolute_signal_to_noise_map)
-
-    @property
-    def potential_chi_squared_map(self) -> Structure:
-        """
-        The potential chi-squared-map of the imaging data_type. This represents how much each pixel can contribute to
-        the chi-squared-map, assuming the model fails to fit it at all (e.g. model value = 0.0).
-        """
-        return np.square(self.absolute_signal_to_noise_map)
-
-    @property
-    def potential_chi_squared_max(self) -> float:
-        """
-        The maximum value of the potential chi-squared-map.
-        """
-        return np.max(self.potential_chi_squared_map)
-
     @cached_property
     def noise_covariance_matrix_inv(self) -> np.ndarray:
         """
         Returns the inverse of the noise covariance matrix, which is used when computing a chi-squared which accounts
         for covariance via a fit.
         """
         return np.linalg.inv(self.noise_covariance_matrix)
 
     def trimmed_after_convolution_from(self, kernel_shape) -> "AbstractDataset":
+        dataset = copy.copy(self)
 
-        imaging = copy.copy(self)
-
-        imaging.data = imaging.data.trimmed_after_convolution_from(
+        dataset.data = dataset.data.trimmed_after_convolution_from(
             kernel_shape=kernel_shape
         )
-        imaging.noise_map = imaging.noise_map.trimmed_after_convolution_from(
+        dataset.noise_map = dataset.noise_map.trimmed_after_convolution_from(
             kernel_shape=kernel_shape
         )
 
-        return imaging
+        return dataset
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/abstract/settings.py` & `autoarray-2023.7.7.1/autoarray/dataset/abstract/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,49 +10,45 @@
 def grid_via_grid_class_from(
     mask: Union[Mask1D, Mask2D],
     grid_class: Union[Type[Grid1D], Type[Grid2D]],
     fractional_accuracy: float,
     relative_accuracy: Optional[float],
     sub_steps: List[int],
 ) -> Optional[Union[Grid1D, Grid2D, Grid2DIterate]]:
-
     if mask.pixel_scales is None:
         return None
 
     if grid_class is None:
         if isinstance(mask, Mask1D):
             grid_class = Grid1D
         elif isinstance(mask, Mask2D):
             grid_class = Grid2D
 
     if grid_class is Grid1D:
-
         return Grid1D.from_mask(mask=mask)
 
     if grid_class is Grid2D:
-
         return Grid2D.from_mask(mask=mask)
 
     elif grid_class is Grid2DIterate:
-
         return Grid2DIterate.from_mask(
             mask=mask,
             fractional_accuracy=fractional_accuracy,
             relative_accuracy=relative_accuracy,
             sub_steps=sub_steps,
         )
 
 
 class AbstractSettingsDataset:
     def __init__(
         self,
         grid_class: Optional[Union[Type[Grid1D], Type[Grid2D]]] = None,
         grid_pixelization_class: Optional[Union[Type[Grid1D], Type[Grid2D]]] = None,
-        sub_size: int = 2,
-        sub_size_pixelization: int = 2,
+        sub_size: int = 1,
+        sub_size_pixelization: int = 4,
         fractional_accuracy: float = 0.9999,
         relative_accuracy: Optional[float] = None,
         sub_steps: Tuple[int] = (2, 4, 8, 16),
     ):
         """
         A dataset is a collection of data structures (e.g. the data, noise-map, PSF), a mask, grid, convolver
         and other utilities that are used for modeling and fitting an image of a strong lens.
@@ -89,25 +85,23 @@
         self.sub_size = sub_size
         self.sub_size_pixelization = sub_size_pixelization
         self.fractional_accuracy = fractional_accuracy
         self.relative_accuracy = relative_accuracy
         self.sub_steps = sub_steps
 
     def grid_from(self, mask) -> Union[Grid1D, Grid2D]:
-
         return grid_via_grid_class_from(
             mask=mask,
             grid_class=self.grid_class,
             fractional_accuracy=self.fractional_accuracy,
             relative_accuracy=self.relative_accuracy,
             sub_steps=self.sub_steps,
         )
 
     def grid_pixelization_from(self, mask) -> Union[Grid1D, Grid2D]:
-
         return grid_via_grid_class_from(
             mask=mask,
             grid_class=self.grid_pixelization_class,
             fractional_accuracy=self.fractional_accuracy,
             relative_accuracy=self.relative_accuracy,
             sub_steps=self.sub_steps,
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/abstract/w_tilde.py` & `autoarray-2023.7.7.1/autoarray/dataset/abstract/w_tilde.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
             The first value of the noise-map used to construct the curvature preload, which is used as a sanity
             check when performing the inversion to ensure the preload corresponds to the data being fitted.
         """
         self.curvature_preload = curvature_preload
         self.noise_map_value = noise_map_value
 
     def check_noise_map(self, noise_map):
-
         if noise_map[0] != self.noise_map_value:
             raise exc.InversionException(
                 "The preloaded values of WTildeImaging are not consistent with the noise-map passed to them, thus "
                 "they cannot be used for the inversion."
                 ""
                 f"The value of the noise map is {noise_map[0]} whereas in WTildeImaging it is {self.noise_map_value}"
                 ""
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/imaging/imaging.py` & `autoarray-2023.7.7.1/autoarray/dataset/imaging/imaging.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Imaging(AbstractDataset):
     def __init__(
         self,
-        image: Array2D,
+        data: Array2D,
         noise_map: Optional[Array2D] = None,
         psf: Optional[Kernel2D] = None,
         noise_covariance_matrix: Optional[np.ndarray] = None,
         settings: SettingsImaging = SettingsImaging(),
         pad_for_convolver: bool = False,
     ):
         """
         A class containing an imaging dataset, including the image data, noise-map and a point spread function (PSF).
 
         Parameters
         ----------
-        image
+        data
             The array of the image data, for example in units of electrons per second.
         noise_map
             An array describing the RMS standard deviation error in each pixel, for example in units of electrons per
             second.
         psf
             An array describing the Point Spread Function kernel of the image which accounts for diffraction due to the
             telescope optics via 2D convolution.
@@ -48,56 +48,57 @@
         """
 
         self.unmasked = None
 
         self.pad_for_convolver = pad_for_convolver
 
         if pad_for_convolver and psf is not None:
-
             try:
-                image.mask.derive_mask.blurring_from(
+                data.mask.derive_mask.blurring_from(
                     kernel_shape_native=psf.shape_native
                 )
             except exc.MaskException:
-                image = image.padded_before_convolution_from(
+                data = data.padded_before_convolution_from(
                     kernel_shape=psf.shape_native, mask_pad_value=1
                 )
                 if noise_map is not None:
                     noise_map = noise_map.padded_before_convolution_from(
                         kernel_shape=psf.shape_native, mask_pad_value=1
                     )
                 logger.info(
                     f"The image and noise map of the `Imaging` objected have been padded to the dimensions"
-                    f"{image.shape}. This is because the blurring region around the mask (which defines where"
+                    f"{data.shape}. This is because the blurring region around the mask (which defines where"
                     f"PSF flux may be convolved into the masked region) extended beyond the edge of the image."
                     f""
                     f"This can be prevented by using a smaller mask, smaller PSF kernel size or manually padding"
                     f"the image and noise-map yourself."
                 )
 
         super().__init__(
-            data=image,
+            data=data,
             noise_map=noise_map,
             noise_covariance_matrix=noise_covariance_matrix,
             settings=settings,
         )
 
         if self.noise_map.native is not None:
-
             if ((self.noise_map.native <= 0.0) * np.invert(self.noise_map.mask)).any():
+                zero_entries = np.argwhere(self.noise_map.native <= 0.0)
+
                 raise exc.DatasetException(
                     f"""
                     A value in the noise-map of the dataset is {np.min(self.noise_map)}. 
 
                     This is less than or equal to zero, and therefore an ill-defined value which must be corrected.
+                    
+                    The 2D indexes of the arrays in the native noise map array are {zero_entries}.
                     """
                 )
 
         if psf is not None and settings.use_normalized_psf:
-
             psf = Kernel2D.no_mask(
                 values=psf.native, pixel_scales=psf.pixel_scales, normalize=True
             )
 
         self.psf = psf
 
     @property
@@ -179,18 +180,18 @@
             lengths=lengths.astype("int"),
             noise_map_value=self.noise_map[0],
         )
 
     @classmethod
     def from_fits(
         cls,
-        image_path: str,
+        data_path: str,
         pixel_scales: ty.PixelScales,
         noise_map_path: str,
-        image_hdu: int = 0,
+        data_hdu: int = 0,
         noise_map_hdu: int = 0,
         psf_path: str = None,
         psf_hdu: int = 0,
         noise_covariance_matrix: Optional[np.ndarray] = None,
     ) -> "Imaging":
         """
         Factory for loading the imaging data_type from .fits files, as well as computing properties like the noise-map,
@@ -198,53 +199,51 @@
 
         This factory also includes a number of routines for converting the imaging-data from unit_label not
         supported by PyAutoLens (e.g. adus, electrons) to electrons per second.
 
         Parameters
         ----------
         noise_map_non_constant
-        image_path
+        data_path
             The path to the image .fits file containing the image (e.g. '/path/to/image.fits')
         pixel_scales
             The size of each pixel in scaled units.
-        image_hdu
-            The hdu the image is contained in the .fits file specified by *image_path*.
+        data_hdu
+            The hdu the image is contained in the .fits file specified by *data_path*.
         psf_path
             The path to the psf .fits file containing the psf (e.g. '/path/to/psf.fits')
         psf_hdu
             The hdu the psf is contained in the .fits file specified by *psf_path*.
         noise_map_path
             The path to the noise_map .fits file containing the noise_map (e.g. '/path/to/noise_map.fits')
         noise_map_hdu
             The hdu the noise_map is contained in the .fits file specified by *noise_map_path*.
         """
 
         image = Array2D.from_fits(
-            file_path=image_path, hdu=image_hdu, pixel_scales=pixel_scales
+            file_path=data_path, hdu=data_hdu, pixel_scales=pixel_scales
         )
 
         noise_map = Array2D.from_fits(
             file_path=noise_map_path, hdu=noise_map_hdu, pixel_scales=pixel_scales
         )
 
         if psf_path is not None:
-
             psf = Kernel2D.from_fits(
                 file_path=psf_path,
                 hdu=psf_hdu,
                 pixel_scales=pixel_scales,
                 normalize=False,
             )
 
         else:
-
             psf = None
 
         return Imaging(
-            image=image,
+            data=image,
             noise_map=noise_map,
             psf=psf,
             noise_covariance_matrix=noise_covariance_matrix,
         )
 
     def apply_mask(self, mask: Mask2D) -> "Imaging":
         """
@@ -256,87 +255,85 @@
         imaging dataset.
 
         Parameters
         ----------
         mask
             The 2D mask that is applied to the image.
         """
-        if self.image.mask.is_all_false:
-            unmasked_imaging = self
+        if self.data.mask.is_all_false:
+            unmasked_dataset = self
         else:
-            unmasked_imaging = self.unmasked
+            unmasked_dataset = self.unmasked
 
-        image = Array2D(
-            values=unmasked_imaging.image.native, mask=mask.derive_mask.sub_1
+        data = Array2D(
+            values=unmasked_dataset.image.native, mask=mask.derive_mask.sub_1
         )
 
         noise_map = Array2D(
-            values=unmasked_imaging.noise_map.native, mask=mask.derive_mask.sub_1
+            values=unmasked_dataset.noise_map.native, mask=mask.derive_mask.sub_1
         )
 
-        if unmasked_imaging.noise_covariance_matrix is not None:
-
-            noise_covariance_matrix = unmasked_imaging.noise_covariance_matrix
+        if unmasked_dataset.noise_covariance_matrix is not None:
+            noise_covariance_matrix = unmasked_dataset.noise_covariance_matrix
 
             noise_covariance_matrix = np.delete(
                 noise_covariance_matrix, mask.derive_indexes.masked_slim, 0
             )
             noise_covariance_matrix = np.delete(
                 noise_covariance_matrix, mask.derive_indexes.masked_slim, 1
             )
 
         else:
-
             noise_covariance_matrix = None
 
-        imaging = Imaging(
-            image=image,
+        dataset = Imaging(
+            data=data,
             noise_map=noise_map,
             psf=self.psf,
             noise_covariance_matrix=noise_covariance_matrix,
             settings=self.settings,
             pad_for_convolver=True,
         )
 
-        imaging.unmasked = unmasked_imaging
+        dataset.unmasked = unmasked_dataset
 
         logger.info(
             f"IMAGING - Data masked, contains a total of {mask.pixels_in_mask} image-pixels"
         )
 
-        return imaging
+        return dataset
 
     def apply_settings(self, settings: SettingsImaging) -> "Imaging":
         """
         Returns a new instance of the imaging with the input `SettingsImaging` applied to them.
 
         This can be used to update settings like the types of grids associated with the dataset that are used
         to perform calculations or putting a limit of the dataset's signal-to-noise.
 
         Parameters
         ----------
         settings
             The settings for the imaging data that control things like the grids used for calculations.
         """
         return Imaging(
-            image=self.image,
+            data=self.data,
             noise_map=self.noise_map,
             psf=self.psf,
             noise_covariance_matrix=self.noise_covariance_matrix,
             settings=settings,
             pad_for_convolver=self.pad_for_convolver,
         )
 
     def output_to_fits(
         self,
-        image_path: str,
+        data_path: str,
         psf_path: str = None,
         noise_map_path: str = None,
         overwrite: bool = False,
     ):
-        self.image.output_to_fits(file_path=image_path, overwrite=overwrite)
+        self.data.output_to_fits(file_path=data_path, overwrite=overwrite)
 
         if self.psf is not None and psf_path is not None:
             self.psf.output_to_fits(file_path=psf_path, overwrite=overwrite)
 
         if self.noise_map is not None and noise_map_path is not None:
             self.noise_map.output_to_fits(file_path=noise_map_path, overwrite=overwrite)
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/imaging/settings.py` & `autoarray-2023.7.7.1/autoarray/dataset/imaging/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/imaging/simulator.py` & `autoarray-2023.7.7.1/autoarray/dataset/imaging/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,8 +119,8 @@
 
         mask = Mask2D.all_false(
             shape_native=image.shape_native, pixel_scales=image.pixel_scales
         )
 
         image = Array2D(values=image, mask=mask)
 
-        return Imaging(image=image, psf=self.psf, noise_map=noise_map)
+        return Imaging(data=image, psf=self.psf, noise_map=noise_map)
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/imaging/w_tilde.py` & `autoarray-2023.7.7.1/autoarray/dataset/imaging/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/interferometer/interferometer.py` & `autoarray-2023.7.7.1/autoarray/dataset/interferometer/interferometer.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,52 +13,52 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Interferometer(AbstractDataset):
     def __init__(
         self,
-        visibilities: Visibilities,
+        data: Visibilities,
         noise_map: VisibilitiesNoiseMap,
         uv_wavelengths: np.ndarray,
         real_space_mask,
         settings: SettingsInterferometer = SettingsInterferometer(),
     ):
         """
         A class containing an interferometer dataset, including the visibilities data, noise-map and the
         uv-plane baseline wavelengths.
 
         Parameters
         ----------
-        visibilities
+        data
             The array of the visibilities data, containing by real and complex values.
         noise_map
             An array describing the RMS standard deviation error in each visibility.
         uv_wavelengths
             The uv-plane baseline wavelengths.
         real_space_mask
             A 2D mask in real-space (e.g. not Fourier space like the visibilities) which defines in real space
             how calculations are performed.
         settings
             Controls settings of how the dataset is set up (e.g. the types of grids used to perform calculations).
         """
         self.real_space_mask = real_space_mask
 
-        super().__init__(data=visibilities, noise_map=noise_map, settings=settings)
+        super().__init__(data=data, noise_map=noise_map, settings=settings)
 
         self.uv_wavelengths = uv_wavelengths
 
         self.transformer = self.settings.transformer_class(
             uv_wavelengths=uv_wavelengths, real_space_mask=real_space_mask
         )
 
     @classmethod
     def from_fits(
         cls,
-        visibilities_path,
+        data_path,
         noise_map_path,
         uv_wavelengths_path,
         real_space_mask,
         visibilities_hdu=0,
         noise_map_hdu=0,
         uv_wavelengths_hdu=0,
         settings: SettingsInterferometer = SettingsInterferometer(),
@@ -67,38 +67,35 @@
         Factory for loading the interferometer data_type from .fits files, as well as computing properties like the
         noise-map, exposure-time map, etc. from the interferometer-data_type.
 
         This factory also includes a number of routines for converting the interferometer-data_type from unit_label
         not supported by PyAutoLens (e.g. adus, electrons) to electrons per second.
         """
 
-        visibilities = Visibilities.from_fits(
-            file_path=visibilities_path, hdu=visibilities_hdu
-        )
+        visibilities = Visibilities.from_fits(file_path=data_path, hdu=visibilities_hdu)
 
         noise_map = VisibilitiesNoiseMap.from_fits(
             file_path=noise_map_path, hdu=noise_map_hdu
         )
 
         uv_wavelengths = array_2d_util.numpy_array_2d_via_fits_from(
             file_path=uv_wavelengths_path, hdu=uv_wavelengths_hdu
         )
 
         return Interferometer(
             real_space_mask=real_space_mask,
-            visibilities=visibilities,
+            data=visibilities,
             noise_map=noise_map,
             uv_wavelengths=uv_wavelengths,
             settings=settings,
         )
 
     def apply_settings(self, settings):
-
         return Interferometer(
-            visibilities=self.visibilities,
+            data=self.data,
             noise_map=self.noise_map,
             uv_wavelengths=self.uv_wavelengths,
             real_space_mask=self.real_space_mask,
             settings=settings,
         )
 
     @cached_property
@@ -132,16 +129,16 @@
 
         w_matrix = inversion_util_secret.w_tilde_via_preload_from(
             w_tilde_preload=curvature_preload,
             native_index_for_slim_index=self.real_space_mask.derive_indexes.native_for_slim,
         )
 
         dirty_image = self.transformer.image_from(
-            visibilities=self.visibilities.real * self.noise_map.real**-2.0
-            + 1j * self.visibilities.imag * self.noise_map.imag**-2.0,
+            visibilities=self.data.real * self.noise_map.real**-2.0
+            + 1j * self.data.imag * self.noise_map.imag**-2.0,
             use_adjoint_scaling=True,
         )
 
         return WTildeInterferometer(
             w_matrix=w_matrix,
             curvature_preload=curvature_preload,
             dirty_image=dirty_image,
@@ -155,45 +152,40 @@
 
     @property
     def visibilities(self):
         return self.data
 
     @property
     def amplitudes(self):
-        return self.visibilities.amplitudes
+        return self.data.amplitudes
 
     @property
     def phases(self):
-        return self.visibilities.phases
+        return self.data.phases
 
     @property
     def uv_distances(self):
         return np.sqrt(
             np.square(self.uv_wavelengths[:, 0]) + np.square(self.uv_wavelengths[:, 1])
         )
 
     @property
     def dirty_image(self):
-        return self.transformer.image_from(visibilities=self.visibilities)
+        return self.transformer.image_from(visibilities=self.data)
 
     @property
     def dirty_noise_map(self):
         return self.transformer.image_from(visibilities=self.noise_map)
 
     @property
     def dirty_signal_to_noise_map(self):
         return self.transformer.image_from(visibilities=self.signal_to_noise_map)
 
     @property
-    def dirty_inverse_noise_map(self):
-        return self.transformer.image_from(visibilities=self.inverse_noise_map)
-
-    @property
     def signal_to_noise_map(self):
-
         signal_to_noise_map_real = np.divide(
             np.real(self.data), np.real(self.noise_map)
         )
         signal_to_noise_map_real[signal_to_noise_map_real < 0] = 0.0
         signal_to_noise_map_imag = np.divide(
             np.imag(self.data), np.imag(self.noise_map)
         )
@@ -207,24 +199,21 @@
 
     @property
     def convolver(self):
         return None
 
     def output_to_fits(
         self,
-        visibilities_path=None,
+        data_path=None,
         noise_map_path=None,
         uv_wavelengths_path=None,
         overwrite=False,
     ):
-
-        if visibilities_path is not None:
-            self.visibilities.output_to_fits(
-                file_path=visibilities_path, overwrite=overwrite
-            )
+        if data_path is not None:
+            self.data.output_to_fits(file_path=data_path, overwrite=overwrite)
 
         if self.noise_map is not None and noise_map_path is not None:
             self.noise_map.output_to_fits(file_path=noise_map_path, overwrite=overwrite)
 
         if self.uv_wavelengths is not None and uv_wavelengths_path is not None:
             array_2d_util.numpy_array_2d_to_fits(
                 array_2d=self.uv_wavelengths,
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/interferometer/settings.py` & `autoarray-2023.7.7.1/autoarray/dataset/interferometer/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/interferometer/simulator.py` & `autoarray-2023.7.7.1/autoarray/dataset/interferometer/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,12 +84,12 @@
         if np.isnan(noise_map).any():
             raise exc.DatasetException(
                 "The noise-map has NaN values in it. This suggests your exposure time and / or"
                 "background sky levels are too low, creating signal counts at or close to 0.0."
             )
 
         return Interferometer(
-            visibilities=visibilities,
+            data=visibilities,
             noise_map=noise_map,
             uv_wavelengths=transformer.uv_wavelengths,
             real_space_mask=image.mask,
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/interferometer/w_tilde.py` & `autoarray-2023.7.7.1/autoarray/dataset/interferometer/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/plot/imaging_plotters.py` & `autoarray-2023.7.7.1/autoarray/fit/plot/fit_imaging_plotters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,258 +1,274 @@
 from typing import Callable
 
+from autoarray.plot.abstract_plotters import Plotter
 from autoarray.plot.visuals.two_d import Visuals2D
 from autoarray.plot.include.two_d import Include2D
 from autoarray.plot.mat_plot.two_d import MatPlot2D
 from autoarray.plot.auto_labels import AutoLabels
-from autoarray.plot.abstract_plotters import Plotter
-from autoarray.dataset.imaging.imaging import Imaging
+from autoarray.fit.fit_imaging import FitImaging
 
 
-class ImagingPlotterMeta(Plotter):
+class FitImagingPlotterMeta(Plotter):
     def __init__(
         self,
-        imaging: Imaging,
+        fit,
         get_visuals_2d: Callable,
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
+        residuals_symmetric_cmap: bool = True,
     ):
         """
-        Plots the attributes of `Imaging` objects using the matplotlib method `imshow()` and many other matplotlib
+        Plots the attributes of `FitImaging` objects using the matplotlib method `imshow()` and many other matplotlib
         functions which customize the plot's appearance.
 
         The `mat_plot_2d` attribute wraps matplotlib function calls to make the figure. By default, the settings
         passed to every matplotlib function called are those specified in the `config/visualize/mat_wrap/*.ini` files,
         but a user can manually input values into `MatPlot2d` to customize the figure's appearance.
 
         Overlaid on the figure are visuals, contained in the `Visuals2D` object. Attributes may be extracted from
-        the `Imaging` and plotted via the visuals object, if the corresponding entry is `True` in the `Include2D`
+        the `FitImaging` and plotted via the visuals object, if the corresponding entry is `True` in the `Include2D`
         object or the `config/visualize/include.ini` file.
 
         Parameters
         ----------
-        imaging
-            The imaging dataset the plotter plots.
+        fit
+            The fit to an imaging dataset the plotter plots.
         get_visuals_2d
-            A function which extracts from the `Imaging` the 2D visuals which are plotted on figures.
+            A function which extracts from the `FitImaging` the 2D visuals which are plotted on figures.
         mat_plot_2d
-            Contains objects which wrap the matplotlib function calls that make 2D plots.
+            Contains objects which wrap the matplotlib function calls that make the plot.
         visuals_2d
-            Contains 2D visuals that can be overlaid on 2D plots.
+            Contains visuals that can be overlaid on the plot.
         include_2d
-            Specifies which attributes of the `Imaging` are extracted and plotted as visuals for 2D plots.
+            Specifies which attributes of the `Array2D` are extracted and plotted as visuals.
+        residuals_symmetric_cmap
+            If true, the `residual_map` and `normalized_residual_map` are plotted with a symmetric color map such
+            that `abs(vmin) = abs(vmax)`.
         """
-
         super().__init__(
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
-        self.imaging = imaging
+        self.fit = fit
         self.get_visuals_2d = get_visuals_2d
+        self.residuals_symmetric_cmap = residuals_symmetric_cmap
 
     def figures_2d(
         self,
-        image: bool = False,
+        data: bool = False,
         noise_map: bool = False,
-        psf: bool = False,
-        inverse_noise_map: bool = False,
         signal_to_noise_map: bool = False,
-        absolute_signal_to_noise_map: bool = False,
-        potential_chi_squared_map: bool = False,
+        model_image: bool = False,
+        residual_map: bool = False,
+        normalized_residual_map: bool = False,
+        chi_squared_map: bool = False,
+        suffix: str = "",
     ):
         """
-        Plots the individual attributes of the plotter's `Imaging` object in 2D.
+        Plots the individual attributes of the plotter's `FitImaging` object in 2D.
 
-        The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
+        The API is such that every plottable attribute of the `FitImaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
-        image
+        data
             Whether to make a 2D plot (via `imshow`) of the image data.
         noise_map
             Whether to make a 2D plot (via `imshow`) of the noise map.
-        psf
-            Whether to make a 2D plot (via `imshow`) of the psf.
-        inverse_noise_map
-            Whether to make a 2D plot (via `imshow`) of the inverse noise map.
         signal_to_noise_map
             Whether to make a 2D plot (via `imshow`) of the signal-to-noise map.
-        absolute_signal_to_noise_map
-            Whether to make a 2D plot (via `imshow`) of the absolute signal to noise map.
-        potential_chi_squared_map
-            Whether to make a 2D plot (via `imshow`) of the potential chi squared map.
+        model_image
+            Whether to make a 2D plot (via `imshow`) of the model image.
+        residual_map
+            Whether to make a 2D plot (via `imshow`) of the residual map.
+        normalized_residual_map
+            Whether to make a 2D plot (via `imshow`) of the normalized residual map.
+        chi_squared_map
+            Whether to make a 2D plot (via `imshow`) of the chi-squared map.
         """
 
-        if image:
+        if data:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.image,
+                array=self.fit.data,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(title="Image", filename="image_2d"),
+                auto_labels=AutoLabels(title="Image", filename=f"data{suffix}"),
             )
 
         if noise_map:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.noise_map,
+                array=self.fit.noise_map,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels("Noise-Map", filename="noise_map"),
+                auto_labels=AutoLabels(
+                    title="Noise-Map", filename=f"noise_map{suffix}"
+                ),
             )
 
-        if psf:
+        if signal_to_noise_map:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.psf,
+                array=self.fit.signal_to_noise_map,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(title="Point Spread Function", filename="psf"),
+                auto_labels=AutoLabels(
+                    title="Signal-To-Noise Map", filename=f"signal_to_noise_map{suffix}"
+                ),
             )
 
-        if inverse_noise_map:
+        if model_image:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.inverse_noise_map,
+                array=self.fit.model_data,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Inverse Noise-Map", filename="inverse_noise_map"
+                    title="Model Image", filename=f"model_image{suffix}"
                 ),
             )
 
-        if signal_to_noise_map:
+        cmap_original = self.mat_plot_2d.cmap
+
+        if self.residuals_symmetric_cmap:
+            self.mat_plot_2d.cmap = self.mat_plot_2d.cmap.symmetric
+
+        if residual_map:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.signal_to_noise_map,
+                array=self.fit.residual_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Signal-To-Noise Map", filename="signal_to_noise_map"
+                    title="Residual Map", filename=f"residual_map{suffix}"
                 ),
             )
 
-        if absolute_signal_to_noise_map:
+        if normalized_residual_map:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.absolute_signal_to_noise_map,
+                array=self.fit.normalized_residual_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Absolute Signal-To-Noise Map",
-                    filename="absolute_signal_to_noise_map",
+                    title="Normalized Residual Map",
+                    filename=f"normalized_residual_map{suffix}",
                 ),
             )
 
-        if potential_chi_squared_map:
+        self.mat_plot_2d.cmap = cmap_original
+
+        if chi_squared_map:
             self.mat_plot_2d.plot_array(
-                array=self.imaging.potential_chi_squared_map,
+                array=self.fit.chi_squared_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Potential Chi-Squared Map",
-                    filename="potential_chi_squared_map",
+                    title="Chi-Squared Map", filename=f"chi_squared_map{suffix}"
                 ),
             )
 
     def subplot(
         self,
-        image: bool = False,
+        data: bool = False,
         noise_map: bool = False,
-        psf: bool = False,
         signal_to_noise_map: bool = False,
-        inverse_noise_map: bool = False,
-        absolute_signal_to_noise_map: bool = False,
-        potential_chi_squared_map: bool = False,
-        auto_filename: str = "subplot_imaging",
+        model_image: bool = False,
+        residual_map: bool = False,
+        normalized_residual_map: bool = False,
+        chi_squared_map: bool = False,
+        auto_filename: str = "subplot_fit",
     ):
         """
-        Plots the individual attributes of the plotter's `Imaging` object in 2D on a subplot.
+        Plots the individual attributes of the plotter's `FitImaging` object in 2D on a subplot.
 
-        The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
+        The API is such that every plottable attribute of the `FitImaging` object is an input parameter of type bool of
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
-        inverse_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the inverse noise map.
+            Whether to include a 2D plot (via `imshow`) of the psf.
         signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the signal-to-noise map.
-        absolute_signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the absolute signal to noise map.
-        potential_chi_squared_map
-            Whether or not to include a 2D plot (via `imshow`) of the potential chi squared map.
+            Whether to include a 2D plot (via `imshow`) of the signal-to-noise map.
+        model_image
+            Whether to include a 2D plot (via `imshow`) of the model image.
+        residual_map
+            Whether to include a 2D plot (via `imshow`) of the residual map.
+        normalized_residual_map
+            Whether to include a 2D plot (via `imshow`) of the normalized residual map.
+        chi_squared_map
+            Whether to include a 2D plot (via `imshow`) of the chi-squared map.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
         self._subplot_custom_plot(
-            image=image,
+            data=data,
             noise_map=noise_map,
-            psf=psf,
             signal_to_noise_map=signal_to_noise_map,
-            inverse_noise_map=inverse_noise_map,
-            absolute_signal_to_noise_map=absolute_signal_to_noise_map,
-            potential_chi_squared_map=potential_chi_squared_map,
+            model_image=model_image,
+            residual_map=residual_map,
+            normalized_residual_map=normalized_residual_map,
+            chi_squared_map=chi_squared_map,
             auto_labels=AutoLabels(filename=auto_filename),
         )
 
-    def subplot_imaging(self):
+    def subplot_fit(self):
         """
-        Standard subplot of the attributes of the plotter's `Imaging` object.
+        Standard subplot of the attributes of the plotter's `FitImaging` object.
         """
-        self.subplot(
-            image=True,
-            noise_map=True,
-            psf=True,
+        return self.subplot(
+            data=True,
             signal_to_noise_map=True,
-            inverse_noise_map=True,
-            potential_chi_squared_map=True,
+            model_image=True,
+            residual_map=True,
+            normalized_residual_map=True,
+            chi_squared_map=True,
         )
 
 
-class ImagingPlotter(Plotter):
+class FitImagingPlotter(Plotter):
     def __init__(
         self,
-        imaging: Imaging,
+        fit: FitImaging,
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
     ):
         """
-        Plots the attributes of `Imaging` objects using the matplotlib method `imshow()` and many other matplotlib
+        Plots the attributes of `FitImaging` objects using the matplotlib method `imshow()` and many other matplotlib
         functions which customize the plot's appearance.
 
         The `mat_plot_2d` attribute wraps matplotlib function calls to make the figure. By default, the settings
         passed to every matplotlib function called are those specified in the `config/visualize/mat_wrap/*.ini` files,
         but a user can manually input values into `MatPlot2d` to customize the figure's appearance.
 
         Overlaid on the figure are visuals, contained in the `Visuals2D` object. Attributes may be extracted from
-        the `Imaging` and plotted via the visuals object, if the corresponding entry is `True` in the `Include2D`
+        the `FitImaging` and plotted via the visuals object, if the corresponding entry is `True` in the `Include2D`
         object or the `config/visualize/include.ini` file.
 
         Parameters
         ----------
-        imaging
-            The imaging dataset the plotter plots.
+        fit
+            The fit to an imaging dataset the plotter plots.
         mat_plot_2d
-            Contains objects which wrap the matplotlib function calls that make 2D plots.
+            Contains objects which wrap the matplotlib function calls that make the plot.
         visuals_2d
-            Contains 2D visuals that can be overlaid on 2D plots.
+            Contains visuals that can be overlaid on the plot.
         include_2d
-            Specifies which attributes of the `Imaging` are extracted and plotted as visuals for 2D plots.
+            Specifies which attributes of the `Array2D` are extracted and plotted as visuals.
         """
-
         super().__init__(
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
-        self.imaging = imaging
+        self.fit = fit
 
-        self._imaging_meta_plotter = ImagingPlotterMeta(
-            imaging=self.imaging,
+        self._fit_imaging_meta_plotter = FitImagingPlotterMeta(
+            fit=self.fit,
             get_visuals_2d=self.get_visuals_2d,
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
         )
 
-        self.figures_2d = self._imaging_meta_plotter.figures_2d
-        self.subplot = self._imaging_meta_plotter.subplot
-        self.subplot_imaging = self._imaging_meta_plotter.subplot_imaging
+        self.figures_2d = self._fit_imaging_meta_plotter.figures_2d
+        self.subplot = self._fit_imaging_meta_plotter.subplot
+        self.subplot_fit = self._fit_imaging_meta_plotter.subplot_fit
 
-    def get_visuals_2d(self):
-        return self.get_2d.via_mask_from(mask=self.imaging.mask)
+    def get_visuals_2d(self) -> Visuals2D:
+        return self.get_2d.via_fit_imaging_from(fit=self.fit)
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/plot/interferometer_plotters.py` & `autoarray-2023.7.7.1/autoarray/dataset/plot/interferometer_plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from autoarray.dataset.interferometer.interferometer import Interferometer
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
 
 class InterferometerPlotter(Plotter):
     def __init__(
         self,
-        interferometer: Interferometer,
+        dataset: Interferometer,
         mat_plot_1d: MatPlot1D = MatPlot1D(),
         visuals_1d: Visuals1D = Visuals1D(),
         include_1d: Include1D = Include1D(),
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
     ):
@@ -32,66 +32,69 @@
 
         Overlaid on the figure are visuals, contained in the `Visuals1D` and `Visuals2D` objects. Attributes may be
         extracted from the `LightProfile` and plotted via the visuals object, if the corresponding entry is `True` in
         the `Include1D` or `Include2D` object or the `config/visualize/include.ini` file.
 
         Parameters
         ----------
-        interferometer
+        dataset
             The interferometer dataset the plotter plots.
         mat_plot_1d
             Contains objects which wrap the matplotlib function calls that make 1D plots.
         visuals_1d
             Contains 1D visuals that can be overlaid on 1D plots.
         include_1d
             Specifies which attributes of the `Interferometer` are extracted and plotted as visuals for 1D plots.
         mat_plot_2d
             Contains objects which wrap the matplotlib function calls that make 2D plots.
         visuals_2d
             Contains 2D visuals that can be overlaid on 2D plots.
         include_2d
             Specifies which attributes of the `Interferometer` are extracted and plotted as visuals for 2D plots.
         """
-        self.interferometer = interferometer
+        self.dataset = dataset
 
         super().__init__(
             mat_plot_1d=mat_plot_1d,
             include_1d=include_1d,
             visuals_1d=visuals_1d,
             mat_plot_2d=mat_plot_2d,
             include_2d=include_2d,
             visuals_2d=visuals_2d,
         )
 
+    @property
+    def interferometer(self):
+        return self.dataset
+
     def get_visuals_2d_real_space(self):
-        return self.get_2d.via_mask_from(mask=self.interferometer.real_space_mask)
+        return self.get_2d.via_mask_from(mask=self.dataset.real_space_mask)
 
     def figures_2d(
         self,
-        visibilities: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         u_wavelengths: bool = False,
         v_wavelengths: bool = False,
         uv_wavelengths: bool = False,
         amplitudes_vs_uv_distances: bool = False,
         phases_vs_uv_distances: bool = False,
         dirty_image: bool = False,
         dirty_noise_map: bool = False,
         dirty_signal_to_noise_map: bool = False,
-        dirty_inverse_noise_map: bool = False,
     ):
         """
         Plots the individual attributes of the plotter's `Interferometer` object in 1D and 2D.
 
         The API is such that every plottable attribute of the `Interferometer` object is an input parameter of type
         bool of the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
-        visibilities
+        data
             Whether to make a 2D plot (via `scatter`) of the visibility data.
         noise_map
             Whether to make a 2D plot (via `scatter`) of the noise-map.
         u_wavelengths
             Whether to make a 1D plot (via `plot`) of the u-wavelengths.
         v_wavelengths
             Whether to make a 1D plot (via `plot`) of the v-wavelengths.
@@ -101,221 +104,193 @@
             Whether to make a 1D plot (via `plot`) of the phases versis the uv distances.
         dirty_image
             Whether to make a 2D plot (via `imshow`) of the dirty image.
         dirty_noise_map
             Whether to make a 2D plot (via `imshow`) of the dirty noise map.
         dirty_signal_to_noise_map
             Whether to make a 2D plot (via `imshow`) of the dirty signal-to-noise map.
-        dirty_inverse_noise_map
-            Whether to make a 2D plot (via `imshow`) of the dirty inverse noise map.
         """
 
-        if visibilities:
-
+        if data:
             self.mat_plot_2d.plot_grid(
-                grid=self.interferometer.visibilities.in_grid,
+                grid=self.dataset.visibilities.in_grid,
                 visuals_2d=self.visuals_2d,
-                auto_labels=AutoLabels(title="Visibilities", filename="visibilities"),
+                auto_labels=AutoLabels(title="Visibilities", filename="data"),
             )
 
         if noise_map:
-
             self.mat_plot_2d.plot_grid(
-                grid=self.interferometer.visibilities.in_grid,
+                grid=self.dataset.visibilities.in_grid,
                 visuals_2d=self.visuals_2d,
-                color_array=self.interferometer.noise_map.real,
+                color_array=self.dataset.noise_map.real,
                 auto_labels=AutoLabels(title="Noise-Map", filename="noise_map"),
             )
 
         if u_wavelengths:
-
             self.mat_plot_1d.plot_yx(
-                y=self.interferometer.uv_wavelengths[:, 0],
+                y=self.dataset.uv_wavelengths[:, 0],
                 x=None,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
                     title="U-Wavelengths",
                     filename="u_wavelengths",
                     ylabel="Wavelengths",
                 ),
                 plot_axis_type_override="linear",
             )
 
         if v_wavelengths:
-
             self.mat_plot_1d.plot_yx(
-                y=self.interferometer.uv_wavelengths[:, 1],
+                y=self.dataset.uv_wavelengths[:, 1],
                 x=None,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
                     title="V-Wavelengths",
                     filename="v_wavelengths",
                     ylabel="Wavelengths",
                 ),
                 plot_axis_type_override="linear",
             )
 
         if uv_wavelengths:
-
             self.mat_plot_2d.plot_grid(
                 grid=Grid2DIrregular.from_yx_1d(
-                    y=self.interferometer.uv_wavelengths[:, 1] / 10**3.0,
-                    x=self.interferometer.uv_wavelengths[:, 0] / 10**3.0,
+                    y=self.dataset.uv_wavelengths[:, 1] / 10**3.0,
+                    x=self.dataset.uv_wavelengths[:, 0] / 10**3.0,
                 ),
                 visuals_2d=self.visuals_2d,
                 auto_labels=AutoLabels(
                     title="UV-Wavelengths", filename="uv_wavelengths"
                 ),
             )
 
         if amplitudes_vs_uv_distances:
-
             self.mat_plot_1d.plot_yx(
-                y=self.interferometer.amplitudes,
-                x=self.interferometer.uv_distances / 10**3.0,
+                y=self.dataset.amplitudes,
+                x=self.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
                     title="Amplitudes vs UV-distances",
                     filename="amplitudes_vs_uv_distances",
-                    ylabel="amplitude (Jy)",
-                    xlabel="U-Wavelengths ($\lambda$)",
+                    yunit="Jy",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
 
         if phases_vs_uv_distances:
-
             self.mat_plot_1d.plot_yx(
-                y=self.interferometer.phases,
-                x=self.interferometer.uv_distances / 10**3.0,
+                y=self.dataset.phases,
+                x=self.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
                     title="Phases vs UV-distances",
                     filename="phases_vs_uv_distances",
-                    ylabel="phase (deg)",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    yunit="deg",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
 
         if dirty_image:
-
             self.mat_plot_2d.plot_array(
-                array=self.interferometer.dirty_image,
+                array=self.dataset.dirty_image,
                 visuals_2d=self.get_visuals_2d_real_space(),
-                auto_labels=AutoLabels(title="Dirty Image", filename="dirty_image_2d"),
+                auto_labels=AutoLabels(title="Dirty Image", filename="dirty_image"),
             )
 
         if dirty_noise_map:
-
             self.mat_plot_2d.plot_array(
-                array=self.interferometer.dirty_noise_map,
+                array=self.dataset.dirty_noise_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
-                    title="Dirty Noise Map", filename="dirty_noise_map_2d"
+                    title="Dirty Noise Map", filename="dirty_noise_map"
                 ),
             )
 
         if dirty_signal_to_noise_map:
-
             self.mat_plot_2d.plot_array(
-                array=self.interferometer.dirty_signal_to_noise_map,
+                array=self.dataset.dirty_signal_to_noise_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
                     title="Dirty Signal-To-Noise Map",
-                    filename="dirty_signal_to_noise_map_2d",
-                ),
-            )
-
-        if dirty_inverse_noise_map:
-
-            self.mat_plot_2d.plot_array(
-                array=self.interferometer.dirty_inverse_noise_map,
-                visuals_2d=self.get_visuals_2d_real_space(),
-                auto_labels=AutoLabels(
-                    title="Dirty Inverse Noise Map",
-                    filename="dirty_inverse_noise_map_2d",
+                    filename="dirty_signal_to_noise_map",
                 ),
             )
 
     def subplot(
         self,
-        visibilities: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         u_wavelengths: bool = False,
         v_wavelengths: bool = False,
         uv_wavelengths: bool = False,
         amplitudes_vs_uv_distances: bool = False,
         phases_vs_uv_distances: bool = False,
         dirty_image: bool = False,
         dirty_noise_map: bool = False,
         dirty_signal_to_noise_map: bool = False,
-        dirty_inverse_noise_map: bool = False,
-        auto_filename: str = "subplot_interferometer",
+        auto_filename: str = "subplot_dataset",
     ):
         """
         Plots the individual attributes of the plotter's `Interferometer` object in 1D and 2D on a subplot.
 
         The API is such that every plottable attribute of the `Interferometer` object is an input parameter of type
         bool of the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
-        visibilities
-            Whether or not to include a 2D plot (via `scatter`) of the visibility data.
+        data
+            Whether to include a 2D plot (via `scatter`) of the visibility data.
         noise_map
-            Whether or not to include a 2D plot (via `scatter`) of the noise-map.
+            Whether to include a 2D plot (via `scatter`) of the noise-map.
         u_wavelengths
-            Whether or not to include a 1D plot (via `plot`) of the u-wavelengths.
+            Whether to include a 1D plot (via `plot`) of the u-wavelengths.
         v_wavelengths
-            Whether or not to include a 1D plot (via `plot`) of the v-wavelengths.
+            Whether to include a 1D plot (via `plot`) of the v-wavelengths.
         amplitudes_vs_uv_distances
-            Whether or not to include a 1D plot (via `plot`) of the amplitudes versis the uv distances.
+            Whether to include a 1D plot (via `plot`) of the amplitudes versis the uv distances.
         phases_vs_uv_distances
-            Whether or not to include a 1D plot (via `plot`) of the phases versis the uv distances.
+            Whether to include a 1D plot (via `plot`) of the phases versis the uv distances.
         dirty_image
-            Whether or not to include a 2D plot (via `imshow`) of the dirty image.
+            Whether to include a 2D plot (via `imshow`) of the dirty image.
         dirty_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the dirty noise map.
+            Whether to include a 2D plot (via `imshow`) of the dirty noise map.
         dirty_signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the dirty signal-to-noise map.
-        dirty_inverse_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the dirty inverse noise map.
+            Whether to include a 2D plot (via `imshow`) of the dirty signal-to-noise map.
         """
         self._subplot_custom_plot(
-            visibilities=visibilities,
+            data=data,
             noise_map=noise_map,
             u_wavelengths=u_wavelengths,
             v_wavelengths=v_wavelengths,
             uv_wavelengths=uv_wavelengths,
             amplitudes_vs_uv_distances=amplitudes_vs_uv_distances,
             phases_vs_uv_distances=phases_vs_uv_distances,
             dirty_image=dirty_image,
             dirty_noise_map=dirty_noise_map,
             dirty_signal_to_noise_map=dirty_signal_to_noise_map,
-            dirty_inverse_noise_map=dirty_inverse_noise_map,
             auto_labels=AutoLabels(filename=auto_filename),
         )
 
-    def subplot_interferometer(self):
+    def subplot_dataset(self):
         """
         Standard subplot of the attributes of the plotter's `Interferometer` object.
         """
         return self.subplot(
-            visibilities=True,
+            data=True,
             uv_wavelengths=True,
             amplitudes_vs_uv_distances=True,
             phases_vs_uv_distances=True,
-            auto_filename="subplot_interferometer",
+            auto_filename="subplot_dataset",
         )
 
     def subplot_dirty_images(self):
         """
         Standard subplot of the dirty attributes of the plotter's `Interferometer` object.
         """
         return self.subplot(
             dirty_image=True,
             dirty_noise_map=True,
             dirty_signal_to_noise_map=True,
-            dirty_inverse_noise_map=True,
             auto_filename="subplot_dirty_images",
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/dataset/preprocess.py` & `autoarray-2023.7.7.1/autoarray/dataset/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
     gain
         The gain of the instrument used in the conversion to / from counts and ADUs.
     """
     return np.divide(gain * array_adus, exposure_time_map)
 
 
 def array_counts_to_counts_per_second(array_counts, exposure_time):
-
     if exposure_time is None:
         raise exc.ArrayException(
             "Cannot convert a Frame2D to units counts per second without an exposure time attribute (exposure_time = None)."
         )
 
     return array_counts / exposure_time
 
@@ -465,30 +464,29 @@
 def data_with_gaussian_noise_added(data, sigma, seed=-1):
     return data + gaussian_noise_via_shape_and_sigma_from(
         shape=data.shape, sigma=sigma, seed=seed
     )
 
 
 def data_with_complex_gaussian_noise_added(data, sigma, seed=-1):
-
     gaussian_noise = gaussian_noise_via_shape_and_sigma_from(
         shape=(data.shape[0], 2), sigma=sigma, seed=seed
     )
 
     return data + gaussian_noise[:, 0] + 1.0j * gaussian_noise[:, 1]
 
 
 def noise_map_with_signal_to_noise_limit_from(
     data, noise_map, signal_to_noise_limit, noise_limit_mask=None
 ):
     """
     Given data and its noise map, increase the noise-values of all data points which signal to noise is above an input
     `signal_to_noise_limit`, such that the signal to noise values do not exceed this limit.
 
-    This may be performed for imaging data with extremely high signal-to-noise regions in the data which are poorly
+    This may be performed for dataset data with extremely high signal-to-noise regions in the data which are poorly
     fit my the model. By downweighting their signal to noise values, the model-fit with focus on other parts of the
     data with low S/N.
 
     A `noise_limit_mask` can be input, such that only noise values corresponding to `False` entries are scaled to the
     capped value.
 
     Parameters
@@ -535,15 +533,14 @@
         return Array1D(values=noise_map_limit, mask=mask)
     return Array2D(noise_map_limit, mask=mask)
 
 
 def visibilities_noise_map_with_signal_to_noise_limit_from(
     data, noise_map, signal_to_noise_limit
 ):
-
     from autoarray.structures.visibilities import VisibilitiesNoiseMap
 
     # TODO : Refacotr into a util
 
     signal_to_noise_map_real = np.divide(np.real(data), np.real(noise_map))
     signal_to_noise_map_real[signal_to_noise_map_real < 0] = 0.0
     signal_to_noise_map_imag = np.divide(np.imag(data), np.imag(noise_map))
```

### Comparing `autoarray-2023.3.27.1/autoarray/exc.py` & `autoarray-2023.7.7.1/autoarray/exc.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/fit/fit_dataset.py` & `autoarray-2023.7.7.1/autoarray/fit/fit_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,14 @@
         warnings.filterwarnings("ignore")
 
         signal_to_noise_map = np.divide(self.data, self.noise_map)
         signal_to_noise_map[signal_to_noise_map < 0] = 0
         return signal_to_noise_map
 
     @property
-    def potential_chi_squared_map(self) -> ty.DataLike:
-        """
-        The signal-to-noise_map of the dataset and noise-map which are fitted.
-        """
-        warnings.filterwarnings("ignore")
-        absolute_signal_to_noise_map = np.divide(np.abs(self.data), self.noise_map)
-        return np.square(absolute_signal_to_noise_map)
-
-    @property
     def residual_map(self) -> Structure:
         """
         Returns the residual-map between the masked dataset and model data, where:
 
         Residuals = (Data - Model_Data).
         """
         return fit_util.residual_map_from(data=self.data, model_data=self.model_data)
@@ -127,15 +118,14 @@
 
     @property
     def model_data(self) -> ty.DataLike:
         return self._model_data
 
 
 class FitDataset(AbstractFitInversion):
-
     # noinspection PyUnresolvedReferences
     def __init__(
         self,
         dataset: AbstractDataset,
         use_mask_in_fit: bool = False,
         profiling_dict: Optional[Dict] = None,
     ):
@@ -236,15 +226,14 @@
         Returns the chi-squared terms of the model data's fit to an dataset, by summing the chi-squared-map.
 
         If the dataset includes a noise covariance matrix, this is used instead to account for covariance in the
         goodness-of-fit.
         """
 
         if self.dataset.noise_covariance_matrix is not None:
-
             return fit_util.chi_squared_with_noise_covariance_from(
                 residual_map=self.residual_map,
                 noise_covariance_matrix_inv=self.dataset.noise_covariance_matrix_inv,
             )
 
         if self.use_mask_in_fit:
             return fit_util.chi_squared_with_mask_from(
@@ -300,27 +289,25 @@
             The log of the determinant of the sum of the curvature and regularization matrices.
         log_regularization_term
             The log of the determinant o the regularization matrix.
         noise_normalization
             The normalization noise_map-term for the data's noise-map.
         """
         if self.inversion is not None:
-
             return fit_util.log_evidence_from(
                 chi_squared=self.chi_squared,
                 regularization_term=self.inversion.regularization_term,
                 log_curvature_regularization_term=self.inversion.log_det_curvature_reg_matrix_term,
                 log_regularization_term=self.inversion.log_det_regularization_matrix_term,
                 noise_normalization=self.noise_normalization,
             )
 
     @property
     @profile_func
     def figure_of_merit(self) -> float:
-
         if self.inversion is not None:
             return self.log_evidence
 
         return self.log_likelihood
 
     @property
     def inversion(self) -> Optional[AbstractInversion]:
```

### Comparing `autoarray-2023.3.27.1/autoarray/fit/fit_imaging.py` & `autoarray-2023.7.7.1/autoarray/fit/fit_imaging.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,12 +62,12 @@
 
     @property
     def model_image(self) -> Array2D:
         return self.model_data
 
     @property
     def mask(self) -> Mask2D:
-        return self.imaging.mask
+        return self.dataset.mask
 
     @property
     def blurred_image(self) -> Array2D:
         raise NotImplementedError
```

### Comparing `autoarray-2023.3.27.1/autoarray/fit/fit_interferometer.py` & `autoarray-2023.7.7.1/autoarray/fit/fit_interferometer.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ):
         """Class to fit a masked interferometer dataset.
 
         Parameters
         ----------
         dataset : MaskedInterferometer
             The masked interferometer dataset that is fitted.
-        model_visibilities : Visibilities
+        model_data : Visibilities
             The model visibilities the masked imaging is fitted with.
         inversion : Inversion
             If the fit uses an `Inversion` this is the instance of the object used to perform the fit. This determines
             if the `log_likelihood` or `log_evidence` is used as the `figure_of_merit`.
         use_mask_in_fit
             If `True`, masked data points are omitted from the fit. If `False` they are not (in most use cases the
             `dataset` will have been processed to remove masked points, for example the `slim` representation).
@@ -53,23 +53,23 @@
             dataset=dataset,
             use_mask_in_fit=use_mask_in_fit,
             profiling_dict=profiling_dict,
         )
 
     @property
     def mask(self) -> np.ndarray:
-        return np.full(shape=self.visibilities.shape, fill_value=False)
+        return np.full(shape=self.data.shape, fill_value=False)
 
     @property
     def interferometer(self) -> Interferometer:
         return self.dataset
 
     @property
     def transformer(self) -> ty.Transformer:
-        return self.interferometer.transformer
+        return self.dataset.transformer
 
     @property
     def visibilities(self) -> Visibilities:
         return self.data
 
     @property
     def model_visibilities(self) -> Visibilities:
@@ -108,19 +108,14 @@
             np.imag(self.data), np.imag(self.noise_map)
         )
         signal_to_noise_map_imag[signal_to_noise_map_imag < 0] = 0.0
 
         return signal_to_noise_map_real + 1.0j * signal_to_noise_map_imag
 
     @property
-    def potential_chi_squared_map(self) -> np.ndarray:
-        """The signal-to-noise_map of the dataset and noise-map which are fitted."""
-        return self.signal_to_noise_map
-
-    @property
     def chi_squared(self) -> float:
         """
         Returns the chi-squared terms of the model data's fit to an dataset, by summing the chi-squared-map.
         """
         return fit_util.chi_squared_complex_with_mask_from(
             chi_squared_map=self.chi_squared_map, mask=self.mask
         )
@@ -134,27 +129,27 @@
         """
         return fit_util.noise_normalization_complex_with_mask_from(
             noise_map=self.noise_map, mask=self.mask
         )
 
     @property
     def dirty_image(self) -> Array2D:
-        return self.transformer.image_from(visibilities=self.visibilities)
+        return self.transformer.image_from(visibilities=self.data)
 
     @property
     def dirty_noise_map(self) -> Array2D:
         return self.transformer.image_from(visibilities=self.noise_map)
 
     @property
     def dirty_signal_to_noise_map(self) -> Array2D:
         return self.transformer.image_from(visibilities=self.signal_to_noise_map)
 
     @property
     def dirty_model_image(self) -> Array2D:
-        return self.transformer.image_from(visibilities=self.model_visibilities)
+        return self.transformer.image_from(visibilities=self.model_data)
 
     @property
     def dirty_residual_map(self) -> Array2D:
         return self.transformer.image_from(visibilities=self.residual_map)
 
     @property
     def dirty_normalized_residual_map(self) -> Array2D:
```

### Comparing `autoarray-2023.3.27.1/autoarray/fit/fit_util.py` & `autoarray-2023.7.7.1/autoarray/fit/fit_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/fit/mock/mock_fit_imaging.py` & `autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         use_mask_in_fit: bool = False,
         noise_map=None,
         model_data=None,
         inversion=None,
         blurred_image=None,
         profiling_dict: Optional[Dict] = None,
     ):
-
         super().__init__(
             dataset=dataset,
             use_mask_in_fit=use_mask_in_fit,
             profiling_dict=profiling_dict,
         )
 
         self._noise_map = noise_map
```

### Comparing `autoarray-2023.3.27.1/autoarray/fit/mock/mock_fit_interferometer.py` & `autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_interferometer.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
         self,
         dataset=MockDataset(),
         use_mask_in_fit: bool = False,
         model_data=None,
         inversion=None,
         noise_map=None,
     ):
-
         super().__init__(dataset=dataset, use_mask_in_fit=use_mask_in_fit)
 
         self._model_data = model_data
         self._inversion = inversion
         self._noise_map = noise_map
 
     @property
```

### Comparing `autoarray-2023.3.27.1/autoarray/fit/plot/fit_imaging_plotters.py` & `autoarray-2023.7.7.1/autoarray/fit/plot/fit_vector_yx_plotters.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from autoarray.plot.abstract_plotters import Plotter
 from autoarray.plot.visuals.two_d import Visuals2D
 from autoarray.plot.include.two_d import Include2D
 from autoarray.plot.mat_plot.two_d import MatPlot2D
 from autoarray.plot.auto_labels import AutoLabels
 from autoarray.fit.fit_imaging import FitImaging
+from autoarray.fit.plot.fit_imaging_plotters import FitImagingPlotterMeta
 
 
-class FitImagingPlotterMeta(Plotter):
+class FitVectorYXPlotterMeta(Plotter):
     def __init__(
         self,
         fit,
         get_visuals_2d: Callable,
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
-        residuals_symmetric_cmap: bool = True,
     ):
         """
         Plots the attributes of `FitImaging` objects using the matplotlib method `imshow()` and many other matplotlib
         functions which customize the plot's appearance.
 
         The `mat_plot_2d` attribute wraps matplotlib function calls to make the figure. By default, the settings
         passed to every matplotlib function called are those specified in the `config/visualize/mat_wrap/*.ini` files,
@@ -38,188 +38,163 @@
             A function which extracts from the `FitImaging` the 2D visuals which are plotted on figures.
         mat_plot_2d
             Contains objects which wrap the matplotlib function calls that make the plot.
         visuals_2d
             Contains visuals that can be overlaid on the plot.
         include_2d
             Specifies which attributes of the `Array2D` are extracted and plotted as visuals.
-        residuals_symmetric_cmap
-            If true, the `residual_map` and `normalized_residual_map` are plotted with a symmetric color map such
-            that `abs(vmin) = abs(vmax)`.
         """
         super().__init__(
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
         self.fit = fit
         self.get_visuals_2d = get_visuals_2d
-        self.residuals_symmetric_cmap = residuals_symmetric_cmap
 
     def figures_2d(
         self,
         image: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         model_image: bool = False,
         residual_map: bool = False,
         normalized_residual_map: bool = False,
         chi_squared_map: bool = False,
-        suffix: str = "",
     ):
         """
         Plots the individual attributes of the plotter's `FitImaging` object in 2D.
 
         The API is such that every plottable attribute of the `FitImaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
         image
             Whether to make a 2D plot (via `imshow`) of the image data.
         noise_map
             Whether to make a 2D plot (via `imshow`) of the noise map.
+        psf
+            Whether to make a 2D plot (via `imshow`) of the psf.
         signal_to_noise_map
             Whether to make a 2D plot (via `imshow`) of the signal-to-noise map.
-        model_image
-            Whether to make a 2D plot (via `imshow`) of the model image.
         residual_map
             Whether to make a 2D plot (via `imshow`) of the residual map.
         normalized_residual_map
             Whether to make a 2D plot (via `imshow`) of the normalized residual map.
         chi_squared_map
             Whether to make a 2D plot (via `imshow`) of the chi-squared map.
         """
 
-        if image:
+        fit_plotter_y = FitImaging(self.fit.data.y_array)
 
+        if image:
             self.mat_plot_2d.plot_array(
                 array=self.fit.data,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(title="Image", filename=f"image_2d{suffix}"),
+                auto_labels=AutoLabels(title="Image", filename="image_2d"),
             )
 
         if noise_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.noise_map,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(
-                    title="Noise-Map", filename=f"noise_map{suffix}"
-                ),
+                auto_labels=AutoLabels(title="Noise-Map", filename="noise_map"),
             )
 
         if signal_to_noise_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.signal_to_noise_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Signal-To-Noise Map", filename=f"signal_to_noise_map{suffix}"
+                    title="Signal-To-Noise Map", filename="signal_to_noise_map"
                 ),
             )
 
         if model_image:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.model_data,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(
-                    title="Model Image", filename=f"model_image{suffix}"
-                ),
+                auto_labels=AutoLabels(title="Model Image", filename="model_image"),
             )
 
-        cmap_original = self.mat_plot_2d.cmap
-
-        if self.residuals_symmetric_cmap:
-
-            self.mat_plot_2d.cmap = self.mat_plot_2d.cmap.symmetric
-
         if residual_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.residual_map,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(
-                    title="Residual Map", filename=f"residual_map{suffix}"
-                ),
+                auto_labels=AutoLabels(title="Residual Map", filename="residual_map"),
             )
 
         if normalized_residual_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.normalized_residual_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Normalized Residual Map",
-                    filename=f"normalized_residual_map{suffix}",
+                    title="Normalized Residual Map", filename="normalized_residual_map"
                 ),
             )
 
-        self.mat_plot_2d.cmap = cmap_original
-
         if chi_squared_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.chi_squared_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title="Chi-Squared Map", filename=f"chi_squared_map{suffix}"
+                    title="Chi-Squared Map", filename="chi_squared_map"
                 ),
             )
 
     def subplot(
         self,
         image: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         model_image: bool = False,
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
         image
-            Whether or not to include a 2D plot (via `imshow`) of the image data.
+            Whether to include a 2D plot (via `imshow`) of the image data.
         noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the noise map.
+            Whether to include a 2D plot (via `imshow`) of the noise map.
         psf
-            Whether or not to include a 2D plot (via `imshow`) of the psf.
+            Whether to include a 2D plot (via `imshow`) of the psf.
         signal_to_noise_map
-            Whether or not to include a 2D plot (via `imshow`) of the signal-to-noise map.
+            Whether to include a 2D plot (via `imshow`) of the signal-to-noise map.
         model_image
-            Whether or not to include a 2D plot (via `imshow`) of the model image.
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
             image=image,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
             model_image=model_image,
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
         return self.subplot(
             image=True,
             signal_to_noise_map=True,
             model_image=True,
@@ -272,11 +247,11 @@
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
         )
 
         self.figures_2d = self._fit_imaging_meta_plotter.figures_2d
         self.subplot = self._fit_imaging_meta_plotter.subplot
-        self.subplot_fit_imaging = self._fit_imaging_meta_plotter.subplot_fit_imaging
+        self.subplot_fit = self._fit_imaging_meta_plotter.subplot_fit
 
     def get_visuals_2d(self) -> Visuals2D:
         return self.get_2d.via_fit_imaging_from(fit=self.fit)
```

### Comparing `autoarray-2023.3.27.1/autoarray/fit/plot/fit_interferometer_plotters.py` & `autoarray-2023.7.7.1/autoarray/fit/plot/fit_interferometer_plotters.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,18 +71,19 @@
 
         self.fit = fit
         self.get_visuals_2d_real_space = get_visuals_2d_real_space
         self.residuals_symmetric_cmap = residuals_symmetric_cmap
 
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
         dirty_image: bool = False,
@@ -97,21 +98,21 @@
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
@@ -131,249 +132,250 @@
             Whether to make a 2D plot (via `imshow`) of the dirty residual map.
         dirty_normalized_residual_map
             Whether to make a 2D plot (via `imshow`) of the dirty normalized residual map.
         dirty_chi_squared_map
             Whether to make a 2D plot (via `imshow`) of the dirty chi-squared map.
         """
 
-        if visibilities:
+        if data:
             self.mat_plot_2d.plot_grid(
-                grid=self.fit.visibilities.in_grid,
+                grid=self.fit.data.in_grid,
                 visuals_2d=self.visuals_2d,
-                auto_labels=AutoLabels(title="Visibilities", filename="visibilities"),
+                auto_labels=AutoLabels(title="Visibilities", filename="data"),
                 color_array=np.real(self.fit.noise_map),
             )
 
         if noise_map:
             self.mat_plot_2d.plot_grid(
-                grid=self.fit.visibilities.in_grid,
+                grid=self.fit.data.in_grid,
                 visuals_2d=self.visuals_2d,
                 auto_labels=AutoLabels(title="Noise-Map", filename="noise_map"),
                 color_array=np.real(self.fit.noise_map),
             )
 
         if signal_to_noise_map:
             self.mat_plot_2d.plot_grid(
-                grid=self.fit.visibilities.in_grid,
+                grid=self.fit.data.in_grid,
                 visuals_2d=self.visuals_2d,
                 auto_labels=AutoLabels(
                     title="Signal-To-Noise Map", filename="signal_to_noise_map"
                 ),
                 color_array=np.real(self.fit.signal_to_noise_map),
             )
 
-        if model_visibilities:
+        if amplitudes_vs_uv_distances:
+            self.mat_plot_1d.plot_yx(
+                y=self.fit.dataset.amplitudes,
+                x=self.fit.dataset.uv_distances / 10**3.0,
+                visuals_1d=self.visuals_1d,
+                auto_labels=AutoLabels(
+                    title="Amplitudes vs UV-distances",
+                    filename="amplitudes_vs_uv_distances",
+                    yunit="Jy",
+                    xunit="k$\lambda$",
+                ),
+                plot_axis_type_override="scatter",
+            )
+
+        if model_data:
             self.mat_plot_2d.plot_grid(
-                grid=self.fit.visibilities.in_grid,
+                grid=self.fit.data.in_grid,
                 visuals_2d=self.visuals_2d,
                 auto_labels=AutoLabels(
-                    title="Model Visibilities", filename="model_visibilities"
+                    title="Model Visibilities", filename="model_data"
                 ),
                 color_array=np.real(self.fit.model_data),
             )
 
         if residual_map_real:
             self.mat_plot_1d.plot_yx(
                 y=np.real(self.fit.residual_map),
-                x=self.fit.interferometer.uv_distances / 10**3.0,
+                x=self.fit.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title="Residual Map vs UV-Distance (real)",
+                    title="Residual vs UV-Distance (real)",
                     filename="real_residual_map_vs_uv_distances",
-                    ylabel="V$_{R,data}$ - V$_{R,model}$",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
         if residual_map_imag:
             self.mat_plot_1d.plot_yx(
                 y=np.imag(self.fit.residual_map),
-                x=self.fit.interferometer.uv_distances / 10**3.0,
+                x=self.fit.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title="Residual Map vs UV-Distance (imag)",
+                    title="Residual vs UV-Distance (imag)",
                     filename="imag_residual_map_vs_uv_distances",
-                    ylabel="V$_{R,data}$ - V$_{R,model}$",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
 
         if normalized_residual_map_real:
-
             self.mat_plot_1d.plot_yx(
                 y=np.real(self.fit.residual_map),
-                x=self.fit.interferometer.uv_distances / 10**3.0,
+                x=self.fit.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title="Normalized Residual Map vs UV-Distance (real)",
+                    title="Norm Residual vs UV-Distance (real)",
                     filename="real_normalized_residual_map_vs_uv_distances",
-                    ylabel="V$_{R,data}$ - V$_{R,model}$",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    yunit="$\sigma$",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
         if normalized_residual_map_imag:
             self.mat_plot_1d.plot_yx(
                 y=np.imag(self.fit.residual_map),
-                x=self.fit.interferometer.uv_distances / 10**3.0,
+                x=self.fit.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title="Normalized Residual Map vs UV-Distance (imag)",
+                    title="Norm Residual vs UV-Distance (imag)",
                     filename="imag_normalized_residual_map_vs_uv_distances",
-                    ylabel="V$_{R,data}$ - V$_{R,model}$",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    yunit="$\sigma$",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
 
         if chi_squared_map_real:
-
             self.mat_plot_1d.plot_yx(
                 y=np.real(self.fit.residual_map),
-                x=self.fit.interferometer.uv_distances / 10**3.0,
+                x=self.fit.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title="Chi-Squared Map vs UV-Distance (real)",
+                    title="Chi-Squared vs UV-Distance (real)",
                     filename="real_chi_squared_map_vs_uv_distances",
-                    ylabel="V$_{R,data}$ - V$_{R,model}$",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    yunit="$\chi^2$",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
         if chi_squared_map_imag:
             self.mat_plot_1d.plot_yx(
                 y=np.imag(self.fit.residual_map),
-                x=self.fit.interferometer.uv_distances / 10**3.0,
+                x=self.fit.dataset.uv_distances / 10**3.0,
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
-                    title="Chi-Squared Map vs UV-Distance (imag)",
+                    title="Chi-Squared vs UV-Distance (imag)",
                     filename="imag_chi_squared_map_vs_uv_distances",
-                    ylabel="V$_{R,data}$ - V$_{R,model}$",
-                    xlabel=r"UV$_{distance}$ (k$\lambda$)",
+                    yunit="$\chi^2$",
+                    xunit="k$\lambda$",
                 ),
                 plot_axis_type_override="scatter",
             )
 
         if dirty_image:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_image,
                 visuals_2d=self.get_visuals_2d_real_space(),
-                auto_labels=AutoLabels(title="Dirty Image", filename="dirty_image_2d"),
+                auto_labels=AutoLabels(title="Dirty Image", filename="dirty_image"),
             )
 
         if dirty_noise_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_noise_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
-                    title="Dirty Noise Map", filename="dirty_noise_map_2d"
+                    title="Dirty Noise Map", filename="dirty_noise_map"
                 ),
             )
 
         if dirty_signal_to_noise_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_signal_to_noise_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
                     title="Dirty Signal-To-Noise Map",
-                    filename="dirty_signal_to_noise_map_2d",
+                    filename="dirty_signal_to_noise_map",
                 ),
             )
 
         if dirty_model_image:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_model_image,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
                     title="Dirty Model Image", filename="dirty_model_image_2d"
                 ),
             )
 
         cmap_original = self.mat_plot_2d.cmap
 
         if self.residuals_symmetric_cmap:
-
             self.mat_plot_2d.cmap = self.mat_plot_2d.cmap.symmetric
 
         if dirty_residual_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_residual_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
                     title="Dirty Residual Map", filename="dirty_residual_map_2d"
                 ),
             )
 
         if dirty_normalized_residual_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_normalized_residual_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
                     title="Dirty Normalized Residual Map",
                     filename="dirty_normalized_residual_map_2d",
                 ),
             )
 
         if self.residuals_symmetric_cmap:
-
             self.mat_plot_2d.cmap = cmap_original
 
         if dirty_chi_squared_map:
-
             self.mat_plot_2d.plot_array(
                 array=self.fit.dirty_chi_squared_map,
                 visuals_2d=self.get_visuals_2d_real_space(),
                 auto_labels=AutoLabels(
                     title="Dirty Chi-Squared Map", filename="dirty_chi_squared_map_2d"
                 ),
             )
 
     def subplot(
         self,
-        visibilities: bool = False,
+        data: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
-        model_visibilities: bool = False,
+        model_data: bool = False,
         residual_map_real: bool = False,
         residual_map_imag: bool = False,
         normalized_residual_map_real: bool = False,
         normalized_residual_map_imag: bool = False,
         chi_squared_map_real: bool = False,
         chi_squared_map_imag: bool = False,
         dirty_image: bool = False,
         dirty_noise_map: bool = False,
         dirty_signal_to_noise_map: bool = False,
         dirty_model_image: bool = False,
         dirty_residual_map: bool = False,
         dirty_normalized_residual_map: bool = False,
         dirty_chi_squared_map: bool = False,
-        auto_filename: str = "subplot_fit_interferometer",
+        auto_filename: str = "subplot_fit",
     ):
         """
         Plots the individual attributes of the plotter's `FitInterferometer` object in 1D and 2D on a subplot.
 
         The API is such that every plottable attribute of the `Interferometer` object is an input parameter of type
         bool of the function, which if switched to `True` means that it is included on the subplot.
 
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
@@ -396,18 +398,18 @@
         dirty_chi_squared_map
             Whether to make a 2D plot (via `imshow`) of the dirty chi-squared map.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
 
         self._subplot_custom_plot(
-            visibilities=visibilities,
+            visibilities=data,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
-            model_visibilities=model_visibilities,
+            model_data=model_data,
             residual_map_real=residual_map_real,
             residual_map_imag=residual_map_imag,
             normalized_residual_map_real=normalized_residual_map_real,
             normalized_residual_map_imag=normalized_residual_map_imag,
             chi_squared_map_real=chi_squared_map_real,
             chi_squared_map_imag=chi_squared_map_imag,
             dirty_image=dirty_image,
@@ -416,26 +418,26 @@
             dirty_model_image=dirty_model_image,
             dirty_residual_map=dirty_residual_map,
             dirty_normalized_residual_map=dirty_normalized_residual_map,
             dirty_chi_squared_map=dirty_chi_squared_map,
             auto_labels=AutoLabels(filename=auto_filename),
         )
 
-    def subplot_fit_interferometer(self):
+    def subplot_fit(self):
         """
         Standard subplot of the attributes of the plotter's `FitInterferometer` object.
         """
         return self.subplot(
             residual_map_real=True,
             normalized_residual_map_real=True,
             chi_squared_map_real=True,
             residual_map_imag=True,
             normalized_residual_map_imag=True,
             chi_squared_map_imag=True,
-            auto_filename="subplot_fit_interferometer",
+            auto_filename="subplot_fit",
         )
 
     def subplot_fit_dirty_images(self):
         """
         Standard subplot of the dirty attributes of the plotter's `FitInterferometer` object.
         """
         return self.subplot(
@@ -503,16 +505,14 @@
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
         )
 
         self.figures_2d = self._fit_interferometer_meta_plotter.figures_2d
         self.subplot = self._fit_interferometer_meta_plotter.subplot
-        self.subplot_fit_interferometer = (
-            self._fit_interferometer_meta_plotter.subplot_fit_interferometer
-        )
+        self.subplot_fit = self._fit_interferometer_meta_plotter.subplot_fit
         self.subplot_fit_dirty_images = (
             self._fit_interferometer_meta_plotter.subplot_fit_dirty_images
         )
 
     def get_visuals_2d_real_space(self) -> Visuals2D:
-        return self.get_2d.via_mask_from(mask=self.fit.interferometer.real_space_mask)
+        return self.get_2d.via_mask_from(mask=self.fit.dataset.real_space_mask)
```

### Comparing `autoarray-2023.3.27.1/autoarray/fixtures.py` & `autoarray-2023.7.7.1/autoarray/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import numpy as np
 
 import autoarray as aa
 
 
 def make_mask_1d_7():
-
     mask = np.array([True, True, False, False, False, True, True])
 
     return aa.Mask1D(mask=mask, pixel_scales=(1.0,), sub_size=1)
 
 
 def make_sub_mask_1d_7():
-
     mask = np.array([True, True, False, False, False, True, True])
 
     return aa.Mask1D(mask=mask, pixel_scales=(1.0,), sub_size=2)
 
 
 def make_mask_2d_7x7():
-
     mask = np.array(
         [
             [True, True, True, True, True, True, True],
             [True, True, True, True, True, True, True],
             [True, True, False, False, False, True, True],
             [True, True, False, False, False, True, True],
             [True, True, False, False, False, True, True],
@@ -149,30 +146,28 @@
 
 
 def make_image_7x7():
     return aa.Array2D.ones(shape_native=(7, 7), pixel_scales=(1.0, 1.0))
 
 
 def make_psf_3x3():
-
     psf = np.array([[0.0, 0.5, 0.0], [0.5, 1.0, 0.5], [0.0, 0.5, 0.0]])
 
     return aa.Kernel2D.no_mask(values=psf, pixel_scales=(1.0, 1.0))
 
 
 def make_psf_3x3_no_blur():
     return aa.Kernel2D.no_blur(pixel_scales=(1.0, 1.0))
 
 
 def make_noise_map_7x7():
     return aa.Array2D.full(fill_value=2.0, shape_native=(7, 7), pixel_scales=(1.0, 1.0))
 
 
 def make_noise_covariance_matrix_7x7():
-
     noise_covariance_matrix_7x7 = np.eye(N=49, M=49)
 
     noise_covariance_matrix_7x7[:, 24] = 1.0
     noise_covariance_matrix_7x7[24, :] = 1.0
 
     return noise_covariance_matrix_7x7
 
@@ -186,31 +181,31 @@
         aa.Grid2DIrregular(values=[(0.1, 0.1), (0.2, 0.2)]),
         aa.Grid2DIrregular(values=[(0.3, 0.3)]),
     ]
 
 
 def make_imaging_7x7():
     return aa.Imaging(
-        image=make_image_7x7(),
+        data=make_image_7x7(),
         psf=make_psf_3x3(),
         noise_map=make_noise_map_7x7(),
     )
 
 
 def make_imaging_covariance_7x7():
     return aa.Imaging(
-        image=make_image_7x7(),
+        data=make_image_7x7(),
         psf=make_psf_3x3(),
         noise_covariance_matrix=make_noise_covariance_matrix_7x7(),
     )
 
 
 def make_imaging_7x7_no_blur():
     return aa.Imaging(
-        image=make_image_7x7(),
+        data=make_image_7x7(),
         psf=make_psf_3x3_no_blur(),
         noise_map=make_noise_map_7x7(),
     )
 
 
 def make_visibilities_7():
     return aa.Visibilities.full(shape_slim=(7,), fill_value=1.0)
@@ -236,52 +231,51 @@
 
 def make_uv_wavelengths_7x2_no_fft():
     return np.ones(shape=(7, 2))
 
 
 def make_interferometer_7():
     return aa.Interferometer(
-        visibilities=make_visibilities_7(),
+        data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2(),
         real_space_mask=make_sub_mask_2d_7x7(),
         settings=aa.SettingsInterferometer(
             grid_class=aa.Grid2D, sub_size=1, transformer_class=aa.TransformerDFT
         ),
     )
 
 
 def make_interferometer_7_no_fft():
     return aa.Interferometer(
-        visibilities=make_visibilities_7(),
+        data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2_no_fft(),
         real_space_mask=make_sub_mask_2d_7x7(),
         settings=aa.SettingsInterferometer(
             grid_class=aa.Grid2D, sub_size=1, transformer_class=aa.TransformerDFT
         ),
     )
 
 
 def make_interferometer_7_grid():
     return aa.Interferometer(
-        visibilities=make_visibilities_7(),
+        data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2(),
         real_space_mask=make_sub_mask_2d_7x7(),
         settings=aa.SettingsInterferometer(
             sub_size=1, transformer_class=aa.TransformerDFT
         ),
     )
 
 
 def make_interferometer_7_lop():
-
     return aa.Interferometer(
-        visibilities=make_visibilities_7(),
+        data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2(),
         real_space_mask=make_mask_2d_7x7(),
         settings=aa.SettingsInterferometer(
             sub_size_pixelization=1, transformer_class=aa.TransformerNUFFT
         ),
     )
@@ -293,54 +287,48 @@
     )
 
 
 ### MASKED DATA ###
 
 
 def make_masked_imaging_7x7():
-
     imaging_7x7 = make_imaging_7x7()
 
     return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
 
 def make_masked_imaging_covariance_7x7():
-
     imaging_7x7 = make_imaging_covariance_7x7()
 
     return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
 
 def make_masked_imaging_7x7_no_blur():
-
     imaging_7x7 = make_imaging_7x7_no_blur()
 
     return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
 
 def make_model_image_7x7():
-
     imaging_7x7 = make_masked_imaging_7x7()
 
     return 5.0 * imaging_7x7.image
 
 
 def make_imaging_fit_x1_plane_7x7():
-
     imaging_7x7 = make_masked_imaging_7x7()
 
     model_data = 5.0 * imaging_7x7.image
 
     return aa.m.MockFitImaging(
         dataset=imaging_7x7, use_mask_in_fit=False, model_data=model_data
     )
 
 
 def make_fit_interferometer_7():
-
     interferometer_7 = make_interferometer_7()
 
     model_data = 5.0 * interferometer_7.visibilities
 
     return aa.m.MockFitInterferometer(
         dataset=interferometer_7, use_mask_in_fit=False, model_data=model_data
     )
@@ -369,15 +357,14 @@
 def make_rectangular_mesh_grid_3x3():
     return aa.Mesh2DRectangular.overlay_grid(
         grid=make_sub_grid_2d_7x7(), shape_native=(3, 3)
     )
 
 
 def make_delaunay_mesh_grid_9():
-
     grid_9 = aa.Grid2D.no_mask(
         values=[
             [0.6, -0.3],
             [0.5, -0.8],
             [0.2, 0.1],
             [0.0, 0.5],
             [-0.3, -0.8],
@@ -390,15 +377,14 @@
         pixel_scales=1.0,
     )
 
     return aa.Mesh2DDelaunay(values=grid_9)
 
 
 def make_voronoi_mesh_grid_9():
-
     grid_9 = aa.Grid2D.no_mask(
         values=[
             [0.6, -0.3],
             [0.5, -0.8],
             [0.2, 0.1],
             [0.0, 0.5],
             [-0.3, -0.8],
@@ -416,83 +402,78 @@
         nearest_pixelization_index_for_slim_index=np.zeros(
             shape=make_grid_2d_7x7().shape_slim, dtype="int"
         ),
     )
 
 
 def make_rectangular_mapper_7x7_3x3():
-
     mapper_grids = aa.MapperGrids(
         source_plane_data_grid=make_sub_grid_2d_7x7(),
         source_plane_mesh_grid=make_rectangular_mesh_grid_3x3(),
         image_plane_mesh_grid=None,
-        hyper_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
+        adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperRectangularNoInterp(
         mapper_grids=mapper_grids, regularization=make_regularization_constant()
     )
 
 
 def make_delaunay_mapper_9_3x3():
-
     mapper_grids = aa.MapperGrids(
         source_plane_data_grid=make_sub_grid_2d_7x7(),
         source_plane_mesh_grid=make_delaunay_mesh_grid_9(),
         image_plane_mesh_grid=aa.Grid2D.uniform(shape_native=(3, 3), pixel_scales=0.1),
-        hyper_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
+        adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperDelaunay(
         mapper_grids=mapper_grids, regularization=make_regularization_constant()
     )
 
 
 def make_voronoi_mapper_9_3x3():
     mapper_grids = aa.MapperGrids(
         source_plane_data_grid=make_sub_grid_2d_7x7(),
         source_plane_mesh_grid=make_voronoi_mesh_grid_9(),
         image_plane_mesh_grid=aa.Grid2D.uniform(shape_native=(3, 3), pixel_scales=0.1),
-        hyper_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
+        adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperVoronoiNoInterp(
         mapper_grids=mapper_grids, regularization=make_regularization_constant()
     )
 
 
 def make_voronoi_mapper_nn_9_3x3():
     mapper_grids = aa.MapperGrids(
         source_plane_data_grid=make_sub_grid_2d_7x7(),
         source_plane_mesh_grid=make_voronoi_mesh_grid_9(),
         image_plane_mesh_grid=aa.Grid2D.uniform(shape_native=(3, 3), pixel_scales=0.1),
-        hyper_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
+        adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperVoronoi(mapper_grids=mapper_grids, regularization=None)
 
 
 def make_rectangular_inversion_7x7_3x3():
-
     return aa.Inversion(
         dataset=make_masked_imaging_7x7(),
         linear_obj_list=[make_rectangular_mapper_7x7_3x3()],
     )
 
 
 def make_delaunay_inversion_9_3x3():
-
     return aa.Inversion(
         dataset=make_masked_imaging_7x7(),
         linear_obj_list=[make_delaunay_mapper_9_3x3()],
     )
 
 
 def make_voronoi_inversion_9_3x3():
-
     return aa.Inversion(
         dataset=make_masked_imaging_7x7(), linear_obj_list=[make_voronoi_mapper_9_3x3()]
     )
 
 
 ### EUCLID DATA ####
```

### Comparing `autoarray-2023.3.27.1/autoarray/geometry/abstract_2d.py` & `autoarray-2023.7.7.1/autoarray/geometry/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/geometry/geometry_1d.py` & `autoarray-2023.7.7.1/autoarray/geometry/geometry_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/geometry/geometry_2d.py` & `autoarray-2023.7.7.1/autoarray/geometry/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/geometry/geometry_2d_irregular.py` & `autoarray-2023.7.7.1/autoarray/geometry/geometry_2d_irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/geometry/geometry_util.py` & `autoarray-2023.7.7.1/autoarray/geometry/geometry_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,14 @@
 @numba_util.jit()
 def pixel_coordinates_1d_from(
     scaled_coordinates_1d: Tuple[float],
     shape_slim: Tuple[int],
     pixel_scales: ty.PixelScales,
     origins: Tuple[float] = (0.0, 0.0),
 ) -> Union[Tuple[float], Tuple[float]]:
-
     central_pixel_coordinates = central_pixel_coordinates_1d_from(shape_slim=shape_slim)
 
     x_pixel = int(
         (scaled_coordinates_1d[0] - origins[0]) / pixel_scales[0]
         + central_pixel_coordinates[0]
         + 0.5
     )
@@ -141,15 +140,14 @@
 @numba_util.jit()
 def scaled_coordinates_1d_from(
     pixel_coordinates_1d: Tuple[float],
     shape_slim: Tuple[int],
     pixel_scales: ty.PixelScales,
     origins: Tuple[float] = (0.0, 0.0),
 ) -> Union[Tuple[float], Tuple[float]]:
-
     central_scaled_coordinates = central_scaled_coordinate_1d_from(
         shape_slim=shape_slim, pixel_scales=pixel_scales, origin=origins
     )
 
     x_pixel = pixel_scales[0] * (
         pixel_coordinates_1d[0] - central_scaled_coordinates[0]
     )
@@ -477,15 +475,14 @@
     grid_pixels_2d_slim = np.zeros((grid_scaled_2d_slim.shape[0], 2))
 
     centres_scaled = central_scaled_coordinate_2d_from(
         shape_native=shape_native, pixel_scales=pixel_scales, origin=origin
     )
 
     for slim_index in range(grid_scaled_2d_slim.shape[0]):
-
         grid_pixels_2d_slim[slim_index, 0] = (
             (-grid_scaled_2d_slim[slim_index, 0] / pixel_scales[0])
             + centres_scaled[0]
             + 0.5
         )
         grid_pixels_2d_slim[slim_index, 1] = (
             (grid_scaled_2d_slim[slim_index, 1] / pixel_scales[1])
@@ -540,15 +537,14 @@
     grid_pixels_2d_slim = np.zeros((grid_scaled_2d_slim.shape[0], 2))
 
     centres_scaled = central_scaled_coordinate_2d_from(
         shape_native=shape_native, pixel_scales=pixel_scales, origin=origin
     )
 
     for slim_index in range(grid_scaled_2d_slim.shape[0]):
-
         grid_pixels_2d_slim[slim_index, 0] = int(
             (-grid_scaled_2d_slim[slim_index, 0] / pixel_scales[0])
             + centres_scaled[0]
             + 0.5
         )
         grid_pixels_2d_slim[slim_index, 1] = int(
             (grid_scaled_2d_slim[slim_index, 1] / pixel_scales[1])
@@ -611,15 +607,14 @@
         pixel_scales=pixel_scales,
         origin=origin,
     )
 
     grid_pixel_indexes_2d_slim = np.zeros(grid_pixels_2d_slim.shape[0])
 
     for slim_index in range(grid_pixels_2d_slim.shape[0]):
-
         grid_pixel_indexes_2d_slim[slim_index] = int(
             grid_pixels_2d_slim[slim_index, 0] * shape_native[1]
             + grid_pixels_2d_slim[slim_index, 1]
         )
 
     return grid_pixel_indexes_2d_slim
 
@@ -667,15 +662,14 @@
     grid_scaled_2d_slim = np.zeros((grid_pixels_2d_slim.shape[0], 2))
 
     centres_scaled = central_scaled_coordinate_2d_from(
         shape_native=shape_native, pixel_scales=pixel_scales, origin=origin
     )
 
     for slim_index in range(grid_scaled_2d_slim.shape[0]):
-
         grid_scaled_2d_slim[slim_index, 0] = (
             -(grid_pixels_2d_slim[slim_index, 0] - centres_scaled[0] - 0.5)
             * pixel_scales[0]
         )
         grid_scaled_2d_slim[slim_index, 1] = (
             grid_pixels_2d_slim[slim_index, 1] - centres_scaled[1] - 0.5
         ) * pixel_scales[1]
@@ -736,7 +730,45 @@
                 (-grid_scaled_2d[y, x, 0] / pixel_scales[0]) + centres_scaled[0] + 0.5
             )
             grid_pixels_2d[y, x, 1] = int(
                 (grid_scaled_2d[y, x, 1] / pixel_scales[1]) + centres_scaled[1] + 0.5
             )
 
     return grid_pixels_2d
+
+
+def extent_symmetric_from(
+    extent: Tuple[float, float, float, float]
+) -> Tuple[float, float, float, float]:
+    """
+    Given an input extent of the form (x_min, x_max, y_min, y_max), this function returns an extent which is
+    symmetric about the origin.
+
+    For example, if the sepration from x_min to x_max is 2.0 and the separation from y_min to y_max is 1.0, the
+    returned extent expands the y-axis to also have a separation of 2.0.
+
+    Parameters
+    ----------
+    extent
+        The extent which is to be made symmetric about the origin.
+
+    Returns
+    -------
+    The new extent which is symmetric about the origin.
+    """
+
+    y_min = extent[2]
+    y_max = extent[3]
+    x_min = extent[0]
+    x_max = extent[1]
+
+    y_sep = y_max - y_min
+    x_sep = x_max - x_min
+
+    if y_sep > x_sep:
+        x_min -= (y_sep - x_sep) / 2
+        x_max += (y_sep - x_sep) / 2
+    elif x_sep > y_sep:
+        y_min -= (x_sep - y_sep) / 2
+        y_max += (x_sep - y_sep) / 2
+
+    return (x_min, x_max, y_min, y_max)
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/abstract.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/abstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from scipy.sparse.linalg import splu
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from autoconf import cached_property
 from autoarray.numba_util import profile_func
 
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
+from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.regularization.abstract import AbstractRegularization
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 from autoarray.structures.visibilities import Visibilities
 
@@ -162,17 +163,15 @@
         A list of the index range of the parameters of each linear object in the inversion of the input cls type.
         """
         index_list = []
 
         pixel_count = 0
 
         for linear_obj in self.linear_obj_list:
-
             if isinstance(linear_obj, cls):
-
                 index_list.append([pixel_count, pixel_count + linear_obj.params])
 
             pixel_count += linear_obj.params
 
         return index_list
 
     def cls_list_from(self, cls: Type, cls_filtered: Optional[Type] = None) -> List:
@@ -256,32 +255,25 @@
     def total_regularizations(self) -> int:
         return sum(
             regularization is not None for regularization in self.regularization_list
         )
 
     @property
     def no_regularization_index_list(self) -> List[int]:
-
         # TODO : Needs to be range based on pixels.
 
         no_regularization_index_list = []
 
-        pixel_count = 0
+        param_range_list = self.param_range_list_from(cls=LinearObj)
 
-        for linear_obj, regularization in zip(
-            self.linear_obj_list, self.regularization_list
+        for linear_obj, regularization, param_range in zip(
+            self.linear_obj_list, self.regularization_list, param_range_list
         ):
-
             if regularization is None:
-
-                for pixel in range(pixel_count, pixel_count + linear_obj.params):
-
-                    no_regularization_index_list.append(pixel)
-
-            pixel_count += linear_obj.params
+                no_regularization_index_list += range(param_range[0], param_range[1])
 
         return no_regularization_index_list
 
     @property
     def mask(self) -> Array2D:
         return self.data.mask
 
@@ -404,38 +396,24 @@
         to ensure if we access it after computing the `curvature_reg_matrix` it is correctly recalculated in a new
         array of memory.
         """
         if not self.has(cls=AbstractRegularization):
             return self.curvature_matrix
 
         if len(self.regularization_list) == 1:
-
             curvature_matrix = self.curvature_matrix
             curvature_matrix += self.regularization_matrix
 
             del self.__dict__["curvature_matrix"]
 
             return curvature_matrix
 
         return np.add(self.curvature_matrix, self.regularization_matrix)
 
     @cached_property
-    def curvature_reg_matrix_solver(self):
-
-        if self.settings.force_edge_pixels_to_zeros:
-
-            curvature_reg_matrix_solver = copy.copy(self.curvature_reg_matrix)
-
-            curvature_reg_matrix_solver[:, self.mapper_edge_pixel_list] = 0.0
-
-            return curvature_reg_matrix_solver
-
-        return self.curvature_reg_matrix
-
-    @cached_property
     @profile_func
     def curvature_reg_matrix_reduced(self) -> np.ndarray:
         """
         The linear system of equations solves for F + regularization_coefficient*H, which is computed below.
 
         This is the curvature reg matrix for only the mappers, which is necessary for computing the log det
         term without the linear light profiles included.
@@ -450,36 +428,105 @@
         )
         curvature_reg_matrix = np.delete(
             curvature_reg_matrix, self.no_regularization_index_list, 1
         )
 
         return curvature_reg_matrix
 
+    @property
+    def mapper_zero_pixel_list(self) -> np.ndarray:
+        mapper_zero_pixel_list = []
+        param_range_list = self.param_range_list_from(cls=LinearObj)
+        for param_range, linear_obj in zip(param_range_list, self.linear_obj_list):
+            if isinstance(linear_obj, AbstractMapper):
+                mapping_matrix_for_image_pixels_source_zero = linear_obj.mapping_matrix[
+                    self.settings.image_pixels_source_zero
+                ]
+                source_pixels_zero = (
+                    np.sum(mapping_matrix_for_image_pixels_source_zero != 0, axis=0)
+                    != 0
+                )
+                mapper_zero_pixel_list.append(
+                    np.where(source_pixels_zero == True)[0] + param_range[0]
+                )
+        return mapper_zero_pixel_list
+
     @cached_property
     @profile_func
     def reconstruction(self) -> np.ndarray:
         """
         Solve the linear system [F + reg_coeff*H] S = D -> S = [F + reg_coeff*H]^-1 D given by equation (12)
-        of https://arxiv.org/pdf/astro-ph/0302587.pdf
+        of https://arxiv.org/pdf/astro-ph/0302587.pdf (Positive-Negative solution)
 
-        S is the vector of reconstructed inversion values.
+        ============================================================================================
+
+        Solve the Eq.(2) of https://arxiv.org/pdf/astro-ph/0302587.pdf (Non-negative solution)
+        Find non-negative solution that minimizes |Z * S - x|^2.
+
+        We use fnnls (https://github.com/jvendrow/fnnls) to optimize the quadratic value. Two commonly used
+        variables in the code are defined as follows:
+            ZTZ := np.dot(Z.T, Z)
+            ZTx := np.dot(Z.T, x)
         """
         if self.settings.use_positive_only_solver:
+            """
+            For the new implementation, we now need to take out the cols and rows of
+            the curvature_reg_matrix that corresponds to the parameters we force to be 0.
+            Similar for the data vector.
+
+            What we actually doing is that we have set the correspoding cols of the Z to be 0.
+            As the curvature_reg_matrix = ZTZ, so the cols and rows are all taken out.
+            And the data_vector = ZTx, so the corresponding row is also taken out.
+            """
+
+            if self.settings.force_edge_pixels_to_zeros:
+                if self.settings.force_edge_image_pixels_to_zeros:
+                    ids_zeros = np.unique(
+                        np.append(
+                            self.mapper_edge_pixel_list, self.mapper_zero_pixel_list
+                        )
+                    )
+                else:
+                    ids_zeros = self.mapper_edge_pixel_list
 
-            return inversion_util.reconstruction_positive_only_from(
-                data_vector=self.data_vector,
-                curvature_reg_matrix=self.curvature_reg_matrix_solver,
-                settings=self.settings,
-            )
+                values_to_solve = np.ones(
+                    np.shape(self.curvature_reg_matrix)[0], dtype=bool
+                )
+                values_to_solve[ids_zeros] = False
+
+                data_vector_input = self.data_vector[values_to_solve]
+
+                curvature_reg_matrix_input = self.curvature_reg_matrix[
+                    values_to_solve, :
+                ][:, values_to_solve]
+
+                solutions = np.zeros(np.shape(self.curvature_reg_matrix)[0])
+
+                solutions[
+                    values_to_solve
+                ] = inversion_util.reconstruction_positive_only_from(
+                    data_vector=data_vector_input,
+                    curvature_reg_matrix=curvature_reg_matrix_input,
+                    settings=self.settings,
+                )
+                return solutions
+            else:
+                solutions = inversion_util.reconstruction_positive_only_from(
+                    data_vector=self.data_vector,
+                    curvature_reg_matrix=self.curvature_reg_matrix,
+                    settings=self.settings,
+                )
+
+                return solutions
 
         mapper_param_range_list = self.param_range_list_from(cls=AbstractMapper)
 
         return inversion_util.reconstruction_positive_negative_from(
             data_vector=self.data_vector,
-            curvature_reg_matrix=self.curvature_reg_matrix_solver,
+            curvature_reg_matrix=self.curvature_reg_matrix,
             mapper_param_range_list=mapper_param_range_list,
         )
 
     @cached_property
     @profile_func
     def reconstruction_reduced(self) -> np.ndarray:
         """
@@ -524,15 +571,14 @@
         The dictionary of ndarrays of values for each individual mapper.
         """
         source_quantity_dict = {}
 
         index = 0
 
         for linear_obj in self.linear_obj_list:
-
             source_quantity_dict[linear_obj] = source_quantity[
                 index : index + linear_obj.params
             ]
 
             index += linear_obj.params
 
         return source_quantity_dict
@@ -653,25 +699,23 @@
         if not self.has(cls=AbstractRegularization):
             return 0.0
 
         if self.preloads.log_det_regularization_matrix_term is not None:
             return self.preloads.log_det_regularization_matrix_term
 
         try:
-
             lu = splu(csc_matrix(self.regularization_matrix_reduced))
             diagL = lu.L.diagonal()
             diagU = lu.U.diagonal()
             diagL = diagL.astype(np.complex128)
             diagU = diagU.astype(np.complex128)
 
             return np.real(np.log(diagL).sum() + np.log(diagU).sum())
 
         except RuntimeError:
-
             try:
                 return 2.0 * np.sum(
                     np.log(
                         np.diag(np.linalg.cholesky(self.regularization_matrix_reduced))
                     )
                 )
             except np.linalg.LinAlgError as e:
@@ -752,145 +796,94 @@
                 extent=extent,
             )
             for mapper in self.cls_list_from(cls=AbstractMapper)
         ]
 
     @property
     def magnification_list(self) -> List[float]:
-
         magnification_list = []
 
         interpolated_reconstruction_list = self.interpolated_reconstruction_list_from(
             shape_native=(401, 401)
         )
 
         for i, linear_obj in enumerate(self.linear_obj_list):
-
             mapped_reconstructed_image = self.mapped_reconstructed_image_dict[
                 linear_obj
             ]
             interpolated_reconstruction = interpolated_reconstruction_list[i]
 
             magnification_list.append(
                 np.sum(mapped_reconstructed_image) / np.sum(interpolated_reconstruction)
             )
 
         return magnification_list
 
     @property
     def brightest_reconstruction_pixel_list(self):
-
         brightest_reconstruction_pixel_list = []
 
         for mapper in self.cls_list_from(cls=AbstractMapper):
-
             brightest_reconstruction_pixel_list.append(
                 np.argmax(self.reconstruction_dict[mapper])
             )
 
         return brightest_reconstruction_pixel_list
 
     @property
     def brightest_reconstruction_pixel_centre_list(self):
-
         brightest_reconstruction_pixel_centre_list = []
 
         for mapper in self.cls_list_from(cls=AbstractMapper):
-
             brightest_reconstruction_pixel = np.argmax(self.reconstruction_dict[mapper])
 
             centre = Grid2DIrregular(
                 values=[mapper.source_plane_mesh_grid[brightest_reconstruction_pixel]]
             )
 
             brightest_reconstruction_pixel_centre_list.append(centre)
 
         return brightest_reconstruction_pixel_centre_list
 
     def regularization_weights_from(self, index: int) -> np.ndarray:
-
         linear_obj = self.linear_obj_list[index]
         regularization = self.regularization_list[index]
 
         if regularization is None:
-
             pixels = linear_obj.params
 
-            return np.zero((pixels,))
+            return np.zeros((pixels,))
 
         return regularization.regularization_weights_from(linear_obj=linear_obj)
 
     @property
     def regularization_weights_mapper_dict(self) -> Dict[LinearObj, np.ndarray]:
-
         regularization_weights_dict = {}
 
         for index, mapper in enumerate(self.cls_list_from(cls=AbstractMapper)):
-
             regularization_weights_dict[mapper] = self.regularization_weights_from(
                 index=index
             )
 
         return regularization_weights_dict
 
     @property
-    def residual_map_mapper_dict(self) -> Dict[LinearObj, np.ndarray]:
-
-        return {
-            mapper: inversion_util.inversion_residual_map_from(
-                reconstruction=self.reconstruction_dict[mapper],
-                data=self.data,
-                slim_index_for_sub_slim_index=mapper.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim,
-                sub_slim_indexes_for_pix_index=mapper.sub_slim_indexes_for_pix_index,
-            )
-            for mapper in self.cls_list_from(cls=AbstractMapper)
-        }
+    @profile_func
+    def _data_vector_mapper(self) -> np.ndarray:
+        raise NotImplementedError
 
     @property
-    def normalized_residual_map_mapper_dict(self) -> Dict[LinearObj, np.ndarray]:
-
-        return {
-            mapper: inversion_util.inversion_normalized_residual_map_from(
-                reconstruction=self.reconstruction_dict[mapper],
-                data=self.data,
-                noise_map_1d=self.noise_map.slim,
-                slim_index_for_sub_slim_index=mapper.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim,
-                sub_slim_indexes_for_pix_index=mapper.sub_slim_indexes_for_pix_index,
-            )
-            for mapper in self.cls_list_from(cls=AbstractMapper)
-        }
+    @profile_func
+    def _curvature_matrix_mapper_diag(self) -> Optional[np.ndarray]:
+        raise NotImplementedError
 
     @property
-    def chi_squared_map_mapper_dict(self) -> Dict[LinearObj, np.ndarray]:
-
-        return {
-            mapper: inversion_util.inversion_chi_squared_map_from(
-                reconstruction=self.reconstruction_dict[mapper],
-                data=self.data,
-                noise_map_1d=self.noise_map.slim,
-                slim_index_for_sub_slim_index=mapper.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim,
-                sub_slim_indexes_for_pix_index=mapper.sub_slim_indexes_for_pix_index,
-            )
-            for mapper in self.cls_list_from(cls=AbstractMapper)
-        }
+    def linear_func_operated_mapping_matrix_dict(self) -> Dict:
+        raise NotImplementedError
 
     @property
-    def curvature_matrix_preload(self) -> np.ndarray:
-        (
-            curvature_matrix_preload,
-            curvature_matrix_counts,
-        ) = inversion_util.curvature_matrix_preload_from(
-            mapping_matrix=self.operated_mapping_matrix
-        )
-
-        return curvature_matrix_preload
+    def data_linear_func_matrix_dict(self):
+        raise NotImplementedError
 
     @property
-    def curvature_matrix_counts(self) -> np.ndarray:
-        (
-            curvature_matrix_preload,
-            curvature_matrix_counts,
-        ) = inversion_util.curvature_matrix_preload_from(
-            mapping_matrix=self.operated_mapping_matrix
-        )
-
-        return curvature_matrix_counts
+    def mapper_operated_mapping_matrix_dict(self) -> Dict:
+        raise NotImplementedError
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/factory.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,28 +68,27 @@
     """
     if settings.use_w_tilde:
         w_tilde = dataset.w_tilde
     else:
         w_tilde = None
 
     if isinstance(dataset, Imaging):
-
         return inversion_imaging_unpacked_from(
-            image=dataset.image,
+            data=dataset.data,
             noise_map=dataset.noise_map,
             convolver=dataset.convolver,
             w_tilde=w_tilde,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     return inversion_interferometer_unpacked_from(
-        visibilities=dataset.visibilities,
+        data=dataset.visibilities,
         noise_map=dataset.noise_map,
         transformer=dataset.transformer,
         w_tilde=w_tilde,
         linear_obj_list=linear_obj_list,
         settings=settings,
         profiling_dict=profiling_dict,
     )
@@ -147,39 +146,38 @@
         A dictionary which contains timing of certain functions calls which is used for profiling.
 
     Returns
     -------
     An `Inversion` whose type is determined by the input `dataset` and `settings`.
     """
     if isinstance(dataset, Imaging):
-
         return inversion_imaging_unpacked_from(
-            image=data,
+            data=data,
             noise_map=noise_map,
             convolver=dataset.convolver,
             w_tilde=w_tilde,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     return inversion_interferometer_unpacked_from(
-        visibilities=data,
+        data=data,
         noise_map=noise_map,
         transformer=dataset.transformer,
         w_tilde=w_tilde,
         linear_obj_list=linear_obj_list,
         settings=settings,
         profiling_dict=profiling_dict,
     )
 
 
 def inversion_imaging_unpacked_from(
-    image: Array2D,
+    data: Array2D,
     noise_map: Array2D,
     convolver: Convolver,
     w_tilde: WTildeImaging,
     linear_obj_list: List[LinearObj],
     settings: SettingsInversion = SettingsInversion(),
     preloads: Preloads = Preloads(),
     profiling_dict: Optional[Dict] = None,
@@ -200,15 +198,15 @@
     input `settings`) which solve for the linear object parameters in different ways.
 
     This factory inspects the type of dataset input and settings of the inversion in order to create the appropriate
     inversion object.
 
     Parameters
     ----------
-    image
+    data
         The `image` data of the `Imaging` dataset which may have been changed.
     noise_map
         The noise_map of the `Imaging` dataset which may have been changed.
     w_tilde
         Object which uses the `Imaging` dataset's PSF / `Convolver` operateor to perform the `Inversion` using the
         w-tilde formalism.
     linear_obj_list
@@ -223,57 +221,55 @@
         A dictionary which contains timing of certain functions calls which is used for profiling.
 
     Returns
     -------
     An `Inversion` whose type is determined by the input `dataset` and `settings`.
     """
 
-    if any(
+    if all(
         isinstance(linear_obj, AbstractLinearObjFuncList)
         for linear_obj in linear_obj_list
     ):
         use_w_tilde = False
     elif preloads.use_w_tilde is not None:
         use_w_tilde = preloads.use_w_tilde
     else:
         use_w_tilde = settings.use_w_tilde
 
     if not settings.use_w_tilde:
         use_w_tilde = False
 
     if preloads.w_tilde is not None:
-
         w_tilde = preloads.w_tilde
 
     if use_w_tilde:
-
         return InversionImagingWTilde(
-            data=image,
+            data=data,
             noise_map=noise_map,
             convolver=convolver,
             w_tilde=w_tilde,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     return InversionImagingMapping(
-        data=image,
+        data=data,
         noise_map=noise_map,
         convolver=convolver,
         linear_obj_list=linear_obj_list,
         settings=settings,
         preloads=preloads,
         profiling_dict=profiling_dict,
     )
 
 
 def inversion_interferometer_unpacked_from(
-    visibilities: Visibilities,
+    data: Visibilities,
     noise_map: VisibilitiesNoiseMap,
     transformer: Union[TransformerDFT, TransformerNUFFT],
     w_tilde: WTildeInterferometer,
     linear_obj_list: List[LinearObj],
     settings: SettingsInversion = SettingsInversion(),
     preloads: Preloads = Preloads(),
     profiling_dict: Optional[Dict] = None,
@@ -295,15 +291,15 @@
     input `settings`) which solve for the linear object parameters in different ways.
 
     This factory inspects the type of dataset input and settings of the inversion in order to create the appropriate
     inversion object.
 
     Parameters
     ----------
-    image
+    data
         The `image` data of the `Imaging` dataset which may have been changed.
     noise_map
         The noise_map of the `Imaging` dataset which may have been changed.
     w_tilde
         Object which uses the `Imaging` dataset's PSF / `Convolver` operateor to perform the `Inversion` using the
         w-tilde formalism.
     linear_obj_list
@@ -331,44 +327,40 @@
         for linear_obj in linear_obj_list
     ):
         use_w_tilde = False
     else:
         use_w_tilde = settings.use_w_tilde
 
     if not settings.use_linear_operators:
-
         if use_w_tilde:
-
             return InversionInterferometerWTilde(
-                data=visibilities,
+                data=data,
                 noise_map=noise_map,
                 transformer=transformer,
                 w_tilde=w_tilde,
                 linear_obj_list=linear_obj_list,
                 settings=settings,
                 preloads=preloads,
                 profiling_dict=profiling_dict,
             )
 
         else:
-
             return InversionInterferometerMapping(
-                data=visibilities,
+                data=data,
                 noise_map=noise_map,
                 transformer=transformer,
                 linear_obj_list=linear_obj_list,
                 settings=settings,
                 preloads=preloads,
                 profiling_dict=profiling_dict,
             )
 
     else:
-
         return InversionInterferometerMappingPyLops(
-            data=visibilities,
+            data=data,
             noise_map=noise_map,
             transformer=transformer,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/abstract.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/abstract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import numpy as np
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Type
 
 from autoconf import cached_property
 
 from autoarray.numba_util import profile_func
 
 from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
+from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.inversion.abstract import AbstractInversion
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.operators.convolver import Convolver
 
+from autoarray.inversion.inversion.imaging import inversion_imaging_util
+
 
 class AbstractInversionImaging(AbstractInversion):
     def __init__(
         self,
         data: Array2D,
         noise_map: Array2D,
         convolver: Convolver,
@@ -102,29 +105,28 @@
         """
 
         return [
             self.convolver.convolve_mapping_matrix(
                 mapping_matrix=linear_obj.mapping_matrix
             )
             if linear_obj.operated_mapping_matrix_override is None
-            else linear_obj.operated_mapping_matrix_override
+            else self.linear_func_operated_mapping_matrix_dict[linear_obj]
             for linear_obj in self.linear_obj_list
         ]
 
-    def _linear_func_preload_dict_map(self, linear_func_preload_dict: Dict) -> Dict:
-
-        linear_func_dict = {}
+    def _updated_cls_key_dict_from(self, cls: Type, preload_dict: Dict) -> Dict:
+        cls_dict = {}
 
         for linear_func, values in zip(
-            self.cls_list_from(cls=AbstractLinearObjFuncList),
-            linear_func_preload_dict.values(),
+            self.cls_list_from(cls=cls),
+            preload_dict.values(),
         ):
-            linear_func_dict[linear_func] = values
+            cls_dict[linear_func] = values
 
-        return linear_func_dict
+        return cls_dict
 
     @cached_property
     @profile_func
     def linear_func_operated_mapping_matrix_dict(self) -> Dict:
         """
         The `operated_mapping_matrix` of a linear object describes the mappings between the observed data's values and
         the linear objects model, including a 2D convolution operation. It is described fully in the method
@@ -136,96 +138,120 @@
 
         Returns
         -------
         A dictionary mapping every linear function object to its operated mapping matrix.
         """
 
         if self.preloads.linear_func_operated_mapping_matrix_dict is not None:
-            return self._linear_func_preload_dict_map(
-                linear_func_preload_dict=self.preloads.linear_func_operated_mapping_matrix_dict
+            return self._updated_cls_key_dict_from(
+                cls=AbstractLinearObjFuncList,
+                preload_dict=self.preloads.linear_func_operated_mapping_matrix_dict,
             )
 
         linear_func_operated_mapping_matrix_dict = {}
 
         for linear_func in self.cls_list_from(cls=AbstractLinearObjFuncList):
-
             if linear_func.operated_mapping_matrix_override is not None:
                 operated_mapping_matrix = linear_func.operated_mapping_matrix_override
             else:
                 operated_mapping_matrix = self.convolver.convolve_mapping_matrix(
                     mapping_matrix=linear_func.mapping_matrix
                 )
 
             linear_func_operated_mapping_matrix_dict[
                 linear_func
             ] = operated_mapping_matrix
 
         return linear_func_operated_mapping_matrix_dict
 
-    @cached_property
-    @profile_func
-    def linear_func_weighted_mapping_vectors_dict(self) -> Dict:
+    @property
+    def data_linear_func_matrix_dict(self):
         """
-        The diagonals of the `curvature_matrix` of linear func objects are computed by multiplying the operated
-        values of each linear func by the noise-map.
+        Returns a matrix that for each data pixel, maps it to the sum of the values of a linear object function
+        convolved with the PSF kernel at the data pixel.
 
-        This property therefore returns a dictionary mapping every linear func object to this quantity.
+        If a linear function in an inversion is fixed, its values can be evaluated and preloaded beforehand. For every
+        data pixel, the PSF convolution with this preloaded linear function can also be preloaded, in a matrix of
+        shape [data_pixels, 1].
+
+        Given that multiple linear functions can be used and fixed in an inversion, this matrix is extended to have
+        dimensions [data_pixels, total_fixed_linear_functions].
+
+        When mapper objects and linear functions are used simultaneously in an inversion, this preloaded matrix
+        significantly speed up the computation of their off-diagonal terms in the curvature matrix.
+
+        This is similar to the preloading performed via the w-tilde formalism, except that there it is the PSF convolved
+        values of each noise-map value pair that are preloaded.
+
+        In **PyAutoGalaxy** and **PyAutoLens**, this preload is used when linear light profiles are fixed in the model.
+        For example, when using a multi Gaussian expansion, the values defining how those Gaussians are evaluated
+        (e.g. `centre`, `ell_comps` and `sigma`) are often fixed in a model, meaning this matrix can be preloaded and
+        used for speed up.
 
         Returns
         -------
-        A dictionary mapping every linear function object to its operated mapping matrix divided by the noise and
-        convolved with the kernel.
+        ndarray
+            A matrix of shape [data_pixels, total_fixed_linear_functions] that for each data pixel, maps it to the sum
+            of the values of a linear object function convolved with the PSF kernel at the data pixel.
         """
-
-        if self.preloads.linear_func_weighted_mapping_vectors_dict is not None:
-            return self._linear_func_preload_dict_map(
-                linear_func_preload_dict=self.preloads.linear_func_weighted_mapping_vectors_dict
+        if self.preloads.data_linear_func_matrix_dict is not None:
+            return self._updated_cls_key_dict_from(
+                cls=AbstractLinearObjFuncList,
+                preload_dict=self.preloads.data_linear_func_matrix_dict,
             )
 
-        linear_func_weighted_mapping_vectors_dict = {}
+        linear_func_list = self.cls_list_from(cls=AbstractLinearObjFuncList)
 
-        for (
-            linear_func,
-            operated_mapping_matrix,
-        ) in self.linear_func_operated_mapping_matrix_dict.items():
+        data_linear_func_matrix_dict = {}
 
-            linear_func_weighted_mapping_vectors_dict[linear_func] = (
-                operated_mapping_matrix / self.noise_map[:, None]
+        for func_index, linear_func in enumerate(linear_func_list):
+            curvature_weights = (
+                self.linear_func_operated_mapping_matrix_dict[linear_func]
+                / self.noise_map[:, None] ** 2
             )
 
-        return linear_func_weighted_mapping_vectors_dict
+            data_linear_func_matrix = (
+                inversion_imaging_util.data_linear_func_matrix_from(
+                    curvature_weights_matrix=curvature_weights,
+                    image_frame_1d_lengths=self.convolver.image_frame_1d_lengths,
+                    image_frame_1d_indexes=self.convolver.image_frame_1d_indexes,
+                    image_frame_1d_kernels=self.convolver.image_frame_1d_kernels,
+                )
+            )
+
+            data_linear_func_matrix_dict[linear_func] = data_linear_func_matrix
+
+        return data_linear_func_matrix_dict
 
     @cached_property
     @profile_func
-    def linear_func_curvature_vectors_dict(self) -> Dict:
+    def mapper_operated_mapping_matrix_dict(self) -> Dict:
         """
-        The rows (and columns) of the `curvature_matrix` of a linear object are computed by dividing the operated
-        values of each linear func by the noise-map squared and convolving with the kernel.
+        The `operated_mapping_matrix` of a `Mapper` object describes the mappings between the observed data's values
+        and the mapper's mesh pixels after a 2D convolution operation. It is described fully in the method
+        `operated_mapping_matrix`.
 
-        This property therefore returns a dictionary mapping every linear func object to this quantity, which is
-        termed the curvature vector and is representative of a linear func's row of the curvature matrix.
+        This property returns a dictionary mapping every mapper object to its corresponded operated mapping
+        matrix, which is used for constructing the matrices that perform the linear inversion in an efficent way
+        for the w_tilde calculation.
 
         Returns
         -------
-        A dictionary mapping every linear function object to its curvature vector (its operated mapping matrix
-        divided by the noise squared convolved with the kernel).
+        A dictionary mapping every mapper object to its operated mapping matrix.
         """
 
-        if self.preloads.linear_func_curvature_vectors_dict is not None:
-            return self._linear_func_preload_dict_map(
-                linear_func_preload_dict=self.preloads.linear_func_curvature_vectors_dict
+        if self.preloads.mapper_operated_mapping_matrix_dict is not None:
+            return self._updated_cls_key_dict_from(
+                cls=AbstractMapper,
+                preload_dict=self.preloads.mapper_operated_mapping_matrix_dict,
             )
 
-        linear_func_curvature_vectors_dict = {}
-
-        for (
-            linear_func,
-            operated_mapping_matrix,
-        ) in self.linear_func_operated_mapping_matrix_dict.items():
+        mapper_operated_mapping_matrix_dict = {}
 
-            linear_func_curvature_vectors_dict[
-                linear_func
-            ] = self.convolver.convolve_mapping_matrix(
-                mapping_matrix=operated_mapping_matrix / self.noise_map[:, None] ** 2
+        for mapper in self.cls_list_from(cls=AbstractMapper):
+            operated_mapping_matrix = self.convolver.convolve_mapping_matrix(
+                mapping_matrix=mapper.mapping_matrix
             )
 
-        return linear_func_curvature_vectors_dict
+            mapper_operated_mapping_matrix_dict[mapper] = operated_mapping_matrix
+
+        return mapper_operated_mapping_matrix_dict
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/inversion_imaging_util.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/inversion_imaging_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,22 +54,20 @@
     image_pixels = len(native_index_for_slim_index)
 
     w_tilde_data = np.zeros((image_pixels,))
 
     weight_map_native = image_native / noise_map_native**2.0
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         value = 0.0
 
         for k0_y in range(kernel_native.shape[0]):
             for k0_x in range(kernel_native.shape[1]):
-
                 weight_value = weight_map_native[
                     ip0_y + k0_y + kernel_shift_y, ip0_x + k0_x + kernel_shift_x
                 ]
 
                 if not np.isnan(weight_value):
                     value += kernel_native[k0_y, k0_x] * weight_value
 
@@ -110,19 +108,17 @@
         the curvature matrix.
     """
     image_pixels = len(native_index_for_slim_index)
 
     w_tilde_curvature = np.zeros((image_pixels, image_pixels))
 
     for ip0 in range(w_tilde_curvature.shape[0]):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         for ip1 in range(ip0, w_tilde_curvature.shape[1]):
-
             ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
             w_tilde_curvature[ip0, ip1] += w_tilde_curvature_value_from(
                 value_native=noise_map_native,
                 kernel_native=kernel_native,
                 ip0_y=ip0_y,
                 ip0_x=ip0_x,
@@ -149,15 +145,15 @@
     datasets.
 
     The limitation of this matrix is that the dimensions of [image_pixels, image_pixels] can exceed many 10s of GB's,
     making it impossible to store in memory and its use in linear algebra calculations slow. This methods creates
     a sparse matrix that can compute the matrix `w_tilde_curvature` efficiently, albeit the linear algebra calculations
     in PyAutoArray bypass this matrix entirely to go straight to the curvature matrix.
 
-    For imaging data, w_tilde is a sparse matrix, whereby non-zero entries are only contained for pairs of image pixels
+    for dataset data, w_tilde is a sparse matrix, whereby non-zero entries are only contained for pairs of image pixels
     where the two pixels overlap due to the kernel size. For example, if the kernel size is (11, 11) and two image
     pixels are separated by more than 20 pixels, the kernel will never convolve flux between the two pixels. Two image
     pixels will only share a convolution if they are within `kernel_overlap_size = 2 * kernel_shape - 1` pixels within
     one another.
 
     Thus, a `w_tilde_curvature_preload` matrix of dimensions [image_pixels, kernel_overlap_size ** 2] can be computed
     which significantly reduces the memory consumption by removing the sparsity. Because the dimensions of the second
@@ -201,21 +197,19 @@
     )
 
     curvature_preload_tmp = np.zeros((image_pixels, kernel_overlap_size))
     curvature_indexes_tmp = np.zeros((image_pixels, kernel_overlap_size))
     curvature_lengths = np.zeros(image_pixels)
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         kernel_index = 0
 
         for ip1 in range(ip0, curvature_preload_tmp.shape[0]):
-
             ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
             noise_value = w_tilde_curvature_value_from(
                 value_native=noise_map_native,
                 kernel_native=kernel_native,
                 ip0_y=ip0_y,
                 ip0_x=ip0_x,
@@ -223,32 +217,29 @@
                 ip1_x=ip1_x,
             )
 
             if ip0 == ip1:
                 noise_value /= 2.0
 
             if noise_value > 0.0:
-
                 curvature_preload_tmp[ip0, kernel_index] = noise_value
                 curvature_indexes_tmp[ip0, kernel_index] = ip1
                 kernel_index += 1
 
         curvature_lengths[ip0] = kernel_index
 
     curvature_total_pairs = int(np.sum(curvature_lengths))
 
     curvature_preload = np.zeros((curvature_total_pairs))
     curvature_indexes = np.zeros((curvature_total_pairs))
 
     index = 0
 
     for i in range(image_pixels):
-
         for data_index in range(int(curvature_lengths[i])):
-
             curvature_preload[index] = curvature_preload_tmp[i, data_index]
             curvature_indexes[index] = curvature_indexes_tmp[i, data_index]
 
             index += 1
 
     return (curvature_preload, curvature_indexes, curvature_lengths)
 
@@ -318,31 +309,28 @@
         return curvature_value
 
     kernel_pixels = kernel_native.shape[0] * kernel_native.shape[1]
     kernel_count = 0
 
     for k0_y in range(kernel_native.shape[0]):
         for k0_x in range(kernel_native.shape[1]):
-
             value = value_native[
                 ip0_y + k0_y + kernel_shift_y, ip0_x + k0_x + kernel_shift_x
             ]
 
             if value > 0.0:
-
                 k1_y = k0_y + ip_y_offset
                 k1_x = k0_x + ip_x_offset
 
                 if (
                     k1_y >= 0
                     and k1_x >= 0
                     and k1_y < kernel_native.shape[0]
                     and k1_x < kernel_native.shape[1]
                 ):
-
                     kernel_count += 1
 
                     kernel_value_0 = kernel_native[k0_y, k0_x]
                     kernel_value_1 = kernel_native[k1_y, k1_x]
 
                     curvature_value += (
                         kernel_value_0 * kernel_value_1 * (1.0 / value) ** 2.0
@@ -390,17 +378,15 @@
     """
 
     data_pixels = w_tilde_data.shape[0]
 
     data_vector = np.zeros(pix_pixels)
 
     for data_0 in range(data_pixels):
-
         for pix_0_index in range(pix_lengths[data_0]):
-
             data_0_weight = data_weights[data_0, pix_0_index]
             pix_0 = data_to_pix_unique[data_0, pix_0_index]
 
             data_vector[pix_0] += data_0_weight * w_tilde_data[data_0]
 
     return data_vector
 
@@ -497,27 +483,23 @@
     data_pixels = curvature_lengths.shape[0]
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     curvature_index = 0
 
     for data_0 in range(data_pixels):
-
         for data_1_index in range(curvature_lengths[data_0]):
-
             data_1 = curvature_indexes[curvature_index]
             w_tilde_value = curvature_preload[curvature_index]
 
             for pix_0_index in range(pix_lengths[data_0]):
-
                 data_0_weight = data_weights[data_0, pix_0_index]
                 pix_0 = data_to_pix_unique[data_0, pix_0_index]
 
                 for pix_1_index in range(pix_lengths[data_1]):
-
                     data_1_weight = data_weights[data_1, pix_1_index]
                     pix_1 = data_to_pix_unique[data_1, pix_1_index]
 
                     curvature_matrix[pix_0, pix_1] += (
                         data_0_weight * data_1_weight * w_tilde_value
                     )
 
@@ -599,89 +581,221 @@
     data_pixels = curvature_lengths.shape[0]
 
     curvature_matrix = np.zeros((pix_pixels_0, pix_pixels_1))
 
     curvature_index = 0
 
     for data_0 in range(data_pixels):
-
         for data_1_index in range(curvature_lengths[data_0]):
-
             data_1 = curvature_indexes[curvature_index]
             w_tilde_value = curvature_preload[curvature_index]
 
             for pix_0_index in range(pix_lengths_0[data_0]):
-
                 data_0_weight = data_weights_0[data_0, pix_0_index]
                 pix_0 = data_to_pix_unique_0[data_0, pix_0_index]
 
                 for pix_1_index in range(pix_lengths_1[data_1]):
-
                     data_1_weight = data_weights_1[data_1, pix_1_index]
                     pix_1 = data_to_pix_unique_1[data_1, pix_1_index]
 
                     curvature_matrix[pix_0, pix_1] += (
                         data_0_weight * data_1_weight * w_tilde_value
                     )
 
             curvature_index += 1
 
     return curvature_matrix
 
 
 @numba_util.jit()
+def data_linear_func_matrix_from(
+    curvature_weights_matrix: np.ndarray,
+    image_frame_1d_lengths: np.ndarray,
+    image_frame_1d_indexes: np.ndarray,
+    image_frame_1d_kernels: np.ndarray,
+) -> np.ndarray:
+    """
+    Returns a matrix that for each data pixel, maps it to the sum of the values of a linear object function convolved
+    with the PSF kernel at the data pixel.
+
+    If a linear function in an inversion is fixed, its values can be evaluated and preloaded beforehand. For every
+    data pixel, the PSF convolution with this preloaded linear function can also be preloaded, in a matrix of
+    shape [data_pixels, 1].
+
+    Given that multiple linear functions can be used and fixed in an inversion, this matrix is extended to have
+    dimensions [data_pixels, total_fixed_linear_functions].
+
+    When mapper objects and linear functions are used simultaneously in an inversion, this preloaded matrix
+    significantly speed up the computation of their off-diagonal terms in the curvature matrix.
+
+    This is similar to the preloading performed via the w-tilde formalism, except that there it is the PSF convolved
+    values of each noise-map value pair that are preloaded.
+
+    In **PyAutoGalaxy** and **PyAutoLens**, this preload is used when linear light profiles are fixed in the model.
+    For example, when using a multi Gaussian expansion, the values defining how those Gaussians are evaluated
+    (e.g. `centre`, `ell_comps` and `sigma`) are often fixed in a model, meaning this matrix can be preloaded and
+    used for speed up.
+
+    Parameters
+    ----------
+    curvature_weights_matrix
+        The operated values of each linear function divided by the noise-map squared, in a matrix of shape
+        [data_pixels, total_fixed_linear_functions].
+    image_frame_indexes
+        The indexes of all masked pixels that the PSF blurs light into (see the `Convolver` object).
+    image_frame_kernels
+        The kernel values of all masked pixels that the PSF blurs light into (see the `Convolver` object).
+    image_frame_length
+        The number of masked pixels it will blur light into (unmasked pixels are excluded, see the `Convolver` object).
+
+    Returns
+    -------
+    ndarray
+        A matrix of shape [data_pixels, total_fixed_linear_functions] that for each data pixel, maps it to the sum of
+        the values of a linear object function convolved with the PSF kernel at the data pixel.
+    """
+    data_pixels = curvature_weights_matrix.shape[0]
+    linear_func_pixels = curvature_weights_matrix.shape[1]
+
+    data_linear_func_matrix_dict = np.zeros(shape=(data_pixels, linear_func_pixels))
+
+    for data_0 in range(data_pixels):
+        for psf_index in range(image_frame_1d_lengths[data_0]):
+            data_index = image_frame_1d_indexes[data_0, psf_index]
+            kernel_value = image_frame_1d_kernels[data_0, psf_index]
+
+            for linear_index in range(linear_func_pixels):
+                data_linear_func_matrix_dict[data_0, linear_index] += (
+                    kernel_value * curvature_weights_matrix[data_index, linear_index]
+                )
+
+    return data_linear_func_matrix_dict
+
+
+@numba_util.jit()
+def curvature_matrix_off_diags_via_data_linear_func_matrix_from(
+    data_linear_func_matrix: np.ndarray,
+    data_to_pix_unique: np.ndarray,
+    data_weights: np.ndarray,
+    pix_lengths: np.ndarray,
+    pix_pixels: int,
+):
+    """
+    Returns the off diagonal terms in the curvature matrix `F` (see Warren & Dye 2003) between a mapper object
+    and a linear func object, using the preloaded `data_linear_func_matrix` of the values of the linear functions.
+
+
+    If a linear function in an inversion is fixed, its values can be evaluated and preloaded beforehand. For every
+    data pixel, the PSF convolution with this preloaded linear function can also be preloaded, in a matrix of
+    shape [data_pixels, 1].
+
+    When mapper objects and linear functions are used simultaneously in an inversion, this preloaded matrix
+    significantly speed up the computation of their off-diagonal terms in the curvature matrix.
+
+    This function performs this efficient calcluation via the preloaded `data_linear_func_matrix`.
+
+    Parameters
+    ----------
+    data_linear_func_matrix
+        A matrix of shape [data_pixels, total_fixed_linear_functions] that for each data pixel, maps it to the sum of
+        the values of a linear object function convolved with the PSF kernel at the data pixel.
+    data_to_pix_unique
+        The indexes of all pixels that each data pixel maps to (see the `Mapper` object).
+    data_weights
+        The weights of all pixels that each data pixel maps to (see the `Mapper` object).
+    pix_lengths
+        The number of pixelization pixels that each data pixel maps to (see the `Mapper` object).
+    pix_pixels
+        The number of pixelization pixels in the pixelization (see the `Mapper` object).
+    """
+
+    linear_func_pixels = data_linear_func_matrix.shape[1]
+
+    off_diag = np.zeros((pix_pixels, linear_func_pixels))
+
+    data_pixels = data_weights.shape[0]
+
+    for data_0 in range(data_pixels):
+        for pix_0_index in range(pix_lengths[data_0]):
+            data_0_weight = data_weights[data_0, pix_0_index]
+            pix_0 = data_to_pix_unique[data_0, pix_0_index]
+
+            for linear_index in range(linear_func_pixels):
+                off_diag[pix_0, linear_index] += (
+                    data_linear_func_matrix[data_0, linear_index] * data_0_weight
+                )
+
+    return off_diag
+
+
+@numba_util.jit()
 def curvature_matrix_off_diags_via_mapper_and_linear_func_curvature_vector_from(
     data_to_pix_unique: np.ndarray,
     data_weights: np.ndarray,
     pix_lengths: np.ndarray,
     pix_pixels: int,
-    curvature_vector: np.ndarray,
+    curvature_weights: np.ndarray,
+    image_frame_1d_lengths: np.ndarray,
+    image_frame_1d_indexes: np.ndarray,
+    image_frame_1d_kernels: np.ndarray,
 ) -> np.ndarray:
     """
     Returns the off diagonal terms in the curvature matrix `F` (see Warren & Dye 2003) between a mapper object
-    and a linear func object.
+    and a linear func object, using the unique mappings between data pixels and pixelization pixels.
+
+    This takes as input the curvature weights of the linear function object, which are the values of the linear
+    function convolved with the PSF and divided by the noise-map squared.
 
-    This uses the unique mappings of the mapper and the curvature vector (its operated mapping matrix
-    divided by the noise squared convolved with the kernel).
+    For each unique mapping between a data pixel and a pixelization pixel, the pixels which that pixel convolves
+    light into are computed, multiplied by their corresponding curvature weights and summed. This process also
+    accounts the sub-pixel mapping of each data pixel to the pixelization pixel
+
+    This is done for every unique mapping of a data pixel to a pixelization pixel, giving the off-diagonal terms in
+    the curvature matrix.
 
     Parameters
     ----------
     data_to_pix_unique
         An array that maps every data pixel index (e.g. the masked image pixel indexes in 1D) to its unique set of
         pixelization pixel indexes (see `data_slim_to_pixelization_unique_from`).
     data_weights
         For every unique mapping between a set of data sub-pixels and a pixelization pixel, the weight of these mapping
         based on the number of sub-pixels that map to pixelization pixel.
     pix_lengths
         A 1D array describing how many unique pixels each data pixel maps too, which is used to iterate over
         `data_to_pix_unique` and `data_weights`.
     pix_pixels
         The total number of pixels in the pixelization that reconstructs the data.
-    curvature_vector
-        The operated values of the linear func divided by the noise-map squared and convolved with the kernel, which is
-        representative of a linear func's row of the curvature matrix.
+    curvature_weights
+        The operated values of the linear func divided by the noise-map squared.
+    image_frame_indexes
+        The indexes of all masked pixels that the PSF blurs light into (see the `Convolver` object).
+    image_frame_kernels
+        The kernel values of all masked pixels that the PSF blurs light into (see the `Convolver` object).
+    image_frame_length
+        The number of masked pixels it will blur light into (unmasked pixels are excluded, see the `Convolver` object).
 
     Returns
     -------
     ndarray
         The curvature matrix `F` (see Warren & Dye 2003).
     """
 
     data_pixels = data_weights.shape[0]
-    linear_func_pixels = curvature_vector.shape[1]
+    linear_func_pixels = curvature_weights.shape[1]
 
-    curvature_matrix = np.zeros((pix_pixels, linear_func_pixels))
+    off_diag = np.zeros((pix_pixels, linear_func_pixels))
 
     for data_0 in range(data_pixels):
-
         for pix_0_index in range(pix_lengths[data_0]):
-
             data_0_weight = data_weights[data_0, pix_0_index]
             pix_0 = data_to_pix_unique[data_0, pix_0_index]
 
-            for linear_index in range(linear_func_pixels):
+            for psf_index in range(image_frame_1d_lengths[data_0]):
+                data_index = image_frame_1d_indexes[data_0, psf_index]
+                kernel_value = image_frame_1d_kernels[data_0, psf_index]
 
-                curvature_matrix[pix_0, linear_index] += (
-                    data_0_weight * curvature_vector[data_0, linear_index]
+                off_diag[pix_0, :] += (
+                    data_0_weight * curvature_weights[data_index, :] * kernel_value
                 )
 
-    return curvature_matrix
+    return off_diag
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/mapping.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,56 @@
             convolver=convolver,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
+    @property
+    @profile_func
+    def _data_vector_mapper(self) -> np.ndarray:
+        """
+        Returns the `data_vector` of all mappers, a 1D vector whose values are solved for by the simultaneous
+        linear equations constructed by this object. The object is described in full in the method `data_vector`.
+
+        This method is used to compute part of the `data_vector` if there are also linear function list objects
+        in the inversion, and is separated into a separate method to enable preloading of the mapper `data_vector`.
+        """
+
+        if self.preloads.data_vector_mapper is not None:
+            return self.preloads.data_vector_mapper
+
+        if not self.has(cls=AbstractMapper):
+            return None
+
+        data_vector = np.zeros(self.total_params)
+
+        mapper_list = self.cls_list_from(cls=AbstractMapper)
+        mapper_param_range_list = self.param_range_list_from(cls=AbstractMapper)
+
+        for i in range(len(mapper_list)):
+            mapper = mapper_list[i]
+            param_range = mapper_param_range_list[i]
+
+            operated_mapping_matrix = self.convolver.convolve_mapping_matrix(
+                mapping_matrix=mapper.mapping_matrix
+            )
+
+            data_vector_mapper = (
+                inversion_imaging_util.data_vector_via_blurred_mapping_matrix_from(
+                    blurred_mapping_matrix=operated_mapping_matrix,
+                    image=self.data,
+                    noise_map=self.noise_map,
+                )
+            )
+
+            data_vector[param_range[0] : param_range[1],] = data_vector_mapper
+
+        return data_vector
+
     @cached_property
     @profile_func
     def data_vector(self) -> np.ndarray:
         """
         The `data_vector` is a 1D vector whose values are solved for by the simultaneous linear equations constructed
         by this object.
 
@@ -74,114 +116,111 @@
 
         If there are multiple linear objects their `operated_mapping_matrix` properties will have already been
         concatenated ensuring their `data_vector` values are solved for simultaneously.
 
         The calculation is described in more detail in `inversion_util.data_vector_via_blurred_mapping_matrix_from`.
         """
 
+        if self.preloads.data_vector_mapper is not None:
+            return self.preloads.data_vector_mapper
+
         if self.preloads.operated_mapping_matrix is not None:
             operated_mapping_matrix = self.preloads.operated_mapping_matrix
         else:
             operated_mapping_matrix = self.operated_mapping_matrix
 
         return inversion_imaging_util.data_vector_via_blurred_mapping_matrix_from(
             blurred_mapping_matrix=operated_mapping_matrix,
             image=self.data,
             noise_map=self.noise_map,
         )
 
-    @cached_property
-    @profile_func
-    def curvature_matrix(self):
-        """
-        The `curvature_matrix` is a 2D matrix which uses the mappings between the data and the linear objects to
-        construct the simultaneous linear equations.
-
-        The linear algebra is described in the paper https://arxiv.org/pdf/astro-ph/0302587.pdf, where the
-        curvature matrix given by equation (4) and the letter F.
-
-        If there are multiple linear objects their `operated_mapping_matrix` properties will have already been
-        concatenated ensuring their `curvature_matrix` values are solved for simultaneously. This includes all
-        diagonal and off-diagonal terms describing the covariances between linear objects.
-
-        The `curvature_matrix` computed here is overwritten in memory when the regularization matrix is added to it,
-        because for large matrices this avoids overhead. For this reason, `curvature_matrix` is not a cached property
-        to ensure if we access it after computing the `curvature_reg_matrix` it is correctly recalculated in a new
-        array of memory.
-        """
-
-        if self.preloads.curvature_matrix is not None:
-
-            # Need to copy because of how curvature_reg_matirx overwrites memory.
-
-            return copy.copy(self.preloads.curvature_matrix)
-
-        if self.preloads.curvature_matrix_preload is None:
-
-            return inversion_util.curvature_matrix_via_mapping_matrix_from(
-                mapping_matrix=self.operated_mapping_matrix,
-                noise_map=self.noise_map,
-                add_to_curvature_diag=self.settings.no_regularization_add_to_curvature_diag,
-                no_regularization_index_list=self.no_regularization_index_list,
-            )
-
-        return inversion_util.curvature_matrix_via_sparse_preload_from(
-            mapping_matrix=self.operated_mapping_matrix,
-            noise_map=self.noise_map,
-            curvature_matrix_preload=self.preloads.curvature_matrix_preload,
-            curvature_matrix_counts=self.preloads.curvature_matrix_counts,
-        )
-
     @property
     @profile_func
-    def _curvature_matrix_mapper_diag(self) -> np.ndarray:
+    def _curvature_matrix_mapper_diag(self) -> Optional[np.ndarray]:
         """
         Returns the diagonal regions of the `curvature_matrix`, a 2D matrix which uses the mappings between the data
         and the linear objects to construct the simultaneous linear equations. The object is described in full in
         the method `curvature_matrix`.
 
         This method computes the diagonal entries of all mapper objects in the `curvature_matrix`. It is separate from
         other calculations to enable preloading of this calculation.
         """
 
         if self.preloads.curvature_matrix_mapper_diag is not None:
             return self.preloads.curvature_matrix_mapper_diag
 
+        if not self.has(cls=AbstractMapper):
+            return None
+
         curvature_matrix = np.zeros((self.total_params, self.total_params))
 
         mapper_list = self.cls_list_from(cls=AbstractMapper)
         mapper_param_range_list = self.param_range_list_from(cls=AbstractMapper)
 
         for i in range(len(mapper_list)):
-
             mapper_i = mapper_list[i]
             mapper_param_range_i = mapper_param_range_list[i]
 
             operated_mapping_matrix = self.convolver.convolve_mapping_matrix(
                 mapping_matrix=mapper_i.mapping_matrix
             )
 
             diag = inversion_util.curvature_matrix_via_mapping_matrix_from(
                 mapping_matrix=operated_mapping_matrix,
                 noise_map=self.noise_map,
-                add_to_curvature_diag=self.settings.no_regularization_add_to_curvature_diag,
+                settings=self.settings,
+                add_to_curvature_diag=True,
                 no_regularization_index_list=self.no_regularization_index_list,
             )
 
             curvature_matrix[
                 mapper_param_range_i[0] : mapper_param_range_i[1],
                 mapper_param_range_i[0] : mapper_param_range_i[1],
             ] = diag
 
         curvature_matrix = inversion_util.curvature_matrix_mirrored_from(
             curvature_matrix=curvature_matrix
         )
 
         return curvature_matrix
 
+    @cached_property
+    @profile_func
+    def curvature_matrix(self):
+        """
+        The `curvature_matrix` is a 2D matrix which uses the mappings between the data and the linear objects to
+        construct the simultaneous linear equations.
+
+        The linear algebra is described in the paper https://arxiv.org/pdf/astro-ph/0302587.pdf, where the
+        curvature matrix given by equation (4) and the letter F.
+
+        If there are multiple linear objects their `operated_mapping_matrix` properties will have already been
+        concatenated ensuring their `curvature_matrix` values are solved for simultaneously. This includes all
+        diagonal and off-diagonal terms describing the covariances between linear objects.
+
+        The `curvature_matrix` computed here is overwritten in memory when the regularization matrix is added to it,
+        because for large matrices this avoids overhead. For this reason, `curvature_matrix` is not a cached property
+        to ensure if we access it after computing the `curvature_reg_matrix` it is correctly recalculated in a new
+        array of memory.
+        """
+
+        if self.preloads.curvature_matrix is not None:
+            # Need to copy because of how curvature_reg_matirx overwrites memory.
+
+            return copy.copy(self.preloads.curvature_matrix)
+
+        return inversion_util.curvature_matrix_via_mapping_matrix_from(
+            mapping_matrix=self.operated_mapping_matrix,
+            noise_map=self.noise_map,
+            settings=self.settings,
+            add_to_curvature_diag=True,
+            no_regularization_index_list=self.no_regularization_index_list,
+        )
+
     @property
     @profile_func
     def mapped_reconstructed_data_dict(self) -> Dict[LinearObj, Array2D]:
         """
         When constructing the simultaneous linear equations (via vectors and matrices) the quantities of each individual
         linear object (e.g. their `mapping_matrix`) are combined into single ndarrays via stacking. This does not track
         which quantities belong to which linear objects, therefore the linear equation's solutions (which are returned
@@ -209,15 +248,14 @@
         reconstruction_dict = self.source_quantity_dict_from(
             source_quantity=self.reconstruction
         )
 
         operated_mapping_matrix_list = self.operated_mapping_matrix_list
 
         for index, linear_obj in enumerate(self.linear_obj_list):
-
             reconstruction = reconstruction_dict[linear_obj]
 
             mapped_reconstructed_image = (
                 inversion_util.mapped_reconstructed_data_via_mapping_matrix_from(
                     mapping_matrix=operated_mapping_matrix_list[index],
                     reconstruction=reconstruction,
                 )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/imaging/w_tilde.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/w_tilde.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import numpy as np
 from typing import Dict, List, Optional
 
 from autoconf import cached_property
 
 from autoarray.numba_util import profile_func
 
@@ -72,14 +73,62 @@
             self.w_tilde = w_tilde
             self.w_tilde.check_noise_map(noise_map=noise_map)
         else:
             self.w_tilde = None
 
     @cached_property
     @profile_func
+    def w_tilde_data(self):
+        return inversion_imaging_util.w_tilde_data_imaging_from(
+            image_native=self.data.native,
+            noise_map_native=self.noise_map.native,
+            kernel_native=self.convolver.kernel.native,
+            native_index_for_slim_index=self.data.mask.derive_indexes.native_for_slim,
+        )
+
+    @property
+    @profile_func
+    def _data_vector_mapper(self) -> np.ndarray:
+        """
+        Returns the `data_vector` of all mappers, a 1D vector whose values are solved for by the simultaneous
+        linear equations constructed by this object. The object is described in full in the method `data_vector`.
+
+        This method is used to compute part of the `data_vector` if there are also linear function list objects
+        in the inversion, and is separated into a separate method to enable preloading of the mapper `data_vector`.
+        """
+
+        if self.preloads.data_vector_mapper is not None:
+            return self.preloads.data_vector_mapper
+
+        if not self.has(cls=AbstractMapper):
+            return None
+
+        data_vector = np.zeros(self.total_params)
+
+        mapper_list = self.cls_list_from(cls=AbstractMapper)
+        mapper_param_range = self.param_range_list_from(cls=AbstractMapper)
+
+        for mapper_index, mapper in enumerate(mapper_list):
+            data_vector_mapper = (
+                inversion_imaging_util.data_vector_via_w_tilde_data_imaging_from(
+                    w_tilde_data=self.w_tilde_data,
+                    data_to_pix_unique=mapper.unique_mappings.data_to_pix_unique,
+                    data_weights=mapper.unique_mappings.data_weights,
+                    pix_lengths=mapper.unique_mappings.pix_lengths,
+                    pix_pixels=mapper.params,
+                )
+            )
+            param_range = mapper_param_range[mapper_index]
+
+            data_vector[param_range[0] : param_range[1],] = data_vector_mapper
+
+        return data_vector
+
+    @cached_property
+    @profile_func
     def data_vector(self) -> np.ndarray:
         """
         Returns the `data_vector`, a 1D vector whose values are solved for by the simultaneous linear equations
         constructed by this object.
 
         The linear algebra is described in the paper https://arxiv.org/pdf/astro-ph/0302587.pdf), where the
         data vector is given by equation (4) and the letter D.
@@ -91,34 +140,28 @@
         """
         if self.has(cls=AbstractLinearObjFuncList):
             return self._data_vector_func_list_and_mapper
         elif self.total(cls=AbstractMapper) == 1:
             return self._data_vector_x1_mapper
         return self._data_vector_multi_mapper
 
-    @cached_property
-    @profile_func
-    def w_tilde_data(self):
-        return inversion_imaging_util.w_tilde_data_imaging_from(
-            image_native=self.data.native,
-            noise_map_native=self.noise_map.native,
-            kernel_native=self.convolver.kernel.native,
-            native_index_for_slim_index=self.data.mask.derive_indexes.native_for_slim,
-        )
-
     @property
     @profile_func
     def _data_vector_x1_mapper(self) -> np.ndarray:
         """
         Returns the `data_vector`, a 1D vector whose values are solved for by the simultaneous linear equations
         constructed by this object. The object is described in full in the method `data_vector`.
 
         This method computes the `data_vector` whenthere is a single mapper object in the `Inversion`,
         which circumvents `np.concatenate` for speed up.
         """
+
+        if self.preloads.data_vector_mapper is not None:
+            return self.preloads.data_vector_mapper
+
         linear_obj = self.linear_obj_list[0]
 
         return inversion_imaging_util.data_vector_via_w_tilde_data_imaging_from(
             w_tilde_data=self.w_tilde_data,
             data_to_pix_unique=linear_obj.unique_mappings.data_to_pix_unique,
             data_weights=linear_obj.unique_mappings.data_weights,
             pix_lengths=linear_obj.unique_mappings.pix_lengths,
@@ -131,14 +174,18 @@
         """
         Returns the `data_vector`, a 1D vector whose values are solved for by the simultaneous linear equations
         constructed by this object. The object is described in full in the method `data_vector`.
 
         This method computes the `data_vector` when there are multiple mapper objects in the `Inversion`,
         which computes the `data_vector` of each object and concatenates them.
         """
+
+        if self.preloads.data_vector_mapper is not None:
+            return self.preloads.data_vector_mapper
+
         return np.concatenate(
             [
                 inversion_imaging_util.data_vector_via_w_tilde_data_imaging_from(
                     w_tilde_data=self.w_tilde_data,
                     data_to_pix_unique=linear_obj.unique_mappings.data_to_pix_unique,
                     data_weights=linear_obj.unique_mappings.data_weights,
                     pix_lengths=linear_obj.unique_mappings.pix_lengths,
@@ -153,63 +200,41 @@
     def _data_vector_func_list_and_mapper(self) -> np.ndarray:
         """
         Returns the `data_vector`, a 1D vector whose values are solved for by the simultaneous linear equations
         constructed by this object. The object is described in full in the method `data_vector`.
 
         This method computes the `data_vector` when there are one or more mapper objects in the `Inversion`,
         which are combined with linear function list objects.
+
+        The `data_vector` corresponding to all mapper objects is computed first, in a separate function. This
+        separation of functions enables the `data_vector` to be preloaded in certain circumstances.
         """
 
-        data_vector = np.zeros(self.total_params)
-
-        mapper_list = self.cls_list_from(cls=AbstractMapper)
-        mapper_param_range = self.param_range_list_from(cls=AbstractMapper)
+        data_vector = self._data_vector_mapper
 
         linear_func_param_range = self.param_range_list_from(
             cls=AbstractLinearObjFuncList
         )
 
-        for mapper_index, mapper in enumerate(mapper_list):
+        for linear_func_index, linear_func in enumerate(
+            self.cls_list_from(cls=AbstractLinearObjFuncList)
+        ):
+            operated_mapping_matrix = self.linear_func_operated_mapping_matrix_dict[
+                linear_func
+            ]
 
-            data_vector_mapper = (
-                inversion_imaging_util.data_vector_via_w_tilde_data_imaging_from(
-                    w_tilde_data=self.w_tilde_data,
-                    data_to_pix_unique=mapper.unique_mappings.data_to_pix_unique,
-                    data_weights=mapper.unique_mappings.data_weights,
-                    pix_lengths=mapper.unique_mappings.pix_lengths,
-                    pix_pixels=mapper.params,
-                )
+            diag = inversion_imaging_util.data_vector_via_blurred_mapping_matrix_from(
+                blurred_mapping_matrix=operated_mapping_matrix,
+                image=self.data,
+                noise_map=self.noise_map,
             )
-            param_range = mapper_param_range[mapper_index]
-
-            data_vector[
-                param_range[0] : param_range[1],
-            ] = data_vector_mapper
-
-            for linear_func_index, linear_func in enumerate(
-                self.cls_list_from(cls=AbstractLinearObjFuncList)
-            ):
-
-                operated_mapping_matrix = self.linear_func_operated_mapping_matrix_dict[
-                    linear_func
-                ]
-
-                diag = (
-                    inversion_imaging_util.data_vector_via_blurred_mapping_matrix_from(
-                        blurred_mapping_matrix=operated_mapping_matrix,
-                        image=self.data,
-                        noise_map=self.noise_map,
-                    )
-                )
 
-                param_range = linear_func_param_range[linear_func_index]
+            param_range = linear_func_param_range[linear_func_index]
 
-                data_vector[
-                    param_range[0] : param_range[1],
-                ] = diag
+            data_vector[param_range[0] : param_range[1],] = diag
 
         return data_vector
 
     @cached_property
     @profile_func
     def curvature_matrix(self) -> np.ndarray:
         """
@@ -228,42 +253,63 @@
 
         The `curvature_matrix` computed here is overwritten in memory when the regularization matrix is added to it,
         because for large matrices this avoids overhead. For this reason, `curvature_matrix` is not a cached property
         to ensure if we access it after computing the `curvature_reg_matrix` it is correctly recalculated in a new
         array of memory.
         """
 
+        if self.preloads.curvature_matrix is not None:
+            # Need to copy because of how curvature_reg_matirx overwrites memory.
+
+            return copy.copy(self.preloads.curvature_matrix)
+
         if self.has(cls=AbstractLinearObjFuncList):
-            return self._curvature_matrix_func_list_and_mapper
+            curvature_matrix = self._curvature_matrix_func_list_and_mapper
         elif self.total(cls=AbstractMapper) == 1:
-            return self._curvature_matrix_x1_mapper
-        return self._curvature_matrix_multi_mapper
+            curvature_matrix = self._curvature_matrix_x1_mapper
+        else:
+            curvature_matrix = self._curvature_matrix_multi_mapper
+
+        curvature_matrix = inversion_util.curvature_matrix_mirrored_from(
+            curvature_matrix=curvature_matrix
+        )
+
+        if len(self.no_regularization_index_list) > 0:
+            curvature_matrix = inversion_util.curvature_matrix_with_added_to_diag_from(
+                curvature_matrix=curvature_matrix,
+                value=self.settings.no_regularization_add_to_curvature_diag_value,
+                no_regularization_index_list=self.no_regularization_index_list,
+            )
+
+        return curvature_matrix
 
     @property
     @profile_func
-    def _curvature_matrix_mapper_diag(self) -> np.ndarray:
+    def _curvature_matrix_mapper_diag(self) -> Optional[np.ndarray]:
         """
         Returns the diagonal regions of the `curvature_matrix`, a 2D matrix which uses the mappings between the data
         and the linear objects to construct the simultaneous linear equations. The object is described in full in
         the method `curvature_matrix`.
 
         This method computes the diagonal entries of all mapper objects in the `curvature_matrix`. It is separate from
         other calculations to enable preloading of this calculation.
         """
 
         if self.preloads.curvature_matrix_mapper_diag is not None:
             return self.preloads.curvature_matrix_mapper_diag
 
+        if not self.has(cls=AbstractMapper):
+            return None
+
         curvature_matrix = np.zeros((self.total_params, self.total_params))
 
         mapper_list = self.cls_list_from(cls=AbstractMapper)
         mapper_param_range_list = self.param_range_list_from(cls=AbstractMapper)
 
         for i in range(len(mapper_list)):
-
             mapper_i = mapper_list[i]
             mapper_param_range_i = mapper_param_range_list[i]
 
             diag = inversion_imaging_util.curvature_matrix_via_w_tilde_curvature_preload_imaging_from(
                 curvature_preload=self.w_tilde.curvature_preload,
                 curvature_indexes=self.w_tilde.indexes,
                 curvature_lengths=self.w_tilde.lengths,
@@ -277,18 +323,14 @@
                 mapper_param_range_i[0] : mapper_param_range_i[1],
                 mapper_param_range_i[0] : mapper_param_range_i[1],
             ] = diag
 
             if self.total(cls=AbstractMapper) == 1:
                 return curvature_matrix
 
-        curvature_matrix = inversion_util.curvature_matrix_mirrored_from(
-            curvature_matrix=curvature_matrix
-        )
-
         return curvature_matrix
 
     @profile_func
     def _curvature_matrix_off_diag_from(
         self, mapper_0: AbstractMapper, mapper_1: AbstractMapper
     ) -> np.ndarray:
         """
@@ -359,36 +401,30 @@
         if self.total(cls=AbstractMapper) == 1:
             return curvature_matrix
 
         mapper_list = self.cls_list_from(cls=AbstractMapper)
         mapper_param_range_list = self.param_range_list_from(cls=AbstractMapper)
 
         for i in range(len(mapper_list)):
-
             mapper_i = mapper_list[i]
             mapper_param_range_i = mapper_param_range_list[i]
 
             for j in range(i + 1, len(mapper_list)):
-
                 mapper_j = mapper_list[j]
                 mapper_param_range_j = mapper_param_range_list[j]
 
                 off_diag = self._curvature_matrix_off_diag_from(
                     mapper_0=mapper_i, mapper_1=mapper_j
                 )
 
                 curvature_matrix[
                     mapper_param_range_i[0] : mapper_param_range_i[1],
                     mapper_param_range_j[0] : mapper_param_range_j[1],
                 ] = off_diag
 
-        curvature_matrix = inversion_util.curvature_matrix_mirrored_from(
-            curvature_matrix=curvature_matrix
-        )
-
         return curvature_matrix
 
     @property
     @profile_func
     def _curvature_matrix_func_list_and_mapper(self) -> np.ndarray:
         """
         The `curvature_matrix` is a 2D matrix which uses the mappings between the data and the linear objects to
@@ -407,59 +443,90 @@
 
         linear_func_list = self.cls_list_from(cls=AbstractLinearObjFuncList)
         linear_func_param_range_list = self.param_range_list_from(
             cls=AbstractLinearObjFuncList
         )
 
         for i in range(len(mapper_list)):
-
             mapper = mapper_list[i]
             mapper_param_range = mapper_param_range_list[i]
 
             for func_index, linear_func in enumerate(linear_func_list):
-
                 linear_func_param_range = linear_func_param_range_list[func_index]
 
-                off_diag = inversion_imaging_util.curvature_matrix_off_diags_via_mapper_and_linear_func_curvature_vector_from(
-                    data_to_pix_unique=mapper.unique_mappings.data_to_pix_unique,
-                    data_weights=mapper.unique_mappings.data_weights,
-                    pix_lengths=mapper.unique_mappings.pix_lengths,
-                    pix_pixels=mapper.params,
-                    curvature_vector=self.linear_func_curvature_vectors_dict[
-                        linear_func
-                    ],
-                )
+                if self.preloads.data_linear_func_matrix_dict is not None:
+                    off_diag = inversion_imaging_util.curvature_matrix_off_diags_via_data_linear_func_matrix_from(
+                        data_linear_func_matrix=self.data_linear_func_matrix_dict[
+                            linear_func
+                        ],
+                        data_to_pix_unique=mapper.unique_mappings.data_to_pix_unique,
+                        data_weights=mapper.unique_mappings.data_weights,
+                        pix_lengths=mapper.unique_mappings.pix_lengths,
+                        pix_pixels=mapper.params,
+                    )
+
+                elif self.preloads.mapper_operated_mapping_matrix_dict is not None:
+                    operated_mapping_matrix = self.mapper_operated_mapping_matrix_dict[
+                        mapper
+                    ]
+
+                    curvature_weights = (
+                        self.linear_func_operated_mapping_matrix_dict[linear_func]
+                    ) / self.noise_map[:, None] ** 2
+
+                    off_diag = np.dot(operated_mapping_matrix.T, curvature_weights)
+
+                else:
+                    curvature_weights = (
+                        self.linear_func_operated_mapping_matrix_dict[linear_func]
+                        / self.noise_map[:, None] ** 2
+                    )
+
+                    off_diag = inversion_imaging_util.curvature_matrix_off_diags_via_mapper_and_linear_func_curvature_vector_from(
+                        data_to_pix_unique=mapper.unique_mappings.data_to_pix_unique,
+                        data_weights=mapper.unique_mappings.data_weights,
+                        pix_lengths=mapper.unique_mappings.pix_lengths,
+                        pix_pixels=mapper.params,
+                        curvature_weights=curvature_weights,
+                        image_frame_1d_lengths=self.convolver.image_frame_1d_lengths,
+                        image_frame_1d_indexes=self.convolver.image_frame_1d_indexes,
+                        image_frame_1d_kernels=self.convolver.image_frame_1d_kernels,
+                    )
 
                 curvature_matrix[
                     mapper_param_range[0] : mapper_param_range[1],
                     linear_func_param_range[0] : linear_func_param_range[1],
                 ] = off_diag
 
         for index_0, linear_func_0 in enumerate(linear_func_list):
-
             linear_func_param_range_0 = linear_func_param_range_list[index_0]
 
-            for index_1, linear_func_1 in enumerate(linear_func_list):
+            weighted_vector_0 = (
+                self.linear_func_operated_mapping_matrix_dict[linear_func_0]
+                / self.noise_map[:, None]
+            )
 
+            for index_1, linear_func_1 in enumerate(linear_func_list):
                 linear_func_param_range_1 = linear_func_param_range_list[index_1]
 
+                weighted_vector_1 = (
+                    self.linear_func_operated_mapping_matrix_dict[linear_func_1]
+                    / self.noise_map[:, None]
+                )
+
                 diag = np.dot(
-                    self.linear_func_weighted_mapping_vectors_dict[linear_func_0].T,
-                    self.linear_func_weighted_mapping_vectors_dict[linear_func_1],
+                    weighted_vector_0.T,
+                    weighted_vector_1,
                 )
 
                 curvature_matrix[
                     linear_func_param_range_0[0] : linear_func_param_range_0[1],
                     linear_func_param_range_1[0] : linear_func_param_range_1[1],
                 ] = diag
 
-        curvature_matrix = inversion_util.curvature_matrix_mirrored_from(
-            curvature_matrix=curvature_matrix
-        )
-
         return curvature_matrix
 
     @property
     @profile_func
     def mapped_reconstructed_data_dict(self) -> Dict[LinearObj, Array2D]:
         """
         When constructing the simultaneous linear equations (via vectors and matrices) the quantities of each individual
@@ -488,19 +555,17 @@
         mapped_reconstructed_data_dict = {}
 
         reconstruction_dict = self.source_quantity_dict_from(
             source_quantity=self.reconstruction
         )
 
         for linear_obj in self.linear_obj_list:
-
             reconstruction = reconstruction_dict[linear_obj]
 
             if isinstance(linear_obj, AbstractMapper):
-
                 mapped_reconstructed_image = inversion_util.mapped_reconstructed_data_via_image_to_pix_unique_from(
                     data_to_pix_unique=linear_obj.unique_mappings.data_to_pix_unique,
                     data_weights=linear_obj.unique_mappings.data_weights,
                     pix_lengths=linear_obj.unique_mappings.pix_lengths,
                     reconstruction=reconstruction,
                 )
 
@@ -510,15 +575,14 @@
                 )
 
                 mapped_reconstructed_image = self.convolver.convolve_image_no_blurring(
                     image=mapped_reconstructed_image
                 )
 
             else:
-
                 operated_mapping_matrix = self.linear_func_operated_mapping_matrix_dict[
                     linear_obj
                 ]
 
                 mapped_reconstructed_image = np.sum(
                     reconstruction * operated_mapping_matrix, axis=1
                 )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/abstract.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
         mapped_reconstructed_image_dict = {}
 
         reconstruction_dict = self.source_quantity_dict_from(
             source_quantity=self.reconstruction
         )
 
         for linear_obj in self.linear_obj_list:
-
             reconstruction = reconstruction_dict[linear_obj]
 
             mapped_reconstructed_image = (
                 inversion_util.mapped_reconstructed_data_via_mapping_matrix_from(
                     mapping_matrix=linear_obj.mapping_matrix,
                     reconstruction=reconstruction,
                 )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/lop.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/lop.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,14 @@
             linear_obj: self.transformer.visibilities_from(image=image)
             for linear_obj, image in mapped_reconstructed_image_dict.items()
         }
 
     @cached_property
     @profile_func
     def preconditioner_matrix(self):
-
         curvature_matrix_approx = np.multiply(
             np.sum(self.noise_map.weight_list_ordered_1d),
             self.linear_obj_list[0].mapping_matrix.T
             @ self.linear_obj_list[0].mapping_matrix,
         )
 
         return np.add(curvature_matrix_approx, self.regularization_matrix)
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/mapping.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,21 +113,19 @@
         imag_curvature_matrix = inversion_util.curvature_matrix_via_mapping_matrix_from(
             mapping_matrix=self.operated_mapping_matrix.imag,
             noise_map=self.noise_map.imag,
         )
 
         curvature_matrix = np.add(real_curvature_matrix, imag_curvature_matrix)
 
-        if (
-            self.settings.no_regularization_add_to_curvature_diag
-            and len(self.no_regularization_index_list) > 0
-        ):
+        if len(self.no_regularization_index_list) > 0:
             curvature_matrix = inversion_util.curvature_matrix_with_added_to_diag_from(
                 curvature_matrix=curvature_matrix,
                 no_regularization_index_list=self.no_regularization_index_list,
+                value=self.settings.no_regularization_add_to_curvature_diag_value,
             )
 
         return curvature_matrix
 
     @property
     @profile_func
     def mapped_reconstructed_data_dict(
@@ -161,15 +159,14 @@
         reconstruction_dict = self.source_quantity_dict_from(
             source_quantity=self.reconstruction
         )
 
         operated_mapping_matrix_list = self.operated_mapping_matrix_list
 
         for index, linear_obj in enumerate(self.linear_obj_list):
-
             reconstruction = reconstruction_dict[linear_obj]
 
             visibilities = (
                 inversion_interferometer_util.mapped_reconstructed_visibilities_from(
                     transformed_mapping_matrix=operated_mapping_matrix_list[index],
                     reconstruction=reconstruction,
                 )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/interferometer/w_tilde.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/w_tilde.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,44 +121,42 @@
         The linear algebra is described in the paper https://arxiv.org/pdf/astro-ph/0302587.pdf, where the
         curvature matrix given by equation (4) and the letter F.
 
         This function computes the diagonal terms of F using the w_tilde formalism.
         """
 
         if self.settings.use_w_tilde_numpy:
-
             return inversion_util.curvature_matrix_via_w_tilde_from(
                 w_tilde=self.w_tilde.w_matrix, mapping_matrix=self.mapping_matrix
             )
 
         from autoarray.inversion.inversion import inversion_util_secret
 
         mapper = self.cls_list_from(cls=AbstractMapper)[0]
 
         if not self.settings.use_source_loop:
-
             return inversion_util_secret.curvature_matrix_via_w_tilde_curvature_preload_interferometer_from(
                 curvature_preload=self.w_tilde.curvature_preload,
                 pix_indexes_for_sub_slim_index=mapper.pix_indexes_for_sub_slim_index,
                 pix_size_for_sub_slim_index=mapper.pix_sizes_for_sub_slim_index,
                 pix_weights_for_sub_slim_index=mapper.pix_weights_for_sub_slim_index,
                 native_index_for_slim_index=self.transformer.real_space_mask.derive_indexes.native_for_slim,
-                pix_pixels=self.linear_obj_list[0].pixels,
+                pix_pixels=self.linear_obj_list[0].params,
             )
 
         (
             sub_slim_indexes_for_pix_index,
             sub_slim_sizes_for_pix_index,
             sub_slim_weights_for_pix_index,
         ) = mapper.sub_slim_indexes_for_pix_index_arr
 
         return inversion_util_secret.curvature_matrix_via_w_tilde_curvature_preload_interferometer_from_2(
             curvature_preload=self.w_tilde.curvature_preload,
             native_index_for_slim_index=self.transformer.real_space_mask.derive_indexes.native_for_slim,
-            pix_pixels=self.linear_obj_list[0].pixels,
+            pix_pixels=self.linear_obj_list[0].params,
             sub_slim_indexes_for_pix_index=sub_slim_indexes_for_pix_index.astype("int"),
             sub_slim_sizes_for_pix_index=sub_slim_sizes_for_pix_index.astype("int"),
             sub_slim_weights_for_pix_index=sub_slim_weights_for_pix_index,
         )
 
     @property
     @profile_func
@@ -189,15 +187,14 @@
             individual mapper (in the image-plane).
         """
         mapped_reconstructed_data_dict = {}
 
         image_dict = self.mapped_reconstructed_image_dict
 
         for linear_obj in self.linear_obj_list:
-
             visibilities = self.transformer.visibilities_from(
                 image=image_dict[linear_obj]
             )
 
             visibilities = Visibilities(visibilities=visibilities)
 
             mapped_reconstructed_data_dict[linear_obj] = visibilities
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/inversion_util.py` & `autoarray-2023.7.7.1/autoarray/preloads.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,555 +1,555 @@
+import logging
 import numpy as np
-from scipy.optimize import nnls
-from typing import List, Optional
+from typing import List
 
 from autoconf import conf
 
-from autoarray.inversion.inversion.settings import SettingsInversion
+from autoarray.inversion.inversion.imaging.abstract import AbstractInversionImaging
+from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
+from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 
-from autoarray import numba_util
 from autoarray import exc
+from autoarray.inversion.inversion.imaging import inversion_imaging_util
 
+logger = logging.getLogger(__name__)
 
-def curvature_matrix_via_w_tilde_from(
-    w_tilde: np.ndarray, mapping_matrix: np.ndarray
-) -> np.ndarray:
-    """
-    Returns the curvature matrix `F` (see Warren & Dye 2003) from `w_tilde`.
-
-    The dimensions of `w_tilde` are [image_pixels, image_pixels], meaning that for datasets with many image pixels
-    this matrix can take up 10's of GB of memory. The calculation of the `curvature_matrix` via this function will
-    therefore be very slow, and the method `curvature_matrix_via_w_tilde_curvature_preload_imaging_from` should be used
-    instead.
-
-    Parameters
-    ----------
-    w_tilde
-        A matrix of dimensions [image_pixels, image_pixels] that encodes the convolution or NUFFT of every image pixel
-        pair on the noise map.
-    mapping_matrix
-        The matrix representing the mappings between sub-grid pixels and pixelization pixels.
-
-    Returns
-    -------
-    ndarray
-        The curvature matrix `F` (see Warren & Dye 2003).
-    """
-
-    return np.dot(mapping_matrix.T, np.dot(w_tilde, mapping_matrix))
-
-
-@numba_util.jit()
-def curvature_matrix_with_added_to_diag_from(
-    curvature_matrix: np.ndarray, no_regularization_index_list: Optional[List] = None
-) -> np.ndarray:
-    """
-    It is common for the `curvature_matrix` computed to not be positive-definite, leading for the inversion
-    via `np.linalg.solve` to fail and raise a `LinAlgError`.
-
-    In many circumstances, adding a small numerical value of `1.0e-8` to the diagonal of the `curvature_matrix`
-    makes it positive definite, such that the inversion is performed without raising an error.
-
-    This function adds this numerical value to the diagonal of the curvature matrix.
-
-    Parameters
-    ----------
-    curvature_matrix
-        The curvature matrix which is being constructed in order to solve a linear system of equations.
-    """
-
-    for i in no_regularization_index_list:
-        curvature_matrix[i, i] += 1e-8
-
-    return curvature_matrix
-
-
-@numba_util.jit()
-def curvature_matrix_mirrored_from(
-    curvature_matrix: np.ndarray,
-) -> np.ndarray:
-
-    curvature_matrix_mirrored = np.zeros(
-        (curvature_matrix.shape[0], curvature_matrix.shape[1])
-    )
-
-    for i in range(curvature_matrix.shape[0]):
-        for j in range(curvature_matrix.shape[1]):
-            if curvature_matrix[i, j] != 0:
-                curvature_matrix_mirrored[i, j] = curvature_matrix[i, j]
-                curvature_matrix_mirrored[j, i] = curvature_matrix[i, j]
-            if curvature_matrix[j, i] != 0:
-                curvature_matrix_mirrored[i, j] = curvature_matrix[j, i]
-                curvature_matrix_mirrored[j, i] = curvature_matrix[j, i]
-
-    return curvature_matrix_mirrored
-
-
-def curvature_matrix_via_mapping_matrix_from(
-    mapping_matrix: np.ndarray,
-    noise_map: np.ndarray,
-    add_to_curvature_diag: bool = False,
-    no_regularization_index_list: Optional[List] = None,
-) -> np.ndarray:
-    """
-    Returns the curvature matrix `F` from a blurred mapping matrix `f` and the 1D noise-map $\sigma$
-     (see Warren & Dye 2003).
-
-    Parameters
-    ----------
-    mapping_matrix
-        The matrix representing the mappings (these could be blurred or transfomed) between sub-grid pixels and
-        pixelization pixels.
-    noise_map
-        Flattened 1D array of the noise-map used by the inversion during the fit.
-    """
-    array = mapping_matrix / noise_map[:, None]
-    curvature_matrix = np.dot(array.T, array)
-
-    if add_to_curvature_diag and len(no_regularization_index_list) > 0:
-        curvature_matrix = curvature_matrix_with_added_to_diag_from(
-            curvature_matrix=curvature_matrix,
-            no_regularization_index_list=no_regularization_index_list,
+logger.setLevel(level="INFO")
+
+
+class Preloads:
+    def __init__(
+        self,
+        w_tilde=None,
+        use_w_tilde=None,
+        sparse_image_plane_grid_pg_list=None,
+        relocated_grid=None,
+        mapper_list=None,
+        operated_mapping_matrix=None,
+        linear_func_operated_mapping_matrix_dict=None,
+        data_linear_func_matrix_dict=None,
+        mapper_operated_mapping_matrix_dict=None,
+        curvature_matrix=None,
+        data_vector_mapper=None,
+        curvature_matrix_mapper_diag=None,
+        regularization_matrix=None,
+        log_det_regularization_matrix_term=None,
+        traced_sparse_grids_list_of_planes=None,
+        sparse_image_plane_grid_list=None,
+    ):
+        self.w_tilde = w_tilde
+        self.use_w_tilde = use_w_tilde
+
+        self.sparse_image_plane_grid_pg_list = sparse_image_plane_grid_pg_list
+        self.relocated_grid = relocated_grid
+        self.mapper_list = mapper_list
+        self.operated_mapping_matrix = operated_mapping_matrix
+        self.linear_func_operated_mapping_matrix_dict = (
+            linear_func_operated_mapping_matrix_dict
         )
+        self.data_linear_func_matrix_dict = data_linear_func_matrix_dict
+        self.mapper_operated_mapping_matrix_dict = mapper_operated_mapping_matrix_dict
+        self.curvature_matrix = curvature_matrix
+        self.data_vector_mapper = data_vector_mapper
+        self.curvature_matrix_mapper_diag = curvature_matrix_mapper_diag
+        self.regularization_matrix = regularization_matrix
+        self.log_det_regularization_matrix_term = log_det_regularization_matrix_term
+
+        self.traced_sparse_grids_list_of_planes = traced_sparse_grids_list_of_planes
+        self.sparse_image_plane_grid_list = sparse_image_plane_grid_list
+
+    @property
+    def check_threshold(self):
+        return conf.instance["general"]["test"]["preloads_check_threshold"]
+
+    def set_w_tilde_imaging(self, fit_0, fit_1):
+        """
+        The w-tilde linear algebra formalism speeds up inversions by computing beforehand quantities that enable
+        efficiently construction of the curvature matrix. These quantities can only be used if the noise-map is
+        fixed, therefore this function preloads these w-tilde quantities if the noise-map does not change.
+
+        This function compares the noise map of two fit's corresponding to two model instances, and preloads wtilde
+        if the noise maps of both fits are the same.
+
+        The preload is typically used through search chaining pipelines, as it is uncommon for the noise map to be
+        scaled during the model-fit (although it is common for a fixed but scaled noise map to be used).
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
+
+        self.w_tilde = None
+        self.use_w_tilde = False
+
+        if fit_0.inversion is None:
+            return
+
+        if not fit_0.inversion.has(cls=AbstractMapper):
+            return
+
+        if np.max(abs(fit_0.noise_map - fit_1.noise_map)) < 1e-8:
+            logger.info("PRELOADS - Computing W-Tilde... May take a moment.")
+
+            from autoarray.dataset.imaging.w_tilde import WTildeImaging
+
+            (
+                preload,
+                indexes,
+                lengths,
+            ) = inversion_imaging_util.w_tilde_curvature_preload_imaging_from(
+                noise_map_native=fit_0.noise_map.native,
+                kernel_native=fit_0.dataset.psf.native,
+                native_index_for_slim_index=fit_0.dataset.mask.derive_indexes.native_for_slim,
+            )
+
+            self.w_tilde = WTildeImaging(
+                curvature_preload=preload,
+                indexes=indexes.astype("int"),
+                lengths=lengths.astype("int"),
+                noise_map_value=fit_0.noise_map[0],
+            )
 
-    return curvature_matrix
+            self.use_w_tilde = True
 
+            logger.info("PRELOADS - W-Tilde preloaded for this model-fit.")
 
-@numba_util.jit()
-def curvature_matrix_preload_from(
-    mapping_matrix: np.ndarray, mapping_matrix_threshold=1.0e-8
-) -> np.ndarray:
-    """
-    Returns a matrix that expresses the non-zero entries of the blurred mapping matrix for an efficient construction of
-    the curvature matrix `F` (see Warren & Dye 2003).
-
-    This is used for models where the blurred mapping matrix does not change, but the noise-map of the values that
-    are used to construct that blurred mapping matrix do change.
-
-    Parameters
-    ----------
-    mapping_matrix
-        The matrix representing the mappings (these could be blurred or transfomed) between sub-grid pixels and
-        pixelization pixels.
-    """
-
-    curvature_matrix_counts = np.zeros(mapping_matrix.shape[0])
-
-    for mask_1d_index in range(mapping_matrix.shape[0]):
-        for pix_index in range(mapping_matrix.shape[1]):
-            if mapping_matrix[mask_1d_index, pix_index] > mapping_matrix_threshold:
-                curvature_matrix_counts[mask_1d_index] += 1
-
-    preload_max = np.max(curvature_matrix_counts)
-
-    curvature_matrix_preload = np.zeros((mapping_matrix.shape[0], int(preload_max)))
-
-    for mask_1d_index in range(mapping_matrix.shape[0]):
-        index = 0
-        for pix_index in range(mapping_matrix.shape[1]):
-            if mapping_matrix[mask_1d_index, pix_index] > mapping_matrix_threshold:
-                curvature_matrix_preload[mask_1d_index, index] = pix_index
-                index += 1
-
-    return curvature_matrix_preload, curvature_matrix_counts
-
-
-@numba_util.jit()
-def curvature_matrix_via_sparse_preload_from(
-    mapping_matrix: np.ndarray,
-    noise_map: np.ndarray,
-    curvature_matrix_preload,
-    curvature_matrix_counts,
-) -> np.ndarray:
-    """
-    Returns the curvature matrix `F` from a blurred mapping matrix `f` and the 1D noise-map $\sigma$
-     (see Warren & Dye 2003) via a sparse preload matrix, which has already mapped out where all non-zero entries
-     and multiplications take place.
-
-    This is used for models where the blurred mapping matrix does not change, but the noise-map of the values that
-    are used to construct that blurred mapping matrix do change.
-
-    Parameters
-    ----------
-    mapping_matrix
-        The matrix representing the mappings (these could be blurred or transfomed) between sub-grid pixels and
-        pixelization pixels.
-    noise_map
-        Flattened 1D array of the noise-map used by the inversion during the fit.
-    """
-    curvature_matrix = np.zeros((mapping_matrix.shape[1], mapping_matrix.shape[1]))
-
-    for mask_1d_index in range(mapping_matrix.shape[0]):
-
-        total_pix = curvature_matrix_counts[mask_1d_index]
-
-        for preload_index_0 in range(total_pix):
-            for preload_index_1 in range(
-                preload_index_0, curvature_matrix_counts[mask_1d_index]
+    def set_relocated_grid(self, fit_0, fit_1):
+        """
+        If the `MassProfile`'s in a model are fixed their traced grids (which may have had coordinates relocated at
+        the border) does not change during the model=fit and can therefore be preloaded.
+
+        This function compares the relocated grids of the mappers of two fit corresponding to two model instances, and
+        preloads the grid if the grids of both fits are the same.
+
+        The preload is typically used in adapt searches, where the mass model is fixed and the parameters are
+        varied.
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
+
+        self.relocated_grid = None
+
+        if fit_0.inversion is None:
+            return
+
+        if (
+            fit_0.inversion.total(cls=AbstractMapper) > 1
+            or fit_0.inversion.total(cls=AbstractMapper) == 0
+        ):
+            return
+
+        mapper_0 = fit_0.inversion.cls_list_from(cls=AbstractMapper)[0]
+        mapper_1 = fit_1.inversion.cls_list_from(cls=AbstractMapper)[0]
+
+        if (
+            mapper_0.source_plane_data_grid.shape[0]
+            == mapper_1.source_plane_data_grid.shape[0]
+        ):
+            if (
+                np.max(
+                    abs(
+                        mapper_0.source_plane_data_grid
+                        - mapper_1.source_plane_data_grid
+                    )
+                )
+                < 1.0e-8
             ):
+                self.relocated_grid = mapper_0.source_plane_data_grid
 
-                pix_index_0 = curvature_matrix_preload[mask_1d_index, preload_index_0]
-                pix_index_1 = curvature_matrix_preload[mask_1d_index, preload_index_1]
+                logger.info(
+                    "PRELOADS - Relocated grid of pxielization preloaded for this model-fit."
+                )
+
+    def set_mapper_list(self, fit_0, fit_1):
+        """
+        If the `MassProfile`'s and `Mesh`'s in a model are fixed, the mapping of image-pixels to the
+        source-pixels does not change during the model-fit and the list of `Mapper`'s containing this information can
+        be preloaded. This includes preloading the `mapping_matrix`.
+
+        This function compares the mapping matrix of two fit's corresponding to two model instances, and preloads the
+        list of mappers if the mapping matrix of both fits are the same.
+
+        The preload is typically used in searches where only light profiles vary (e.g. when only the lens's light is
+        being fitted for).
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
+
+        self.mapper_list = None
 
-                curvature_matrix[pix_index_0, pix_index_1] += (
-                    mapping_matrix[mask_1d_index, pix_index_0]
-                    * mapping_matrix[mask_1d_index, pix_index_1]
-                ) / noise_map[mask_1d_index] ** 2
+        if fit_0.inversion is None:
+            return
 
-    for i in range(mapping_matrix.shape[1]):
-        for j in range(mapping_matrix.shape[1]):
-            curvature_matrix[j, i] = curvature_matrix[i, j]
+        if fit_0.inversion.total(cls=AbstractMapper) == 0:
+            return
 
-    return curvature_matrix
+        from autoarray.inversion.inversion.interferometer.lop import (
+            InversionInterferometerMappingPyLops,
+        )
 
+        if isinstance(fit_0.inversion, InversionInterferometerMappingPyLops):
+            return
 
-@numba_util.jit()
-def mapped_reconstructed_data_via_image_to_pix_unique_from(
-    data_to_pix_unique: np.ndarray,
-    data_weights: np.ndarray,
-    pix_lengths: np.ndarray,
-    reconstruction: np.ndarray,
-) -> np.ndarray:
-    """
-    Returns the reconstructed data vector from the blurred mapping matrix `f` and solution vector *S*.
+        inversion_0 = fit_0.inversion
+        inversion_1 = fit_1.inversion
 
-    Parameters
-    ----------
-    mapping_matrix
-        The matrix representing the blurred mappings between sub-grid pixels and pixelization pixels.
+        if inversion_0.mapping_matrix.shape[1] == inversion_1.mapping_matrix.shape[1]:
+            if np.allclose(inversion_0.mapping_matrix, inversion_1.mapping_matrix):
+                self.mapper_list = inversion_0.cls_list_from(cls=AbstractMapper)
+
+                logger.info(
+                    "PRELOADS - Mappers of planes preloaded for this model-fit."
+                )
+
+    def set_operated_mapping_matrix_with_preloads(self, fit_0, fit_1):
+        """
+        If the `MassProfile`'s and `Mesh`'s in a model are fixed, the mapping of image-pixels to the
+        source-pixels does not change during the model-fit and matrices used to perform the linear algebra in an
+        inversion can be preloaded, which help efficiently construct the curvature matrix.
+
+        This function compares the operated mapping matrix of two fit's corresponding to two model instances, and
+        preloads the mapper if the mapping matrix of both fits are the same.
+
+        The preload is typically used in searches where only light profiles vary (e.g. when only the lens's light is
+        being fitted for).
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
 
-    """
+        self.operated_mapping_matrix = None
 
-    data_pixels = data_to_pix_unique.shape[0]
+        from autoarray.inversion.inversion.interferometer.lop import (
+            InversionInterferometerMappingPyLops,
+        )
 
-    mapped_reconstructed_data = np.zeros(data_pixels)
+        if isinstance(fit_0.inversion, InversionInterferometerMappingPyLops):
+            return
 
-    for data_0 in range(data_pixels):
-        for pix_0 in range(pix_lengths[data_0]):
+        inversion_0 = fit_0.inversion
+        inversion_1 = fit_1.inversion
 
-            pix_for_data = data_to_pix_unique[data_0, pix_0]
+        if inversion_0 is None:
+            return
 
-            mapped_reconstructed_data[data_0] += (
-                data_weights[data_0, pix_0] * reconstruction[pix_for_data]
-            )
+        if (
+            inversion_0.operated_mapping_matrix.shape[1]
+            == inversion_1.operated_mapping_matrix.shape[1]
+        ):
+            if (
+                np.max(
+                    abs(
+                        inversion_0.operated_mapping_matrix
+                        - inversion_1.operated_mapping_matrix
+                    )
+                )
+                < 1e-8
+            ):
+                self.operated_mapping_matrix = inversion_0.operated_mapping_matrix
 
-    return mapped_reconstructed_data
+                logger.info(
+                    "PRELOADS - Inversion linear algebra quantities preloaded for this model-fit."
+                )
+
+    def set_linear_func_inversion_dicts(self, fit_0, fit_1):
+        """
+        If the `MassProfile`'s and `Mesh`'s in a model are fixed, the mapping of image-pixels to the
+        source-pixels does not change during the model-fit and matrices used to perform the linear algebra in an
+        inversion can be preloaded, which help efficiently construct the curvature matrix.
+
+        This function compares the operated mapping matrix of two fit's corresponding to two model instances, and
+        preloads the mapper if the mapping matrix of both fits are the same.
+
+        The preload is typically used in searches where only light profiles vary (e.g. when only the lens's light is
+        being fitted for).
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
+
+        self.linear_func_operated_mapping_matrix_dict = None
+
+        inversion_0 = fit_0.inversion
+        inversion_1 = fit_1.inversion
+
+        if inversion_0 is None:
+            return
+
+        if not inversion_0.has(cls=AbstractLinearObjFuncList):
+            return
+
+        try:
+            inversion_0.linear_func_operated_mapping_matrix_dict
+        except NotImplementedError:
+            return
+
+        if not hasattr(inversion_0, "linear_func_operated_mapping_matrix_dict"):
+            return
+
+        should_preload = False
+
+        for operated_mapping_matrix_0, operated_mapping_matrix_1 in zip(
+            inversion_0.linear_func_operated_mapping_matrix_dict.values(),
+            inversion_1.linear_func_operated_mapping_matrix_dict.values(),
+        ):
+            if (
+                np.max(abs(operated_mapping_matrix_0 - operated_mapping_matrix_1))
+                < 1e-8
+            ):
+                should_preload = True
 
+        if should_preload:
+            self.linear_func_operated_mapping_matrix_dict = (
+                inversion_0.linear_func_operated_mapping_matrix_dict
+            )
+            self.data_linear_func_matrix_dict = inversion_0.data_linear_func_matrix_dict
 
-@numba_util.jit()
-def mapped_reconstructed_data_via_mapping_matrix_from(
-    mapping_matrix: np.ndarray, reconstruction: np.ndarray
-) -> np.ndarray:
-    """
-    Returns the reconstructed data vector from the blurred mapping matrix `f` and solution vector *S*.
-
-    Parameters
-    ----------
-    mapping_matrix
-        The matrix representing the blurred mappings between sub-grid pixels and pixelization pixels.
-
-    """
-    mapped_reconstructed_data = np.zeros(mapping_matrix.shape[0])
-    for i in range(mapping_matrix.shape[0]):
-        for j in range(reconstruction.shape[0]):
-            mapped_reconstructed_data[i] += reconstruction[j] * mapping_matrix[i, j]
-
-    return mapped_reconstructed_data
-
-
-def reconstruction_positive_negative_from(
-    data_vector: np.ndarray,
-    curvature_reg_matrix: np.ndarray,
-    mapper_param_range_list,
-    force_check_reconstruction: bool = False,
-):
-    """
-    Solve the linear system [F + reg_coeff*H] S = D -> S = [F + reg_coeff*H]^-1 D given by equation (12)
-    of https://arxiv.org/pdf/astro-ph/0302587.pdf
-
-    S is the vector of reconstructed inversion values.
-
-    This reconstruction uses a linear algebra solver that allows for negative and positives values in the solution.
-    By allowing negative values, the solver is efficient, but there are many inference problems where negative values
-    are nonphysical or undesirable.
-
-    This function checks that the solution does not give a linear algebra error (e.g. because the input matrix is
-    not positive-definitive).
-
-    It also explicitly checks solutions where all reconstructed values go to the same value, and raises an exception if
-    this occurs. This solution occurs in many scenarios when it is clear not a valid solution, and therefore is checked
-    for and removed.
-
-    Parameters
-    ----------
-    data_vector
-        The `data_vector` D which is solved for.
-    curvature_reg_matrix
-        The sum of the curvature and regularization matrices.
-    mapper_param_range_list
-        A list of lists, where each list contains the range of values in the solution vector (reconstruction) that
-        correspond to values that are part of a mapper's mesh.
-    force_check_reconstruction
-        If `True`, the reconstruction is forced to check for solutions where all reconstructed values go to the same
-        value irrespective of the configuration file value.
-
-    Returns
-    -------
-    curvature_reg_matrix
-        The curvature_matrix plus regularization matrix, overwriting the curvature_matrix in memory.
-    """
-    try:
-        reconstruction = np.linalg.solve(curvature_reg_matrix, data_vector)
-    except np.linalg.LinAlgError as e:
-        raise exc.InversionException() from e
-
-    if (
-        conf.instance["general"]["inversion"]["check_reconstruction"]
-        or force_check_reconstruction
-    ):
+            logger.info(
+                "PRELOADS - Inversion linear light profile operated mapping matrix / data linear func matrix preloaded for this model-fit."
+            )
 
-        for mapper_param_range in mapper_param_range_list:
-            if np.allclose(
-                a=reconstruction[mapper_param_range[0] : mapper_param_range[1]],
-                b=reconstruction[mapper_param_range[0]],
+    def set_curvature_matrix(self, fit_0, fit_1):
+        """
+        If the `MassProfile`'s and `Mesh`'s in a model are fixed, the mapping of image-pixels to the
+        source-pixels does not change during the model-fit and therefore its associated curvature matrix is also
+        fixed, meaning the curvature matrix preloaded.
+
+        If linear ``LightProfiles``'s are included, the regions of the curvature matrix associatd with these
+        objects vary but the diagonals of the mapper do not change. In this case, the `curvature_matrix_mapper_diag`
+        is preloaded.
+
+        This function compares the curvature matrix of two fit's corresponding to two model instances, and preloads
+        this value if it is the same for both fits.
+
+        The preload is typically used in **PyAutoGalaxy** inversions using a `Rectangular` pixelization.
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
+
+        self.curvature_matrix = None
+        self.data_vector_mapper = None
+        self.curvature_matrix_mapper_diag = None
+        self.mapper_operated_mapping_matrix_dict = None
+
+        inversion_0 = fit_0.inversion
+        inversion_1 = fit_1.inversion
+
+        if inversion_0 is None:
+            return
+
+        try:
+            inversion_0._curvature_matrix_mapper_diag
+        except NotImplementedError:
+            return
+
+        if inversion_0.curvature_matrix.shape == inversion_1.curvature_matrix.shape:
+            if (
+                np.max(abs(inversion_0.curvature_matrix - inversion_1.curvature_matrix))
+                < 1e-8
             ):
-                raise exc.InversionException()
-
-    return reconstruction
+                self.curvature_matrix = inversion_0.curvature_matrix
 
+                logger.info(
+                    "PRELOADS - Inversion Curvature Matrix preloaded for this model-fit."
+                )
+
+                return
+
+            if inversion_0._curvature_matrix_mapper_diag is not None:
+                if (
+                    np.max(
+                        abs(
+                            inversion_0._curvature_matrix_mapper_diag
+                            - inversion_1._curvature_matrix_mapper_diag
+                        )
+                    )
+                    < 1e-8
+                ):
+                    self.mapper_operated_mapping_matrix_dict = (
+                        inversion_0.mapper_operated_mapping_matrix_dict
+                    )
+                    self.data_vector_mapper = inversion_0._data_vector_mapper
+                    self.curvature_matrix_mapper_diag = (
+                        inversion_0._curvature_matrix_mapper_diag
+                    )
+
+                    logger.info(
+                        "PRELOADS - Inversion Curvature Matrix Mapper Diag preloaded for this model-fit."
+                    )
+
+    def set_regularization_matrix_and_term(self, fit_0, fit_1):
+        """
+        If the `MassProfile`'s and `Mesh`'s in a model are fixed, the mapping of image-pixels to the
+        source-pixels does not change during the model-fit and therefore its associated regularization matrices are
+        also fixed, meaning the log determinant of the regularization matrix term of the Bayesian evidence can be
+        preloaded.
+
+        This function compares the value of the log determinant of the regularization matrix of two fit's corresponding
+        to two model instances, and preloads this value if it is the same for both fits.
+
+        The preload is typically used in searches where only light profiles vary (e.g. when only the lens's light is
+        being fitted for).
+
+        Parameters
+        ----------
+        fit_0
+            The first fit corresponding to a model with a specific set of unit-values.
+        fit_1
+            The second fit corresponding to a model with a different set of unit-values.
+        """
+        self.regularization_matrix = None
+        self.log_det_regularization_matrix_term = None
+
+        inversion_0 = fit_0.inversion
+        inversion_1 = fit_1.inversion
+
+        if inversion_0 is None:
+            return
+
+        if inversion_0.total(cls=AbstractMapper) == 0:
+            return
+
+        if (
+            abs(
+                inversion_0.log_det_regularization_matrix_term
+                - inversion_1.log_det_regularization_matrix_term
+            )
+            < 1e-8
+        ):
+            self.regularization_matrix = inversion_0.regularization_matrix
+            self.log_det_regularization_matrix_term = (
+                inversion_0.log_det_regularization_matrix_term
+            )
 
-def reconstruction_positive_only_from(
-    data_vector: np.ndarray,
-    curvature_reg_matrix: np.ndarray,
-    settings: SettingsInversion = SettingsInversion(),
-):
-    """
-    Solve the linear system [F + reg_coeff*H] S = D -> S = [F + reg_coeff*H]^-1 D given by equation (12)
-    of https://arxiv.org/pdf/astro-ph/0302587.pdf
-
-    S is the vector of reconstructed inversion values.
-
-    This reconstruction uses a linear algebra solver that allows only positives values in the solution.
-    By not allowing negative values, the solver is slower than methods which allow negative values, but there are
-    many inference problems where negative values are nonphysical or undesirable and removing them improves the solution.
-
-    This function checks that the solution does not give a linear algebra error (e.g. because the input matrix is
-    not positive-definitive) and that it avoids solutions where all reconstructed values go to the same value. If these
-    occur it raises an exception.
-
-    Parameters
-    ----------
-    data_vector
-        The `data_vector` D which is solved for.
-    curvature_reg_matrix
-        The sum of the curvature and regularization matrices.
-    settings
-        Controls the settings of the inversion, for this function where the solution is checked to not be all
-        the same values.
-
-    Returns
-    -------
-    curvature_reg_matrix
-        The curvature_matrix plus regularization matrix, overwriting the curvature_matrix in memory.
-    """
-
-    try:
-
-        reconstruction = nnls(
-            curvature_reg_matrix,
-            (data_vector).T,
-            maxiter=settings.positive_only_maxiter,
-        )[0]
-
-    except (RuntimeError, np.linalg.LinAlgError) as e:
-        raise exc.InversionException() from e
-
-    return reconstruction
-
-
-def preconditioner_matrix_via_mapping_matrix_from(
-    mapping_matrix: np.ndarray,
-    regularization_matrix: np.ndarray,
-    preconditioner_noise_normalization: float,
-) -> np.ndarray:
-    """
-    Returns the preconditioner matrix `{` from a mapping matrix `f` and the sum of the inverse of the 1D noise-map
-    values squared (see Powell et al. 2020).
-
-    Parameters
-    ----------
-    mapping_matrix
-        The matrix representing the mappings between sub-grid pixels and pixelization pixels.
-    regularization_matrix
-        The matrix defining how the pixelization's pixels are regularized with one another for smoothing (H).
-    preconditioner_noise_normalization
-        The sum of (1.0 / noise-map**2.0) every value in the noise-map.
-    """
-
-    curvature_matrix = curvature_matrix_via_mapping_matrix_from(
-        mapping_matrix=mapping_matrix,
-        noise_map=np.ones(shape=(mapping_matrix.shape[0])),
-    )
-
-    return (
-        preconditioner_noise_normalization * curvature_matrix
-    ) + regularization_matrix
-
-
-def inversion_residual_map_from(
-    *,
-    reconstruction: np.ndarray,
-    data: np.ndarray,
-    slim_index_for_sub_slim_index: np.ndarray,
-    sub_slim_indexes_for_pix_index: [list],
-):
-    """
-    Returns the residual-map of the `reconstruction` of an `Inversion` on its pixel-grid.
-
-    For this residual-map, each pixel on the `reconstruction`'s pixel-grid corresponds to the sum of absolute residual
-    values in the `residual_map` of the reconstructed `data` divided by the number of data-points that it maps too,
-    (to normalize its value).
-
-    This provides information on where in the `Inversion`'s `reconstruction` it is least able to accurately fit the
-    `data`.
-
-    Parameters
-    ----------
-    reconstruction
-        The values computed by the `Inversion` for the `reconstruction`, which are used in this function to compute
-        the `residual_map` values.
-    data
-        The array of `data` that the `Inversion` fits.
-    slim_index_for_sub_slim_index
-        The mappings between the observed grid's sub-pixels and observed grid's pixels.
-    sub_slim_indexes_for_pix_index
-        The mapping of every pixel on the `LinearEqn`'s `reconstruction`'s pixel-grid to the `data` pixels.
-
-    Returns
-    -------
-    np.ndarray
-        The residuals of the `Inversion`'s `reconstruction` on its pixel-grid, computed by mapping the `residual_map`
-        from the fit to the data.
-    """
-    residual_map = np.zeros(shape=len(sub_slim_indexes_for_pix_index))
-
-    for pix_index, sub_slim_indexes in enumerate(sub_slim_indexes_for_pix_index):
-
-        sub_mask_total = 0
-        for sub_mask_1d_index in sub_slim_indexes:
-            sub_mask_total += 1
-            mask_1d_index = slim_index_for_sub_slim_index[sub_mask_1d_index]
-            residual = data[mask_1d_index] - reconstruction[pix_index]
-            residual_map[pix_index] += np.abs(residual)
-
-        if sub_mask_total > 0:
-            residual_map[pix_index] /= sub_mask_total
-
-    return residual_map.copy()
-
-
-def inversion_normalized_residual_map_from(
-    *,
-    reconstruction,
-    data,
-    noise_map_1d,
-    slim_index_for_sub_slim_index,
-    sub_slim_indexes_for_pix_index,
-):
-    """
-    Returns the normalized residual-map of the `reconstruction` of an `Inversion` on its pixel-grid.
-
-    For this normalized residual-map, each pixel on the `reconstruction`'s pixel-grid corresponds to the sum of
-    absolute normalized residual values in the `normalized residual_map` of the reconstructed `data` divided by the
-    number of data-points that it maps too (to normalize its value).
-
-    This provides information on where in the `Inversion`'s `reconstruction` it is least able to accurately fit the
-    `data`.
-
-    Parameters
-    ----------
-    reconstruction
-        The values computed by the `Inversion` for the `reconstruction`, which are used in this function to compute
-        the `normalized residual_map` values.
-    data
-        The array of `data` that the `Inversion` fits.
-    slim_index_for_sub_slim_index
-        The mappings between the observed grid's sub-pixels and observed grid's pixels.
-    sub_slim_indexes_for_pix_index
-        The mapping of every pixel on the `LinearEqn`'s `reconstruction`'s pixel-grid to the `data` pixels.
-
-    Returns
-    -------
-    np.ndarray
-        The normalized residuals of the `Inversion`'s `reconstruction` on its pixel-grid, computed by mapping the
-        `normalized_residual_map` from the fit to the data.
-    """
-    normalized_residual_map = np.zeros(shape=len(sub_slim_indexes_for_pix_index))
-
-    for pix_index, sub_slim_indexes in enumerate(sub_slim_indexes_for_pix_index):
-        sub_mask_total = 0
-        for sub_mask_1d_index in sub_slim_indexes:
-            sub_mask_total += 1
-            mask_1d_index = slim_index_for_sub_slim_index[sub_mask_1d_index]
-            residual = data[mask_1d_index] - reconstruction[pix_index]
-            normalized_residual_map[pix_index] += np.abs(
-                (residual / noise_map_1d[mask_1d_index])
+            logger.info(
+                "PRELOADS - Inversion Log Det Regularization Matrix Term preloaded for this model-fit."
             )
 
-        if sub_mask_total > 0:
-            normalized_residual_map[pix_index] /= sub_mask_total
+    def check_via_fit(self, fit):
+        import copy
+
+        settings_inversion = copy.deepcopy(fit.settings_inversion)
 
-    return normalized_residual_map.copy()
+        fit_with_preloads = fit.refit_with_new_preloads(
+            preloads=self, settings_inversion=settings_inversion
+        )
+
+        fit_without_preloads = fit.refit_with_new_preloads(
+            preloads=self.__class__(use_w_tilde=False),
+            settings_inversion=settings_inversion,
+        )
 
+        try:
+            if (
+                abs(
+                    fit_with_preloads.figure_of_merit
+                    - fit_without_preloads.figure_of_merit
+                )
+                > self.check_threshold
+            ):
+                raise exc.PreloadsException(
+                    f"""
+                    The log likelihood of fits using and not using preloads are not consistent by a value larger than
+                    the preloads check threshold of {self.check_threshold}, indicating preloading has gone wrong.
+
+                    The likelihood values are: 
+
+                    With Preloads: {fit_with_preloads.figure_of_merit}
+                    Without Preloads: {fit_without_preloads.figure_of_merit}
+                    
+                    Double check that the model-fit is set up correctly and that the preloads are being used correctly.
+                    
+                    This exception can be turned off by setting the general.yaml -> test -> check_preloads to False
+                    in the config files. However, care should be taken when doing this.
+                    """
+                )
+
+        except exc.InversionException:
+            data_vector_difference = np.max(
+                np.abs(
+                    fit_with_preloads.inversion.data_vector
+                    - fit_without_preloads.inversion.data_vector
+                )
+            )
 
-def inversion_chi_squared_map_from(
-    *,
-    reconstruction,
-    data,
-    noise_map_1d,
-    slim_index_for_sub_slim_index,
-    sub_slim_indexes_for_pix_index,
-):
-    """
-    Returns the chi-squared-map of the `reconstruction` of an `Inversion` on its pixel-grid.
-
-    For this chi-squared-map, each pixel on the `reconstruction`'s pixel-grid corresponds to the sum of chi-squared
-    values in the `chi_squared_map` of the reconstructed `data` divided by the number of data-points that it maps too,
-    (to normalize its value).
-
-    This provides information on where in the `Inversion`'s `reconstruction` it is least able to accurately fit the
-    `data`.
-
-    Parameters
-    ----------
-    reconstruction
-        The values computed by the `Inversion` for the `reconstruction`, which are used in this function to compute
-        the `chi_squared_map` values.
-    data
-        The array of `data` that the `Inversion` fits.
-    slim_index_for_sub_slim_index
-        The mappings between the observed grid's sub-pixels and observed grid's pixels.
-    sub_slim_indexes_for_pix_index
-        The mapping of every pixel on the `LinearEqn`'s `reconstruction`'s pixel-grid to the `data` pixels.
-
-    Returns
-    -------
-    np.ndarray
-        The chi-squareds of the `Inversion`'s `reconstruction` on its pixel-grid, computed by mapping the `chi-squared_map`
-        from the fit to the data.
-    """
-    chi_squared_map = np.zeros(shape=len(sub_slim_indexes_for_pix_index))
-
-    for pix_index, sub_slim_indexes in enumerate(sub_slim_indexes_for_pix_index):
-        sub_mask_total = 0
-        for sub_mask_1d_index in sub_slim_indexes:
-            sub_mask_total += 1
-            mask_1d_index = slim_index_for_sub_slim_index[sub_mask_1d_index]
-            residual = data[mask_1d_index] - reconstruction[pix_index]
-            chi_squared_map[pix_index] += (
-                residual / noise_map_1d[mask_1d_index]
-            ) ** 2.0
+            if data_vector_difference > 1.0e-4:
+                raise exc.PreloadsException(
+                    f"""
+                    The data vectors of fits using and not using preloads are not consistent, indicating 
+                    preloading has gone wrong.
+
+                    The maximum value a data vector absolute value difference is: {data_vector_difference} 
+                    """
+                )
+
+            curvature_reg_matrix_difference = np.max(
+                np.abs(
+                    fit_with_preloads.inversion.curvature_reg_matrix
+                    - fit_without_preloads.inversion.curvature_reg_matrix
+                )
+            )
 
-        if sub_mask_total > 0:
-            chi_squared_map[pix_index] /= sub_mask_total
+            if curvature_reg_matrix_difference > 1.0e-4:
+                raise exc.PreloadsException(
+                    f"""
+                    The curvature matrices of fits using and not using preloads are not consistent, indicating 
+                    preloading has gone wrong.
+
+                    The maximum value of a curvature matrix absolute value difference is: {curvature_reg_matrix_difference} 
+                    """
+                )
+
+    @property
+    def info(self) -> List[str]:
+        """
+        The information on what has or has not been preloaded, which is written to the file `preloads.summary`.
+
+        Returns
+        -------
+            A list of strings containing statements on what has or has not been preloaded.
+        """
+        line = [f"W Tilde = {self.w_tilde is not None}\n"]
+        line += [f"Relocated Grid = {self.relocated_grid is not None}\n"]
+        line += [f"Mapper = {self.mapper_list is not None}\n"]
+        line += [
+            f"Blurred Mapping Matrix = {self.operated_mapping_matrix is not None}\n"
+        ]
+        line += [
+            f"Inversion Linear Func (Linear Light Profile) Dicts = {self.linear_func_operated_mapping_matrix_dict is not None}\n"
+        ]
+        line += [f"Curvature Matrix = {self.curvature_matrix is not None}\n"]
+        line += [
+            f"Curvature Matrix Mapper Diag = {self.curvature_matrix_mapper_diag is not None}\n"
+        ]
+        line += [f"Regularization Matrix = {self.regularization_matrix is not None}\n"]
+        line += [
+            f"Log Det Regularization Matrix Term = {self.log_det_regularization_matrix_term is not None}\n"
+        ]
 
-    return chi_squared_map.copy()
+        return line
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/inversion_util_secret.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,22 +54,20 @@
     image_pixels = len(native_index_for_slim_index)
 
     w_tilde_data = np.zeros(image_pixels)
 
     weight_map_real = visibilities_real / noise_map_real**2.0
 
     for ip0 in range(image_pixels):
-
         value = 0.0
 
         y = grid_radians_slim[ip0, 1]
         x = grid_radians_slim[ip0, 0]
 
         for vis_1d_index in range(uv_wavelengths.shape[0]):
-
             value += weight_map_real[vis_1d_index] ** -2.0 * np.cos(
                 2.0
                 * np.pi
                 * (
                     y * uv_wavelengths[vis_1d_index, 0]
                     + x * uv_wavelengths[vis_1d_index, 1]
                 )
@@ -115,20 +113,18 @@
         matrix.
     """
 
     w_tilde = np.zeros((grid_radians_slim.shape[0], grid_radians_slim.shape[0]))
 
     for i in range(w_tilde.shape[0]):
         for j in range(i, w_tilde.shape[1]):
-
             y_offset = grid_radians_slim[i, 1] - grid_radians_slim[j, 1]
             x_offset = grid_radians_slim[i, 0] - grid_radians_slim[j, 0]
 
             for vis_1d_index in range(uv_wavelengths.shape[0]):
-
                 w_tilde[i, j] += noise_map_real[vis_1d_index] ** -2.0 * np.cos(
                     2.0
                     * np.pi
                     * (
                         y_offset * uv_wavelengths[vis_1d_index, 0]
                         + x_offset * uv_wavelengths[vis_1d_index, 1]
                     )
@@ -193,15 +189,15 @@
     - The value precomputed for pixel pair [0,3] is the same as pixel pairs [1,4], [2,5], [3,6], [4,7] and [5,8].
     - The values of pixels paired with themselves are also computed repeatedly for the standard calculation (e.g. 9
     times using the mask above).
     The `w_tilde_preload` method instead only computes each value once. To do this, it stores the preload values in a
     matrix of dimensions [shape_masked_pixels_y, shape_masked_pixels_x, 2], where `shape_masked_pixels` is the (y,x)
     size of the vertical and horizontal extent of unmasked pixels, e.g. the spatial extent over which the real space
     grid extends.
-    Each entry in the matrix `w_tilde_preload[:,:,0]` provides the the precomputed NUFFT value mapping an image pixel
+    Each entry in the matrix `w_tilde_preload[:,:,0]` provides the precomputed NUFFT value mapping an image pixel
     to a pixel offset by that much in the y and x directions, for example:
     - w_tilde_preload[0,0,0] gives the precomputed values of image pixels that are offset in the y direction by 0 and
     in the x direction by 0 - the values of pixels paired with themselves.
     - w_tilde_preload[1,0,0] gives the precomputed values of image pixels that are offset in the y direction by 1 and
     in the x direction by 0 - the values of pixel pairs [0,3], [1,4], [2,5], [3,6], [4,7] and [5,8]
     - w_tilde_preload[0,1,0] gives the precomputed values of image pixels that are offset in the y direction by 0 and
     in the x direction by 1 - the values of pixel pairs [0,1], [1,2], [3,4], [4,5], [6,7] and [7,9].
@@ -238,15 +234,14 @@
     grid_radians_2d = grid_radians_2d[0:y_shape, 0:x_shape]
 
     grid_y_shape = grid_radians_2d.shape[0]
     grid_x_shape = grid_radians_2d.shape[1]
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             y_offset = grid_radians_2d[0, 0, 0] - grid_radians_2d[i, j, 0]
             x_offset = grid_radians_2d[0, 0, 1] - grid_radians_2d[i, j, 1]
 
             for vis_1d_index in range(uv_wavelengths.shape[0]):
                 curvature_preload[i, j] += noise_map_real[
                     vis_1d_index
                 ] ** -2.0 * np.cos(
@@ -256,17 +251,15 @@
                         x_offset * uv_wavelengths[vis_1d_index, 0]
                         + y_offset * uv_wavelengths[vis_1d_index, 1]
                     )
                 )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if j > 0:
-
                 y_offset = (
                     grid_radians_2d[0, -1, 0]
                     - grid_radians_2d[i, grid_x_shape - j - 1, 0]
                 )
                 x_offset = (
                     grid_radians_2d[0, -1, 1]
                     - grid_radians_2d[i, grid_x_shape - j - 1, 1]
@@ -282,17 +275,15 @@
                             x_offset * uv_wavelengths[vis_1d_index, 0]
                             + y_offset * uv_wavelengths[vis_1d_index, 1]
                         )
                     )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if i > 0:
-
                 y_offset = (
                     grid_radians_2d[-1, 0, 0]
                     - grid_radians_2d[grid_y_shape - i - 1, j, 0]
                 )
                 x_offset = (
                     grid_radians_2d[-1, 0, 1]
                     - grid_radians_2d[grid_y_shape - i - 1, j, 1]
@@ -308,17 +299,15 @@
                             x_offset * uv_wavelengths[vis_1d_index, 0]
                             + y_offset * uv_wavelengths[vis_1d_index, 1]
                         )
                     )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if i > 0 and j > 0:
-
                 y_offset = (
                     grid_radians_2d[-1, -1, 0]
                     - grid_radians_2d[grid_y_shape - i - 1, grid_x_shape - j - 1, 0]
                 )
                 x_offset = (
                     grid_radians_2d[-1, -1, 1]
                     - grid_radians_2d[grid_y_shape - i - 1, grid_x_shape - j - 1, 1]
@@ -361,19 +350,17 @@
     """
 
     slim_size = len(native_index_for_slim_index)
 
     w_tilde_via_preload = np.zeros((slim_size, slim_size))
 
     for i in range(slim_size):
-
         i_y, i_x = native_index_for_slim_index[i]
 
         for j in range(i, slim_size):
-
             j_y, j_x = native_index_for_slim_index[j]
 
             y_diff = j_y - i_y
             x_diff = j_x - i_x
 
             w_tilde_via_preload[i, j] = w_tilde_preload[y_diff, x_diff]
 
@@ -437,29 +424,25 @@
     preload = curvature_preload[0, 0]
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     image_pixels = len(native_index_for_slim_index)
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         for ip0_pix in range(pix_size_for_sub_slim_index[ip0]):
-
             sp0 = pix_indexes_for_sub_slim_index[ip0, ip0_pix]
 
             ip0_weight = pix_weights_for_sub_slim_index[ip0, ip0_pix]
 
             for ip1 in range(ip0 + 1, image_pixels):
-
                 ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
                 for ip1_pix in range(pix_size_for_sub_slim_index[ip1]):
-
                     sp1 = pix_indexes_for_sub_slim_index[ip1, ip1_pix]
 
                     ip1_weight = pix_weights_for_sub_slim_index[ip1, ip1_pix]
 
                     y_diff = ip1_y - ip0_y
                     x_diff = ip1_x - ip0_x
 
@@ -472,33 +455,28 @@
     for i in range(pix_pixels):
         for j in range(pix_pixels):
             curvature_matrix_new[i, j] = curvature_matrix[i, j] + curvature_matrix[j, i]
 
     curvature_matrix = curvature_matrix_new
 
     for ip0 in range(image_pixels):
-
         for ip0_pix in range(pix_size_for_sub_slim_index[ip0]):
-
             for ip1_pix in range(pix_size_for_sub_slim_index[ip0]):
-
                 sp0 = pix_indexes_for_sub_slim_index[ip0, ip0_pix]
                 sp1 = pix_indexes_for_sub_slim_index[ip0, ip1_pix]
 
                 ip0_weight = pix_weights_for_sub_slim_index[ip0, ip0_pix]
                 ip1_weight = pix_weights_for_sub_slim_index[ip0, ip1_pix]
 
                 if sp0 > sp1:
-
                     curvature_matrix[sp0, sp1] += preload * ip0_weight * ip1_weight
 
                     curvature_matrix[sp1, sp0] += preload * ip0_weight * ip1_weight
 
                 elif sp0 == sp1:
-
                     curvature_matrix[sp0, sp1] += preload * ip0_weight * ip1_weight
 
     return curvature_matrix
 
 
 @numba_util.jit()
 def curvature_matrix_via_w_tilde_curvature_preload_interferometer_from_1(
@@ -550,25 +528,22 @@
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     image_pixels = len(native_index_for_slim_index)
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         for ip0_pix in range(pix_size_for_sub_slim_index[ip0]):
-
             sp0 = pix_indexes_for_sub_slim_index[ip0, ip0_pix]
 
             ip0_weight = pix_weights_for_sub_slim_index[ip0, ip0_pix]
 
             for ip1 in range(image_pixels):
-
                 ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
                 for ip1_pix in range(pix_size_for_sub_slim_index[ip1]):
                     sp1 = pix_indexes_for_sub_slim_index[ip1, ip1_pix]
 
                     ip1_weight = pix_weights_for_sub_slim_index[ip1, ip1_pix]
 
@@ -630,29 +605,27 @@
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     image_pixels = len(native_index_for_slim_index)
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         # This would be used to create multiple source pixels (e.g. sp0 -> sp2) with interpolation.
 
         sp0 = pix_indexes_for_sub_slim_index[
             ip0, 0
         ]  # <- This 0 would iterate over all image-pixel-to-source-pixel interpolations.
 
         # This would have weights 0.0 -> 1.0 for interpolation.
 
         ip0_weight = 1.0
 
         for ip1 in range(image_pixels):
-
             ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
             # Same arrays for interpolation case
 
             sp1 = pix_indexes_for_sub_slim_index[ip1, 0]
             ip1_weight = 1.0
 
@@ -714,24 +687,21 @@
     ndarray
         The curvature matrix `F` (see Warren & Dye 2003).
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     for sp0 in range(pix_pixels):
-
         ip_size_0 = sub_slim_sizes_for_pix_index[sp0]
 
         for sp1 in range(sp0, pix_pixels):
-
             val = 0.0
             ip_size_1 = sub_slim_sizes_for_pix_index[sp1]
 
             for ip0_tmp in range(ip_size_0):
-
                 ip0 = sub_slim_indexes_for_pix_index[sp0, ip0_tmp]
                 ip0_weight = sub_slim_weights_for_pix_index[sp0, ip0_tmp]
 
                 ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
                 for ip1_tmp in range(ip_size_1):
                     ip1 = sub_slim_indexes_for_pix_index[sp1, ip1_tmp]
@@ -801,17 +771,15 @@
     ndarray
         The curvature matrix `F` (see Warren & Dye 2003).
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     for sp0 in range(pix_pixels):
-
         for sp1 in range(sp0, pix_pixels):
-
             val = 0.0
 
             ip0 = sub_slim_indexes_for_pix_index[sp0, 0]
             ip0_weight = sub_slim_weights_for_pix_index[sp0, 0]
 
             ip0_y, ip0_x = native_index_for_slim_index[ip0]
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/inversion/inversion_util_secret_clean.py` & `autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret_clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,20 @@
     image_pixels = len(native_index_for_slim_index)
 
     w_tilde_data = np.zeros(image_pixels)
 
     weight_map_real = visibilities_real / noise_map_real**2.0
 
     for ip0 in range(image_pixels):
-
         value = 0.0
 
         y = grid_radians_slim[ip0, 1]
         x = grid_radians_slim[ip0, 0]
 
         for vis_1d_index in range(uv_wavelengths.shape[0]):
-
             value += weight_map_real[vis_1d_index] ** -2.0 * np.cos(
                 2.0
                 * np.pi
                 * (
                     y * uv_wavelengths[vis_1d_index, 0]
                     + x * uv_wavelengths[vis_1d_index, 1]
                 )
@@ -133,15 +131,15 @@
     - The values of pixels paired with themselves are also computed repeatedly for the standard calculation (e.g. 9
       times using the mask above).
 
     The `w_tilde_preload` method instead only computes each value once. To do this, it stores the preload values in a
     matrix of dimensions [shape_masked_pixels_y, shape_masked_pixels_x, 2], where `shape_masked_pixels` is the (y,x)
     size of the vertical and horizontal extent of unmasked pixels, e.g. the spatial extent over which the real space
     grid extends.
-    Each entry in the matrix `w_tilde_preload[:,:,0]` provides the the precomputed NUFFT value mapping an image pixel
+    Each entry in the matrix `w_tilde_preload[:,:,0]` provides the precomputed NUFFT value mapping an image pixel
     to a pixel offset by that much in the y and x directions, for example:
 
     - w_tilde_preload[0,0,0] gives the precomputed values of image pixels that are offset in the y direction by 0 and
       in the x direction by 0 - the values of pixels paired with themselves.
 
     - w_tilde_preload[1,0,0] gives the precomputed values of image pixels that are offset in the y direction by 1 and
       in the x direction by 0 - the values of pixel pairs [0,3], [1,4], [2,5], [3,6], [4,7] and [5,8]
@@ -184,15 +182,14 @@
     grid_radians_2d = grid_radians_2d[0:y_shape, 0:x_shape]
 
     grid_y_shape = grid_radians_2d.shape[0]
     grid_x_shape = grid_radians_2d.shape[1]
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             y_offset = grid_radians_2d[0, 0, 0] - grid_radians_2d[i, j, 0]
             x_offset = grid_radians_2d[0, 0, 1] - grid_radians_2d[i, j, 1]
 
             for vis_1d_index in range(uv_wavelengths.shape[0]):
                 curvature_preload[i, j] += noise_map_real[
                     vis_1d_index
                 ] ** -2.0 * np.cos(
@@ -202,17 +199,15 @@
                         x_offset * uv_wavelengths[vis_1d_index, 0]
                         + y_offset * uv_wavelengths[vis_1d_index, 1]
                     )
                 )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if j > 0:
-
                 y_offset = (
                     grid_radians_2d[0, -1, 0]
                     - grid_radians_2d[i, grid_x_shape - j - 1, 0]
                 )
                 x_offset = (
                     grid_radians_2d[0, -1, 1]
                     - grid_radians_2d[i, grid_x_shape - j - 1, 1]
@@ -228,17 +223,15 @@
                             x_offset * uv_wavelengths[vis_1d_index, 0]
                             + y_offset * uv_wavelengths[vis_1d_index, 1]
                         )
                     )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if i > 0:
-
                 y_offset = (
                     grid_radians_2d[-1, 0, 0]
                     - grid_radians_2d[grid_y_shape - i - 1, j, 0]
                 )
                 x_offset = (
                     grid_radians_2d[-1, 0, 1]
                     - grid_radians_2d[grid_y_shape - i - 1, j, 1]
@@ -254,17 +247,15 @@
                             x_offset * uv_wavelengths[vis_1d_index, 0]
                             + y_offset * uv_wavelengths[vis_1d_index, 1]
                         )
                     )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if i > 0 and j > 0:
-
                 y_offset = (
                     grid_radians_2d[-1, -1, 0]
                     - grid_radians_2d[grid_y_shape - i - 1, grid_x_shape - j - 1, 0]
                 )
                 x_offset = (
                     grid_radians_2d[-1, -1, 1]
                     - grid_radians_2d[grid_y_shape - i - 1, grid_x_shape - j - 1, 1]
@@ -347,15 +338,15 @@
     times using the mask above).
 
     The `w_tilde_preload` method instead only computes each value once. To do this, it stores the preload values in a
     matrix of dimensions [shape_masked_pixels_y, shape_masked_pixels_x, 2], where `shape_masked_pixels` is the (y,x)
     size of the vertical and horizontal extent of unmasked pixels, e.g. the spatial extent over which the real space
     grid extends.
 
-    Each entry in the matrix `w_tilde_preload[:,:,0]` provides the the precomputed NUFFT value mapping an image pixel
+    Each entry in the matrix `w_tilde_preload[:,:,0]` provides the precomputed NUFFT value mapping an image pixel
     to a pixel offset by that much in the y and x directions, for example:
 
     - w_tilde_preload[0,0,0] gives the precomputed values of image pixels that are offset in the y direction by 0 and
     in the x direction by 0 - the values of pixels paired with themselves.
     - w_tilde_preload[1,0,0] gives the precomputed values of image pixels that are offset in the y direction by 1 and
     in the x direction by 0 - the values of pixel pairs [0,3], [1,4], [2,5], [3,6], [4,7] and [5,8]
     - w_tilde_preload[0,1,0] gives the precomputed values of image pixels that are offset in the y direction by 0 and
@@ -397,15 +388,14 @@
     grid_radians_2d = grid_radians_2d[0:y_shape, 0:x_shape]
 
     grid_y_shape = grid_radians_2d.shape[0]
     grid_x_shape = grid_radians_2d.shape[1]
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             y_offset = grid_radians_2d[0, 0, 0] - grid_radians_2d[i, j, 0]
             x_offset = grid_radians_2d[0, 0, 1] - grid_radians_2d[i, j, 1]
 
             for vis_1d_index in range(uv_wavelengths.shape[0]):
                 curvature_preload[i, j] += noise_map_real[
                     vis_1d_index
                 ] ** -2.0 * np.cos(
@@ -415,17 +405,15 @@
                         x_offset * uv_wavelengths[vis_1d_index, 0]
                         + y_offset * uv_wavelengths[vis_1d_index, 1]
                     )
                 )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if j > 0:
-
                 y_offset = (
                     grid_radians_2d[0, -1, 0]
                     - grid_radians_2d[i, grid_x_shape - j - 1, 0]
                 )
                 x_offset = (
                     grid_radians_2d[0, -1, 1]
                     - grid_radians_2d[i, grid_x_shape - j - 1, 1]
@@ -441,17 +429,15 @@
                             x_offset * uv_wavelengths[vis_1d_index, 0]
                             + y_offset * uv_wavelengths[vis_1d_index, 1]
                         )
                     )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if i > 0:
-
                 y_offset = (
                     grid_radians_2d[-1, 0, 0]
                     - grid_radians_2d[grid_y_shape - i - 1, j, 0]
                 )
                 x_offset = (
                     grid_radians_2d[-1, 0, 1]
                     - grid_radians_2d[grid_y_shape - i - 1, j, 1]
@@ -467,17 +453,15 @@
                             x_offset * uv_wavelengths[vis_1d_index, 0]
                             + y_offset * uv_wavelengths[vis_1d_index, 1]
                         )
                     )
 
     for i in range(y_shape):
         for j in range(x_shape):
-
             if i > 0 and j > 0:
-
                 y_offset = (
                     grid_radians_2d[-1, -1, 0]
                     - grid_radians_2d[grid_y_shape - i - 1, grid_x_shape - j - 1, 0]
                 )
                 x_offset = (
                     grid_radians_2d[-1, -1, 1]
                     - grid_radians_2d[grid_y_shape - i - 1, grid_x_shape - j - 1, 1]
@@ -520,19 +504,17 @@
     """
 
     slim_size = len(native_index_for_slim_index)
 
     w_tilde_via_preload = np.zeros((slim_size, slim_size))
 
     for i in range(slim_size):
-
         i_y, i_x = native_index_for_slim_index[i]
 
         for j in range(i, slim_size):
-
             j_y, j_x = native_index_for_slim_index[j]
 
             y_diff = j_y - i_y
             x_diff = j_x - i_x
 
             w_tilde_via_preload[i, j] = w_tilde_preload[y_diff, x_diff]
 
@@ -595,29 +577,25 @@
     preload = curvature_preload[0, 0]
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     image_pixels = len(native_index_for_slim_index)
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         for ip0_pix in range(pix_size_for_sub_slim_index[ip0]):
-
             sp0 = pix_indexes_for_sub_slim_index[ip0, ip0_pix]
 
             ip0_weight = pix_weights_for_sub_slim_index[ip0, ip0_pix]
 
             for ip1 in range(ip0 + 1, image_pixels):
-
                 ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
                 for ip1_pix in range(pix_size_for_sub_slim_index[ip1]):
-
                     sp1 = pix_indexes_for_sub_slim_index[ip1, ip1_pix]
 
                     ip1_weight = pix_weights_for_sub_slim_index[ip1, ip1_pix]
 
                     y_diff = ip1_y - ip0_y
                     x_diff = ip1_x - ip0_x
 
@@ -630,33 +608,28 @@
     for i in range(pix_pixels):
         for j in range(pix_pixels):
             curvature_matrix_new[i, j] = curvature_matrix[i, j] + curvature_matrix[j, i]
 
     curvature_matrix = curvature_matrix_new
 
     for ip0 in range(image_pixels):
-
         for ip0_pix in range(pix_size_for_sub_slim_index[ip0]):
-
             for ip1_pix in range(pix_size_for_sub_slim_index[ip0]):
-
                 sp0 = pix_indexes_for_sub_slim_index[ip0, ip0_pix]
                 sp1 = pix_indexes_for_sub_slim_index[ip0, ip1_pix]
 
                 ip0_weight = pix_weights_for_sub_slim_index[ip0, ip0_pix]
                 ip1_weight = pix_weights_for_sub_slim_index[ip0, ip1_pix]
 
                 if sp0 > sp1:
-
                     curvature_matrix[sp0, sp1] += preload * ip0_weight * ip1_weight
 
                     curvature_matrix[sp1, sp0] += preload * ip0_weight * ip1_weight
 
                 elif sp0 == sp1:
-
                     curvature_matrix[sp0, sp1] += preload * ip0_weight * ip1_weight
 
     return curvature_matrix
 
 
 @numba_util.jit()
 def curvature_matrix_via_w_tilde_curvature_preload_interferometer_from_1(
@@ -708,25 +681,22 @@
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     image_pixels = len(native_index_for_slim_index)
 
     for ip0 in range(image_pixels):
-
         ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
         for ip0_pix in range(pix_size_for_sub_slim_index[ip0]):
-
             sp0 = pix_indexes_for_sub_slim_index[ip0, ip0_pix]
 
             ip0_weight = pix_weights_for_sub_slim_index[ip0, ip0_pix]
 
             for ip1 in range(image_pixels):
-
                 ip1_y, ip1_x = native_index_for_slim_index[ip1]
 
                 for ip1_pix in range(pix_size_for_sub_slim_index[ip1]):
                     sp1 = pix_indexes_for_sub_slim_index[ip1, ip1_pix]
 
                     ip1_weight = pix_weights_for_sub_slim_index[ip1, ip1_pix]
 
@@ -788,24 +758,21 @@
     ndarray
         The curvature matrix `F` (see Warren & Dye 2003).
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     for sp0 in range(pix_pixels):
-
         ip_size_0 = sub_slim_sizes_for_pix_index[sp0]
 
         for sp1 in range(sp0, pix_pixels):
-
             val = 0.0
             ip_size_1 = sub_slim_sizes_for_pix_index[sp1]
 
             for ip0_tmp in range(ip_size_0):
-
                 ip0 = sub_slim_indexes_for_pix_index[sp0, ip0_tmp]
                 ip0_weight = sub_slim_weights_for_pix_index[sp0, ip0_tmp]
 
                 ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
                 for ip1_tmp in range(ip_size_1):
                     ip1 = sub_slim_indexes_for_pix_index[sp1, ip1_tmp]
@@ -875,24 +842,21 @@
     ndarray
         The curvature matrix `F` (see Warren & Dye 2003).
     """
 
     curvature_matrix = np.zeros((pix_pixels, pix_pixels))
 
     for sp0 in range(pix_pixels):
-
         ip_size_0 = sub_slim_sizes_for_pix_index[sp0]
 
         for sp1 in range(sp0, pix_pixels):
-
             val = 0.0
             ip_size_1 = sub_slim_sizes_for_pix_index[sp1]
 
             for ip0_tmp in range(ip_size_0):
-
                 ip0 = sub_slim_indexes_for_pix_index[sp0, ip0_tmp]
                 ip0_weight = sub_slim_weights_for_pix_index[sp0, ip0_tmp]
 
                 ip0_y, ip0_x = native_index_for_slim_index[ip0]
 
                 for ip1_tmp in range(ip_size_1):
                     ip1 = sub_slim_indexes_for_pix_index[sp1, ip1_tmp]
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/linear_obj/func_list.py` & `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/func_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
         neighbors_sizes[0] -= 1
         neighbors_sizes[-1] -= 1
 
         neighbors = -1 * np.ones(shape=(self.params, 2))
 
         for pixel_index in range(self.params):
-
             neighbors[pixel_index, 0] = pixel_index - 1
             neighbors[pixel_index, 1] = pixel_index + 1
 
         neighbors[0, 0] = 1
         neighbors[0, 1] = -1
         neighbors[-1, 1] = -1
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/linear_obj/linear_obj.py` & `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/linear_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,11 +152,10 @@
         modules.
 
         For multiple mappers, the regularization matrix is computed as the block diagonal of each individual mapper.
         The scipy function `block_diag` has an overhead associated with it and if there is only one mapper and
         regularization it is bypassed.
         """
         if self.regularization is None:
-
             return np.zeros((self.params, self.params))
 
         return self.regularization.regularization_matrix_from(linear_obj=self)
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/linear_obj/neighbors.py` & `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/neighbors.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/linear_obj/unique_mappings.py` & `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/unique_mappings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_inversion.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,62 +11,60 @@
         self,
         data=None,
         noise_map=None,
         linear_obj_list=None,
         operated_mapping_matrix=None,
         data_vector=None,
         curvature_matrix=None,
+        data_vector_mapper=None,
         curvature_matrix_mapper_diag=None,
+        mapper_operated_mapping_matrix_dict=None,
         regularization_matrix=None,
         curvature_reg_matrix=None,
         reconstruction: np.ndarray = None,
         reconstruction_dict: List[np.ndarray] = None,
         mapped_reconstructed_data_dict=None,
         mapped_reconstructed_image_dict=None,
         errors: np.ndarray = None,
         errors_dict: List[np.ndarray] = None,
         regularization_term=None,
         log_det_curvature_reg_matrix_term=None,
         log_det_regularization_matrix_term=None,
-        curvature_matrix_preload=None,
-        curvature_matrix_counts=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-
         super().__init__(
             data=data,
             noise_map=noise_map,
             linear_obj_list=linear_obj_list or [],
             settings=settings,
             preloads=preloads,
         )
 
         self._operated_mapping_matrix = operated_mapping_matrix
         self._data_vector = data_vector
         self._regularization_matrix = regularization_matrix
         self._curvature_matrix = curvature_matrix
-        self._curvature_matrix_mapper_diag = curvature_matrix_mapper_diag
+        self.__data_vector_mapper = data_vector_mapper
+        self.__curvature_matrix_mapper_diag = curvature_matrix_mapper_diag
+        self._mapper_operated_mapping_matrix_dict = mapper_operated_mapping_matrix_dict
         self._curvature_reg_matrix = curvature_reg_matrix
         self._reconstruction = reconstruction
         self._reconstruction_dict = reconstruction_dict
 
         self._mapped_reconstructed_data_dict = mapped_reconstructed_data_dict
         self._mapped_reconstructed_image_dict = mapped_reconstructed_image_dict
 
         self._errors = errors
         self._errors_dict = errors_dict
 
         self._regularization_term = regularization_term
         self._log_det_curvature_reg_matrix_term = log_det_curvature_reg_matrix_term
         self._log_det_regularization_matrix_term = log_det_regularization_matrix_term
 
-        self._curvature_matrix_preload = curvature_matrix_preload
-        self._curvature_matrix_counts = curvature_matrix_counts
-
     @property
     def operated_mapping_matrix(self) -> np.ndarray:
         if self._operated_mapping_matrix is None:
             return super().operated_mapping_matrix
 
         return self._operated_mapping_matrix
 
@@ -74,50 +72,59 @@
     def data_vector(self) -> np.ndarray:
         if self._data_vector is None:
             return super().data_vector
         return self._data_vector
 
     @property
     def regularization_matrix(self):
-
         if self._regularization_matrix is None:
             return super().regularization_matrix
 
         return self._regularization_matrix
 
     @property
     def curvature_matrix(self):
-
         if self._curvature_matrix is None:
             return super().curvature_matrix
 
         return self._curvature_matrix
 
     @property
-    def curvature_matrix_mapper_diag(self):
+    def _data_vector_mapper(self):
+        if self.__data_vector_mapper is None:
+            return super()._data_vector_mapper
+
+        return self.__data_vector_mapper
 
-        if self._curvature_matrix_mapper_diag is None:
+    @property
+    def _curvature_matrix_mapper_diag(self):
+        if self.__curvature_matrix_mapper_diag is None:
             return super()._curvature_matrix_mapper_diag
 
-        return self._curvature_matrix_mapper_diag
+        return self.__curvature_matrix_mapper_diag
+
+    @property
+    def mapper_operated_mapping_matrix_dict(self):
+        if self._mapper_operated_mapping_matrix_dict is None:
+            return super().mapper_operated_mapping_matrix_dict
+
+        return self._mapper_operated_mapping_matrix_dict
 
     @property
     def curvature_reg_matrix(self):
         return self._curvature_reg_matrix
 
     @property
     def reconstruction(self):
-
         if self._reconstruction is None:
             return super().reconstruction
         return self._reconstruction
 
     @property
     def reconstruction_dict(self):
-
         if self._reconstruction_dict is None:
             return super().reconstruction_dict
         return self._reconstruction_dict
 
     @property
     def mapped_reconstructed_data_dict(self):
         """
@@ -156,56 +163,37 @@
         if self._mapped_reconstructed_image_dict is None:
             return super().mapped_reconstructed_image_dict
 
         return self._mapped_reconstructed_image_dict
 
     @property
     def errors(self):
-
         if self._errors is None:
             return super().errors
         return self._errors
 
     @property
     def errors_dict(self):
-
         if self._errors_dict is None:
             return super().errors_dict
         return self._errors_dict
 
     @property
     def regularization_term(self):
-
         if self._regularization_term is None:
             return super().regularization_term
 
         return self._regularization_term
 
     @property
     def log_det_curvature_reg_matrix_term(self):
-
         if self._log_det_curvature_reg_matrix_term is None:
             return super().log_det_curvature_reg_matrix_term
 
         return self._log_det_curvature_reg_matrix_term
 
     @property
     def log_det_regularization_matrix_term(self):
-
         if self._log_det_regularization_matrix_term is None:
             return super().log_det_regularization_matrix_term
 
         return self._log_det_regularization_matrix_term
-
-    @property
-    def curvature_matrix_preload(self):
-        if self._curvature_matrix_preload is None:
-            return super().curvature_matrix_preload
-
-        return self._curvature_matrix_preload
-
-    @property
-    def curvature_matrix_counts(self):
-        if self._curvature_matrix_counts is None:
-            return super().curvature_matrix_counts
-
-        return self._curvature_matrix_counts
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_inversion_imaging.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_imaging.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,42 +12,33 @@
         self,
         data=None,
         noise_map=None,
         convolver=None,
         linear_obj_list=None,
         operated_mapping_matrix=None,
         linear_func_operated_mapping_matrix_dict=None,
-        linear_func_weighted_mapping_vectors_dict=None,
-        linear_func_curvature_vectors_dict=None,
-        curvature_matrix_preload=None,
-        curvature_matrix_counts=None,
+        data_linear_func_matrix_dict=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-
         super().__init__(
             data=data,
             noise_map=noise_map,
             convolver=convolver,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
         )
 
         self._operated_mapping_matrix = operated_mapping_matrix
 
         self._linear_func_operated_mapping_matrix_dict = (
             linear_func_operated_mapping_matrix_dict
         )
-        self._linear_func_weighted_mapping_vectors_dict = (
-            linear_func_weighted_mapping_vectors_dict
-        )
-        self._linear_func_curvature_vectors_dict = linear_func_curvature_vectors_dict
-        self._curvature_matrix_preload = curvature_matrix_preload
-        self._curvature_matrix_counts = curvature_matrix_counts
+        self._data_linear_func_matrix_dict = data_linear_func_matrix_dict
 
     @property
     def operated_mapping_matrix(self) -> np.ndarray:
         if self._operated_mapping_matrix is None:
             return super().operated_mapping_matrix
 
         return self._operated_mapping_matrix
@@ -56,45 +47,23 @@
     def linear_func_operated_mapping_matrix_dict(self) -> Dict:
         if self._linear_func_operated_mapping_matrix_dict is None:
             return super().linear_func_operated_mapping_matrix_dict
 
         return self._linear_func_operated_mapping_matrix_dict
 
     @property
-    def linear_func_weighted_mapping_vectors_dict(self) -> Dict:
-        if self._linear_func_weighted_mapping_vectors_dict is None:
-            return super().linear_func_weighted_mapping_vectors_dict
+    def data_linear_func_matrix_dict(self) -> Dict:
+        if self._data_linear_func_matrix_dict is None:
+            return super().data_linear_func_matrix_dict
 
-        return self._linear_func_weighted_mapping_vectors_dict
-
-    @property
-    def linear_func_curvature_vectors_dict(self) -> Dict:
-        if self._linear_func_curvature_vectors_dict is None:
-            return super().linear_func_curvature_vectors_dict
-
-        return self._linear_func_curvature_vectors_dict
-
-    @property
-    def curvature_matrix_preload(self):
-        if self._curvature_matrix_preload is None:
-            return super().curvature_matrix_preload
-
-        return self._curvature_matrix_preload
-
-    @property
-    def curvature_matrix_counts(self):
-        if self._curvature_matrix_counts is None:
-            return super().curvature_matrix_counts
-
-        return self._curvature_matrix_counts
+        return self._data_linear_func_matrix_dict
 
 
 class MockWTildeImaging:
     def check_noise_map(self, noise_map):
-
         pass
 
 
 class MockInversionImagingWTilde(InversionImagingWTilde):
     def __init__(
         self,
         data=None,
@@ -102,15 +71,14 @@
         convolver=None,
         w_tilde=None,
         linear_obj_list=None,
         curvature_matrix_mapper_diag=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-
         super().__init__(
             data=data,
             noise_map=noise_map,
             convolver=convolver,
             w_tilde=w_tilde or MockWTildeImaging(),
             linear_obj_list=linear_obj_list,
             settings=settings,
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_inversion_interferometer.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_interferometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         noise_map=None,
         transformer=None,
         linear_obj_list=None,
         operated_mapping_matrix=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-
         super().__init__(
             data=data,
             noise_map=noise_map,
             transformer=transformer,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_linear_obj.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         self,
         parameters=None,
         grid=None,
         mapping_matrix=None,
         operated_mapping_matrix_override=None,
         regularization=None,
     ):
-
         super().__init__(regularization=regularization)
 
         self.grid = grid
         self._parameters = parameters
         self._mapping_matrix = mapping_matrix
         self._operated_mapping_matrix_override = operated_mapping_matrix_override
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_linear_obj_func_list.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj_func_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import numpy as np
 
 from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
 
 
 class MockLinearObjFuncList(AbstractLinearObjFuncList):
     def __init__(
-        self, parameters=None, grid=None, mapping_matrix=None, regularization=None
+        self,
+        parameters=None,
+        grid=None,
+        mapping_matrix=None,
+        regularization=None,
+        operated_mapping_matrix_override=None,
     ):
-
         super().__init__(grid=grid, regularization=regularization)
 
         self._parameters = parameters
         self._mapping_matrix = mapping_matrix
+        self._operated_mapping_matrix_override = operated_mapping_matrix_override
 
     @property
     def params(self) -> int:
         return self._parameters
 
     @property
     def mapping_matrix(self) -> np.ndarray:
         return self._mapping_matrix
+
+    @property
+    def operated_mapping_matrix_override(self) -> np.ndarray:
+        return self._operated_mapping_matrix_override
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_mapper.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 
 class MockMapper(AbstractMapper):
     def __init__(
         self,
         source_plane_data_grid=None,
         source_plane_mesh_grid=None,
-        hyper_data=None,
+        adapt_data=None,
         edge_pixel_list=None,
         regularization=None,
         pix_sub_weights=None,
         pix_sub_weights_split_cross=None,
         mapping_matrix=None,
         pixel_signals=None,
         parameters=None,
         interpolated_array=None,
     ):
-
         mapper_grids = MapperGrids(
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
-            hyper_data=hyper_data,
+            adapt_data=adapt_data,
         )
 
         super().__init__(mapper_grids=mapper_grids, regularization=regularization)
 
         self._edge_pixel_list = edge_pixel_list
         self._pix_sub_weights = pix_sub_weights
         self._pix_sub_weights_split_cross = pix_sub_weights_split_cross
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_mesh.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mesh.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,41 +7,38 @@
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.sparse_2d import Grid2DSparse
 from autoarray.preloads import Preloads
 
 
 class MockMesh(AbstractMesh):
     def __init__(self, image_plane_mesh_grid=None):
-
         super().__init__()
 
         self.image_plane_mesh_grid = image_plane_mesh_grid
 
     def mapper_grids_from(
         self,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Grid2DSparse = None,
         image_plane_mesh_grid: Grid2DSparse = None,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings=SettingsPixelization(),
         preloads: Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ) -> MapperGrids:
-
         return MapperGrids(
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
             image_plane_mesh_grid=self.image_plane_mesh_grid,
-            hyper_data=hyper_data,
+            adapt_data=adapt_data,
             settings=settings,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     def image_plane_mesh_grid_from(
-        self, image_plane_data_grid, hyper_data, settings=None
+        self, image_plane_data_grid, adapt_data, settings=None
     ):
-
-        if hyper_data is not None and self.image_plane_mesh_grid is not None:
-            return hyper_data * self.image_plane_mesh_grid
+        if adapt_data is not None and self.image_plane_mesh_grid is not None:
+            return adapt_data * self.image_plane_mesh_grid
 
         return self.image_plane_mesh_grid
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/mock/mock_pixelization.py` & `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_pixelization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from autoarray.inversion.pixelization.pixelization import Pixelization
 
 
 class MockPixelization(Pixelization):
     def __init__(
         self, mesh=None, regularization=None, mapper=None, image_plane_mesh_grid=None
     ):
-
         super().__init__(mesh=mesh, regularization=regularization)
 
         self.mapper = mapper
         self.image_plane_mesh_grid = image_plane_mesh_grid
 
     # noinspection PyUnusedLocal,PyShadowingNames
     def mapper_grids_from(
         self,
         source_plane_data_grid,
         source_plane_mesh_grid,
         image_plane_mesh_grid=None,
-        hyper_data=None,
+        adapt_data=None,
         settings=None,
         preloads=None,
         profiling_dict=None,
     ):
         return self.mapper
 
     def image_plane_mesh_grid_from(
-        self, image_plane_data_grid, hyper_data, settings=None
+        self, image_plane_data_grid, adapt_data, settings=None
     ):
-
-        if hyper_data is not None and self.image_plane_mesh_grid is not None:
-            return hyper_data * self.image_plane_mesh_grid
+        if adapt_data is not None and self.image_plane_mesh_grid is not None:
+            return adapt_data * self.image_plane_mesh_grid
 
         return self.image_plane_mesh_grid
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/abstract.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools
 import numpy as np
 from typing import Dict, List, Optional, Tuple
 
+from autoconf import conf
 from autoconf import cached_property
 
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.linear_obj.func_list import UniqueMappings
 from autoarray.inversion.linear_obj.neighbors import Neighbors
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
 from autoarray.inversion.regularization.abstract import AbstractRegularization
@@ -105,16 +106,16 @@
         return self.mapper_grids.image_plane_mesh_grid
 
     @property
     def edge_pixel_list(self) -> List[int]:
         return self.source_plane_mesh_grid.edge_pixel_list
 
     @property
-    def hyper_data(self) -> np.ndarray:
-        return self.mapper_grids.hyper_data
+    def adapt_data(self) -> np.ndarray:
+        return self.mapper_grids.adapt_data
 
     @property
     def neighbors(self) -> Neighbors:
         return self.source_plane_mesh_grid.neighbors
 
     @property
     def pix_sub_weights(self) -> "PixSubWeights":
@@ -233,23 +234,25 @@
         To perform an `Inversion` efficiently the linear algebra can bypass the calculation of a `mapping_matrix` and
         instead use the w-tilde formalism, which requires these unique mappings for efficient computation. For
         convenience, these mappings and associated metadata are packaged into the class `UniqueMappings`.
 
         A full description of these mappings is given in the
         function `mapper_util.data_slim_to_pixelization_unique_from()`.
         """
+
         (
             data_to_pix_unique,
             data_weights,
             pix_lengths,
         ) = mapper_util.data_slim_to_pixelization_unique_from(
             data_pixels=self.source_plane_data_grid.shape_slim,
             pix_indexes_for_sub_slim_index=self.pix_indexes_for_sub_slim_index,
             pix_sizes_for_sub_slim_index=self.pix_sizes_for_sub_slim_index,
             pix_weights_for_sub_slim_index=self.pix_weights_for_sub_slim_index,
+            pix_pixels=self.params,
             sub_size=self.source_plane_data_grid.sub_size,
         )
 
         return UniqueMappings(
             data_to_pix_unique=data_to_pix_unique,
             data_weights=data_weights,
             pix_lengths=pix_lengths,
@@ -277,15 +280,15 @@
             total_mask_pixels=self.source_plane_data_grid.mask.pixels_in_mask,
             slim_index_for_sub_slim_index=self.slim_index_for_sub_slim_index,
             sub_fraction=self.source_plane_data_grid.mask.sub_fraction,
         )
 
     def pixel_signals_from(self, signal_scale: float) -> np.ndarray:
         """
-        Returns the (hyper) signal in each pixelization pixel, where this signal is an estimate of the expected signal
+        Returns the signal in each pixelization pixel, where this signal is an estimate of the expected signal
         each pixelization pixel contains given the data pixels it maps too.
 
         A full description of this is given in the function `mapper_util.adaptive_pixel_signals_from().
 
         Parameters
         ----------
         signal_scale
@@ -295,15 +298,15 @@
         return mapper_util.adaptive_pixel_signals_from(
             pixels=self.pixels,
             signal_scale=signal_scale,
             pixel_weights=self.pix_weights_for_sub_slim_index,
             pix_indexes_for_sub_slim_index=self.pix_indexes_for_sub_slim_index,
             pix_size_for_sub_slim_index=self.pix_sizes_for_sub_slim_index,
             slim_index_for_sub_slim_index=self.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim,
-            hyper_data=self.hyper_data,
+            adapt_data=self.adapt_data,
         )
 
     def pix_indexes_for_slim_indexes(self, pix_indexes: List) -> List[List]:
         """
         Returns the index mappings between every masked data-point (not subgridded) on the data and the mapper
         pixels / parameters that it maps too.
 
@@ -357,14 +360,43 @@
             The masked 2D array of values in its slim representation (e.g. the image data) which are mapped to the
             source domain in order to compute their average values.
         """
         return mapper_util.mapped_to_source_via_mapping_matrix_from(
             mapping_matrix=self.mapping_matrix, array_slim=array.binned.slim
         )
 
+    def extent_from(
+        self, values: np.ndarray = None, zoom_to_brightest: bool = True
+    ) -> Tuple[float, float, float, float]:
+        if zoom_to_brightest and values is not None:
+            zoom_percent = conf.instance["visualize"]["general"]["zoom"][
+                "inversion_percent"
+            ]
+
+            fractional_value = np.max(values) * zoom_percent
+            fractional_bool = values > fractional_value
+            true_indices = np.argwhere(fractional_bool)
+            true_grid = self.source_plane_mesh_grid[true_indices]
+
+            from autoarray.geometry import geometry_util
+
+            try:
+                return geometry_util.extent_symmetric_from(
+                    extent=(
+                        np.min(true_grid[:, 0, 1]),
+                        np.max(true_grid[:, 0, 1]),
+                        np.min(true_grid[:, 0, 0]),
+                        np.max(true_grid[:, 0, 0]),
+                    )
+                )
+            except ValueError:
+                return self.source_plane_mesh_grid.geometry.extent
+
+        return self.source_plane_mesh_grid.geometry.extent
+
     def interpolated_array_from(
         self,
         values: np.ndarray,
         shape_native: Tuple[int, int] = (401, 401),
         extent: Optional[Tuple[float, float, float, float]] = None,
     ) -> Array2D:
         """
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/delaunay.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/delaunay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/factory.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,31 +41,27 @@
         MapperRectangularNoInterp,
     )
     from autoarray.inversion.pixelization.mappers.delaunay import MapperDelaunay
     from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoi
     from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoiNoInterp
 
     if isinstance(mapper_grids.source_plane_mesh_grid, Mesh2DRectangular):
-
         return MapperRectangularNoInterp(
             mapper_grids=mapper_grids,
             regularization=regularization,
             profiling_dict=profiling_dict,
         )
     elif isinstance(mapper_grids.source_plane_mesh_grid, Mesh2DDelaunay):
-
         return MapperDelaunay(
             mapper_grids=mapper_grids,
             regularization=regularization,
             profiling_dict=profiling_dict,
         )
     elif isinstance(mapper_grids.source_plane_mesh_grid, Mesh2DVoronoi):
-
         if mapper_grids.source_plane_mesh_grid.uses_interpolation:
-
             return MapperVoronoi(
                 mapper_grids=mapper_grids,
                 regularization=regularization,
                 profiling_dict=profiling_dict,
             )
 
         return MapperVoronoiNoInterp(
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/mapper_grids.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_grids.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class MapperGrids:
     def __init__(
         self,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Abstract2DMesh = None,
         image_plane_mesh_grid: Grid2DSparse = None,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings: SettingsPixelization = SettingsPixelization(),
         preloads: Preloads = None,
         profiling_dict: Optional[Dict] = None,
     ):
         """
         Groups the different grids used by `Mesh` objects, the `mesh` package and the `pixelization` package, which
         create the following four grids:
@@ -49,15 +49,15 @@
             A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
             `source` reference frame.
         source_plane_mesh_grid
             The 2D grid of (y,x) centres of every pixelization pixel in the `source` frame.
         image_plane_mesh_grid
             The sparse set of (y,x) coordinates computed from the unmasked data in the `data` frame. This has a
             transformation applied to it to create the `source_plane_mesh_grid`.
-        hyper_data
+        adapt_data
             An image which is used to determine the `image_plane_mesh_grid` and therefore adapt the distribution of
             pixels of the Delaunay grid to the data it discretizes.
         settings
             Settings controlling the pixelization for example if a border is used to relocate its exterior coordinates.
         preloads
             Preloads in memory certain arrays which may be known beforehand in order to speed up the calculation,
             for example the `source_plane_mesh_grid` could be preloaded.
@@ -66,11 +66,11 @@
         """
 
         from autoarray.preloads import Preloads
 
         self.source_plane_data_grid = source_plane_data_grid
         self.source_plane_mesh_grid = source_plane_mesh_grid
         self.image_plane_mesh_grid = image_plane_mesh_grid
-        self.hyper_data = hyper_data
+        self.adapt_data = adapt_data
         self.settings = settings
         self.preloads = preloads or Preloads()
         self.profiling_dict = profiling_dict
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/mapper_util.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,30 @@
 
 @numba_util.jit()
 def sub_slim_indexes_for_pix_index(
     pix_indexes_for_sub_slim_index: np.ndarray,
     pix_weights_for_sub_slim_index: np.ndarray,
     pix_pixels: int,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-
     sub_slim_sizes_for_pix_index = np.zeros(pix_pixels)
 
     for pix_indexes in pix_indexes_for_sub_slim_index:
         for pix_index in pix_indexes:
-
             sub_slim_sizes_for_pix_index[pix_index] += 1
 
     max_pix_size = np.max(sub_slim_sizes_for_pix_index)
 
     sub_slim_indexes_for_pix_index = -1 * np.ones(shape=(pix_pixels, int(max_pix_size)))
     sub_slim_weights_for_pix_index = -1 * np.ones(shape=(pix_pixels, int(max_pix_size)))
     sub_slim_sizes_for_pix_index = np.zeros(pix_pixels)
 
     for slim_index, pix_indexes in enumerate(pix_indexes_for_sub_slim_index):
-
         pix_weights = pix_weights_for_sub_slim_index[slim_index]
 
         for pix_index, pix_weight in zip(pix_indexes, pix_weights):
-
             sub_slim_indexes_for_pix_index[
                 pix_index, int(sub_slim_sizes_for_pix_index[pix_index])
             ] = slim_index
 
             sub_slim_weights_for_pix_index[
                 pix_index, int(sub_slim_sizes_for_pix_index[pix_index])
             ] = pix_weight
@@ -53,14 +49,15 @@
 
 @numba_util.jit()
 def data_slim_to_pixelization_unique_from(
     data_pixels,
     pix_indexes_for_sub_slim_index: np.ndarray,
     pix_sizes_for_sub_slim_index: np.ndarray,
     pix_weights_for_sub_slim_index,
+    pix_pixels: int,
     sub_size: int,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Create an array describing the unique mappings between the sub-pixels of every slim data pixel and the pixelization
     pixels, which is used to perform efficiently linear algebra calculations.
 
     For example, assuming `sub_size=2`:
@@ -104,43 +101,36 @@
     sub_fraction = 1.0 / (sub_size**2.0)
 
     max_pix_mappings = int(np.max(pix_sizes_for_sub_slim_index))
 
     data_to_pix_unique = -1 * np.ones((data_pixels, max_pix_mappings * sub_size**2))
     data_weights = np.zeros((data_pixels, max_pix_mappings * sub_size**2))
     pix_lengths = np.zeros(data_pixels)
+    pix_check = -1 * np.ones(shape=pix_pixels)
 
     for ip in range(data_pixels):
+        pix_check[:] = -1
 
         pix_size = 0
 
         ip_sub_start = ip * sub_size**2
         ip_sub_end = ip_sub_start + sub_size**2
 
         for ip_sub in range(ip_sub_start, ip_sub_end):
+            for pix_interp_index in range(pix_sizes_for_sub_slim_index[ip_sub]):
+                pix = pix_indexes_for_sub_slim_index[ip_sub, pix_interp_index]
+                pixel_weight = pix_weights_for_sub_slim_index[ip_sub, pix_interp_index]
 
-            for pix_to_slim_index in range(pix_sizes_for_sub_slim_index[ip_sub]):
-
-                pix = pix_indexes_for_sub_slim_index[ip_sub, pix_to_slim_index]
-                pixel_weight = pix_weights_for_sub_slim_index[ip_sub, pix_to_slim_index]
-
-                stored_already = False
-
-                for i in range(pix_size):
-
-                    if data_to_pix_unique[ip, i] == pix:
-
-                        data_weights[ip, i] += sub_fraction * pixel_weight
-                        stored_already = True
-
-                if not stored_already:
+                if pix_check[pix] > -0.5:
+                    data_weights[ip, int(pix_check[pix])] += sub_fraction * pixel_weight
 
+                else:
                     data_to_pix_unique[ip, pix_size] = pix
                     data_weights[ip, pix_size] += sub_fraction * pixel_weight
-
+                    pix_check[pix] = pix_size
                     pix_size += 1
 
         pix_lengths[ip] = pix_size
 
     return data_to_pix_unique, data_weights, pix_lengths
 
 
@@ -218,36 +208,33 @@
         An array of length (voronoi_pixels) which gives the number of neighbors of every pixel in the
         Voronoi grid.
     """
 
     pix_indexes_for_sub_slim_index = np.zeros(shape=(grid.shape[0], 1))
 
     for sub_slim_index in range(grid.shape[0]):
-
         nearest_pix_index = nearest_pixelization_index_for_slim_index[
             slim_index_for_sub_slim_index[sub_slim_index]
         ]
 
         whiletime = 0
 
         while True:
-
             if whiletime > 1000000:
                 raise exc.MeshException
 
             nearest_pix_center = mesh_grid[nearest_pix_index]
 
             sub_pixel_to_nearest_pix_distance = (
                 grid[sub_slim_index, 0] - nearest_pix_center[0]
             ) ** 2 + (grid[sub_slim_index, 1] - nearest_pix_center[1]) ** 2
 
             closest_separation_pix_to_neighbor = 1.0e8
 
             for neighbor_pix_index in range(neighbors_sizes[nearest_pix_index]):
-
                 neighbor = neighbors[nearest_pix_index, neighbor_pix_index]
 
                 distance_to_neighbor = (
                     grid[sub_slim_index, 0] - mesh_grid[neighbor, 0]
                 ) ** 2 + (grid[sub_slim_index, 1] - mesh_grid[neighbor, 1]) ** 2
 
                 if distance_to_neighbor < closest_separation_pix_to_neighbor:
@@ -299,19 +286,17 @@
     pix_indexes_for_sub_slim_index
         The mappings from a data sub-pixel index to a pixelization pixel index.
     """
 
     pixel_weights = np.zeros(pix_indexes_for_sub_slim_index.shape)
 
     for sub_slim_index in range(slim_index_for_sub_slim_index.shape[0]):
-
         pix_indexes = pix_indexes_for_sub_slim_index[sub_slim_index]
 
         if pix_indexes[1] != -1:
-
             vertices_of_the_simplex = source_plane_mesh_grid[pix_indexes]
 
             sub_gird_coordinate_on_source_place = source_plane_data_grid[sub_slim_index]
 
             area_0 = mesh_util.delaunay_triangle_area_from(
                 corner_0=vertices_of_the_simplex[1],
                 corner_1=vertices_of_the_simplex[2],
@@ -440,14 +425,15 @@
     return (
         pix_indexes_for_sub_slim_index,
         pix_indexes_for_sub_slim_index_sizes,
         pix_weights_for_sub_slim_index,
     )
 
 
+@numba_util.jit()
 def remove_bad_entries_voronoi_nn(
     bad_indexes,
     pix_weights_for_sub_slim_index,
     pix_indexes_for_sub_slim_index,
     grid,
     mesh_grid,
 ):
@@ -490,63 +476,61 @@
 def adaptive_pixel_signals_from(
     pixels: int,
     pixel_weights: np.ndarray,
     signal_scale: float,
     pix_indexes_for_sub_slim_index: np.ndarray,
     pix_size_for_sub_slim_index: np.ndarray,
     slim_index_for_sub_slim_index: np.ndarray,
-    hyper_data: np.ndarray,
+    adapt_data: np.ndarray,
 ) -> np.ndarray:
     """
-    Returns the (hyper) signal in each pixel, where the signal is the sum of its mapped data values.
+    Returns the signal in each pixel, where the signal is the sum of its mapped data values.
     These pixel-signals are used to compute the effective regularization weight of each pixel.
 
     The pixel signals are computed as follows:
 
     1) Divide by the number of mappe data points in the pixel, to ensure all pixels have the same
        'relative' signal (i.e. a pixel with 10 pixels doesn't have x2 the signal of one with 5).
 
     2) Divided by the maximum pixel-signal, so that all signals vary between 0 and 1. This ensures that the
        regularization weight_list are defined identically for any data quantity or signal-to-noise_map ratio.
 
-    3) Raised to the power of the hyper-parameter *signal_scale*, so the method can control the relative
+    3) Raised to the power of the parameter *signal_scale*, so the method can control the relative
        contribution regularization in different regions of pixelization.
 
     Parameters
     ----------
     pixels
         The total number of pixels in the pixelization the regularization scheme is applied to.
     signal_scale
         A factor which controls how rapidly the smoothness of regularization varies from high signal regions to
         low signal regions.
     regular_to_pix
         A 1D array util every pixel on the grid to a pixel on the pixelization.
-    hyper_data
+    adapt_data
         The image of the galaxy which is used to compute the weigghted pixel signals.
     """
 
     pixel_signals = np.zeros((pixels,))
     pixel_sizes = np.zeros((pixels,))
 
     for sub_slim_index in range(len(pix_indexes_for_sub_slim_index)):
-
         vertices_indexes = pix_indexes_for_sub_slim_index[sub_slim_index]
 
         mask_1d_index = slim_index_for_sub_slim_index[sub_slim_index]
 
         pix_size_tem = pix_size_for_sub_slim_index[sub_slim_index]
 
         if pix_size_tem > 1:
-
             pixel_signals[vertices_indexes[:pix_size_tem]] += (
-                hyper_data[mask_1d_index] * pixel_weights[sub_slim_index]
+                adapt_data[mask_1d_index] * pixel_weights[sub_slim_index]
             )
             pixel_sizes[vertices_indexes] += 1
         else:
-            pixel_signals[vertices_indexes[0]] += hyper_data[mask_1d_index]
+            pixel_signals[vertices_indexes[0]] += adapt_data[mask_1d_index]
             pixel_sizes[vertices_indexes[0]] += 1
 
     pixel_sizes[pixel_sizes == 0] = 1
     pixel_signals /= pixel_sizes
     pixel_signals /= np.max(pixel_signals)
 
     return pixel_signals**signal_scale
@@ -633,19 +617,17 @@
     sub_fraction
         The fractional area each sub-pixel takes up in an pixel.
     """
 
     mapping_matrix = np.zeros((total_mask_pixels, pixels))
 
     for sub_slim_index in range(slim_index_for_sub_slim_index.shape[0]):
-
         slim_index = slim_index_for_sub_slim_index[sub_slim_index]
 
         for pix_count in range(pix_size_for_sub_slim_index[sub_slim_index]):
-
             pix_index = pix_indexes_for_sub_slim_index[sub_slim_index, pix_count]
             pix_weight = pix_weights_for_sub_slim_index[sub_slim_index, pix_count]
 
             mapping_matrix[slim_index][pix_index] += sub_fraction * pix_weight
 
     return mapping_matrix
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/rectangular.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/rectangular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mappers/voronoi.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/voronoi.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/abstract.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
         Parameters
         ----------
         source_plane_data_grid
             A 2D (y,x) grid of coordinates, whose coordinates outside the border are relocated to its edge.
         """
         if preloads.relocated_grid is None:
-
             if settings.use_border:
                 return source_plane_data_grid.relocated_grid_from(
                     grid=source_plane_data_grid
                 )
             return source_plane_data_grid
 
         return preloads.relocated_grid
@@ -92,31 +91,30 @@
         return source_plane_mesh_grid
 
     def mapper_grids_from(
         self,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Grid2DSparse = None,
         image_plane_mesh_grid: Grid2DSparse = None,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings=SettingsPixelization(),
         preloads: Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         raise NotImplementedError
 
     def mesh_grid_from(
         self,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Grid2DSparse,
         sparse_index_for_slim_index: np.ndarray = None,
     ):
         raise NotImplementedError
 
-    def weight_map_from(self, hyper_data: np.ndarray):
-
+    def weight_map_from(self, adapt_data: np.ndarray):
         raise NotImplementedError()
 
     @property
     def is_stochastic(self):
         return False
 
     def __str__(self):
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/delaunay.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/delaunay.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         super().__init__()
         self.shape = (int(shape[0]), int(shape[1]))
         self.pixels = self.shape[0] * self.shape[1]
 
     def image_plane_mesh_grid_from(
         self,
         image_plane_data_grid: Grid2D,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings=SettingsPixelization(),
     ):
         """
         Computes the ``mesh_grid`` in the image-plane, by overlaying a uniform grid of coordinates over the
         masked 2D data (see ``Grid2DSparse.from_grid_and_unmasked_2d_grid_shape()``).
 
         For a ``DelaunayMagnification`` this grid is computed by overlaying a 2D grid with dimensions ``shape`` over the
@@ -124,15 +124,15 @@
         retained.
 
         Parameters
         ----------
         image_plane_mesh_grid
             The sparse set of (y,x) coordinates computed from the unmasked data in the image-plane. This has a
             transformation applied to it to create the ``source_plane_mesh_grid``.
-        hyper_data
+        adapt_data
             An image which is used to determine the ``image_plane_mesh_grid`` and therefore adapt the distribution of
             pixels of the Delaunay grid to the data it discretizes.
         settings
             Settings controlling the pixelization for example if a border is used to relocate its exterior coordinates.
         """
         return Grid2DSparse.from_grid_and_unmasked_2d_grid_shape(
             grid=image_plane_data_grid, unmasked_sparse_shape=self.shape
@@ -184,64 +184,64 @@
         """
         super().__init__()
 
         self.pixels = int(pixels)
         self.weight_floor = weight_floor
         self.weight_power = weight_power
 
-    def weight_map_from(self, hyper_data: np.ndarray):
+    def weight_map_from(self, adapt_data: np.ndarray):
         """
-        Computes a ``weight_map`` from an input ``hyper_data``, where this image represents components in the masked 2d
+        Computes a ``weight_map`` from an input ``adapt_data``, where this image represents components in the masked 2d
         data in the image-plane. This applies the ``weight_floor`` and ``weight_power`` attributes of the class, which
         scale the weights to make different components upweighted relative to one another.
 
         Parameters
         ----------
-        hyper_data
+        adapt_data
             A image which represents one or more components in the masked 2D data in the image-plane.
 
         Returns
         -------
         The weight map which is used to adapt the Delaunay pixels in the image-plane to components in the data.
         """
-        weight_map = (hyper_data - np.min(hyper_data)) / (
-            np.max(hyper_data) - np.min(hyper_data)
-        ) + self.weight_floor * np.max(hyper_data)
+        weight_map = (adapt_data - np.min(adapt_data)) / (
+            np.max(adapt_data) - np.min(adapt_data)
+        ) + self.weight_floor * np.max(adapt_data)
 
         return np.power(weight_map, self.weight_power)
 
     def image_plane_mesh_grid_from(
         self,
         image_plane_data_grid: Grid2D,
-        hyper_data: np.ndarray,
+        adapt_data: np.ndarray,
         settings=SettingsPixelization(),
     ):
         """
         Computes the ``mesh_grid`` in the image-plane, by overlaying a uniform grid of coordinates over the
         masked 2D data (see ``Grid2DSparse.from_grid_and_unmasked_2d_grid_shape()``).
 
         The ``data_pixelization_grid`` is transformed to the ``source_plane_mesh_grid``, and it is these (y,x) values
         which then act the centres of the Delaunay pixelization's pixels.
 
         For a ``DelaunayBrightnessImage`` this grid is computed by applying a KMeans clustering algorithm to the masked
-        data's values, where these values are reweighted by the ``hyper_data`` so that the algorithm can adapt to
+        data's values, where these values are reweighted by the ``adapt_data`` so that the algorithm can adapt to
         specific parts of the data.
 
         Parameters
         ----------
         image_plane_mesh_grid
             The sparse set of (y,x) coordinates computed from the unmasked data in the image-plane. This has a
             transformation applied to it to create the ``source_plane_mesh_grid``.
-        hyper_data
+        adapt_data
             An image which is used to determine the ``image_plane_mesh_grid`` and therefore adapt the distribution of
             pixels of the Delaunay grid to the data it discretizes.
         settings
             Settings controlling the pixelization for example if a border is used to relocate its exterior coordinates.
         """
-        weight_map = self.weight_map_from(hyper_data=hyper_data)
+        weight_map = self.weight_map_from(adapt_data=adapt_data)
 
         return Grid2DSparse.from_total_pixels_grid_and_weight_map(
             total_pixels=self.pixels,
             grid=image_plane_data_grid,
             weight_map=weight_map,
             seed=settings.kmeans_seed,
             stochastic=settings.is_stochastic,
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/mesh_util.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/mesh_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,14 @@
 
     simplices = delaunay.simplices
     pixel_points = delaunay.points
 
     interpolated_array = np.zeros(len(interpolation_grid_slim))
 
     for slim_index in range(len(interpolation_grid_slim)):
-
         simplex_index = simplex_index_for_interpolate_index[slim_index]
         interpolating_point = interpolation_grid_slim[slim_index]
 
         if simplex_index == -1:
             cloest_pixel_index = np.argmin(
                 np.sum((pixel_points - interpolating_point) ** 2.0, axis=1)
             )
@@ -581,15 +580,15 @@
                 # finite ridge: already in the region
                 continue
 
             # Compute the missing endpoint of an infinite ridge
 
             t = voronoi.points[p2] - voronoi.points[p1]  # tangent
             t /= np.linalg.norm(t)
-            n = np.array([-t[1], t[0]])  # hyper
+            n = np.array([-t[1], t[0]])
 
             midpoint = voronoi.points[[p1, p2]].mean(axis=0)
             direction = np.sign(np.dot(midpoint - center, n)) * n
             far_point = voronoi.vertices[v2] + direction * radius
 
             region.append(len(vertex_list))
             vertex_list.append(far_point.tolist())
@@ -608,15 +607,14 @@
 
 def voronoi_nn_interpolated_array_from(
     shape_native: Tuple[int, int],
     interpolation_grid_slim: np.ndarray,
     pixel_values: np.ndarray,
     voronoi: scipy.spatial.Voronoi,
 ) -> np.ndarray:
-
     try:
         from autoarray.util.nn import nn_py
     except ImportError as e:
         raise ImportError(
             "In order to use the VoronoiNN pixelization you must install the "
             "Natural Neighbor Interpolation c package.\n\n"
             ""
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/rectangular.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/rectangular.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         return False
 
     def mapper_grids_from(
         self,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Grid2D = None,
         image_plane_mesh_grid: Grid2D = None,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings: SettingsPixelization = SettingsPixelization(),
         preloads: Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         """
         Mapper objects describe the mappings between pixels in the masked 2D data and the pixels in a pixelization,
         in both the `data` and `source` frames.
@@ -92,15 +92,15 @@
             A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
             `source` reference frame.
         source_plane_mesh_grid
             Not used for a rectangular pixelization, because the pixelization grid in the `source` frame is computed
             by overlaying the `source_plane_data_grid` with the rectangular pixelization.
         image_plane_mesh_grid
             Not used for a rectangular pixelization.
-        hyper_data
+        adapt_data
             Not used for a rectangular pixelization.
         settings
             Settings controlling the pixelization for example if a border is used to relocate its exterior coordinates.
         preloads
             Object which may contain preloaded arrays of quantities computed in the pixelization, which are passed via
             this object speed up the calculation.
         profiling_dict
@@ -116,15 +116,15 @@
         )
         mesh_grid = self.mesh_grid_from(source_plane_data_grid=relocated_grid)
 
         return MapperGrids(
             source_plane_data_grid=relocated_grid,
             source_plane_mesh_grid=mesh_grid,
             image_plane_mesh_grid=image_plane_mesh_grid,
-            hyper_data=hyper_data,
+            adapt_data=adapt_data,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
 
     @profile_func
     def mesh_grid_from(
         self,
@@ -150,14 +150,14 @@
         return Mesh2DRectangular.overlay_grid(
             shape_native=self.shape, grid=source_plane_data_grid
         )
 
     def image_plane_mesh_grid_from(
         self,
         image_plane_data_grid: Grid2D,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings=SettingsPixelization(),
     ):
         """
         Not used for rectangular pixelization.
         """
         return None
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/triangulation.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/triangulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class Triangulation(AbstractMesh):
     def mapper_grids_from(
         self,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Grid2DSparse = None,
         image_plane_mesh_grid: Grid2DSparse = None,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings=SettingsPixelization(),
         preloads: Preloads = Preloads(),
         profiling_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         """
         Mapper objects describe the mappings between pixels in the masked 2D data and the pixels in a mesh,
         in both the `data` and `source` frames.
@@ -51,15 +51,15 @@
         source_plane_mesh_grid
             The centres of every Voronoi pixel in the `source` frame, which are initially derived by computing a sparse
             set of (y,x) coordinates computed from the unmasked data in the `data` frame and applying a transformation
             to this.
         image_plane_mesh_grid
             The sparse set of (y,x) coordinates computed from the unmasked data in the `data` frame. This has a
             transformation applied to it to create the `source_plane_mesh_grid`.
-        hyper_data
+        adapt_data
             Not used for a rectangular mesh.
         settings
             Settings controlling the mesh for example if a border is used to relocate its exterior coordinates.
         preloads
             Object which may contain preloaded arrays of quantities computed in the mesh, which are passed via
             this object speed up the calculation.
         profiling_dict
@@ -77,24 +77,23 @@
         relocated_source_plane_mesh_grid = self.relocated_mesh_grid_from(
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
             settings=settings,
         )
 
         try:
-
             source_plane_mesh_grid = self.mesh_grid_from(
                 source_plane_data_grid=source_plane_data_grid,
                 source_plane_mesh_grid=relocated_source_plane_mesh_grid,
                 sparse_index_for_slim_index=source_plane_mesh_grid.sparse_index_for_slim_index,
             )
         except ValueError as e:
             raise e
 
         return MapperGrids(
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
             image_plane_mesh_grid=image_plane_mesh_grid,
-            hyper_data=hyper_data,
+            adapt_data=adapt_data,
             preloads=preloads,
             profiling_dict=profiling_dict,
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/voronoi.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         self.shape = (int(shape[0]), int(shape[1]))
         self.pixels = self.shape[0] * self.shape[1]
 
     def image_plane_mesh_grid_from(
         self,
         image_plane_data_grid: Grid2D,
-        hyper_data: np.ndarray = None,
+        adapt_data: np.ndarray = None,
         settings=SettingsPixelization(),
     ) -> Grid2DSparse:
         """
         Computes the `mesh_grid` in the `data` frame, by overlaying a uniform grid of coordinates over the
         masked 2D data (see `Grid2DSparse.from_grid_and_unmasked_2d_grid_shape()`).
 
         For a `VoronoiMagnification` this grid is computed by overlaying a 2D grid with dimensions `shape` over the
@@ -135,15 +135,15 @@
         retained.
 
         Parameters
         ----------
         image_plane_mesh_grid
             The sparse set of (y,x) coordinates computed from the unmasked data in the `data` frame. This has a
             transformation applied to it to create the `source_plane_mesh_grid`.
-        hyper_data
+        adapt_data
             An image which is used to determine the `image_plane_mesh_grid` and therefore adapt the distribution of
             pixels of the Voronoi grid to the data it discretizes.
         settings
             Settings controlling the pixelization for example if a border is used to relocate its exterior coordinates.
         """
         return Grid2DSparse.from_grid_and_unmasked_2d_grid_shape(
             grid=image_plane_data_grid, unmasked_sparse_shape=self.shape
@@ -196,64 +196,64 @@
         """
         super().__init__()
 
         self.pixels = int(pixels)
         self.weight_floor = weight_floor
         self.weight_power = weight_power
 
-    def weight_map_from(self, hyper_data: np.ndarray) -> np.ndarray:
+    def weight_map_from(self, adapt_data: np.ndarray) -> np.ndarray:
         """
-        Computes a `weight_map` from an input `hyper_data`, where this image represents components in the masked 2d
+        Computes a `weight_map` from an input `adapt_data`, where this image represents components in the masked 2d
         data in the `data` frame. This applies the `weight_floor` and `weight_power` attributes of the class, which
         scale the weights to make different components upweighted relative to one another.
 
         Parameters
         ----------
-        hyper_data
+        adapt_data
             A image which represents one or more components in the masked 2D data in the `data` frame.
 
         Returns
         -------
         The weight map which is used to adapt the Voronoi pixels in the `data` frame to components in the data.
         """
-        weight_map = (hyper_data - np.min(hyper_data)) / (
-            np.max(hyper_data) - np.min(hyper_data)
-        ) + self.weight_floor * np.max(hyper_data)
+        weight_map = (adapt_data - np.min(adapt_data)) / (
+            np.max(adapt_data) - np.min(adapt_data)
+        ) + self.weight_floor * np.max(adapt_data)
 
         return np.power(weight_map, self.weight_power)
 
     def image_plane_mesh_grid_from(
         self,
         image_plane_data_grid: Grid2D,
-        hyper_data: np.ndarray,
+        adapt_data: np.ndarray,
         settings=SettingsPixelization(),
     ):
         """
         Computes the `mesh_grid` in the `data` frame, by overlaying a uniform grid of coordinates over the
         masked 2D data (see `Grid2DSparse.from_grid_and_unmasked_2d_grid_shape()`).
 
         The `data_pixelization_grid` is transformed to the `source_plane_mesh_grid`, and it is these (y,x) values
         which then act the centres of the Voronoi mesh's pixels.
 
         For a `VoronoiBrightnessImage` this grid is computed by applying a KMeans clustering algorithm to the masked
-        data's values, where these values are reweighted by the `hyper_data` so that the algorithm can adapt to
+        data's values, where these values are reweighted by the `adapt_data` so that the algorithm can adapt to
         specific parts of the data.
 
         Parameters
         ----------
         image_plane_mesh_grid
             The sparse set of (y,x) coordinates computed from the unmasked data in the `data` frame. This has a
             transformation applied to it to create the `source_plane_mesh_grid`.
-        hyper_data
+        adapt_data
             An image which is used to determine the `image_plane_mesh_grid` and therefore adapt the distribution of
             pixels of the Voronoi grid to the data it discretizes.
         settings
             Settings controlling the pixelization for example if a border is used to relocate its exterior coordinates.
         """
-        weight_map = self.weight_map_from(hyper_data=hyper_data)
+        weight_map = self.weight_map_from(adapt_data=adapt_data)
 
         return Grid2DSparse.from_total_pixels_grid_and_weight_map(
             total_pixels=self.pixels,
             grid=image_plane_data_grid,
             weight_map=weight_map,
             seed=settings.kmeans_seed,
             stochastic=settings.is_stochastic,
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/mesh/voronoi_nn.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi_nn.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/pixelization.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/pixelization.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         change position from the image-plane to source-plane.
 
 
         **Pixelization Uses**
 
         The following objects / packages are used with a ``Pixelization``:
 
-        - ``Mapper``: Computes the mappings between the the image's (y,x) grid and the mesh's pixels.
+        - ``Mapper``: Computes the mappings between the image's (y,x) grid and the mesh's pixels.
         - ``Inversion``: Use the ``Pixelization`` to reconstruct the data on the mesh via linear algebra.
         - ``Regularization``: Apply smoothing to the solutions computed using an ``Inversion``.
 
         In the example above, a ``Rectangular`` ``Mesh`` object is used. Other meshes are available (e.g.
         ``Delaunay``, ``Voronoi``).
 
         **Source Code API**
@@ -158,13 +158,12 @@
         Returns a ``MapperGrids`` object, which contains all of the different grids used by a
         pixelization (``image_plane_data_grid``, ``image_plane_mesh_grid``, ``source_plane_data_grid``,
         ``source_plane_mesh_grid``).
         """
         return self.mesh.mapper_grids_from
 
     def __repr__(self):
-
         string = "{}\n{}".format(self.__class__.__name__, str(self.mesh))
         if self.regularization is not None:
             string += "{}\n{}".format(self.__class__.__name__, str(self.regularization))
 
         return string
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/pixelization/settings.py` & `autoarray-2023.7.7.1/autoarray/inversion/pixelization/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/plot/inversion_plotters.py` & `autoarray-2023.7.7.1/autoarray/inversion/plot/inversion_plotters.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,17 +39,15 @@
             The inversion the plotter plots.
         mat_plot_2d
             Contains objects which wrap the matplotlib function calls that make 2D plots.
         visuals_2d
             Contains 2D visuals that can be overlaid on 2D plots.
         include_2d
             Specifies which attributes of the `Inversion` are extracted and plotted as visuals for 2D plots.
-        residuals_symmetric_cmap
-            If true, the `residual_map` and `normalized_residual_map` are plotted with a symmetric color map such
-            that `abs(vmin) = abs(vmax)`.
+
         """
         super().__init__(
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
         self.inversion = inversion
         self.residuals_symmetric_cmap = residuals_symmetric_cmap
@@ -90,33 +88,31 @@
 
         Parameters
         ----------
         reconstructed_image
             Whether to make a 2D plot (via `imshow`) of the reconstructed image data.
         """
         if reconstructed_image:
-
             self.mat_plot_2d.plot_array(
                 array=self.inversion.mapped_reconstructed_image,
                 visuals_2d=self.get_visuals_2d_for_data(),
                 auto_labels=AutoLabels(
                     title="Reconstructed Image", filename="reconstructed_image"
                 ),
             )
 
     def figures_2d_of_pixelization(
         self,
         pixelization_index: int = 0,
         reconstructed_image: bool = False,
         reconstruction: bool = False,
         errors: bool = False,
-        residual_map: bool = False,
-        normalized_residual_map: bool = False,
-        chi_squared_map: bool = False,
         regularization_weights: bool = False,
+        zoom_to_brightest: bool = True,
+        interpolate_to_uniform: bool = False,
     ):
         """
         Plots the individual attributes of a specific `Mapper` of the plotter's `Inversion` object in 2D.
 
         The API is such that every plottable attribute of the `Mapper` and `Inversion` object is an input parameter of
         type bool of the function, which if switched to `True` means that it is plotted.
 
@@ -126,142 +122,95 @@
             The index of the `Mapper` in the `Inversion`'s `linear_obj_list` that is plotted.
         reconstructed_image
             Whether to make a 2D plot (via `imshow`) of the mapper's reconstructed image data.
         reconstruction
             Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane reconstruction.
         errors
             Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane errors.
-        residual_map
-            Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane residual map.
-        normalized_residual_map
-            Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane normalized residual
-            map.
-        chi_squared_map
-            Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane chi-squared map.
-        residual_map
-            Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane regularization
-            weights.
+        zoom_to_brightest
+            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
+            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
+        interpolate_to_uniform
+            If `True`, the mapper's reconstruction is interpolated to a uniform grid before plotting, for example
+            meaning that an irregular Delaunay grid can be plotted as a uniform grid.
         """
 
         if not self.inversion.has(cls=AbstractMapper):
             return
 
         mapper_plotter = self.mapper_plotter_from(mapper_index=pixelization_index)
 
         if reconstructed_image:
-
             array = self.inversion.mapped_reconstructed_image_dict[
                 mapper_plotter.mapper
             ]
 
             self.mat_plot_2d.plot_array(
                 array=array,
                 visuals_2d=self.get_visuals_2d_for_data(),
                 auto_labels=AutoLabels(
                     title="Reconstructed Image", filename="reconstructed_image"
                 ),
             )
 
         if reconstruction:
-
             vmax_custom = False
 
             if "vmax" in self.mat_plot_2d.cmap.kwargs:
                 if self.mat_plot_2d.cmap.kwargs["vmax"] is None:
-
                     reconstruction_vmax_factor = conf.instance["visualize"]["general"][
                         "inversion"
                     ]["reconstruction_vmax_factor"]
 
                     self.mat_plot_2d.cmap.kwargs[
                         "vmax"
                     ] = reconstruction_vmax_factor * np.max(
                         self.inversion.reconstruction
                     )
                     vmax_custom = True
 
-            source_pixelization_values = self.inversion.reconstruction_dict[
-                mapper_plotter.mapper
-            ]
+            pixel_values = self.inversion.reconstruction_dict[mapper_plotter.mapper]
 
             mapper_plotter.plot_source_from(
-                source_pixelization_values=source_pixelization_values,
+                pixel_values=pixel_values,
+                zoom_to_brightest=zoom_to_brightest,
+                interpolate_to_uniform=interpolate_to_uniform,
                 auto_labels=AutoLabels(
-                    title="Source Inversion", filename="reconstruction"
+                    title="Source Reconstruction", filename="reconstruction"
                 ),
             )
 
             if vmax_custom:
                 self.mat_plot_2d.cmap.kwargs["vmax"] = None
 
         if errors:
-
             try:
-
                 mapper_plotter.plot_source_from(
-                    source_pixelization_values=self.inversion.errors_dict[
-                        mapper_plotter.mapper
-                    ],
+                    pixel_values=self.inversion.errors_dict[mapper_plotter.mapper],
                     auto_labels=AutoLabels(title="Errors", filename="errors"),
                 )
 
             except TypeError:
-
                 pass
 
-        cmap_original = self.mat_plot_2d.cmap
-
-        if self.residuals_symmetric_cmap:
-
-            self.mat_plot_2d.cmap = self.mat_plot_2d.cmap.symmetric
-
-        if residual_map:
-
-            mapper_plotter.plot_source_from(
-                source_pixelization_values=self.inversion.residual_map_mapper_dict[
-                    mapper_plotter.mapper
-                ],
-                auto_labels=AutoLabels(title="Residual Map", filename="residual_map"),
-            )
-
-        if normalized_residual_map:
-
-            mapper_plotter.plot_source_from(
-                source_pixelization_values=self.inversion.normalized_residual_map_mapper_dict[
-                    mapper_plotter.mapper
-                ],
-                auto_labels=AutoLabels(
-                    title="Normalized Residual Map", filename="normalized_residual_map"
-                ),
-            )
-
-        self.mat_plot_2d.cmap = cmap_original
-
-        if chi_squared_map:
-
-            mapper_plotter.plot_source_from(
-                source_pixelization_values=self.inversion.chi_squared_map_mapper_dict[
-                    mapper_plotter.mapper
-                ],
-                auto_labels=AutoLabels(
-                    title="Chi-Squared Map", filename="chi_squared_map"
-                ),
-            )
+        # TODO : NEed to understand why this raises an error in voronoi_drawer.
 
         if regularization_weights:
-
-            mapper_plotter.plot_source_from(
-                source_pixelization_values=self.inversion.regularization_weights_mapper_dict[
-                    mapper_plotter.mapper
-                ],
-                auto_labels=AutoLabels(
-                    title="Regularization weight_list",
-                    filename="regularization_weights",
-                ),
-            )
+            try:
+                mapper_plotter.plot_source_from(
+                    pixel_values=self.inversion.regularization_weights_mapper_dict[
+                        mapper_plotter.mapper
+                    ],
+                    auto_labels=AutoLabels(
+                        title="Regularization weight_list",
+                        filename="regularization_weights",
+                    ),
+                )
+            except IndexError:
+                pass
 
     def subplot_of_mapper(
         self, mapper_index: int = 0, auto_filename: str = "subplot_inversion"
     ):
         """
         Plots the individual attributes of a specific `Mapper` of the plotter's `Inversion` object in 2D on a subplot.
 
@@ -277,22 +226,34 @@
         self.figures_2d_of_pixelization(
             pixelization_index=mapper_index, reconstructed_image=True
         )
         self.figures_2d_of_pixelization(
             pixelization_index=mapper_index, reconstruction=True
         )
         self.figures_2d_of_pixelization(pixelization_index=mapper_index, errors=True)
+
+        try:
+            self.figures_2d_of_pixelization(
+                pixelization_index=mapper_index, regularization_weights=True
+            )
+        except IndexError:
+            pass
+
+        self.set_title(label="Source Reconstruction (Unzoomed)")
         self.figures_2d_of_pixelization(
-            pixelization_index=mapper_index, residual_map=True
-        )
-        self.figures_2d_of_pixelization(
-            pixelization_index=mapper_index, normalized_residual_map=True
+            pixelization_index=mapper_index,
+            reconstruction=True,
+            zoom_to_brightest=False,
         )
+        self.set_title(label=None)
+
+        self.set_title(label="Errors (Unzoomed)")
         self.figures_2d_of_pixelization(
-            pixelization_index=mapper_index, chi_squared_map=True
+            pixelization_index=mapper_index, errors=True, zoom_to_brightest=False
         )
+        self.set_title(label=None)
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename=f"{auto_filename}_{mapper_index}"
         )
 
         self.close_subplot_figure()
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/plot/mapper_plotters.py` & `autoarray-2023.7.7.1/autoarray/inversion/plot/mapper_plotters.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         solution_vector
             A vector of values which can culor the pixels of the mapper's source pixels.
         """
         self.mat_plot_2d.plot_mapper(
             mapper=self.mapper,
             visuals_2d=self.get_2d.via_mapper_for_source_from(mapper=self.mapper),
             interpolate_to_uniform=interpolate_to_uniform,
-            source_pixelization_values=solution_vector,
+            pixel_values=solution_vector,
             auto_labels=AutoLabels(
                 title="Pixelization Mesh (Image-Plane)", filename="mapper"
             ),
         )
 
     def subplot_image_and_mapper(
         self, image: Array2D, interpolate_to_uniform: bool = True
@@ -105,15 +105,14 @@
         self.mat_plot_2d.plot_array(
             array=image,
             visuals_2d=self.get_visuals_2d_for_data(),
             auto_labels=AutoLabels(title="Image (Image-Plane)"),
         )
 
         if self.visuals_2d.pix_indexes is not None:
-
             indexes = self.mapper.pix_indexes_for_slim_indexes(
                 pix_indexes=self.visuals_2d.pix_indexes
             )
 
             self.mat_plot_2d.index_scatter.scatter_grid_indexes(
                 grid=self.mapper.source_plane_data_grid.mask.derive_grid.unmasked,
                 indexes=indexes,
@@ -124,26 +123,36 @@
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename="subplot_image_and_mapper"
         )
         self.close_subplot_figure()
 
     def plot_source_from(
         self,
-        source_pixelization_values: np.ndarray,
+        pixel_values: np.ndarray,
+        zoom_to_brightest: bool = True,
+        interpolate_to_uniform: bool = False,
         auto_labels: AutoLabels = AutoLabels(),
     ):
         """
         Plot the source of the `Mapper` where the coloring is specified by an input set of values.
 
         Parameters
         ----------
-        source_pixelization_values
+        pixel_values
             The values of the mapper's source pixels used for coloring the figure.
+        zoom_to_brightest
+            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
+            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
+        interpolate_to_uniform
+            If `True`, the mapper's reconstruction is interpolated to a uniform grid before plotting, for example
+            meaning that an irregular Delaunay grid can be plotted as a uniform grid.
         auto_labels
             The labels given to the figure.
         """
         self.mat_plot_2d.plot_mapper(
             mapper=self.mapper,
             visuals_2d=self.get_visuals_2d_for_source(),
             auto_labels=auto_labels,
-            source_pixelization_values=source_pixelization_values,
+            pixel_values=pixel_values,
+            zoom_to_brightest=zoom_to_brightest,
+            interpolate_to_uniform=interpolate_to_uniform,
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/abstract.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     PyLopsOperator = object
 
 
 class AbstractRegularization:
     def __init__(self):
         """
         Abstract base class for a regularization-scheme, which is applied to a pixelization to enforce a \
-        smooth-source solution and prevent over-fitting noise_map in the hyper_galaxies. This is achieved by computing a \
+        smooth-source solution and prevent over-fitting. This is achieved by computing a \
         'regularization term' - which is the sum of differences in reconstructed flux between every set of neighboring \
         pixels. This regularization term is added to the solution's chi-squared as a penalty term. This effects \
         a pixelization in the following ways:
 
         1) The regularization matrix (see below) is added to the curvature matrix used by the inversion to \
-           linearly invert and fit the hyper_galaxies. Thus, it changes the pixelization in a linear manner, ensuring that \
+           linearly invert and fit the data. Thus, it changes the pixelization in a linear manner, ensuring that \
            the minimum chi-squared solution is achieved accounting for the penalty term.
 
-        2) The log likelihood of the pixelization's fit to the hyper_galaxies changes from L = -0.5 *(chi^2 + noise_normalization) \
+        2) The log likelihood of the pixelization's fit to the dataset changes from L = -0.5 *(chi^2 + noise_normalization) \
            to L = -0.5 (chi^2 + coefficients * regularization_term + noise_normalization). The regularization \
-           coefficient is a 'hyper_galaxies-parameter' which determines how strongly we smooth the pixelization's reconstruction.
+           coefficient is a parameter which determines how strongly we smooth the pixelization's reconstruction.
 
         The value of the coefficients(s) is set using the Bayesian framework of (Suyu 2006) and this \
         is described further in the (*inversion.inversion* class).
 
         The regularization matrix, H, is calculated by defining a set of B matrices which describe how the \
         pixels neighbor one another. For example, lets take a 3x3 square grid:
         ______
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/adaptive_brightness.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/adaptive_brightness_split.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/brightness_zeroth.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/brightness_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/constant.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/constant.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/constant_split.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/constant_zeroth.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_zeroth.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from autoarray.inversion.regularization.abstract import AbstractRegularization
 
 from autoarray.inversion.regularization import regularization_util
 
 
 class ConstantZeroth(AbstractRegularization):
     def __init__(self, coefficient_neighbor=1.0, coefficient_zeroth=1.0):
-
         super().__init__()
 
         self.coefficient_neighbor = coefficient_neighbor
         self.coefficient_zeroth = coefficient_zeroth
 
     def regularization_weights_from(self, linear_obj: LinearObj) -> np.ndarray:
         """
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/regularization_util.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/regularization_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,21 +331,19 @@
     """
 
     max_j = np.shape(splitted_weights)[1] - 1
 
     splitted_weights *= -1.0
 
     for i in range(len(splitted_mappings)):
-
         pixel_index = i // 4
 
         flag = 0
 
         for j in range(splitted_sizes[i]):
-
             if splitted_mappings[i][j] == pixel_index:
                 splitted_weights[i][j] += 1.0
                 flag = 1
 
             if j >= max_j:
                 raise exc.MeshException(
                     f"The number of Voronoi natural neighbours exceeds {max_j}."
@@ -362,31 +360,28 @@
 @numba_util.jit()
 def pixel_splitted_regularization_matrix_from(
     regularization_weights: np.ndarray,
     splitted_mappings: np.ndarray,
     splitted_sizes: np.ndarray,
     splitted_weights: np.ndarray,
 ) -> np.ndarray:
-
     # I'm not sure what is the best way to add surface brightness weight to the regularization scheme here.
     # Currently, I simply mulitply the i-th weight to the i-th source pixel, but there should be different ways.
     # Need to keep an eye here.
 
     parameters = int(len(splitted_mappings) / 4)
 
     regularization_matrix = np.zeros(shape=(parameters, parameters))
 
     regularization_weight = regularization_weights**2.0
 
     for i in range(parameters):
-
         regularization_matrix[i, i] += 2e-8
 
         for j in range(4):
-
             k = i * 4 + j
 
             size = splitted_sizes[k]
             mapping = splitted_mappings[k]
             weight = splitted_weights[k]
 
             for l in range(size):
```

### Comparing `autoarray-2023.3.27.1/autoarray/inversion/regularization/zeroth.py` & `autoarray-2023.7.7.1/autoarray/inversion/regularization/zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/layout/layout.py` & `autoarray-2023.7.7.1/autoarray/layout/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         cls,
         roe_corner,
         shape_native,
         parallel_overscan=None,
         serial_prescan=None,
         serial_overscan=None,
     ):
-
         parallel_overscan = layout_util.rotate_region_via_roe_corner_from(
             region=parallel_overscan, shape_native=shape_native, roe_corner=roe_corner
         )
         serial_prescan = layout_util.rotate_region_via_roe_corner_from(
             region=serial_prescan, shape_native=shape_native, roe_corner=roe_corner
         )
         serial_overscan = layout_util.rotate_region_via_roe_corner_from(
@@ -114,15 +113,14 @@
             shape_2d=shape_native,
             parallel_overscan=parallel_overscan,
             serial_prescan=serial_prescan,
             serial_overscan=serial_overscan,
         )
 
     def layout_extracted_from(self, extraction_region):
-
         parallel_overscan = layout_util.region_after_extraction(
             original_region=self.parallel_overscan, extraction_region=extraction_region
         )
         serial_prescan = layout_util.region_after_extraction(
             original_region=self.serial_prescan, extraction_region=extraction_region
         )
         serial_overscan = layout_util.region_after_extraction(
@@ -134,15 +132,14 @@
             shape_2d=self.shape_2d,
             parallel_overscan=parallel_overscan,
             serial_prescan=serial_prescan,
             serial_overscan=serial_overscan,
         )
 
     def new_rotated_from(self, roe_corner):
-
         parallel_overscan = layout_util.rotate_region_via_roe_corner_from(
             region=self.parallel_overscan,
             shape_native=self.shape_2d,
             roe_corner=roe_corner,
         )
         serial_prescan = layout_util.rotate_region_via_roe_corner_from(
             region=self.serial_prescan,
```

### Comparing `autoarray-2023.3.27.1/autoarray/layout/layout_util.py` & `autoarray-2023.7.7.1/autoarray/layout/layout_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     Parameters
     ----------
     array
         The array which is rotated.
     roe_corner
         The corner of the array at which the read-out electronics are located (e.g. (1, 1) is the bottom-right corner).
-        The rotation is based on this such that the the read-out electronics are in the bottom-left (e.g. (1, 0)).
+        The rotation is based on this such that the read-out electronics are in the bottom-left (e.g. (1, 0)).
 
     Returns
     -------
     ndarray
         The rotated array where the read out electronics are at the bottom left corner, (1, 0).
     """
     if roe_corner == (1, 0):
@@ -57,15 +57,15 @@
     ----------
     region
         The coordinates on the image of the (y0, y1, x0, y1) ``Region2D`` that are rotated.
     shape_native
         The 2D shape of the `Array2D` the regions are located on, required to determine the rotated `region`.
     roe_corner
         The corner of the ``Array2D``at which the read-out electronics are located (e.g. (1, 1) is the bottom-right corner).
-        The rotation is based on this such that the the read-out electronics are in the bottom-left (e.g. (1, 0)).
+        The rotation is based on this such that the read-out electronics are in the bottom-left (e.g. (1, 0)).
 
     Returns
     -------
     aa.Region2D
         The rotated (y0, y1, x0, x1) ``Region2D`` where the read out electronics are at the bottom left corner, (1, 0).
     """
     if region is None:
@@ -113,15 +113,15 @@
     ----------
     pattern_ci : ac.CIPaattern
         The charge-injection pattern of the ``Array2D`` that is rotated.
     shape_native
         The 2D shape of the ``Array2D`` the regions are located on, required to determine the rotated ``region``.
     roe_corner
         The corner of the ``Array2D``at which the read-out electronics are located (e.g. (1, 1) is the bottom-right corner).
-        The rotation is based on this such that the the read-out electronics are in the bottom-left (e.g. (1, 0)).
+        The rotation is based on this such that the read-out electronics are in the bottom-left (e.g. (1, 0)).
 
     Returns
     -------
     aa.Region2D
         The rotated (y0, y1, x0, x1) ``Region2D`` where the read out electronics are at the bottom left corner, (1, 0).
     """
     new_pattern_ci = deepcopy(pattern_ci)
@@ -135,15 +135,14 @@
 
     return new_pattern_ci
 
 
 def region_after_extraction(
     original_region: Region2DLike, extraction_region: Region2DLike
 ) -> Optional[Region2D]:
-
     if original_region is None:
         return None
 
     y0, y1 = x0x1_after_extraction(
         x0o=original_region[0],
         x1o=original_region[1],
         x0e=extraction_region[0],
```

### Comparing `autoarray-2023.3.27.1/autoarray/layout/region.py` & `autoarray-2023.7.7.1/autoarray/layout/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         Parameters
         ----------
         pixels
             A tuple defining the pixel coordinates used to compute the front region.
         """
 
         if pixels_from_end is not None:
-
             pixels = (self.total_pixels - pixels_from_end, self.total_pixels)
 
         x_min = self.x0 + pixels[0]
         x_max = self.x0 + pixels[1]
 
         return Region1D((x_min, x_max))
 
@@ -248,15 +247,14 @@
         pixels_from_end
             Alternative row pixel index specification, which extracts this number of pixels from the end of
             the region. For example, if the region is 100 pixels and `pixels_from_end=10`, the last 10 pixels of
             the region are extracted.
         """
 
         if pixels_from_end is not None:
-
             pixels = (self.total_rows - pixels_from_end, self.total_rows)
 
         y_coord = self.y0
         y_min = y_coord + pixels[0]
         y_max = y_coord + pixels[1]
 
         return Region2D((y_min, y_max, self.x0, self.x1))
@@ -322,15 +320,14 @@
         Parameters
         ----------
         pixels
             A tuple defining the pixel columns used to compute the serial front region.
         """
 
         if pixels_from_end is not None:
-
             pixels = (self.total_columns - pixels_from_end, self.total_columns)
 
         x_min, x_max = self.serial_x_front_range_from(pixels)
         return Region2D(region=(self.y0, self.y1, x_min, x_max))
 
     def serial_trailing_region_from(
         self, pixels: Tuple[int, int] = (0, 1)
```

### Comparing `autoarray-2023.3.27.1/autoarray/mask/abstract_mask.py` & `autoarray-2023.7.7.1/autoarray/mask/abstract_mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from autoarray import type as ty
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class Mask(AbstractNDArray, ABC):
-
     pixel_scales = None
 
     # noinspection PyUnusedLocal
     def __new__(
         cls,
         mask: np.ndarray,
         origin: tuple,
@@ -52,15 +51,14 @@
         obj = mask.view(cls)
         obj.sub_size = sub_size
         obj.pixel_scales = pixel_scales
         obj.origin = origin
         return obj
 
     def __array_finalize__(self, obj):
-
         if isinstance(obj, Mask):
             self.sub_size = obj.sub_size
             self.pixel_scales = obj.pixel_scales
             self.origin = obj.origin
         else:
             self.sub_size = 1
             self.pixel_scales = None
```

### Comparing `autoarray-2023.3.27.1/autoarray/mask/derive/grid_1d.py` & `autoarray-2023.7.7.1/autoarray/mask/derive/grid_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/mask/derive/grid_2d.py` & `autoarray-2023.7.7.1/autoarray/mask/derive/grid_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/mask/derive/indexes_2d.py` & `autoarray-2023.7.7.1/autoarray/mask/derive/indexes_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/mask/derive/mask_1d.py` & `autoarray-2023.7.7.1/autoarray/mask/derive/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/mask/derive/mask_2d.py` & `autoarray-2023.7.7.1/autoarray/mask/derive/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/mask/mask_1d.py` & `autoarray-2023.7.7.1/autoarray/mask/mask_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 
 class Mask1D(Mask):
     def __new__(
         cls,
         mask: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
         sub_size: int = 1,
-        origin: Tuple[
-            float,
-        ] = (0.0,),
+        origin: Tuple[float,] = (0.0,),
         invert: bool = False,
     ):
         """
         A 1D mask, representing 1D data on a uniform line of pixels with equal spacing.
 
         When applied to 1D data it extracts or masks the unmasked image pixels corresponding to mask entries that
         are `False` or 0).
@@ -71,15 +69,14 @@
             mask=mask,
             pixel_scales=pixel_scales,
             sub_size=sub_size,
             origin=origin,
         )
 
     def __array_finalize__(self, obj):
-
         super().__array_finalize__(obj=obj)
 
         if isinstance(obj, Mask1D):
             pass
         else:
             self.origin = (0.0,)
```

### Comparing `autoarray-2023.3.27.1/autoarray/mask/mask_1d_util.py` & `autoarray-2023.7.7.1/autoarray/mask/mask_1d_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,13 @@
     sub_native_index_for_sub_slim_index_1d = np.zeros(shape=total_sub_pixels)
 
     sub_slim_index = 0
 
     for x in range(mask_1d.shape[0]):
         if not mask_1d[x]:
             for x1 in range(sub_size):
-
                 sub_native_index_for_sub_slim_index_1d[sub_slim_index] = (
                     x * sub_size
                 ) + x1
                 sub_slim_index += 1
 
     return sub_native_index_for_sub_slim_index_1d
```

### Comparing `autoarray-2023.3.27.1/autoarray/mask/mask_2d.py` & `autoarray-2023.7.7.1/autoarray/mask/mask_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from autoarray.mask import mask_2d_util
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class Mask2D(Mask):
-
     # noinspection PyUnusedLocal
     def __new__(
         cls,
         mask: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
         sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
@@ -293,15 +292,14 @@
             sub_size=sub_size,
             origin=origin,
         )
 
         return obj
 
     def __array_finalize__(self, obj):
-
         super().__array_finalize__(obj=obj)
 
         if not isinstance(obj, Mask2D):
             self.origin = (0.0, 0.0)
 
     @property
     def geometry(self) -> Geometry2D:
@@ -871,15 +869,14 @@
         y0, x0 = np.amin(where, axis=1)
         y1, x1 = np.amax(where, axis=1)
 
         return (y1 - y0 + 1, x1 - x0 + 1)
 
     @property
     def zoom_centre(self) -> Tuple[float, float]:
-
         extraction_grid_1d = self.geometry.grid_pixels_2d_from(
             grid_scaled_2d=self.derive_grid.unmasked_sub_1.slim
         )
         y_pixels_max = np.max(extraction_grid_1d[:, 0])
         y_pixels_min = np.min(extraction_grid_1d[:, 0])
         x_pixels_max = np.max(extraction_grid_1d[:, 1])
         x_pixels_min = np.min(extraction_grid_1d[:, 1])
@@ -887,26 +884,24 @@
         return (
             ((y_pixels_max + y_pixels_min - 1.0) / 2.0),
             ((x_pixels_max + x_pixels_min - 1.0) / 2.0),
         )
 
     @property
     def zoom_offset_pixels(self) -> Tuple[float, float]:
-
         if self.pixel_scales is None:
             return self.geometry.central_pixel_coordinates
 
         return (
             self.zoom_centre[0] - self.geometry.central_pixel_coordinates[0],
             self.zoom_centre[1] - self.geometry.central_pixel_coordinates[1],
         )
 
     @property
     def zoom_offset_scaled(self) -> Tuple[float, float]:
-
         return (
             -self.pixel_scales[0] * self.zoom_offset_pixels[0],
             self.pixel_scales[1] * self.zoom_offset_pixels[1],
         )
 
     @property
     def zoom_region(self) -> List[int]:
```

### Comparing `autoarray-2023.3.27.1/autoarray/mask/mask_2d_util.py` & `autoarray-2023.7.7.1/autoarray/mask/mask_2d_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
     """
 
     total_sparse_pixels = 0
 
     for unmasked_sparse_pixel_index in range(
         unmasked_sparse_grid_pixel_centres.shape[0]
     ):
-
         y = unmasked_sparse_grid_pixel_centres[unmasked_sparse_pixel_index, 0]
         x = unmasked_sparse_grid_pixel_centres[unmasked_sparse_pixel_index, 1]
 
         if not mask_2d[y, x]:
             total_sparse_pixels += 1
 
     return total_sparse_pixels
@@ -176,15 +175,14 @@
 
     centres_scaled = mask_2d_centres_from(
         shape_native=mask_2d.shape, pixel_scales=pixel_scales, centre=centre
     )
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
-
             y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
             x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
 
             r_scaled = np.sqrt(x_scaled**2 + y_scaled**2)
 
             if r_scaled <= radius:
                 mask_2d[y, x] = False
@@ -233,15 +231,14 @@
 
     centres_scaled = mask_2d_centres_from(
         shape_native=mask_2d.shape, pixel_scales=pixel_scales, centre=centre
     )
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
-
             y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
             x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
 
             r_scaled = np.sqrt(x_scaled**2 + y_scaled**2)
 
             if outer_radius >= r_scaled >= inner_radius:
                 mask_2d[y, x] = False
@@ -296,15 +293,14 @@
 
     centres_scaled = mask_2d_centres_from(
         shape_native=mask_2d.shape, pixel_scales=pixel_scales, centre=centre
     )
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
-
             y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
             x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
 
             r_scaled = np.sqrt(x_scaled**2 + y_scaled**2)
 
             if (
                 inner_radius >= r_scaled
@@ -334,15 +330,14 @@
         All input ``pixel_coordinates`` are buffed with `False` entries in all 8 neighboring directions by this
         amount.
     """
 
     mask_2d = np.full(shape=shape_native, fill_value=True)
 
     for y, x in pixel_coordinates:
-
         mask_2d[y, x] = False
 
     if buffer == 0:
         return mask_2d
     else:
         return buffed_mask_2d_from(mask_2d=mask_2d, buffer=buffer)
 
@@ -432,15 +427,14 @@
 
     centres_scaled = mask_2d_centres_from(
         shape_native=mask_2d.shape, pixel_scales=pixel_scales, centre=centre
     )
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
-
             y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
             x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
 
             r_scaled_elliptical = elliptical_radius_from(
                 y_scaled, x_scaled, angle, axis_ratio
             )
 
@@ -509,15 +503,14 @@
 
     centres_scaled = mask_2d_centres_from(
         shape_native=mask_2d.shape, pixel_scales=pixel_scales, centre=centre
     )
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
-
             y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
             x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
 
             inner_r_scaled_elliptical = elliptical_radius_from(
                 y_scaled, x_scaled, inner_phi, inner_axis_ratio
             )
 
@@ -683,28 +676,24 @@
         The 1D indexes of all unmasked pixels on the mask.
     """
 
     mask_pixel_total = 0
 
     for y in range(0, mask_2d.shape[0]):
         for x in range(0, mask_2d.shape[1]):
-
             if mask_2d[y, x] == return_masked_indexes:
-
                 mask_pixel_total += 1
 
     mask_pixels = np.zeros(mask_pixel_total)
     mask_index = 0
     regular_index = 0
 
     for y in range(0, mask_2d.shape[0]):
         for x in range(0, mask_2d.shape[1]):
-
             if mask_2d[y, x] == return_masked_indexes:
-
                 mask_pixels[mask_index] = regular_index
                 mask_index += 1
 
             regular_index += 1
 
     return mask_pixels
 
@@ -917,15 +906,14 @@
     int
         The total number of border pixels.
     """
 
     border_pixel_total = 0
 
     for i in range(edge_pixels.shape[0]):
-
         if check_if_border_pixel(mask_2d, edge_pixels[i], native_to_slim):
             border_pixel_total += 1
 
     return border_pixel_total
 
 
 @numba_util.jit()
@@ -986,21 +974,19 @@
     )
 
     border_pixels = np.zeros(border_pixel_total)
 
     border_pixel_index = 0
 
     for edge_pixel_index in range(edge_pixels.shape[0]):
-
         if check_if_border_pixel(
             mask_2d=mask_2d,
             edge_pixel_slim=edge_pixels[edge_pixel_index],
             native_to_slim=sub_native_index_for_sub_slim_index_2d,
         ):
-
             border_pixels[border_pixel_index] = edge_pixels[edge_pixel_index]
             border_pixel_index += 1
 
     return border_pixels
 
 
 def sub_border_pixel_slim_indexes_from(
@@ -1044,15 +1030,15 @@
     )
 
     sub_grid_2d_slim = grid_2d_util.grid_2d_slim_via_mask_from(
         mask_2d=mask_2d, pixel_scales=(1.0, 1.0), sub_size=sub_size, origin=(0.0, 0.0)
     )
     mask_centre = grid_2d_util.grid_2d_centre_from(grid_2d_slim=sub_grid_2d_slim)
 
-    for (border_1d_index, border_pixel) in enumerate(border_pixels):
+    for border_1d_index, border_pixel in enumerate(border_pixels):
         sub_border_pixels_of_border_pixel = sub_slim_indexes_for_slim_index[
             int(border_pixel)
         ]
 
         sub_border_pixels[
             border_1d_index
         ] = grid_2d_util.furthest_grid_2d_slim_index_from(
@@ -1085,15 +1071,14 @@
     buffed_mask_2d = mask_2d.copy()
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
             if not mask_2d[y, x]:
                 for y0 in range(y - buffer, y + 1 + buffer):
                     for x0 in range(x - buffer, x + 1 + buffer):
-
                         if (
                             y0 >= 0
                             and x0 >= 0
                             and y0 <= mask_2d.shape[0] - 1
                             and x0 <= mask_2d.shape[1] - 1
                         ):
                             buffed_mask_2d[y0, x0] = False
@@ -1414,15 +1399,14 @@
     )
 
     mask_index = 0
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
             if not mask_2d[y, x]:
-
                 flag = True
 
                 if x + 1 < mask_2d.shape[1]:
                     if not mask_2d[y, x + 1]:
                         mask_neighbors[
                             mask_index
                         ] = sub_slim_index_for_sub_native_index[y, x + 1]
```

### Comparing `autoarray-2023.3.27.1/autoarray/mock.py` & `autoarray-2023.7.7.1/autoarray/mock.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/numba_util.py` & `autoarray-2023.7.7.1/autoarray/numba_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,50 +27,44 @@
     parallel = conf.instance["general"]["numba"]["parallel"]
 except Exception:
     nopython = True
     cache = True
     parallel = False
 
 try:
-
     import numba
 
 except ModuleNotFoundError:
-
     logger.warning(
         f"\n******************************************************************************\n"
-        f"Numba is not being used, either because it is disabled in `config.general.ini` "
+        f"Numba is not being used, either because it is disabled in `config/general.yaml` "
         f"or because it is not installed.\n\n. "
         f"This will lead to slow performance.\n\n. "
         f"Install numba as described at the following webpage for improved performance. \n"
         f"********************************************************************************"
     )
 
 
 def jit(nopython=nopython, cache=cache, parallel=parallel):
     def wrapper(func):
-
         try:
             use_numba = conf.instance["general"]["numba"]["use_numba"]
 
             if not use_numba:
                 return func
 
         except KeyError:
-
             pass
 
         try:
-
             import numba
 
             return numba.jit(func, nopython=nopython, cache=cache, parallel=parallel)
 
         except ModuleNotFoundError:
-
             return func
 
     return wrapper
 
 
 def profile_func(func: Callable):
     """
@@ -122,26 +116,22 @@
         last_key_after_call = (
             list(obj.profiling_dict)[-1] if obj.profiling_dict else None
         )
 
         profile_call_max = 5
 
         for i in range(profile_call_max):
-
             key_func = f"{func.__name__}_{i}"
 
             if key_func not in obj.profiling_dict:
-
                 if last_key_before_call == last_key_after_call:
                     obj.profiling_dict[key_func] = time_func
                 else:
                     for key, value in reversed(list(obj.profiling_dict.items())):
-
                         if last_key_before_call == key:
-
                             obj.profiling_dict[key_func] = time_func
                             break
 
                         time_func -= obj.profiling_dict[key]
 
                 break
```

### Comparing `autoarray-2023.3.27.1/autoarray/operators/convolver.py` & `autoarray-2023.7.7.1/autoarray/operators/convolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,32 +347,28 @@
         image_frame_1d_kernels,
         image_frame_1d_lengths,
         blurring_1d_array,
         blurring_frame_1d_indexes,
         blurring_frame_1d_kernels,
         blurring_frame_1d_lengths,
     ):
-
         blurred_image_1d = np.zeros(image_1d_array.shape)
 
         for image_1d_index in range(len(image_1d_array)):
-
             frame_1d_indexes = image_frame_1d_indexes[image_1d_index]
             frame_1d_kernel = image_frame_1d_kernels[image_1d_index]
             frame_1d_length = image_frame_1d_lengths[image_1d_index]
             image_value = image_1d_array[image_1d_index]
 
             for kernel_1d_index in range(frame_1d_length):
-
                 vector_index = frame_1d_indexes[kernel_1d_index]
                 kernel_value = frame_1d_kernel[kernel_1d_index]
                 blurred_image_1d[vector_index] += image_value * kernel_value
 
         for blurring_1d_index in range(len(blurring_1d_array)):
-
             frame_1d_indexes = blurring_frame_1d_indexes[blurring_1d_index]
             frame_1d_kernel = blurring_frame_1d_kernels[blurring_1d_index]
             frame_1d_length = blurring_frame_1d_lengths[blurring_1d_index]
             image_value = blurring_1d_array[blurring_1d_index]
 
             for kernel_1d_index in range(frame_1d_length):
                 vector_index = frame_1d_indexes[kernel_1d_index]
@@ -425,26 +421,23 @@
     @numba_util.jit()
     def convolve_no_blurring_jit(
         image_1d_array,
         image_frame_1d_indexes,
         image_frame_1d_kernels,
         image_frame_1d_lengths,
     ):
-
         blurred_image_1d = np.zeros(image_1d_array.shape)
 
         for image_1d_index in range(len(image_1d_array)):
-
             frame_1d_indexes = image_frame_1d_indexes[image_1d_index]
             frame_1d_kernel = image_frame_1d_kernels[image_1d_index]
             frame_1d_length = image_frame_1d_lengths[image_1d_index]
             image_value = image_1d_array[image_1d_index]
 
             for kernel_1d_index in range(frame_1d_length):
-
                 vector_index = frame_1d_indexes[kernel_1d_index]
                 kernel_value = frame_1d_kernel[kernel_1d_index]
                 blurred_image_1d[vector_index] += image_value * kernel_value
 
         return blurred_image_1d
 
     def convolve_mapping_matrix(self, mapping_matrix):
@@ -476,15 +469,15 @@
 
         And source pixel 2:
 
         [[0.0, 0.0, 0.0]],
         [[0.0, 1.0, 1.0]]
         [[0.0, 0.0, 0.0]]
 
-        We then convolve each of these with our PSF kernel, in 2 dimensions, like we would a hyper grid. For
+        We then convolve each of these with our PSF kernel, in 2 dimensions, like we would a grid. For
         example, using the kernel below:
 
         kernel:
 
         [[0.0, 0.1, 0.0]]
         [[0.1, 0.6, 0.1]]
         [[0.0, 0.1, 0.0]]
@@ -529,24 +522,21 @@
     @numba_util.jit()
     def convolve_matrix_jit(
         mapping_matrix,
         image_frame_1d_indexes,
         image_frame_1d_kernels,
         image_frame_1d_lengths,
     ):
-
         blurred_mapping_matrix = np.zeros(mapping_matrix.shape)
 
         for pixel_1d_index in range(mapping_matrix.shape[1]):
             for image_1d_index in range(mapping_matrix.shape[0]):
-
                 value = mapping_matrix[image_1d_index, pixel_1d_index]
 
                 if value > 0:
-
                     frame_1d_indexes = image_frame_1d_indexes[image_1d_index]
                     frame_1d_kernel = image_frame_1d_kernels[image_1d_index]
                     frame_1d_length = image_frame_1d_lengths[image_1d_index]
 
                     for kernel_1d_index in range(frame_1d_length):
                         vector_index = frame_1d_indexes[kernel_1d_index]
                         kernel_value = frame_1d_kernel[kernel_1d_index]
```

### Comparing `autoarray-2023.3.27.1/autoarray/operators/transformer.py` & `autoarray-2023.7.7.1/autoarray/operators/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,58 +11,53 @@
 class PyLopsPlaceholder:
     pass
 
 
 try:
     from pynufft.linalg.nufft_cpu import NUFFT_cpu
 except ModuleNotFoundError:
-
     NUFFT_cpu = NUFFTPlaceholder
 
 try:
     import pylops
 
     PyLopsOperator = pylops.LinearOperator
 except ModuleNotFoundError:
-
     PyLopsOperator = PyLopsPlaceholder
 
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.visibilities import Visibilities
 
 from autoarray.structures.arrays import array_2d_util
 from autoarray.operators import transformer_util
 
 
 def pynufft_exception():
-
     raise ModuleNotFoundError(
         "\n--------------------\n"
         "You are attempting to perform interferometer analysis.\n\n"
         "However, the optional library PyNUFFT (https://github.com/jyhmiinlin/pynufft) is not installed.\n\n"
         "Install it via the command `pip install pynufft==2022.2.2`.\n\n"
         "----------------------"
     )
 
 
 def pylops_exception():
-
     raise ModuleNotFoundError(
         "\n--------------------\n"
         "You are attempting to perform interferometer analysis.\n\n"
         "However, the optional library PyLops (https://github.com/PyLops/pylops) is not installed.\n\n"
         "Install it via the command `pip install pylops==1.18.3`.\n\n"
         "----------------------"
     )
 
 
 class TransformerDFT(PyLopsOperator):
     def __init__(self, uv_wavelengths, real_space_mask, preload_transform=True):
-
         if isinstance(self, PyLopsPlaceholder):
             pylops_exception()
 
         super().__init__()
 
         self.uv_wavelengths = uv_wavelengths.astype("float")
         self.real_space_mask = real_space_mask.derive_mask.sub_1
@@ -70,15 +65,14 @@
 
         self.total_visibilities = uv_wavelengths.shape[0]
         self.total_image_pixels = self.real_space_mask.pixels_in_mask
 
         self.preload_transform = preload_transform
 
         if preload_transform:
-
             self.preload_real_transforms = transformer_util.preload_real_transforms(
                 grid_radians=self.grid, uv_wavelengths=self.uv_wavelengths
             )
 
             self.preload_imag_transforms = transformer_util.preload_imag_transforms(
                 grid_radians=self.grid, uv_wavelengths=self.uv_wavelengths
             )
@@ -94,35 +88,31 @@
 
         # NOTE: This is the scaling factor that needs to be applied to the adjoint operator
         self.adjoint_scaling = (2.0 * self.grid.shape_native[0]) * (
             2.0 * self.grid.shape_native[1]
         )
 
     def visibilities_from(self, image):
-
         if self.preload_transform:
-
             visibilities = transformer_util.visibilities_via_preload_jit_from(
                 image_1d=image.binned,
                 preloaded_reals=self.preload_real_transforms,
                 preloaded_imags=self.preload_imag_transforms,
             )
 
         else:
-
             visibilities = transformer_util.visibilities_jit(
                 image_1d=image.binned,
                 grid_radians=self.grid,
                 uv_wavelengths=self.uv_wavelengths,
             )
 
         return Visibilities(visibilities=visibilities)
 
     def image_from(self, visibilities, use_adjoint_scaling: bool = False):
-
         image_slim = transformer_util.image_via_jit_from(
             n_pixels=self.grid.shape[0],
             grid_radians=self.grid,
             uv_wavelengths=self.uv_wavelengths,
             visibilities=visibilities.in_array,
         )
 
@@ -131,35 +121,31 @@
             mask_2d=self.real_space_mask,
             sub_size=self.real_space_mask.sub_size,
         )
 
         return Array2D(values=image_native, mask=self.real_space_mask)
 
     def transform_mapping_matrix(self, mapping_matrix):
-
         if self.preload_transform:
-
             return transformer_util.transformed_mapping_matrix_via_preload_jit_from(
                 mapping_matrix=mapping_matrix,
                 preloaded_reals=self.preload_real_transforms,
                 preloaded_imags=self.preload_imag_transforms,
             )
 
         else:
-
             return transformer_util.transformed_mapping_matrix_jit(
                 mapping_matrix=mapping_matrix,
                 grid_radians=self.grid,
                 uv_wavelengths=self.uv_wavelengths,
             )
 
 
 class TransformerNUFFT(NUFFT_cpu, PyLopsOperator):
     def __init__(self, uv_wavelengths, real_space_mask):
-
         if isinstance(self, NUFFTPlaceholder):
             pynufft_exception()
 
         if isinstance(self, PyLopsPlaceholder):
             pylops_exception()
 
         super(TransformerNUFFT, self).__init__()
@@ -209,15 +195,14 @@
 
         # NOTE: This is the scaling factor that needs to be applied to the adjoint operator
         self.adjoint_scaling = (2.0 * self.grid.shape_native[0]) * (
             2.0 * self.grid.shape_native[1]
         )
 
     def initialize_plan(self, ratio=2, interp_kernel=(6, 6)):
-
         if not isinstance(ratio, int):
             ratio = int(ratio)
 
         # ... NOTE : The u,v coordinated should be given in the order ...
         visibilities_normalized = np.array(
             [
                 self.uv_wavelengths[:, 1]
@@ -247,31 +232,27 @@
         return Visibilities(
             visibilities=self.forward(
                 image.binned.native[::-1, :]
             )  # flip due to PyNUFFT internal flip
         )
 
     def image_from(self, visibilities, use_adjoint_scaling: bool = False):
-
         image = np.real(self.adjoint(visibilities))[::-1, :]
 
         if use_adjoint_scaling:
-
             image *= self.adjoint_scaling
 
         return Array2D(values=image, mask=self.real_space_mask)
 
     def transform_mapping_matrix(self, mapping_matrix):
-
         transformed_mapping_matrix = 0 + 0j * np.zeros(
             (self.uv_wavelengths.shape[0], mapping_matrix.shape[1])
         )
 
         for source_pixel_1d_index in range(mapping_matrix.shape[1]):
-
             image_2d = array_2d_util.array_2d_native_from(
                 array_2d_slim=mapping_matrix[:, source_pixel_1d_index],
                 mask_2d=self.grid.mask,
                 sub_size=1,
             )
 
             image = Array2D(values=image_2d, mask=self.grid.mask)
@@ -311,15 +292,14 @@
                     with the size of Nd or Nd + (batch, )
         :rtype: numpy array with the dtype of numpy.complex64
         """
 
         warnings.filterwarnings("ignore")
 
         def a_complex_from(a_real, a_imag):
-
             return a_real + 1j * a_imag
 
         y = a_complex_from(
             a_real=y[: int(self.shape[0] / 2.0)], a_imag=y[int(self.shape[0] / 2.0) :]
         )
 
         x2d = np.real(self.xx2x(self.k2xx(self.y2k(y))))
```

### Comparing `autoarray-2023.3.27.1/autoarray/operators/transformer_util.py` & `autoarray-2023.7.7.1/autoarray/operators/transformer_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
             )
 
     return preloaded_real_transforms
 
 
 @numba_util.jit()
 def preload_imag_transforms(grid_radians, uv_wavelengths):
-
     preloaded_imag_transforms = np.zeros(
         shape=(grid_radians.shape[0], uv_wavelengths.shape[0])
     )
 
     for image_1d_index in range(grid_radians.shape[0]):
         for vis_1d_index in range(uv_wavelengths.shape[0]):
             preloaded_imag_transforms[image_1d_index, vis_1d_index] += np.sin(
@@ -70,15 +69,14 @@
             )
 
     return preloaded_imag_transforms
 
 
 @numba_util.jit()
 def visibilities_via_preload_jit_from(image_1d, preloaded_reals, preloaded_imags):
-
     visibilities = 0 + 0j * np.zeros(shape=(preloaded_reals.shape[1]))
 
     for image_1d_index in range(image_1d.shape[0]):
         for vis_1d_index in range(preloaded_reals.shape[1]):
             vis_real = (
                 image_1d[image_1d_index] * preloaded_reals[image_1d_index, vis_1d_index]
             )
@@ -88,15 +86,14 @@
             visibilities[vis_1d_index] += vis_real + 1j * vis_imag
 
     return visibilities
 
 
 @numba_util.jit()
 def visibilities_jit(image_1d, grid_radians, uv_wavelengths):
-
     visibilities = 0 + 0j * np.zeros(shape=(uv_wavelengths.shape[0]))
 
     for image_1d_index in range(image_1d.shape[0]):
         for vis_1d_index in range(uv_wavelengths.shape[0]):
             vis_real = image_1d[image_1d_index] * np.cos(
                 -2.0
                 * np.pi
@@ -116,20 +113,18 @@
             visibilities[vis_1d_index] += vis_real + 1j * vis_imag
 
     return visibilities
 
 
 @numba_util.jit()
 def image_via_jit_from(n_pixels, grid_radians, uv_wavelengths, visibilities):
-
     image_1d = np.zeros(n_pixels)
 
     for image_1d_index in range(image_1d.shape[0]):
         for vis_1d_index in range(uv_wavelengths.shape[0]):
-
             image_1d[image_1d_index] += visibilities[vis_1d_index, 0] * np.cos(
                 2.0
                 * np.pi
                 * (
                     grid_radians[image_1d_index, 1] * uv_wavelengths[vis_1d_index, 0]
                     + grid_radians[image_1d_index, 0] * uv_wavelengths[vis_1d_index, 1]
                 )
@@ -147,53 +142,45 @@
     return image_1d
 
 
 @numba_util.jit()
 def transformed_mapping_matrix_via_preload_jit_from(
     mapping_matrix, preloaded_reals, preloaded_imags
 ):
-
     transfomed_mapping_matrix = 0 + 0j * np.zeros(
         (preloaded_reals.shape[1], mapping_matrix.shape[1])
     )
 
     for pixel_1d_index in range(mapping_matrix.shape[1]):
         for image_1d_index in range(mapping_matrix.shape[0]):
-
             value = mapping_matrix[image_1d_index, pixel_1d_index]
 
             if value > 0:
-
                 for vis_1d_index in range(preloaded_reals.shape[1]):
-
                     vis_real = value * preloaded_reals[image_1d_index, vis_1d_index]
                     vis_imag = value * preloaded_imags[image_1d_index, vis_1d_index]
                     transfomed_mapping_matrix[vis_1d_index, pixel_1d_index] += (
                         vis_real + 1j * vis_imag
                     )
 
     return transfomed_mapping_matrix
 
 
 @numba_util.jit()
 def transformed_mapping_matrix_jit(mapping_matrix, grid_radians, uv_wavelengths):
-
     transfomed_mapping_matrix = 0 + 0j * np.zeros(
         (uv_wavelengths.shape[0], mapping_matrix.shape[1])
     )
 
     for pixel_1d_index in range(mapping_matrix.shape[1]):
         for image_1d_index in range(mapping_matrix.shape[0]):
-
             value = mapping_matrix[image_1d_index, pixel_1d_index]
 
             if value > 0:
-
                 for vis_1d_index in range(uv_wavelengths.shape[0]):
-
                     vis_real = value * np.cos(
                         -2.0
                         * np.pi
                         * (
                             grid_radians[image_1d_index, 1]
                             * uv_wavelengths[vis_1d_index, 0]
                             + grid_radians[image_1d_index, 0]
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/__init__.py` & `autoarray-2023.7.7.1/autoarray/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/abstract_plotters.py` & `autoarray-2023.7.7.1/autoarray/plot/abstract_plotters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from autoconf import conf
+
 from autoarray.plot.wrap.base.abstract import set_backend
 
 set_backend()
 
 import matplotlib.pyplot as plt
 from typing import Optional, Tuple
 
@@ -21,51 +23,46 @@
         mat_plot_1d: MatPlot1D = None,
         visuals_1d: Visuals1D = None,
         include_1d: Include1D = None,
         mat_plot_2d: MatPlot2D = None,
         visuals_2d: Visuals2D = None,
         include_2d: Include2D = None,
     ):
-
         self.visuals_1d = visuals_1d
         self.include_1d = include_1d
         self.mat_plot_1d = mat_plot_1d
 
         self.visuals_2d = visuals_2d
         self.include_2d = include_2d
         self.mat_plot_2d = mat_plot_2d
 
         self.subplot_figsize = None
 
     def set_title(self, label):
-
         if self.mat_plot_1d is not None:
             self.mat_plot_1d.title.manual_label = label
 
         if self.mat_plot_2d is not None:
             self.mat_plot_2d.title.manual_label = label
 
     def set_filename(self, filename):
-
         if self.mat_plot_1d is not None:
             self.mat_plot_1d.output.filename = filename
 
         if self.mat_plot_2d is not None:
             self.mat_plot_2d.output.filename = filename
 
     def set_format(self, format):
-
         if self.mat_plot_1d is not None:
             self.mat_plot_1d.output._format = format
 
         if self.mat_plot_2d is not None:
             self.mat_plot_2d.output._format = format
 
     def set_mat_plot_1d_for_multi_plot(self, is_for_multi_plot, color: str):
-
         self.mat_plot_1d.set_for_multi_plot(
             is_for_multi_plot=is_for_multi_plot, color=color
         )
 
     def set_mat_plots_for_subplot(
         self, is_for_subplot, number_subplots=None, subplot_shape=None
     ):
@@ -78,15 +75,14 @@
             self.mat_plot_2d.set_for_subplot(is_for_subplot=is_for_subplot)
             self.mat_plot_2d.number_subplots = number_subplots
             self.mat_plot_2d.subplot_shape = subplot_shape
             self.mat_plot_2d.subplot_index = 1
 
     @property
     def is_for_subplot(self):
-
         if self.mat_plot_1d is not None:
             if self.mat_plot_1d.is_for_subplot:
                 return True
 
         if self.mat_plot_2d is not None:
             if self.mat_plot_2d.is_for_subplot:
                 return True
@@ -95,15 +91,16 @@
 
     def open_subplot_figure(
         self,
         number_subplots: int,
         subplot_shape: Optional[Tuple[int, int]] = None,
         subplot_figsize: Optional[Tuple[int, int]] = None,
     ):
-        """Setup a figure for plotting an image.
+        """
+        Setup a figure for plotting an image.
 
         Parameters
         ----------
         figsize
             The size of the figure in (total_y_pixels, total_x_pixels).
         as_subplot
             If the figure is a subplot, the setup_figure function is omitted to ensure that each subplot does not create a \
@@ -118,24 +115,24 @@
 
         self.subplot_figsize = subplot_figsize
 
         figsize = self.get_subplot_figsize(number_subplots=number_subplots)
         plt.figure(figsize=figsize)
 
     def close_subplot_figure(self):
-
         try:
             self.mat_plot_2d.figure.close()
         except AttributeError:
             self.mat_plot_1d.figure.close()
         self.set_mat_plots_for_subplot(is_for_subplot=False)
         self.subplot_figsize = None
 
     def get_subplot_figsize(self, number_subplots):
-        """Get the size of a sub plotter in (total_y_pixels, total_x_pixels), based on the number of subplots that are going to be plotted.
+        """
+        Get the size of a sub plotter in (total_y_pixels, total_x_pixels), based on the number of subplots that are going to be plotted.
 
         Parameters
         ----------
         number_subplots
             The number of subplots that are to be plotted in the figure.
         """
 
@@ -146,41 +143,43 @@
             if self.mat_plot_1d.figure.config_dict["figsize"] is not None:
                 return self.mat_plot_1d.figure.config_dict["figsize"]
 
         if self.mat_plot_2d is not None:
             if self.mat_plot_2d.figure.config_dict["figsize"] is not None:
                 return self.mat_plot_2d.figure.config_dict["figsize"]
 
-        if number_subplots <= 2:
-            return (18, 8)
-        elif number_subplots <= 4:
-            return (13, 10)
-        elif number_subplots <= 6:
-            return (18, 12)
-        elif number_subplots <= 9:
-            return (25, 20)
-        elif number_subplots <= 12:
-            return (25, 20)
-        elif number_subplots <= 16:
-            return (25, 20)
-        elif number_subplots <= 20:
-            return (25, 20)
-        else:
-            return (25, 20)
+        try:
+            subplot_shape = self.mat_plot_1d.get_subplot_shape(
+                number_subplots=number_subplots
+            )
+        except AttributeError:
+            subplot_shape = self.mat_plot_2d.get_subplot_shape(
+                number_subplots=number_subplots
+            )
+
+        subplot_shape_to_figsize_factor = conf.instance["visualize"]["general"][
+            "subplot_shape_to_figsize_factor"
+        ]
+        subplot_shape_to_figsize_factor = tuple(
+            map(int, subplot_shape_to_figsize_factor[1:-1].split(","))
+        )
 
-    def _subplot_custom_plot(self, **kwargs):
+        return (
+            subplot_shape[1] * subplot_shape_to_figsize_factor[1],
+            subplot_shape[0] * subplot_shape_to_figsize_factor[0],
+        )
 
+    def _subplot_custom_plot(self, **kwargs):
         figures_dict = dict(
             (key, value) for key, value in kwargs.items() if value is True
         )
 
         self.open_subplot_figure(number_subplots=len(figures_dict))
 
         for index, (key, value) in enumerate(figures_dict.items()):
-
             if value:
                 try:
                     self.figures_2d(**{key: True})
                 except AttributeError:
                     self.figures_1d(**{key: True})
 
         try:
@@ -191,19 +190,17 @@
             self.mat_plot_1d.output.subplot_to_figure(
                 auto_filename=kwargs["auto_labels"].filename
             )
 
         self.close_subplot_figure()
 
     def subplot_of_plotters_figure(self, plotter_list, name):
-
         self.open_subplot_figure(number_subplots=len(plotter_list))
 
         for i, plotter in enumerate(plotter_list):
-
             plotter.figures_2d(**{name: True})
 
         self.mat_plot_2d.output.subplot_to_figure(auto_filename=f"subplot_{name}")
 
         self.close_subplot_figure()
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/get_visuals/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/get_visuals/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/get_visuals/one_d.py` & `autoarray-2023.7.7.1/autoarray/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/get_visuals/two_d.py` & `autoarray-2023.7.7.1/autoarray/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/include/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/include/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/include/one_d.py` & `autoarray-2023.7.7.1/autoarray/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/include/two_d.py` & `autoarray-2023.7.7.1/autoarray/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/mat_plot/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/mat_plot/abstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from autoconf import conf
+
 from autoarray.plot.wrap.base.abstract import set_backend
 
 set_backend()
 
 import copy
 import matplotlib.pyplot as plt
 from typing import Optional, List, Tuple, Union
 
 from autoarray.plot.wrap import base as wb
+from autoarray import exc
 
 
 class AbstractMatPlot:
     def __init__(
         self,
         units: Optional[wb.Units] = None,
         figure: Optional[wb.Figure] = None,
@@ -120,16 +123,16 @@
 
         A `MatPlot` class contains many of the `MatWrap` objects which customize matplotlib figures. One
         may have a standard `MatPlot` object, which customizes many figures in the same way, for example:
 
         mat_plot_2d_base = aplt.MatPlot2D(
             yticks=aplt.YTicks(fontsize=18),
             xticks=aplt.XTicks(fontsize=18),
-            ylabel=aplt.YLabel(label=""),
-            xlabel=aplt.XLabel(label=""),
+            ylabel=aplt.YLabel(ylabel=""),
+            xlabel=aplt.XLabel(xlabel=""),
         )
 
         However, one may require many unique `MatPlot` objects for a number of different figures, which all use
         these settings. These can be created by creating the unique `MatPlot` objects and adding the above object
         to each:
 
         mat_plot_2d = aplt.MatPlot2D(
@@ -144,78 +147,85 @@
 
         mat_plot_2d = mat_plot_2d + mat_plot_2d_base
         """
 
         other = copy.deepcopy(other)
 
         for attr, value in self.__dict__.items():
-
             try:
                 if value.kwargs.get("is_default") is not True:
                     other.__dict__[attr] = value
             except AttributeError:
                 pass
 
         return other
 
     def set_for_subplot(self, is_for_subplot: bool):
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
         self.is_for_subplot = is_for_subplot
         self.output.bypass = is_for_subplot
 
         for attr, value in self.__dict__.items():
             if hasattr(value, "is_for_subplot"):
                 value.is_for_subplot = is_for_subplot
 
-    def get_subplot_rows_columns(self, number_subplots):
+    def get_subplot_shape(self, number_subplots):
         """
         Get the size of a sub plotter in (total_y_pixels, total_x_pixels), based on the number of subplots that are
         going to be plotted.
 
         Parameters
         ----------
         number_subplots
             The number of subplots that are to be plotted in the figure.
         """
 
         if self.subplot_shape is not None:
             return self.subplot_shape
 
-        if number_subplots <= 2:
-            return 1, 2
-        elif number_subplots <= 4:
-            return 2, 2
-        elif number_subplots <= 6:
-            return 2, 3
-        elif number_subplots <= 9:
-            return 3, 3
-        elif number_subplots <= 12:
-            return 3, 4
-        elif number_subplots <= 16:
-            return 4, 4
-        elif number_subplots <= 20:
-            return 4, 5
-        else:
-            return 6, 6
+        subplot_shape_dict = conf.instance["visualize"]["general"]["subplot_shape"]
+
+        try:
+            subplot_shape = subplot_shape_dict[number_subplots]
+        except KeyError:
+            try:
+                key = min(
+                    filter(lambda x: x > number_subplots, subplot_shape_dict.keys())
+                )
+                subplot_shape = subplot_shape_dict[key]
+            except ValueError:
+                raise exc.PlottingException(
+                    f"""
+                    The number of subplots is greater than the maximum number of subplots specified
+                    in the visualization/general.yaml config file, in the section "subplot_shape".
+                    
+                    The total number of subplots in the figure is {number_subplots}, whereas this config file only
+                    specifies the subplot shape for up to a number of subplots less than this.
+
+                    To fix this, add a new entry to the "subplot_shape" section of the visualization/general.yaml.           
+                    """
+                )
+
+        return tuple(map(int, subplot_shape[1:-1].split(",")))
 
     def setup_subplot(
         self,
         aspect: Optional[Tuple[float, float]] = None,
-        subplot_rows_columns: Tuple[int, int] = None,
+        subplot_shape: Tuple[int, int] = None,
     ):
         """
         Setup a new figure to be plotted on a subplot, which is used by a `Plotter` when plotting multiple images
         on a subplot.
 
         Every time a new figure is plotted on the subplot, the counter `subplot_index` increases by 1.
 
@@ -225,26 +235,26 @@
 
         Every time
 
         Parameters
         ----------
         aspect
             The aspect ratio of the overall subplot.
-        subplot_rows_columns
+        subplot_shape
             The number of rows and columns in the subplot.
         """
-        if subplot_rows_columns is None:
-            rows, columns = self.get_subplot_rows_columns(
-                number_subplots=self.number_subplots
-            )
-        else:
-            rows = subplot_rows_columns[0]
-            columns = subplot_rows_columns[1]
+        if subplot_shape is None:
+            subplot_shape = self.get_subplot_shape(number_subplots=self.number_subplots)
 
         if aspect is None:
-            ax = plt.subplot(rows, columns, self.subplot_index)
+            ax = plt.subplot(subplot_shape[0], subplot_shape[1], self.subplot_index)
         else:
-            ax = plt.subplot(rows, columns, self.subplot_index, aspect=float(aspect))
+            ax = plt.subplot(
+                subplot_shape[0],
+                subplot_shape[1],
+                self.subplot_index,
+                aspect=float(aspect),
+            )
 
         self.subplot_index += 1
 
         return ax
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/mat_plot/one_d.py` & `autoarray-2023.7.7.1/autoarray/plot/mat_plot/one_d.py`

 * *Files 15% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self.is_for_subplot = False
 
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
@@ -146,17 +146,19 @@
         visuals_1d: Visuals1D,
         auto_labels: AutoLabels,
         x: Optional[Union[np.ndarray, Iterable, List, Array1D]] = None,
         plot_axis_type_override: Optional[str] = None,
         y_errors=None,
         x_errors=None,
         y_extra=None,
+        ls_errorbar="",
+        text_manual_dict=None,
+        text_manual_dict_y=None,
         bypass: bool = False,
     ):
-
         if (y is None) or np.count_nonzero(y) == 0:
             return
 
         ax = None
 
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
@@ -186,59 +188,96 @@
             y=y,
             x=x,
             label=auto_labels.legend,
             plot_axis_type=plot_axis_type,
             y_errors=y_errors,
             x_errors=x_errors,
             y_extra=y_extra,
+            ls_errorbar=ls_errorbar,
         )
 
         if visuals_1d.shaded_region is not None:
-
             self.fill_between.fill_between_shaded_regions(
                 x=x, y1=visuals_1d.shaded_region[0], y2=visuals_1d.shaded_region[1]
             )
 
         if "extent" in self.axis.config_dict:
             self.axis.set()
 
-        self.ylabel.set(units=self.units, include_brackets=False)
-        self.xlabel.set(units=self.units, include_brackets=False)
-
         self.tickparams.set()
 
         if plot_axis_type == "symlog":
             plt.yscale("symlog")
 
+        if x_errors is not None:
+            min_value_x = np.nanmin(x - x_errors)
+            max_value_x = np.nanmax(x + x_errors)
+        else:
+            min_value_x = np.nanmin(x)
+            max_value_x = np.nanmax(x)
+
+        if y_errors is not None:
+            min_value_y = np.nanmin(y - y_errors)
+            max_value_y = np.nanmax(y + y_errors)
+        else:
+            min_value_y = np.nanmin(y)
+            max_value_y = np.nanmax(y)
+
         self.xticks.set(
-            array=x,
-            min_value=np.min(x),
-            max_value=np.max(x),
+            min_value=min_value_x,
+            max_value=max_value_x,
+            pixels=len(x),
             units=self.units,
             use_integers=use_integers,
+            is_for_1d_plot=True,
         )
 
-        # TODO : Implement properly
-
-        # self.yticks.set(
-        #     array=y,
-        #     min_value=np.min(y),
-        #     max_value=np.max(y),
-        #     units=self.units,
-        # )
+        self.yticks.set(
+            min_value=min_value_y,
+            max_value=max_value_y,
+            pixels=len(y),
+            units=self.units,
+            yunit=auto_labels.yunit,
+            is_for_1d_plot=True,
+            is_log10="logy" in plot_axis_type,
+        )
 
         self.title.set(auto_title=auto_labels.title)
-        self.ylabel.set(units=self.units, auto_label=auto_labels.ylabel)
-        self.xlabel.set(units=self.units, auto_label=auto_labels.xlabel)
+        self.ylabel.set(auto_label=auto_labels.ylabel)
+        self.xlabel.set(auto_label=auto_labels.xlabel)
 
         if not isinstance(self.text, list):
             self.text.set()
         else:
             [text.set() for text in self.text]
 
+        # This is a horrific hack to get CTI plots to work, refactor one day.
+
+        from autoarray.plot.wrap.base.text import Text
+
+        if text_manual_dict is not None and ax is not None:
+            y = text_manual_dict_y
+            text_manual_list = []
+
+            for key, value in text_manual_dict.items():
+                text_manual_list.append(
+                    Text(
+                        x=0.95,
+                        y=y,
+                        s=f"{key} : {value}",
+                        c="b",
+                        transform=ax.transAxes,
+                        horizontalalignment="right",
+                        fontsize=12,
+                    )
+                )
+                y = y - 0.05
+
+            [text.set() for text in text_manual_list]
+
         if not isinstance(self.annotate, list):
             self.annotate.set()
         else:
             [annotate.set() for annotate in self.annotate]
 
         visuals_1d.plot_via_plotter(plotter=self)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/mat_plot/two_d.py` & `autoarray-2023.7.7.1/autoarray/plot/mat_plot/two_d.py`

 * *Files 11% similar despite different names*

```diff
@@ -239,89 +239,88 @@
 
         if array.mask.is_all_false:
             buffer = 0
         else:
             buffer = 1
 
         if conf.instance["visualize"]["general"]["general"]["zoom_around_mask"]:
-
             extent = array.extent_of_zoomed_array(buffer=buffer)
             array = array.zoomed_around_mask(buffer=buffer)
 
         else:
-
             extent = array.geometry.extent
 
         ax = None
 
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
         else:
             if not bypass:
                 ax = self.setup_subplot()
 
         aspect = self.figure.aspect_from(shape_native=array.shape_native)
-        norm_scale = self.cmap.norm_from(array=array)
+        norm = self.cmap.norm_from(array=array)
 
         origin = conf.instance["visualize"]["general"]["general"]["imshow_origin"]
 
         plt.imshow(
             X=array.native,
             aspect=aspect,
             cmap=self.cmap.cmap,
-            norm=norm_scale,
+            norm=norm,
             extent=extent,
             origin=origin,
         )
 
         if visuals_2d.array_overlay is not None:
             self.array_overlay.overlay_array(
                 array=visuals_2d.array_overlay, figure=self.figure
             )
 
         extent_axis = self.axis.config_dict.get("extent")
 
         if extent_axis is None:
-
             extent_axis = extent
 
         self.axis.set(extent=extent_axis)
 
         self.tickparams.set()
 
         self.yticks.set(
-            array=array,
             min_value=extent_axis[2],
             max_value=extent_axis[3],
             units=self.units,
+            pixels=array.shape_native[0],
         )
 
         self.xticks.set(
-            array=array,
             min_value=extent_axis[0],
             max_value=extent_axis[1],
             units=self.units,
+            pixels=array.shape_native[1],
         )
 
         self.title.set(auto_title=auto_labels.title)
-        self.ylabel.set(units=self.units, include_brackets=True)
-        self.xlabel.set(units=self.units, include_brackets=True)
+        self.ylabel.set()
+        self.xlabel.set()
 
         if not isinstance(self.text, list):
             self.text.set()
         else:
             [text.set() for text in self.text]
 
         if not isinstance(self.annotate, list):
             self.annotate.set()
         else:
             [annotate.set() for annotate in self.annotate]
 
         if self.colorbar is not False:
-            cb = self.colorbar.set(ax=ax)
+            cb = self.colorbar.set(
+                units=self.units, ax=ax, norm=norm, cb_unit=auto_labels.cb_unit
+            )
             self.colorbar_tickparams.set(cb=cb)
 
         grid_indexes = None
 
         if visuals_2d.indexes is not None or visuals_2d.pix_indexes is not None:
             grid_indexes = array.mask.derive_grid.unmasked
 
@@ -354,24 +353,22 @@
 
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
         else:
             ax = self.setup_subplot()
 
         if color_array is None:
-
             if y_errors is None and x_errors is None:
                 self.grid_scatter.scatter_grid(grid=grid)
             else:
                 self.grid_errorbar.errorbar_grid(
                     grid=grid, y_errors=y_errors, x_errors=x_errors
                 )
 
         elif color_array is not None:
-
             cmap = plt.get_cmap(self.cmap.cmap)
 
             if y_errors is None and x_errors is None:
                 self.grid_scatter.scatter_grid_colored(
                     grid=grid, color_array=color_array, cmap=cmap
                 )
             else:
@@ -380,153 +377,143 @@
                     cmap=cmap,
                     color_array=color_array,
                     y_errors=y_errors,
                     x_errors=x_errors,
                 )
 
             if self.colorbar is not None:
-
                 colorbar = self.colorbar.set_with_color_values(
-                    cmap=self.cmap.cmap, color_values=color_array, ax=ax
+                    units=self.units,
+                    cmap=self.cmap.cmap,
+                    color_values=color_array,
+                    ax=ax,
                 )
                 if colorbar is not None and self.colorbar_tickparams is not None:
                     self.colorbar_tickparams.set(cb=colorbar)
 
         self.title.set(auto_title=auto_labels.title)
-        self.ylabel.set(units=self.units, include_brackets=True)
-        self.xlabel.set(units=self.units, include_brackets=True)
+        self.ylabel.set()
+        self.xlabel.set()
 
         if not isinstance(self.text, list):
             self.text.set()
         else:
             [text.set() for text in self.text]
 
         if not isinstance(self.annotate, list):
             self.annotate.set()
         else:
             [annotate.set() for annotate in self.annotate]
 
         extent = self.axis.config_dict.get("extent")
 
         if extent is None:
-
             extent = np.asarray(grid.geometry.extent)
             extent = extent + (buffer * extent)
 
         self.axis.set(extent=extent, grid=grid)
 
         self.tickparams.set()
 
         if not self.axis.symmetric_around_centre:
-            self.yticks.set(
-                array=None, min_value=extent[2], max_value=extent[3], units=self.units
-            )
-            self.xticks.set(
-                array=None, min_value=extent[0], max_value=extent[1], units=self.units
-            )
+            self.yticks.set(min_value=extent[2], max_value=extent[3], units=self.units)
+            self.xticks.set(min_value=extent[0], max_value=extent[1], units=self.units)
 
         visuals_2d.plot_via_plotter(plotter=self, grid_indexes=grid)
 
         if not self.is_for_subplot:
             self.output.to_figure(structure=grid, auto_filename=auto_labels.filename)
             self.figure.close()
 
     def plot_mapper(
         self,
         mapper: Union[MapperRectangularNoInterp, MapperVoronoiNoInterp],
         visuals_2d: Visuals2D,
         auto_labels: AutoLabels,
-        interpolate_to_uniform: bool = True,
-        source_pixelization_values=None,
+        interpolate_to_uniform: bool = False,
+        pixel_values: np.ndarray = Optional[None],
+        zoom_to_brightest: bool = True,
     ):
-
         if isinstance(mapper, MapperRectangularNoInterp):
-
             self._plot_rectangular_mapper(
                 mapper=mapper,
                 visuals_2d=visuals_2d,
                 auto_labels=auto_labels,
-                interpolate_to_uniform=interpolate_to_uniform,
-                source_pixelization_values=source_pixelization_values,
+                pixel_values=pixel_values,
+                zoom_to_brightest=zoom_to_brightest,
             )
 
         elif isinstance(mapper, MapperDelaunay):
             self._plot_delaunay_mapper(
                 mapper=mapper,
                 visuals_2d=visuals_2d,
                 auto_labels=auto_labels,
                 interpolate_to_uniform=interpolate_to_uniform,
-                source_pixelization_values=source_pixelization_values,
+                pixel_values=pixel_values,
+                zoom_to_brightest=zoom_to_brightest,
             )
         else:
-
             self._plot_voronoi_mapper(
                 mapper=mapper,
                 visuals_2d=visuals_2d,
                 auto_labels=auto_labels,
                 interpolate_to_uniform=interpolate_to_uniform,
-                source_pixelization_values=source_pixelization_values,
+                pixel_values=pixel_values,
+                zoom_to_brightest=zoom_to_brightest,
             )
 
     def _plot_rectangular_mapper(
         self,
         mapper: MapperRectangularNoInterp,
         visuals_2d: Visuals2D,
         auto_labels: AutoLabels,
-        interpolate_to_uniform: bool = True,
-        source_pixelization_values=None,
+        pixel_values: np.ndarray = Optional[None],
+        zoom_to_brightest: bool = True,
     ):
-
-        if source_pixelization_values is not None:
-
+        if pixel_values is not None:
             solution_array_2d = array_2d_util.array_2d_native_from(
-                array_2d_slim=source_pixelization_values,
+                array_2d_slim=pixel_values,
                 mask_2d=np.full(
                     fill_value=False, shape=mapper.source_plane_mesh_grid.shape_native
                 ),
                 sub_size=1,
             )
 
-            source_pixelization_values = Array2D.no_mask(
+            pixel_values = Array2D.no_mask(
                 values=solution_array_2d,
                 sub_size=1,
                 pixel_scales=mapper.source_plane_mesh_grid.pixel_scales,
                 origin=mapper.source_plane_mesh_grid.origin,
             )
 
         extent = self.axis.config_dict.get("extent")
-        extent = (
-            extent
-            if extent is not None
-            else mapper.source_plane_mesh_grid.geometry.extent
-        )
+        if extent is None:
+            extent = mapper.extent_from(
+                values=pixel_values, zoom_to_brightest=zoom_to_brightest
+            )
 
         aspect_inv = self.figure.aspect_for_subplot_from(extent=extent)
 
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
         else:
             ax = self.setup_subplot(aspect=aspect_inv)
 
-        if source_pixelization_values is not None:
+        if pixel_values is not None:
             self.plot_array(
-                array=source_pixelization_values,
+                array=pixel_values,
                 visuals_2d=visuals_2d,
                 auto_labels=auto_labels,
                 bypass=True,
             )
 
         self.axis.set(extent=extent, grid=mapper.source_plane_mesh_grid)
 
-        self.yticks.set(
-            array=None, min_value=extent[2], max_value=extent[3], units=self.units
-        )
-        self.xticks.set(
-            array=None, min_value=extent[0], max_value=extent[1], units=self.units
-        )
+        self.yticks.set(min_value=extent[2], max_value=extent[3], units=self.units)
+        self.xticks.set(min_value=extent[0], max_value=extent[1], units=self.units)
 
         if not isinstance(self.text, list):
             self.text.set()
         else:
             [text.set() for text in self.text]
 
         if not isinstance(self.annotate, list):
@@ -537,162 +524,163 @@
         self.grid_plot.plot_rectangular_grid_lines(
             extent=mapper.source_plane_mesh_grid.geometry.extent,
             shape_native=mapper.shape_native,
         )
 
         self.title.set(auto_title=auto_labels.title)
         self.tickparams.set()
-        self.ylabel.set(units=self.units, include_brackets=True)
-        self.xlabel.set(units=self.units, include_brackets=True)
+        self.ylabel.set()
+        self.xlabel.set()
 
         visuals_2d.plot_via_plotter(
             plotter=self, grid_indexes=mapper.source_plane_data_grid, mapper=mapper
         )
 
         if not self.is_for_subplot:
             self.output.to_figure(structure=None, auto_filename=auto_labels.filename)
             self.figure.close()
 
     def _plot_delaunay_mapper(
         self,
         mapper: MapperDelaunay,
         visuals_2d: Visuals2D,
         auto_labels: AutoLabels,
-        interpolate_to_uniform: bool = True,
-        source_pixelization_values=None,
+        interpolate_to_uniform: bool = False,
+        pixel_values: np.ndarray = Optional[None],
+        zoom_to_brightest: bool = True,
     ):
-
         extent = self.axis.config_dict.get("extent")
-        extent = (
-            extent
-            if extent is not None
-            else mapper.source_plane_mesh_grid.geometry.extent
-        )
+        if extent is None:
+            extent = mapper.extent_from(
+                values=pixel_values, zoom_to_brightest=zoom_to_brightest
+            )
 
         aspect_inv = self.figure.aspect_for_subplot_from(extent=extent)
 
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
         else:
             ax = self.setup_subplot(aspect=aspect_inv)
 
         self.axis.set(extent=extent, grid=mapper.source_plane_mesh_grid)
 
         self.tickparams.set()
-        self.yticks.set(
-            array=None, min_value=extent[2], max_value=extent[3], units=self.units
-        )
-        self.xticks.set(
-            array=None, min_value=extent[0], max_value=extent[1], units=self.units
-        )
+        self.yticks.set(min_value=extent[2], max_value=extent[3], units=self.units)
+        self.xticks.set(min_value=extent[0], max_value=extent[1], units=self.units)
 
         if not isinstance(self.text, list):
             self.text.set()
         else:
             [text.set() for text in self.text]
 
         if not isinstance(self.annotate, list):
             self.annotate.set()
         else:
             [annotate.set() for annotate in self.annotate]
 
-        self.interpolated_reconstruction.imshow_reconstruction(
+        interpolation_array = self.interpolated_reconstruction.imshow_reconstruction(
             mapper=mapper,
-            pixel_values=source_pixelization_values,
+            pixel_values=pixel_values,
+            units=self.units,
             cmap=self.cmap,
             colorbar=self.colorbar,
             colorbar_tickparams=self.colorbar_tickparams,
             aspect=aspect_inv,
             ax=ax,
         )
 
         self.title.set(auto_title=auto_labels.title)
-        self.ylabel.set(units=self.units, include_brackets=True)
-        self.xlabel.set(units=self.units, include_brackets=True)
+        self.ylabel.set()
+        self.xlabel.set()
 
         visuals_2d.plot_via_plotter(
             plotter=self, grid_indexes=mapper.source_plane_data_grid, mapper=mapper
         )
 
         if not self.is_for_subplot:
-            self.output.to_figure(structure=None, auto_filename=auto_labels.filename)
+            self.output.to_figure(
+                structure=interpolation_array, auto_filename=auto_labels.filename
+            )
             self.figure.close()
 
     def _plot_voronoi_mapper(
         self,
         mapper: MapperVoronoiNoInterp,
         visuals_2d: Visuals2D,
         auto_labels: AutoLabels,
-        interpolate_to_uniform: bool = True,
-        source_pixelization_values=None,
+        interpolate_to_uniform: bool = False,
+        pixel_values: np.ndarray = Optional[None],
+        zoom_to_brightest: bool = True,
     ):
-
         extent = self.axis.config_dict.get("extent")
-        extent = (
-            extent
-            if extent is not None
-            else mapper.source_plane_mesh_grid.geometry.extent
-        )
+
+        if extent is None:
+            extent = mapper.extent_from(
+                values=pixel_values, zoom_to_brightest=zoom_to_brightest
+            )
 
         aspect_inv = self.figure.aspect_for_subplot_from(extent=extent)
 
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
         else:
             ax = self.setup_subplot(aspect=aspect_inv)
 
         self.axis.set(extent=extent, grid=mapper.source_plane_mesh_grid)
 
         plt.gca().set_aspect(aspect_inv)
 
         self.tickparams.set()
-        self.yticks.set(
-            array=None, min_value=extent[2], max_value=extent[3], units=self.units
-        )
-        self.xticks.set(
-            array=None, min_value=extent[0], max_value=extent[1], units=self.units
-        )
+        self.yticks.set(min_value=extent[2], max_value=extent[3], units=self.units)
+        self.xticks.set(min_value=extent[0], max_value=extent[1], units=self.units)
 
         if not isinstance(self.text, list):
             self.text.set()
         else:
             [text.set() for text in self.text]
 
         if not isinstance(self.annotate, list):
             self.annotate.set()
         else:
             [annotate.set() for annotate in self.annotate]
 
         if not interpolate_to_uniform:
-
             self.voronoi_drawer.draw_voronoi_pixels(
                 mapper=mapper,
-                pixel_values=source_pixelization_values,
+                units=self.units,
+                pixel_values=pixel_values,
                 cmap=self.cmap,
                 colorbar=self.colorbar,
                 colorbar_tickparams=self.colorbar_tickparams,
                 ax=ax,
             )
 
         else:
-
             self.interpolated_reconstruction.imshow_reconstruction(
                 mapper=mapper,
-                pixel_values=source_pixelization_values,
+                pixel_values=pixel_values,
+                units=self.units,
                 cmap=self.cmap,
                 colorbar=self.colorbar,
                 colorbar_tickparams=self.colorbar_tickparams,
                 aspect=aspect_inv,
                 ax=ax,
             )
 
         self.title.set(auto_title=auto_labels.title)
-        self.ylabel.set(units=self.units, include_brackets=True)
-        self.xlabel.set(units=self.units, include_brackets=True)
+        self.ylabel.set()
+        self.xlabel.set()
 
         visuals_2d.plot_via_plotter(
             plotter=self, grid_indexes=mapper.source_plane_data_grid, mapper=mapper
         )
 
+        if pixel_values is not None:
+            interpolation_array = mapper.interpolated_array_from(values=pixel_values)
+        else:
+            interpolation_array = None
+
         if not self.is_for_subplot:
-            self.output.to_figure(structure=None, auto_filename=auto_labels.filename)
+            self.output.to_figure(
+                structure=interpolation_array, auto_filename=auto_labels.filename
+            )
             self.figure.close()
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/multi_plotters.py` & `autoarray-2023.7.7.1/autoarray/plot/multi_plotters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-class MultiFigurePlotter:
-    def __init__(self, plotter_list):
+from typing import Tuple
 
-        self.plotter_list = plotter_list
 
-    def subplot_of_figure(self, func_name, figure_name, **kwargs):
+class MultiFigurePlotter:
+    def __init__(self, plotter_list, subplot_shape: Tuple[int, int] = None):
+        self.plotter_list = plotter_list
+        self.subplot_shape = subplot_shape
 
+    def subplot_of_figure(self, func_name, figure_name, filename_suffix="", **kwargs):
         number_subplots = len(self.plotter_list)
 
-        self.plotter_list[0].open_subplot_figure(number_subplots=number_subplots)
+        self.plotter_list[0].open_subplot_figure(
+            number_subplots=number_subplots, subplot_shape=self.subplot_shape
+        )
 
         for i, plotter in enumerate(self.plotter_list):
-
             func = getattr(plotter, func_name)
             func(**{**{figure_name: True}, **kwargs})
 
         if self.plotter_list[0].mat_plot_1d is not None:
             self.plotter_list[0].mat_plot_1d.output.subplot_to_figure(
-                auto_filename=f"subplot_{figure_name}_list"
+                auto_filename=f"subplot_{figure_name}{filename_suffix}_list"
             )
         if self.plotter_list[0].mat_plot_2d is not None:
             self.plotter_list[0].mat_plot_2d.output.subplot_to_figure(
-                auto_filename=f"subplot_{figure_name}_list"
+                auto_filename=f"subplot_{figure_name}{filename_suffix}_list"
             )
         self.plotter_list[0].close_subplot_figure()
 
 
 class MultiYX1DPlotter:
     def __init__(self, plotter_list, color_list=None, legend_labels=None):
-
         self.plotter_list = plotter_list
 
         if color_list is None:
             color_list = 10 * ["k", "r", "b", "g", "c", "m", "y"]
 
         self.color_list = color_list
         self.legend_labels = legend_labels
 
     def figure_1d(self, func_name, figure_name, **kwargs):
-
         self.plotter_list[0].mat_plot_1d.figure.open()
 
         for i, plotter in enumerate(self.plotter_list):
-
             plotter.set_mat_plot_1d_for_multi_plot(
                 is_for_multi_plot=True, color=self.color_list[i]
             )
 
             if self.legend_labels is not None:
                 plotter.mat_plot_1d.yx_plot.label = self.legend_labels[i]
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/visuals/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/visuals/abstract.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         include_2d = Include2D(mask=True)
         array_plotter = aplt.Array2DPlotter(array=masked_array, include_2d=include_2d)
         array_plotter.figure()
 
         Because `mask=True` in `Include2D` the function `figure` extracts the `Mask2D` from the `masked_array`
         and plots it. It does this by creating a new `Visuals2D` object.
 
-        If the user did not manually input a `Visuals2d` object, the one created in `function_array` is the one used to
+        If the user did not manually input a `Visuals2D` object, the one created in `function_array` is the one used to
         plot the image
 
         However, if the user specifies their own `Visuals2D` object and passed it to the plotter, e.g.:
 
         visuals_2d = Visuals2D(origin=(0.0, 0.0))
         include_2d = Include2D(mask=True)
         array_plotter = aplt.Array2DPlotter(array=masked_array, include_2d=include_2d)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/visuals/one_d.py` & `autoarray-2023.7.7.1/autoarray/plot/visuals/one_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,25 @@
         self,
         origin: Optional[Grid1D] = None,
         mask: Optional[Mask1D] = None,
         points: Optional[Grid1D] = None,
         vertical_line: Optional[float] = None,
         shaded_region: Optional[List[Union[List, Array1D, np.ndarray]]] = None,
     ):
-
         self.origin = origin
         self.mask = mask
         self.points = points
         self.vertical_line = vertical_line
         self.shaded_region = shaded_region
 
     @property
     def include(self):
         return Include1D()
 
     def plot_via_plotter(self, plotter):
-
         if self.points is not None:
-
             plotter.yx_scatter.scatter_yx(y=self.points, x=np.arange(len(self.points)))
 
         if self.vertical_line is not None:
-
             plotter.vertical_line_axvline.axvline_vertical_line(
                 vertical_line=self.vertical_line
             )
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/visuals/two_d.py` & `autoarray-2023.7.7.1/autoarray/plot/visuals/two_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         array_overlay: Optional[Array2D] = None,
         parallel_overscan=None,
         serial_prescan=None,
         serial_overscan=None,
         indexes=None,
         pix_indexes=None,
     ):
-
         self.origin = origin
         self.mask = mask
         self.border = border
         self.lines = lines
         self.positions = positions
         self.grid = grid
         self.mesh_grid = mesh_grid
@@ -43,15 +42,14 @@
         self.parallel_overscan = parallel_overscan
         self.serial_prescan = serial_prescan
         self.serial_overscan = serial_overscan
         self.indexes = indexes
         self.pix_indexes = pix_indexes
 
     def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None):
-
         if self.origin is not None:
             plotter.origin_scatter.scatter_grid(
                 grid=Grid2DIrregular(values=self.origin)
             )
 
         if self.mask is not None:
             plotter.mask_scatter.scatter_grid(
@@ -81,13 +79,12 @@
 
         if self.indexes is not None:
             plotter.index_scatter.scatter_grid_indexes(
                 grid=grid_indexes, indexes=self.indexes
             )
 
         if self.pix_indexes is not None and mapper is not None:
-
             indexes = mapper.pix_indexes_for_slim_indexes(pix_indexes=self.pix_indexes)
 
             plotter.index_scatter.scatter_grid_indexes(
                 grid=mapper.source_plane_data_grid, indexes=indexes
             )
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/__init__.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/abstract.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         hpc_mode = False
 
     if hpc_mode:
         matplotlib.use("Agg")
 
 
 def remove_spaces_and_commas_from(colors):
-
     colors = [color.strip(",").strip(" ") for color in colors]
     colors = list(filter(None, colors))
     if len(colors) == 1:
         return colors[0]
     return colors
 
 
@@ -64,39 +63,33 @@
         aplt.Array2D(values=arr, plotter=plotter)
 
         The `Plotter` object is detailed in the `autoarray.plot.plotter` package.
 
         The matplotlib wrapper objects in ths module also use configuration files to choose their default settings.
         For example, in `autoarray.config.visualize.mat_base.Figure.ini` you will note the section:
 
-        [figure]
+        figure:
         figsize=(7, 7)
 
-        [subplot]
+        subplot:
         figsize=auto
 
         This specifies that when a data structure (like the `Array2D` above) is plotted, the figsize will always
         be  (7,7) when a single figure is plotted and it will be chosen automatically if a subplot is plotted. This
         allows one to customize the matplotlib settings of every plot in a project.
         """
 
         self.is_for_subplot = False
         self.kwargs = kwargs
 
     @property
     def config_dict(self):
-
-        if not self.is_for_subplot:
-            category = "figure"
-        else:
-            category = "subplot"
-
         config_dict = conf.instance["visualize"][self.config_folder][
             self.__class__.__name__
-        ][category]
+        ][self.config_category]
 
         if "c" in config_dict:
             config_dict["c"] = remove_spaces_and_commas_from(colors=config_dict["c"])
 
         config_dict = {**config_dict, **self.kwargs}
 
         if "c" in config_dict:
@@ -107,7 +100,13 @@
             config_dict.pop("is_default")
 
         return config_dict
 
     @property
     def config_folder(self):
         return "mat_wrap"
+
+    @property
+    def config_category(self):
+        if self.is_for_subplot:
+            return "subplot"
+        return "figure"
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/annotate.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/annotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 
     This object wraps the following Matplotlib methods:
 
     - plt.annotate: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.text.html
     """
 
     def set(self):
-
         if "x" not in self.kwargs and "y" not in self.kwargs and "s" not in self.kwargs:
             return
 
         plt.annotate(**self.config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/axis.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,25 +38,23 @@
         config_dict = self.config_dict
         extent_dict = config_dict.get("extent")
 
         if extent_dict is not None:
             config_dict.pop("extent")
 
         if self.symmetric_around_centre:
-
             ymin = np.min(grid[:, 0])
             ymax = np.max(grid[:, 0])
             xmin = np.min(grid[:, 1])
             xmax = np.max(grid[:, 1])
 
             x = np.max([np.abs(xmin), np.abs(xmax)])
             y = np.max([np.abs(ymin), np.abs(ymax)])
 
             extent_symmetric = [-x, x, -y, y]
 
             return plt.axis(extent_symmetric, **config_dict)
 
         else:
-
             if extent_dict is not None:
                 return plt.axis(extent_dict, **config_dict)
             return plt.axis(extent, **config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/cmap.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/cmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,29 +35,26 @@
 
         super().__init__(**kwargs)
 
         self._symmetric = symmetric
 
     @property
     def symmetric(self):
-
         cmap = copy.copy(self)
 
         cmap._symmetric = True
 
         return cmap
 
     def vmin_from(self, array: np.ndarray):
-
         if self.config_dict["vmin"] is None:
             return np.min(array)
         return self.config_dict["vmin"]
 
     def vmax_from(self, array: np.ndarray):
-
         if self.config_dict["vmax"] is None:
             return np.max(array)
         return self.config_dict["vmax"]
 
     def norm_from(self, array: np.ndarray) -> object:
         """
         Returns the `Normalization` object which scales of the colormap.
@@ -76,21 +73,14 @@
 
         if self._symmetric:
             if vmin < 0.0 and vmax > 0.0:
                 if abs(vmin) > abs(vmax):
                     vmax = abs(vmin)
                 else:
                     vmin = -vmax
-            else:
-                logger.info(
-                    """
-                    Cannot make symmetric Cmap (e.g. vmax = -vmin) because 
-                    both vmin and vmax are positive or negative.
-                    """
-                )
 
         if isinstance(self.config_dict["norm"], colors.Normalize):
             return self.config_dict["norm"]
 
         if self.config_dict["norm"] in "linear":
             return colors.Normalize(vmin=vmin, vmax=vmax)
         elif self.config_dict["norm"] in "log":
@@ -110,15 +100,13 @@
         raise exc.PlottingException(
             "The normalization (norm) supplied to the plotter is not a valid string must be "
             "{linear, log, symmetric_log}"
         )
 
     @property
     def cmap(self):
-
         if self.config_dict["cmap"] == "default":
-
             from autoarray.plot.wrap.segmentdata import segmentdata
 
             return LinearSegmentedColormap(name="default", segmentdata=segmentdata)
 
         return self.config_dict["cmap"]
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/colorbar.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/voronoi_drawer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,86 @@
 import matplotlib.pyplot as plt
-import matplotlib.cm as cm
 import numpy as np
-from typing import List, Optional
+from typing import Optional
 
-from autoarray.plot.wrap.base.abstract import AbstractMatWrap
+from autoarray.plot.wrap.two_d.abstract import AbstractMatWrap2D
+from autoarray.plot.wrap.base.units import Units
+from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoiNoInterp
+from autoarray.inversion.pixelization.mesh import mesh_util
 
-from autoarray import exc
+from autoarray.plot.wrap import base as wb
 
 
-class Colorbar(AbstractMatWrap):
-    def __init__(
-        self,
-        manual_tick_labels: Optional[List[float]] = None,
-        manual_tick_values: Optional[List[float]] = None,
-        manual_alignment: Optional[str] = None,
-        **kwargs,
-    ):
-        """
-        Customizes the colorbar of the plotted figure.
+class VoronoiDrawer(AbstractMatWrap2D):
+    """
+    Draws Voronoi pixels from a `MapperVoronoiNoInterp` object (see `inversions.mapper`). This includes both drawing
+    each Voronoi cell and coloring it according to a color value.
 
-        This object wraps the following Matplotlib method:
+    The mapper contains the grid of (y,x) coordinate where the centre of each Voronoi cell is plotted.
 
-        - plt.colorbar: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.colorbar.html
+    This object wraps methods described in below:
 
-        The colorbar object `cb` that is created is also customized using the following methods:
+    https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.fill.html
+    """
 
-        - cb.set_yticklabels: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.axes.Axes.set_yticklabels.html
+    def draw_voronoi_pixels(
+        self,
+        mapper: MapperVoronoiNoInterp,
+        pixel_values: Optional[np.ndarray],
+        units: Units,
+        cmap: Optional[wb.Cmap],
+        colorbar: Optional[wb.Colorbar],
+        colorbar_tickparams: Optional[wb.ColorbarTickParams] = None,
+        ax=None,
+    ):
+        """
+        Draws the Voronoi pixels of the input `mapper` using its `mesh_grid` which contains the (y,x)
+        coordinate of the centre of every Voronoi cell. This uses the method `plt.fill`.
 
         Parameters
         ----------
-        manual_tick_labels
-            Manually override the colorbar tick labels to an input list of float.
-        manual_tick_values
-            If the colorbar tick labels are manually specified the locations on the colorbar they appear running 0 -> 1.
+        mapper
+            A mapper object which contains the Voronoi mesh.
+        pixel_values
+            An array used to compute the color values that every Voronoi cell is plotted using.
+        cmap
+            The colormap used to plot each Voronoi cell.
+        colorbar
+            The `Colorbar` object in `mat_base` used to set the colorbar of the figure the Voronoi mesh is plotted on.
         """
 
-        super().__init__(**kwargs)
+        if ax is None:
+            ax = plt.gca()
 
-        self.manual_tick_labels = manual_tick_labels
-        self.manual_tick_values = manual_tick_values
-        self.manual_alignment = manual_alignment
+        regions, vertices = mesh_util.voronoi_revised_from(voronoi=mapper.voronoi)
 
-    def set(self, ax=None):
-        """
-        Set the figure's colorbar, optionally overriding the tick labels and values with manual inputs.
-        """
+        if pixel_values is not None:
+            vmin = cmap.vmin_from(array=pixel_values)
+            vmax = cmap.vmax_from(array=pixel_values)
 
-        if self.manual_tick_values is None and self.manual_tick_labels is None:
-            cb = plt.colorbar(**self.config_dict, ax=ax)
-        elif (
-            self.manual_tick_values is not None and self.manual_tick_labels is not None
-        ):
-            cb = plt.colorbar(ticks=self.manual_tick_values, ax=ax, **self.config_dict)
-            cb.ax.set_yticklabels(
-                labels=self.manual_tick_labels, va=self.manual_alignment or "center"
-            )
-        else:
-            raise exc.PlottingException(
-                "Only 1 entry of tick_values or tick_labels was input. You must either supply"
-                "both the values and labels, or neither."
-            )
+            color_values = np.where(pixel_values > vmax, vmax, pixel_values)
+            color_values = np.where(pixel_values < vmin, vmin, color_values)
 
-        return cb
+            if vmax != vmin:
+                color_array = (color_values - vmin) / (vmax - vmin)
+            else:
+                color_array = np.ones(color_values.shape[0])
 
-    def set_with_color_values(self, cmap: str, color_values: np.ndarray, ax=None):
-        """
-        Set the figure's colorbar using an array of already known color values.
+            cmap = plt.get_cmap(cmap.cmap)
 
-        This method is used for producing the color bar on a Voronoi mesh plot, which is unable to use the in-built
-        Matplotlib colorbar method.
+            if colorbar is not None:
+                cb = colorbar.set_with_color_values(
+                    units=units, cmap=cmap, color_values=color_values, ax=ax
+                )
 
-        Parameters
-        ----------
-        cmap
-            The colormap used to map normalized data values to RGBA
-            colors (see https://matplotlib.org/3.3.2/api/cm_api.html).
-        color_values
-            The values of the pixels on the Voronoi mesh which are used to create the colorbar.
-        """
+                if cb is not None and colorbar_tickparams is not None:
+                    colorbar_tickparams.set(cb=cb)
 
-        mappable = cm.ScalarMappable(cmap=cmap)
-        mappable.set_array(color_values)
+        else:
+            cmap = plt.get_cmap("Greys")
+            color_array = np.zeros(shape=mapper.pixels)
 
-        if self.manual_tick_values is None and self.manual_tick_labels is None:
-            cb = plt.colorbar(mappable=mappable, ax=ax, **self.config_dict)
-        elif (
-            self.manual_tick_values is not None and self.manual_tick_labels is not None
-        ):
-            cb = plt.colorbar(
-                mappable=mappable,
-                ax=ax,
-                ticks=self.manual_tick_values,
-                **self.config_dict,
-            )
-            cb.ax.set_yticklabels(
-                labels=self.manual_tick_labels, va=self.manual_alignment or "center"
-            )
+        for region, index in zip(regions, range(mapper.pixels)):
+            polygon = vertices[region]
+            color = cmap(color_array[index])
 
-        return cb
+            plt.fill(*zip(*polygon), facecolor=color, zorder=-1, **self.config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/figure.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/figure.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import matplotlib.pyplot as plt
 from typing import Union, Tuple
 
 from autoarray.plot.wrap.base.abstract import AbstractMatWrap
 
 
 class Aspect(Enum):
-
     square = 1
     auto = 2
     equal = 3
 
 
 class Figure(AbstractMatWrap):
     """
@@ -38,15 +37,14 @@
             config_dict["figsize"] = tuple(
                 map(int, config_dict["figsize"][1:-1].split(","))
             )
 
         return config_dict
 
     def aspect_for_subplot_from(self, extent):
-
         ratio = float((extent[1] - extent[0]) / (extent[3] - extent[2]))
 
         aspect = Aspect[self.config_dict["aspect"]]
 
         if aspect == Aspect.square:
             return ratio
         elif aspect == Aspect.auto:
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/legend.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/legend.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,21 +9,18 @@
 
     This object wraps the following Matplotlib methods:
 
     - plt.legend: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.legend.html
     """
 
     def __init__(self, include=True, **kwargs):
-
         super().__init__(**kwargs)
 
         self.include = include
 
     def set(self):
-
         if self.include:
-
             config_dict = self.config_dict
             config_dict.pop("include") if "include" in config_dict else None
             config_dict.pop("include_2d") if "include_2d" in config_dict else None
 
             plt.legend(**config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/output.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/output.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         path: Optional[str] = None,
         filename: Optional[str] = None,
         prefix: Optional[str] = None,
         suffix: Optional[str] = None,
         format: Union[str, List[str]] = None,
         format_folder: bool = False,
         bypass: bool = False,
-        bbox_inches: Optional[str] = None,
+        bbox_inches: str = "tight",
         **kwargs,
     ):
         """
         Sets how the figure or subplot is output, either by displaying it on the screen or writing it to hard-disk.
 
         This object wraps the following Matplotlib methods:
 
@@ -47,17 +47,14 @@
             If `True`, all images are output in a folder giving the format name, for
             example `path/to/output/png/filename.png`. This can make managing large image catalogues easier.
         bypass
             Whether to bypass the `plt.show` or `plt.savefig` methods, used when plotting a subplot.
         """
         self.path = path
 
-        if path is not None and path:
-            os.makedirs(path, exist_ok=True)
-
         self.filename = filename
         self.prefix = prefix
         self.suffix = suffix
         self._format = format
         self.format_folder = format_folder
         self.bypass = bypass
         self.bbox_inches = bbox_inches
@@ -73,29 +70,27 @@
     @property
     def format_list(self):
         if not isinstance(self.format, list):
             return [self.format]
         return self.format
 
     def output_path_from(self, format):
-
         if format in "show":
             return None
 
         if self.format_folder:
             output_path = path.join(self.path, format)
         else:
             output_path = self.path
 
         os.makedirs(output_path, exist_ok=True)
 
         return output_path
 
     def filename_from(self, auto_filename):
-
         filename = auto_filename if self.filename is None else self.filename
 
         if self.prefix is not None:
             filename = f"{self.prefix}{filename}"
 
         if self.suffix is not None:
             filename = f"{filename}{self.suffix}"
@@ -115,17 +110,19 @@
         auto_filename
             If the filename is not manually specified this name is used instead, which is defined in the parent plotter.
         """
 
         filename = self.filename_from(auto_filename=auto_filename)
 
         for format in self.format_list:
-
             output_path = self.output_path_from(format=format)
 
+            if format != "show":
+                os.makedirs(output_path, exist_ok=True)
+
             if not self.bypass:
                 if format == "show":
                     plt.show()
                 elif format == "png":
                     plt.savefig(
                         path.join(output_path, f"{filename}.png"),
                         bbox_inches=self.bbox_inches,
@@ -151,17 +148,19 @@
         auto_filename
             If the filename is not manually specified this name is used instead, which is defined in the parent plotter.
         """
 
         filename = self.filename_from(auto_filename=auto_filename)
 
         for format in self.format_list:
-
             output_path = self.output_path_from(format=format)
 
+            if format != "show":
+                os.makedirs(output_path, exist_ok=True)
+
             if format == "show":
                 plt.show()
             elif format == "png":
                 plt.savefig(
                     path.join(output_path, f"{filename}.png"),
                     bbox_inches=self.bbox_inches,
                 )
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/text.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/text.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 
     This object wraps the following Matplotlib methods:
 
     - plt.text: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.text.html
     """
 
     def set(self):
-
         if "x" not in self.kwargs and "y" not in self.kwargs and "s" not in self.kwargs:
             return
 
         plt.text(**self.config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/tickparams.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/tickparams.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/base/title.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/base/title.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         """
 
         super().__init__(**kwargs)
 
         self.manual_label = self.kwargs.get("label")
 
     def set(self, auto_title=None):
-
         config_dict = self.config_dict
 
         label = auto_title if self.manual_label is None else self.manual_label
 
         if "label" in config_dict:
             config_dict.pop("label")
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/avxline.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/avxline.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
         if self.no_label:
             label = None
 
         plt.axvline(x=vertical_line, label=label, **self.config_dict)
 
         if vertical_errors is not None:
-
             config_dict = self.config_dict
 
             if "linestyle" in config_dict:
                 config_dict.pop("linestyle")
 
             plt.axvline(x=vertical_errors[0], linestyle="--", **config_dict)
             plt.axvline(x=vertical_errors[1], linestyle="--", **config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/fill_between.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/fill_between.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,11 +44,10 @@
         y1
             The second line of ydata that defines the region that is filled in.
         """
 
         config_dict = self.config_dict
 
         if self.match_color_to_yx:
-
             config_dict["color"] = plt.gca().lines[-1].get_color()
 
         plt.fill_between(x=x, y1=y1, y2=y2, **config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/yx_plot.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         y: Union[np.ndarray, Array1D],
         x: Union[np.ndarray, Array1D],
         label: str = None,
         plot_axis_type=None,
         y_errors=None,
         x_errors=None,
         y_extra=None,
+        ls_errorbar="",
     ):
         """
         Plots 1D y-data against 1D x-data using the matplotlib method `plt.plot`, `plt.semilogy`, `plt.loglog`,
         or `plt.scatter`.
 
         Parameters
         ----------
@@ -58,22 +59,22 @@
         elif plot_axis_type == "semilogy":
             plt.semilogy(x, y, label=label, **self.config_dict)
         elif plot_axis_type == "loglog":
             plt.loglog(x, y, label=label, **self.config_dict)
         elif plot_axis_type == "scatter":
             plt.scatter(x, y, label=label, **self.config_dict)
         elif plot_axis_type == "errorbar" or plot_axis_type == "errorbar_logy":
-
             plt.errorbar(
                 x,
                 y,
                 yerr=y_errors,
                 xerr=x_errors,
-                marker="o",
+                #     marker="o",
                 fmt="o",
+                # ls=ls_errorbar,
                 **self.config_dict
             )
             if y_extra is not None:
                 plt.plot(x, y_extra, c="r")
             if plot_axis_type == "errorbar_logy":
                 plt.yscale("log")
         else:
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/one_d/yx_scatter.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_scatter.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/segmentdata.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/segmentdata.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/__init__.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/abstract.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/array_overlay.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/array_overlay.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,12 +12,11 @@
     - plt.imshow: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.imshow.html
 
     This uses the `Units` and coordinate system of the `Array2D` to overlay it on on the coordinate system of the
     figure that is plotted.
     """
 
     def overlay_array(self, array, figure):
-
         aspect = figure.aspect_from(shape_native=array.shape_native)
         extent = array.extent_of_zoomed_array(buffer=0)
 
         plt.imshow(X=array.native, aspect=aspect, extent=extent, **self.config_dict)
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/grid_errorbar.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_errorbar.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/grid_plot.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         Parameters
         ----------
         grid
             The grid of (y,x) coordinates that is plotted.
         """
 
         try:
-
             color = self.config_dict["c"]
 
             if isinstance(color, list):
                 color = color[0]
 
             config_dict = self.config_dict
             config_dict.pop("c")
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/grid_scatter.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_scatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
         color = itertools.cycle(self.config_dict["c"])
         config_dict = self.config_dict
         config_dict.pop("c")
 
         try:
             for grid in grid_list:
-
                 plt.scatter(y=grid[:, 0], x=grid[:, 1], c=next(color), **config_dict)
         except IndexError:
             return None
 
     def scatter_grid_colored(
         self, grid: Union[np.ndarray, Grid2D], color_array: np.ndarray, cmap: str
     ):
@@ -141,38 +140,34 @@
                 indexes = [indexes]
 
         color = itertools.cycle(self.config_dict["c"])
         config_dict = self.config_dict
         config_dict.pop("c")
 
         for index_list in indexes:
-
             if all([isinstance(index, float) for index in index_list]) or all(
                 [isinstance(index, int) for index in index_list]
             ):
-
                 plt.scatter(
                     y=grid[index_list, 0],
                     x=grid[index_list, 1],
                     color=next(color),
                     **config_dict,
                 )
 
             elif all([isinstance(index, tuple) for index in index_list]) or all(
                 [isinstance(index, list) for index in index_list]
             ):
-
                 ys, xs = map(list, zip(*index_list))
 
                 plt.scatter(
                     y=grid.native[ys, xs, 0],
                     x=grid.native[ys, xs, 1],
                     color=next(color),
                     **config_dict,
                 )
 
             else:
-
                 raise exc.PlottingException(
                     "The indexes input into the grid_scatter_index method do not conform to a "
                     "useable type"
                 )
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/interpolated_reconstruction.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/interpolated_reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from typing import Union
 
 from autoarray.plot.wrap.two_d.abstract import AbstractMatWrap2D
+from autoarray.plot.wrap.base.units import Units
 from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoiNoInterp
 from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoi
 from autoarray.inversion.pixelization.mappers.delaunay import MapperDelaunay
 
 from autoarray.plot.wrap import base as wb
 
 
@@ -28,14 +29,15 @@
     - plt.imshow: https://matplotlib.org/3.3.2/api/_as_gen/matplotlib.pyplot.imshow.html
     """
 
     def imshow_reconstruction(
         self,
         mapper: Union[MapperDelaunay, MapperVoronoiNoInterp, MapperVoronoi],
         pixel_values: np.ndarray,
+        units: Units,
         cmap: wb.Cmap,
         colorbar: wb.Colorbar,
         colorbar_tickparams: wb.ColorbarTickParams = None,
         aspect=None,
         ax=None,
     ):
         """
@@ -79,22 +81,23 @@
 
         color_values = np.where(pixel_values > vmax, vmax, pixel_values)
         color_values = np.where(pixel_values < vmin, vmin, color_values)
 
         cmap = plt.get_cmap(cmap.cmap)
 
         if colorbar is not None:
-
             colorbar = colorbar.set_with_color_values(
-                cmap=cmap, color_values=color_values, ax=ax
+                units=units, cmap=cmap, color_values=color_values, ax=ax
             )
             if colorbar is not None and colorbar_tickparams is not None:
                 colorbar_tickparams.set(cb=colorbar)
 
         interpolation_array = mapper.interpolated_array_from(values=pixel_values)
 
         plt.imshow(
             X=interpolation_array.native,
             cmap=cmap,
             extent=mapper.source_plane_mesh_grid.geometry.extent_square,
             aspect=aspect,
         )
+
+        return interpolation_array
```

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/patch_overlay.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/patch_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/plot/wrap/two_d/vector_yx_quiver.py` & `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/vector_yx_quiver.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/structures/abstract_structure.py` & `autoarray-2023.7.7.1/autoarray/structures/abstract_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from autoarray.mask.derive.mask_2d import DeriveMask2D
 
 from autoarray import exc
 
 
 class Structure(AbstractNDArray, ABC):
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
     @property
     @abstractmethod
     def slim(self) -> "Structure":
         """
@@ -67,17 +66,15 @@
 
     @property
     def pixel_scale(self) -> float:
         return self.mask.pixel_scale
 
     @property
     def pixel_area(self):
-
         if len(self.pixel_scales) != 2:
-
             raise exc.GridException("Cannot compute area of structure which is not 2D.")
 
         return self.pixel_scales[0] * self.pixel_scales[1]
 
     @property
     def total_area(self):
         return self.total_pixels * self.pixel_area
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/arrays/array_1d_util.py` & `autoarray-2023.7.7.1/autoarray/structures/arrays/array_1d_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 
     return line_1d_slim
 
 
 def array_1d_native_from(
     array_1d_slim: np.ndarray, mask_1d: np.ndarray, sub_size: int
 ) -> np.ndarray:
-
     sub_shape = mask_1d.shape[0] * sub_size
 
     native_index_for_slim_index_1d = mask_1d_util.native_index_for_slim_index_1d_from(
         mask_1d=mask_1d, sub_size=sub_size
     ).astype("int")
 
     return array_1d_via_indexes_1d_from(
@@ -181,15 +180,14 @@
     -------
     ndarray
         The native 1D array of values mapped from the slimmed array with dimensions (total_x_pixels).
     """
     array_1d_native = np.zeros(sub_shape)
 
     for slim_index in range(len(native_index_for_slim_index_1d)):
-
         array_1d_native[native_index_for_slim_index_1d[slim_index]] = array_1d_slim[
             slim_index
         ]
 
     return array_1d_native
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/arrays/array_2d_util.py` & `autoarray-2023.7.7.1/autoarray/structures/arrays/array_2d_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     ----------
     array_2d
         The input structure which is converted to its slim representation.
     mask_2d
         The mask of the output Array2D.
     """
     if len(array_2d.shape) == 1:
-
         if array_2d.shape[0] != mask_2d.sub_pixels_in_mask:
             raise exc.ArrayException(
                 f"""
                 The input array is a slim 1D array, but it does not have the same number of entries as sub-pixels in
                 the mask.
 
                 This indicates that the number of unmaksed pixels in the mask  is different to the input slim array 
@@ -69,15 +68,14 @@
                 Input array_2d_slim.shape = {array_2d.shape[0]}
                 Input mask_2d.sub_pixels_in_mask = {mask_2d.sub_pixels_in_mask}
                 Input mask_2d.shape_native = {mask_2d.shape_native}
                 """
             )
 
     if len(array_2d.shape) == 2:
-
         if array_2d.shape != mask_2d.sub_shape_native:
             raise exc.ArrayException(
                 f"""
                 The input array is 2D but not the same dimensions as the mask.
     
                 This indicates the mask's shape, multiplied by its `sub_size`, is different to the input array shape.
     
@@ -154,15 +152,14 @@
     array_2d
         The input structure which is converted to its slim representation.
     mask_2d
         The mask of the output Array2D.
     """
 
     if len(array_2d.shape) == 1:
-
         array_2d_slim = array_2d
 
         return array_2d_slim
 
     return array_2d_slim_from(
         array_2d_native=array_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
     )
@@ -182,15 +179,14 @@
     array_2d
         The input structure which is converted to an ndarray if it is a list.
     mask_2d
         The mask of the output Array2D.
     """
 
     if len(array_2d.shape) == 2:
-
         array_2d_native = array_2d * np.invert(mask_2d)
 
         if array_2d.shape != mask_2d.sub_shape_native:
             raise exc.ArrayException(
                 "The input array is 2D but not the same dimensions as the sub-mask "
                 "(e.g. the mask 2D shape multipled by its sub size.)"
             )
@@ -304,15 +300,14 @@
     resize_array = resize_array_2d(array_2d=array_2d, new_shape=(2,2), origin=(2, 2))
     """
 
     y_is_even = int(array_2d.shape[0]) % 2 == 0
     x_is_even = int(array_2d.shape[1]) % 2 == 0
 
     if origin == (-1, -1):
-
         if y_is_even:
             y_centre = int(array_2d.shape[0] / 2)
         elif not y_is_even:
             y_centre = int(array_2d.shape[0] / 2)
 
         if x_is_even:
             x_centre = int(array_2d.shape[1] / 2)
@@ -436,15 +431,14 @@
     --------
     indexes_slim = np.array([0, 1, 2, 5])
     indexes_2d = index_2d_for_index_slim_from(indexes_slim=indexes_slim, shape=(3,3))
     """
     index_2d_for_index_slim = np.zeros((indexes_slim.shape[0], 2))
 
     for i, index_slim in enumerate(indexes_slim):
-
         index_2d_for_index_slim[i, 0] = int(index_slim / shape_native[1])
         index_2d_for_index_slim[i, 1] = int(index_slim % shape_native[1])
 
     return index_2d_for_index_slim
 
 
 @numba_util.jit()
@@ -649,15 +643,14 @@
     -------
     ndarray
         The native 2D array of values mapped from the slimmed array with dimensions (total_values, total_values).
     """
     sub_array_native_2d = np.zeros(sub_shape)
 
     for slim_index in range(len(native_index_for_slim_index_2d)):
-
         sub_array_native_2d[
             native_index_for_slim_index_2d[slim_index, 0],
             native_index_for_slim_index_2d[slim_index, 1],
         ] = array_2d_slim[slim_index]
 
     return sub_array_native_2d
 
@@ -734,15 +727,14 @@
 
 @numba_util.jit()
 def array_2d_native_complex_via_indexes_from(
     array_2d_slim: np.ndarray,
     sub_shape_native: Tuple[int, int],
     native_index_for_slim_index_2d: np.ndarray,
 ) -> np.ndarray:
-
     sub_array_2d = 0 + 0j * np.zeros(sub_shape_native)
 
     for slim_index in range(len(native_index_for_slim_index_2d)):
         sub_array_2d[
             native_index_for_slim_index_2d[slim_index, 0],
             native_index_for_slim_index_2d[slim_index, 1],
         ] = array_2d_slim[slim_index]
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/arrays/irregular.py` & `autoarray-2023.7.7.1/autoarray/structures/arrays/irregular.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 from os import path
 from typing import List, Union
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-
     from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
 from autoarray.structures.abstract_structure import Structure
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
@@ -47,15 +46,14 @@
             A collection of values.
         """
 
         if len(values) == 0:
             return []
 
         if type(values) is list:
-
             if isinstance(values, ArrayIrregular):
                 return values
 
             values = np.asarray(values)
 
         obj = values.view(cls)
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/arrays/kernel_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/arrays/kernel_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,14 @@
         pixel_scales: ty.PixelScales,
         y_stddev: float,
         x_stddev: float,
         theta: float,
         centre: Tuple[float, float] = (0.0, 0.0),
         normalize: bool = False,
     ) -> "Kernel2D":
-
         x_stddev = (
             x_stddev * (units.deg).to(units.arcsec) / (2.0 * np.sqrt(2.0 * np.log(2.0)))
         )
         y_stddev = (
             y_stddev * (units.deg).to(units.arcsec) / (2.0 * np.sqrt(2.0 * np.log(2.0)))
         )
 
@@ -391,57 +390,52 @@
             rescale_factor,
             anti_aliasing=False,
             mode="constant",
             multichannel=False,
         )
 
         if kernel_rescaled.shape[0] % 2 == 0 and kernel_rescaled.shape[1] % 2 == 0:
-
             kernel_rescaled = resize(
                 kernel_rescaled,
                 output_shape=(
                     kernel_rescaled.shape[0] + 1,
                     kernel_rescaled.shape[1] + 1,
                 ),
                 anti_aliasing=False,
                 mode="constant",
             )
 
         elif kernel_rescaled.shape[0] % 2 == 0 and kernel_rescaled.shape[1] % 2 != 0:
-
             kernel_rescaled = resize(
                 kernel_rescaled,
                 output_shape=(kernel_rescaled.shape[0] + 1, kernel_rescaled.shape[1]),
                 anti_aliasing=False,
                 mode="constant",
             )
 
         elif kernel_rescaled.shape[0] % 2 != 0 and kernel_rescaled.shape[1] % 2 == 0:
-
             kernel_rescaled = resize(
                 kernel_rescaled,
                 output_shape=(kernel_rescaled.shape[0], kernel_rescaled.shape[1] + 1),
                 anti_aliasing=False,
                 mode="constant",
             )
 
         if self.pixel_scales is not None:
-
             pixel_scale_factors = (
                 self.mask.shape[0] / kernel_rescaled.shape[0],
                 self.mask.shape[1] / kernel_rescaled.shape[1],
             )
 
             pixel_scales = (
                 self.pixel_scales[0] * pixel_scale_factors[0],
                 self.pixel_scales[1] * pixel_scale_factors[1],
             )
 
         else:
-
             pixel_scales = None
 
         return Kernel2D.no_mask(
             values=kernel_rescaled, pixel_scales=pixel_scales, normalize=normalize
         )
 
     @property
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/arrays/uniform_1d.py` & `autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         values: Union[np.ndarray, List],
         mask: Mask1D,
         header: Optional[Header] = None,
         store_native: bool = False,
         *args,
         **kwargs
     ):
-
         values = array_1d_util.convert_array_1d(
             array_1d=values, mask_1d=mask, store_native=store_native
         )
 
         obj = values.view(cls)
         obj.mask = mask
         obj.header = header
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/arrays/uniform_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         store_native
             If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels]. This avoids
             mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
 
         Examples
         --------
 
-        This example uses the ``Array2D.no_mask`` method to create the the ``Array2D``.
+        This example uses the ``Array2D.no_mask`` method to create the ``Array2D``.
 
         Different methods using different inputs are available and documented throughout this webpage.
 
         .. code-block:: python
 
             import autoarray as aa
 
@@ -341,15 +341,14 @@
         obj = values.view(cls)
         obj.mask = mask
         obj.header = header
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
         if hasattr(obj, "header"):
             self.header = obj.header
         else:
             self.header = None
@@ -710,15 +709,14 @@
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = array_2d_util.convert_array(array=values)
 
         if len(values.shape) == 1:
-
             if shape_native is None:
                 raise exc.ArrayException(
                     f"""
                     The input array is not in its native shape (an ndarray / list of shape [total_y_pixels, total_x_pixels])
                     and the shape_native parameter has not been input the Array2D function.
 
                     Either change the input array to be its native shape or input its shape_native input the function.
@@ -731,15 +729,14 @@
                 raise exc.ArrayException(
                     """
                     The input shape_native parameter is not a tuple of type (int, int)
                     """
                 )
 
         else:
-
             shape_native = (
                 int(values.shape[0] / sub_size),
                 int(values.shape[1] / sub_size),
             )
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/grid_1d_util.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/grid_1d_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 import numpy as np
 from typing import TYPE_CHECKING, List, Union, Tuple
 
 if TYPE_CHECKING:
-
     from autoarray.mask.mask_1d import Mask1D
 
 from autoarray.structures.arrays import array_1d_util
 from autoarray import numba_util
 from autoarray.geometry import geometry_util
 from autoarray.structures.grids import grid_2d_util
 from autoarray.mask import mask_1d_util
@@ -153,21 +152,18 @@
 
     sub_index = 0
 
     x_sub_half = pixel_scales[0] / 2
     x_sub_step = pixel_scales[0] / (sub_size)
 
     for x in range(mask_1d.shape[0]):
-
         if not mask_1d[x]:
-
             x_scaled = (x - centres_scaled[0]) * pixel_scales[0]
 
             for x1 in range(sub_size):
-
                 grid_1d[sub_index] = (
                     x_scaled - x_sub_half + x1 * x_sub_step + (x_sub_step / 2.0)
                 )
                 sub_index += 1
 
     return grid_1d
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/grid_2d_util.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/grid_2d_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from autoarray.geometry import geometry_util
 from autoarray import numba_util
 from autoarray.mask import mask_2d_util
 from autoarray import type as ty
 
 
 def check_grid_slim(grid, shape_native):
-
     if shape_native is None:
         raise exc.GridException(
             f"""
             The input grid is not in its native shape (an ndarray / list of shape [total_y_pixels, total_x_pixels, 2])
             and the shape_native parameter has not been input the Grid2D function.
 
             Either change the input array to be its native shape or input its shape_native input the function.
@@ -32,15 +31,14 @@
             """
             The input shape_native parameter is not a tuple of type (int, int).
             """
         )
 
 
 def convert_grid(grid: Union[np.ndarray, List]) -> np.ndarray:
-
     if type(grid) is list:
         grid = np.asarray(grid)
 
     return grid
 
 
 def check_grid_2d(grid_2d: np.ndarray):
@@ -50,32 +48,29 @@
         )
 
     if 2 < len(grid_2d.shape) > 3:
         raise exc.GridException("The dimensions of the input grid array is not 2 or 3")
 
 
 def check_grid_2d_and_mask_2d(grid_2d: np.ndarray, mask_2d: Mask2D):
-
     if len(grid_2d.shape) == 2:
-
         if grid_2d.shape[0] != mask_2d.sub_pixels_in_mask:
             raise exc.GridException(
                 f"""
                 The input 2D grid does not have the same number of values as sub-pixels in
                 the mask.
                 
                 The shape of the input grid_2d is {grid_2d.shape}.
                 The mask shape_native is {mask_2d.shape_native}.
                 The mask number of sub-pixels is {mask_2d.sub_pixels_in_mask}. 
                 The mask sub size is {mask_2d.sub_size}).
                 """
             )
 
     elif len(grid_2d.shape) == 3:
-
         if (grid_2d.shape[0], grid_2d.shape[1]) != mask_2d.sub_shape_native:
             raise exc.GridException(
                 f"""
                 The input 2D grid is not the same dimensions as the sub-mask
                 (e.g. the mask 2D shape multipled by its sub size.)
 
                 The shape of the input grid_2d is {grid_2d.shape}.
@@ -260,23 +255,20 @@
     y_sub_step = pixel_scales[0] / (sub_size)
 
     x_sub_half = pixel_scales[1] / 2
     x_sub_step = pixel_scales[1] / (sub_size)
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
-
             if not mask_2d[y, x]:
-
                 y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
                 x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
 
                 for y1 in range(sub_size):
                     for x1 in range(sub_size):
-
                         grid_slim[sub_index, 0] = -(
                             y_scaled - y_sub_half + y1 * y_sub_step + (y_sub_step / 2.0)
                         )
                         grid_slim[sub_index, 1] = (
                             x_scaled - x_sub_half + x1 * x_sub_step + (x_sub_step / 2.0)
                         )
                         sub_index += 1
@@ -604,15 +596,14 @@
     grid_scaled_2d_slim_radii = np.zeros((shape_slim, 2))
 
     grid_scaled_2d_slim_radii[:, 0] += centre[0]
 
     radii = centre[1]
 
     for slim_index in range(shape_slim):
-
         grid_scaled_2d_slim_radii[slim_index, 1] = radii
         radii += pixel_scale / sub_size
 
     return grid_scaled_2d_slim_radii
 
 
 @numba_util.jit()
@@ -660,45 +651,40 @@
         np.add(
             np.square(np.subtract(grid[:, 0], border_origin[0])),
             np.square(np.subtract(grid[:, 1], border_origin[1])),
         )
     )
 
     for pixel_index in range(grid.shape[0]):
-
         if grid_radii[pixel_index] > border_min_radii:
-
             closest_pixel_index = np.argmin(
                 np.square(grid[pixel_index, 0] - border_grid[:, 0])
                 + np.square(grid[pixel_index, 1] - border_grid[:, 1])
             )
 
             move_factor = (
                 border_grid_radii[closest_pixel_index] / grid_radii[pixel_index]
             )
 
             if move_factor < 1.0:
-
                 grid_relocated[pixel_index, :] = (
                     move_factor * (grid[pixel_index, :] - border_origin[:])
                     + border_origin[:]
                 )
 
     return grid_relocated
 
 
 @numba_util.jit()
 def furthest_grid_2d_slim_index_from(
     grid_2d_slim: np.ndarray, slim_indexes: np.ndarray, coordinate: Tuple[float, float]
 ) -> int:
-
     distance_to_centre = 0.0
 
     for slim_index in slim_indexes:
-
         y = grid_2d_slim[slim_index, 0]
         x = grid_2d_slim[slim_index, 1]
         distance_to_centre_new = (x - coordinate[1]) ** 2 + (y - coordinate[0]) ** 2
 
         if distance_to_centre_new >= distance_to_centre:
             distance_to_centre = distance_to_centre_new
             furthest_grid_2d_slim_index = slim_index
@@ -815,21 +801,19 @@
     y_upscale_half = pixel_scales[0] / 2
     y_upscale_step = pixel_scales[0] / upscale_factor
 
     x_upscale_half = pixel_scales[1] / 2
     x_upscale_step = pixel_scales[1] / upscale_factor
 
     for slim_index in range(grid_slim.shape[0]):
-
         y_grid = grid_slim[slim_index, 0]
         x_grid = grid_slim[slim_index, 1]
 
         for y in range(upscale_factor):
             for x in range(upscale_factor):
-
                 grid_2d_slim_upscaled[upscale_index, 0] = (
                     y_grid
                     + y_upscale_half
                     - y * y_upscale_step
                     - (y_upscale_step / 2.0)
                 )
                 grid_2d_slim_upscaled[upscale_index, 1] = (
@@ -857,12 +841,11 @@
             y_inside.append(grid_2d[i, 0])
             x_inside.append(grid_2d[i, 1])
 
     return np.asarray(y_inside, x_inside)
 
 
 def compute_polygon_area(points):
-
     x = points[:, 1]
     y = points[:, 0]
 
     return 0.5 * np.abs(np.dot(x, np.roll(y, 1)) - np.dot(y, np.roll(x, 1)))
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/irregular_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/irregular_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             The irregular grid of (y,x) coordinates.
         """
 
         if len(values) == 0:
             return []
 
         if type(values) is list:
-
             if isinstance(values[0], Grid2DIrregular):
                 return values
 
             values = np.asarray(values)
 
         obj = values.view(cls)
 
@@ -151,15 +150,15 @@
         self, deflection_grid: np.ndarray
     ) -> "Grid2DIrregular":
         """
         Returns a new Grid2DIrregular from this grid coordinates, where the (y,x) coordinates of this grid have a
         grid of (y,x) values, termed the deflection grid, subtracted from them to determine the new grid of (y,x)
         values.
 
-        This is used by **PyAutoLens** to perform grid ray-tracing.
+        This is to perform grid ray-tracing.
 
         Parameters
         ----------
         deflection_grid
             The grid of (y,x) coordinates which is subtracted from this grid.
         """
         return Grid2DIrregular(values=self - deflection_grid)
@@ -277,15 +276,14 @@
         ArrayIrregular
             The further distances of every coordinate to every other coordinate on the irregular grid.
         """
 
         radial_distances_max = np.zeros((self.shape[0]))
 
         for i in range(self.shape[0]):
-
             x_distances = np.square(np.subtract(self[i, 0], self[:, 0]))
             y_distances = np.square(np.subtract(self[i, 1], self[:, 1]))
 
             radial_distances_max[i] = np.sqrt(np.max(np.add(x_distances, y_distances)))
 
         return self.values_from(array_slim=radial_distances_max)
 
@@ -304,15 +302,14 @@
         The grid of coordinates corresponding to the closest coordinate of each coordinate of this instance of
         the `Grid2DIrregular` to the input grid.
         """
 
         grid_of_closest = np.zeros((grid_pair.shape[0], 2))
 
         for i in range(grid_pair.shape[0]):
-
             x_distances = np.square(np.subtract(grid_pair[i, 0], self[:, 0]))
             y_distances = np.square(np.subtract(grid_pair[i, 1], self[:, 1]))
 
             radial_distances = np.add(x_distances, y_distances)
 
             grid_of_closest[i, :] = self[np.argmin(radial_distances), :]
 
@@ -361,15 +358,14 @@
             )
 
         with open(file_path, "w+") as f:
             json.dump(self.in_list, f)
 
 
 class Grid2DIrregularTransformed(Grid2DIrregular):
-
     pass
 
 
 class Grid2DIrregularUniform(Grid2DIrregular):
     def __new__(
         cls,
         values: np.ndarray,
@@ -432,15 +428,14 @@
 
         obj.shape_native = shape_native
         obj.pixel_scales = pixel_scales
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "_internal_list"):
             self._internal_list = obj._internal_list
 
         if hasattr(obj, "shape_native"):
             self.shape_native = obj.shape_native
 
         if hasattr(obj, "pixel_scales"):
@@ -460,15 +455,14 @@
     def from_grid_sparse_uniform_upscale(
         cls,
         grid_sparse_uniform: np.ndarray,
         upscale_factor: int,
         pixel_scales,
         shape_native=None,
     ) -> "Grid2DIrregularUniform":
-
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         grid_upscaled_1d = grid_2d_util.grid_2d_slim_upscaled_from(
             grid_slim=grid_sparse_uniform,
             upscale_factor=upscale_factor,
             pixel_scales=pixel_scales,
         )
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/iterate_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/iterate_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from autoarray.geometry import geometry_util
 from autoarray.structures.grids import grid_2d_util
 
 from autoarray import type as ty
 
 
 def sub_steps_from(sub_steps):
-
     if sub_steps is None:
         return [2, 4, 8, 16]
     return sub_steps
 
 
 class Grid2DIterate(Grid2D):
     def __new__(
@@ -86,15 +85,14 @@
         obj.fractional_accuracy = fractional_accuracy
         obj.relative_accuracy = relative_accuracy
         obj.sub_steps = sub_steps
 
         return obj
 
     def __array_finalize__(self, obj):
-
         super().__array_finalize__(obj)
 
         if hasattr(obj, "grid"):
             self.grid = obj.grid
 
         if hasattr(obj, "fractional_accuracy"):
             self.fractional_accuracy = obj.fractional_accuracy
@@ -152,19 +150,17 @@
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = grid_2d_util.convert_grid(grid=values)
 
         if len(values.shape) == 2:
-
             grid_2d_util.check_grid_slim(grid=values, shape_native=shape_native)
 
         else:
-
             shape_native = (int(values.shape[0]), int(values.shape[1]))
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
             sub_size=1,
             origin=origin,
@@ -450,24 +446,22 @@
             mask=padded_mask,
             fractional_accuracy=self.fractional_accuracy,
             sub_steps=self.sub_steps,
         )
 
     @staticmethod
     def array_at_sub_size_from(func: Callable, cls, mask: Mask2D, sub_size) -> Array2D:
-
         mask_higher_sub = mask.mask_new_sub_size_from(mask=mask, sub_size=sub_size)
 
         grid_compute = Grid2D.from_mask(mask=mask_higher_sub)
         array_higher_sub = func(cls, grid_compute)
         return grid_compute.structure_2d_from(result=array_higher_sub).binned.native
 
     @staticmethod
     def grid_at_sub_size_from(func: Callable, cls, mask: Mask2D, sub_size) -> Grid2D:
-
         mask_higher_sub = mask.mask_new_sub_size_from(mask=mask, sub_size=sub_size)
 
         grid_compute = Grid2D.from_mask(mask=mask_higher_sub)
         grid_higher_sub = func(cls, grid_compute)
         return grid_compute.structure_2d_from(result=grid_higher_sub).binned.native
 
     def threshold_mask_via_arrays_from(
@@ -529,41 +523,35 @@
           therefore does not need to be iteratively computed at higher levels of sub-gridding.
 
         - ``False`` entries signify the function has not been evaluated in that pixel to desired fractional accuracy and
           therefore must be iterative computed at higher levels of sub-gridding to meet this accuracy.
         """
 
         if fractional_accuracy_threshold is not None:
-
             for y in range(threshold_mask.shape[0]):
                 for x in range(threshold_mask.shape[1]):
                     if not array_higher_mask[y, x]:
-
                         if array_lower_sub_2d[y, x] > 0:
-
                             fractional_accuracy = (
                                 array_lower_sub_2d[y, x] / array_higher_sub_2d[y, x]
                             )
 
                             if fractional_accuracy > 1.0:
                                 fractional_accuracy = 1.0 / fractional_accuracy
 
                         else:
-
                             fractional_accuracy = 0.0
 
                         if fractional_accuracy < fractional_accuracy_threshold:
                             threshold_mask[y, x] = False
 
         if relative_accuracy_threshold is not None:
-
             for y in range(threshold_mask.shape[0]):
                 for x in range(threshold_mask.shape[1]):
                     if not array_higher_mask[y, x]:
-
                         if (
                             abs(array_lower_sub_2d[y, x] - array_higher_sub_2d[y, x])
                             > relative_accuracy_threshold
                         ):
                             threshold_mask[y, x] = False
 
         return threshold_mask
@@ -603,39 +591,35 @@
             return array_lower_sub_2d.slim
 
         iterated_array = np.zeros(shape=self.shape_native)
 
         threshold_mask_lower_sub = self.mask
 
         for sub_size in self.sub_steps[:-1]:
-
             array_higher_sub = self.array_at_sub_size_from(
                 func=func, cls=cls, mask=threshold_mask_lower_sub, sub_size=sub_size
             )
 
             try:
-
                 threshold_mask_higher_sub = self.threshold_mask_via_arrays_from(
                     array_lower_sub_2d=array_lower_sub_2d,
                     array_higher_sub_2d=array_higher_sub,
                 )
 
                 iterated_array = self.iterated_array_jit_from(
                     iterated_array=iterated_array,
                     threshold_mask_higher_sub=threshold_mask_higher_sub,
                     threshold_mask_lower_sub=threshold_mask_lower_sub,
                     array_higher_sub_2d=array_higher_sub,
                 )
 
             except ZeroDivisionError:
-
                 return self.return_iterated_array_result(iterated_array=iterated_array)
 
             if threshold_mask_higher_sub.is_all_true:
-
                 return self.return_iterated_array_result(iterated_array=iterated_array)
 
             array_lower_sub_2d = array_higher_sub
             threshold_mask_lower_sub = threshold_mask_higher_sub
 
         array_higher_sub = self.array_at_sub_size_from(
             func=func,
@@ -753,27 +737,23 @@
         - ``False`` entries signify the function has not been evaluated in that pixel to desired fractional accuracy and
           therefore must be iterative computed at higher levels of sub-gridding to meet this accuracy.
         """
 
         for y in range(threshold_mask.shape[0]):
             for x in range(threshold_mask.shape[1]):
                 if not grid_higher_mask[y, x]:
-
                     if abs(grid_higher_sub_2d[y, x, 0]) > 0:
-
                         fractional_accuracy_y = (
                             grid_lower_sub_2d[y, x, 0] / grid_higher_sub_2d[y, x, 0]
                         )
 
                     else:
-
                         fractional_accuracy_y = 1.0
 
                     if abs(grid_higher_sub_2d[y, x, 1]) > 0:
-
                         fractional_accuracy_x = (
                             grid_lower_sub_2d[y, x, 1] / grid_higher_sub_2d[y, x, 1]
                         )
 
                     else:
                         fractional_accuracy_x = 1.0
 
@@ -787,19 +767,17 @@
                         fractional_accuracy_y, fractional_accuracy_x
                     )
 
                     if fractional_accuracy < fractional_accuracy_threshold:
                         threshold_mask[y, x] = False
 
         if relative_accuracy_threshold is not None:
-
             for y in range(threshold_mask.shape[0]):
                 for x in range(threshold_mask.shape[1]):
                     if not grid_higher_mask[y, x]:
-
                         relative_accuracy_y = abs(
                             grid_lower_sub_2d[y, x, 0] - grid_higher_sub_2d[y, x, 0]
                         )
                         relative_accuracy_x = abs(
                             grid_lower_sub_2d[y, x, 1] - grid_higher_sub_2d[y, x, 1]
                         )
 
@@ -847,15 +825,14 @@
             return grid_lower_sub_2d.slim
 
         iterated_grid = np.zeros(shape=(self.shape_native[0], self.shape_native[1], 2))
 
         threshold_mask_lower_sub = self.mask
 
         for sub_size in self.sub_steps[:-1]:
-
             grid_higher_sub = self.grid_at_sub_size_from(
                 func=func, cls=cls, mask=threshold_mask_lower_sub, sub_size=sub_size
             )
 
             threshold_mask_higher_sub = self.threshold_mask_via_grids_from(
                 grid_lower_sub_2d=grid_lower_sub_2d, grid_higher_sub_2d=grid_higher_sub
             )
@@ -864,15 +841,14 @@
                 iterated_grid=iterated_grid,
                 threshold_mask_higher_sub=threshold_mask_higher_sub,
                 threshold_mask_lower_sub=threshold_mask_lower_sub,
                 grid_higher_sub_2d=grid_higher_sub,
             )
 
             if threshold_mask_higher_sub.is_all_true:
-
                 iterated_grid_1d = grid_2d_util.grid_2d_slim_from(
                     mask=self.mask, grid_2d_native=iterated_grid, sub_size=1
                 )
 
                 return Grid2D(values=iterated_grid_1d, mask=self.mask.derive_mask.sub_1)
 
             grid_lower_sub_2d = grid_higher_sub
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/sparse_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
         obj = values.view(cls)
         obj.sparse_index_for_slim_index = sparse_index_for_slim_index
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
         if hasattr(obj, "sparse_index_for_slim_index"):
             self.sparse_index_for_slim_index = obj.sparse_index_for_slim_index
 
     @classmethod
@@ -168,15 +167,15 @@
         Parameters
         ----------
         total_pixels
             The total number of pixels in the Grid2DSparse and input into the KMeans algortihm.
         grid : Grid2D
             The grid of (y,x) coordinates corresponding to the weight map.
         weight_map
-            The 2D array of weight values that the KMeans clustering algorithm adapts to to determine the Grid2DSparse.
+            The 2D array of weight values that the KMeans clustering algorithm adapts to determine the Grid2DSparse.
         n_iter
             The number of times the KMeans algorithm is repeated.
         max_iter
             The maximum number of iterations in one run of the KMeans algorithm.
         seed or None
             The random number seed, which can be used to reproduce Grid2DSparse's for the same inputs.
         stochastic
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/sparse_2d_util.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     """
 
     unmasked_sparse_for_sparse = np.zeros(total_sparse_pixels)
 
     pixel_index = 0
 
     for full_pixel_index in range(unmasked_sparse_grid_pixel_centres.shape[0]):
-
         y = unmasked_sparse_grid_pixel_centres[full_pixel_index, 0]
         x = unmasked_sparse_grid_pixel_centres[full_pixel_index, 1]
 
         if not mask[y, x]:
             unmasked_sparse_for_sparse[pixel_index] = full_pixel_index
             pixel_index += 1
 
@@ -69,15 +68,14 @@
 
     total_unmasked_sparse_pixels = unmasked_sparse_grid_pixel_centres.shape[0]
 
     sparse_for_unmasked_sparse = np.zeros(total_unmasked_sparse_pixels)
     pixel_index = 0
 
     for unmasked_sparse_pixel_index in range(total_unmasked_sparse_pixels):
-
         y = unmasked_sparse_grid_pixel_centres[unmasked_sparse_pixel_index, 0]
         x = unmasked_sparse_grid_pixel_centres[unmasked_sparse_pixel_index, 1]
 
         sparse_for_unmasked_sparse[unmasked_sparse_pixel_index] = pixel_index
 
         if not mask[y, x]:
             if pixel_index < total_sparse_pixels - 1:
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/uniform_1d.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/uniform_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 import numpy as np
 from typing import TYPE_CHECKING, List, Union, Tuple
 
 if TYPE_CHECKING:
-
     from autoarray.structures.arrays.uniform_1d import Array1D
     from autoarray.structures.grids.uniform_2d import Grid2D
     from autoarray.structures.grids.transformed_2d import Grid2DTransformed
     from autoarray.structures.grids.transformed_2d import Grid2DTransformedNumpy
 
 from autoarray.structures.abstract_structure import Structure
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/grids/uniform_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/grids/uniform_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,19 +285,17 @@
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = grid_2d_util.convert_grid(grid=values)
 
         if len(values.shape) == 2:
-
             grid_2d_util.check_grid_slim(grid=values, shape_native=shape_native)
 
         else:
-
             shape_native = (
                 int(values.shape[0] / sub_size),
                 int(values.shape[1] / sub_size),
             )
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
@@ -571,22 +569,20 @@
         buffer_around_corners
             Whether the grid is buffered such that the (y,x) values in the centre of its masks' edge pixels align
             with the input bounding box values.
         """
         y_min, y_max, x_min, x_max = bounding_box
 
         if not buffer_around_corners:
-
             pixel_scales = (
                 (y_max - y_min) / (shape_native[0]),
                 (x_max - x_min) / (shape_native[1]),
             )
 
         else:
-
             pixel_scales = (
                 (y_max - y_min) / (shape_native[0] - 1),
                 (x_max - x_min) / (shape_native[1] - 1),
             )
         origin = ((y_max + y_min) / 2.0, (x_max + x_min) / 2.0)
 
         return cls.uniform(
@@ -864,15 +860,14 @@
 
         if not isinstance(coordinates, list):
             coordinates = [coordinates]
 
         distance_mask = np.full(fill_value=False, shape=self.shape_native)
 
         for coordinate in coordinates:
-
             distances = self.distances_to_coordinate_from(coordinate=coordinate)
 
             distance_mask += distances.native < distance
 
         mask = Mask2D(
             mask=distance_mask,
             pixel_scales=self.pixel_scales,
@@ -1094,15 +1089,14 @@
         )
 
         grid_radial_projected_2d = geometry_util.transform_grid_2d_from_reference_frame(
             grid_2d=grid_radial_projected_2d, centre=centre, angle=0.0
         )
 
         if conf.instance["general"]["grid"]["remove_projected_centre"]:
-
             grid_radial_projected_2d = grid_radial_projected_2d[1:, :]
 
         return Grid2DIrregular(values=grid_radial_projected_2d)
 
     @property
     def shape_native_scaled_interior(self) -> Tuple[float, float]:
         """
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/header.py` & `autoarray-2023.7.7.1/autoarray/structures/header.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     def __init__(
         self,
         header_sci_obj: Dict = None,
         header_hdu_obj: Dict = None,
         original_roe_corner: Tuple[int, int] = None,
         readout_offsets: Optional[Tuple] = None,
     ):
-
         self.header_sci_obj = header_sci_obj
         self.header_hdu_obj = header_hdu_obj
         self.original_roe_corner = original_roe_corner
         self.readout_offsets = readout_offsets
 
     @property
     def date_of_observation(self) -> str:
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mesh/abstract_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/mesh/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mesh/delaunay_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/mesh/delaunay_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mesh/rectangular_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/mesh/rectangular_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mesh/triangulation_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/mesh/triangulation_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         - The corners of the Delaunay triangulles used to construct a Delaunay triangulation.
         - The centers of a Voronoi pixels used to constract a Voronoi mesh.
 
         These reflect the closely related geometric properties of the Delaunay and Voronoi grids, whereby the corner
         points of Delaunay triangles by definition represent the centres of the corresponding Voronoi mesh.
 
-        Different pixelizations, mappers and regularization schemes combine the the Delaunay and Voronoi
+        Different pixelizations, mappers and regularization schemes combine the Delaunay and Voronoi
         geometries in different ways to perform an Inversion. Thus, having all geometric methods contained in the
         single class here is necessary.
 
         The input `grid` of source pixel centres is ordered arbitrarily, given that there is no regular pattern
         for a Delaunay triangulation and Voronoi mesh's indexing to follow.
 
         This class is used in conjuction with the `inversion/pixelizations` package to create Voronoi meshs
@@ -75,15 +75,14 @@
             )
 
         if hasattr(obj, "uses_interpolation"):
             self.uses_interpolation = obj.uses_interpolation
 
     @property
     def geometry(self):
-
         shape_native_scaled = (
             np.amax(self[:, 0]).astype("float") - np.amin(self[:, 0]).astype("float"),
             np.amax(self[:, 1]).astype("float") - np.amin(self[:, 1]).astype("float"),
         )
 
         scaled_maxima = (
             np.amax(self[:, 0]).astype("float"),
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mesh/voronoi_2d.py` & `autoarray-2023.7.7.1/autoarray/structures/mesh/voronoi_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,24 +62,22 @@
             reconstructed source is returned on.
         """
         interpolation_grid = self.interpolation_grid_from(
             shape_native=shape_native, extent=extent
         )
 
         if use_nn:
-
             interpolated_array = mesh_util.voronoi_nn_interpolated_array_from(
                 shape_native=shape_native,
                 interpolation_grid_slim=interpolation_grid.slim,
                 pixel_values=values,
                 voronoi=self.voronoi,
             )
 
         else:
-
             interpolated_array = griddata(
                 points=self.voronoi.points, values=values, xi=interpolation_grid
             )
 
             interpolated_array = np.flipud(
                 np.fliplr(interpolated_array.reshape(shape_native).T)
             )
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mock/mock_grid.py` & `autoarray-2023.7.7.1/autoarray/structures/mock/mock_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from autoarray.geometry.abstract_2d import AbstractGeometry2D
 from autoarray.inversion.linear_obj.neighbors import Neighbors
 from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
 
 
 class MockGeometry(AbstractGeometry2D):
     def __init__(self, extent):
-
         self._extent = extent
 
     @property
     def extent(self) -> Tuple[float, float, float, float]:
         return self._extent
 
 
@@ -63,10 +62,9 @@
     @property
     def extent(self) -> Tuple[float, float, float, float]:
         return self._extent
 
 
 class MockMeshGrid:
     def __init__(self, neighbors=None, neighbors_sizes=None):
-
         self.neighbors = Neighbors(arr=neighbors, sizes=neighbors_sizes)
         self.shape = (len(self.neighbors.sizes),)
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/mock/mock_structure_decorators.py` & `autoarray-2023.7.7.1/autoarray/structures/mock/mock_structure_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 def radial_grid_from(grid):
     return np.sqrt(np.add(np.square(grid[:, 0]), np.square(grid[:, 1])))
 
 
 def ndarray_1d_from(profile, grid):
-
     sersic_constant = (
         (2 * 2.0)
         - (1.0 / 3.0)
         + (4.0 / (405.0 * 2.0))
         + (46.0 / (25515.0 * 2.0**2))
         + (131.0 / (1148175.0 * 2.0**3))
         - (2194697.0 / (30690717750.0 * 2.0**4))
@@ -196,15 +195,14 @@
                 grid=grid, radius=np.full(grid.shape[0], 2.0)
             )
         ]
 
 
 class MockGrid1DLikeObj:
     def __init__(self, centre=(0.0, 0.0), angle=0.0):
-
         self.centre = centre
         self.angle = angle
 
     @structure_decorators.grid_1d_to_structure
     def ndarray_1d_from(self, grid):
         return np.ones(shape=grid.shape[0])
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/plot/structure_plotters.py` & `autoarray-2023.7.7.1/autoarray/structures/plot/structure_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/structures/structure_decorators.py` & `autoarray-2023.7.7.1/autoarray/structures/structure_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,15 +502,15 @@
 
     return wrapper
 
 
 def relocate_to_radial_minimum(func):
     """ Checks whether any coordinates in the grid are radially near (0.0, 0.0), which can lead to numerical faults in \
     the evaluation of a function (e.g. numerical integration reaching a singularity at (0.0, 0.0)). If any coordinates
-    are radially within the the radial minimum threshold, their (y,x) coordinates are shifted to that value to ensure
+    are radially within the radial minimum threshold, their (y,x) coordinates are shifted to that value to ensure
     they are evaluated at that coordinate.
 
     The value the (y,x) coordinates are rounded to is set in the 'radial_min.ini' config.
 
     Parameters
     ----------
     func : (profile, *args, **kwargs) -> Object
@@ -543,15 +543,14 @@
         """
 
         grid_radial_minimum = conf.instance["grids"]["radial_minimum"][
             "radial_minimum"
         ][cls.__class__.__name__]
 
         with np.errstate(all="ignore"):  # Division by zero fixed via isnan
-
             grid_radii = cls.radial_grid_from(grid=grid)
 
             grid_radial_scale = np.where(
                 grid_radii < grid_radial_minimum, grid_radial_minimum / grid_radii, 1.0
             )
             grid = np.multiply(grid, grid_radial_scale[:, None])
         grid[np.isnan(grid)] = grid_radial_minimum
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/vectors/abstract.py` & `autoarray-2023.7.7.1/autoarray/structures/vectors/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class AbstractVectorYX2D(Structure):
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
         if hasattr(obj, "grid"):
             self.grid = obj.grid
 
     @property
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/vectors/irregular.py` & `autoarray-2023.7.7.1/autoarray/structures/vectors/irregular.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
         obj = values.view(cls)
         obj.grid = Grid2DIrregular(values=grid)
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "grid"):
             self.grid = obj.grid
 
     @property
     def slim(self) -> np.ndarray:
         """
         The vector-field in its 1D representation, an ndarray of shape [total_vectors, 2].
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/vectors/uniform.py` & `autoarray-2023.7.7.1/autoarray/structures/vectors/uniform.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,14 @@
         obj = values.view(cls)
         obj.grid = Grid2D(values=grid, mask=mask)
         obj.mask = mask
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
         if hasattr(obj, "grid"):
             self.grid = obj.grid
 
     @classmethod
@@ -278,15 +277,14 @@
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = grid_2d_util.convert_grid(grid=values)
 
         if len(values.shape) == 2:
-
             if shape_native is None:
                 raise exc.VectorYXException(
                     f"""
                     The input vectors are not in their native shape (an ndarray / list of 
                     shape [total_y_pixels, total_x_pixels, 2]) and the shape_native parameter has not been input the 
                     VectorYX2D function.
     
@@ -300,15 +298,14 @@
                 raise exc.GridException(
                     """
                     The input shape_native parameter is not a tuple of type (int, int).
                     """
                 )
 
         else:
-
             shape_native = (
                 int(values.shape[0] / sub_size),
                 int(values.shape[1] / sub_size),
             )
 
         grid = Grid2D.uniform(
             shape_native=shape_native,
```

### Comparing `autoarray-2023.3.27.1/autoarray/structures/visibilities.py` & `autoarray-2023.7.7.1/autoarray/structures/visibilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from autoarray.structures.arrays import array_2d_util
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class AbstractVisibilities(Structure):
-
     # noinspection PyUnusedLocal
     def __new__(cls, visibilities: Union[np.ndarray, List[complex]], *args, **kwargs):
         """
         A collection of (real, imag) visibilities which are used to represent the data in an `Interferometer` dataset.
 
         The (real, imag) visibilities are stored as a 1D complex NumPy array of shape [total_visibilities]. These can
         be mapped to a 2D real NumPy array of shape [total_visibilities, 2] and a `Grid2DIrregular` data structure
@@ -54,15 +53,14 @@
         obj.ordered_1d = np.concatenate(
             (np.real(visibilities), np.imag(visibilities)), axis=0
         )
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "ordered_1d"):
             self.ordered_1d = obj.ordered_1d
 
     @property
     def slim(self) -> "AbstractVisibilities":
         return self
 
@@ -205,15 +203,14 @@
         visibilities_1d = array_2d_util.numpy_array_2d_via_fits_from(
             file_path=file_path, hdu=hdu
         )
         return cls(visibilities=visibilities_1d)
 
 
 class VisibilitiesNoiseMap(Visibilities):
-
     # noinspection PyUnusedLocal
     def __new__(cls, visibilities: Union[np.ndarray, List[complex]], *args, **kwargs):
         """
         A collection of (real, imag) visibilities noise-map values which are used to represent the noise-map in
         an `Interferometer` dataset.
 
         This data structure behaves the same as the `Visibilities` structure (see `AbstractVisibilities.__new__`). The
@@ -250,13 +247,12 @@
         obj.weight_list_ordered_1d = np.concatenate(
             (weight_list[:, 0], weight_list[:, 1]), axis=0
         )
 
         return obj
 
     def __array_finalize__(self, obj):
-
         if hasattr(obj, "ordered_1d"):
             self.ordered_1d = obj.ordered_1d
 
         if hasattr(obj, "weight_list_ordered_1d"):
             self.weight_list_ordered_1d = obj.weight_list_ordered_1d
```

### Comparing `autoarray-2023.3.27.1/autoarray/type.py` & `autoarray-2023.7.7.1/autoarray/type.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/__init__.py` & `autoarray-2023.7.7.1/autoarray/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/misc_util.py` & `autoarray-2023.7.7.1/autoarray/util/misc_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/README.md` & `autoarray-2023.7.7.1/autoarray/util/nn/README.md`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/nn_py.py` & `autoarray-2023.7.7.1/autoarray/util/nn/nn_py.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         ctypes.POINTER(ctypes.c_double),
         ctypes.POINTER(ctypes.c_int),
         ctypes.c_int,
     )
     interpolate_from.restype = ctypes.c_int
 
     def natural_interpolation_weights(x_in, y_in, x_target, y_target, max_nneighbours):
-
         nin = len(x_in)
         nout = len(x_target)
 
         z_in = np.zeros(len(x_in), dtype=np.double)
 
         weights_out = np.zeros(nout * max_nneighbours, dtype=np.double)
         neighbour_indexes_out = np.zeros(nout * max_nneighbours, dtype=np.intc) - 1
@@ -69,15 +68,14 @@
 
         return (
             weights_out.reshape((nout, max_nneighbours)),
             neighbour_indexes_out.reshape((nout, max_nneighbours)),
         )
 
     def natural_interpolation(x_in, y_in, z_in, x_target, y_target):
-
         nin = len(x_in)
         nout = len(x_target)
 
         z_target = np.zeros(nout, dtype=np.double)
         z_marker = np.zeros(nout, dtype=np.intc)
 
         flag = interpolate_from(
```

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/README.md` & `autoarray-2023.7.7.1/autoarray/util/nn/src/README.md`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/.indent.pro` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/.indent.pro`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/CHANGELOG` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CHANGELOG`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/CUSTOMISE` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CUSTOMISE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/LICENSE` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/LICENSE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/README` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/configure` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/configure.in` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure.in`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/delaunay.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/delaunay.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/delaunay_internal.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay_internal.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/distribute.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/distribute.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/generate.awk` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/generate.awk`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/suptitle.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/suptitle.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/test.sh` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/1/viewexample.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/README` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/data.txt` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/makefile` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/makefile`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/mpitest.sh` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/mpitest.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/suptitle.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/suptitle.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/test.sh` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/viewdata.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewdata.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/viewexample.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/2/viewinterp.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/README` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/3/test.sh` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/README` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/data.txt` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/test.sh` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/viewdata.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewdata.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/viewexample.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/4/viewinterp.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/data.txt` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/viewexample.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/viewinterp.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/5/viewinterp2.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp2.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/README` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/data.txt` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/6/viewinterp.m` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/examples/README` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/hash.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/hash.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/install-sh` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/install-sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/istack.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/istack.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/istack_internal.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack_internal.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/lpi.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/lpi.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/makefile.example` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.example`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/makefile.in` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.in`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/makefile_autolens` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile_autolens`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/minell.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/minell.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/mkinstalldirs` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/mkinstalldirs`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nan.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nan.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nn.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nn_internal.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn_internal.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnai.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnai.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnbathy.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnbathy.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nncommon-vulnerable.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon-vulnerable.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nncommon.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnhpi_customized.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnhpi_customized.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/nnpi.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnpi.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/preader.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/preader.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/sample.py` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/sample.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/triangle.c` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray/util/nn/src/nn/triangle.h` & `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/autoarray.egg-info/SOURCES.txt` & `autoarray-2023.7.7.1/autoarray.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,16 @@
 autoarray/structures/plot/__init__.py
 autoarray/structures/plot/structure_plotters.py
 autoarray/structures/vectors/__init__.py
 autoarray/structures/vectors/abstract.py
 autoarray/structures/vectors/irregular.py
 autoarray/structures/vectors/uniform.py
 autoarray/util/__init__.py
+autoarray/util/cholesky_funcs.py
+autoarray/util/fnnls.py
 autoarray/util/misc_util.py
 autoarray/util/nn/README.md
 autoarray/util/nn/nn_py.py
 autoarray/util/nn/src/README.md
 autoarray/util/nn/src/nn/.indent.pro
 autoarray/util/nn/src/nn/CHANGELOG
 autoarray/util/nn/src/nn/CUSTOMISE
```

### Comparing `autoarray-2023.3.27.1/docs/Makefile` & `autoarray-2023.7.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/docs/conf.py` & `autoarray-2023.7.7.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     "doc_module": "pyautoarray",
     # Insert links to documentation of objects in the examples
     "reference_url": {"pyautoarray": None},
 }
 
 # -- Options for HTML output -------------------------------------------------
 
-# The theme to use for HTML and HTML Help pages.  See the documentation for
+# theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
 html_last_updated_fmt = "%b %d, %Y"
 html_title = "PyAutoArray"
 html_short_title = "PyAutoArray"
 pygments_style = "default"
```

### Comparing `autoarray-2023.3.27.1/docs/make.bat` & `autoarray-2023.7.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/files/release.sh` & `autoarray-2023.7.7.1/files/release.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/files/to_do_list` & `autoarray-2023.7.7.1/files/to_do_list`

 * *Files identical despite different names*

### Comparing `autoarray-2023.3.27.1/setup.py` & `autoarray-2023.7.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.3.27.1")
+version = environ.get("VERSION", "2023.7.7.1")
 requirements.extend([f"autoconf=={version}"])
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
-    for (path, directories, filenames) in os.walk(directory):
+    for path, directories, filenames in os.walk(directory):
         for directory in directories:
             paths.append(f"{path}/{directory}".replace("/", "."))
     return paths
 
 
 setup(
     name="autoarray",
```

### Comparing `autoarray-2023.3.27.1/to_do_list` & `autoarray-2023.7.7.1/to_do_list`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
 - Think very carefully about how Preloads and w_tilde interface with database. Pickle array? Large filesize
-but fast. Need to be careful with hyper galaxies.
+but fast. Need to be careful with galaxies.
 
 
 __Refactor__
 
 - Use composition in visualization MatPlot objects instead of inheritance.
 - Extract geometry from mask package.
 - auto_labels in visuals as a config loady thing.
```

