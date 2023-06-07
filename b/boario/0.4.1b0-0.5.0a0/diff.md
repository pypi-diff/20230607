# Comparing `tmp/boario-0.4.1b0.tar.gz` & `tmp/boario-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "boario-0.5.0a0.tar", max compression
```

## Comparing `boario-0.4.1b0.tar` & `boario-0.5.0a0.tar`

### file list

```diff
@@ -1,343 +1,12 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 boario-0.4.1b0/CONTRIBUTING.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 boario-0.4.1b0/requirements.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 boario-0.4.1b0/testpyrightconfig.json
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/__init__.py
--rw-r--r--   0        0        0    28775 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/event.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/extended_models.py
--rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/indicators.py
--rw-r--r--   0        0        0    61446 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/model_base.py
--rw-r--r--   0        0        0    27307 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/simulation.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 boario-0.4.1b0/boario/utils/misc.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/aggreg_exio3.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/csv_from_indicators.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/flood_country_aggreg.py
--rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/generate-example-files.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/indicator_from_folder.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/indicators_batch.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/model_testing.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/mono_run.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/mono_run_2.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 boario-0.4.1b0/scripts/versatile-env.yml
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/__init__.pyi
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_typing.pyi
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_version.pyi
--rw-r--r--   0        0        0    26216 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/conftest.pyi
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/testing.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_config/__init__.pyi
--rw-r--r--   0        0        0     8900 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_config/config.pyi
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_config/dates.pyi
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_config/display.pyi
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_config/localization.pyi
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/__init__.pyi
--rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/algos.pyi
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/arrays.pyi
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/groupby.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/hashing.pyi
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/hashtable.pyi
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/index.pyi
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/indexing.pyi
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/internals.pyi
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/interval.pyi
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/join.pyi
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/json.pyi
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/lib.pyi
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/missing.pyi
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/ops.pyi
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/ops_dispatch.pyi
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/parsers.pyi
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/properties.pyi
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/reduction.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/reshape.pyi
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/sparse.pyi
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/testing.pyi
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslib.pyi
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/writers.pyi
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/__init__.pyi
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/ccalendar.pyi
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/conversion.pyi
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/dtypes.pyi
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/fields.pyi
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/nattype.pyi
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/np_datetime.pyi
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/offsets.pyi
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/parsing.pyi
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/period.pyi
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/strptime.pyi
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/timedeltas.pyi
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/timestamps.pyi
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/timezones.pyi
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/tzconversion.pyi
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/tslibs/vectorized.pyi
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/window/aggregations.pyi
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_libs/window/indexers.pyi
--rw-r--r--   0        0        0    15222 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/__init__.pyi
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/_hypothesis.pyi
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/_io.pyi
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/_random.pyi
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/_warnings.pyi
--rw-r--r--   0        0        0    19021 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/asserters.pyi
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/compat.pyi
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/_testing/contexts.pyi
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/api/__init__.pyi
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/api/extensions/__init__.pyi
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/api/indexers/__init__.pyi
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/api/interchange/__init__.pyi
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/api/types/__init__.pyi
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/arrays/__init__.pyi
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/__init__.pyi
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/_optional.pyi
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/chainmap.pyi
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/pickle_compat.pyi
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/pyarrow.pyi
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/numpy/__init__.pyi
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/compat/numpy/function.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/__init__.pyi
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/accessor.pyi
--rw-r--r--   0        0        0    23044 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/algorithms.pyi
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/api.pyi
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/apply.pyi
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arraylike.pyi
--rw-r--r--   0        0        0    20637 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/base.pyi
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/common.pyi
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/config_init.pyi
--rw-r--r--   0        0        0    12286 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/construction.pyi
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/describe.pyi
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/flags.pyi
--rw-r--r--   0        0        0   227028 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/frame.pyi
--rw-r--r--   0        0        0   244582 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/generic.pyi
--rw-r--r--   0        0        0    20620 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexing.pyi
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/missing.pyi
--rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/nanops.pyi
--rw-r--r--   0        0        0    21004 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/resample.pyi
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/roperator.pyi
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/sample.pyi
--rw-r--r--   0        0        0   119354 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/series.pyi
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/shared_docs.pyi
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/sorting.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/__init__.pyi
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/executor.pyi
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/kernels/__init__.pyi
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/kernels/mean_.pyi
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/kernels/min_max_.pyi
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/kernels/shared.pyi
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/kernels/sum_.pyi
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/_numba/kernels/var_.pyi
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/__init__.pyi
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/masked_reductions.pyi
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/putmask.pyi
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/quantile.pyi
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/replace.pyi
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/take.pyi
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/array_algos/transforms.pyi
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/__init__.pyi
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/_mixins.pyi
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/_ranges.pyi
--rw-r--r--   0        0        0    27086 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/base.pyi
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/boolean.pyi
--rw-r--r--   0        0        0    44244 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/categorical.pyi
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/datetimelike.pyi
--rw-r--r--   0        0        0    25252 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/datetimes.pyi
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/floating.pyi
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/integer.pyi
--rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/interval.pyi
--rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/masked.pyi
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/numeric.pyi
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/numpy_.pyi
--rw-r--r--   0        0        0    10020 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/period.pyi
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/string_.pyi
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/string_arrow.pyi
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/timedeltas.pyi
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/arrow/__init__.pyi
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/arrow/_arrow_utils.pyi
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/arrow/array.pyi
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/arrow/dtype.pyi
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/arrow/extension_types.pyi
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/sparse/__init__.pyi
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/sparse/accessor.pyi
--rw-r--r--   0        0        0    16515 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/sparse/array.pyi
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/sparse/dtype.pyi
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/arrays/sparse/scipy_sparse.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/__init__.pyi
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/align.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/api.pyi
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/check.pyi
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/common.pyi
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/engines.pyi
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/eval.pyi
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/expr.pyi
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/expressions.pyi
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/ops.pyi
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/parsing.pyi
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/pytables.pyi
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/computation/scope.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/__init__.pyi
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/api.pyi
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/astype.pyi
--rw-r--r--   0        0        0    10020 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/base.pyi
--rw-r--r--   0        0        0    15435 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/cast.pyi
--rw-r--r--   0        0        0    32598 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/common.pyi
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/concat.pyi
--rw-r--r--   0        0        0    16316 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/dtypes.pyi
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/generic.pyi
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/inference.pyi
--rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/dtypes/missing.pyi
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/__init__.pyi
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/base.pyi
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/categorical.pyi
--rw-r--r--   0        0        0    12625 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/generic.pyi
--rw-r--r--   0        0        0    44577 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/groupby.pyi
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/grouper.pyi
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/indexing.pyi
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/numba_.pyi
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/groupby/ops.pyi
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexers/__init__.pyi
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexers/objects.pyi
--rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexers/utils.pyi
--rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/accessors.pyi
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/api.pyi
--rw-r--r--   0        0        0    81332 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/base.pyi
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/category.pyi
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/datetimelike.pyi
--rw-r--r--   0        0        0    19996 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/datetimes.pyi
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/extension.pyi
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/frozen.pyi
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/interval.pyi
--rw-r--r--   0        0        0    40304 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/multi.pyi
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/numeric.pyi
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/period.pyi
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/range.pyi
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/indexes/timedeltas.pyi
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/interchange/buffer.pyi
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/interchange/column.pyi
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/interchange/dataframe.pyi
--rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/interchange/dataframe_protocol.pyi
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/interchange/from_dataframe.pyi
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/interchange/utils.pyi
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/__init__.pyi
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/api.pyi
--rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/array_manager.pyi
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/base.pyi
--rw-r--r--   0        0        0    18961 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/blocks.pyi
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/concat.pyi
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/construction.pyi
--rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/managers.pyi
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/internals/ops.pyi
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/__init__.pyi
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/array_ops.pyi
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/common.pyi
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/dispatch.pyi
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/docstrings.pyi
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/invalid.pyi
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/mask_ops.pyi
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/methods.pyi
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/ops/missing.pyi
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/api.pyi
--rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/concat.pyi
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/encoding.pyi
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/melt.pyi
--rw-r--r--   0        0        0    17563 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/merge.pyi
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/pivot.pyi
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/reshape.pyi
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/tile.pyi
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/reshape/util.pyi
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/strings/__init__.pyi
--rw-r--r--   0        0        0    62941 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/strings/accessor.pyi
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/strings/base.pyi
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/strings/object_array.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/tools/__init__.pyi
--rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/tools/datetimes.pyi
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/tools/numeric.pyi
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/tools/timedeltas.pyi
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/tools/times.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/util/__init__.pyi
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/util/hashing.pyi
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/util/numba_.pyi
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/__init__.pyi
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/common.pyi
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/doc.pyi
--rw-r--r--   0        0        0    16510 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/ewm.pyi
--rw-r--r--   0        0        0    19347 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/expanding.pyi
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/numba_.pyi
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/online.pyi
--rw-r--r--   0        0        0    36207 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/core/window/rolling.pyi
--rw-r--r--   0        0        0    16479 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/errors/__init__.pyi
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/__init__.pyi
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/api.pyi
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/clipboards.pyi
--rw-r--r--   0        0        0    10050 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/common.pyi
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/date_converters.pyi
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/feather_format.pyi
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/gbq.pyi
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/html.pyi
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/orc.pyi
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parquet.pyi
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/pickle.pyi
--rw-r--r--   0        0        0    48583 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/pytables.pyi
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/spss.pyi
--rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sql.pyi
--rw-r--r--   0        0        0    22766 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/stata.pyi
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/xml.pyi
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/clipboard/__init__.pyi
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/__init__.pyi
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_base.pyi
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_odfreader.pyi
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_odswriter.pyi
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_openpyxl.pyi
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_pyxlsb.pyi
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_util.pyi
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_xlrd.pyi
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_xlsxwriter.pyi
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/excel/_xlwt.pyi
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/__init__.pyi
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/_color_data.pyi
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/console.pyi
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/css.pyi
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/csvs.pyi
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/excel.pyi
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/format.pyi
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/html.pyi
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/info.pyi
--rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/latex.pyi
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/printing.pyi
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/string.pyi
--rw-r--r--   0        0        0   104532 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/style.pyi
--rw-r--r--   0        0        0    22153 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/style_render.pyi
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/formats/xml.pyi
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/json/__init__.pyi
--rw-r--r--   0        0        0    17268 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/json/_json.pyi
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/json/_normalize.pyi
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/json/_table_schema.pyi
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parsers/__init__.pyi
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parsers/arrow_parser_wrapper.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parsers/base_parser.pyi
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parsers/c_parser_wrapper.pyi
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parsers/python_parser.pyi
--rw-r--r--   0        0        0    23985 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/parsers/readers.pyi
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sas/__init__.pyi
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sas/_sas.pyi
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sas/sas7bdat.pyi
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sas/sas_constants.pyi
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sas/sas_xport.pyi
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/io/sas/sasreader.pyi
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/plotting/__init__.pyi
--rw-r--r--   0        0        0    42967 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/plotting/_core.pyi
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/plotting/_misc.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/tests/__init__.pyi
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/tseries/__init__.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/tseries/api.pyi
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/tseries/frequencies.pyi
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/tseries/offsets.pyi
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/__init__.pyi
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/_decorators.pyi
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/_exceptions.pyi
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/_print_versions.pyi
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/_test_decorators.pyi
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/_tester.pyi
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/_validators.pyi
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/testing.pyi
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 boario-0.4.1b0/typings/pandas/util/version/__init__.pyi
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 boario-0.4.1b0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 boario-0.4.1b0/LICENSE
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 boario-0.4.1b0/README.rst
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 boario-0.4.1b0/pyproject.toml
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 boario-0.4.1b0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 12:53:43.248820 boario-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     4176 2023-06-07 13:53:07.484155 boario-0.5.0a0/README.rst
+-rw-r--r--   0        0        0     1793 2023-06-07 13:34:43.699811 boario-0.5.0a0/boario/__init__.py
+-rw-r--r--   0        0        0    52394 2023-06-07 13:34:43.699811 boario-0.5.0a0/boario/event.py
+-rw-r--r--   0        0        0     7791 2023-06-07 13:34:43.699811 boario-0.5.0a0/boario/extended_models.py
+-rw-r--r--   0        0        0    28717 2023-06-07 13:34:43.699811 boario-0.5.0a0/boario/indicators.py
+-rw-r--r--   0        0        0    70186 2023-06-07 13:34:43.703811 boario-0.5.0a0/boario/model_base.py
+-rw-r--r--   0        0        0    40625 2023-06-07 13:34:43.703811 boario-0.5.0a0/boario/simulation.py
+-rw-r--r--   0        0        0     4944 2023-06-07 13:34:43.703811 boario-0.5.0a0/boario/utils/misc.py
+-rw-r--r--   0        0        0     4065 2023-06-07 13:34:43.703811 boario-0.5.0a0/boario/utils/recovery_functions.py
+-rw-r--r--   0        0        0     2113 2023-06-07 13:47:28.318350 boario-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5116 1970-01-01 00:00:00.000000 boario-0.5.0a0/PKG-INFO
```

### Comparing `boario-0.4.1b0/boario/event.py` & `boario-0.5.0a0/boario/indicators.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,597 +10,740 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
-from typing import Callable, Optional
-from numpy.typing import ArrayLike
-import warnings
+
+from typing import Optional, Union
+
+from boario.extended_models import ARIOPsiModel
+from boario.simulation import Simulation
+import numpyencoder
+import json
+import pathlib
 import numpy as np
+import pandas as pd
+import itertools
+from boario.utils import misc
+import dask.dataframe as da
 from boario import logger
-import math
-import inspect
-from functools import partial
-
-__all__ = ['Event']
-
-def linear_recovery(elapsed_temporal_unit:int,init_kapital_destroyed:np.ndarray,recovery_time:int):
-    """Linear Kapital recovery function
-
-    Kapital is entirely recovered when `recovery_time` has passed since event
-    started recovering
-
-    Parameters
-    ----------
-    init_kapital_destroyed : float
-        Initial kapital destroyed
-    elapsed_temporal_unit : int
-        Elapsed time since event started recovering
-    recovery_time : int
-        Total time it takes the event to fully recover
-
-    Examples
-    --------
-    FIXME: Add docs.
-
-    """
-
-    return init_kapital_destroyed * (1-(elapsed_temporal_unit/recovery_time))
-
-def convexe_recovery(elapsed_temporal_unit:int,init_kapital_destroyed:np.ndarray,recovery_time:int):
-    """Convexe Kapital recovery function
-
-    Kapital is recovered with characteristic time `recovery_time`. (This doesn't mean Kapital is fully recovered after this time !)
-    This function models a recovery similar as the one happening in the rebuilding case, for the same characteristic time.
-
-    Parameters
-    ----------
-    init_kapital_destroyed : float
-        Initial kapital destroyed
-    elapsed_temporal_unit : int
-        Elapsed time since event started recovering
-    recovery_time : int
-        Total time it takes the event to fully recover
-
-    """
-    return init_kapital_destroyed * (1-(1/recovery_time))**elapsed_temporal_unit
-
-def convexe_recovery_scaled(elapsed_temporal_unit:int,init_kapital_destroyed:np.ndarray,recovery_time:int,scaling_factor:float=4):
-    """Convexe Kapital recovery function (scaled to match other recovery duration)
-
-    Kapital is mostly recovered (>95% by default for most cases) when `recovery_time` has passed since event
-    started recovering.
-
-    Parameters
-    ----------
-    init_kapital_destroyed : float
-        Initial kapital destroyed
-    elapsed_temporal_unit : int
-        Elapsed time since event started recovering
-    recovery_time : int
-        Total time it takes the event to fully recover
-    scaling_factor: float
-        Used to scale the exponent in the function so that kapital is mostly rebuilt after `recovery_time`.
-    A value of 4 insure >95% of kapital is recovered for a reasonable range of `recovery_time` values.
-
-    """
-    return init_kapital_destroyed * (1-(1/recovery_time))**(scaling_factor*elapsed_temporal_unit)
-
-def concave_recovery(elapsed_temporal_unit:int,init_kapital_destroyed:np.ndarray,recovery_time:int,steep_factor:float=0.000001,half_recovery_time:Optional[int]=None):
-    """Concave (s-shaped) Kapital recovery function
-
-    Kapital is mostly (>95% in most cases) recovered when `recovery_time` has passed since event started recovering.
-
-    Parameters
-    ----------
-    init_kapital_destroyed : float
-        Initial kapital destroyed
-    elapsed_temporal_unit : int
-        Elapsed time since event started recovering
-    recovery_time : int
-        Total time it takes the event to fully recover
-    steep_factor: float
-        This coefficient governs the slope of the central part of the s-shape, smaller values lead to a steeper slope. As such it also affect the percentage of kapital rebuilt
-    after `recovery_time` has elapsed. A value of 0.000001 should insure 95% of the kapital is rebuild for a reasonable range of recovery duration.
-    half_recovery_time : int
-        This can by use to change the time the inflexion point of the s-shape curve is attained. By default it is set to half the recovery duration.
-
-    """
-    if half_recovery_time is None:
-        tau_h = 2
-    else:
-        tau_h = recovery_time/half_recovery_time
-    exponent = (np.log(recovery_time)-np.log(steep_factor))/(np.log(recovery_time)-np.log(tau_h))
-    return (init_kapital_destroyed * recovery_time)/(recovery_time + steep_factor*(elapsed_temporal_unit**exponent))
-
-
-class Event(object):
-    """Create an event shocking the model from a dictionary.
-
-    Events store all information about a unique shock during simulation such as
-    time of occurrence, duration, type of shock, amount of damages. Computation
-    of recovery or initialy requested rebuilding demand is also done in this
-    class.
-
-    Parameters
-    ----------
-
-    event : dict
-        A dictionary holding the necessary information to define an event.
-
-    Examples
-    --------
-    FIXME: Add docs.
-
-    """
-
-    # Class Attributes
-    __required_class_attributes = ["possible_sectors","possible_regions","temporal_unit_range","z_shape","y_shape","x_shape","regions_idx","sectors_idx","monetary_unit","sectors_gva_shares","Z_distrib","mrio_name"]
-    possible_sectors : np.ndarray = None #type: ignore
-    """List of sectors present in the MRIO used by the model"""
-    possible_regions : np.ndarray = None #type: ignore
-    """List of regions present in the MRIO used by the model"""
-    temporal_unit_range : int = None #type: ignore
-    """Maximum temporal unit simulated"""
-    z_shape : tuple[int,int] = None #type: ignore
-    """Shape of the Z (intermediate consumption) matrix in the model"""
-    y_shape : tuple[int,int] = None #type: ignore
-    """Shape of the Y (final demand) matrix in the model"""
-    x_shape : tuple[int,int] = None #type: ignore
-    """Shape of the x (production) vector in the model"""
-    regions_idx : np.ndarray = None #type: ignore
-    """lexicographic region indexes"""
-    sectors_idx : np.ndarray = None #type: ignore
-    """lexicographic sector indexes"""
-    monetary_unit : int = None #type: ignore
-    """Amount of unitary currency used in the MRIO (e.g. 1000000 if in € millions)"""
-    sectors_gva_shares : np.ndarray = None #type: ignore
-    """Fraction of total (regional) GVA for each sectors"""
-    Z_distrib: np.ndarray = None #type: ignore
-    """Normalized intermediate consumption matrix"""
-    mrio_name: str = ""
-    """MRIO identification"""
-
-    # Instance Attributes
-    shock_type = None
-    """Type of shock (arbitrary production capacity loss (wip), productive kapital destroyed (with or without rebuilding demand)) (`str`)"""
-    name = None
-    """Name of the event (`str`)"""
-    total_kapital_destroyed = None
-    """Total amount of kapital destroyed by the event (`int`|`None`)"""
-    happened : bool = False
-    """Boolean stating if the event already happened during the simulation (`bool`)"""
-    rebuild_tau = None
-    """Characteristic number of temporal unit required to recover or rebuild the from the event (`int`)"""
-    over = None
-    """Boolean stating if the event is over (completely recovered or rebuilt)"""
-    event_dict = None
-    """Dictionary of the event"""
-
-    _recoverable_kind : bool = False
-    _recoverable : bool = False
-    _rebuildable_kind : bool = False
-    _rebuildable : bool = False
-    _recovery_fun : Optional[Callable] = None
-    _regional_sectoral_kapital_destroyed_evol = None
-
-    def __init__(self, event:dict) -> None:
-        super().__init__()
-        if event.get("globals_var") is not None:
-            for k,v in event["globals_var"].items():
-                if Event.__dict__[k] != v:
-                    logger.warning("""You are trying to load an event which was simulated under different global vars, this might break: key:{} with value {} in dict and {} in Event class""".format(k,v,Event.__dict__[k]))
-        for v in Event.__required_class_attributes:
-            if Event.__dict__[v] is None:
-                raise AttributeError("Required Event Class attribute {} is not set yet so instantiating an Event isn't possible".format(v))
-        self.shock_type = event["shock_type"]
-        self.name = event.get("name","unnamed")
-        self.occurrence = event.get("occur",1)
-        self.duration = event.get("duration",1)
-        self.aff_regions = event["aff_regions"]
-        self.aff_sectors = event["aff_sectors"]
-        self.dmg_regional_distrib = event.get("dmg_regional_distrib",[1/self.aff_regions.size for _ in range(self.aff_regions.size)])
-        self.dmg_sectoral_distrib_type = event.get("dmg_sectoral_distrib_type","equally shared")
-        self.dmg_sectoral_distrib = event.get("dmg_sectoral_distrib",[1/self.aff_sectors.size for _ in range(self.aff_sectors.size)])
-        self.rebuilding_sectors = event.get("rebuilding_sectors")
-        self.total_kapital_destroyed = event.get("kapital_damage")
-        self.regional_sectoral_kapital_destroyed = None
-        self.rebuilding_demand_house = None
-        self.rebuilding_demand_indus = None
-        self.production_share_allocated = None
-        self.prod_cap_delta_arbitrary = None
-        self.happened = False
-        self._recoverable_kind : bool = False
-        self._recoverable : bool = False
-        self._rebuildable_kind : bool = False
-        self._rebuildable : bool = False
-        self._recovery_fun : Optional[Callable] = None
-        self.rebuild_tau = event.get("rebuild_tau")
-        self.over = False
-        self.init_shock(event)
-        self.event_dict = event
-        self.event_dict["globals_vars"] = {
-            "possible_sectors" : list(self.possible_sectors),
-            "possible_regions" : list(self.possible_regions),
-            "temporal_unit_range" : self.temporal_unit_range,
-            "z_shape" : self.z_shape,
-            "y_shape" : self.y_shape,
-            "x_shape" : self.x_shape,
-            "monetary_unit" : self.monetary_unit,
-            "mrio_used" : self.mrio_name
-            }
-
-    @property
-    def recovery_function(self)->Optional[Callable]:
-        """The recovery function used for recovery (`Callable`)"""
-        return self._recovery_fun
-
-    @recovery_function.setter
-    def recovery_function(self,r_fun:str|Callable|None):
-        if self.shock_type == "kapital_destroyed_recover":
-            if r_fun is None:
-                r_fun = "linear"
-            if self.recovery_time is None:
-                raise AttributeError("Impossible to set recovery function if no recovery time is given.")
-            if isinstance(r_fun,str):
-                if r_fun == "linear":
-                    fun = linear_recovery
-                elif r_fun == "convexe":
-                    fun = convexe_recovery_scaled
-                elif r_fun == "convexe noscale":
-                    fun = convexe_recovery
-                elif r_fun == "concave":
-                    fun = concave_recovery
-                else:
-                    raise NotImplementedError("No implemented recovery function corresponding to {}".format(r_fun))
-            elif callable(r_fun):
-                r_fun_argsspec = inspect.getfullargspec(r_fun)
-                r_fun_args = r_fun_argsspec.args + r_fun_argsspec.kwonlyargs
-                if not all(args in r_fun_args for args in ["init_kapital_destroyed","elapsed_temporal_unit","recovery_time"]):
-                    raise ValueError("Recovery function has to have at least the following keyword arguments: {}".format(["init_kapital_destroyed","elapsed_temporal_unit","recovery_time"]))
-                fun = r_fun
+from boario.event import *
 
