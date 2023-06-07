# Comparing `tmp/LensCalcPy-0.0.1.tar.gz` & `tmp/LensCalcPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LensCalcPy-0.0.1.tar", last modified: Tue May 16 19:35:00 2023, max compression
+gzip compressed data, was "LensCalcPy-0.0.2.tar", last modified: Wed Jun  7 17:02:24 2023, max compression
```

## Comparing `LensCalcPy-0.0.1.tar` & `LensCalcPy-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-05-16 19:35:00.325748 LensCalcPy-0.0.1/
--rw-rw-r--   0 nolansmyth   (501) staff       (20)    11337 2023-01-20 02:50:04.000000 LensCalcPy-0.0.1/LICENSE
-drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-05-16 19:35:00.320387 LensCalcPy-0.0.1/LensCalcPy/
--rw-r--r--   0 nolansmyth   (501) staff       (20)       22 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/__init__.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)    14407 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/_modidx.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)      138 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/core.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)    11685 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/ffp.py
-drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-05-16 19:35:00.324928 LensCalcPy-0.0.1/LensCalcPy/interpolations/
--rw-r--r--   0 nolansmyth   (501) staff       (20)        0 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/interpolations/__init__.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)      303 2023-05-16 19:17:14.000000 LensCalcPy-0.0.1/LensCalcPy/interpolations/interps.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)    27456 2023-05-15 02:20:48.000000 LensCalcPy-0.0.1/LensCalcPy/interpolations/m_avg_interp.pkl
--rw-r--r--   0 nolansmyth   (501) staff       (20)    42176 2023-05-16 00:02:08.000000 LensCalcPy-0.0.1/LensCalcPy/interpolations/ut_interp_m31.pkl
--rw-r--r--   0 nolansmyth   (501) staff       (20)     1905 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/lens.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)     2112 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/parameters.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)     2409 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/pbh.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)     2992 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/stats.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)     7179 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/survey.py
--rw-r--r--   0 nolansmyth   (501) staff       (20)     7618 2023-05-16 19:29:05.000000 LensCalcPy-0.0.1/LensCalcPy/utils.py
-drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-05-16 19:35:00.323811 LensCalcPy-0.0.1/LensCalcPy.egg-info/
--rw-r--r--   0 nolansmyth   (501) staff       (20)     5255 2023-05-16 19:35:00.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/PKG-INFO
--rw-r--r--   0 nolansmyth   (501) staff       (20)      657 2023-05-16 19:35:00.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/SOURCES.txt
--rw-r--r--   0 nolansmyth   (501) staff       (20)        1 2023-05-16 19:35:00.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/dependency_links.txt
--rw-r--r--   0 nolansmyth   (501) staff       (20)       42 2023-05-16 19:35:00.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/entry_points.txt
--rw-r--r--   0 nolansmyth   (501) staff       (20)        1 2023-04-22 23:50:14.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/not-zip-safe
--rw-r--r--   0 nolansmyth   (501) staff       (20)       50 2023-05-16 19:35:00.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/requires.txt
--rw-r--r--   0 nolansmyth   (501) staff       (20)       11 2023-05-16 19:35:00.000000 LensCalcPy-0.0.1/LensCalcPy.egg-info/top_level.txt
--rw-rw-r--   0 nolansmyth   (501) staff       (20)      111 2023-01-20 02:50:04.000000 LensCalcPy-0.0.1/MANIFEST.in
--rw-r--r--   0 nolansmyth   (501) staff       (20)     5255 2023-05-16 19:35:00.325506 LensCalcPy-0.0.1/PKG-INFO
--rw-r--r--   0 nolansmyth   (501) staff       (20)     4475 2023-05-16 19:31:05.000000 LensCalcPy-0.0.1/README.md
--rw-r--r--   0 nolansmyth   (501) staff       (20)      961 2023-05-16 19:23:34.000000 LensCalcPy-0.0.1/settings.ini
--rw-r--r--   0 nolansmyth   (501) staff       (20)       38 2023-05-16 19:35:00.325821 LensCalcPy-0.0.1/setup.cfg
--rw-rw-r--   0 nolansmyth   (501) staff       (20)     2734 2023-05-16 18:54:33.000000 LensCalcPy-0.0.1/setup.py
+drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-06-07 17:02:24.155654 LensCalcPy-0.0.2/
+-rw-rw-r--   0 nolansmyth   (501) staff       (20)    11337 2023-01-20 02:50:04.000000 LensCalcPy-0.0.2/LICENSE
+drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-06-07 17:02:24.153021 LensCalcPy-0.0.2/LensCalcPy/
+-rw-r--r--   0 nolansmyth   (501) staff       (20)       22 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/__init__.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)    12435 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/_modidx.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)      138 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/core.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     8690 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/ffp.py
+drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-06-07 17:02:24.154564 LensCalcPy-0.0.2/LensCalcPy/interpolations/
+-rw-r--r--   0 nolansmyth   (501) staff       (20)        0 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/interpolations/__init__.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)      158 2023-06-02 18:37:42.000000 LensCalcPy-0.0.2/LensCalcPy/interpolations/interps.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)    42176 2023-05-16 00:02:08.000000 LensCalcPy-0.0.2/LensCalcPy/interpolations/ut_interp_m31.pkl
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     1854 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/lens.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     2306 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/parameters.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     2438 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/pbh.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     2784 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/stats.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     3758 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/survey.py
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     8139 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/LensCalcPy/utils.py
+drwxr-xr-x   0 nolansmyth   (501) staff       (20)        0 2023-06-07 17:02:24.154194 LensCalcPy-0.0.2/LensCalcPy.egg-info/
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     5343 2023-06-07 17:02:24.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/PKG-INFO
+-rw-r--r--   0 nolansmyth   (501) staff       (20)      614 2023-06-07 17:02:24.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/SOURCES.txt
+-rw-r--r--   0 nolansmyth   (501) staff       (20)        1 2023-06-07 17:02:24.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/dependency_links.txt
+-rw-r--r--   0 nolansmyth   (501) staff       (20)       42 2023-06-07 17:02:24.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/entry_points.txt
+-rw-r--r--   0 nolansmyth   (501) staff       (20)        1 2023-04-22 23:50:14.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/not-zip-safe
+-rw-r--r--   0 nolansmyth   (501) staff       (20)       50 2023-06-07 17:02:24.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/requires.txt
+-rw-r--r--   0 nolansmyth   (501) staff       (20)       11 2023-06-07 17:02:24.000000 LensCalcPy-0.0.2/LensCalcPy.egg-info/top_level.txt
+-rw-rw-r--   0 nolansmyth   (501) staff       (20)      111 2023-01-20 02:50:04.000000 LensCalcPy-0.0.2/MANIFEST.in
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     5343 2023-06-07 17:02:24.155428 LensCalcPy-0.0.2/PKG-INFO
+-rw-r--r--   0 nolansmyth   (501) staff       (20)     4563 2023-06-05 19:31:27.000000 LensCalcPy-0.0.2/README.md
+-rw-r--r--   0 nolansmyth   (501) staff       (20)      866 2023-06-07 17:02:19.000000 LensCalcPy-0.0.2/settings.ini
+-rw-r--r--   0 nolansmyth   (501) staff       (20)       38 2023-06-07 17:02:24.155721 LensCalcPy-0.0.2/setup.cfg
+-rw-rw-r--   0 nolansmyth   (501) staff       (20)     2734 2023-05-16 18:54:33.000000 LensCalcPy-0.0.2/setup.py
```

### Comparing `LensCalcPy-0.0.1/LICENSE` & `LensCalcPy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LensCalcPy-0.0.1/LensCalcPy/_modidx.py` & `LensCalcPy-0.0.2/LensCalcPy/_modidx.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,41 +7,30 @@
                 'lib_path': 'LensCalcPy'},
   'syms': { 'LensCalcPy.core': {'LensCalcPy.core.foo': ('mw.html#foo', 'LensCalcPy/core.py')},
             'LensCalcPy.ffp': { 'LensCalcPy.ffp.Ffp': ('ffp.html#ffp', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.__init__': ('ffp.html#ffp.__init__', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.__str__': ('ffp.html#ffp.__str__', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.compute_differential_rate': ( 'ffp.html#ffp.compute_differential_rate',
                                                                                   'LensCalcPy/ffp.py'),
+                                'LensCalcPy.ffp.Ffp.differential_rate': ('ffp.html#ffp.differential_rate', 'LensCalcPy/ffp.py'),
+                                'LensCalcPy.ffp.Ffp.differential_rate_integrand': ( 'ffp.html#ffp.differential_rate_integrand',
+                                                                                    'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.differential_rate_integrand_m31': ( 'ffp.html#ffp.differential_rate_integrand_m31',
                                                                                         'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.differential_rate_integrand_mw': ( 'ffp.html#ffp.differential_rate_integrand_mw',
                                                                                        'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.differential_rate_m31': ('ffp.html#ffp.differential_rate_m31', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.differential_rate_mw': ('ffp.html#ffp.differential_rate_mw', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.differential_rate_total': ('ffp.html#ffp.differential_rate_total', 'LensCalcPy/ffp.py'),
+                                'LensCalcPy.ffp.Ffp.mass_func': ('ffp.html#ffp.mass_func', 'LensCalcPy/ffp.py'),
+                                'LensCalcPy.ffp.Ffp.pl_norm': ('ffp.html#ffp.pl_norm', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.Ffp.umin_upper_bound': ('ffp.html#ffp.umin_upper_bound', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation': ('ffp.html#ffppopulation', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.__init__': ('ffp.html#ffppopulation.__init__', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.__str__': ('ffp.html#ffppopulation.__str__', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.compute_differential_rate': ( 'ffp.html#ffppopulation.compute_differential_rate',
-                                                                                            'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.differential_rate_total': ( 'ffp.html#ffppopulation.differential_rate_total',
-                                                                                          'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.generate_ffps': ('ffp.html#ffppopulation.generate_ffps', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.generate_sample': ( 'ffp.html#ffppopulation.generate_sample',
-                                                                                  'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.get_weighted_te': ( 'ffp.html#ffppopulation.get_weighted_te',
-                                                                                  'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.FfpPopulation.make_te_interp': ( 'ffp.html#ffppopulation.make_te_interp',
-                                                                                 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.cut': ('ffp.html#cut', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.einasto': ('ffp.html#einasto', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.fE': ('ffp.html#fe', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.m_avg_ffp': ('ffp.html#m_avg_ffp', 'LensCalcPy/ffp.py'),
-                                'LensCalcPy.ffp.make_m_avg_interp': ('ffp.html#make_m_avg_interp', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_FFPs_m31': ('ffp.html#rho_ffps_m31', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_FFPs_mw': ('ffp.html#rho_ffps_mw', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_bulge_m31': ('ffp.html#rho_bulge_m31', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_bulge_mw': ('ffp.html#rho_bulge_mw', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_disk_m31': ('ffp.html#rho_disk_m31', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_nucleus_m31': ('ffp.html#rho_nucleus_m31', 'LensCalcPy/ffp.py'),
                                 'LensCalcPy.ffp.rho_thick_mw': ('ffp.html#rho_thick_mw', 'LensCalcPy/ffp.py'),
@@ -72,15 +61,14 @@
                                 'LensCalcPy.pbh.Pbh.differential_rate_m31': ('pbh.html#pbh.differential_rate_m31', 'LensCalcPy/pbh.py'),
                                 'LensCalcPy.pbh.Pbh.differential_rate_mw': ('pbh.html#pbh.differential_rate_mw', 'LensCalcPy/pbh.py'),
                                 'LensCalcPy.pbh.Pbh.differential_rate_total': ('pbh.html#pbh.differential_rate_total', 'LensCalcPy/pbh.py'),
                                 'LensCalcPy.pbh.Pbh.umin_upper_bound': ('pbh.html#pbh.umin_upper_bound', 'LensCalcPy/pbh.py')},
             'LensCalcPy.stats': { 'LensCalcPy.stats.generate_observed_counts_with_bump': ( 'stats.html#generate_observed_counts_with_bump',
                                                                                            'LensCalcPy/stats.py'),
                                   'LensCalcPy.stats.get_MLE_params': ('stats.html#get_mle_params', 'LensCalcPy/stats.py'),
-                                  'LensCalcPy.stats.get_observed_counts': ('stats.html#get_observed_counts', 'LensCalcPy/stats.py'),
                                   'LensCalcPy.stats.likelihood': ('stats.html#likelihood', 'LensCalcPy/stats.py'),
                                   'LensCalcPy.stats.llr_test': ('stats.html#llr_test', 'LensCalcPy/stats.py'),
                                   'LensCalcPy.stats.neg_log_likelihood': ('stats.html#neg_log_likelihood', 'LensCalcPy/stats.py'),
                                   'LensCalcPy.stats.power_law': ('stats.html#power_law', 'LensCalcPy/stats.py')},
             'LensCalcPy.survey': { 'LensCalcPy.survey.Survey': ('survey.html#survey', 'LensCalcPy/survey.py'),
                                    'LensCalcPy.survey.Survey.__init__': ('survey.html#survey.__init__', 'LensCalcPy/survey.py'),
                                    'LensCalcPy.survey.Survey.__str__': ('survey.html#survey.__str__', 'LensCalcPy/survey.py'),
@@ -89,19 +77,15 @@
                                    'LensCalcPy.survey.Survey.get_crossing_time_rates': ( 'survey.html#survey.get_crossing_time_rates',
                                                                                          'LensCalcPy/survey.py'),
                                    'LensCalcPy.survey.Survey.get_crossing_times_rates_ffp': ( 'survey.html#survey.get_crossing_times_rates_ffp',
                                                                                               'LensCalcPy/survey.py'),
                                    'LensCalcPy.survey.Survey.get_crossing_times_rates_pbh': ( 'survey.html#survey.get_crossing_times_rates_pbh',
                                                                                               'LensCalcPy/survey.py'),
                                    'LensCalcPy.survey.Survey.get_events_observed': ( 'survey.html#survey.get_events_observed',
-                                                                                     'LensCalcPy/survey.py'),
-                                   'LensCalcPy.survey.Survey.get_lens_masses': ( 'survey.html#survey.get_lens_masses',
-                                                                                 'LensCalcPy/survey.py'),
-                                   'LensCalcPy.survey.Survey.get_num_events': ('survey.html#survey.get_num_events', 'LensCalcPy/survey.py'),
-                                   'LensCalcPy.survey.Survey.num_pbh': ('survey.html#survey.num_pbh', 'LensCalcPy/survey.py')},
+                                                                                     'LensCalcPy/survey.py')},
             'LensCalcPy.utils': { 'LensCalcPy.utils.density_m31': ('utils.html#density_m31', 'LensCalcPy/utils.py'),
                                   'LensCalcPy.utils.density_mw': ('utils.html#density_mw', 'LensCalcPy/utils.py'),
                                   'LensCalcPy.utils.displacement': ('utils.html#displacement', 'LensCalcPy/utils.py'),
                                   'LensCalcPy.utils.dist': ('utils.html#dist', 'LensCalcPy/utils.py'),
                                   'LensCalcPy.utils.dist_m31': ('utils.html#dist_m31', 'LensCalcPy/utils.py'),
                                   'LensCalcPy.utils.dist_mw': ('utils.html#dist_mw', 'LensCalcPy/utils.py'),
                                   'LensCalcPy.utils.einstein_rad': ('utils.html#einstein_rad', 'LensCalcPy/utils.py'),
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy/interpolations/ut_interp_m31.pkl` & `LensCalcPy-0.0.2/LensCalcPy/interpolations/ut_interp_m31.pkl`

 * *Files identical despite different names*

### Comparing `LensCalcPy-0.0.1/LensCalcPy/lens.py` & `LensCalcPy-0.0.2/LensCalcPy/lens.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,10 +54,9 @@
             umin_bounds = [0, ut]
             d_bounds = [0, ds]
             result, error = nquad(integrand_func, [umin_bounds, d_bounds], args=[t])
             return result
 
     @abstractmethod
     def compute_differential_rate(self, t, finite=False):
-        # return self.differential_rate(t, finite)
         pass
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy/parameters.py` & `LensCalcPy-0.0.2/LensCalcPy/parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,26 +24,28 @@
 # %% ../nbs/05_parameters.ipynb 4
 #Survey parameters
 # ds = 9.0 # kpc
 # dsM31 = 770 # kpc
 # survey_area = 0.16 # survey area in square degrees
 # obsTime = 1825*24 # observation time in hours
 # n_sources = 8.7e7 # number of sources in the survey
+
 # l = 1.0 #degrees
 # b = -1.03 #degrees
+l = 121.2 #degrees
+b = -21.6 #degrees
+
 
-l = 121.2
-b = -21.6
-ds = 770
+ds = 770 #distance to source in kpc
 dsM31 = 770 # kpc
-obsTime = 7
-survey_area = 0
-n_sources = 8.7e7
-efficiency = 0.6
-lam = 6000
+obsTime = 7 # observation time in hours
+survey_area = 0 # survey area in square degrees
+n_sources = 8.7e7 # number of sources in the survey
+efficiency = 0.6 # efficiency of the survey
+lam = 6000 # wavelength in angstroms
 
 
 # %% ../nbs/05_parameters.ipynb 5
 # Disk Params
 zthinSol = 0.329  # scale height of thin disk in solar neighborhood, kpc
 zthickSol = 0.903  # scale height of thick disk in solar neighborhood
 zthin45 = 0.6 * zthinSol  # scale height, kpc
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy/pbh.py` & `LensCalcPy-0.0.2/LensCalcPy/pbh.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from tqdm import tqdm
 # from multiprocessing import Pool
 from pathos.multiprocessing import ProcessingPool as Pool
 import functools
 import pickle
 from abc import ABC, abstractmethod
 
+from fastcore.test import *
+
 # %% ../nbs/00_pbh.ipynb 5
 class Pbh(Lens):
     """A class to represent a PBH population"""
 
     def __init__(self,
                 mass: float, # PBH mass in solar masses
                 f_dm: float # PBH fraction of the DM density
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy/stats.py` & `LensCalcPy-0.0.2/LensCalcPy/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_stats.ipynb.
 
 # %% auto 0
-__all__ = ['power_law', 'likelihood', 'generate_observed_counts_with_bump', 'neg_log_likelihood', 'get_MLE_params', 'llr_test',
-           'get_observed_counts']
+__all__ = ['power_law', 'likelihood', 'generate_observed_counts_with_bump', 'neg_log_likelihood', 'get_MLE_params', 'llr_test']
 
 # %% ../nbs/06_stats.ipynb 3
 import numpy as np
 from scipy.stats import poisson, norm
 from scipy.optimize import minimize
 import matplotlib.pyplot as plt
 from scipy.stats import chi2
@@ -63,12 +62,7 @@
     #log likelihood of the alternative hypothesis (non-zero bump height)
     ll_alt = -neg_log_likelihood(optimized_params, bin_centers, observed_counts)
 
     llr = 2 * (ll_alt - ll_null)
 
     return llr
     
-
-# %% ../nbs/06_stats.ipynb 17
-def get_observed_counts(lens_masses, bin_edges):
-    observed_counts, _ = np.histogram(lens_masses, bins=bin_edges)
-    return observed_counts
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy/utils.py` & `LensCalcPy-0.0.2/LensCalcPy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_utils.ipynb.
 
 # %% auto 0
-__all__ = ['ut_interp', 'm_avg_interp', 'm_low_interp', 'm_high_interp', 'dist_mw', 'dist_m31', 'density_mw', 'density_m31',
-           'mass_enclosed_mw', 'mass_enclosed_m31', 'velocity_dispersion_mw', 'velocity_dispersion_m31', 'dist',
-           'einstein_rad', 'velocity_radial', 'get_primed_coords', 'scientific_format', 'w_func', 'rho_func',
-           'magnification', 'magnification_wave', 'displacement', 'integrand_polar_wave', 'integrand_polar',
-           'magnification_finite_wave', 'magnification_finite', 'u_t_finite', 'u_t_finite_wave', 'make_ut_interp']
+__all__ = ['ut_interp', 'm_low_interp', 'm_high_interp', 'dist_mw', 'dist_m31', 'density_mw', 'density_m31', 'mass_enclosed_mw',
+           'mass_enclosed_m31', 'velocity_dispersion_mw', 'velocity_dispersion_m31', 'dist', 'einstein_rad',
+           'velocity_radial', 'get_primed_coords', 'scientific_format', 'w_func', 'rho_func', 'magnification',
+           'magnification_wave', 'displacement', 'integrand_polar_wave', 'integrand_polar', 'magnification_finite_wave',
+           'magnification_finite', 'u_t_finite', 'u_t_finite_wave', 'make_ut_interp']
 
 # %% ../nbs/04_utils.ipynb 3
 from .parameters import *
 import numpy as np
 from numpy import pi
 from scipy.integrate import quad, nquad
 from scipy.optimize import brentq
 from pathos.multiprocessing import ProcessingPool as Pool
 from scipy.interpolate import interp2d
 import pickle
-from .interpolations.interps import ut_interp, m_avg_interp
+from .interpolations.interps import ut_interp
 
 import matplotlib.pyplot as plt
 
+from fastcore.test import *
+
 # %% ../nbs/04_utils.ipynb 4
-# #Put 0 indent assignments so that variables will be in __all__
+#Put 0 indent assignments so that variables will be in __all__
 ut_interp = ut_interp
-m_avg_interp = m_avg_interp
 
-# %% ../nbs/04_utils.ipynb 6
+# %% ../nbs/04_utils.ipynb 5
 def dist_mw(d: float, # distance from the Sun in kpc
             ) -> float: #distance to the MW center in kpc
     return np.sqrt(d**2 + rEarth**2 - 2*d*rEarth*np.cos(np.radians(l))*np.cos(np.radians(b)))
 
 def dist_m31(d: float, # distance from the Sun in kpc
              ) -> float: #distance to the M31 center in kpc
             return dsM31 - d
@@ -48,51 +49,68 @@
 
 def mass_enclosed_m31(r: float  # distance to M31 center in kpc
                         ) -> float : # enclosed DM mass in Msun
     return 4*pi * rhocM31 * rsM31**3 * (np.log(1 + r/rsM31) - (r/rsM31)/(1 + r/rsM31))
 
 def velocity_dispersion_mw(r: float, # distance from the MW center in kpc
                         ) -> float: # velocity dispersion in km/s
+    if r == 0:
+        return 0
     return np.sqrt(G * mass_enclosed_mw(r) / r) 
 
 def velocity_dispersion_m31(r: float, # distance from the M31 center in kpc
                         ) -> float: # velocity dispersion in km/s
+    if r == 0:
+        return 0
     return np.sqrt(G * mass_enclosed_m31(r) / r)
 
 def dist(d: float # distance from the Sun in kpc
          ) -> float: #weighted lensing distance in kpc
     return d * (1 - d/ds)
 
 def einstein_rad(d: float, # distance from the Sun in kpc
                  mass: float, # mass of the lens in Msun
                  ) -> float:
     return (4 * G * mass * dist(d)/c**2)**(1/2)
 
-
 def velocity_radial(d: float, # distance from the Sun in kpc
                     mass: float, # mass of the lens in Msun
                     umin: float, # minimum impact parameter
                     t: float, # crossing time in hours
                     ut: float, # threshold impact parameter
                     ) -> float: # radial velocity in km/s
     return 2*einstein_rad(d, mass) * (ut**2 - umin**2)**(1/2) / t * kpctokm
 
 # from below 16 of https://iopscience.iop.org/article/10.3847/1538-4357/ac07a8/pdf*)
 # alphabar = 27 Degrees xp-axis is aligned with the major axis
 # of the Galactic bar,where \[Alpha]bar=27\[Degree] is applied as the bar angle.
-# assuming z ~= 0 and we are looking at line of sight to galactic center from Sun
-# galactocentric coordniates x', y' as function of d, distance from Sun
+# galactocentric coordniates x', y', z' as function of d, distance from Sun
 
-def get_primed_coords(d: float # distance from Sun
+def get_primed_coords(d: float, # distance from Sun in km
+                      l: float = l, # galactic longitude in degrees
+                      b: float = b, # galactic latitude in degrees
                       )-> tuple:
-    """Get galactocentric coordinates x', y' as function of d, distance from Sun
+    """Get galactocentric coordinates x', y' given galactic latitude and longitude l, b, and distance d
     """
-    x = rEarth - d
-    y = 0
-    return (x**2 + y**2)**0.5 * np.cos(alphabar*pi/180), (x**2 + y**2)**0.5 * np.sin(alphabar*pi/180)
+    # convert angles from degrees to radians
+    l_rad = np.deg2rad(l)
+    b_rad = np.deg2rad(b)
+    alpha_rad = np.deg2rad(alphabar)
+
+    # calculate unrotated Cartesian coordinates
+    x_unrot = rEarth - d * np.cos(b_rad) * np.cos(l_rad)
+    y_unrot = d * np.cos(b_rad) * np.sin(l_rad)
+
+    # rotate the coordinates
+    x_prime = x_unrot * np.cos(alpha_rad) - y_unrot * np.sin(alpha_rad)
+    y_prime = x_unrot * np.sin(alpha_rad) + y_unrot * np.cos(alpha_rad)
+
+    z_prime = d * np.sin(b_rad)
+
+    return x_prime, y_prime, z_prime
 
 def scientific_format(x, pos):
     """
     Formats a number in scientific notation in latex
     """
     a, b = '{:.1e}'.format(x).split('e')
     b = int(b)
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy.egg-info/PKG-INFO` & `LensCalcPy-0.0.2/LensCalcPy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LensCalcPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculate Microlensing Observables
 Home-page: https://github.com/NolanSmyth/LensCalcPy
 Author: Nolan Smyth
 Author-email: nolanwsmyth@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,68 +31,69 @@
 
 ``` sh
 pip install LensCalcPy
 ```
 
 ## How to use
 
-### Note that all functionality is currently for a survey of the MW bulge. Will be able to customize to other surveys soon.
-
 We can calculate the distribution of crossing times for a given PBH
 population
 
 ``` python
 f_pbh = 1 # fraction of dark matter in PBHs
 
 ts = np.logspace(-2, 1, 30)
 pbhs = [Pbh(10**(i), f_pbh) for i in np.linspace(-9, -7, 3)]
 result = np.zeros((len(pbhs), len(ts)))
 for i, pbh in enumerate(pbhs):
     result[i, :] = pbh.compute_differential_rate(ts)
 ```
 
+    /Users/nolansmyth/opt/anaconda3/lib/python3.9/site-packages/scipy/integrate/quadpack.py:879: IntegrationWarning: The integral is probably divergent, or slowly convergent.
+      quad_r = quad(f, low, high, args=args, full_output=self.full_output,
+
 ``` python
 for i, pbh in enumerate(pbhs):
-    # plt.loglog(ts, result[i], label=r"$M_{\rm{PBH}} = " + str(pbh.m_pbh) + "M_{\odot}$")
     plt.loglog(ts, result[i], label=r"$M_{\rm{PBH}} = $" + scientific_format(pbh.mass,0) + "$M_{\odot}$")
 
-
-plt.xlabel(r"$t$ [hr]")
-plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]")
+plt.xlabel(r"$t_E$ [h]", fontsize=16)
+plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]", fontsize=16)
 plt.xlim(1e-2, 1e1)
 plt.ylim(1e-10, 1e-4)
 
 plt.legend()
 plt.show()
 ```
 
 ![](index_files/figure-commonmark/cell-3-output-1.png)
 
 Similarly, we can calculate the distribution of crossing times for an
 FFP population
 
 ``` python
-mMin = 1e-7  # solar masses
 alpha = 2
-fp = FfpPopulation(mMin, alpha)
+fp = Ffp(alpha)
 ```
 
 ``` python
-ts = np.logspace(-2, np.log10(1e3), num=100)
+ts = np.logspace(-2, np.log10(1e3), num=30)
 diff_rates = fp.compute_differential_rate(ts, finite=False)
+```
 
+``` python
+#Note: event rate normalized to 1 FFP/ISO per host star
 plt.loglog(ts, diff_rates, color="blue")
 plt.xlabel(r"$t_E$ [h]", fontsize=16)
 plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]", fontsize=16)
 plt.xlim([0.009, 1e3])
-plt.ylim([1e-20, 1e-7])
+plt.ylim([1e-32, 1e-13])
 plt.show()
 ```
 
-![](index_files/figure-commonmark/cell-5-output-1.png)
+![](index_files/figure-commonmark/cell-6-output-1.png)
 
 ## Statistics
 
 Eventually will be able to perform statistical analysis on the
 distributions of crossing times for a given population and compare with
 output from [PopSyCLE](https://github.com/jluastro/PopSyCLE/). For now,
 here’s a toy example assuming perfect mass reconstruction
@@ -138,15 +139,15 @@
 plt.title("Observed Counts vs Initial Expected Counts")
 
 
 plt.tight_layout()
 plt.show()
 ```
 
-![](index_files/figure-commonmark/cell-7-output-1.png)
+![](index_files/figure-commonmark/cell-8-output-1.png)
 
 ``` python
 # Calculate the likelihood ratio test statistic
 lr_statistic = llr_test(bin_centers, observed_counts)
 
 # Calculate the p-value using a chi-square distribution
 p_value = chi2.sf(lr_statistic, df=2)  # Two degrees of freedom for the difference in number of parameters
```

### Comparing `LensCalcPy-0.0.1/LensCalcPy.egg-info/SOURCES.txt` & `LensCalcPy-0.0.2/LensCalcPy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 LensCalcPy.egg-info/dependency_links.txt
 LensCalcPy.egg-info/entry_points.txt
 LensCalcPy.egg-info/not-zip-safe
 LensCalcPy.egg-info/requires.txt
 LensCalcPy.egg-info/top_level.txt
 LensCalcPy/interpolations/__init__.py
 LensCalcPy/interpolations/interps.py
-LensCalcPy/interpolations/m_avg_interp.pkl
 LensCalcPy/interpolations/ut_interp_m31.pkl
```

### Comparing `LensCalcPy-0.0.1/PKG-INFO` & `LensCalcPy-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LensCalcPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculate Microlensing Observables
 Home-page: https://github.com/NolanSmyth/LensCalcPy
 Author: Nolan Smyth
 Author-email: nolanwsmyth@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,68 +31,69 @@
 
 ``` sh
 pip install LensCalcPy
 ```
 
 ## How to use
 
-### Note that all functionality is currently for a survey of the MW bulge. Will be able to customize to other surveys soon.
-
 We can calculate the distribution of crossing times for a given PBH
 population
 
 ``` python
 f_pbh = 1 # fraction of dark matter in PBHs
 
 ts = np.logspace(-2, 1, 30)
 pbhs = [Pbh(10**(i), f_pbh) for i in np.linspace(-9, -7, 3)]
 result = np.zeros((len(pbhs), len(ts)))
 for i, pbh in enumerate(pbhs):
     result[i, :] = pbh.compute_differential_rate(ts)
 ```
 
+    /Users/nolansmyth/opt/anaconda3/lib/python3.9/site-packages/scipy/integrate/quadpack.py:879: IntegrationWarning: The integral is probably divergent, or slowly convergent.
+      quad_r = quad(f, low, high, args=args, full_output=self.full_output,
+
 ``` python
 for i, pbh in enumerate(pbhs):
-    # plt.loglog(ts, result[i], label=r"$M_{\rm{PBH}} = " + str(pbh.m_pbh) + "M_{\odot}$")
     plt.loglog(ts, result[i], label=r"$M_{\rm{PBH}} = $" + scientific_format(pbh.mass,0) + "$M_{\odot}$")
 
-
-plt.xlabel(r"$t$ [hr]")
-plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]")
+plt.xlabel(r"$t_E$ [h]", fontsize=16)
+plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]", fontsize=16)
 plt.xlim(1e-2, 1e1)
 plt.ylim(1e-10, 1e-4)
 
 plt.legend()
 plt.show()
 ```
 
 ![](index_files/figure-commonmark/cell-3-output-1.png)
 
 Similarly, we can calculate the distribution of crossing times for an
 FFP population
 
 ``` python
-mMin = 1e-7  # solar masses
 alpha = 2
-fp = FfpPopulation(mMin, alpha)
+fp = Ffp(alpha)
 ```
 
 ``` python
-ts = np.logspace(-2, np.log10(1e3), num=100)
+ts = np.logspace(-2, np.log10(1e3), num=30)
 diff_rates = fp.compute_differential_rate(ts, finite=False)
+```
 
+``` python
+#Note: event rate normalized to 1 FFP/ISO per host star
 plt.loglog(ts, diff_rates, color="blue")
 plt.xlabel(r"$t_E$ [h]", fontsize=16)
 plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]", fontsize=16)
 plt.xlim([0.009, 1e3])
-plt.ylim([1e-20, 1e-7])
+plt.ylim([1e-32, 1e-13])
 plt.show()
 ```
 
-![](index_files/figure-commonmark/cell-5-output-1.png)
+![](index_files/figure-commonmark/cell-6-output-1.png)
 
 ## Statistics
 
 Eventually will be able to perform statistical analysis on the
 distributions of crossing times for a given population and compare with
 output from [PopSyCLE](https://github.com/jluastro/PopSyCLE/). For now,
 here’s a toy example assuming perfect mass reconstruction
@@ -138,15 +139,15 @@
 plt.title("Observed Counts vs Initial Expected Counts")
 
 
 plt.tight_layout()
 plt.show()
 ```
 
-![](index_files/figure-commonmark/cell-7-output-1.png)
+![](index_files/figure-commonmark/cell-8-output-1.png)
 
 ``` python
 # Calculate the likelihood ratio test statistic
 lr_statistic = llr_test(bin_centers, observed_counts)
 
 # Calculate the p-value using a chi-square distribution
 p_value = chi2.sf(lr_statistic, df=2)  # Two degrees of freedom for the difference in number of parameters
```

### Comparing `LensCalcPy-0.0.1/README.md` & `LensCalcPy-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,68 +9,69 @@
 
 ``` sh
 pip install LensCalcPy
 ```
 
 ## How to use
 
-### Note that all functionality is currently for a survey of the MW bulge. Will be able to customize to other surveys soon.
-
 We can calculate the distribution of crossing times for a given PBH
 population
 
 ``` python
 f_pbh = 1 # fraction of dark matter in PBHs
 
 ts = np.logspace(-2, 1, 30)
 pbhs = [Pbh(10**(i), f_pbh) for i in np.linspace(-9, -7, 3)]
 result = np.zeros((len(pbhs), len(ts)))
 for i, pbh in enumerate(pbhs):
     result[i, :] = pbh.compute_differential_rate(ts)
 ```
 
+    /Users/nolansmyth/opt/anaconda3/lib/python3.9/site-packages/scipy/integrate/quadpack.py:879: IntegrationWarning: The integral is probably divergent, or slowly convergent.
+      quad_r = quad(f, low, high, args=args, full_output=self.full_output,
+
 ``` python
 for i, pbh in enumerate(pbhs):
-    # plt.loglog(ts, result[i], label=r"$M_{\rm{PBH}} = " + str(pbh.m_pbh) + "M_{\odot}$")
     plt.loglog(ts, result[i], label=r"$M_{\rm{PBH}} = $" + scientific_format(pbh.mass,0) + "$M_{\odot}$")
 
-
-plt.xlabel(r"$t$ [hr]")
-plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]")
+plt.xlabel(r"$t_E$ [h]", fontsize=16)
+plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]", fontsize=16)
 plt.xlim(1e-2, 1e1)
 plt.ylim(1e-10, 1e-4)
 
 plt.legend()
 plt.show()
 ```
 
 ![](index_files/figure-commonmark/cell-3-output-1.png)
 
 Similarly, we can calculate the distribution of crossing times for an
 FFP population
 
 ``` python
-mMin = 1e-7  # solar masses
 alpha = 2
-fp = FfpPopulation(mMin, alpha)
+fp = Ffp(alpha)
 ```
 
 ``` python
-ts = np.logspace(-2, np.log10(1e3), num=100)
+ts = np.logspace(-2, np.log10(1e3), num=30)
 diff_rates = fp.compute_differential_rate(ts, finite=False)
+```
 
+``` python
+#Note: event rate normalized to 1 FFP/ISO per host star
 plt.loglog(ts, diff_rates, color="blue")
 plt.xlabel(r"$t_E$ [h]", fontsize=16)
 plt.ylabel(r"$d\Gamma/dt$ [events/star/hr/hr]", fontsize=16)
 plt.xlim([0.009, 1e3])
-plt.ylim([1e-20, 1e-7])
+plt.ylim([1e-32, 1e-13])
 plt.show()
 ```
 
-![](index_files/figure-commonmark/cell-5-output-1.png)
+![](index_files/figure-commonmark/cell-6-output-1.png)
 
 ## Statistics
 
 Eventually will be able to perform statistical analysis on the
 distributions of crossing times for a given population and compare with
 output from [PopSyCLE](https://github.com/jluastro/PopSyCLE/). For now,
 here’s a toy example assuming perfect mass reconstruction
@@ -116,15 +117,15 @@
 plt.title("Observed Counts vs Initial Expected Counts")
 
 
 plt.tight_layout()
 plt.show()
 ```
 
-![](index_files/figure-commonmark/cell-7-output-1.png)
+![](index_files/figure-commonmark/cell-8-output-1.png)
 
 ``` python
 # Calculate the likelihood ratio test statistic
 lr_statistic = llr_test(bin_centers, observed_counts)
 
 # Calculate the p-value using a chi-square distribution
 p_value = chi2.sf(lr_statistic, df=2)  # Two degrees of freedom for the difference in number of parameters
```

### Comparing `LensCalcPy-0.0.1/settings.ini` & `LensCalcPy-0.0.2/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = LensCalcPy
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = LensCalcPy
+version = 0.0.2
 min_python = 3.7
 license = apache2
-
-### nbdev ###
 doc_path = _docs
 lib_path = LensCalcPy
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://NolanSmyth.github.io
+doc_baseurl = /LensCalcPy
+git_url = https://github.com/NolanSmyth/LensCalcPy
+title = LensCalcPy
 audience = Developers
 author = Nolan Smyth
 author_email = nolanwsmyth@gmail.com
-copyright = 2023 onwards, %(author)s
+copyright = 2023 onwards, Nolan Smyth
 description = Calculate Microlensing Observables
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = NolanSmyth
-
-### Optional ###
 requirements = numpy scipy matplotlib astropy pathos tqdm
-# dev_requirements = 
-# console_scripts =
+black_formatting = False
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `LensCalcPy-0.0.1/setup.py` & `LensCalcPy-0.0.2/setup.py`

 * *Files identical despite different names*

