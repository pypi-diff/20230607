# Comparing `tmp/sdv-1.2.0.dev0.tar.gz` & `tmp/sdv-1.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdv-1.2.0.dev0.tar", last modified: Tue Jun  6 20:53:32 2023, max compression
+gzip compressed data, was "sdv-1.2.0.dev1.tar", last modified: Wed Jun  7 18:57:18 2023, max compression
```

## Comparing `sdv-1.2.0.dev0.tar` & `sdv-1.2.0.dev1.tar`

### file list

```diff
@@ -1,657 +1,657 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.073773 sdv-1.2.0.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.2.0.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8110 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67391 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.2.0.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    78227 2023-06-06 20:53:32.074042 sdv-1.2.0.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9801 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.945238 sdv-1.2.0.dev0/docs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/Makefile
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.946083 sdv-1.2.0.dev0/docs/api_reference/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.946624 sdv-1.2.0.dev0/docs/api_reference/constraints/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.966401 sdv-1.2.0.dev0/docs/api_reference/constraints/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/base.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/api_reference/constraints/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/evaluation.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/api_reference/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.966950 sdv-1.2.0.dev0/docs/api_reference/lite/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.968863 sdv-1.2.0.dev0/docs/api_reference/lite/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/api_reference/lite/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/api_reference/lite/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.969757 sdv-1.2.0.dev0/docs/api_reference/metadata/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.979028 sdv-1.2.0.dev0/docs/api_reference/metadata/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/dataset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/metadata/table.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.980265 sdv-1.2.0.dev0/docs/api_reference/metrics/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.017914 sdv-1.2.0.dev0/docs/api_reference/metrics/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/demos.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/relational.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.2.0.dev0/docs/api_reference/metrics/timeseries.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.018487 sdv-1.2.0.dev0/docs/api_reference/relational/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.019604 sdv-1.2.0.dev0/docs/api_reference/relational/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/relational/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.020018 sdv-1.2.0.dev0/docs/api_reference/sampling/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.020642 sdv-1.2.0.dev0/docs/api_reference/sampling/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/sampling/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/sampling/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/sdv.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.021721 sdv-1.2.0.dev0/docs/api_reference/tabular/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.029773 sdv-1.2.0.dev0/docs/api_reference/tabular/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/copulas.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/tabular/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.030140 sdv-1.2.0.dev0/docs/api_reference/timeseries/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.031362 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/api_reference/timeseries/par.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6934 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/conf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.031874 sdv-1.2.0.dev0/docs/developer_guides/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8613 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/docs/developer_guides/contributing.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/developer_guides/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/developer_guides/overview.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.032723 sdv-1.2.0.dev0/docs/developer_guides/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/developer_guides/sdv/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/developer_guides/sdv/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/developer_guides/sdv/metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.2.0.dev0/docs/developer_guides/sdv/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.033384 sdv-1.2.0.dev0/docs/getting_started/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/getting_started/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2557 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/getting_started/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/getting_started/quickstart.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/history.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.044170 sdv-1.2.0.dev0/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/CTGAN-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/Copulas-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/DataCebo-Blue.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.2.0.dev0/docs/images/DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/DeepEcho-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/RDT-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/images/Real-vs-Synthetic-Evaluation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/SDGym-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/SDMetrics-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22394 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/SDV-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    64162 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/images/SDV-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/SDV.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/images/Single-Table-Metadata-Example.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/images/custom_constraint.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/images/datacebo-logo-dark-mode.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/images/datacebo-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/google_colab.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.0.dev0/docs/images/hma1_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.2.0.dev0/docs/images/metadata_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.2.0.dev0/docs/images/metadata_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/mybinder.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.0.dev0/docs/images/quickstart_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.2.0.dev0/docs/images/rdt_main_tranformation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/images/slack.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6075 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/docs/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/make.bat
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.045994 sdv-1.2.0.dev0/docs/savefig/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.2.0.dev0/docs/savefig/copulagan_experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.2.0.dev0/docs/savefig/copulagan_experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.2.0.dev0/docs/savefig/copulagan_experience_years_3.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.2.0.dev0/docs/savefig/experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.2.0.dev0/docs/savefig/experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.2.0.dev0/docs/savefig/experience_years_3.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:31.937907 sdv-1.2.0.dev0/docs/sdv_theme/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.046270 sdv-1.2.0.dev0/docs/sdv_theme/static/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/sdv_theme/static/slack-32.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.046530 sdv-1.2.0.dev0/docs/user_guides/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.047868 sdv-1.2.0.dev0/docs/user_guides/benchmarking/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/benchmarking/datasets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1885 2023-02-02 20:58:41.000000 sdv-1.2.0.dev0/docs/user_guides/benchmarking/docker.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/benchmarking/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2562 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/benchmarking/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/benchmarking/run.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/benchmarking/synthesizers.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.048659 sdv-1.2.0.dev0/docs/user_guides/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.2.0.dev0/docs/user_guides/evaluation/evaluation_framework.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.2.0.dev0/docs/user_guides/evaluation/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.2.0.dev0/docs/user_guides/evaluation/synthetic_data_metrics.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.049704 sdv-1.2.0.dev0/docs/user_guides/relational/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/relational/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/relational/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.2.0.dev0/docs/user_guides/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/relational/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/relational/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/relational/relational_metadata.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.053008 sdv-1.2.0.dev0/docs/user_guides/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/custom_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/gaussian_copula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/handling_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/table_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/tabular_preset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.2.0.dev0/docs/user_guides/single_table/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.053596 sdv-1.2.0.dev0/docs/user_guides/timeseries/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/docs/user_guides/timeseries/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.2.0.dev0/docs/user_guides/timeseries/par.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.054120 sdv-1.2.0.dev0/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2023-06-06 20:53:11.000000 sdv-1.2.0.dev0/sdv/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.055954 sdv-1.2.0.dev0/sdv/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/sdv/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18019 2023-04-20 22:38:57.000000 sdv-1.2.0.dev0/sdv/constraints/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      799 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/constraints/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    53574 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/sdv/constraints/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5822 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/sdv/constraints/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.056898 sdv-1.2.0.dev0/sdv/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    34794 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/sdv/data_processing/data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.2.0.dev0/sdv/data_processing/datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/data_processing/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/data_processing/numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/data_processing/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.057368 sdv-1.2.0.dev0/sdv/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6625 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/datasets/demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1117 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/datasets/local.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      694 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/errors.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.057848 sdv-1.2.0.dev0/sdv/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3701 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/evaluation/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3239 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/evaluation/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.058185 sdv-1.2.0.dev0/sdv/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7153 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/sdv/lite/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.059432 sdv-1.2.0.dev0/sdv/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3060 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/sdv/metadata/anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/metadata/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/metadata/metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29106 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/sdv/metadata/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21941 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/sdv/metadata/single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/metadata/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-04-20 18:31:25.000000 sdv-1.2.0.dev0/sdv/metadata/visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.060195 sdv-1.2.0.dev0/sdv/metrics/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/metrics/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/metrics/demos.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/metrics/relational.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/metrics/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/metrics/timeseries.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.060683 sdv-1.2.0.dev0/sdv/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/sdv/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20699 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/sdv/multi_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    23027 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/sdv/multi_table/hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.061267 sdv-1.2.0.dev0/sdv/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      103 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8638 2023-06-01 02:59:19.000000 sdv-1.2.0.dev0/sdv/sampling/hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5578 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/sdv/sampling/independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/sdv/sampling/tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.061603 sdv-1.2.0.dev0/sdv/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14850 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/sdv/sequential/par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.062725 sdv-1.2.0.dev0/sdv/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/sdv/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45383 2023-06-01 02:59:19.000000 sdv-1.2.0.dev0/sdv/single_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11148 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/sdv/single_table/copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14901 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/sdv/single_table/copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9895 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/sdv/single_table/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      341 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/single_table/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10141 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/sdv/single_table/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5800 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/sdv/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.055097 sdv-1.2.0.dev0/sdv.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    78227 2023-06-06 20:53:31.000000 sdv-1.2.0.dev0/sdv.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35730 2023-06-06 20:53:31.000000 sdv-1.2.0.dev0/sdv.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-06 20:53:31.000000 sdv-1.2.0.dev0/sdv.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-06 20:53:31.000000 sdv-1.2.0.dev0/sdv.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1479 2023-06-06 20:53:31.000000 sdv-1.2.0.dev0/sdv.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-06-06 20:53:31.000000 sdv-1.2.0.dev0/sdv.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2023-06-06 20:53:32.074544 sdv-1.2.0.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3853 2023-06-06 20:53:11.000000 sdv-1.2.0.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.063039 sdv-1.2.0.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.063320 sdv-1.2.0.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.063490 sdv-1.2.0.dev0/tests/integration/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12132 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/integration/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/dataset.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.063793 sdv-1.2.0.dev0/tests/integration/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3324 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/datasets/test_demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.064295 sdv-1.2.0.dev0/tests/integration/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1133 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1131 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.064608 sdv-1.2.0.dev0/tests/integration/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/tests/integration/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.065240 sdv-1.2.0.dev0/tests/integration/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      596 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/integration/metadata/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4369 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6200 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/metadata/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.065521 sdv-1.2.0.dev0/tests/integration/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22620 2023-04-20 18:31:25.000000 sdv-1.2.0.dev0/tests/integration/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.065844 sdv-1.2.0.dev0/tests/integration/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6268 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.066680 sdv-1.2.0.dev0/tests/integration/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/single_table/custom_constraints.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29336 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/tests/integration/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12402 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/tests/integration/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2528 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/integration/single_table/test_ctgan.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.066862 sdv-1.2.0.dev0/tests/readme_test/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.2.0.dev0/tests/readme_test/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.067630 sdv-1.2.0.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.068462 sdv-1.2.0.dev0/tests/unit/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/unit/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    32384 2023-04-20 22:38:57.000000 sdv-1.2.0.dev0/tests/unit/constraints/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   162819 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/tests/unit/constraints/test_tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6700 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/tests/unit/constraints/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.069311 sdv-1.2.0.dev0/tests/unit/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    79588 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/tests/unit/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.2.0.dev0/tests/unit/data_processing/test_datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/data_processing/test_numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/data_processing/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.069736 sdv-1.2.0.dev0/tests/unit/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9876 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/datasets/test_demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2498 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/datasets/test_local.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.070164 sdv-1.2.0.dev0/tests/unit/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2865 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2533 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.070512 sdv-1.2.0.dev0/tests/unit/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/unit/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10135 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/unit/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.071316 sdv-1.2.0.dev0/tests/unit/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/unit/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5258 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/unit/metadata/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/metadata/test_metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    75538 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/tests/unit/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    66306 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/tests/unit/metadata/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.071818 sdv-1.2.0.dev0/tests/unit/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    41567 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/tests/unit/multi_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    28011 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/tests/unit/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.072430 sdv-1.2.0.dev0/tests/unit/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.0.dev0/tests/unit/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13830 2023-06-01 02:59:19.000000 sdv-1.2.0.dev0/tests/unit/sampling/test_hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11155 2023-06-05 19:46:25.000000 sdv-1.2.0.dev0/tests/unit/sampling/test_independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.2.0.dev0/tests/unit/sampling/test_tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.072714 sdv-1.2.0.dev0/tests/unit/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29331 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/unit/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-06 20:53:32.073626 sdv-1.2.0.dev0/tests/unit/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    77568 2023-06-01 02:59:19.000000 sdv-1.2.0.dev0/tests/unit/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13777 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/unit/single_table/test_copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/unit/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10328 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/unit/single_table/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8358 2023-03-28 20:22:54.000000 sdv-1.2.0.dev0/tests/unit/single_table/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-06 20:45:58.000000 sdv-1.2.0.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5572 2023-05-25 15:59:25.000000 sdv-1.2.0.dev0/tests/unit/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.2.0.dev0/tests/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.669325 sdv-1.2.0.dev1/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.2.0.dev1/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8110 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    69753 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.2.0.dev1/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    80589 2023-06-07 18:57:18.669595 sdv-1.2.0.dev1/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9801 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.531666 sdv-1.2.0.dev1/docs/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/Makefile
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.532636 sdv-1.2.0.dev1/docs/api_reference/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.533117 sdv-1.2.0.dev1/docs/api_reference/constraints/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.552514 sdv-1.2.0.dev1/docs/api_reference/constraints/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/base.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/evaluation.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.553017 sdv-1.2.0.dev1/docs/api_reference/lite/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.554771 sdv-1.2.0.dev1/docs/api_reference/lite/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/lite/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/lite/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.555437 sdv-1.2.0.dev1/docs/api_reference/metadata/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.563780 sdv-1.2.0.dev1/docs/api_reference/metadata/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/dataset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/table.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.565037 sdv-1.2.0.dev1/docs/api_reference/metrics/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.601733 sdv-1.2.0.dev1/docs/api_reference/metrics/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/demos.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/relational.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/timeseries.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.602259 sdv-1.2.0.dev1/docs/api_reference/relational/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.603335 sdv-1.2.0.dev1/docs/api_reference/relational/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/relational/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.603750 sdv-1.2.0.dev1/docs/api_reference/sampling/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.604337 sdv-1.2.0.dev1/docs/api_reference/sampling/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/sdv.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.605323 sdv-1.2.0.dev1/docs/api_reference/tabular/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.613580 sdv-1.2.0.dev1/docs/api_reference/tabular/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/copulas.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.613972 sdv-1.2.0.dev1/docs/api_reference/timeseries/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.615146 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/par.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6934 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/conf.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.615840 sdv-1.2.0.dev1/docs/developer_guides/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8613 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/docs/developer_guides/contributing.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/overview.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.616710 sdv-1.2.0.dev1/docs/developer_guides/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.617398 sdv-1.2.0.dev1/docs/getting_started/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/getting_started/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2557 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/getting_started/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/getting_started/quickstart.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/history.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.629065 sdv-1.2.0.dev1/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/CTGAN-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/Copulas-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/DataCebo-Blue.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.2.0.dev1/docs/images/DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/DeepEcho-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/RDT-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/Real-vs-Synthetic-Evaluation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDGym-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDMetrics-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22394 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDV-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    64162 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/SDV-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDV.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/Single-Table-Metadata-Example.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/images/custom_constraint.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/datacebo-logo-dark-mode.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/datacebo-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/google_colab.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/hma1_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/metadata_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/metadata_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/mybinder.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/quickstart_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.2.0.dev1/docs/images/rdt_main_tranformation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/slack.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6075 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/make.bat
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.631152 sdv-1.2.0.dev1/docs/savefig/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_3.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.2.0.dev1/docs/savefig/experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.2.0.dev1/docs/savefig/experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.2.0.dev1/docs/savefig/experience_years_3.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.524823 sdv-1.2.0.dev1/docs/sdv_theme/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.631402 sdv-1.2.0.dev1/docs/sdv_theme/static/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/sdv_theme/static/slack-32.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.631652 sdv-1.2.0.dev1/docs/user_guides/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.632964 sdv-1.2.0.dev1/docs/user_guides/benchmarking/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/datasets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1885 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/docker.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2562 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/run.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/synthesizers.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.633739 sdv-1.2.0.dev1/docs/user_guides/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/evaluation/evaluation_framework.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/evaluation/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/evaluation/synthetic_data_metrics.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.634806 sdv-1.2.0.dev1/docs/user_guides/relational/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/relational_metadata.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.638035 sdv-1.2.0.dev1/docs/user_guides/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/custom_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/gaussian_copula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/handling_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/table_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/tabular_preset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.638700 sdv-1.2.0.dev1/docs/user_guides/timeseries/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/timeseries/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/timeseries/par.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.639898 sdv-1.2.0.dev1/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2023-06-06 20:54:02.000000 sdv-1.2.0.dev1/sdv/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.642558 sdv-1.2.0.dev1/sdv/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/sdv/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18056 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/sdv/constraints/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      799 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/constraints/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    53574 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/constraints/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5822 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/constraints/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.644002 sdv-1.2.0.dev1/sdv/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    34822 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/sdv/data_processing/data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/sdv/data_processing/datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.644575 sdv-1.2.0.dev1/sdv/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6625 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/datasets/demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1117 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/datasets/local.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      694 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/errors.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.645120 sdv-1.2.0.dev1/sdv/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3701 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/evaluation/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3239 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/evaluation/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.645444 sdv-1.2.0.dev1/sdv/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7153 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/lite/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.647597 sdv-1.2.0.dev1/sdv/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3060 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/metadata/anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29106 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/metadata/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21941 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/metadata/single_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/sdv/metadata/visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.648575 sdv-1.2.0.dev1/sdv/metrics/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/demos.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/relational.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/timeseries.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.649280 sdv-1.2.0.dev1/sdv/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/sdv/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20699 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/multi_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    23027 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/multi_table/hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.650300 sdv-1.2.0.dev1/sdv/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      103 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8638 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/sdv/sampling/hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5578 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/sampling/independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/sampling/tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.650695 sdv-1.2.0.dev1/sdv/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14850 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/sequential/par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.652288 sdv-1.2.0.dev1/sdv/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/sdv/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45383 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/sdv/single_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/sdv/single_table/copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14901 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/single_table/copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9895 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/single_table/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      341 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/single_table/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10141 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/single_table/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5800 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.641094 sdv-1.2.0.dev1/sdv.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    80589 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35730 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1479 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2023-06-07 18:57:18.670143 sdv-1.2.0.dev1/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3853 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.652726 sdv-1.2.0.dev1/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.653101 sdv-1.2.0.dev1/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.653357 sdv-1.2.0.dev1/tests/integration/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12132 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/integration/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/dataset.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.653672 sdv-1.2.0.dev1/tests/integration/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3324 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/datasets/test_demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.654191 sdv-1.2.0.dev1/tests/integration/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1133 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1131 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.654484 sdv-1.2.0.dev1/tests/integration/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/tests/integration/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.655225 sdv-1.2.0.dev1/tests/integration/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      596 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/integration/metadata/test_anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4369 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6200 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/metadata/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.655542 sdv-1.2.0.dev1/tests/integration/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22620 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/tests/integration/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.656222 sdv-1.2.0.dev1/tests/integration/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6268 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.657530 sdv-1.2.0.dev1/tests/integration/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/single_table/custom_constraints.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29343 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/tests/integration/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12402 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/tests/integration/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2528 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/single_table/test_ctgan.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.657713 sdv-1.2.0.dev1/tests/readme_test/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.2.0.dev1/tests/readme_test/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.658443 sdv-1.2.0.dev1/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.659978 sdv-1.2.0.dev1/tests/unit/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    32384 2023-04-20 22:38:57.000000 sdv-1.2.0.dev1/tests/unit/constraints/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   162819 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/constraints/test_tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6700 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/constraints/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.661084 sdv-1.2.0.dev1/tests/unit/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    79609 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.661640 sdv-1.2.0.dev1/tests/unit/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9876 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/datasets/test_demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2498 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/datasets/test_local.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.662002 sdv-1.2.0.dev1/tests/unit/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2865 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2533 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.662332 sdv-1.2.0.dev1/tests/unit/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10135 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.664714 sdv-1.2.0.dev1/tests/unit/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5258 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    75538 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    66306 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.665571 sdv-1.2.0.dev1/tests/unit/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    41567 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/multi_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    28011 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.666673 sdv-1.2.0.dev1/tests/unit/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/tests/unit/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13830 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/tests/unit/sampling/test_hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11155 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/sampling/test_independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/sampling/test_tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.667345 sdv-1.2.0.dev1/tests/unit/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29331 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.669050 sdv-1.2.0.dev1/tests/unit/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    77568 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10328 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8358 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5572 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/utils.py
```

### Comparing `sdv-1.2.0.dev0/CONTRIBUTING.rst` & `sdv-1.2.0.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/HISTORY.md` & `sdv-1.2.0.dev1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,56 @@
 # Release Notes
 