-            else:
-                raise ValueError("Given recovery function is not a str or callable")
+__all__ = ["Indicators"]
 
-            r_fun_partial = partial(fun, init_kapital_destroyed=self._regional_sectoral_kapital_destroyed_0, recovery_time=self.recovery_time)
-            self._recovery_fun = r_fun_partial
-        else:
-            self._recovery_fun = None
 
-    @property
-    def occurrence(self)->int:
-        """The temporal unit of occurrence of the event."""
-        return self._occur
-
-    @occurrence.setter
-    def occurrence(self, value:int):
-        if not 0 <= value <= self.temporal_unit_range:
-            raise ValueError("Occurrence of event is not in the range of simulation steps : {} not in [0-{}]".format(value, self.temporal_unit_range))
-        else:
-            self._occur=value
+def create_df(data, regions, sectors):
+    df = pd.DataFrame(
+        data,
+        columns=pd.MultiIndex.from_product(
+            [regions, sectors], names=["region", "sector"]
+        ),
+    )
+    df = df.interpolate()
+    df = df.rename_axis("step")
+    return df
+
+
+def df_from_memmap(memmap: np.memmap, indexes: dict) -> pd.DataFrame:
+    a = pd.DataFrame(
+        memmap,
+        columns=pd.MultiIndex.from_product([indexes["regions"], indexes["sectors"]]),
+    )
+    a["step"] = a.index
+    return a
+
+
+def stock_df_from_memmap(
+    memmap: np.memmap, indexes: dict, timesteps: int, timesteps_simulated: int
+) -> pd.DataFrame:
+    a = pd.DataFrame(
+        memmap.reshape(timesteps * indexes["n_sectors"], -1),
+        index=pd.MultiIndex.from_product(
+            [timesteps, indexes["sectors"]], names=["step", "stock of"]
+        ),
+        columns=pd.MultiIndex.from_product([indexes["regions"], indexes["sectors"]]),
+    )
+    a = a.loc[pd.IndexSlice[:timesteps_simulated, :]]
+    return a
+
+
+class Indicators(object):
+    record_files_list = [
+        "final_demand",
+        "intermediate_demand",
+        "final_demand_unmet",
+        "production_capacity",
+        "production_realised",
+        "limiting_inputs",
+        "overproduction",
+        "rebuild_demand",
+        "rebuild_prod",
+        "productive_capital_to_recover",
+    ]
+
+    params_list = ["simulated_params", "simulated_events"]
+
+    def __init__(
+        self,
+        *,
+        has_crashed,
+        params,
+        regions,
+        sectors,
+        productive_capital,
+        prod,
+        prodmax,
+        overprod,
+        final_demand,
+        io_demand,
+        r_demand,
+        r_prod,
+        fd_unmet,
+        limiting_stocks,
+        n_temporal_units_to_sim: int,
+        n_temporal_units_by_step: int,
+        events: list[Event],
+        results_storage: Optional[str | pathlib.Path] = None,
+        psi_param: Optional[float] = None,
+        inventory_restoration_tau: Optional[int | list[int]] = None,
+        stocks=None,
+        stocks_treatment=False,
+        include_crash: bool = False,
+    ) -> None:
+        logger.info("Instantiating indicators")
+        if not include_crash:
+            if has_crashed:
+                raise RuntimeError(
+                    "Simulation crashed and include_crash is False, I won't compute indicators"
+                )
+        steps = [i for i in range(n_temporal_units_to_sim)]
+
+        self.params = params
+        self.n_rows = n_temporal_units_to_sim
+        self.n_temporal_units_by_step = n_temporal_units_by_step
+
+        self.productive_capital_to_recover_df = create_df(
+            productive_capital, regions, sectors
+        )
+        self.production_realised_df = create_df(prod, regions, sectors)
+        self.production_capacity_df = create_df(prodmax, regions, sectors)
+        self.overproduction_df = create_df(overprod, regions, sectors)
+        self.final_demand_df = create_df(final_demand, regions, sectors)
+        self.intermediate_demand_df = create_df(io_demand, regions, sectors)
+        self.rebuild_demand_df = create_df(r_demand, regions, sectors)
+        self.rebuild_prod_df = create_df(r_prod, regions, sectors)
+        self.final_demand_unmet_df = create_df(fd_unmet, regions, sectors)
+
+        if stocks_treatment:
+            stocks_df = pd.DataFrame(
+                stocks.reshape(n_temporal_units_to_sim * len(sectors), -1),
+                index=pd.MultiIndex.from_product(
+                    [steps, sectors], names=["step", "stock of"]
+                ),
+                columns=pd.MultiIndex.from_product(
+                    [regions, sectors],
+                    names=["region", "sector"],
+                ),
+            )
+            stocks_df = stocks_df.replace([np.inf, -np.inf], np.nan).dropna(how="all")
+            stocks_df = stocks_df.astype(np.float32)
+            stocks_df = (
+                stocks_df.groupby("stock of")
+                .pct_change()
+                .fillna(0)
+                .add(1)
+                .groupby("stock of")
+                .cumprod()
+                .sub(1)
+            )  # type: ignore
+            stocks_df = stocks_df.melt(ignore_index=False).rename(
+                columns={
+                    "variable_0": "region",
+                    "variable_1": "sector",
+                    "variable_2": "stock of",
+                }
+            )
+            stocks_df = stocks_df.reset_index()
+            stocks_df["step"] = stocks_df["step"].astype("uint16")
+            stocks_df["stock of"] = stocks_df["stock of"].astype("category")
+            stocks_df["region"] = stocks_df["region"].astype("category")
+            stocks_df["sector"] = stocks_df["sector"].astype("category")
 
-    @property
-    def duration(self)->int:
-        """The duration of the event."""
-        return self._duration
-
-    @duration.setter
-    def duration(self, value:int):
-        if not 0 <= self.occurrence + value <= self.temporal_unit_range:
-            raise ValueError("Occurrence + duration of event is not in the range of simulation steps : {} + {} not in [0-{}]".format(self.occurrence, value, self.temporal_unit_range))
         else:
-            self._duration=value
+            stocks_df = None
 
-    @property
-    def aff_regions(self)->np.ndarray:
-        """The array of regions affected by the event"""
-        return self._aff_regions
-
-    @property
-    def aff_regions_idx(self)->np.ndarray:
-        """The array of lexicographically ordered affected region indexes"""
-        return self._aff_regions_idx
-
-    @aff_regions.setter
-    def aff_regions(self, value:ArrayLike|str):
-        if isinstance(value,str):
-            value = [value]
-        value = np.array(value)
-        impossible_regions = np.setdiff1d(value,self.possible_regions)
-        if impossible_regions.size > 0:
-            raise ValueError("These regions are not in the model : {}".format(impossible_regions))
-        else:
-            self._aff_regions = value
-            self._aff_regions_idx = np.searchsorted(self.possible_regions, value)
+        self.inputs_stocks_df = stocks_df
+        del stocks_df
+        # self.df_stocks = self.df_stocks.interpolate()
+
+        self.treated_loss_df = (
+            self.final_demand_unmet_df.melt(ignore_index=False)
+            .rename(
+                columns={
+                    "variable_0": "region",
+                    "variable_1": "fd_cat",
+                    "value": "fdloss",
+                }
+            )
+            .reset_index()
+        )
+
+        self.limiting_inputs_df = limiting_stocks
+        # pd.DataFrame(
+        #     limiting_stocks.reshape(n_temporal_units_to_sim * len(sectors), -1),
+        #     index=pd.MultiIndex.from_product(
+        #         [steps, sectors], names=["step", "stock of"]
+        #     ),
+        #     columns=pd.MultiIndex.from_product(
+        #         [regions, sectors], names=["region", "sector"]
+        #     ),
+        # )
+        self.aff_regions = []
+        self.aff_sectors = []
+        for e in events:
+            if isinstance(e, dict):
+                self.aff_sectors.append(e["aff_sectors"])
+                self.aff_regions.append(e["aff_regions"])
+            elif isinstance(e, Event):
+                self.aff_sectors.append(e.aff_sectors)
+                self.aff_regions.append(e.aff_regions)
+            else:
+                raise ValueError(f"Unrecognised event of type {type(e)}")
 
-    @property
-    def aff_sectors(self)->np.ndarray:
-        """The array of affected sectors by the event"""
-        return self._aff_sectors
-
-    @property
-    def aff_sectors_idx(self)->np.ndarray:
-        """The array of lexicographically ordered affected sectors indexes"""
-        return self._aff_sectors_idx
-
-    @aff_sectors.setter
-    def aff_sectors(self, value:ArrayLike|str):
-        if isinstance(value,str):
-            value = [value]
-        value = np.array(value)
-        impossible_sectors = np.setdiff1d(value,self.possible_sectors)
-        if impossible_sectors.size > 0 :
-            raise ValueError("These sectors are not in the model : {}".format(impossible_sectors))
-        else:
-            self._aff_sectors = value
-            self._aff_sectors_idx = np.searchsorted(self.possible_sectors, value)
+        self.aff_regions = list(misc.flatten(self.aff_regions))
+        self.aff_sectors = list(misc.flatten(self.aff_sectors))
 
-    @property
-    def dmg_regional_distrib(self)->np.ndarray:
-        """The array specifying how damages are distributed among affected regions"""
-        return self._dmg_regional_distrib
-
-    @dmg_regional_distrib.setter
-    def dmg_regional_distrib(self,value:ArrayLike):
-        if self.aff_regions is None:
-            raise AttributeError("Affected regions attribute isn't set yet")
-        value = np.array(value)
-        if value.size != self.aff_regions.size:
-            raise ValueError("There are {} affected regions by the event and length of given damage distribution is {}".format(self.aff_regions.size,value.size))
-        s = value.sum()
-        if not math.isclose(s,1):
-            raise ValueError("Damage distribution doesn't sum up to 1 but to {}, which is not valid".format(s))
-        self._dmg_regional_distrib = value
-
-    @property
-    def dmg_sectoral_distrib(self)->np.ndarray:
-        """The array specifying how damages are distributed among affected sectors"""
-        return self._dmg_sectoral_distrib
-
-    @dmg_sectoral_distrib.setter
-    def dmg_sectoral_distrib(self,value:ArrayLike):
-        if self.aff_sectors is None:
-            raise AttributeError("Affected sectors attribute isn't set yet")
-        value = np.array(value)
-        if value.size != self.aff_sectors.size:
-            raise ValueError("There are {} affected sectors by the event and length of given damage distribution is {}".format(self.aff_sectors.size,value.size))
-        s = value.sum()
-        if not math.isclose(s,1):
-            raise ValueError("Damage distribution doesn't sum up to 1 but to {}, which is not valid".format(s))
-        self._dmg_sectoral_distrib = value
-
-    @property
-    def dmg_sectoral_distrib_type(self)->str:
-        """The type of damages distribution among sectors (currently only 'gdp')"""
-        return self._dmg_sectoral_distrib_type
-
-    @dmg_sectoral_distrib_type.setter
-    def dmg_sectoral_distrib_type(self,value:str):
-        self._dmg_sectoral_distrib_type=value
-
-    @property
-    def rebuilding_sectors(self)->Optional[np.ndarray]:
-        """The (optional) array of rebuilding sectors"""
-        return self._rebuilding_sectors
-
-    @property
-    def rebuilding_sectors_idx(self)->Optional[np.ndarray]:
-        """The (optional) array of indexes of the rebuilding sectors (in lexicographic order)"""
-        return self._rebuilding_sectors_idx
-
-    @property
-    def rebuilding_sectors_shares(self)->Optional[np.ndarray]:
-        """The array specifying how rebuilding demand is distributed along the rebuilding sectors"""
-        return self._rebuilding_sectors_shares
-
-    @rebuilding_sectors.setter
-    def rebuilding_sectors(self, value:dict[str,float]|None):
-        if value is None:
-            self._rebuilding_sectors = None
-            self._rebuilding_sectors_idx = None
-        else:
-            reb_sectors = np.array(list(value.keys()))
-            reb_shares = np.array(list(value.values()))
-            impossible_sectors = np.setdiff1d(reb_sectors,self.possible_sectors)
-            if impossible_sectors.size > 0 :
-                raise ValueError("These sectors are not in the model : {}".format(impossible_sectors))
+        self.rebuilding_sectors = []
+
+        # This is working but wrong ! I need to fix it
+        for e in events:
+            if isinstance(e, dict):
+                self.rebuilding_sectors.append(e.get("rebuilding_sectors"))
+            if isinstance(e, EventKapitalRebuild):
+                self.rebuilding_sectors.append(list(e.rebuilding_sectors))
             else:
-                self._rebuilding_sectors = reb_sectors
-                self._rebuilding_sectors_idx = np.searchsorted(self.possible_sectors, reb_sectors)
-                self._rebuilding_sectors_shares = reb_shares
-
-    @property
-    def regional_sectoral_kapital_destroyed(self)->Optional[np.ndarray]:
-        """The (optional) array of kapital destroyed per industry (ie region x sector)"""
-        return self._regional_sectoral_kapital_destroyed
-
-    @regional_sectoral_kapital_destroyed.setter
-    def regional_sectoral_kapital_destroyed(self,value:ArrayLike|None):
-        if value is None:
-            self._regional_sectoral_kapital_destroyed = None
+                self.rebuilding_sectors = []
+
+        self.rebuilding_sectors = list(misc.flatten(self.rebuilding_sectors))
+        # This is also wrong but will settle for now
+        gdp_dmg_share = -1.0
+        self.indicators = {
+            "region": self.aff_regions,
+            "gdp_dmg_share": gdp_dmg_share,
+            "tot_fd_unmet": "unset",
+            "aff_fd_unmet": "unset",
+            "rebuild_durations": "unset",
+            "shortage_b": False,
+            "shortage_date_start": "unset",
+            "shortage_date_end": "unset",
+            "shortage_date_max": "unset",
+            "shortage_ind_max": "unset",
+            "shortage_ind_mean": "unset",
+            "10_first_shortages_(step,region,sector,stock_of)": "unset",
+            "prod_gain_tot": "unset",
+            "prod_lost_tot": "unset",
+            "prod_gain_unaff": "unset",
+            "prod_lost_unaff": "unset",
+            "psi": psi_param,
+            "inv_tau": inventory_restoration_tau,
+            "n_temporal_units_to_sim": n_temporal_units_to_sim,
+            "has_crashed": has_crashed,
+        }
+        if results_storage is not None:
+            self.storage_path = (pathlib.Path(results_storage)).resolve() / "indicators"
+            self.parquets_path = (pathlib.Path(results_storage)).resolve() / "parquets"
+            self.storage = self.storage_path / "indicators.json"
+            self.parquets_path.mkdir(parents=True, exist_ok=True)
+            self.storage_path.mkdir(parents=True, exist_ok=True)
+            self.save_dfs()
+
+    @classmethod
+    def from_simulation(
+        cls,
+        sim: Simulation,
+        results_storage: Optional[str | pathlib.Path] = None,
+        stocks_treatment: bool = False,
+        include_crash: bool = False,
+    ) -> Indicators:
+        if isinstance(sim.model, ARIOPsiModel):
+            psi = sim.model.psi
+            inventory_restoration_tau = list(sim.model.restoration_tau)
+        else:
+            psi = None
+            inventory_restoration_tau = None
+
+        prod = getattr(sim, "production_realised")
+        productive_capital = getattr(sim, "productive_capital_to_recover")
+        prodmax = getattr(sim, "production_capacity")
+        overprod = getattr(sim, "overproduction")
+        final_demand = getattr(sim, "final_demand")
+        io_demand = getattr(sim, "intermediate_demand")
+        r_demand = getattr(sim, "rebuild_demand")
+        r_prod = getattr(sim, "rebuild_prod")
+        fd_unmet = getattr(sim, "final_demand_unmet")
+        if stocks_treatment:
+            stocks = getattr(sim, "inputs_stocks")
         else:
-            value = np.array(value)
-            if value.shape != self.x_shape:
-                raise ValueError("Incorrect shape give for regional_sectoral_kapital_destroyed: {} given and {} expected".format(value.shape, self.x_shape))
-            self._regional_sectoral_kapital_destroyed = value
-
-    @property
-    def rebuilding_demand_house(self)->Optional[np.ndarray]:
-        """The optional array of rebuilding demand from households"""
-        return self._rebuilding_demand_house
-
-    @rebuilding_demand_house.setter
-    def rebuilding_demand_house(self,value:ArrayLike|None):
-        if value is None:
-            self._rebuilding_demand_house = None
+            stocks = None
+
+        limiting_stocks = getattr(sim, "limiting_inputs")
+        return cls(
+            has_crashed=sim.has_crashed,
+            params=sim.params_dict,
+            regions=sim.model.regions,
+            sectors=sim.model.sectors,
+            productive_capital=productive_capital,
+            prod=prod,
+            prodmax=prodmax,
+            overprod=overprod,
+            final_demand=final_demand,
+            io_demand=io_demand,
+            r_demand=r_demand,
+            r_prod=r_prod,
+            fd_unmet=fd_unmet,
+            limiting_stocks=limiting_stocks,
+            n_temporal_units_to_sim=sim.n_temporal_units_to_sim,
+            n_temporal_units_by_step=sim.model.n_temporal_units_by_step,
+            events=sim.all_events,
+            results_storage=results_storage,
+            psi_param=psi,
+            inventory_restoration_tau=inventory_restoration_tau,
+            stocks=stocks,
+            stocks_treatment=stocks_treatment,
+            include_crash=include_crash,
+        )
+
+    @classmethod
+    def from_folder(
+        cls,
+        folder: Union[str, pathlib.Path],
+        include_crash: bool = False,
+    ) -> Indicators:
+        if not isinstance(folder, pathlib.Path):
+            folder = pathlib.Path(folder)
+            if not folder.exists():
+                raise FileNotFoundError(str("Directory does not exist:" + str(folder)))
+
+        with (folder / "jsons" / "indexes.json").open() as f:
+            indexes = json.load(f)
+
+        params_folder = folder / "jsons"
+        records_folder = folder / "records"
+        params_file = {f.stem: f for f in params_folder.glob("*.json")}
+        absentee = [f for f in cls.params_list if f not in params_file.keys()]
+        if absentee:
+            raise FileNotFoundError(
+                "Some of the required parameters files not found (looked for {} in {}".format(
+                    cls.params_list, folder
+                )
+            )
+
+        record_files = [f for f in records_folder.glob("*") if f.is_file()]
+        absentee = [
+            f
+            for f in cls.record_files_list
+            if f not in [fn.name for fn in record_files]
+        ]
+        if absentee:
+            raise FileNotFoundError(
+                "Some of the required records are not there : {}".format(absentee)
+            )
+
+        with params_file["simulated_params"].open("r") as f:
+            params = json.load(f)
+
+        with params_file["simulated_events"].open("r") as f:
+            events = json.load(f)
+
+        if "has_crashed" in params:
+            has_crashed = params["has_crashed"]
         else:
-            value = np.array(value)
-            if value.shape != self.y_shape:
-                raise ValueError("Incorrect shape give for rebuilding_demand_house: {} given and {} expected".format(value.shape, self.y_shape))
-            self._rebuilding_demand_house = value
-
-    @property
-    def rebuilding_demand_indus(self)->Optional[np.ndarray]:
-        """The optional array of rebuilding demand from industries (to rebuild their kapital)"""
-        return self._rebuilding_demand_indus
-
-    @rebuilding_demand_indus.setter
-    def rebuilding_demand_indus(self,value:ArrayLike|None):
-        if value is None:
-            self._rebuilding_demand_indus = value
+            has_crashed = False
+
+        results_storage = folder.absolute()
+        records_path = records_folder.absolute()
+        n_temporal_units_to_sim = params["n_temporal_units_to_sim"]
+        t = n_temporal_units_to_sim
+        n_temporal_units_by_step = params["n_temporal_units_by_step"]
+        regions = indexes["regions"]
+        sectors = indexes["sectors"]
+        psi = params.get("psi_param")
+        inventory_restoration_tau = params.get("inventory_restoration_tau")
+        prod = np.memmap(
+            records_path / "production_realised",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        productive_capital = np.memmap(
+            records_path / "productive_capital_to_recover",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        prodmax = np.memmap(
+            records_path / "production_capacity",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        overprod = np.memmap(
+            records_path / "overproduction",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        final_demand = np.memmap(
+            records_path / "final_demand",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        io_demand = np.memmap(
+            records_path / "intermediate_demand",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        r_demand = np.memmap(
+            records_path / "rebuild_demand",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        r_prod = np.memmap(
+            records_path / "rebuild_prod",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_industries"]),
+        )
+        fd_unmet = np.memmap(
+            records_path / "final_demand_unmet",
+            mode="r+",
+            dtype="float64",
+            shape=(t, indexes["n_regions"] * indexes["n_sectors"]),
+        )
+        limiting_stocks = np.memmap(
+            records_path / "limiting_inputs",
+            mode="r+",
+            dtype="byte",
+            shape=(t * indexes["n_sectors"], indexes["n_industries"]),
+        )
+        if params.get("register_stocks", False):
+            if not (records_path / "inputs_stocks").exists():
+                raise FileNotFoundError(
+                    "Stocks record file was not found {}".format(
+                        records_path / "stocks_record"
+                    )
+                )
+            stocks = np.memmap(
+                records_path / "stocks_record",
+                mode="r+",
+                dtype="float64",
+                shape=(t * indexes["n_sectors"], indexes["n_industries"]),
+            )
+            stocks_treatment = True
         else:
-            value = np.array(value)
-            if value.shape != self.z_shape:
-                raise ValueError("Incorrect shape give for rebuilding_demand_indus: {} given and {} expected".format(value.shape, self.z_shape))
-            self._rebuilding_demand_indus = value
-            # Also update kapital destroyed
-            self._regional_sectoral_kapital_destroyed = value.sum(axis=0)
-
-    @property
-    def recoverable(self)->Optional[bool]:
-        """A boolean stating if an event can start recover"""
-        return self._recoverable
-
-    @recoverable.setter
-    def recoverable(self,current_temporal_unit:int):
-        if self._recoverable_kind:
-            reb = (self.occurrence + self.duration) <= current_temporal_unit
-            if reb and not self.recoverable :
-                logger.info("Temporal_Unit : {} ~ Event named {} that occured at {} in {} for {} damages has started recovering (no rebuilding demand)".format(current_temporal_unit,self.name,self.occurrence, self._aff_regions, self.total_kapital_destroyed))
-            self._recoverable = reb
-
-    @property
-    def rebuildable(self)->Optional[bool]:
-        """A boolean stating if an event can start rebuild"""
-        return self._rebuildable
-
-    @rebuildable.setter
-    def rebuildable(self,current_temporal_unit:int):
-        if self._rebuildable_kind:
-            reb = (self.occurrence + self.duration) <= current_temporal_unit
-            if reb and not self.rebuildable :
-                logger.info("Temporal_Unit : {} ~ Event named {} that occured at {} in {} for {} damages has started rebuilding".format(current_temporal_unit,self.name,self.occurrence, self._aff_regions, self.total_kapital_destroyed))
-            self._rebuildable = reb
-
-    @property
-    def prod_cap_delta_arbitrary(self)->Optional[np.ndarray]:
-        """The optional array storing arbitrary (as in not related to kapital destroyed) production capacity loss"""
-        return self._prod_cap_delta_arbitrary
-
-    @prod_cap_delta_arbitrary.setter
-    def prod_cap_delta_arbitrary(self, value:dict[str,float]|None):
-        if value is None:
-            self._prod_cap_delta_arbitrary = None
+            stocks = None
+            stocks_treatment = False
+
+        return cls(
+            has_crashed=has_crashed,
+            params=params,
+            regions=regions,
+            sectors=sectors,
+            productive_capital=productive_capital,
+            prod=prod,
+            prodmax=prodmax,
+            overprod=overprod,
+            final_demand=final_demand,
+            io_demand=io_demand,
+            r_demand=r_demand,
+            r_prod=r_prod,
+            fd_unmet=fd_unmet,
+            limiting_stocks=limiting_stocks,
+            n_temporal_units_to_sim=n_temporal_units_to_sim,
+            n_temporal_units_by_step=n_temporal_units_by_step,
+            events=events,
+            results_storage=results_storage,
+            psi_param=psi,
+            inventory_restoration_tau=inventory_restoration_tau,
+            stocks=stocks,
+            stocks_treatment=stocks_treatment,
+            include_crash=include_crash,
+        )
+
+    def calc_top_failing_sect(self):
+        pass
+
+    def calc_tot_fd_unmet(self):
+        self.indicators["tot_fd_unmet"] = self.treated_loss_df["fdloss"].sum()
+
+    def calc_aff_fd_unmet(self):
+        # TODO: check this
+        self.indicators["aff_fd_unmet"] = self.treated_loss_df[
+            self.treated_loss_df.region.isin(self.aff_regions)
+        ]["fdloss"].sum()
+
+    def calc_rebuild_durations(self):
+        rebuilding = (
+            self.rebuild_demand_df.reset_index()
+            .melt(
+                id_vars="step",
+                var_name=["region", "sector"],
+                value_name="rebuild_demand",
+            )
+            .groupby("step")
+            .sum(numeric_only=True)
+            .ne(0)
+            .rebuild_demand.to_numpy()
+        )
+        self.indicators["rebuild_durations"] = [
+            sum(1 for _ in group) for key, group in itertools.groupby(rebuilding) if key
+        ]
+
+    def calc_recovery_duration(self):
+        pass
+
+    def calc_general_shortage(self):
+        # TODO: replace hard values by soft.
+        n_regions = self.limiting_inputs_df.columns.levels[0].size
+        n_sectors = self.limiting_inputs_df.columns.levels[1].size
+        # have only steps in index (next step not possible with multiindex)
+        a = self.limiting_inputs_df.unstack()
+        # select only simulated steps (we can't store nan in bool or byte dtype array)
+        a = a.iloc[lambda x: x.index % self.n_temporal_units_by_step == 0]
+        # We put -1 initially, so this should check we have correctly selected the simulated rows
+        assert (a >= 0).all().all()
+        # put input stocks as columns and the rest as index
+        a = a.stack().T.stack(level=0)
+        # sum for all input and divide by n_sector to get "input shortage fraction"
+        # by industry
+        b = a.sum(axis=1).groupby(["step", "region", "sector"]).sum() / n_sectors
+        # by sector
+        c = b.groupby(["step", "region"]).sum() / n_sectors
+        # by region
+        c = c.groupby("step").sum() / n_regions
+        if not c.ne(0).any():
+            self.indicators["shortage_b"] = False
         else:
-            if self.aff_regions is None:
-                raise AttributeError("Affected regions attribute isn't set yet")
-            aff_sectors = np.array(list(value.keys()))
-            aff_shares = np.array(list(value.values()))
-            impossible_sectors = np.setdiff1d(aff_sectors,self.possible_sectors)
-            if impossible_sectors.size > 0 :
-                raise ValueError("These sectors are not in the model : {}".format(impossible_sectors))
-            self._aff_sectors = aff_sectors
-            self._aff_sectors_idx = np.searchsorted(self.possible_sectors, aff_sectors)
-            aff_industries_idx = np.array([self.possible_sectors.size * ri + si for ri in self.regions_idx for si in self._aff_sectors_idx])
-            self._prod_cap_delta_arbitrary = np.zeros(shape=self.possible_sectors.size)
-            self._prod_cap_delta_arbitrary[aff_industries_idx] = np.tile(aff_shares,self._aff_regions.size)
-
-    def init_shock(self, event:dict):
-        """Initiate shock from the event. Methods called by __init__.
-
-        Sets the rebuilding demand for households and industry.
-
-        First, if multiple regions are affected, it computes the vector of how damages are distributed across these.
-        Then it computes the vector of how regional damages are distributed across affected sectors.
-        It produces a ``n_regions`` * ``n_sectors`` sized vector hence stores the damage (i.e. capital destroyed) for all industries.
-
-        This method also computes the `rebuilding demand` matrices from households and industries, i.e. the demand addressed to the rebuilding
-        industries consequent to the shock.
-
-        See :ref:`How to define Events <boario-events>` for further detail on how to parameter these distribution.
-
-        Parameters
-        ----------
-        event : dict
-            A dictionary holding the relevant information to describe the event.
-
-        Raises
-        ------
-        ValueError
-            Raised if the production share allocated to rebuilding (in either
-            the impacted regions or the others) is not in [0,1].
-        """
-
-        if self.shock_type in {"kapital_destroyed_rebuild","kapital_destroyed_recover"}:
-            if self.total_kapital_destroyed is None:
-                raise AttributeError("Total kapital destroyed isn't set yet, this shouldn't happen.")
-            regions_idx = np.arange(self.possible_regions.size)
-            aff_industries_idx = np.array([self.possible_sectors.size * ri + si for ri in self._aff_regions_idx for si in self._aff_sectors_idx])
-            if not isinstance(self.total_kapital_destroyed, (int,float)):
-                raise ValueError("Kapital damages is {}, which is not valid".format(type(self.total_kapital_destroyed)))
-            self.total_kapital_destroyed /= self.monetary_unit
-            self.remaining_kapital_destroyed = self.total_kapital_destroyed
-            regional_damages = np.array(self.dmg_regional_distrib) * self.total_kapital_destroyed
-            # GDP CASE
-            if self.dmg_sectoral_distrib_type == "gdp":
-                shares = self.sectors_gva_shares.reshape((self.possible_regions.size,self.possible_sectors.size))
-                self.dmg_sectoral_distrib = (shares[self._aff_regions_idx][:,self._aff_sectors_idx]/shares[self._aff_regions_idx][:,self._aff_sectors_idx].sum(axis=1)[:,np.newaxis])
-
-            regional_sectoral_damages = regional_damages * self.dmg_sectoral_distrib
-            tmp = np.zeros(self.x_shape,dtype="float")
-            tmp[aff_industries_idx] = regional_sectoral_damages
-            self._regional_sectoral_kapital_destroyed_0 = tmp.copy()
-            self.regional_sectoral_kapital_destroyed = tmp.copy()
-            if self._regional_sectoral_kapital_destroyed is None:
-                    raise ValueError("Rebuilding sectors are not set for this event")
-            if self.shock_type == "kapital_destroyed_rebuild":
-                self._rebuildable_kind = True
-            # REBUILDING
-                if self._rebuilding_sectors_idx is None:
-                    raise ValueError("Rebuilding sectors are not set for this event")
-                rebuilding_industries_idx = np.array([self.possible_sectors.size * ri + si for ri in self._aff_regions_idx for si in self._rebuilding_sectors_idx])
-                rebuilding_industries_RoW_idx = np.array([self.possible_sectors.size * ri + si for ri in regions_idx if ri not in self._aff_regions_idx for si in self._rebuilding_sectors_idx])
-                rebuilding_demand = np.outer(self._rebuilding_sectors_shares,regional_sectoral_damages)
-                tmp = np.zeros(self.z_shape,dtype="float")
-                mask = np.ix_(np.union1d(rebuilding_industries_RoW_idx,rebuilding_industries_idx),aff_industries_idx)
-
-                tmp[mask] = self.Z_distrib[mask] * np.tile(rebuilding_demand, (self.possible_regions.size,1))
-                self.rebuilding_demand_indus = tmp
-                self.rebuilding_demand_house = np.zeros(shape=self.y_shape)
-            else:
-                self._rebuildable_kind = False
-                self._recoverable_kind = True
-                self.recovery_time = event.get("recovery_time")
-                self.recovery_function = event.get("recovery_function")
-
-        elif self.shock_type == "production_capacity_loss":
-            self.prod_cap_delta = event["prod_cap_delta"]
-
-    def recovery(self,current_temporal_unit:int):
-        if not self._recoverable_kind or self._rebuildable_kind:
-            raise AttributeError("Event is not initiated as a recoverable event")
-        elapsed = current_temporal_unit - (self.occurrence + self.duration)
-        if elapsed < 0:
-            raise RuntimeError("Trying to recover before event is over")
-        if self.recovery_function is None:
-            raise RuntimeError("Trying to recover event while recovery function isn't set yet")
-        res = self.recovery_function(elapsed_temporal_unit=elapsed)
-        precision = int(math.log10(self.monetary_unit)) + 1
-        res = np.around(res,precision)
-        if not np.any(res):
-            self.over = True
-        self.regional_sectoral_kapital_destroyed = res
-
-    def __repr__(self):
-        #TODO: find ways to represent long lists
-        return f''' [Representation WIP]
-        Event(
-              name = {self.name},
-              occur = {self.occurrence},
-              duration = {self.duration}
-              aff_regions = {self.aff_regions},
-              aff_sectors = {self.aff_sectors},
-             )
-        '''
+            self.indicators["shortage_b"] = True
+            shortage_date_start = c.ne(0.0).idxmax()
+            self.indicators["shortage_date_start"] = shortage_date_start
+            shortage_date_end = c.loc[shortage_date_start:].eq(0).idxmax()
+            self.indicators["shortage_date_end"] = shortage_date_end
+            self.indicators["shortage_date_max"] = c.idxmax()
+            self.indicators["shortage_ind_max"] = c.max()
+            self.indicators["shortage_ind_mean"] = c.loc[
+                shortage_date_start:shortage_date_end
+            ].mean()
+
+    def calc_first_shortages(self):
+        a = self.limiting_inputs_df.stack([0, 1])  # type: ignore
+        a = a.swaplevel(1, 2).swaplevel(2, 3)
+        b = a[a > 0]
+        b = b[:10]
+        res = list(b.index)  # type:ignore
+        self.indicators["10_first_shortages_(step,region,sector,stock_of)"] = res
+
+    def calc_tot_prod_change(self):
+        df2 = self.production_realised_df.copy()
+        # df2.columns=df2.columns.droplevel(0)
+        prod_chg = df2 - df2.iloc[0, :]
+        # Round to € to avoid floating error differences
+        prod_chg = prod_chg.round(6)
+        # Aggregate rebuilding and non-rebuilding sectors
+        prod_chg_agg_1 = pd.concat(
+            [
+                prod_chg.loc[:, pd.IndexSlice[:, self.rebuilding_sectors]]
+                .groupby("region", axis=1)
+                .sum(),
+                prod_chg.loc[
+                    prod_chg.index.difference(
+                        prod_chg.loc[
+                            :, pd.IndexSlice[:, self.rebuilding_sectors]
+                        ].columns
+                    )
+                ]
+                .groupby("region", axis=1)
+                .sum(),
+            ],
+            keys=["rebuilding", "non-rebuilding"],
+            names=["sectors affected"],
+            axis=1,
+        )
+
+        n_semesters = self.n_rows // (self.params["year_to_temporal_unit_factor"] // 2)
+        row_to_semester = self.params["year_to_temporal_unit_factor"] // 2
+        modulo = self.params["year_to_temporal_unit_factor"] % 2
+        logger.info(
+            "There are {} semesters [{} rows, each representing a {}th of a year]".format(
+                n_semesters, self.n_rows, self.params["year_to_temporal_unit_factor"]
+            )
+        )
+        prod_chg_sect_sem_l = []
+        for sem in range(0, n_semesters):
+            prod_chg_sect_sem_l.append(
+                prod_chg_agg_1.iloc[
+                    sem * row_to_semester : ((sem + 1) * row_to_semester)
+                    + (sem % 2) * modulo
+                ]
+                .sum()
+                .T
+            )
+
+        prod_chg_region = pd.concat(
+            prod_chg_sect_sem_l,
+            keys=["semester {}".format(v + 1) for v in range(n_semesters)],
+            names=["semester"],
+        )
+        aff_regions = "~".join(self.aff_regions)
+        self.prod_chg_region = pd.DataFrame({aff_regions: prod_chg_region}).T
+        prod_chg_sect = prod_chg.sum()
+        tmp = prod_chg_sect.sort_values(ascending=False, key=abs).head(5).to_dict()
+        self.indicators["top_5_sector_chg"] = {str(k): v for k, v in tmp.items()}
+
+        self.indicators["prod_gain_tot"] = prod_chg.mul(prod_chg.gt(0)).sum().sum()
+        self.indicators["prod_lost_tot"] = prod_chg.mul(~prod_chg.gt(0)).sum().sum() * (
+            -1
+        )
+        prod_chg = prod_chg.drop(self.aff_regions, axis=1)
+        self.indicators["prod_gain_unaff"] = prod_chg.mul(prod_chg.gt(0)).sum().sum()
+        self.indicators["prod_lost_unaff"] = prod_chg.mul(
+            ~prod_chg.gt(0)
+        ).sum().sum() * (-1)
+
+    def update_indicators(self):
+        logger.info("(Re)computing all indicators")
+        logger.info("Tot fd unmet")
+        self.calc_tot_fd_unmet()
+        logger.info("aff fd unmet")
+        self.calc_aff_fd_unmet()
+        logger.info("rebuild durations")
+        self.calc_rebuild_durations()
+        logger.info("recovery duration")
+        self.calc_recovery_duration()
+        logger.info("general shortage")
+        self.calc_general_shortage()
+        logger.info("tot prod change")
+        self.calc_tot_prod_change()
+        logger.info("fd loss region")
+        self.calc_fd_loss_region()
+        logger.info("first shortages")
+        self.calc_first_shortages()
+
+    def write_indicators(self, storage_path=None):
+        if storage_path is None and not hasattr(self, "storage_path"):
+            raise ValueError(
+                f"You are attempting to save indicators but no storage path was specified either in the Indicators class or to this method."
+            )
+        storage_path = self.storage_path if storage_path is None else storage_path
+        storage_path = pathlib.Path(storage_path).resolve()
+        logger.info("Writing indicators to json")
+        if hasattr(self, "prod_chg_region"):
+            self.prod_chg_region.to_json(
+                storage_path / "prod_chg.json", indent=4, orient="split"
+            )
+        if hasattr(self, "fd_loss_region"):
+            self.fd_loss_region.to_json(
+                storage_path / "fd_loss.json", indent=4, orient="split"
+            )
+        with (storage_path / "indicators.json").open("w") as f:
+            json.dump(self.indicators, f, cls=numpyencoder.NumpyEncoder, indent=4)
+
+    def calc_fd_loss_region(self):
+        fd_loss = self.final_demand_unmet_df.copy().round(6)
+        fd_loss_agg_1 = pd.concat(
+            [
+                fd_loss.loc[:, pd.IndexSlice[:, self.rebuilding_sectors]]
+                .groupby("region", axis=1)
+                .sum(),
+                fd_loss.loc[
+                    fd_loss.index.difference(
+                        fd_loss.loc[
+                            :, pd.IndexSlice[:, self.rebuilding_sectors]
+                        ].columns
+                    )
+                ]
+                .groupby("region", axis=1)
+                .sum(),
+            ],
+            keys=["rebuilding", "non-rebuilding"],
+            names=["sectors affected"],
+            axis=1,
+        )
+
+        n_semesters = self.n_rows // (self.params["year_to_temporal_unit_factor"] // 2)
+        row_to_semester = self.params["year_to_temporal_unit_factor"] // 2
+        modulo = self.params["year_to_temporal_unit_factor"] % 2
+        logger.info(
+            "There are {} semesters [{} rows, each representing a {}th of a year]".format(
+                n_semesters, self.n_rows, self.params["year_to_temporal_unit_factor"]
+            )
+        )
+        fd_loss_sect_sem_l = []
+        for sem in range(0, n_semesters):
+            fd_loss_sect_sem_l.append(
+                fd_loss_agg_1.iloc[
+                    sem * row_to_semester : ((sem + 1) * row_to_semester)
+                    + (sem % 2) * modulo
+                ]
+                .sum()
+                .T
+            )
+
+        fd_loss_region = pd.concat(
+            fd_loss_sect_sem_l,
+            keys=["semester {}".format(v + 1) for v in range(n_semesters)],
+            names=["semester"],
+        )
+        aff_regions = "~".join(self.aff_regions)
+        self.fd_loss_region = pd.DataFrame({aff_regions: fd_loss_region}).T
+        fd_loss_sect = fd_loss.sum()
+        tmp = fd_loss_sect.sort_values(ascending=False, key=abs).head(5).to_dict()
+        self.indicators["top_5_sector_fdloss"] = {str(k): v for k, v in tmp.items()}
+
+    def save_dfs(self):
+        logger.info("Saving computed dataframe to results folder")
+        self.production_realised_df.to_parquet(
+            self.parquets_path / "production_realised_df.parquet"
+        )
+        self.productive_capital_to_recover_df.to_parquet(
+            self.parquets_path / "productive_capital_to_recover_df.parquet"
+        )
+        self.production_capacity_df.to_parquet(
+            self.parquets_path / "production_capacity_df.parquet"
+        )
+        self.overproduction_df.to_parquet(
+            self.parquets_path / "overproduction_df.parquet"
+        )
+        self.final_demand_unmet_df.to_parquet(
+            self.parquets_path / "final_demand_unmet_df.parquet"
+        )
+        self.final_demand_df.to_parquet(self.parquets_path / "final_demand_df.parquet")
+        self.intermediate_demand_df.to_parquet(
+            self.parquets_path / "intermediate_demand_df.parquet"
+        )
+        self.rebuild_demand_df.to_parquet(
+            self.parquets_path / "rebuild_demand_df.parquet"
+        )
+        self.treated_loss_df.to_parquet(self.parquets_path / "treated_df_loss.parquet")
+        if self.inputs_stocks_df is not None:
+            ddf = da.from_pandas(self.inputs_stocks_df, chunksize=10000000)
+            ddf.to_parquet(
+                self.parquets_path / "treated_df_stocks.parquet", engine="pyarrow"
+            )
+        if self.limiting_inputs_df is not None:
+            # ddf_l = da.from_pandas(self.df_limiting, chunksize=10000000)
+            # ddf_l = ddf_l.melt(ignore_index=False).rename(columns={'variable_0':'region','variable_1':'sector', 'variable_2':'stock of'})
+            # ddf_l = ddf_l.reset_index()
+            # ddf_l['step'] = ddf_l['step'].astype("uint16")
+            # ddf_l['stock of'] = ddf_l['stock of'].astype("category")
+            # ddf_l['region'] = ddf_l['region'].astype("category")
+            # ddf_l['sector'] = ddf_l['sector'].astype("category")
+            self.limiting_inputs_df.to_parquet(
+                self.parquets_path / "treated_df_limiting_inputs.parquet",
+                engine="pyarrow",
+            )
+        # self.df_limiting.to_feather(self.parquets_path/"treated_df_limiting.feather")
```

### Comparing `boario-0.4.1b0/boario/model_base.py` & `boario-0.5.0a0/boario/model_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,592 +16,926 @@
 
 from __future__ import annotations
 import json
 import pathlib
 import typing
 from typing import Optional
 import numpy as np
-from numpy.typing import ArrayLike
+import numpy.typing as npt
+import pandas as pd
+from pymrio.core.mriosystem import IOSystem
 
 from boario import logger, warn_once
-from boario.event import Event
-from pymrio.core.mriosystem import IOSystem
+from boario.event import (
+    Event,
+    EventKapitalDestroyed,
+    EventKapitalRebuild,
+    EventArbitraryProd,
+)
 from boario.utils.misc import lexico_reindex
 
 
-__all__ = ["ARIOBaseModel","INV_THRESHOLD","VALUE_ADDED_NAMES","VA_idx", "lexico_reindex"]
-
-INV_THRESHOLD = 0 #20 #temporal_units
-
-VALUE_ADDED_NAMES = ['VA', 'Value Added', 'value added',
-                        'factor inputs', 'factor_inputs', 'Factors Inputs',
-                        'Satellite Accounts', 'satellite accounts', 'satellite_accounts',
-                     'satellite']
-
-VA_idx = np.array(['Taxes less subsidies on products purchased: Total',
-       'Other net taxes on production',
-       "Compensation of employees; wages, salaries, & employers' social contributions: Low-skilled",
-       "Compensation of employees; wages, salaries, & employers' social contributions: Medium-skilled",
-       "Compensation of employees; wages, salaries, & employers' social contributions: High-skilled",
-       'Operating surplus: Consumption of fixed capital',
-       'Operating surplus: Rents on land',
-       'Operating surplus: Royalties on resources',
-       'Operating surplus: Remaining net operating surplus'], dtype=object)
+__all__ = [
+    "ARIOBaseModel",
+    "INV_THRESHOLD",
+    "VALUE_ADDED_NAMES",
+    "VA_idx",
+    "lexico_reindex",
+]
+
+INV_THRESHOLD = 0  # 20 #temporal_units
+
+TECHNOLOGY_THRESHOLD = (
+    0.00001  # Do not care about input if producing requires less than this value
+)
+
+VALUE_ADDED_NAMES = [
+    "VA",
+    "Value Added",
+    "value added",
+    "factor inputs",
+    "factor_inputs",
+    "Factors Inputs",
+    "Satellite Accounts",
+    "satellite accounts",
+    "satellite_accounts",
+    "satellite",
+]
+
+VA_idx = np.array(
+    [
+        "Taxes less subsidies on products purchased: Total",
+        "Other net taxes on production",
+        "Compensation of employees; wages, salaries, & employers' social contributions: Low-skilled",
+        "Compensation of employees; wages, salaries, & employers' social contributions: Medium-skilled",
+        "Compensation of employees; wages, salaries, & employers' social contributions: High-skilled",
+        "Operating surplus: Consumption of fixed capital",
+        "Operating surplus: Rents on land",
+        "Operating surplus: Royalties on resources",
+        "Operating surplus: Remaining net operating surplus",
+    ],
+    dtype=object,
+)
+
+
+class ARIOBaseModel:
+    def __init__(
+        self,
+        pym_mrio: IOSystem,
+        *,
+        order_type: str = "alt",
+        alpha_base: float = 1.0,
+        alpha_max: float = 1.25,
+        alpha_tau: int = 365,
+        rebuild_tau: int = 60,
+        main_inv_dur: int = 90,
+        monetary_factor: int = 10**6,
+        temporal_units_by_step: int = 1,
+        iotable_year_to_temporal_unit_factor: int = 365,
+        infinite_inventories_sect: Optional[list] = None,
+        inventory_dict: Optional[dict] = None,
+        productive_capital_vector: Optional[
+            pd.Series | npt.NDArray | pd.DataFrame
+        ] = None,
+        productive_capital_to_VA_dict: Optional[dict] = None,
+    ) -> None:
+        r"""The core of an ARIO model.  Handles the different arrays containing the mrio tables.
+
+        `ARIOBaseModel` wrap all the data and functions used in the core of the most basic version of the ARIO
+        model (based on :cite:`2013:hallegatte` and :cite:`2020:guan`).
+
+        An ARIOBaseModel instance based is build on the given IOSystem.
+        Most default parameters are the same as in :cite:`2013:hallegatte` and
+        default order mechanisms comes from :cite:`2020:guan`. By default each
+        industry capital stock is 4 times its value added (:cite:`2008:hallegatte`).
 
-class ARIOBaseModel(object):
-    r"""The core of an ARIO3 model.  Handles the different arrays containing the mrio tables.
-
-    A ARIOBaseModel wrap all the data and functions used in the core of the most basic version of the ARIO
-    model (based on Hallegatte2013 and Guan2020).
+        Parameters
+        ----------
+        pym_mrio : IOSystem
+            The IOSystem to base the model on.
+        order_type : str, default "alt"
+            The type of orders mechanism to use. Currently, can be "alt" or
+            "noalt". See :ref:`boario-math`
+        alpha_base : float, default 1.0
+            Base value of overproduction factor :math:`\alpha^{b}` (Default to 1.0).
+        alpha_max : float, default 1.25
+            Maximum factor of overproduction :math:`\alpha^{\textrm{max}}` (default should be 1.25).
+        alpha_tau : int, default 365
+            Characteristic time of overproduction :math:`\tau_{\alpha}` in ``n_temporal_units_by_step`` (default should be 365 days).
+        rebuild_tau : int, default 60
+            Rebuilding characteristic time :math:`\tau_{\textrm{REBUILD}}` (see :ref:`boario-math`). Overwritten by per event value if it exists.
+        main_inv_dur : int, default 90
+            The default numbers of days for inputs inventory to use if it is not defined for an input.
+        monetary_factor : int, default 10**6
+            Monetary unit factor (i.e. if the tables unit is 10^6 € instead of 1 €, it should be set to 10^6).
+        temporal_units_by_step: int, default 1
+            The number of temporal_units between each step. (Current version of the model showed inconsistencies with values other than `1`).
+        iotable_year_to_temporal_unit_factor : int, default 365
+            The (inverse of the) factor by which MRIO data should be multiplied in order to get "per temporal unit value", assuming IO data is yearly.
+        infinite_inventories_sect: list, optional
+            List of inputs (sector) considered never constraining for production.
+        inventory_dict: dict, optional
+            Dictionary in the form input:initial_inventory_size, (where input is a sector, and initial_inventory_size is in "temporal_unit" (defaults to a day))
+        productive_capital_vector: ArrayLike, optional
+            Array of capital per industry if you need to give it exogenously.
+        productive_capital_to_VA_dict: dict, optional
+            Dictionary in the form sector:ratio. Where ratio is used to estimate capital stock based on the value added of the sector.
 
-    Attributes
-    ----------
+        Notes
+        -----
 
-    results_storage : pathlib.Path
-                      The path where the results of the simulation are stored.
-    regions : numpy.ndarray of str
-              An array of the regions of the model.
-    n_regions : int
-                The number :math:`m` of regions.
-    sectors : numpy.ndarray of str
-              An array of the sectors of the model.
-    n_sectors : int
-                The number :math:`n` of sectors.
-    fd_cat : numpy.ndarray of str
-             An array of the final demand categories of the model (``["Final demand"]`` if there is only one)
-    n_fd_cat : int
-               The numbers of final demand categories.
-    monetary_unit : int
-                    monetary unit prefix (i.e. if the tables unit is 10^6 € instead of 1 €, it should be set to 10^6).
-    temporal_units_by_step : int
-                     The number of temporal_units between each step. (Current version of the model was not tested with values other than `1`).
-    year_to_temporal_unit_factor : int
-                               Kinda deprecated, should be equal to `temporal_units_by_step`.
-    rebuild_tau : int
-                  Rebuilding characteristic time :math:`\tau_{\textrm{REBUILD}}` (see :ref:`boario-math`).
-    overprod_max : float
-                   Maximum factor of overproduction :math:`\alpha^{\textrm{max}}` (default should be 1.25).
-    overprod_tau : float
-                   Characteristic time of overproduction :math:`\tau_{\alpha}` in ``temporal_units_by_step`` (default should be 365 days).
-    overprod_base : float
-                    Base value of overproduction factor :math:`\alpha^{b}` (Default to 1.0).
-    inv_duration : numpy.ndarray of int
-                   Array :math:`\mathbf{s}` of size :math:`n` (sectors), setting for each input the initial number of ``temporal_units_by_step`` of stock for the input. (see :ref:`boario-math`).
-    restoration_tau : numpy.ndarray of int
-                      Array of size :math:`n` setting for each inputs its characteristic restoration time :math:`\tau_{\textrm{INV}}` in ``temporal_units_by_step``. (see :ref:`boario-math`).
-    Z_0 : numpy.ndarray of float
-          2-dim square matrix array :math:`\ioz` of size :math:`(n \times m, n \times m)` representing the intermediate (transaction) matrix (see :ref:`boario-math-init`).
-    Z_C : numpy.ndarray of float
-          2-dim matrix array :math:`\ioz^{\sectorsset}` of size :math:`(n, n \times m)` representing the intermediate (transaction) matrix aggregated by inputs (see :ref:`here <boario-math-z-agg>`).
-    Z_distrib : numpy.ndarray of float
-                :math:`\ioz` normalised by :math:`\ioz^{\sectorsset}`, i.e. representing for each input the share of the total ordered transiting from an industry to another (see :ref:`here <boario-math-z-agg>`).
-    Y_0 : numpy.ndarray of float
-          2-dim array :math:`\ioy` of size :math:`(n \times m, m \times \text{number of final demand categories})` representing the final demand matrix.
-    X_0 : numpy.ndarray of float
-          Array :math:`\iox(0)` of size :math:`n \times m` representing the initial gross production.
-    gdp_df : pandas.DataFrame
-             Dataframe of the total GDP of each region of the model
-    VA_0 : numpy.ndarray of float
-           Array :math:`\iov` of size :math:`n \times m` representing the total value added for each sectors.
-    tech_mat : numpy.ndarray
-               2-dim array :math:`\ioa` of size :math:`(n \times m, n \times m)` representing the technical coefficients matrix
-    overprod : numpy.ndarray
-               Array of size :math:`n \times m` representing the overproduction coefficients vector :math:`\mathbf{\alpha}(t)`.
-    Raises
-    ------
-    RuntimeError
-        A RuntimeError can occur when data is inconsistent (negative stocks for
-        instance)
-    ValueError
-    NotImplementedError
-    """
+        It is recommended to use ``productive_capital_to_VA_dict`` if you have a more precise estimation of
+        the ratio of (Capital Stock / Value Added) per sectors than the default 4/1 ratio.
+        You may also feed in directly a ``productive_capital_vector`` if you did your estimation before-hand.
+        (This is especially useful if you have events based of an exposure layer for instance)
+
+        Regarding inventories, they default to 90 days for all inputs (ie sectors).
+        You can set some inputs to be never constraining for production by listing them
+        in ``infinite_inventories_sect`` or directly feed in a dictionary of the inventory
+        duration for each input.
 
-    def __init__(self,
-                 pym_mrio: IOSystem,
-                 mrio_params: dict,
-                 simulation_params: dict,
-                 results_storage: pathlib.Path
-                 ) -> None:
+        """
 
         logger.debug("Initiating new ARIOBaseModel instance")
         super().__init__()
-
         ################ Parameters variables #######################
-        logger.info("IO system metadata :\n{}".format(str(pym_mrio.meta)))
-        logger.info("Simulation parameters:\n{}".format(json.dumps(simulation_params, indent=4)))
+        try:
+            logger.info(
+                "IO system metadata :\n{}\n{}\n{}\n{}".format(
+                    str(pym_mrio.meta.description),
+                    str(pym_mrio.meta.name),
+                    str(pym_mrio.meta.system),
+                    str(pym_mrio.meta.version),
+                )
+            )
+        except AttributeError:
+            logger.warning(
+                "It seems the MRIOT you loaded doesn't have metadata to print."
+            )
+
         pym_mrio = lexico_reindex(pym_mrio)
-        self.mrio_params : dict = mrio_params
-        self.main_inv_dur : int = mrio_params['main_inv_dur']
+        self.main_inv_dur: int = main_inv_dur
+        r"""int, default 90: The default numbers of days for inputs inventory to use if it is not defined for an input."""
 
-        results_storage = results_storage.absolute()
-        self.records_storage:pathlib.Path = results_storage/"records"
-        logger.info("Results storage is: {}".format(self.records_storage))
         reg = pym_mrio.get_regions()
-        reg = typing.cast("list[str]",reg)
+        reg = typing.cast("list[str]", reg)
         self.regions = np.array(sorted(reg))
+        r"""numpy.ndarray of str : An array of the regions of the model."""
+
         self.n_regions = len(reg)
+        r"""int : The number :math:`m` of regions."""
+
         sec = pym_mrio.get_sectors()
-        sec = typing.cast("list[str]",sec)
+        sec = typing.cast("list[str]", sec)
         self.sectors = np.array(sorted(sec))
+        r"""numpy.ndarray of str: An array of the sectors of the model."""
+
         self.n_sectors = len(sec)
+        r"""int : The number :math:`n` of sectors."""
+
+        self.industries = pd.MultiIndex.from_product(
+            [self.regions, self.sectors], names=["region", "sector"]
+        )
+        r"""pandas.MultiIndex : A pandas MultiIndex of the industries (region,sector) of the model."""
+
+        self.n_industries = len(self.industries)
+        r"""int : The number :math:`m * n` of industries."""
+
         try:
-            self.fd_cat = np.array(sorted(list(pym_mrio.get_Y_categories()))) #type: ignore
-            self.n_fd_cat = len(pym_mrio.get_Y_categories()) #type: ignore
+            self.final_demand_cat = np.array(sorted(list(pym_mrio.get_Y_categories())))  # type: ignore
+            r"""numpy.ndarray of str: An array of the final demand categories of the model (``["Final demand"]`` if there is only one)"""
+
+            self.n_fd_cat = len(pym_mrio.get_Y_categories())  # type: ignore
+            r"""int: The numbers of final demand categories."""
+
         except KeyError:
             self.n_fd_cat = 1
-            self.fd_cat = np.array(["Final demand"])
+            self.final_demand_cat = np.array(["Final demand"])
         except IndexError:
-            self.n_fd_cat= 1
-            self.fd_cat = np.array(["Final demand"])
-        self.monetary_unit = mrio_params['monetary_unit']
-        logger.info("Monetary unit from params is: %s", self.monetary_unit)
-        if pym_mrio.unit is None:
-            raise ValueError("Problem reading monetary unit from MRIO")
-        logger.info("Monetary unit from loaded mrio is: %s", pym_mrio.unit.unit.unique()[0])
-        #self.psi = simulation_params['psi_param']
-        self.n_temporal_units_by_step = simulation_params['temporal_units_by_step']
-        self.iotable_year_to_temporal_unit_factor = simulation_params['year_to_temporal_unit_factor'] # 365 for yearly IO tables
+            self.n_fd_cat = 1
+            self.final_demand_cat = np.array(["Final demand"])
+
+        if hasattr(pym_mrio, "monetary_factor"):
+            logger.warning(
+                f"Custom monetary factor found in the mrio pickle file, continuing with this one ({getattr(pym_mrio,'monetary_factor')})"
+            )
+            self.monetary_factor = getattr(pym_mrio, "monetary_factor")
+        else:
+            self.monetary_factor = monetary_factor
+        r"""int, default 10^6: Monetary unit factor (i.e. if the tables unit is 10^6 € instead of 1 €, it should be set to 10^6)."""
+
+        self.n_temporal_units_by_step = temporal_units_by_step
+        r"""int, default 1: The number of temporal_units between each step. (Current version of the model was not tested with values other than `1`)."""
+
+        self.iotable_year_to_temporal_unit_factor = iotable_year_to_temporal_unit_factor
+        r"""int, default 365: The (inverse of the) factor by which MRIO data should be multiplied in order to get "per temporal unit value", assuming IO data is yearly."""
+
         if self.iotable_year_to_temporal_unit_factor != 365:
-            logger.warning("iotable_to_daily_step_factor is not set to 365 (days). This should probably not be the case if the IO tables you use are on a yearly basis.")
-        self.steply_factor =  self.n_temporal_units_by_step / self.iotable_year_to_temporal_unit_factor
-        self.rebuild_tau = simulation_params['rebuild_tau']
-        self.overprod_max = simulation_params['alpha_max']
-        self.overprod_tau = self.n_temporal_units_by_step / simulation_params['alpha_tau']
-        self.overprod_base = simulation_params['alpha_base']
-        inv = mrio_params['inventories_dict']
-        inventories = [ np.inf if inv[k]=='inf' else inv[k] for k in sorted(inv.keys())]
-        self.inv_duration = np.array(inventories)  / self.n_temporal_units_by_step
-        if (self.inv_duration <= 1).any() :
-            logger.warning("At least one product has inventory duration lower than the numbers of temporal units in one step ({}), model will set it to 2 by default, but you should probably check this !".format(self.n_temporal_units_by_step))
+            logger.warning(
+                "iotable_to_daily_step_factor is not set to 365 (days). This should probably not be the case if the IO tables you use are on a yearly basis."
+            )
+
+        self.steply_factor = (
+            self.n_temporal_units_by_step / self.iotable_year_to_temporal_unit_factor
+        )
+        self.rebuild_tau = rebuild_tau
+        r"""int: Rebuilding characteristic time :math:`\tau_{\textrm{REBUILD}}` (see :ref:`boario-math`)."""
+
+        self.overprod_max = alpha_max
+        r"""float: Maximum factor of overproduction :math:`\alpha^{\textrm{max}}` (default should be 1.25)."""
+
+        self.overprod_tau = self.n_temporal_units_by_step / alpha_tau
+        r"""float: Characteristic time of overproduction :math:`\tau_{\alpha}` in ``n_temporal_units_by_step`` (default should be 365 days)."""
+
+        self.overprod_base = alpha_base
+        r"""float: Base value of overproduction factor :math:`\alpha^{b}` (Default to 1.0)."""
+
+        if inventory_dict is None:
+            infinite_inventories_sect = (
+                [] if infinite_inventories_sect is None else infinite_inventories_sect
+            )
+            self.inventories = [
+                np.inf if sector in infinite_inventories_sect else main_inv_dur
+                for sector in self.sectors
+            ]
+            r"""numpy.ndarray of int: Array :math:`\mathbf{s}` of size :math:`n` (sectors), setting for each input the initial number of ``n_temporal_units_by_step`` of stock for the input. (see :ref:`boario-math`)."""
+
+        else:
+            infinite_inventories_sect = (
+                [] if infinite_inventories_sect is None else infinite_inventories_sect
+            )
+            self.inventories = [
+                np.inf
+                if inventory_dict[k] in ["inf", "Inf", "Infinity", "infinity"]
+                or k in infinite_inventories_sect
+                else inventory_dict[k]
+                for k in sorted(inventory_dict.keys())
+            ]
+
+        logger.debug(f"inventories: {self.inventories}")
+        logger.debug(f"n_temporal_units_by_step: {self.n_temporal_units_by_step}")
+        self.inv_duration = np.array(self.inventories) / self.n_temporal_units_by_step
+
+        if (self.inv_duration <= 1).any():
+            logger.warning(
+                f"At least one product has inventory duration lower than the numbers of temporal units in one step ({self.n_temporal_units_by_step}), model will set it to 2 by default, but you should probably check this !"
+            )
             self.inv_duration[self.inv_duration <= 1] = 2
         #################################################################
 
-
         ######## INITIAL MRIO STATE (in step temporality) ###############
         if pym_mrio.Z is None:
-            raise ValueError("Z attribute of given MRIO doesn't exist, this is a problem")
+            raise ValueError(
+                "Z attribute of given MRIO doesn't exist, this is a problem"
+            )
         if pym_mrio.Y is None:
-            raise ValueError("Y attribute of given MRIO doesn't exist, this is a problem")
+            raise ValueError(
+                "Y attribute of given MRIO doesn't exist, this is a problem"
+            )
         if pym_mrio.x is None:
-            raise ValueError("x attribute of given MRIO doesn't exist, this is a problem")
+            raise ValueError(
+                "x attribute of given MRIO doesn't exist, this is a problem"
+            )
         self._matrix_id = np.eye(self.n_sectors)
         self._matrix_I_sum = np.tile(self._matrix_id, self.n_regions)
         self.Z_0 = pym_mrio.Z.to_numpy()
-        self.Z_C = (self._matrix_I_sum @ self.Z_0)
-        with np.errstate(divide='ignore',invalid='ignore'):
-            self.Z_distrib = (np.divide(self.Z_0,(np.tile(self.Z_C, (self.n_regions, 1)))))
+        r"""numpy.ndarray of float: 2-dim square matrix array :math:`\ioz` of size :math:`(n \times m, n \times m)` representing the daily intermediate (transaction) matrix (see :ref:`boario-math-init`)."""
+
+        self.Z_C = self._matrix_I_sum @ self.Z_0
+        r"""numpy.ndarray of float: 2-dim matrix array :math:`\ioz^{\sectorsset}` of size :math:`(n, n \times m)` representing the intermediate (transaction) matrix aggregated by inputs (see :ref:`here <boario-math-z-agg>`)."""
+
+        with np.errstate(divide="ignore", invalid="ignore"):
+            self.Z_distrib = np.divide(
+                self.Z_0, (np.tile(self.Z_C, (self.n_regions, 1)))
+            )
+            r"""numpy.ndarray of float: math:`\ioz` normalised by :math:`\ioz^{\sectorsset}`, i.e. representing for each input the share of the total ordered transiting from an industry to another (see :ref:`here <boario-math-z-agg>`)."""
+
         self.Z_distrib = np.nan_to_num(self.Z_distrib)
-        self.Z_0 = (pym_mrio.Z.to_numpy() * self.steply_factor)
-        self.Y_0 = (pym_mrio.Y.to_numpy() * self.steply_factor)
+        self.Z_0 = pym_mrio.Z.to_numpy() * self.steply_factor
+
+        self.Y_0 = pym_mrio.Y.to_numpy()
+        self.Y_C = self._matrix_I_sum @ self.Y_0
+        r"""numpy.ndarray of float: 2-dim matrix array :math:`\ioy^{\sectorsset}` of size :math:`(n, m \times \text{number of final demand categories})` representing the final demand matrix aggregated by inputs (see :ref:`here <boario-math-z-agg>`)."""
+
+        with np.errstate(divide="ignore", invalid="ignore"):
+            self.Y_distrib = np.divide(
+                self.Y_0, (np.tile(self.Y_C, (self.n_regions, 1)))
+            )
+            r"""numpy.ndarray of float: math:`\ioy` normalised by :math:`\ioy^{\sectorsset}`, i.e. representing for each input the share of the total ordered transiting from an industry to final demand (see :ref:`here <boario-math-z-agg>`)."""
+
+        self.Y_distrib = np.nan_to_num(self.Y_distrib)
+
+        self.Y_0 = pym_mrio.Y.to_numpy() * self.steply_factor
+        r"""numpy.ndarray of float: 2-dim array :math:`\ioy` of size :math:`(n \times m, m \times \text{number of final demand categories})` representing the daily final demand matrix."""
+
         tmp = np.array(pym_mrio.x.T)
-        self.X_0 = (tmp.flatten() * self.steply_factor)
+        self.X_0 = tmp.flatten() * self.steply_factor
+        r"""numpy.ndarray of float: Array :math:`\iox(0)` of size :math:`n \times m` representing the initial daily gross production."""
+
         del tmp
-        value_added = (pym_mrio.x.T - pym_mrio.Z.sum(axis=0))
+        value_added = pym_mrio.x.T - pym_mrio.Z.sum(axis=0)
         value_added = value_added.reindex(sorted(value_added.index), axis=0)
         value_added = value_added.reindex(sorted(value_added.columns), axis=1)
+        if (value_added < 0).any().any():
+            logger.warning(
+                f"""Found negative values in the value added, will set to 0. Note that sectors with null value added are not impacted by capital destruction.
+                industries with negative VA: {(value_added[value_added < 0].dropna(axis=1)).columns}
+                """
+            )
+
         value_added[value_added < 0] = 0.0
-        self.gdp_df = value_added.groupby('region',axis=1).sum()
-        self.VA_0 = (value_added.to_numpy().flatten())
-        self.tech_mat = ((self._matrix_I_sum @ pym_mrio.A).to_numpy()) #type: ignore #to_numpy is not superfluous !
-        kratio = mrio_params['capital_ratio_dict']
-        kratio_ordered = [kratio[k] for k in sorted(kratio.keys())]
-        self.kstock_ratio_to_VA = np.tile(np.array(kratio_ordered),self.n_regions)
+        self.gdp_df = value_added.groupby("region", axis=1).sum()
+        r"""pandas.DataFrame: Dataframe of the total GDP of each region of the model"""
+
+        self.VA_0 = value_added.to_numpy().flatten()
+        r"""numpy.ndarray of float: Array :math:`\iov` of size :math:`n \times m` representing the total value added for each sectors."""
+
+        self.tech_mat = (self._matrix_I_sum @ pym_mrio.A).to_numpy()  # type: ignore #to_numpy is not superfluous !
+        r"""numpy.ndarray of float: 2-dim array :math:`\ioa` of size :math:`(n \times m, n \times m)` representing the technical coefficients matrix."""
+
+        if productive_capital_vector is not None:
+            self.k_stock = productive_capital_vector
+            """numpy.ndarray of float: Array of size :math:`n \times m` representing the estimated stock of capital of each industry."""
+
+            if isinstance(self.k_stock, pd.DataFrame):
+                self.k_stock = self.k_stock.squeeze().sort_index().to_numpy()
+        elif productive_capital_to_VA_dict is None:
+            logger.warning(f"No capital to VA dictionary given, considering 4/1 ratio")
+            self.kstock_ratio_to_VA = 4
+            self.k_stock = self.VA_0 * self.kstock_ratio_to_VA
+        else:
+            kratio = productive_capital_to_VA_dict
+            kratio_ordered = [kratio[k] for k in sorted(kratio.keys())]
+            self.kstock_ratio_to_VA = np.tile(np.array(kratio_ordered), self.n_regions)
+            self.k_stock = self.VA_0 * self.kstock_ratio_to_VA
         if value_added.ndim > 1:
-            self.gdp_share_sector = (self.VA_0 / value_added.sum(axis=0).groupby('region').transform('sum').to_numpy())
+            self.gdp_share_sector = (
+                self.VA_0
+                / value_added.sum(axis=0).groupby("region").transform("sum").to_numpy()
+            )
         else:
-            self.gdp_share_sector = (self.VA_0 / value_added.groupby('region').transform('sum').to_numpy())
+            self.gdp_share_sector = (
+                self.VA_0 / value_added.groupby("region").transform("sum").to_numpy()
+            )
         self.gdp_share_sector = self.gdp_share_sector.flatten()
-        self.matrix_share_thresh = self.Z_C > np.tile(self.X_0, (self.n_sectors, 1)) * 0.00001 # [n_sectors, n_regions*n_sectors]
+        r"""numpy.ndarray of float: Array of size :math:`n \times m` representing the estimated share of a sector in its regional economy."""
+
+        self.matrix_share_thresh = (
+            self.Z_C > np.tile(self.X_0, (self.n_sectors, 1)) * TECHNOLOGY_THRESHOLD
+        )  # [n_sectors, n_regions*n_sectors]
+        r"""numpy.ndarray of float: 2-dim square matrix array of size :math:`(n , n \times m)` representing the threshold under which an input is not considered being an input (0.00001)."""
         #################################################################
 
         ####### SIMULATION VARIABLES ####################################
-        self.overprod = np.full((self.n_regions * self.n_sectors), self.overprod_base, dtype=np.float64)
-        with np.errstate(divide='ignore',invalid='ignore'):
-            self.matrix_stock = ((np.tile(self.X_0, (self.n_sectors, 1)) * self.tech_mat) * self.inv_duration[:,np.newaxis])
-        self.matrix_stock = np.nan_to_num(self.matrix_stock,nan=np.inf, posinf=np.inf)
+        self.overprod = np.full(
+            (self.n_regions * self.n_sectors), self.overprod_base, dtype=np.float64
+        )
+        r"""numpy.ndarray of float: Array of size :math:`n \times m` representing the overproduction coefficients vector :math:`\mathbf{\alpha}(t)`."""
+
+        with np.errstate(divide="ignore", invalid="ignore"):
+            self.matrix_stock = (
+                np.tile(self.X_0, (self.n_sectors, 1)) * self.tech_mat
+            ) * self.inv_duration[:, np.newaxis]
+        self.matrix_stock = np.nan_to_num(self.matrix_stock, nan=np.inf, posinf=np.inf)
+        r"""numpy.ndarray of float: 2-dim square matrix array :math:`\ioinv` of size :math:`(n \times m, n \times m)` representing the stock of inputs (see :ref:`boario-math-init`)."""
+
         self.matrix_stock_0 = self.matrix_stock.copy()
         self.matrix_orders = self.Z_0.copy()
+        r"""numpy.ndarray of float: 2-dim square matrix array :math:`\ioorders` of size :math:`(n \times m, n \times m)` representing the matrix of orders."""
+
         self.production = self.X_0.copy()
+        r"""numpy.ndarray of float: Array :math:`\iox(t)` of size :math:`n \times m` representing the current gross production."""
+
         self.intmd_demand = self.Z_0.copy()
         self.final_demand = self.Y_0.copy()
         self.rebuilding_demand = None
-        #self.rebuild_demand = np.zeros(shape = np.concatenate([self.Z_0,self.Y_0],axis=1).shape)
-        # self.prod_max_toward_rebuilding = None
-        self.kapital_lost = np.zeros(self.production.shape)
-        self.order_type = simulation_params['order_type']
+        self.productive_capital_lost = np.zeros(self.production.shape)
+        r"""numpy.ndarray of float: Array of size :math:`n \times m` representing the estimated stock of capital currently destroyed for each industry."""
 
-        self.prod_cap_delta = np.zeros(shape = self.X_0.shape)
+        self.order_type = order_type
         #################################################################
 
         ################## SIMULATION TRACKING VARIABLES ################
         self.in_shortage = False
+        r"""Boolean stating if at least one industry is in shortage (i.e.) if at least one of its inputs inventory is low enough to reduce production."""
+
         self.had_shortage = False
-        self.records_storage.mkdir(parents=True, exist_ok=True)
-        self.production_evolution = np.memmap(self.records_storage/"iotable_XVA_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.production_evolution.fill(np.nan)
-        self.production_cap_evolution = np.memmap(self.records_storage/"iotable_X_max_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.production_cap_evolution.fill(np.nan)
-        self.final_demand_evolution = np.memmap(self.records_storage/"final_demand_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.final_demand_evolution.fill(np.nan)
-        self.io_demand_evolution = np.memmap(self.records_storage/"io_demand_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.io_demand_evolution.fill(np.nan)
-
-        self.rebuild_demand_evolution = np.memmap(self.records_storage/"rebuild_demand_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.rebuild_demand_evolution.fill(np.nan)
-        self.overproduction_evolution = np.memmap(self.records_storage/"overprodvector_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.overproduction_evolution.fill(np.nan)
-        self.final_demand_unmet_evolution = np.memmap(self.records_storage/"final_demand_unmet_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.final_demand_unmet_evolution.fill(np.nan)
-        self.rebuild_production_evolution = np.memmap(self.records_storage/"rebuild_prod_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.rebuild_production_evolution.fill(np.nan)
-        if simulation_params['register_stocks']:
-            self.stocks_evolution = np.memmap(self.records_storage/"stocks_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors, self.n_sectors*self.n_regions))
-            self.stocks_evolution.fill(np.nan)
-        self.limiting_stocks_evolution = np.memmap(self.records_storage/"limiting_stocks_record", dtype='byte', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors, self.n_sectors*self.n_regions))
-        self.limiting_stocks_evolution.fill(-1)
-        self.regional_sectoral_kapital_destroyed_evol = np.memmap(self.records_storage/"iotable_kapital_destroyed_record", dtype='float64', mode="w+", shape=(simulation_params['n_temporal_units_to_sim'], self.n_sectors*self.n_regions))
-        self.regional_sectoral_kapital_destroyed_evol.fill(np.nan)
-        #############################################################################
+        r"""Boolean stating if at least one industry was in shortage at some point."""
+
+        self.rebuild_prod = np.zeros(shape=self.X_0.shape)
+        r"""numpy.ndarray of float: Array of size :math:`n \times m` representing the remaining stock of rebuilding demand asked of each industry."""
+
+        self.final_demand_not_met = np.zeros(self.Y_0.shape)
+        r"""numpy.ndarray of float: Array of size :math:`n \times m` representing the final demand that could not be met at current step for each industry."""
+
+        #################################################################
 
         ### Internals
         self._prod_delta_type = None
 
         #### POST INIT ####
         ### Event Class Attribute setting
-        Event.possible_regions = self.regions.copy()
+        logger.debug(
+            f"Setting possible regions (currently: {Event.possible_regions}) to: {self.regions}"
+        )
+        Event.possible_regions = pd.CategoricalIndex(
+            self.regions, name="region", copy=True
+        )
+        logger.debug(f"Possible regions is now {Event.possible_regions}")
         Event.regions_idx = np.arange(self.n_regions)
-        Event.possible_sectors = self.sectors.copy()
+        Event.possible_sectors = pd.CategoricalIndex(
+            self.sectors, name="sector", copy=True
+        )
+        Event.possible_final_demand_cat = pd.CategoricalIndex(
+            pym_mrio.get_Y_categories(), name="final demand", copy=True
+        )
         Event.sectors_idx = np.arange(self.n_sectors)
-        Event.temporal_unit_range = simulation_params["n_temporal_units_to_sim"]
         Event.z_shape = self.Z_0.shape
         Event.y_shape = self.Y_0.shape
         Event.x_shape = self.X_0.shape
-        Event.monetary_unit = self.monetary_unit
+        Event.model_monetary_factor = monetary_factor
         Event.sectors_gva_shares = self.gdp_share_sector.copy()
         Event.Z_distrib = self.Z_distrib.copy()
+        Event.Y_distrib = self.Y_distrib.copy()
+        # logger.warning(f"{value_added}")
+        Event.gva_df = value_added.iloc[0].copy()
 
         meta = pym_mrio.meta.metadata
-        Event.mrio_name = meta["name"] + "_" + meta["description"] + "_" + meta["system"] + "_" + meta["version"]
+        assert isinstance(meta, dict)
+        # meta = {"name":"unnamed", "description":"", "system":"unknown","version":"unknown"}
+        try:
+            Event.mrio_name = "_".join(
+                [
+                    str(meta["name"]),
+                    str(meta["description"]),
+                    str(meta["system"]),
+                    str(meta["version"]),
+                ]
+            )
+        except TypeError:
+            Event.mrio_name = "custom - method WIP"
 
         # initialize those (it's not very nice, but otherwise python complains)
-        self._indus_rebuild_demand_tot = None
-        self._house_rebuild_demand_tot = None
-        self._indus_rebuild_demand = None
-        self._house_rebuild_demand = None
-        self._tot_rebuild_demand = None
-        self._kapital_lost = None
-        self._prod_cap_delta_kapital = None
-        self._prod_cap_delta_arbitrary = None
-        self._prod_cap_delta_tot = None
-
-
-        ### Dump indexes
-        self.write_index(results_storage/"jsons"/"indexes.json")
+        self._indus_rebuild_demand_tot: npt.NDArray = np.array([])
+        self._house_rebuild_demand_tot: npt.NDArray = np.array([])
+        self._indus_rebuild_demand: npt.NDArray = np.array([])
+        self._house_rebuild_demand: npt.NDArray = np.array([])
+        self._tot_rebuild_demand: npt.NDArray = np.array([])
+        self._productive_capital_lost: npt.NDArray = np.zeros(self.VA_0.shape)
+        self._prod_cap_delta_productive_capital: npt.NDArray = np.zeros(
+            len(self.industries)
+        )
+        self._prod_cap_delta_arbitrary: npt.NDArray = np.zeros(len(self.industries))
+        self._prod_cap_delta_tot: npt.NDArray = np.zeros(len(self.industries))
 
     ## Properties
 
     @property
-    def tot_rebuild_demand(self) -> Optional[np.ndarray]:
+    def tot_rebuild_demand(self) -> npt.NDArray:
+        r"""Returns current total rebuilding demand (as the sum of rebuilding demand addressed to each industry)"""
         tmp = []
-        if self._indus_rebuild_demand_tot is not None:
+        logger.debug("Trying to return tot_rebuilding demand")
+        if np.any(self._indus_rebuild_demand_tot > 0):
             tmp.append(self._indus_rebuild_demand_tot)
-        if self._house_rebuild_demand_tot is not None:
+        if np.any(self._house_rebuild_demand_tot > 0):
             tmp.append(self._house_rebuild_demand_tot)
-        if tmp != []:
-            ret = np.concatenate(tmp,axis=1).sum(axis=1)
+        if tmp:
+            ret = np.concatenate(tmp, axis=1).sum(axis=1)
             self._tot_rebuild_demand = ret
         else:
-            self._tot_rebuild_demand = None
+            self._tot_rebuild_demand = np.array([])
         return self._tot_rebuild_demand
 
     @tot_rebuild_demand.setter
-    def tot_rebuild_demand(self, source:list[Event]):
-        """Compute and update total rebuilding demand.
-
-        Compute and update total rebuilding demand for the given list of events. Only events
-        tagged as rebuildable are accounted for.
+    def tot_rebuild_demand(self, source: list[EventKapitalRebuild]):
+        r"""Computes and updates total rebuilding demand based on a list of events.
 
-        TODO: ADD MATH
+        Compute and update rebuilding demand for the given list of events. Only events
+        tagged as rebuildable are accounted for. Both `house_rebuild_demand` and
+        `indus_rebuild_demand` are updated.
 
         Parameters
         ----------
-        events : 'list[Event]'
-            A list of Event objects
+        events : 'list[EventKapitalRebuild]'
+            A list of EventKapitalRebuild objects
         """
+        logger.debug(f"Trying to set tot_rebuilding demand from {source}")
         if not isinstance(source, list):
-            ValueError("Setting tot_rebuild_demand can only be done with a list of events, not a {}".format(type(source)))
-
+            ValueError(
+                f"Setting tot_rebuild_demand can only be done with a list of events, not a {type(source)}"
+            )
         self.house_rebuild_demand = source
         self.indus_rebuild_demand = source
 
     @property
-    def house_rebuild_demand(self)->Optional[np.ndarray]:
+    def house_rebuild_demand(self) -> npt.NDArray:
+        r"""Returns household rebuilding demand matrix.
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\ioy`, containing the sum of all currently
+            rebuildable final demand stock.
+        """
+
         return self._house_rebuild_demand
 
     @property
-    def house_rebuild_demand_tot(self)->Optional[np.ndarray]:
+    def house_rebuild_demand_tot(self) -> npt.NDArray:
+        r"""Returns total household rebuilding demand vector.
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\iox`, containing the sum of all currently
+            rebuildable households demands.
+        """
+
         return self._house_rebuild_demand_tot
 
     @house_rebuild_demand.setter
-    def house_rebuild_demand(self, source:list[Event]):
-        r"""Compute rebuild demand from household demand from a list of events
+    def house_rebuild_demand(self, source: list[EventKapitalRebuild]):
+        r"""Computes rebuild demand from household from a list of events
 
-        Compute and return rebuilding final households demand for the given list of events
-        by summing the rebuilding_demand_house member of each event. Only events
-        tagged as rebuildable are accounted for. The shape of the array
-        returned is the same as the final demand member (``Y_0`` | :math:`\ioy`) of the calling MrioSystem.
+        Computes and sets rebuilding final households demand for the given list of events
+        by summing the `rebuilding_demand_house member` of each event and multiplying it
+        by the characteristic rebuilding time (inverse of its value). Only events
+        tagged as rebuildable are accounted for.
+
+        If the event has its own rebuilding characteristic time :math:`\tau_{\textrm{REBUILD}}` it is applied,
+        else the model rebuilding characteristic time is used.
 
         Parameters
         ----------
         events : 'list[Event]'
             A list of Event objects
 
-        Returns
-        -------
-        np.ndarray
-            An array of same shape as Y_0, containing the sum of all currently
-            rebuildable final demand stock from all events in the given list.
-
-        Notes
-        -----
-
-        Currently the model wasn't tested with such a rebuilding demand. Only intermediate demand is considered.
         """
         tmp = []
-        for ev in source:
-            if ev.rebuildable:
-                if ev.rebuild_tau is None:
+        for evnt in source:
+            if evnt.rebuildable:
+                if evnt.rebuild_tau is None:
                     rebuild_tau = self.rebuild_tau
                 else:
-                    rebuild_tau = ev.rebuild_tau
+                    rebuild_tau = evnt.rebuild_tau
                     warn_once(logger, "Event has a custom rebuild_tau")
-                if ev._rebuilding_demand_house is not None:
-                    tmp.append(ev._rebuilding_demand_house * (self.n_temporal_units_by_step / rebuild_tau))
-        if tmp == []:
-            self._house_rebuild_demand = None
-            self._house_rebuild_demand_tot = None
+                if len(evnt.rebuilding_demand_house) > 0:
+                    tmp.append(
+                        evnt.rebuilding_demand_house
+                        * (self.n_temporal_units_by_step / rebuild_tau)
+                    )
+        if not tmp:
+            self._house_rebuild_demand = np.array([])
+            self._house_rebuild_demand_tot = np.array([])
         else:
-            house_reb_dem = np.stack(tmp,axis=-1)
+            house_reb_dem = np.stack(tmp, axis=-1)
             tot = house_reb_dem.sum(axis=1)
             self._house_rebuild_demand = house_reb_dem
             self._house_rebuild_demand_tot = tot
 
     @property
-    def indus_rebuild_demand(self)->Optional[np.ndarray]:
+    def indus_rebuild_demand(self) -> npt.NDArray:
+        r"""Returns industrial rebuilding demand matrix.
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\ioz`, containing the sum of all currently
+            rebuildable intermediate demand stock.
+        """
+
         return self._indus_rebuild_demand
 
     @property
-    def indus_rebuild_demand_tot(self)->Optional[np.ndarray]:
+    def indus_rebuild_demand_tot(self) -> npt.NDArray:
+        r"""Returns total industrial rebuilding demand vector.
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\iox`, containing the sum of all currently
+            rebuildable intermediate demands.
+        """
+
         return self._indus_rebuild_demand_tot
 
     @indus_rebuild_demand.setter
-    def indus_rebuild_demand(self, source:list[Event]):
-        r"""Compute rebuild demand from economic sectors (i.e. not households)
+    def indus_rebuild_demand(self, source: list[EventKapitalRebuild]):
+        r"""Computes rebuild demand from economic sectors (i.e. not households)
 
-        Compute and return rebuilding 'intermediate demand' for the given list of events
-        by summing the rebuildind_demand_indus of each event. Only events
-        tagged as rebuildable are accounted for. The shape of the array
-        returned is the same as the intermediate demand member (``Z_0`` | :math:`\ioz`) of the calling
-        MrioSystem.
+        Computes and sets rebuilding 'intermediate demand' for the given list of events
+        by summing the `rebuildind_demand_indus` of each event. Only events
+        tagged as rebuildable are accounted for.
 
         Parameters
         ----------
         events : 'list[Event]'
             A list of Event objects
 
-        Returns
-        -------
-        np.ndarray
-            An array of same shape as Z_0, containing the sum of all currently
-            rebuildable intermediate demand stock from all events in the given list.
         """
+
         tmp = []
-        for ev in source:
-            if ev.rebuildable:
-                if ev.rebuild_tau is None:
+        for evnt in source:
+            if evnt.rebuildable:
+                if evnt.rebuild_tau is None:
                     rebuild_tau = self.rebuild_tau
                 else:
-                    rebuild_tau = ev.rebuild_tau
+                    rebuild_tau = evnt.rebuild_tau
                     warn_once(logger, "Event has a custom rebuild_tau")
-                tmp.append(ev._rebuilding_demand_indus * (self.n_temporal_units_by_step / rebuild_tau))
-
-        if tmp == []:
-            self._indus_rebuild_demand = None
-            self._indus_rebuild_demand_tot = None
+                tmp.append(
+                    evnt.rebuilding_demand_indus
+                    * (self.n_temporal_units_by_step / rebuild_tau)
+                )
+
+        if not tmp:
+            self._indus_rebuild_demand = np.array([])
+            self._indus_rebuild_demand_tot = np.array([])
         else:
-            indus_reb_dem = np.stack(tmp,axis=-1)
+            indus_reb_dem = np.stack(tmp, axis=-1)
             self._indus_rebuild_demand = indus_reb_dem
             self._indus_rebuild_demand_tot = indus_reb_dem.sum(axis=1)
+            # logger.debug(f"Setting indus_rebuild_demand_tot to {indus_reb_dem}")
+
     @property
-    def kapital_lost(self) -> Optional[np.ndarray]:
-        return self._kapital_lost
+    def productive_capital_lost(self) -> npt.NDArray:
+        r"""Returns current stock of destroyed capital
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\iox`, containing the "stock"
+        of capital currently destroyed for each industry.
+        """
 
-    @kapital_lost.setter
-    def kapital_lost(self, source:list[Event]|np.ndarray
-                              ) -> None:
-        if isinstance(source,list):
-            if source != []:
-                events_K = [ev for ev in source if "kapital_destroyed" in ev.shock_type]
-                self._kapital_lost = np.add.reduce(np.array([e.regional_sectoral_kapital_destroyed for e in events_K]))
+        return self._productive_capital_lost
+
+    @productive_capital_lost.setter
+    def productive_capital_lost(
+        self, source: list[EventKapitalDestroyed] | npt.NDArray
+    ) -> None:
+        r"""Computes current capital lost and update production delta accordingly.
+
+        Computes and sets the current stock of capital lost by each industry of
+        the model due to the given list of events. Also update the production
+        capacity lost accordingly by computing the ratio of capital lost of
+        capital stock.
+
+        Parameters
+        ----------
+        source : list[EventKapitalDestroyed] | npt.NDArray
+            Either a list of events to consider for the destruction
+        of capital or directly a vector of destroyed capital for each industry.
+
+        """
+
+        logger.debug("Updating productive_capital lost from list of events")
+        if isinstance(source, list):
+            if source:
+                self._productive_capital_lost = np.add.reduce(
+                    np.array(
+                        [
+                            e.regional_sectoral_productive_capital_destroyed
+                            for e in source
+                        ]
+                    )
+                )
             else:
-                self._kapital_lost = np.zeros(self.VA_0.shape)
-        elif isinstance(source,np.ndarray):
-            self._kapital_lost = source
-
-        productivity_loss_from_K = np.zeros(shape=self._kapital_lost.shape)
-        k_stock = (self.VA_0 * self.kstock_ratio_to_VA)
-        np.divide(self._kapital_lost, k_stock, out=productivity_loss_from_K, where=k_stock!=0)
-        self._prod_cap_delta_kapital = productivity_loss_from_K
-        if (self._prod_cap_delta_kapital > 0.0).any():
+                self._productive_capital_lost = np.zeros(self.VA_0.shape)
+        elif isinstance(source, np.ndarray):
+            self._productive_capital_lost = source
+
+        productivity_loss_from_capital_destroyed = np.zeros(
+            shape=self._productive_capital_lost.shape
+        )
+        np.divide(
+            self._productive_capital_lost,
+            self.k_stock,
+            out=productivity_loss_from_capital_destroyed,
+            where=self.k_stock != 0,
+        )
+        logger.debug("Updating production delta from productive_capital loss")
+        self._prod_cap_delta_productive_capital = (
+            productivity_loss_from_capital_destroyed
+        )
+        if (self._prod_cap_delta_productive_capital > 0.0).any():
             if self._prod_delta_type is None:
-                self._prod_delta_type = "from_kapital"
+                self._prod_delta_type = "from_productive_capital"
             elif self._prod_delta_type == "from_arbitrary":
-                self._prod_delta_type = "mixed_from_kapital_from_arbitrary"
+                self._prod_delta_type = "mixed_from_productive_capital_from_arbitrary"
 
     @property
-    def prod_cap_delta_arbitrary(self) -> Optional[np.ndarray]:
+    def prod_cap_delta_arbitrary(self) -> npt.NDArray:
+        r"""Return the possible "arbitrary" production capacity lost vector if
+        it was set.
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\iox`, stating the amount of production
+        capacity lost arbitrarily (ie exogenous).
+        """
         return self._prod_cap_delta_arbitrary
 
     @prod_cap_delta_arbitrary.setter
-    def prod_cap_delta_arbitrary(self, source: list[Event]|np.ndarray):
-        if isinstance(source,list):
-            event_arb = np.array([ev for ev in source if ev.prod_cap_delta_arbitrary is not None])
+    def prod_cap_delta_arbitrary(self, source: list[EventArbitraryProd] | npt.NDArray):
+        """Computes and sets the loss of production capacity from "arbitrary" sources.
+
+        Parameters
+        ----------
+        source : list[Event] | npt.NDArray
+            Either a list of Event objects with arbitrary production losses
+            set, or directly a vector of production capacity loss.
+
+        """
+
+        if isinstance(source, list):
+            event_arb = np.array(
+                [
+                    ev.prod_cap_delta_arbitrary
+                    for ev in source
+                    if len(ev.prod_cap_delta_arbitrary) > 0
+                ]
+            )
             if event_arb.size == 0:
-                self._prod_cap_delta_arbitrary = np.zeros(shape = self.X_0.shape)
+                self._prod_cap_delta_arbitrary = np.zeros(shape=self.X_0.shape)
             else:
-                self._prod_cap_delta_arbitrary = np.max.reduce(event_arb)
+                self._prod_cap_delta_arbitrary = np.maximum.reduce(event_arb)
         else:
-            self._prod_capt_delta_arbitrary= source
+            self._prod_capt_delta_arbitrary = source
         assert self._prod_cap_delta_arbitrary is not None
         if (self._prod_cap_delta_arbitrary > 0.0).any():
             if self._prod_delta_type is None:
                 self._prod_delta_type = "from_arbitrary"
-            elif self._prod_delta_type == "from_kapital":
-                self._prod_delta_type = "mixed_from_kapital_from_arbitrary"
+            elif self._prod_delta_type == "from_productive_capital":
+                self._prod_delta_type = "mixed_from_productive_capital_from_arbitrary"
 
     @property
-    def prod_cap_delta_kapital(self) -> Optional[np.ndarray]:
-        return self._prod_cap_delta_kapital
+    def prod_cap_delta_productive_capital(self) -> npt.NDArray:
+        r"""Return the possible production capacity lost due to capital destroyed vector if
+        it was set.
+
+        Returns
+        -------
+        npt.NDArray
+            An array of same shape as math:`\iox`, stating the amount of production
+        capacity lost due to capital destroyed.
+        """
+
+        return self._prod_cap_delta_productive_capital
 
     @property
-    def prod_cap_delta_tot(self) -> np.ndarray:
+    def prod_cap_delta_tot(self) -> npt.NDArray:
+        r"""Computes and return total current production delta.
+
+        Returns
+        -------
+        npt.NDArray
+            The total production delta (ie share of production capacity lost)
+            for each industry.
+
+        """
+
+        logger.debug("Trying to retrieve current production delta")
         tmp = []
         if self._prod_delta_type is None:
             raise AttributeError("Production delta doesn't appear to be set yet.")
-        elif self._prod_delta_type == "from_kapital":
-            tmp.append(self._prod_cap_delta_kapital)
+        elif self._prod_delta_type == "from_productive_capital":
+            logger.debug(
+                "Production delta is only set from productive_capital destruction"
+            )
+            tmp.append(self._prod_cap_delta_productive_capital)
         elif self._prod_delta_type == "from_arbitrary":
+            logger.debug("Production delta is only set from arbitrary delta")
             tmp.append(self._prod_cap_delta_arbitrary)
-        elif self._prod_delta_type == "mixed_from_kapital_from_arbitrary":
-            tmp.append(self._prod_cap_delta_kapital)
+        elif self._prod_delta_type == "mixed_from_productive_capital_from_arbitrary":
+            logger.debug(
+                "Production delta is a mixed form of productive_capital destruction and arbitrary delta"
+            )
+            tmp.append(self._prod_cap_delta_productive_capital)
             tmp.append(self._prod_cap_delta_arbitrary)
         else:
-            raise NotImplementedError("Production delta type {} not recognised".format(self._prod_delta_type))
-        tmp.append(np.ones(shape=self.X_0.shape))
-        #logger.debug("tmp: {}".format(tmp))
-        self._prod_cap_delta_tot = np.amin(np.stack(tmp,axis=-1),axis=1)
-        assert self._prod_cap_delta_tot.shape == self.X_0.shape, "expected shape {}, received {}".format(self.X_0.shape, self._prod_cap_delta_tot.shape)
+            raise NotImplementedError(
+                f"Production delta type {self._prod_delta_type} not recognised"
+            )
+        # tmp.append(np.ones(shape=self.X_0.shape))
+        # logger.debug("tmp: {}".format(tmp))
+        self._prod_cap_delta_tot = np.amax(np.stack(tmp, axis=-1), axis=1)
+        assert (
+            self._prod_cap_delta_tot.shape == self.X_0.shape
+        ), f"expected shape {self.X_0.shape}, received {self._prod_cap_delta_tot.shape}"
         return self._prod_cap_delta_tot
 
     @prod_cap_delta_tot.setter
     def prod_cap_delta_tot(self, source: list[Event]):
-        if not isinstance(source,list):
-            ValueError("Setting prod_cap_delta_tot can only be done with a list of events, not a {}".format(type(source)))
+        r"""Computes and sets the loss of production capacity from both "arbitrary" sources and
+        capital destroyed.
+
+        Parameters
+        ----------
+        source : list[Event]
+            A list of Event objects.
+
+        """
 
-        self.kapital_lost = source
-        self.prod_cap_delta_arbitrary = source
+        logger.debug("Updating total production delta from list of events")
+        if not isinstance(source, list):
+            ValueError(
+                f"Setting prod_cap_delta_tot can only be done with a list of events, not a {type(source)}"
+            )
+
+        self.productive_capital_lost = [
+            event for event in source if isinstance(event, EventKapitalDestroyed)
+        ]
+        self.prod_cap_delta_arbitrary = [
+            event for event in source if isinstance(event, EventArbitraryProd)
+        ]
 
     def update_system_from_events(self, events: list[Event]) -> None:
-        """Update MrioSystem variables according to given list of events
+        """Update model variables according to given list of events
 
-        Compute kapital loss for each industry affected as the sum of their total rebuilding demand (to each rebuilding sectors and for each events). This information is stored as a 1D array ``kapital_lost`` of size :math:`n \time m`.
-        Also compute the total rebuilding demand.
+        Computes and sets both the total production delta from all events, and the total rebuilding demand.
 
         Parameters
         ----------
         events : 'list[Event]'
             List of events (as Event objects) to consider.
 
         """
+        logger.debug("Updating system from list of events")
         self.prod_cap_delta_tot = events
-        self.tot_rebuild_demand = events
-
+        self.tot_rebuild_demand = [
+            event for event in events if isinstance(event, EventKapitalRebuild)
+        ]
 
     @property
-    def production_cap(self)->np.ndarray:
+    def production_cap(self) -> npt.NDArray:
         r"""Compute and update production capacity.
 
-        Compute and update production capacity from possible kapital damage and overproduction.
+        Compute and update production capacity from current total production delta and overproduction.
 
         .. math::
 
             x^{Cap}_{f}(t) = \alpha_{f}(t) (1 - \Delta_{f}(t)) x_{f}(t)
 
         Raises
         ------
         ValueError
-            Raised if any industry has negative production (probably from kapital loss too high)
+            Raised if any industry has negative production.
         """
         production_cap = self.X_0.copy()
-        if (self._prod_delta_type is not None):
+        if self._prod_delta_type is not None:
             prod_delta_tot = self.prod_cap_delta_tot.copy()
-            if (prod_delta_tot > 0.).any():
+            if (prod_delta_tot > 0.0).any():
                 production_cap = production_cap * (1 - prod_delta_tot)
         if (self.overprod > 1.0).any():
             production_cap = production_cap * self.overprod
-        if (production_cap < 0).any() :
-            raise ValueError("Production capacity was found negative for at least on industry")
+        if (production_cap < 0).any():
+            raise ValueError(
+                "Production capacity was found negative for at least on industry"
+            )
         return production_cap
 
     @property
-    def total_demand(self) -> np.ndarray:
-        """Computes and updates total demand
-
-        Update total rebuild demand (and apply rebuilding characteristic time
-        if ``separate_rebuilding`` is False, then sum/reduce rebuilding, orders
-        and final demand together and accordingly update vector of total
-        demand.
-
-        Parameters
-        ----------
-        events : 'list[Event]'
-            List of Event to consider for rebuilding demand.
-        separate_rebuilding : bool
-            A boolean specifying if rebuilding demand should be treated as a whole (true) or under the characteristic time/proportional scheme strategy.
-        Returns
-        -------
-        None
+    def total_demand(self) -> npt.NDArray:
+        r"""Computes and returns total demand as the sum of intermediate demand (orders), final demand, and possible rebuilding demand."""
 
-        """
-        if (self.matrix_orders < 0).any() :
+        if (self.matrix_orders < 0).any():
             raise RuntimeError("Some matrix orders are negative which shouldn't happen")
 
         tot_dem = self.matrix_orders.sum(axis=1) + self.final_demand.sum(axis=1)
-        if (tot_dem < 0).any() :
+        if (tot_dem < 0).any():
             raise RuntimeError("Some total demand are negative which shouldn't happen")
-        if self.tot_rebuild_demand is not None:
+        if len(self.tot_rebuild_demand) > 0:
             tot_dem += self.tot_rebuild_demand
         return tot_dem
 
     @property
-    def production_opt(self) -> np.ndarray:
+    def production_opt(self) -> npt.NDArray:
+        r"""Computes and returns "optimal production" :math:`\iox^{textrm{Opt}}`, as the per industry minimum between
+        total demand and production capacity.
+
+        """
+
         return np.fmin(self.total_demand, self.production_cap)
 
     @property
-    def inventory_constraints_opt(self) -> np.ndarray:
+    def inventory_constraints_opt(self) -> npt.NDArray:
+        r"""Computes and returns inventory constraints for "optimal production" (see :meth:`calc_inventory_constraints`)"""
+
         return self.calc_inventory_constraints(self.production_opt)
 
     @property
-    def inventory_constraints_act(self) -> np.ndarray:
+    def inventory_constraints_act(self) -> npt.NDArray:
+        r"""Computes and returns inventory constraints for "actual production" (see :meth:`calc_inventory_constraints`)"""
         return self.calc_inventory_constraints(self.production)
 
-    def calc_production(self, current_temporal_unit:int) -> np.ndarray:
-        r"""Compute and update actual production
+    def calc_production(self, current_temporal_unit: int) -> npt.NDArray:
+        r"""Computes and updates actual production. See :ref:`boario-math-prod`.
 
-        1. Compute ``production_opt`` and ``inventory_constraints`` as :
+        1. Computes ``production_opt`` and ``inventory_constraints`` as :
 
         .. math::
            :nowrap:
 
                 \begin{alignat*}{4}
                       \iox^{\textrm{Opt}}(t) &= (x^{\textrm{Opt}}_{f}(t))_{f \in \firmsset} &&= \left ( \min \left ( d^{\textrm{Tot}}_{f}(t), x^{\textrm{Cap}}_{f}(t) \right ) \right )_{f \in \firmsset} && \text{Optimal production}\\
                       \mathbf{\ioinv}^{\textrm{Cons}}(t) &= (\omega^{\textrm{Cons},f}_p(t))_{\substack{p \in \sectorsset\\f \in \firmsset}} &&=
@@ -626,82 +960,102 @@
                 \begin{alignat*}{4}
                     \iox^{a}(t) &= (x^{a}_{f}(t))_{f \in \firmsset} &&= \left \{ \begin{aligned}
                                                            & x^{\textrm{Opt}}_{f}(t) & \text{if $\omega_{p}^f(t) \geq \omega^{\textrm{Cons},f}_p(t)$}\\
                                                            & x^{\textrm{Opt}}_{f}(t) \cdot \min_{p \in \sectorsset} \left ( \frac{\omega^s_{p}(t)}{\omega^{\textrm{Cons,f}}_p(t)} \right ) & \text{if $\omega_{p}^f(t) < \omega^{\textrm{Cons},f}_p(t)$}
                                                            \end{aligned} \right. \quad &&
                 \end{alignat*}
 
-        Also warns in log if such shortages happen.
+        Also warns in logs if such shortages happen.
 
 
         Parameters
         ----------
         current_temporal_unit : int
             current step number
 
         """
-        #1.
+        # 1.
         production_opt = self.production_opt.copy()
         inventory_constraints = self.inventory_constraints_opt.copy()
-        #2.
-        if (stock_constraint := (self.matrix_stock < inventory_constraints) * self.matrix_share_thresh).any():
+        # 2.
+        if (
+            stock_constraint := (self.matrix_stock < inventory_constraints)
+            * self.matrix_share_thresh
+        ).any():
             if not self.in_shortage:
-                logger.info('At least one industry entered shortage regime. (step:{})'.format(current_temporal_unit))
+                logger.info(
+                    f"At least one industry entered shortage regime. (step:{current_temporal_unit})"
+                )
             self.in_shortage = True
             self.had_shortage = True
             production_ratio_stock = np.ones(shape=self.matrix_stock.shape)
-            np.divide(self.matrix_stock, inventory_constraints, out=production_ratio_stock, where=(self.matrix_share_thresh * (inventory_constraints!=0)))
+            np.divide(
+                self.matrix_stock,
+                inventory_constraints,
+                out=production_ratio_stock,
+                where=(self.matrix_share_thresh * (inventory_constraints != 0)),
+            )
             production_ratio_stock[production_ratio_stock > 1] = 1
             if (production_ratio_stock < 1).any():
-                production_max = np.tile(production_opt, (self.n_sectors, 1)) * production_ratio_stock
-                assert not (np.min(production_max,axis=0) < 0).any()
+                production_max = (
+                    np.tile(production_opt, (self.n_sectors, 1))
+                    * production_ratio_stock
+                )
+                assert not (np.min(production_max, axis=0) < 0).any()
                 self.production = np.min(production_max, axis=0)
             else:
                 assert not (production_opt < 0).any()
                 self.production = production_opt
         else:
             if self.in_shortage:
                 self.in_shortage = False
-                logger.info('All industries exited shortage regime. (step:{})'.format(current_temporal_unit))
+                logger.info(
+                    f"All industries exited shortage regime. (step:{current_temporal_unit})"
+                )
             assert not (production_opt < 0).any()
             self.production = production_opt
         return stock_constraint
 
-    def calc_inventory_constraints(self, production:np.ndarray) -> np.ndarray :
-        """Compute inventory constraint (no psi parameter)
+    def calc_inventory_constraints(self, production: npt.NDArray) -> npt.NDArray:
+        r"""Compute inventory constraints (no psi parameter, for the psi version,
+        the recommended one, see :meth:`~boario.extended_models.ARIOPsiModel.calc_inventory_constraints`)
 
-        See :meth:`calc_production`.
+        See :meth:`calc_production` for how inventory constraints are computed.
 
         Parameters
         ----------
-        production : np.ndarray
-            production vector
+        production : npt.NDArray
+            The production vector to consider.
 
         Returns
         -------
-        np.ndarray
-            A boolean NDArray `stock_constraint` of the same shape as ``matrix_stock`` (ie `(n_sectors,n_regions*n_sectors)`), with ``True`` for any input not meeting the inventory constraints.
+        npt.NDArray
+            For each input, for each industry, the size of the inventory required to produce at `production` level
+        for the duration goal (`inv_duration`).
 
         """
-        inventory_constraints = (np.tile(production, (self.n_sectors, 1)) * self.tech_mat)
-        tmp = np.tile(np.nan_to_num(self.inv_duration, posinf=0.)[:,np.newaxis],(1,self.n_regions*self.n_sectors))
+        inventory_constraints = np.tile(production, (self.n_sectors, 1)) * self.tech_mat
+        tmp = np.tile(
+            np.nan_to_num(self.inv_duration, posinf=0.0)[:, np.newaxis],
+            (1, self.n_regions * self.n_sectors),
+        )
         return inventory_constraints * tmp
 
-
-
-    def distribute_production(self,
-                              current_temporal_unit: int, rebuildable_events: 'list[Event]',
-                              scheme:str='proportional', separate_rebuilding:bool=False) -> list[Event]:
+    def distribute_production(
+        self,
+        rebuildable_events: list[EventKapitalRebuild],
+        scheme: str = "proportional",
+    ) -> list[EventKapitalRebuild]:
         r"""Production distribution module
 
     #. Computes rebuilding demand for each rebuildable events (applying the `rebuild_tau` characteristic time)
 
     #. Creates/Computes total demand matrix (Intermediate + Final + Rebuild)
 
-    #. Assesses if total demand is greater than realized production, hence requiring rationning
+    #. Assesses if total demand is greater than realized production, hence requiring rationing
 
     #. Distributes production proportionally to demand such that :
 
         .. math::
            :nowrap:
 
                \begin{alignat*}{4}
@@ -768,368 +1122,444 @@
     RuntimeError
         If negative values are found in places there's should not be any
     ValueError
         If an attempt to run an unimplemented distribution scheme is tried
 
 """
 
-        if scheme != 'proportional':
-            raise ValueError("Scheme %s not implemented"% scheme)
+        if scheme != "proportional":
+            raise ValueError(f"Scheme {scheme} is currently not implemented")
 
-        list_of_demands = [self.matrix_orders, self.final_demand]
+        # list_of_demands = [self.matrix_orders, self.final_demand]
         ## 1. Calc demand from rebuilding requirements (with characteristic time rebuild_tau)
-        if rebuildable_events != []:
+        house_reb_dem_per_event = (
+            house_reb_dem_tot_per_event
+        ) = indus_reb_dem_per_event = indus_reb_dem_tot_per_event = None
+
+        if rebuildable_events:
+            logger.debug("There are rebuildable events")
             n_events = len(rebuildable_events)
             tot_rebuilding_demand_summed = self.tot_rebuild_demand.copy()
             # debugging assert
-            assert tot_rebuilding_demand_summed.shape == self.X_0.shape
+            if not tot_rebuilding_demand_summed.shape == self.X_0.shape:
+                raise RuntimeError(
+                    f"received {tot_rebuilding_demand_summed.shape}, expected {self.X_0.shape}"
+                )
             indus_reb_dem_tot_per_event = self.indus_rebuild_demand_tot.copy()
             indus_reb_dem_per_event = self.indus_rebuild_demand.copy()
 
             # expected shape assert (debug also)
-            exp_shape_indus_per_event = (self.n_sectors*self.n_regions,self.n_sectors*self.n_regions,n_events)
-            exp_shape_indus_tot_per_event = (self.n_sectors*self.n_regions,n_events)
-            assert indus_reb_dem_per_event.shape == exp_shape_indus_per_event, "expected shape is {}, given shape is {}".format(exp_shape_indus_per_event, indus_reb_dem_per_event.shape)
-            assert indus_reb_dem_tot_per_event.shape == exp_shape_indus_tot_per_event, "expected shape is {}, given shape is {}".format(exp_shape_indus_tot_per_event, indus_reb_dem_tot_per_event.shape)
+            exp_shape_indus_per_event = (
+                self.n_sectors * self.n_regions,
+                self.n_sectors * self.n_regions,
+                n_events,
+            )
+            exp_shape_indus_tot_per_event = (self.n_sectors * self.n_regions, n_events)
+            assert (
+                indus_reb_dem_per_event.shape == exp_shape_indus_per_event
+            ), "expected shape is {}, given shape is {}".format(
+                exp_shape_indus_per_event, indus_reb_dem_per_event.shape
+            )
+            assert (
+                indus_reb_dem_tot_per_event.shape == exp_shape_indus_tot_per_event
+            ), "expected shape is {}, given shape is {}".format(
+                exp_shape_indus_tot_per_event, indus_reb_dem_tot_per_event.shape
+            )
 
             house_reb_dem_tot_per_event = self.house_rebuild_demand_tot.copy()
             house_reb_dem_per_event = self.house_rebuild_demand.copy()
 
             # expected shape assert (debug also)
-            exp_shape_house = (self.n_sectors*self.n_regions,self.n_fd_cat*self.n_regions,n_events)
-            exp_shape_house_tot = (self.n_sectors*self.n_regions,n_events)
+            exp_shape_house = (
+                self.n_sectors * self.n_regions,
+                self.n_fd_cat * self.n_regions,
+                n_events,
+            )
+            exp_shape_house_tot = (self.n_sectors * self.n_regions, n_events)
             assert house_reb_dem_per_event.shape == exp_shape_house
             assert house_reb_dem_tot_per_event.shape == exp_shape_house_tot
             h_reb = (house_reb_dem_tot_per_event > 0).any()
-            ind_reb=(indus_reb_dem_tot_per_event > 0).any()
+            ind_reb = (indus_reb_dem_tot_per_event > 0).any()
         else:
             tot_rebuilding_demand_summed = np.zeros(shape=self.X_0.shape)
             h_reb = False
             ind_reb = False
 
         ## 2. Concat to have total demand matrix (Intermediate + Final + Rebuild)
-        tot_demand = np.concatenate([self.matrix_orders, self.final_demand, np.expand_dims(tot_rebuilding_demand_summed,1)], axis=1)
+        tot_demand = np.concatenate(
+            [
+                self.matrix_orders,
+                self.final_demand,
+                np.expand_dims(tot_rebuilding_demand_summed, 1),
+            ],
+            axis=1,
+        )
         ## 3. Does production meet total demand
-        rationning_required = (self.production - tot_demand.sum(axis=1))<(-1/self.monetary_unit)
-        rationning_mask = np.tile(rationning_required[:,np.newaxis],(1,tot_demand.shape[1]))
-        demand_share = np.full(tot_demand.shape,0.0)
-        tot_dem_summed = np.expand_dims(np.sum(tot_demand, axis=1, where=rationning_mask),1)
+        logger.debug(f"tot demand shape : {tot_demand.shape}")
+        rationing_required = (self.production - tot_demand.sum(axis=1)) < (
+            -1 / self.monetary_factor
+        )
+        rationning_mask = np.tile(
+            rationing_required[:, np.newaxis], (1, tot_demand.shape[1])
+        )
+        demand_share = np.full(tot_demand.shape, 0.0)
+        tot_dem_summed = np.expand_dims(
+            np.sum(tot_demand, axis=1, where=rationning_mask), 1
+        )
         # Get demand share
-        np.divide(tot_demand, tot_dem_summed, where=(tot_dem_summed!=0), out=demand_share)
+        np.divide(
+            tot_demand, tot_dem_summed, where=(tot_dem_summed != 0), out=demand_share
+        )
         distributed_production = tot_demand.copy()
         # 4. distribute production proportionally to demand
-        np.multiply(demand_share, np.expand_dims(self.production,1), out=distributed_production, where=rationning_mask)
-        intmd_distribution = distributed_production[:,:self.n_sectors * self.n_regions]
+        np.multiply(
+            demand_share,
+            np.expand_dims(self.production, 1),
+            out=distributed_production,
+            where=rationning_mask,
+        )
+        intmd_distribution = distributed_production[
+            :, : self.n_sectors * self.n_regions
+        ]
         # Stock use is simply production times technical coefs
-        stock_use = np.tile(self.production, (self.n_sectors,1)) * self.tech_mat
-        if (stock_use < 0).any() :
-            raise RuntimeError("Stock use contains negative values, this should not happen")
+        stock_use = np.tile(self.production, (self.n_sectors, 1)) * self.tech_mat
+        if (stock_use < 0).any():
+            raise RuntimeError(
+                "Stock use contains negative values, this should not happen"
+            )
         # 5. Restock is the production from each supplier, summed.
         stock_add = self._matrix_I_sum @ intmd_distribution
         if (stock_add < 0).any():
-            raise RuntimeError("stock_add (restocking) contains negative values, this should not happen")
+            raise RuntimeError(
+                "stock_add (restocking) contains negative values, this should not happen"
+            )
         if not np.allclose(stock_add, stock_use):
             self.matrix_stock = self.matrix_stock - stock_use + stock_add
             if (self.matrix_stock < 0).any():
-                self.matrix_stock.dump(self.records_storage/"matrix_stock_dump.pkl")
-                logger.error("Negative values in the stocks, matrix has been dumped in the results dir : \n {}".format(self.records_storage/"matrix_stock_dump.pkl"))
-                raise RuntimeError("stock_add (restocking) contains negative values, this should not happen")
+                raise RuntimeError(
+                    "matrix_stock contains negative values, this should not happen"
+                )
 
         # 6. Compute final demand not met due to rationing
-        final_demand_not_met = self.final_demand - distributed_production[:,self.n_sectors*self.n_regions:(self.n_sectors*self.n_regions + self.n_fd_cat*self.n_regions)]
+        final_demand_not_met = (
+            self.final_demand
+            - distributed_production[
+                :,
+                self.n_sectors
+                * self.n_regions : (
+                    self.n_sectors * self.n_regions + self.n_fd_cat * self.n_regions
+                ),
+            ]
+        )
         final_demand_not_met = final_demand_not_met.sum(axis=1)
         # avoid -0.0 (just in case)
-        final_demand_not_met[final_demand_not_met==0.] = 0.
-        self.write_final_demand_unmet(current_temporal_unit, final_demand_not_met)
+        final_demand_not_met[final_demand_not_met == 0.0] = 0.0
+        self.final_demand_not_met = final_demand_not_met.copy()
 
         # 7. Compute production delivered to rebuilding
-        rebuild_prod = distributed_production[:,(self.n_sectors*self.n_regions + self.n_fd_cat*self.n_regions):].copy().flatten()
-        self.write_rebuild_prod(current_temporal_unit,rebuild_prod) #type: ignore
+        logger.debug(f"distributed prod shape : {distributed_production.shape}")
+        rebuild_prod = (
+            distributed_production[
+                :, (self.n_sectors * self.n_regions + self.n_fd_cat * self.n_regions) :
+            ]
+            .copy()
+            .flatten()
+        )
+        self.rebuild_prod = rebuild_prod.copy()
+
+        logger.debug(
+            f"tot_rebuilding_demand_summed: {pd.Series(tot_rebuilding_demand_summed, index=self.industries)}"
+        )
 
         if h_reb and ind_reb:
-            #logger.debug("Entering here")
-            indus_shares = np.divide(indus_reb_dem_tot_per_event, tot_rebuilding_demand_summed, where=(tot_rebuilding_demand_summed!=0))
-            house_shares = np.divide(house_reb_dem_tot_per_event, tot_rebuilding_demand_summed, where=(tot_rebuilding_demand_summed!=0))
-            #logger.debug("indus_shares: {}".format(indus_shares))
-            assert np.allclose(indus_shares + house_shares,np.ones(shape=indus_shares.shape))
+            logger.debug(
+                "There are both household rebuilding demand and industry rebuilding demand"
+            )
+            logger.debug(
+                f"indus_reb_dem_tot_per_event: {pd.DataFrame(indus_reb_dem_tot_per_event, index=self.industries)}"
+            )
+            logger.debug(
+                f"house_reb_dem_tot_per_event: {pd.DataFrame(house_reb_dem_tot_per_event, index=self.industries)}"
+            )
+            logger.debug(
+                f"dem_tot_per_event: {pd.DataFrame(house_reb_dem_tot_per_event+indus_reb_dem_tot_per_event, index=self.industries)}"  # type: ignore
+            )
+
+            tot_reb_dem_divider = np.tile(
+                tot_rebuilding_demand_summed[:, np.newaxis],
+                (1, indus_reb_dem_tot_per_event.shape[1]),
+            )
+            indus_shares = np.divide(
+                indus_reb_dem_tot_per_event,
+                tot_reb_dem_divider,
+                out=np.zeros_like(indus_reb_dem_tot_per_event),
+                where=tot_reb_dem_divider != 0,
+            )
+            house_shares = np.divide(
+                house_reb_dem_tot_per_event,
+                tot_reb_dem_divider,
+                out=np.zeros_like(house_reb_dem_tot_per_event),
+                where=tot_reb_dem_divider != 0,
+            )
+            # np.around(house_shares, 6, out=house_shares)
+            # np.around(indus_shares, 6, out=indus_shares)
+            logger.debug(
+                f"indus_shares: {pd.DataFrame(indus_shares, index=self.industries)}"
+            )
+            logger.debug(
+                f"house_shares: {pd.DataFrame(house_shares, index=self.industries)}"
+            )
+
+            #             tot_reb = pd.Series(tot_rebuilding_demand_summed, index=self.industries)
+            #             indus_reb_dem_tot = pd.DataFrame(indus_reb_dem_tot_per_event, index=self.industries)[0]
+            #             house_reb_dem_tot = pd.DataFrame(house_reb_dem_tot_per_event, index=self.industries)[0]
+            #             np.around(indus_shares,10,indus_shares)
+            #             np.around(house_shares,10,house_shares)
+            #             np.around(tmp,10,tmp)
+            #             indus_df = pd.DataFrame(indus_shares,index=self.industries)[0]
+            #             house_df = pd.DataFrame(house_shares,index=self.industries)[0]
+            #             tmp_df=pd.DataFrame(tmp, index=self.industries)[0]
+
+            #             debug_df = pd.concat([tot_reb, indus_reb_dem_tot, house_reb_dem_tot, tot_reb-(house_reb_dem_tot+indus_reb_dem_tot), indus_df, house_df, tmp_df], axis=1)
+            #             #logger.info(debug_df[debug_df.iloc[:,6]!=0].to_string())
+            #             debug_str = f"""
+            # {debug_df[debug_df.iloc[:,6]!=0].to_string()}
+            # """
+            assert np.allclose(
+                (indus_shares + house_shares)[tot_rebuilding_demand_summed != 0], 1.0
+            )
+
         elif h_reb:
             house_shares = np.ones(house_reb_dem_tot_per_event.shape)
             indus_shares = np.zeros(indus_reb_dem_tot_per_event.shape)
         elif ind_reb:
             house_shares = np.zeros(house_reb_dem_tot_per_event.shape)
             indus_shares = np.ones(indus_reb_dem_tot_per_event.shape)
-            #logger.debug("indus_shares: {}".format(indus_shares.shape))
+            # logger.debug("indus_shares: {}".format(indus_shares.shape))
         else:
             return []
 
-        indus_rebuild_prod = rebuild_prod[:,np.newaxis] * indus_shares #type:ignore
-        house_rebuild_prod = rebuild_prod[:,np.newaxis] * house_shares #type:ignore
+        logger.debug(f"rebuild_prod: {rebuild_prod}")
+        logger.debug(f"indus_shares: {indus_shares}")
+
+        indus_rebuild_prod = rebuild_prod[:, np.newaxis] * indus_shares  # type:ignore
+        house_rebuild_prod = rebuild_prod[:, np.newaxis] * house_shares  # type:ignore
+
+        if ind_reb:
+            logger.debug(
+                f"indus_rebuild_prod: {pd.DataFrame(indus_rebuild_prod, index=self.industries)}"
+            )
+        if h_reb:
+            logger.debug(
+                f"house_rebuild_prod: {pd.DataFrame(house_rebuild_prod, index=self.industries)}"
+            )
+            # logger.debug(f"tot_rebuilding_demand_summed: {pd.DataFrame(tot_rebuilding_demand_summed, index=self.industries)}")
+        # logger.debug(f"house_rebuild_prod: {pd.Series(house_rebuild_prod.flatten(), index=self.industries)}")
 
         indus_rebuild_prod_distributed = np.zeros(shape=indus_reb_dem_per_event.shape)
         house_rebuild_prod_distributed = np.zeros(shape=house_reb_dem_per_event.shape)
         if ind_reb:
             # 1. We normalize rebuilding demand by total rebuilding demand (i.e. we get for each client asking, the share of the total demand)
             # This is done by broadcasting total demand and then dividing. (Perhaps this is not efficient ?)
-            indus_rebuilding_demand_shares = np.zeros(shape=indus_reb_dem_per_event.shape)
-            indus_rebuilding_demand_broad = np.broadcast_to(indus_reb_dem_tot_per_event[:,np.newaxis],indus_reb_dem_per_event.shape)
-            np.divide(indus_reb_dem_per_event,indus_rebuilding_demand_broad, where=(indus_rebuilding_demand_broad!=0), out=indus_rebuilding_demand_shares)
+            indus_rebuilding_demand_shares = np.zeros(
+                shape=indus_reb_dem_per_event.shape
+            )
+            indus_rebuilding_demand_broad = np.broadcast_to(
+                indus_reb_dem_tot_per_event[:, np.newaxis],
+                indus_reb_dem_per_event.shape,
+            )
+            np.divide(
+                indus_reb_dem_per_event,
+                indus_rebuilding_demand_broad,
+                where=(indus_rebuilding_demand_broad != 0),
+                out=indus_rebuilding_demand_shares,
+            )
 
             # 2. Then we multiply those shares by the total production (each client get production proportional to its demand relative to total demand)
-            indus_rebuild_prod_broad = np.broadcast_to(indus_rebuild_prod[:,np.newaxis],indus_reb_dem_per_event.shape)
-            np.multiply(indus_rebuilding_demand_shares,indus_rebuild_prod_broad,out=indus_rebuild_prod_distributed)
+            indus_rebuild_prod_broad = np.broadcast_to(
+                indus_rebuild_prod[:, np.newaxis], indus_reb_dem_per_event.shape
+            )
+            np.multiply(
+                indus_rebuilding_demand_shares,
+                indus_rebuild_prod_broad,
+                out=indus_rebuild_prod_distributed,
+            )
 
         if h_reb:
-            house_rebuilding_demand_shares = np.zeros(shape=indus_reb_dem_per_event.shape)
-            house_rebuilding_demand_broad = np.broadcast_to(house_reb_dem_tot_per_event[:,np.newaxis],house_reb_dem_per_event.shape)
-            np.divide(house_reb_dem_per_event,house_rebuilding_demand_broad, where=(house_rebuilding_demand_broad!=0), out=house_rebuilding_demand_shares)
-            house_rebuild_prod_broad = np.broadcast_to(house_rebuild_prod[:,np.newaxis],house_reb_dem_per_event.shape)
-            np.multiply(house_rebuilding_demand_shares,house_rebuild_prod_broad,out=house_rebuild_prod_distributed)
+            house_rebuilding_demand_shares = np.zeros(
+                shape=house_reb_dem_per_event.shape
+            )
+            house_rebuilding_demand_broad = np.broadcast_to(
+                house_reb_dem_tot_per_event[:, np.newaxis],
+                house_reb_dem_per_event.shape,
+            )
+            np.divide(
+                house_reb_dem_per_event,
+                house_rebuilding_demand_broad,
+                where=(house_rebuilding_demand_broad != 0),
+                out=house_rebuilding_demand_shares,
+            )
+            house_rebuild_prod_broad = np.broadcast_to(
+                house_rebuild_prod[:, np.newaxis], house_reb_dem_per_event.shape
+            )
+            np.multiply(
+                house_rebuilding_demand_shares,
+                house_rebuild_prod_broad,
+                out=house_rebuild_prod_distributed,
+            )
 
         # update rebuilding demand
         events_to_remove = []
-        for e_id, e in enumerate(rebuildable_events):
-            if e.rebuilding_demand_indus is not None:
-                e.rebuilding_demand_indus -= indus_rebuild_prod_distributed[:,:,e_id]
-            if e.rebuilding_demand_house is not None:
-                e.rebuilding_demand_house -= house_rebuild_prod_distributed[:,:,e_id]
-            if (e.rebuilding_demand_indus < (10/self.monetary_unit)).all() and (e.rebuilding_demand_house < (10/self.monetary_unit)).all():
-                events_to_remove.append(e)
+        for e_id, evnt in enumerate(rebuildable_events):
+            if len(evnt.rebuilding_demand_indus) > 0:
+                evnt.rebuilding_demand_indus -= indus_rebuild_prod_distributed[
+                    :, :, e_id
+                ]
+            if len(evnt.rebuilding_demand_house) > 0:
+                evnt.rebuilding_demand_house -= house_rebuild_prod_distributed[
+                    :, :, e_id
+                ]
+            if (evnt.rebuilding_demand_indus < (10 / self.monetary_factor)).all() and (
+                evnt.rebuilding_demand_house < (10 / self.monetary_factor)
+            ).all():
+                events_to_remove.append(evnt)
         return events_to_remove
 
-    def calc_matrix_stock_gap(self, matrix_stock_goal) -> np.ndarray:
+    def calc_matrix_stock_gap(self, matrix_stock_goal) -> npt.NDArray:
+        """Computes and returns inputs stock gap matrix
+
+        The gap is simply the difference between the goal (given as argument)
+        and the current stock.
+
+        Parameters
+        ----------
+        matrix_stock_goal : npt.NDArray of float
+            The target inventories.
+
+        Returns
+        -------
+        npt.NDArray
+            The (only positive) gap between goal and current inventories.
+
+        Raises
+        ------
+        RuntimeError
+            If NaN are found in the result.
+
+        """
         matrix_stock_gap = np.zeros(matrix_stock_goal.shape)
         # logger.debug("matrix_stock_goal: {}".format(matrix_stock_goal.shape))
         # logger.debug("matrix_stock: {}".format(self.matrix_stock.shape))
         # logger.debug("matrix_stock_goal_finite: {}".format(matrix_stock_goal[np.isfinite(matrix_stock_goal)].shape))
         # logger.debug("matrix_stock_finite: {}".format(self.matrix_stock[np.isfinite(self.matrix_stock)].shape))
-        matrix_stock_gap[np.isfinite(matrix_stock_goal)] = (matrix_stock_goal[np.isfinite(matrix_stock_goal)] - self.matrix_stock[np.isfinite(self.matrix_stock)])
-        if (np.isnan(matrix_stock_gap).any()):
+        matrix_stock_gap[np.isfinite(matrix_stock_goal)] = (
+            matrix_stock_goal[np.isfinite(matrix_stock_goal)]
+            - self.matrix_stock[np.isfinite(self.matrix_stock)]
+        )
+        if np.isnan(matrix_stock_gap).any():
             raise RuntimeError("NaN in matrix stock gap")
         matrix_stock_gap[matrix_stock_gap < 0] = 0
         return matrix_stock_gap
 
-
     def calc_orders(self) -> None:
-        """TODO describe function
+        r"""Computes and sets the orders (intermediate demand) for the next step.
 
-        :param stocks_constraints:
-        :type stocks_constraints:
-        :returns:
+        See :ref:`Order module <boario-math-orders>`
 
+        Raises
+        ------
+        RuntimeError
+            If negative orders are found, which shouldn't happen.
         """
-        #total_demand = self.total_demand
+
+        # total_demand = self.total_demand
         production_opt = self.production_opt.copy()
         matrix_stock_goal = np.tile(production_opt, (self.n_sectors, 1)) * self.tech_mat
         # Check this !
-        with np.errstate(invalid='ignore'):
-            matrix_stock_goal *= self.inv_duration[:,np.newaxis]
+        with np.errstate(invalid="ignore"):
+            matrix_stock_goal *= self.inv_duration[:, np.newaxis]
         if np.allclose(self.matrix_stock, matrix_stock_goal):
-            matrix_stock_gap = matrix_stock_goal * 0
+            matrix_stock_gap = np.zeros(matrix_stock_goal.shape)
         else:
             matrix_stock_gap = self.calc_matrix_stock_gap(matrix_stock_goal)
-        matrix_stock_gap += (np.tile(self.production, (self.n_sectors, 1)) * self.tech_mat)
+        matrix_stock_gap += (
+            np.tile(self.production, (self.n_sectors, 1)) * self.tech_mat
+        )
         if self.order_type == "alt":
             prod_ratio = np.ones(shape=self.X_0.shape)
-            np.divide(self.production,self.X_0, out=prod_ratio, where=self.X_0!=0)
+            np.divide(
+                self.production_cap, self.X_0, out=prod_ratio, where=self.X_0 != 0
+            )
             Z_prod = self.Z_0 * prod_ratio[:, np.newaxis]
-            Z_Cprod = np.tile(self._matrix_I_sum @ Z_prod,(self.n_regions,1))
-            out=np.zeros(shape=Z_prod.shape)
-            np.divide(Z_prod,Z_Cprod,out=out, where=Z_Cprod!=0)
-            tmp = (np.tile(matrix_stock_gap, (self.n_regions, 1)) * out)
+            Z_Cprod = np.tile(self._matrix_I_sum @ Z_prod, (self.n_regions, 1))
+            out = np.zeros(shape=Z_prod.shape)
+            np.divide(Z_prod, Z_Cprod, out=out, where=Z_Cprod != 0)
+            tmp = np.tile(matrix_stock_gap, (self.n_regions, 1)) * out
         else:
-            tmp = (np.tile(matrix_stock_gap, (self.n_regions, 1)) * self.Z_distrib)
+            tmp = np.tile(matrix_stock_gap, (self.n_regions, 1)) * self.Z_distrib
         if (tmp < 0).any():
             raise RuntimeError("Negative orders computed")
         self.matrix_orders = tmp
 
-
     def calc_overproduction(self) -> None:
+        r"""Computes and updates the overproduction vector.
+
+        See :ref:`Overproduction module <boario-math-overprod>`
+
+        """
+
         scarcity = np.full(self.production.shape, 0.0)
         total_demand = self.total_demand.copy()
-        scarcity[total_demand!=0] = (total_demand[total_demand!=0] - self.production[total_demand!=0]) / total_demand[total_demand!=0]
+        scarcity[total_demand != 0] = (
+            total_demand[total_demand != 0] - self.production[total_demand != 0]
+        ) / total_demand[total_demand != 0]
         scarcity[np.isnan(scarcity)] = 0
-        overprod_chg = (((self.overprod_max - self.overprod) * (scarcity) * self.overprod_tau) + ((self.overprod_base - self.overprod) * (scarcity == 0) * self.overprod_tau)).flatten()
+        overprod_chg = (
+            ((self.overprod_max - self.overprod) * scarcity * self.overprod_tau)
+            + (
+                (self.overprod_base - self.overprod)
+                * (scarcity == 0)
+                * self.overprod_tau
+            )
+        ).flatten()
         self.overprod += overprod_chg
-        self.overprod[self.overprod < 1.] = 1.
-
-    def check_stock_increasing(self, current_temporal_unit:int):
-        tmp = np.full(self.matrix_stock.shape,0.0)
-        mask = np.isfinite(self.matrix_stock_0)
-        np.subtract(self.matrix_stock,self.matrix_stock_0, out=tmp, where=mask)
-        check_1 = tmp > 0.0
-        tmp = np.full(self.matrix_stock.shape,0.0)
-        np.subtract(self.stocks_evolution[current_temporal_unit], self.stocks_evolution[current_temporal_unit-1], out=tmp, where=mask)
-        check_2 = (tmp >= 0.0)
-        return (check_1 & check_2).all()
-
-    def check_production_eq_strict(self):
-        return ((np.isclose(self.production, self.X_0)) | np.greater(self.production, self.X_0)).all()
-
-    def check_production_eq_soft(self, current_temporal_unit:int, period:int = 10) -> bool:
-        return self.check_monotony(self.production_evolution, current_temporal_unit, period)
-
-    def check_stocks_monotony(self, current_temporal_unit:int, period:int = 10) -> bool:
-        return self.check_monotony(self.stocks_evolution, current_temporal_unit, period)
-
-    def check_initial_equilibrium(self)-> bool:
-        return (np.allclose(self.production, self.X_0) and np.allclose(self.matrix_stock, self.matrix_stock_0))
-
-    def check_equilibrium_soft(self, current_temporal_unit:int):
-        return (self.check_stock_increasing(current_temporal_unit) and self.check_production_eq_strict)
-
-    def check_equilibrium_monotony(self, current_temporal_unit:int, period:int=10) -> bool:
-        return self.check_production_eq_soft(current_temporal_unit, period) and self.check_stocks_monotony(current_temporal_unit, period)
-
-    def check_monotony(self, x, current_temporal_unit:int, period:int = 10) -> bool:
-        return np.allclose(x[current_temporal_unit], x[current_temporal_unit-period], atol=0.0001)
-
-    def check_crash(self, prod_threshold : float=0.80) -> int:
-        """Check for economic crash
-
-        This method look at the production vector and returns the number of
-        industries which production is less than a certain share (default 20%) of the starting
-        production.
-
-        Parameters
-        ----------
-        prod_threshold : float, default: 0.8
-            An industry is counted as 'crashed' if its current production is less than its starting production times (1 - `prod_threshold`).
+        self.overprod[self.overprod < 1.0] = 1.0
 
+    def reset_module(
+        self,
+    ) -> None:
+        """Resets the model to initial state [Deprecated]
 
+        This method has not been checked extensively.
         """
-        tmp = np.full(self.production.shape, 0.0)
-        checker = np.full(self.production.shape, 0.0)
-        mask = self.X_0 != 0
-        np.subtract(self.X_0, self.production, out=tmp, where=mask)
-        np.divide(tmp, self.X_0, out=checker, where=mask)
-        return np.where(checker >= prod_threshold)[0].size
-
-    def reset_module(self,
-                 simulation_params: dict,
-                 ) -> None:
-        # Reset OUTPUTS
-        logger.warning("This method is quite probably deprecated")
-        self.reset_record_files(simulation_params['n_temporal_units_to_sim'], simulation_params['register_stocks'])
-        # Reset variable attributes
-        self.kapital_lost = np.zeros(self.production.shape)
-        self.overprod = np.full((self.n_regions * self.n_sectors), self.overprod_base, dtype=np.float64)
-        with np.errstate(divide='ignore',invalid='ignore'):
-            self.matrix_stock = ((np.tile(self.X_0, (self.n_sectors, 1)) * self.tech_mat) * self.inv_duration[:,np.newaxis])
-        self.matrix_stock = np.nan_to_num(self.matrix_stock,nan=np.inf, posinf=np.inf)
-        self.matrix_stock_0 = self.matrix_stock.copy()
+
+        self.productive_capital_lost = np.zeros(self.production.shape)
+        self.overprod = np.full(
+            (self.n_regions * self.n_sectors), self.overprod_base, dtype=np.float64
+        )
+        self.matrix_stock = self.matrix_stock_0.copy()
         self.matrix_orders = self.Z_0.copy()
         self.production = self.X_0.copy()
         self.intmd_demand = self.Z_0.copy()
         self.final_demand = self.Y_0.copy()
-        self.rebuilding_demand = None
-        self.prod_max_toward_rebuilding = None
-
-    def update_params(self, new_params:dict) -> None:
-        """Update the parameters of the model.
-
-        Replace each parameters with given new ones.
-
-        .. warning::
-            Be aware this method calls :meth:`~boario.model_base.reset_record_files`, which resets the memmap files located in the results directory !
-
-        Parameters
-        ----------
-        new_params : dict
-            Dictionary of new parameters to use.
-
-        """
-        logger.warning("This method is quite probably deprecated")
-        self.n_temporal_units_by_step = new_params['temporal_units_by_step']
-        self.iotable_year_to_temporal_unit_factor = new_params['year_to_temporal_unit_factor']
-        self.rebuild_tau = new_params['rebuild_tau']
-        self.overprod_max = new_params['alpha_max']
-        self.overprod_tau = new_params['alpha_tau']
-        self.overprod_base = new_params['alpha_base']
-        if self.records_storage != pathlib.Path(new_params['output_dir']+"/"+new_params['results_storage']):
-            self.records_storage = pathlib.Path(new_params['output_dir']+"/"+new_params['results_storage'])
-        self.reset_record_files(new_params['n_temporal_units_to_sim'], new_params['register_stocks'])
-
-    def reset_record_files(self, n_temporal_units:int, reg_stocks: bool) -> None:
-        """Reset results memmaps
-
-        This method creates/resets the :class:`memmaps <numpy.memmap>` arrays used to track
-        production, demand, overproduction, etc.
-
-        Parameters
-        ----------
-        n_steps : int
-            number of steps of the simulation (memmaps size are predefined)
-        reg_stocks : bool
-            If true, create/reset the stock memmap (which can be huge)
-
-        """
-        self.production_evolution = np.memmap(self.records_storage/"iotable_XVA_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.production_evolution.fill(np.nan)
-        self.production_cap_evolution = np.memmap(self.records_storage/"iotable_X_max_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.production_cap_evolution.fill(np.nan)
-        self.io_demand_evolution = np.memmap(self.records_storage/"io_demand_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.io_demand_evolution.fill(np.nan)
-        self.final_demand_evolution = np.memmap(self.records_storage/"final_demand_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.final_demand_evolution.fill(np.nan)
-        self.rebuild_demand_evolution = np.memmap(self.records_storage/"rebuild_demand_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.rebuild_demand_evolution.fill(np.nan)
-        self.overproduction_evolution = np.memmap(self.records_storage/"overprodvector_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.overproduction_evolution.fill(np.nan)
-        self.final_demand_unmet_evolution = np.memmap(self.records_storage/"final_demand_unmet_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.final_demand_unmet_evolution.fill(np.nan)
-        self.rebuild_production_evolution = np.memmap(self.records_storage/"rebuild_prod_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.rebuild_production_evolution.fill(np.nan)
-        if reg_stocks:
-            self.stocks_evolution = np.memmap(self.records_storage/"stocks_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors, self.n_sectors*self.n_regions))
-            self.stocks_evolution.fill(np.nan)
-        self.limiting_stocks_evolution = np.memmap(self.records_storage/"limiting_stocks_record", dtype='byte', mode="w+", shape=(n_temporal_units, self.n_sectors, self.n_sectors*self.n_regions))
-        self.limiting_stocks_evolution.fill(-1)
-        self.regional_sectoral_kapital_destroyed_evol = np.memmap(self.records_storage/"iotable_kapital_destroyed_record", dtype='float64', mode="w+", shape=(n_temporal_units, self.n_sectors*self.n_regions))
-        self.regional_sectoral_kapital_destroyed_evol.fill(np.nan)
-
-
-    def write_production(self, current_temporal_unit:int) -> None:
-        self.production_evolution[current_temporal_unit] = self.production
-
-    def write_kapital_lost(self, current_temporal_unit:int) -> None:
-        self.regional_sectoral_kapital_destroyed_evol[current_temporal_unit] = self._kapital_lost
-
-    def write_production_max(self, current_temporal_unit:int) -> None:
-        self.production_cap_evolution[current_temporal_unit] = self.production_cap
-
-    def write_io_demand(self, current_temporal_unit:int) -> None:
-         self.io_demand_evolution[current_temporal_unit] = self.matrix_orders.sum(axis=1)
-
-    def write_final_demand(self, current_temporal_unit:int) -> None:
-         self.final_demand_evolution[current_temporal_unit] = self.final_demand.sum(axis=1)
-
-    def write_rebuild_demand(self, current_temporal_unit:int) -> None:
-        to_write = np.full(self.n_regions*self.n_sectors,0.0)
-        if (r_dem := self.tot_rebuild_demand) is not None:
-            self.rebuild_demand_evolution[current_temporal_unit] = r_dem
-        else:
-            self.rebuild_demand_evolution[current_temporal_unit] = to_write
-
-    def write_rebuild_prod(self, current_temporal_unit:int, rebuild_prod_agg:np.ndarray) -> None:
-        self.rebuild_production_evolution[current_temporal_unit] = rebuild_prod_agg
-
-    def write_overproduction(self, current_temporal_unit:int) -> None:
-        self.overproduction_evolution[current_temporal_unit] = self.overprod
-
-    def write_final_demand_unmet(self, current_temporal_unit:int, final_demand_unmet:np.ndarray) -> None:
-        self.final_demand_unmet_evolution[current_temporal_unit] = final_demand_unmet
-
-    def write_stocks(self, current_temporal_unit:int) -> None:
-        self.stocks_evolution[current_temporal_unit] = self.matrix_stock
-
-    def write_limiting_stocks(self, current_temporal_unit:int,
-                              limiting_stock:np.ndarray) -> None:
-        self.limiting_stocks_evolution[current_temporal_unit] = limiting_stock
+        self.final_demand_not_met = np.zeros(self.Y_0.shape)
+        self.rebuilding_demand = np.array([])
+        self.in_shortage = False
+        self.had_shortage = False
+        self._prod_delta_type = None
+        self._indus_rebuild_demand_tot = np.array([])
+        self._house_rebuild_demand_tot = np.array([])
+        self._indus_rebuild_demand = np.array([])
+        self._house_rebuild_demand = np.array([])
+        self._tot_rebuild_demand = np.array([])
+        self._prod_cap_delta_productive_capital = np.array([])
+        self._prod_cap_delta_arbitrary = np.array([])
+        self._prod_cap_delta_tot = np.array([])
 
-    def write_index(self, index_file:str|pathlib.Path) -> None:
+    def write_index(self, index_file: str | pathlib.Path) -> None:
         """Write the indexes of the different dataframes of the model in a json file.
 
         In order to easily rebuild the dataframes from the 'raw' data, this
         method create a JSON file with all columns and indexes names, namely :
 
         * regions names
         * sectors names
@@ -1138,28 +1568,38 @@
 
         Parameters
         ----------
         index_file : pathlib.Path
             Path to the file to save the indexes.
         """
 
-        indexes= {
-            "regions":list(self.regions),
-            "sectors":list(self.sectors),
-            "fd_cat":list(self.fd_cat),
-            "n_sectors":self.n_sectors,
-            "n_regions":self.n_regions,
-            "n_industries":self.n_sectors*self.n_regions
+        indexes = {
+            "regions": list(self.regions),
+            "sectors": list(self.sectors),
+            "fd_cat": list(self.final_demand_cat),
+            "n_sectors": self.n_sectors,
+            "n_regions": self.n_regions,
+            "n_industries": self.n_sectors * self.n_regions,
         }
-        if isinstance(index_file,str):
-            index_file=pathlib.Path(index_file)
+        if isinstance(index_file, str):
+            index_file = pathlib.Path(index_file)
         index_file.parent.mkdir(parents=True, exist_ok=True)
-        with index_file.open('w') as f:
-            json.dump(indexes,f)
+        with index_file.open("w") as ffile:
+            json.dump(indexes, ffile)
 
-    def change_inv_duration(self, new_dur:int, old_dur:Optional[int]=None) -> None:
+    def change_inv_duration(self, new_dur, old_dur=None) -> None:
+        # replace this method by a property !
         if old_dur is None:
             old_dur = self.main_inv_dur
         old_dur = float(old_dur) / self.n_temporal_units_by_step
         new_dur = float(new_dur) / self.n_temporal_units_by_step
-        logger.info("Changing (main) inventories duration from {} steps to {} steps (there are {} temporal units by step so duration is {})".format(old_dur, new_dur, self.n_temporal_units_by_step, new_dur*self.n_temporal_units_by_step))
-        self.inv_duration = np.where(self.inv_duration==old_dur, new_dur, self.inv_duration)
+        logger.info(
+            "Changing (main) inventories duration from {} steps to {} steps (there are {} temporal units by step so duration is {})".format(
+                old_dur,
+                new_dur,
+                self.n_temporal_units_by_step,
+                new_dur * self.n_temporal_units_by_step,
+            )
+        )
+        self.inv_duration = np.where(
+            self.inv_duration == old_dur, new_dur, self.inv_duration
+        )
```

### Comparing `boario-0.4.1b0/LICENSE` & `boario-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `boario-0.4.1b0/README.rst` & `boario-0.5.0a0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 #######
 BoARIO
 #######
 
 BoARIO : The Adaptative Regional Input Output model in python.
 
+.. _`Documentation Website`: https://spjuhel.github.io/BoARIO/boario-what-is.html
+
+Disclaimer
+===========
+
+This work is in progress. The code has not been extensively tested. Any results produced with the model should be interpreted with great care.
+Do not hesitate to contact the author when using the model !
+
 What is BoARIO ?
 =================
 
 BoARIO, is a python implementation project of the Adaptative Regional Input Output (ARIO) model [`Hallegatte 2013`_].
 
 Its objectives are to give an accessible and inter-operable implementation of ARIO, as well as tools to visualize and analyze simulation outputs and to
 evaluate the effects of many parameters of the model.
@@ -19,59 +27,67 @@
 
 It is still an ongoing project (in parallel of a PhD project).
 
 .. _`Stadler 2021`: https://openresearchsoftware.metajnl.com/articles/10.5334/jors.251/
 .. _`Hallegatte 2013`: https://doi.org/10.1111/j.1539-6924.2008.01046.x
 .. _`Pymrio`: https://pymrio.readthedocs.io/en/latest/intro.html
 
-Here is a non-exhaustive chronology of academic works with or about the ARIO model :
+You can find most academic literature using ARIO or related models `here <https://spjuhel.github.io/BoARIO/boario-references.html>`_
 
-.. image:: https://raw.githubusercontent.com/spjuhel/BoARIO/master/imgs/chronology.svg?sanitize=true
-           :width: 900
-           :alt: ADEME Logo
 
-Where to get it ?
-===================
+What is ARIO ?
+===============
+
+ARIO stands for Adaptive Regional Input-Output. It is an hybrid input-output / agent-based economic model,
+designed to compute indirect costs from economic shocks. Its first version dates back to 2008 and has originally
+been developed to assess the indirect costs of natural disasters (Hallegatte 2008).
+
+In ARIO, the economy is modelled as a set of economic sectors and a set of regions.
+Each economic sector produces its generic product and draws inputs from an inventory.
+Each sector answers to a total demand consisting of a final demand (household consumption,
+public spending and private investments) of all regions (local demand and exports) and
+intermediate demand (through inputs inventory resupply). An initial equilibrium state of
+the economy is built based on multi-regional input-output tables (MRIO tables).
+
+
+Where to get BoARIO ?
+==========================
 
 You can install BoARIO from ``pip`` with:
 
 .. code:: console
 
    pip install boario
 
 
 The full source code is also available on Github at: https://github.com/spjuhel/BoARIO
 
-More info in the `installation page`_ of the documentation.
-
-.. _installation page: https://spjuhel.github.io/BoARIO/boario-installation.html
+More info in the `installation <https://spjuhel.github.io/BoARIO/boario-installation.html>`_ page of the documentation.
 
 How does BoARIO work?
 =========================
 
 In a nutshell, BoARIO takes the following inputs :
 
-- an IO table (such as EXIOBASE3 or EORA26) in the form of an `IOSystem` object (define by the `pymrio` package)
+- an IO table (such as EXIOBASE3 or EORA26) in the form of an ``pymrio.IOSystem`` object, using the `Pymrio`_ python package.
 
-- simulation and mrio parameters (as json files or dictionaries), which govern the simulation,
+- multiple parameters which govern the simulation,
 
-- event(s) description(s) (as json files or dictionaries), which are used as the perturbation to analyse during the simulation
+- event(s) description(s), which are used as the perturbation to analyse during the simulation
 
-in order to produce the following outputs:
+And produce the following outputs:
 
-- the step by step, sector by sector, region by region evolution of most of the variables involved in the simulation (production, demand, stocks, ...)
+- the step by step, sector by sector, region by region evolution of most of the variables involved in the simulation (`production`, `demand`, `stocks`, ...)
 
-- aggregated indicators for the whole simulation (shortages duration, aggregated impacts, ...)
+- aggregated indicators for the whole simulation (`shortages duration`, `aggregated impacts`, ...)
 
 Example of use
 =================
 
-See `boario-quickstart`_.
-
-.. _boario-quickstart: https://spjuhel.github.io/BoARIO/boario-quickstart.html
+See `Boario quickstart <https://spjuhel.github.io/BoARIO/boario-quickstart.html>`_.
 
 Credits
 ========
 
 Associated PhD project
 ------------------------
 
@@ -84,20 +100,19 @@
            :alt: ADEME Logo
 
 .. _`ADEME`: https://www.ademe.fr/
 
 Development
 ------------
 
-* Samuel Juhel
+* Samuel Juhel (pro@sjuhel.org)
 
 Contributions
 ---------------
 
-* Be the first `contributor`_ !
-
-.. _`contributor`: https://spjuhel.github.io/BoARIO/development.html
+All `contributions <https://spjuhel.github.io/BoARIO/development.html>`_ to the project are welcome !
 
 Acknowledgements
 ------------------
 
-I would like to thank Vincent Viguie, Fabio D'Andrea my PhD supervisors as well as Célian Colon for their inputs during the model implementaiton.
+I would like to thank Vincent Viguie, Fabio D'Andrea my PhD supervisors as well as Célian Colon, Alessio Ciulo and Adrien Delahais
+for their inputs during the model implementation.
```

### Comparing `boario-0.4.1b0/pyproject.toml` & `boario-0.5.0a0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-[build-system]
-requires = [
-    "hatchling>=1.9.0",
-]
-build-backend = "hatchling.build"
-
-[project]
+[tool.poetry]
 name = "boario"
-dynamic = [
-    "version",
-]
-description = "A Python implementation of ARIO models"
+version = "0.5.0a"
+description = "BoARIO : The Adaptative Regional Input Output model in python."
+authors = ["Samuel Juhel <pro@sjuhel.org>"]
+license = "GNU General Public License v3 or later (GPLv3+)"
 readme = "README.rst"
-license = ""
-requires-python = ">=3.7, <4"
-dependencies = [
-"numpy>=1.17.4",
-"dask>=2021.9.0",
-"coloredlogs>=15.0.1",
-"country_converter>=0.7.4",
-"nptyping>=1.4.4",
-"numpyencoder>=0.3.0",
-"pandas>=1.4.1",
-"progressbar2>=2.4",
-"pymrio>=0.4.6",
-"odfpy>=1.4.1",
-"pyarrow>=9.0.0",
-]
 
-authors = [
-    { name = "Samuel JUHEL", email = "pro@sjuhel.org" },
-]
+[tool.poetry.dependencies]
+python=">=3.9"
+coloredlogs = "^15.0.1"
+country-converter = "^1.0.0"
+dask = ">=2023"
+numpy = "<1.24"
+numpyencoder = "^0.3.0"
+odfpy = "^1.4.1"
+pandas = ">=1.5,<2.0"
+progressbar2 = "^4.2.0"
+pyarrow = "^11.0.0"
+pymrio = "^0.4.8"
+
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+pygit2 = "^1.12.1"
+ipykernel = "^6.23.0"
+black = "^23.3.0"
+sphinxcontrib-bibtex = "^2.5.0"
+sphinx-autoapi = "^2.1.0"
+sphinx-automodapi = "^0.15.0"
+sphinx-copybutton = "^0.5.2"
+pydata-sphinx-theme = "^0.13.3"
+nbsphinx = "^0.9.2"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[project]
 keywords = [
     "ario",
     "economics",
     "events",
     "extreme",
     "impact",
     "indirect",
     "input-output",
     "modeling",
     "mrio",
 ]
+name = "boario"
+
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -57,69 +66,23 @@
 
 [project.urls]
 "Bug Reports" = "https://github.com/spjuhel/BoARIO/issues"
 Documentation = "https://spjuhel.github.io/BoARIO/index.html"
 Homepage = "https://github.com/spjuhel/BoARIO"
 Source = "https://github.com/spjuhel/BoARIO/"
 
-[tool.hatch.version]
-path = "boario/__init__.py"
-
-[tool.hatch.build.targets.sdist]
-exclude = [
-    "/.github",
-    "/docs",
-    "/.git",
-    "/imgs",
-    "/src",
-    "/testing",
-    "/.snakemake",
-    "/JupyNotebooks",
-    "/other",
-    "/new_docs",
-    "/pyrightconfig.json",
-    "/DOC_BUILDING_REMINDER",
-    "/launch.json",
-    "/.envrc",
-    "/.gitignore",
-    "/api-examples",
-]
-
-[tool.hatch.build.targets.wheel]
-packages = [
-    "boario",
-]
-
-[[tool.hatch.envs.test.matrix]]
-python = [
-    "37",
-    "38",
-    "39",
-    "310",
-    "311",
-]
-
-[tool.hatch.envs.test]
-python = "3.8"
-
 [tool.pyright]
 include = ["boario","scripts"]
 exclude = ["**/node_modules",
     "**/__pycache__",
     "src/",
-    "api-examples"
+    "api-examples",
+    "docs/",
+    "dist/",
+    "imgs/",
+    "other/",
+    "tests/",
+    "dist/"
 ]
-ignore = ["src/oldstuff"]
-defineConstant = { DEBUG = true }
-stubPath = "boario/stubs"
-pythonPath = "/home/sjuhel/mambaforge-pypy3/envs/boario-dev/bin/python"
-venvPath = "/home/sjuhel/mambaforge-pypy3/envs/boario-dev/"
-
-reportMissingImports = true
-reportMissingTypeStubs = false
 
-pythonVersion = "3.8"
-pythonPlatform = "Linux"
-
-executionEnvironments = [
-  { root = "src" }
-]
+defineConstant = { DEBUG = true }
+stubPath = "boario/stubs"
```