+## 1.2.0 - 2023-06-07
+
+This release adds a parameter called `verbose` to the `HMASynthesizer`. Setting it to True will show progress bars during the fitting steps. Additionally, performance optimizations were made to the modeling and initialization of the `HMASynthesizer`.
+
+Multiple changes were made to enhance constraints. The `Range` constraint was improved to be able to generate more accurate data when null values are provided. Constraints are also now validated against the data when running `validate()` on any synthesizer.
+
+Finally, some warnings were resolved.
+
+### New Features
+
+* Report fitting progress for the HMASynthesizer - Issue [#1440](https://github.com/sdv-dev/SDV/issues/1440) by @pvk-developer
+
+### Bugs Fixed
+
+* Range constraint does not produce cases of missing values & may create violative data - Issue [#1393](https://github.com/sdv-dev/SDV/issues/1393) by @R-Palazzo
+* Synthesizers don't validate constraints during validate() - Issue [#1402](https://github.com/sdv-dev/SDV/issues/1402) by @pvk-developer
+* Confusing error during metadata validation - Issue [#1417](https://github.com/sdv-dev/SDV/issues/1417) by @frances-h
+* SettingWithCopyWarning when conditional sampling - [#1436](https://github.com/sdv-dev/SDV/issues/1436) by @pvk-developer
+* HMASynthesizer is modeling child tables - Issue [#1442](https://github.com/sdv-dev/SDV/issues/1442) by @pvk-developer
+* ValueError when sampling PII columns - Issue [#1445](https://github.com/sdv-dev/SDV/issues/1445) by @pvk-developer
+
+### Internal
+
+* Add BaseHierarchicalSampler Mixin - Issue [#1394](https://github.com/sdv-dev/SDV/issues/1394) by @frances-h
+* Add BaseIndependentSampler Mixin - Issue [#1395](https://github.com/sdv-dev/SDV/issues/1395) by @frances-h
+* Synthesizers created twice during HMA init - Issue [#1418](https://github.com/sdv-dev/SDV/issues/1418) by @frances-h
+* Get rid of unnecessary methods for single table sampling - Issue [#1430](https://github.com/sdv-dev/SDV/issues/1430) by @amontanez24
+* Detect all addons from top level __init__ - PR [#1453](https://github.com/sdv-dev/SDV/pull/1453) by @frances-h
+
+### Maintenance
+
+* Upgrade to torch 2.0 - Issue [#1365](https://github.com/sdv-dev/SDV/issues/1365) by @fealho
+* During fit, there is a FutureWarning (due to RDT 1.5.0) - Issue [#1456](https://github.com/sdv-dev/SDV/issues/1456) by @amontanez24
+
 ## 1.1.0 - 2023-05-10
 
 This release adds a new initialization parameter to synthesizers called `locales` that allows users to set the locales to use for all columns that have a locale based `sdtype` (eg. `address` or `phone_number`). Additionally, it adds support for Pandas 2.0!
 
 Multiple enhancements were made to improve the performance of data and metadata validation in synthesizers. The `Inequality` constraint was improved to be able to generate more scenarios of data concerning the presence of NaNs. Finally, many warnings have been resolved.
 
 ### New Features
 
 * Add add-on detection for new constraints - Issue [#1397](https://github.com/sdv-dev/SDV/issues/1397) by @frances-h
 * Add add-on detection for multi and single table synthesizers - Issue [#1385](https://github.com/sdv-dev/SDV/issues/1385) by @frances-h
 * Setting a locale for all my anonymized (PII) columns - Issue [#1371](https://github.com/sdv-dev/SDV/issues/1371) by @frances-h
 
-### Bigs Fixed
+### Bugs Fixed
 
 * Skip checking for Faker function if its a default sdtype - PR [#1410](https://github.com/sdv-dev/SDV/pull/1410) by @pvk-developer
 * Inequality constraint does not produce all possibilities of missing values - Issue [#1392](https://github.com/sdv-dev/SDV/issues/1392) by @R-Palazzo
 * Deprecated locale warning - Issue [#1400](https://github.com/sdv-dev/SDV/issues/1400) by @frances-h
 
 ### Maintenance
```

### Comparing `sdv-1.2.0.dev0/LICENSE` & `sdv-1.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/PKG-INFO` & `sdv-1.2.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.2.0.dev0
+Version: 1.2.0.dev1
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
@@ -242,27 +242,61 @@
 [Get started using the SDV package](https://bit.ly/sdv-docs) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # Release Notes
 
+## 1.2.0 - 2023-06-07
+
+This release adds a parameter called `verbose` to the `HMASynthesizer`. Setting it to True will show progress bars during the fitting steps. Additionally, performance optimizations were made to the modeling and initialization of the `HMASynthesizer`.
+
+Multiple changes were made to enhance constraints. The `Range` constraint was improved to be able to generate more accurate data when null values are provided. Constraints are also now validated against the data when running `validate()` on any synthesizer.
+
+Finally, some warnings were resolved.
+
+### New Features
+
+* Report fitting progress for the HMASynthesizer - Issue [#1440](https://github.com/sdv-dev/SDV/issues/1440) by @pvk-developer
+
+### Bugs Fixed
+
+* Range constraint does not produce cases of missing values & may create violative data - Issue [#1393](https://github.com/sdv-dev/SDV/issues/1393) by @R-Palazzo
+* Synthesizers don't validate constraints during validate() - Issue [#1402](https://github.com/sdv-dev/SDV/issues/1402) by @pvk-developer
+* Confusing error during metadata validation - Issue [#1417](https://github.com/sdv-dev/SDV/issues/1417) by @frances-h
+* SettingWithCopyWarning when conditional sampling - [#1436](https://github.com/sdv-dev/SDV/issues/1436) by @pvk-developer
+* HMASynthesizer is modeling child tables - Issue [#1442](https://github.com/sdv-dev/SDV/issues/1442) by @pvk-developer
+* ValueError when sampling PII columns - Issue [#1445](https://github.com/sdv-dev/SDV/issues/1445) by @pvk-developer
+
+### Internal
+
+* Add BaseHierarchicalSampler Mixin - Issue [#1394](https://github.com/sdv-dev/SDV/issues/1394) by @frances-h
+* Add BaseIndependentSampler Mixin - Issue [#1395](https://github.com/sdv-dev/SDV/issues/1395) by @frances-h
+* Synthesizers created twice during HMA init - Issue [#1418](https://github.com/sdv-dev/SDV/issues/1418) by @frances-h
+* Get rid of unnecessary methods for single table sampling - Issue [#1430](https://github.com/sdv-dev/SDV/issues/1430) by @amontanez24
+* Detect all addons from top level __init__ - PR [#1453](https://github.com/sdv-dev/SDV/pull/1453) by @frances-h
+
+### Maintenance
+
+* Upgrade to torch 2.0 - Issue [#1365](https://github.com/sdv-dev/SDV/issues/1365) by @fealho
+* During fit, there is a FutureWarning (due to RDT 1.5.0) - Issue [#1456](https://github.com/sdv-dev/SDV/issues/1456) by @amontanez24
+
 ## 1.1.0 - 2023-05-10
 
 This release adds a new initialization parameter to synthesizers called `locales` that allows users to set the locales to use for all columns that have a locale based `sdtype` (eg. `address` or `phone_number`). Additionally, it adds support for Pandas 2.0!
 
 Multiple enhancements were made to improve the performance of data and metadata validation in synthesizers. The `Inequality` constraint was improved to be able to generate more scenarios of data concerning the presence of NaNs. Finally, many warnings have been resolved.
 
 ### New Features
 
 * Add add-on detection for new constraints - Issue [#1397](https://github.com/sdv-dev/SDV/issues/1397) by @frances-h
 * Add add-on detection for multi and single table synthesizers - Issue [#1385](https://github.com/sdv-dev/SDV/issues/1385) by @frances-h
 * Setting a locale for all my anonymized (PII) columns - Issue [#1371](https://github.com/sdv-dev/SDV/issues/1371) by @frances-h
 
-### Bigs Fixed
+### Bugs Fixed
 
 * Skip checking for Faker function if its a default sdtype - PR [#1410](https://github.com/sdv-dev/SDV/pull/1410) by @pvk-developer
 * Inequality constraint does not produce all possibilities of missing values - Issue [#1392](https://github.com/sdv-dev/SDV/issues/1392) by @R-Palazzo
 * Deprecated locale warning - Issue [#1400](https://github.com/sdv-dev/SDV/issues/1400) by @frances-h
 
 ### Maintenance
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.2.0.dev0 Summary: Generate synthetic
+Metadata-Version: 2.1 Name: sdv Version: 1.2.0.dev1 Summary: Generate synthetic
 data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -131,27 +131,58 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://bit.ly/sdv-docs) -- a fully integrated solution and your one-stop shop
 for synthetic data. Or, use the standalone libraries for specific needs. #
-Release Notes ## 1.1.0 - 2023-05-10 This release adds a new initialization
-parameter to synthesizers called `locales` that allows users to set the locales
-to use for all columns that have a locale based `sdtype` (eg. `address` or
+Release Notes ## 1.2.0 - 2023-06-07 This release adds a parameter called
+`verbose` to the `HMASynthesizer`. Setting it to True will show progress bars
+during the fitting steps. Additionally, performance optimizations were made to
+the modeling and initialization of the `HMASynthesizer`. Multiple changes were
+made to enhance constraints. The `Range` constraint was improved to be able to
+generate more accurate data when null values are provided. Constraints are also
+now validated against the data when running `validate()` on any synthesizer.
+Finally, some warnings were resolved. ### New Features * Report fitting
+progress for the HMASynthesizer - Issue [#1440](https://github.com/sdv-dev/SDV/
+issues/1440) by @pvk-developer ### Bugs Fixed * Range constraint does not
+produce cases of missing values & may create violative data - Issue [#1393]
+(https://github.com/sdv-dev/SDV/issues/1393) by @R-Palazzo * Synthesizers don't
+validate constraints during validate() - Issue [#1402](https://github.com/sdv-
+dev/SDV/issues/1402) by @pvk-developer * Confusing error during metadata
+validation - Issue [#1417](https://github.com/sdv-dev/SDV/issues/1417) by
+@frances-h * SettingWithCopyWarning when conditional sampling - [#1436](https:/
+/github.com/sdv-dev/SDV/issues/1436) by @pvk-developer * HMASynthesizer is
+modeling child tables - Issue [#1442](https://github.com/sdv-dev/SDV/issues/
+1442) by @pvk-developer * ValueError when sampling PII columns - Issue [#1445]
+(https://github.com/sdv-dev/SDV/issues/1445) by @pvk-developer ### Internal *
+Add BaseHierarchicalSampler Mixin - Issue [#1394](https://github.com/sdv-dev/
+SDV/issues/1394) by @frances-h * Add BaseIndependentSampler Mixin - Issue
+[#1395](https://github.com/sdv-dev/SDV/issues/1395) by @frances-h *
+Synthesizers created twice during HMA init - Issue [#1418](https://github.com/
+sdv-dev/SDV/issues/1418) by @frances-h * Get rid of unnecessary methods for
+single table sampling - Issue [#1430](https://github.com/sdv-dev/SDV/issues/
+1430) by @amontanez24 * Detect all addons from top level __init__ - PR [#1453]
+(https://github.com/sdv-dev/SDV/pull/1453) by @frances-h ### Maintenance *
+Upgrade to torch 2.0 - Issue [#1365](https://github.com/sdv-dev/SDV/issues/
+1365) by @fealho * During fit, there is a FutureWarning (due to RDT 1.5.0) -
+Issue [#1456](https://github.com/sdv-dev/SDV/issues/1456) by @amontanez24 ##
+1.1.0 - 2023-05-10 This release adds a new initialization parameter to
+synthesizers called `locales` that allows users to set the locales to use for
+all columns that have a locale based `sdtype` (eg. `address` or
 `phone_number`). Additionally, it adds support for Pandas 2.0! Multiple
 enhancements were made to improve the performance of data and metadata
 validation in synthesizers. The `Inequality` constraint was improved to be able
 to generate more scenarios of data concerning the presence of NaNs. Finally,
 many warnings have been resolved. ### New Features * Add add-on detection for
 new constraints - Issue [#1397](https://github.com/sdv-dev/SDV/issues/1397) by
 @frances-h * Add add-on detection for multi and single table synthesizers -
 Issue [#1385](https://github.com/sdv-dev/SDV/issues/1385) by @frances-h *
 Setting a locale for all my anonymized (PII) columns - Issue [#1371](https://
-github.com/sdv-dev/SDV/issues/1371) by @frances-h ### Bigs Fixed * Skip
+github.com/sdv-dev/SDV/issues/1371) by @frances-h ### Bugs Fixed * Skip
 checking for Faker function if its a default sdtype - PR [#1410](https://
 github.com/sdv-dev/SDV/pull/1410) by @pvk-developer * Inequality constraint
 does not produce all possibilities of missing values - Issue [#1392](https://
 github.com/sdv-dev/SDV/issues/1392) by @R-Palazzo * Deprecated locale warning -
 Issue [#1400](https://github.com/sdv-dev/SDV/issues/1400) by @frances-h ###
 Maintenance * Use cached Faker instance to discover if an sdtype is a Faker
 function. - Issue [#1405](https://github.com/sdv-dev/SDV/issues/1405) by @pvk-
```

### Comparing `sdv-1.2.0.dev0/README.md` & `sdv-1.2.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/Makefile` & `sdv-1.2.0.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/constraints/tabular.rst` & `sdv-1.2.0.dev1/docs/api_reference/constraints/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst` & `sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst` & `sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metadata/dataset.rst` & `sdv-1.2.0.dev1/docs/api_reference/metadata/dataset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metadata/table.rst` & `sdv-1.2.0.dev1/docs/api_reference/metadata/table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/relational.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/relational.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/tabular.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/metrics/timeseries.rst` & `sdv-1.2.0.dev1/docs/api_reference/metrics/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst` & `sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst` & `sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/conf.py` & `sdv-1.2.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/developer_guides/contributing.rst` & `sdv-1.2.0.dev1/docs/developer_guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/developer_guides/overview.rst` & `sdv-1.2.0.dev1/docs/developer_guides/overview.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/developer_guides/sdv/constraints.rst` & `sdv-1.2.0.dev1/docs/developer_guides/sdv/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/developer_guides/sdv/metadata.rst` & `sdv-1.2.0.dev1/docs/developer_guides/sdv/metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/developer_guides/sdv/tabular.rst` & `sdv-1.2.0.dev1/docs/developer_guides/sdv/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/getting_started/install.rst` & `sdv-1.2.0.dev1/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/getting_started/quickstart.rst` & `sdv-1.2.0.dev1/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/CTGAN-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/CTGAN-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/Copulas-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/Copulas-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/DataCebo-Blue.png` & `sdv-1.2.0.dev1/docs/images/DataCebo-Blue.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/DataCebo.png` & `sdv-1.2.0.dev1/docs/images/DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/DeepEcho-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/DeepEcho-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/RDT-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/RDT-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/Real-vs-Synthetic-Evaluation.png` & `sdv-1.2.0.dev1/docs/images/Real-vs-Synthetic-Evaluation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/SDGym-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/SDGym-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/SDMetrics-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/SDMetrics-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/SDV-DataCebo.png` & `sdv-1.2.0.dev1/docs/images/SDV-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/SDV-logo.png` & `sdv-1.2.0.dev1/docs/images/SDV-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/SDV.png` & `sdv-1.2.0.dev1/docs/images/SDV.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/Single-Table-Metadata-Example.png` & `sdv-1.2.0.dev1/docs/images/Single-Table-Metadata-Example.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/custom_constraint.png` & `sdv-1.2.0.dev1/docs/images/custom_constraint.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/datacebo-logo-dark-mode.png` & `sdv-1.2.0.dev1/docs/images/datacebo-logo-dark-mode.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/datacebo-logo.png` & `sdv-1.2.0.dev1/docs/images/datacebo-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/google_colab.png` & `sdv-1.2.0.dev1/docs/images/google_colab.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/hma1_1.png` & `sdv-1.2.0.dev1/docs/images/hma1_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/metadata_1.png` & `sdv-1.2.0.dev1/docs/images/metadata_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/metadata_2.png` & `sdv-1.2.0.dev1/docs/images/metadata_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/mybinder.png` & `sdv-1.2.0.dev1/docs/images/mybinder.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/quickstart_1.png` & `sdv-1.2.0.dev1/docs/images/quickstart_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/rdt_main_tranformation.png` & `sdv-1.2.0.dev1/docs/images/rdt_main_tranformation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/images/slack.png` & `sdv-1.2.0.dev1/docs/images/slack.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/index.rst` & `sdv-1.2.0.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/make.bat` & `sdv-1.2.0.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/savefig/copulagan_experience_years_1.png` & `sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/savefig/copulagan_experience_years_2.png` & `sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/savefig/copulagan_experience_years_3.png` & `sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/savefig/experience_years_1.png` & `sdv-1.2.0.dev1/docs/savefig/experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/savefig/experience_years_2.png` & `sdv-1.2.0.dev1/docs/savefig/experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/savefig/experience_years_3.png` & `sdv-1.2.0.dev1/docs/savefig/experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/sdv_theme/static/slack-32.png` & `sdv-1.2.0.dev1/docs/sdv_theme/static/slack-32.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/benchmarking/datasets.rst` & `sdv-1.2.0.dev1/docs/user_guides/benchmarking/datasets.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/benchmarking/docker.rst` & `sdv-1.2.0.dev1/docs/user_guides/benchmarking/docker.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/benchmarking/index.rst` & `sdv-1.2.0.dev1/docs/user_guides/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/benchmarking/install.rst` & `sdv-1.2.0.dev1/docs/user_guides/benchmarking/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/benchmarking/run.rst` & `sdv-1.2.0.dev1/docs/user_guides/benchmarking/run.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/benchmarking/synthesizers.rst` & `sdv-1.2.0.dev1/docs/user_guides/benchmarking/synthesizers.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/evaluation/evaluation_framework.rst` & `sdv-1.2.0.dev1/docs/user_guides/evaluation/evaluation_framework.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/relational/constraints.rst` & `sdv-1.2.0.dev1/docs/user_guides/relational/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/relational/hma1.rst` & `sdv-1.2.0.dev1/docs/user_guides/relational/hma1.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/relational/relational_metadata.rst` & `sdv-1.2.0.dev1/docs/user_guides/relational/relational_metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/copulagan.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/copulagan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/ctgan.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/ctgan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/custom_constraints.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/custom_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/gaussian_copula.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/gaussian_copula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/handling_constraints.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/handling_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/index.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/tabular_preset.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/tabular_preset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/single_table/tvae.rst` & `sdv-1.2.0.dev1/docs/user_guides/single_table/tvae.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/docs/user_guides/timeseries/par.rst` & `sdv-1.2.0.dev1/docs/user_guides/timeseries/par.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/__init__.py` & `sdv-1.2.0.dev1/sdv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # configure logging for the library with a null handler (nothing is printed by default). See
 # http://docs.python-guide.org/en/latest/writing/logging/
 
 """Top-level package for SDV."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.2.0.dev0'
+__version__ = '1.2.0.dev1'
 
 
 import sys
 import warnings
 from operator import attrgetter
 
 from pkg_resources import iter_entry_points
```

### Comparing `sdv-1.2.0.dev0/sdv/constraints/__init__.py` & `sdv-1.2.0.dev1/sdv/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/constraints/base.py` & `sdv-1.2.0.dev1/sdv/constraints/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,30 +406,30 @@
         transformers = {}
         for column_name, data in data_to_model.items():
             dtype = data.dropna().infer_objects().dtype.kind
             if dtype in ('i', 'f'):
                 sdtypes[column_name] = 'numerical'
                 transformers = FloatFormatter(
                     missing_value_replacement='mean',
-                    model_missing_values=True,
+                    missing_value_generation='from_column'
                 )
             elif dtype == 'O':
                 sdtypes[column_name] = 'categorical'
                 transformers[column_name] = OneHotEncoder
             elif dtype == 'M':
                 sdtypes[column_name] = 'datetime'
                 transformers[column_name] = UnixTimestampEncoder(
                     missing_value_replacement='mean',
-                    model_missing_values=True,
+                    missing_value_generation='from_column'
                 )
             elif dtype == 'b':
                 sdtypes[column_name] = 'boolean'
                 transformers[column_name] = BinaryEncoder(
                     missing_value_replacement=-1,
-                    model_missing_values=True
+                    missing_value_generation='from_column'
                 )
 
         return {'sdtypes': sdtypes, 'transformers': transformers}
 
     def fit(self, table_data):
         """Fit the ``ColumnsModel``.
```

### Comparing `sdv-1.2.0.dev0/sdv/constraints/errors.py` & `sdv-1.2.0.dev1/sdv/constraints/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/constraints/tabular.py` & `sdv-1.2.0.dev1/sdv/constraints/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/constraints/utils.py` & `sdv-1.2.0.dev1/sdv/constraints/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/data_processing/data_processor.py` & `sdv-1.2.0.dev1/sdv/data_processing/data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,36 +59,36 @@
     """
 
     _DEFAULT_TRANSFORMERS_BY_SDTYPE = {
         'numerical': rdt.transformers.FloatFormatter(
             learn_rounding_scheme=True,
             enforce_min_max_values=True,
             missing_value_replacement='mean',
-            model_missing_values=False,
+            missing_value_generation='random',
         ),
         'categorical': rdt.transformers.LabelEncoder(add_noise=True),
         'boolean': rdt.transformers.LabelEncoder(add_noise=True),
         'datetime': rdt.transformers.UnixTimestampEncoder(
             missing_value_replacement='mean',
-            model_missing_values=False,
+            missing_value_generation='random',
         ),
         'id': rdt.transformers.RegexGenerator()
     }
     _DTYPE_TO_SDTYPE = {
         'i': 'numerical',
         'f': 'numerical',
         'O': 'categorical',
         'b': 'boolean',
         'M': 'datetime',
     }
 
     def _update_numerical_transformer(self, enforce_rounding, enforce_min_max_values):
         custom_float_formatter = rdt.transformers.FloatFormatter(
             missing_value_replacement='mean',
-            model_missing_values=False,
+            missing_value_generation='random',
             learn_rounding_scheme=enforce_rounding,
             enforce_min_max_values=enforce_min_max_values
         )
         self._transformers_by_sdtype.update({'numerical': custom_float_formatter})
 
     def __init__(self, metadata, enforce_rounding=True, enforce_min_max_values=True,
                  model_kwargs=None, table_name=None, locales=None):
@@ -433,15 +433,15 @@
         missing_columns = set(columns_created_by_constraints) - config['transformers'].keys()
         for column in missing_columns:
             dtype_kind = data[column].dtype.kind
             if dtype_kind in ('i', 'f'):
                 config['sdtypes'][column] = 'numerical'
                 config['transformers'][column] = rdt.transformers.FloatFormatter(
                     missing_value_replacement='mean',
-                    model_missing_values=False,
+                    missing_value_generation='random',
                     enforce_min_max_values=self._enforce_min_max_values
                 )
             else:
                 sdtype = self._DTYPE_TO_SDTYPE.get(dtype_kind, 'categorical')
                 config['sdtypes'][column] = sdtype
                 config['transformers'][column] = self._get_transformer_instance(sdtype, {})
```

### Comparing `sdv-1.2.0.dev0/sdv/data_processing/datetime_formatter.py` & `sdv-1.2.0.dev1/sdv/data_processing/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/data_processing/errors.py` & `sdv-1.2.0.dev1/sdv/data_processing/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/data_processing/numerical_formatter.py` & `sdv-1.2.0.dev1/sdv/data_processing/numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/data_processing/utils.py` & `sdv-1.2.0.dev1/sdv/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/datasets/demo.py` & `sdv-1.2.0.dev1/sdv/datasets/demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/datasets/local.py` & `sdv-1.2.0.dev1/sdv/datasets/local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/errors.py` & `sdv-1.2.0.dev1/sdv/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/evaluation/multi_table.py` & `sdv-1.2.0.dev1/sdv/evaluation/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/evaluation/single_table.py` & `sdv-1.2.0.dev1/sdv/evaluation/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/lite/single_table.py` & `sdv-1.2.0.dev1/sdv/lite/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/metadata/anonymization.py` & `sdv-1.2.0.dev1/sdv/metadata/anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/metadata/metadata_upgrader.py` & `sdv-1.2.0.dev1/sdv/metadata/metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/metadata/multi_table.py` & `sdv-1.2.0.dev1/sdv/metadata/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/metadata/single_table.py` & `sdv-1.2.0.dev1/sdv/metadata/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/metadata/utils.py` & `sdv-1.2.0.dev1/sdv/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/metadata/visualization.py` & `sdv-1.2.0.dev1/sdv/metadata/visualization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/multi_table/base.py` & `sdv-1.2.0.dev1/sdv/multi_table/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/multi_table/hma.py` & `sdv-1.2.0.dev1/sdv/multi_table/hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/sampling/hierarchical_sampler.py` & `sdv-1.2.0.dev1/sdv/sampling/hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/sampling/independent_sampler.py` & `sdv-1.2.0.dev1/sdv/sampling/independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/sampling/tabular.py` & `sdv-1.2.0.dev1/sdv/sampling/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/sequential/par.py` & `sdv-1.2.0.dev1/sdv/sequential/par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/single_table/base.py` & `sdv-1.2.0.dev1/sdv/single_table/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/single_table/copulagan.py` & `sdv-1.2.0.dev1/sdv/single_table/copulagan.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                 sdtypes[column] = 'numerical'
                 distribution = self._numerical_distributions.get(
                     column,
                     self._default_distribution
                 )
 
                 transformers[column] = rdt.transformers.GaussianNormalizer(
-                    model_missing_values=True,
+                    missing_value_generation='from_column',
                     distribution=distribution,
                 )
 
             else:
                 sdtypes[column] = sdtype or 'categorical'
                 transformers[column] = None
```

### Comparing `sdv-1.2.0.dev0/sdv/single_table/copulas.py` & `sdv-1.2.0.dev1/sdv/single_table/copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/single_table/ctgan.py` & `sdv-1.2.0.dev1/sdv/single_table/ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/single_table/utils.py` & `sdv-1.2.0.dev1/sdv/single_table/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv/utils.py` & `sdv-1.2.0.dev1/sdv/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv.egg-info/PKG-INFO` & `sdv-1.2.0.dev1/sdv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.2.0.dev0
+Version: 1.2.0.dev1
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
@@ -242,27 +242,61 @@
 [Get started using the SDV package](https://bit.ly/sdv-docs) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # Release Notes
 
+## 1.2.0 - 2023-06-07
+
+This release adds a parameter called `verbose` to the `HMASynthesizer`. Setting it to True will show progress bars during the fitting steps. Additionally, performance optimizations were made to the modeling and initialization of the `HMASynthesizer`.
+
+Multiple changes were made to enhance constraints. The `Range` constraint was improved to be able to generate more accurate data when null values are provided. Constraints are also now validated against the data when running `validate()` on any synthesizer.
+
+Finally, some warnings were resolved.
+
+### New Features
+
+* Report fitting progress for the HMASynthesizer - Issue [#1440](https://github.com/sdv-dev/SDV/issues/1440) by @pvk-developer
+
+### Bugs Fixed
+
+* Range constraint does not produce cases of missing values & may create violative data - Issue [#1393](https://github.com/sdv-dev/SDV/issues/1393) by @R-Palazzo
+* Synthesizers don't validate constraints during validate() - Issue [#1402](https://github.com/sdv-dev/SDV/issues/1402) by @pvk-developer
+* Confusing error during metadata validation - Issue [#1417](https://github.com/sdv-dev/SDV/issues/1417) by @frances-h
+* SettingWithCopyWarning when conditional sampling - [#1436](https://github.com/sdv-dev/SDV/issues/1436) by @pvk-developer
+* HMASynthesizer is modeling child tables - Issue [#1442](https://github.com/sdv-dev/SDV/issues/1442) by @pvk-developer
+* ValueError when sampling PII columns - Issue [#1445](https://github.com/sdv-dev/SDV/issues/1445) by @pvk-developer
+
+### Internal
+
+* Add BaseHierarchicalSampler Mixin - Issue [#1394](https://github.com/sdv-dev/SDV/issues/1394) by @frances-h
+* Add BaseIndependentSampler Mixin - Issue [#1395](https://github.com/sdv-dev/SDV/issues/1395) by @frances-h
+* Synthesizers created twice during HMA init - Issue [#1418](https://github.com/sdv-dev/SDV/issues/1418) by @frances-h
+* Get rid of unnecessary methods for single table sampling - Issue [#1430](https://github.com/sdv-dev/SDV/issues/1430) by @amontanez24
+* Detect all addons from top level __init__ - PR [#1453](https://github.com/sdv-dev/SDV/pull/1453) by @frances-h
+
+### Maintenance
+
+* Upgrade to torch 2.0 - Issue [#1365](https://github.com/sdv-dev/SDV/issues/1365) by @fealho
+* During fit, there is a FutureWarning (due to RDT 1.5.0) - Issue [#1456](https://github.com/sdv-dev/SDV/issues/1456) by @amontanez24
+
 ## 1.1.0 - 2023-05-10
 
 This release adds a new initialization parameter to synthesizers called `locales` that allows users to set the locales to use for all columns that have a locale based `sdtype` (eg. `address` or `phone_number`). Additionally, it adds support for Pandas 2.0!
 
 Multiple enhancements were made to improve the performance of data and metadata validation in synthesizers. The `Inequality` constraint was improved to be able to generate more scenarios of data concerning the presence of NaNs. Finally, many warnings have been resolved.
 
 ### New Features
 
 * Add add-on detection for new constraints - Issue [#1397](https://github.com/sdv-dev/SDV/issues/1397) by @frances-h
 * Add add-on detection for multi and single table synthesizers - Issue [#1385](https://github.com/sdv-dev/SDV/issues/1385) by @frances-h
 * Setting a locale for all my anonymized (PII) columns - Issue [#1371](https://github.com/sdv-dev/SDV/issues/1371) by @frances-h
 
-### Bigs Fixed
+### Bugs Fixed
 
 * Skip checking for Faker function if its a default sdtype - PR [#1410](https://github.com/sdv-dev/SDV/pull/1410) by @pvk-developer
 * Inequality constraint does not produce all possibilities of missing values - Issue [#1392](https://github.com/sdv-dev/SDV/issues/1392) by @R-Palazzo
 * Deprecated locale warning - Issue [#1400](https://github.com/sdv-dev/SDV/issues/1400) by @frances-h
 
 ### Maintenance
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.2.0.dev0 Summary: Generate synthetic
+Metadata-Version: 2.1 Name: sdv Version: 1.2.0.dev1 Summary: Generate synthetic
 data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -131,27 +131,58 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://bit.ly/sdv-docs) -- a fully integrated solution and your one-stop shop
 for synthetic data. Or, use the standalone libraries for specific needs. #
-Release Notes ## 1.1.0 - 2023-05-10 This release adds a new initialization
-parameter to synthesizers called `locales` that allows users to set the locales
-to use for all columns that have a locale based `sdtype` (eg. `address` or
+Release Notes ## 1.2.0 - 2023-06-07 This release adds a parameter called
+`verbose` to the `HMASynthesizer`. Setting it to True will show progress bars
+during the fitting steps. Additionally, performance optimizations were made to
+the modeling and initialization of the `HMASynthesizer`. Multiple changes were
+made to enhance constraints. The `Range` constraint was improved to be able to
+generate more accurate data when null values are provided. Constraints are also
+now validated against the data when running `validate()` on any synthesizer.
+Finally, some warnings were resolved. ### New Features * Report fitting
+progress for the HMASynthesizer - Issue [#1440](https://github.com/sdv-dev/SDV/
+issues/1440) by @pvk-developer ### Bugs Fixed * Range constraint does not
+produce cases of missing values & may create violative data - Issue [#1393]
+(https://github.com/sdv-dev/SDV/issues/1393) by @R-Palazzo * Synthesizers don't
+validate constraints during validate() - Issue [#1402](https://github.com/sdv-
+dev/SDV/issues/1402) by @pvk-developer * Confusing error during metadata
+validation - Issue [#1417](https://github.com/sdv-dev/SDV/issues/1417) by
+@frances-h * SettingWithCopyWarning when conditional sampling - [#1436](https:/
+/github.com/sdv-dev/SDV/issues/1436) by @pvk-developer * HMASynthesizer is
+modeling child tables - Issue [#1442](https://github.com/sdv-dev/SDV/issues/
+1442) by @pvk-developer * ValueError when sampling PII columns - Issue [#1445]
+(https://github.com/sdv-dev/SDV/issues/1445) by @pvk-developer ### Internal *
+Add BaseHierarchicalSampler Mixin - Issue [#1394](https://github.com/sdv-dev/
+SDV/issues/1394) by @frances-h * Add BaseIndependentSampler Mixin - Issue
+[#1395](https://github.com/sdv-dev/SDV/issues/1395) by @frances-h *
+Synthesizers created twice during HMA init - Issue [#1418](https://github.com/
+sdv-dev/SDV/issues/1418) by @frances-h * Get rid of unnecessary methods for
+single table sampling - Issue [#1430](https://github.com/sdv-dev/SDV/issues/
+1430) by @amontanez24 * Detect all addons from top level __init__ - PR [#1453]
+(https://github.com/sdv-dev/SDV/pull/1453) by @frances-h ### Maintenance *
+Upgrade to torch 2.0 - Issue [#1365](https://github.com/sdv-dev/SDV/issues/
+1365) by @fealho * During fit, there is a FutureWarning (due to RDT 1.5.0) -
+Issue [#1456](https://github.com/sdv-dev/SDV/issues/1456) by @amontanez24 ##
+1.1.0 - 2023-05-10 This release adds a new initialization parameter to
+synthesizers called `locales` that allows users to set the locales to use for
+all columns that have a locale based `sdtype` (eg. `address` or
 `phone_number`). Additionally, it adds support for Pandas 2.0! Multiple
 enhancements were made to improve the performance of data and metadata
 validation in synthesizers. The `Inequality` constraint was improved to be able
 to generate more scenarios of data concerning the presence of NaNs. Finally,
 many warnings have been resolved. ### New Features * Add add-on detection for
 new constraints - Issue [#1397](https://github.com/sdv-dev/SDV/issues/1397) by
 @frances-h * Add add-on detection for multi and single table synthesizers -
 Issue [#1385](https://github.com/sdv-dev/SDV/issues/1385) by @frances-h *
 Setting a locale for all my anonymized (PII) columns - Issue [#1371](https://
-github.com/sdv-dev/SDV/issues/1371) by @frances-h ### Bigs Fixed * Skip
+github.com/sdv-dev/SDV/issues/1371) by @frances-h ### Bugs Fixed * Skip
 checking for Faker function if its a default sdtype - PR [#1410](https://
 github.com/sdv-dev/SDV/pull/1410) by @pvk-developer * Inequality constraint
 does not produce all possibilities of missing values - Issue [#1392](https://
 github.com/sdv-dev/SDV/issues/1392) by @R-Palazzo * Deprecated locale warning -
 Issue [#1400](https://github.com/sdv-dev/SDV/issues/1400) by @frances-h ###
 Maintenance * Use cached Faker instance to discover if an sdtype is a Faker
 function. - Issue [#1405](https://github.com/sdv-dev/SDV/issues/1405) by @pvk-
```

### Comparing `sdv-1.2.0.dev0/sdv.egg-info/SOURCES.txt` & `sdv-1.2.0.dev1/sdv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/sdv.egg-info/requires.txt` & `sdv-1.2.0.dev1/sdv.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Faker<15,>=10
 graphviz<1,>=0.13.2
 tqdm<5,>=4.15
 copulas<0.10,>=0.9.0
 ctgan<0.8,>=0.7.2
 deepecho<0.5,>=0.4.1
-rdt<2,>=1.4.2
+rdt<2,>=1.5.0
 sdmetrics<0.11,>=0.10.0
 cloudpickle<3.0,>=2.1.0
 boto3<2,>=1.15.0
 botocore<2,>=1.18
 
 [:python_version < "3.10"]
 numpy<2,>=1.20.0
```

### Comparing `sdv-1.2.0.dev0/setup.cfg` & `sdv-1.2.0.dev1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0.dev0
+current_version = 1.2.0.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdv-1.2.0.dev0/setup.py` & `sdv-1.2.0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "numpy>=1.23.3,<2;python_version>='3.10'",
     "pandas>=1.1.3;python_version<'3.10'",
     "pandas>=1.5.0;python_version>='3.10'",
     'tqdm>=4.15,<5',
     'copulas>=0.9.0,<0.10',
     'ctgan>=0.7.2,<0.8',
     'deepecho>=0.4.1,<0.5',
-    'rdt>=1.4.2,<2',
+    'rdt>=1.5.0,<2',
     'sdmetrics>=0.10.0,<0.11',
     'cloudpickle>=2.1.0,<3.0',
     'boto3>=1.15.0,<2',
     'botocore>=1.18,<2'
 ]
 
 pomegranate_requires = [
@@ -132,10 +132,10 @@
     name='sdv',
     packages=find_packages(include=['sdv', 'sdv.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDV',
-    version='1.2.0.dev0',
+    version='1.2.0.dev1',
     zip_safe=False,
 )
```

### Comparing `sdv-1.2.0.dev0/tests/integration/data_processing/test_data_processor.py` & `sdv-1.2.0.dev1/tests/integration/data_processing/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/dataset.py` & `sdv-1.2.0.dev1/tests/integration/dataset.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/datasets/test_demo.py` & `sdv-1.2.0.dev1/tests/integration/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/evaluation/test_multi_table.py` & `sdv-1.2.0.dev1/tests/integration/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/evaluation/test_single_table.py` & `sdv-1.2.0.dev1/tests/integration/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/lite/test_single_table.py` & `sdv-1.2.0.dev1/tests/integration/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/metadata/test_anonymization.py` & `sdv-1.2.0.dev1/tests/integration/metadata/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/metadata/test_multi_table.py` & `sdv-1.2.0.dev1/tests/integration/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/metadata/test_single_table.py` & `sdv-1.2.0.dev1/tests/integration/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/multi_table/test_hma.py` & `sdv-1.2.0.dev1/tests/integration/multi_table/test_hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/sequential/test_par.py` & `sdv-1.2.0.dev1/tests/integration/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/single_table/custom_constraints.py` & `sdv-1.2.0.dev1/tests/integration/single_table/custom_constraints.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/single_table/test_base.py` & `sdv-1.2.0.dev1/tests/integration/single_table/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,15 +522,15 @@
     # Assert
     assert isinstance(transformers['numerical_col'], FloatFormatter)
     assert isinstance(transformers['pii_col'], AnonymizedFaker)
     assert isinstance(transformers['primary_key'], RegexGenerator)
     assert isinstance(transformers['categorical_col'], LabelEncoder)
 
     assert transformers['numerical_col'].missing_value_replacement == 'mean'
-    assert transformers['numerical_col'].model_missing_values is False
+    assert transformers['numerical_col'].missing_value_generation == 'random'
     assert transformers['numerical_col'].learn_rounding_scheme is False
     assert transformers['numerical_col'].enforce_min_max_values is False
 
     assert transformers['pii_col'].provider_name == 'address'
     assert transformers['pii_col'].function_name == 'address'
 
     assert transformers['primary_key'].regex_format == 'user-[0-9]{3}'
```

### Comparing `sdv-1.2.0.dev0/tests/integration/single_table/test_copulas.py` & `sdv-1.2.0.dev1/tests/integration/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/integration/single_table/test_ctgan.py` & `sdv-1.2.0.dev1/tests/integration/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/readme_test/README.md` & `sdv-1.2.0.dev1/tests/readme_test/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/constraints/test_base.py` & `sdv-1.2.0.dev1/tests/unit/constraints/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/constraints/test_tabular.py` & `sdv-1.2.0.dev1/tests/unit/constraints/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/constraints/test_utils.py` & `sdv-1.2.0.dev1/tests/unit/constraints/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/data_processing/test_data_processor.py` & `sdv-1.2.0.dev1/tests/unit/data_processing/test_data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1060,20 +1060,20 @@
             'id': 'text',
             'date': 'datetime'
         }
 
         int_transformer = config['transformers']['created_int']
         assert isinstance(int_transformer, FloatFormatter)
         assert int_transformer.missing_value_replacement == 'mean'
-        assert int_transformer.model_missing_values is False
+        assert int_transformer.missing_value_generation == 'random'
 
         float_transformer = config['transformers']['created_float']
         assert isinstance(float_transformer, FloatFormatter)
         assert float_transformer.missing_value_replacement == 'mean'
-        assert float_transformer.model_missing_values is False
+        assert float_transformer.missing_value_generation == 'random'
 
         assert isinstance(config['transformers']['bool'], LabelEncoder)
         assert isinstance(config['transformers']['created_bool'], LabelEncoder)
         assert isinstance(config['transformers']['categorical'], LabelEncoder)
         assert isinstance(config['transformers']['created_categorical'], LabelEncoder)
 
         assert isinstance(config['transformers']['int'], FloatFormatter)
@@ -1085,15 +1085,15 @@
         first_name_transformer = config['transformers']['first_name']
         assert first_name_transformer == 'AnonymizedFaker'
         assert primary_regex_generator == 'RegexGenerator'
 
         datetime_transformer = config['transformers']['date']
         assert isinstance(datetime_transformer, UnixTimestampEncoder)
         assert datetime_transformer.missing_value_replacement == 'mean'
-        assert datetime_transformer.model_missing_values is False
+        assert datetime_transformer.missing_value_generation == 'random'
         assert datetime_transformer.datetime_format == '%Y-%m-%d'
         assert dp._primary_key == 'id'
 
         dp.create_anonymized_transformer.calls == [
             call('email', {'sdtype': 'email', 'pii': True, 'locales': locales}),
             call('first_name', {'sdtype': 'first_name', 'locales': locales})
```

### Comparing `sdv-1.2.0.dev0/tests/unit/data_processing/test_datetime_formatter.py` & `sdv-1.2.0.dev1/tests/unit/data_processing/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/data_processing/test_numerical_formatter.py` & `sdv-1.2.0.dev1/tests/unit/data_processing/test_numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/data_processing/test_utils.py` & `sdv-1.2.0.dev1/tests/unit/data_processing/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/datasets/test_demo.py` & `sdv-1.2.0.dev1/tests/unit/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/datasets/test_local.py` & `sdv-1.2.0.dev1/tests/unit/datasets/test_local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/evaluation/test_multi_table.py` & `sdv-1.2.0.dev1/tests/unit/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/evaluation/test_single_table.py` & `sdv-1.2.0.dev1/tests/unit/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/lite/test_single_table.py` & `sdv-1.2.0.dev1/tests/unit/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/metadata/test_anonymization.py` & `sdv-1.2.0.dev1/tests/unit/metadata/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/metadata/test_metadata_upgrader.py` & `sdv-1.2.0.dev1/tests/unit/metadata/test_metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/metadata/test_multi_table.py` & `sdv-1.2.0.dev1/tests/unit/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/metadata/test_single_table.py` & `sdv-1.2.0.dev1/tests/unit/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/multi_table/test_base.py` & `sdv-1.2.0.dev1/tests/unit/multi_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/multi_table/test_hma.py` & `sdv-1.2.0.dev1/tests/unit/multi_table/test_hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/sampling/test_hierarchical_sampler.py` & `sdv-1.2.0.dev1/tests/unit/sampling/test_hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/sampling/test_independent_sampler.py` & `sdv-1.2.0.dev1/tests/unit/sampling/test_independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/sampling/test_tabular.py` & `sdv-1.2.0.dev1/tests/unit/sampling/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/sequential/test_par.py` & `sdv-1.2.0.dev1/tests/unit/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/single_table/test_base.py` & `sdv-1.2.0.dev1/tests/unit/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/single_table/test_copulagan.py` & `sdv-1.2.0.dev1/tests/unit/single_table/test_copulagan.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,16 +211,16 @@
         })
 
         # Run
         config = instance._create_gaussian_normalizer_config(processed_data)
 
         # Assert
         expected_calls = [
-            call(model_missing_values=True, distribution=GammaUnivariate),
-            call(model_missing_values=True, distribution=BetaUnivariate),
+            call(missing_value_generation='from_column', distribution=GammaUnivariate),
+            call(missing_value_generation='from_column', distribution=BetaUnivariate),
         ]
         expected_config = {
             'transformers': {
                 'name': None,
                 'age': mock_rdt.transformers.GaussianNormalizer.return_value,
                 'account': mock_rdt.transformers.GaussianNormalizer.return_value,
                 'name#age': None
```

### Comparing `sdv-1.2.0.dev0/tests/unit/single_table/test_copulas.py` & `sdv-1.2.0.dev1/tests/unit/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/single_table/test_ctgan.py` & `sdv-1.2.0.dev1/tests/unit/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/single_table/test_utils.py` & `sdv-1.2.0.dev1/tests/unit/single_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/test___init__.py` & `sdv-1.2.0.dev1/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/unit/test_utils.py` & `sdv-1.2.0.dev1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev0/tests/utils.py` & `sdv-1.2.0.dev1/tests/utils.py`

 * *Files identical despite different names*

