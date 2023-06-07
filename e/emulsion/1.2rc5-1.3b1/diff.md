# Comparing `tmp/emulsion-1.2rc5.tar.gz` & `tmp/emulsion-1.3beta1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emulsion-1.2rc5.tar", last modified: Wed Jun  7 09:29:15 2023, max compression
+gzip compressed data, was "dist/emulsion-1.3b1.tar", last modified: Thu Dec 15 12:43:18 2022, max compression
```

## Comparing `emulsion-1.2rc5.tar` & `emulsion-1.3beta1.tar`

### file list

```diff
@@ -1,216 +1,243 @@
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.073421 emulsion-1.2rc5/
--rw-r--r--   0 picault    (501) staff       (20)    10174 2023-06-07 09:29:02.000000 emulsion-1.2rc5/LICENSE
--rw-r--r--   0 picault    (501) staff       (20)      278 2023-06-07 09:29:01.000000 emulsion-1.2rc5/MANIFEST.in
--rw-r--r--   0 picault    (501) staff       (20)     1161 2023-06-07 09:29:02.000000 emulsion-1.2rc5/NOTICE
--rw-r--r--   0 picault    (501) staff       (20)     2818 2023-06-07 09:29:15.073302 emulsion-1.2rc5/PKG-INFO
--rw-r--r--   0 picault    (501) staff       (20)     4773 2023-06-07 09:29:02.000000 emulsion-1.2rc5/README.md
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.049968 emulsion-1.2rc5/doc/
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.050015 emulsion-1.2rc5/doc/html/
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.050119 emulsion-1.2rc5/doc/html/_static/
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.053620 emulsion-1.2rc5/doc/html/_static/benchmark/
--rw-r--r--   0 picault    (501) staff       (20)     1964 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model1-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)     7166 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model1.yaml
--rw-r--r--   0 picault    (501) staff       (20)     3042 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model2-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8348 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model2.yaml
--rw-r--r--   0 picault    (501) staff       (20)     3247 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model2b-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8552 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model2b.yaml
--rw-r--r--   0 picault    (501) staff       (20)     4212 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model3-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9926 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model3.yaml
--rw-r--r--   0 picault    (501) staff       (20)     5205 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model3b-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10917 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model3b.yaml
--rw-r--r--   0 picault    (501) staff       (20)     6859 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model4-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12564 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model4.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8486 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model5-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)    14248 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model5.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9929 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model6-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)    15822 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model6.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10581 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model7-short.yaml
--rw-r--r--   0 picault    (501) staff       (20)    16478 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/benchmark/model7.yaml
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.050278 emulsion-1.2rc5/doc/html/_static/models/
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.059517 emulsion-1.2rc5/doc/html/_static/models/features/
--rw-r--r--   0 picault    (501) staff       (20)     7978 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_ABC.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9784 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SEIRS.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9452 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9620 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIRS_periodic_risk.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10395 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11486 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_demo_prototypes.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11003 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_demo_random.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12332 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12790 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12266 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11079 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_age_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10550 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_aggreg.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9658 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_cumul_inc.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10235 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10670 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8445 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_duration.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11556 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/IBM_gest.yaml
--rw-r--r--   0 picault    (501) staff       (20)     7990 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_ABC.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9560 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SEIRS.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9098 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9966 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIRS_periodic_risk.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9917 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11501 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_demo_prototypes.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10720 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_demo_random.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12252 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12807 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11735 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9376 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_cumul_inc.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9584 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10555 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_lockdown.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10265 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10139 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8407 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/compart_duration.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9788 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_ABC-old.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8842 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_ABC.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9305 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_ABC2.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10201 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SEIRS.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9771 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10090 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIRS_periodic_risk.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10713 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11574 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_demo_prototypes.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11234 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_demo_random.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12810 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)    13458 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12477 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11487 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_age_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10972 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_aggreg.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9933 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_cumul_inc.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10552 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8960 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_lockdown.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10613 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11491 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12720 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_metapop_params.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10881 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8890 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_duration.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12031 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/features/hybrid_gest.yaml
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.059618 emulsion-1.2rc5/doc/html/_static/models/quickstart/
--rw-r--r--   0 picault    (501) staff       (20)    13418 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/quickstart/quickstart.yaml
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.060022 emulsion-1.2rc5/doc/html/_static/models/transition/
--rw-r--r--   0 picault    (501) staff       (20)      755 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/transition/compart_SIR_JA_demo-1.1.yaml
--rw-r--r--   0 picault    (501) staff       (20)     1039 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/transition/compart_SIR_JA_demo-1.2.yaml
--rw-r--r--   0 picault    (501) staff       (20)      412 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/transition/hybrid_SIR_JA_demo-1.1.yaml
--rw-r--r--   0 picault    (501) staff       (20)      341 2023-06-07 09:29:14.000000 emulsion-1.2rc5/doc/html/_static/models/transition/hybrid_SIR_JA_demo-1.2.yaml
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.050513 emulsion-1.2rc5/models/
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.065997 emulsion-1.2rc5/models/features/
--rw-r--r--   0 picault    (501) staff       (20)     7978 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_ABC.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9784 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SEIRS.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9452 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9620 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIRS_periodic_risk.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10395 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11486 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_demo_prototypes.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11003 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_demo_random.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12332 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)     7512 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_metapop_data.py
--rw-r--r--   0 picault    (501) staff       (20)    12790 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12266 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_JA_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11079 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_age_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10550 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_aggreg.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9658 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_cumul_inc.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10235 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_SIR_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8445 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_duration.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11556 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/IBM_gest.yaml
--rw-r--r--   0 picault    (501) staff       (20)     7990 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_ABC.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9560 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SEIRS.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9098 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9966 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIRS_periodic_risk.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9917 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11501 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_demo_prototypes.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10720 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_demo_random.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12252 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)     7323 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_metapop_data.py
--rw-r--r--   0 picault    (501) staff       (20)    12807 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11735 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_JA_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9376 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_cumul_inc.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9584 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10555 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_SIR_lockdown.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8407 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/compart_duration.yaml
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.066697 emulsion-1.2rc5/models/features/data/
--rw-r--r--   0 picault    (501) staff       (20)      183 2023-06-07 09:29:01.000000 emulsion-1.2rc5/models/features/data/initial_individuals.csv
--rw-r--r--   0 picault    (501) staff       (20)     1711 2023-06-07 09:29:01.000000 emulsion-1.2rc5/models/features/data/moves.csv
--rw-r--r--   0 picault    (501) staff       (20)    13373 2023-06-07 09:29:01.000000 emulsion-1.2rc5/models/features/data/pop_parameters.csv
--rw-r--r--   0 picault    (501) staff       (20)      209 2023-06-07 09:29:01.000000 emulsion-1.2rc5/models/features/data/pop_structure.csv
--rw-r--r--   0 picault    (501) staff       (20)      207 2023-06-07 09:29:01.000000 emulsion-1.2rc5/models/features/data/population_size.csv
--rw-r--r--   0 picault    (501) staff       (20)       98 2023-06-07 09:29:01.000000 emulsion-1.2rc5/models/features/data/test_pop.csv
--rw-r--r--   0 picault    (501) staff       (20)     9788 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_ABC-old.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8842 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_ABC.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9305 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_ABC2.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10201 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SEIRS.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9771 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10090 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIRS_periodic_risk.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10713 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11574 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_demo_prototypes.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11234 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_demo_random.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12810 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_metapop.yaml
--rw-r--r--   0 picault    (501) staff       (20)     7529 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_metapop_data.py
--rw-r--r--   0 picault    (501) staff       (20)    13458 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_metapop_data.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12477 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_JA_struct.yaml
--rw-r--r--   0 picault    (501) staff       (20)    11487 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_age_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10972 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_aggreg.yaml
--rw-r--r--   0 picault    (501) staff       (20)     9933 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_cumul_inc.yaml
--rw-r--r--   0 picault    (501) staff       (20)    10552 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_demo.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12720 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_SIR_metapop_params.yaml
--rw-r--r--   0 picault    (501) staff       (20)     8890 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_duration.yaml
--rw-r--r--   0 picault    (501) staff       (20)    12031 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/features/hybrid_gest.yaml
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.066820 emulsion-1.2rc5/models/quickstart/
--rw-r--r--   0 picault    (501) staff       (20)    13418 2023-06-07 09:29:02.000000 emulsion-1.2rc5/models/quickstart/quickstart.yaml
--rw-r--r--   0 picault    (501) staff       (20)       38 2023-06-07 09:29:15.073458 emulsion-1.2rc5/setup.cfg
--rw-r--r--   0 picault    (501) staff       (20)    12218 2023-06-07 09:29:02.000000 emulsion-1.2rc5/setup.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.050673 emulsion-1.2rc5/src/
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.067191 emulsion-1.2rc5/src/emulsion/
--rw-r--r--   0 picault    (501) staff       (20)     1767 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/__init__.py
--rw-r--r--   0 picault    (501) staff       (20)    22619 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/__main__.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.068989 emulsion-1.2rc5/src/emulsion/agent/
--rw-r--r--   0 picault    (501) staff       (20)     1957 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/__init__.py
--rw-r--r--   0 picault    (501) staff       (20)    26712 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/action.py
--rw-r--r--   0 picault    (501) staff       (20)     7718 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/atoms.py
--rw-r--r--   0 picault    (501) staff       (20)    13543 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/comparts.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.069515 emulsion-1.2rc5/src/emulsion/agent/core/
--rw-r--r--   0 picault    (501) staff       (20)     2054 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/core/__init__.py
--rw-r--r--   0 picault    (501) staff       (20)    20265 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/core/abstract_agent.py
--rw-r--r--   0 picault    (501) staff       (20)    27803 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/core/emulsion_agent.py
--rw-r--r--   0 picault    (501) staff       (20)     7874 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/core/groups.py
--rw-r--r--   0 picault    (501) staff       (20)     3304 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/exceptions.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.070549 emulsion-1.2rc5/src/emulsion/agent/managers/
--rw-r--r--   0 picault    (501) staff       (20)     2436 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/__init__.py
--rw-r--r--   0 picault    (501) staff       (20)    19693 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/abstract_process_manager.py
--rw-r--r--   0 picault    (501) staff       (20)    24867 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/compart_process_manager.py
--rw-r--r--   0 picault    (501) staff       (20)     7225 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/functions.py
--rw-r--r--   0 picault    (501) staff       (20)    14519 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/group_manager.py
--rw-r--r--   0 picault    (501) staff       (20)    14440 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/ibm_process_manager.py
--rw-r--r--   0 picault    (501) staff       (20)     5587 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/metapop_process_manager.py
--rw-r--r--   0 picault    (501) staff       (20)    25768 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/managers/multi_process_manager.py
--rw-r--r--   0 picault    (501) staff       (20)     3511 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/meta.py
--rw-r--r--   0 picault    (501) staff       (20)     8826 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/process.py
--rw-r--r--   0 picault    (501) staff       (20)    19927 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/agent/views.py
--rwxr-xr-x   0 picault    (501) staff       (20)     2896 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/init_emulsion.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.071227 emulsion-1.2rc5/src/emulsion/model/
--rw-r--r--   0 picault    (501) staff       (20)     1781 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/model/__init__.py
--rw-r--r--   0 picault    (501) staff       (20)    66638 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/model/emulsion_model.py
--rw-r--r--   0 picault    (501) staff       (20)     2314 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/model/exceptions.py
--rw-r--r--   0 picault    (501) staff       (20)    12265 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/model/functions.py
--rw-r--r--   0 picault    (501) staff       (20)    31696 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/model/state_machines.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.071356 emulsion-1.2rc5/src/emulsion/resources/
--rw-r--r--   0 picault    (501) staff       (20)    23385 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/resources/emulsion.tx
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.073136 emulsion-1.2rc5/src/emulsion/tools/
--rw-r--r--   0 picault    (501) staff       (20)     1923 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/__init__.py
--rw-r--r--   0 picault    (501) staff       (20)     9588 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/calendar.py
--rw-r--r--   0 picault    (501) staff       (20)     1313 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/debug.py
--rw-r--r--   0 picault    (501) staff       (20)    17222 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/functions.py
--rw-r--r--   0 picault    (501) staff       (20)    27664 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/getters.py
--rw-r--r--   0 picault    (501) staff       (20)     4843 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/graph.py
--rw-r--r--   0 picault    (501) staff       (20)    22906 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/misc.py
--rw-r--r--   0 picault    (501) staff       (20)     3519 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/parallel.py
--rw-r--r--   0 picault    (501) staff       (20)    12876 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/plot.py
--rw-r--r--   0 picault    (501) staff       (20)     3762 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/preprocessor.py
--rw-r--r--   0 picault    (501) staff       (20)    20654 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/simulation.py
--rw-r--r--   0 picault    (501) staff       (20)     5677 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/state.py
--rw-r--r--   0 picault    (501) staff       (20)     2777 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/timing.py
--rw-r--r--   0 picault    (501) staff       (20)     4884 2023-06-07 09:29:02.000000 emulsion-1.2rc5/src/emulsion/tools/view.py
-drwxr-xr-x   0 picault    (501) staff       (20)        0 2023-06-07 09:29:15.067954 emulsion-1.2rc5/src/emulsion.egg-info/
--rw-r--r--   0 picault    (501) staff       (20)     2818 2023-06-07 09:29:15.000000 emulsion-1.2rc5/src/emulsion.egg-info/PKG-INFO
--rw-r--r--   0 picault    (501) staff       (20)     8341 2023-06-07 09:29:15.000000 emulsion-1.2rc5/src/emulsion.egg-info/SOURCES.txt
--rw-r--r--   0 picault    (501) staff       (20)        1 2023-06-07 09:29:15.000000 emulsion-1.2rc5/src/emulsion.egg-info/dependency_links.txt
--rw-r--r--   0 picault    (501) staff       (20)       52 2023-06-07 09:29:15.000000 emulsion-1.2rc5/src/emulsion.egg-info/entry_points.txt
--rw-r--r--   0 picault    (501) staff       (20)      387 2023-06-07 09:29:15.000000 emulsion-1.2rc5/src/emulsion.egg-info/requires.txt
--rw-r--r--   0 picault    (501) staff       (20)        9 2023-06-07 09:29:15.000000 emulsion-1.2rc5/src/emulsion.egg-info/top_level.txt
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.859658 emulsion-1.3b1/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10174 2022-12-15 12:42:48.000000 emulsion-1.3b1/LICENSE
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)      301 2022-12-15 12:42:46.000000 emulsion-1.3b1/MANIFEST.in
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1161 2022-12-15 12:42:48.000000 emulsion-1.3b1/NOTICE
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     2934 2022-12-15 12:43:18.855658 emulsion-1.3b1/PKG-INFO
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     4548 2022-12-15 12:42:48.000000 emulsion-1.3b1/README.md
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/doc/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/doc/html/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/doc/html/_static/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.827658 emulsion-1.3b1/doc/html/_static/benchmark/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     1964 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model1-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     7166 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model1.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     3042 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model2-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8348 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model2.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     3247 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model2b-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8552 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model2b.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     4212 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model3-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9926 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model3.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     5205 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model3b-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10917 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model3b.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     6859 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model4-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12564 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model4.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8486 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model5-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    14248 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model5.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9929 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model6-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    15822 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model6.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10581 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model7-short.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    16478 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/benchmark/model7.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/doc/html/_static/models/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.835658 emulsion-1.3b1/doc/html/_static/models/features/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9784 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SEIRS.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9452 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9620 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIRS_periodic_risk.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10395 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11486 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_demo_prototypes.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11003 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_demo_random.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12816 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_metapop.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12790 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_metapop_data.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12266 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_struct.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11079 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_age_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10550 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_aggreg.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9658 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_cumul_inc.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10235 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8445 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_duration.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11556 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/IBM_gest.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9560 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SEIRS.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9544 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SEIRS_tmp.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9098 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9966 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIRS_periodic_risk.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9917 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10720 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_demo_random.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12252 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_metapop.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12807 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_metapop_data.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11735 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_struct.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9376 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_cumul_inc.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9584 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8407 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/compart_duration.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10201 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SEIRS.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9771 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10090 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIRS_periodic_risk.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10713 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11574 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_demo_prototypes.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11234 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_demo_random.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    13656 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_metapop.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    13458 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_metapop_data.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12477 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_struct.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11487 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_age_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10972 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_aggreg.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9933 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_cumul_inc.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10552 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12735 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_metapop_params.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8890 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_duration.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12031 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/features/hybrid_gest.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.835658 emulsion-1.3b1/doc/html/_static/models/quickstart/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    13404 2022-12-15 12:43:18.000000 emulsion-1.3b1/doc/html/_static/models/quickstart/quickstart.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/models/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.843658 emulsion-1.3b1/models/features/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9784 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SEIRS.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9452 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9620 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIRS_periodic_risk.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10395 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11486 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_demo_prototypes.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11003 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_demo_random.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12816 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_metapop.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     7512 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_metapop_data.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12790 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_metapop_data.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12266 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_JA_struct.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11079 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_age_demo.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10550 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_aggreg.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9658 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_cumul_inc.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10235 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_SIR_demo.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     8445 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_duration.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11556 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/IBM_gest.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9560 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SEIRS.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9544 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SEIRS_tmp.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9098 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9966 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIRS_periodic_risk.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9917 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_JA_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10720 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_JA_demo_random.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    12252 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_JA_metapop.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     7323 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_JA_metapop_data.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12807 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_JA_metapop_data.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    11735 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_JA_struct.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9376 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_cumul_inc.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9584 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_SIR_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     8407 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/compart_duration.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.843658 emulsion-1.3b1/models/features/data/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)      183 2022-12-15 12:42:46.000000 emulsion-1.3b1/models/features/data/initial_individuals.csv
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1711 2022-12-15 12:42:46.000000 emulsion-1.3b1/models/features/data/moves.csv
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    13373 2022-12-15 12:42:46.000000 emulsion-1.3b1/models/features/data/pop_parameters.csv
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      209 2022-12-15 12:42:46.000000 emulsion-1.3b1/models/features/data/pop_structure.csv
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)      207 2022-12-15 12:42:46.000000 emulsion-1.3b1/models/features/data/population_size.csv
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)       98 2022-12-15 12:42:46.000000 emulsion-1.3b1/models/features/data/test_pop.csv
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10201 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SEIRS.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9771 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10090 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIRS_periodic_risk.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10713 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_demo.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11574 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_demo_prototypes.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11234 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_demo_random.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    13656 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_metapop.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     7529 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_metapop_data.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    13458 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_metapop_data.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    12477 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_JA_struct.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11487 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_age_demo.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10972 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_aggreg.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9933 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_cumul_inc.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10552 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_demo.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    12735 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_SIR_metapop_params.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     8890 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_duration.yaml
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    12031 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/features/hybrid_gest.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.843658 emulsion-1.3b1/models/quickstart/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    13404 2022-12-15 12:42:48.000000 emulsion-1.3b1/models/quickstart/quickstart.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)       38 2022-12-15 12:43:18.859658 emulsion-1.3b1/setup.cfg
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    12009 2022-12-15 12:42:48.000000 emulsion-1.3b1/setup.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/src/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.843658 emulsion-1.3b1/src/emulsion/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1785 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    30511 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/__main__.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.847658 emulsion-1.3b1/src/emulsion/agent/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1957 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    27357 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/action.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    12691 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/atoms.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    13380 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/comparts.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.847658 emulsion-1.3b1/src/emulsion/agent/core/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     2054 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/core/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    23464 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/core/abstract_agent.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    29036 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/core/emulsion_agent.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     7914 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/core/groups.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     3303 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/exceptions.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.847658 emulsion-1.3b1/src/emulsion/agent/managers/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     2436 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    23865 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/abstract_process_manager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    24984 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/compart_process_manager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     7225 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/functions.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    17241 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/group_manager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    13422 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/ibm_process_manager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     5658 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/metapop_process_manager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    28317 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/managers/multi_process_manager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     3511 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/meta.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     8818 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/process.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    22569 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/agent/views.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     2885 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/init_emulsion.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.847658 emulsion-1.3b1/src/emulsion/model/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1781 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/model/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    65802 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/model/emulsion_model.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     2314 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/model/exceptions.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    14396 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/model/functions.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    35473 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/model/state_machines.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.851658 emulsion-1.3b1/src/emulsion/organization/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     7914 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/AbstractParse.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10448 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/AtomicSpace.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     3229 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/Constante.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)    10004 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationAction.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    41950 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationConstraint.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     3587 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationException.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10635 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationGraph.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    29464 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationManager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    52295 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationModel.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      756 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationPosition.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    11071 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationProcess.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     6823 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/OrganizationPropagate.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    16864 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/Passport.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     2666 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/__init__.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.851658 emulsion-1.3b1/src/emulsion/organization/managers/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     2890 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/managers/OrganizationProcessManager.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1856 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/managers/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     5669 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/organization_function.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.851658 emulsion-1.3b1/src/emulsion/organization/utils/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1749 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/utils/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9388 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/organization/utils/organization_plot.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.851658 emulsion-1.3b1/src/emulsion/resources/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    23385 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/resources/emulsion.tx
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.851658 emulsion-1.3b1/src/emulsion/scripts/
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     4964 2022-12-15 12:42:47.000000 emulsion-1.3b1/src/emulsion/scripts/emulsion-completion.sh
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.823658 emulsion-1.3b1/src/emulsion/templates/
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.851658 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      547 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/groups.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      181 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/head.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      229 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/initials.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      413 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/levels.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     1660 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/organizations.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      249 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/outputs.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      127 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/parameters.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      465 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/prototypes.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      585 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/state_machines.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)       63 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/EMUL_templates/statevars.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.855658 emulsion-1.3b1/src/emulsion/templates/YAML_templates/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      547 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/groups.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      181 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/head.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      229 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/initials.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      413 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/levels.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     1660 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/organizations.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      249 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/outputs.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      127 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/parameters.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      465 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/prototypes.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      585 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/state_machines.yaml
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)       63 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/YAML_templates/statevars.yaml
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.855658 emulsion-1.3b1/src/emulsion/templates/main_template/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      186 2022-12-15 12:42:46.000000 emulsion-1.3b1/src/emulsion/templates/main_template/main.emul
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.855658 emulsion-1.3b1/src/emulsion/tools/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      261 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/DebugGlobal.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     1923 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/__init__.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     9588 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/calendar.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     1446 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/debug.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    15503 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/functions.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    25977 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/getters.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     4843 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/graph.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    26218 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/misc.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     3519 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/parallel.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     2143 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/persist.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    10461 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/plot.py
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     3762 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/preprocessor.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)    23023 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/simulation.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     5668 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/state.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     2777 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/timing.py
+-rwxrwxr-x   0 vsicard   (1000) vsicard   (1000)     4884 2022-12-15 12:42:48.000000 emulsion-1.3b1/src/emulsion/tools/view.py
+drwxrwxr-x   0 vsicard   (1000) vsicard   (1000)        0 2022-12-15 12:43:18.843658 emulsion-1.3b1/src/emulsion.egg-info/
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     2934 2022-12-15 12:43:18.000000 emulsion-1.3b1/src/emulsion.egg-info/PKG-INFO
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)     9260 2022-12-15 12:43:18.000000 emulsion-1.3b1/src/emulsion.egg-info/SOURCES.txt
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)        1 2022-12-15 12:43:18.000000 emulsion-1.3b1/src/emulsion.egg-info/dependency_links.txt
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)       97 2022-12-15 12:43:18.000000 emulsion-1.3b1/src/emulsion.egg-info/entry_points.txt
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)      377 2022-12-15 12:43:18.000000 emulsion-1.3b1/src/emulsion.egg-info/requires.txt
+-rw-rw-r--   0 vsicard   (1000) vsicard   (1000)        9 2022-12-15 12:43:18.000000 emulsion-1.3b1/src/emulsion.egg-info/top_level.txt
```

### Comparing `emulsion-1.2rc5/LICENSE` & `emulsion-1.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/NOTICE` & `emulsion-1.3b1/NOTICE`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/PKG-INFO` & `emulsion-1.3b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: emulsion
-Version: 1.2rc5
+Version: 1.3b1
 Summary: Epidemiological Multi-Level Simulation framework
 Home-page: https://sourcesup.renater.fr/emulsion-public/
-Download-URL: https://pypi.org/project/emulsion/
-Author: Sébastien Picault, Yu-Lin Huang, Vianney Sicard and Pauline Ezanno
+Author: Sebastien Picault, Yu-Lin Huang, Vianney Sicard and Pauline Ezanno
 Author-email: sebastien.picault@inrae.fr
 Maintainer: Sébastien Picault
 Maintainer-email: sebastien.picault@inrae.fr
 License: Apache-2.0
+Download-URL: https://pypi.org/project/emulsion/
 Project-URL: Documentation, https://sourcesup.renater.fr/emulsion-public/
-Project-URL: Source Code, https://forgemia.inra.fr/dynamo/software/emulsion-public
+Project-URL: Source Code, https://git.renater.fr/emulsion-public.git
+Description: 
+        Framework EMULSION is intended for modellers in epidemiology, to help
+        them design, simulate, and revise complex mechanistic stochastic
+        models, without having to write or rewrite huge amounts of code.
+        
+        It comes with a *Domain-Specific Language* to represent all components
+        of epidemiological models (assumptions, model structure,
+        parameters...) in an explicit, intelligible and revisable way, and
+        thus facilitate interactions with other scientists (biologists,
+        veterinarians, economists...) throughout the modelling
+        process. EMULSION models are automatically processed by a modular
+        simulation engine, which, if needed, can also incorporate small code
+        add-ons for representing very specific features of a model.
+        
+        Models can use classical modelling paradigms (compartments,
+        individual-based models, metapopulations) and multiple scales (from
+        individuals to metapopulations), thanks to recent research in
+        Artificial Intelligence.
+        
 Keywords: epidemiological modelling,computational epidemiology,multilevel modelling,compartment-based models,individual-based models,metapopulations,agent-based simulation,animal health,artificial intelligence,stochastic models,mechanistic models
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Unix Shell
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Provides-Extra: doc
 Provides-Extra: dev
-License-File: LICENSE
-License-File: NOTICE
-
-
-Framework EMULSION is intended for modellers in epidemiology, to help
-them design, simulate, and revise complex mechanistic stochastic
-models, without having to write or rewrite huge amounts of code.
-
-It comes with a *Domain-Specific Language* to represent all components
-of epidemiological models (assumptions, model structure,
-parameters...) in an explicit, intelligible and revisable way, and
-thus facilitate interactions with other scientists (biologists,
-veterinarians, economists...) throughout the modelling
-process. EMULSION models are automatically processed by a modular
-simulation engine, which, if needed, can also incorporate small code
-add-ons for representing very specific features of a model.
-
-Models can use classical modelling paradigms (compartments,
-individual-based models, metapopulations) and multiple scales (from
-individuals to metapopulations), thanks to recent research in
-Artificial Intelligence.
```

### Comparing `emulsion-1.2rc5/README.md` & `emulsion-1.3b1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 EMULSION: Epidemiological Multi-Level Simulation framework
 ======================
 
-![Version](https://img.shields.io/badge/version-1.2rc5-f16152.svg)
+![Version](https://img.shields.io/badge/version-1.3beta1-f16152.svg)
 ![License](https://img.shields.io/badge/license-Apache--2.0-8cd0c3.svg)
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
 - [EMULSION - Quick Start](#emulsion---quick-start)
     - [Part A - General information](#part-a---general-information)
@@ -32,25 +32,24 @@
 specific features of a model.
 
 Models can use classical modelling paradigms (compartments,
 individual-based models, metapopulations) and multiple scales (from
 individuals to metapopulations), thanks to recent research in
 Artificial Intelligence.
 
-### Version 1.2rc5
-### License: Apache-2.0
-### Contributors and contact:
-- Sébastien Picault (`sebastien.picault@inrae.fr`)
-- Yu-Lin Huang
-- Vianney Sicard
-- Sandie Arnoux
-- Gaël Beaunée
-- Pauline Ezanno (`pauline.ezanno@inrae.fr`)
-
-### How to cite:
+- **Version 1.3beta1**
+- **License:** Apache-2.0
+- **Contributors and contact:**
+  - Sébastien Picault (`sebastien.picault@inrae.fr`)
+  - Yu-Lin Huang
+  - Vianney Sicard
+  - Sandie Arnoux
+  - Gaël Beaunée
+  - Pauline Ezanno (`pauline.ezanno@inrae.fr`)
+- **How to cite:**
   S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée, P. Ezanno
   (2019). "EMULSION: Transparent and flexible multiscale stochastic
   models in human, animal and plant epidemiology", _PLoS Computational
   Biology_ **15(9):** e1007342. `DOI: 10.1371/journal.pcbi.1007342`
 
   BibTeX:
 
@@ -66,32 +65,23 @@
           volume =	 {15},
           number =	 {9},
           pages =	 {e1007342},
           DOI =		 {10.1371/journal.pcbi.1007342},
           url =		 {https://doi.org/10.1371/journal.pcbi.1007342}
         }
 
-### Funding
-This research was funded by: 
-- INRAE, the French National Research Institute for Agriculture, Food and Environment:
-  - Animal Health Division
-  - Partnerships and Innovation Transfer Division ("DPTI")
-- the European Union:
-  - the European fund for the regional development (FEDER) of Pays de la Loire
-  - project H2020 DECIDE (101000494)
-- the French Research Agency (ANR):
-  - Program Investments for the Future, project ANR-10-BINF-0007 (MIHMES)
-  - project ANR-16-CE32-0007-01 (CADENCE)
-- the French Région Pays de la Loire: 
-  - PULSAR grant 
-  - CAENOME Ph.D. grant
-- the Carnot Institute "France Futur Élevage" (SEPTIME project)
-- the For and On Regional Development (PSDR) French research programme, funded by
-  INRAE and the French regions of Bretagne, Pays de la Loire, Normandie and Nouvelle
-  Aquitaine (SANT'Innov)
+- **Funding** This research was funded by the French Research Agency
+ (ANR) through projects MIHMES (ANR-10-BINF-07) and CADENCE
+ (ANR-16-CE32-0007-01), the European fund for the Regional Development
+ (FEDER) of Pays-de-la-Loire, and the Animal Health Division of the
+ French National Research Institute for Agriculture, Food and
+ Environment (INRAE). This work was also supported by the SANT'Innov
+ project of the For and On Regional Development (PSDR) French research
+ programme, which is funded by INRAE and the French regions of
+ Bretagne, Pays de la Loire, Normandie and Nouvelle Aquitaine.
 
 
 Part B - Getting Started
 ---------------------
 
 Please refer to [EMULSION on-line documentation](https://sourcesup.renater.fr/www/emulsion-public/).
 
@@ -109,8 +99,8 @@
   | `models/X/outputs/` | Default location for outputs of model X |
   | `models/X/img/`     | Default location for image files generated by model X (plots, diagrams, maps...) |
   | `scripts/`       | Location for (shell/R) utility scripts and syntactic rules    |
   | `src/`       | Location of EMULSION source files  |
 
 
 -----
-_Last update: 2023-05-11, S. Picault (`sebastien.picault@inrae.fr`)_
+_Last update: 2020-10-19, S. Picault (`sebastien.picault@inrae.fr`)_
```

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model1-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model1-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model1.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model1.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model2-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model2-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model2.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model2.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model2b-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model2b-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model2b.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model2b.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model3-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model3-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model3.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model3.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model3b-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model3b-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model3b.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model3b.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model4-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model4-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model4.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model4.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model5-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model5-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model5.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model5.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model6-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model6-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model6.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model6.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model7-short.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model7-short.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/benchmark/model7.yaml` & `emulsion-1.3b1/doc/html/_static/benchmark/model7.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_ABC.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_duration.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -60,23 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: IBM_ABC
+model_name: hybrid_duration
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" model, i.e. with individuals grouped according to
-  relevant variables such as their health state. '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  abstract: 'This model demonstrate how to assign a duration to a state.'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -102,15 +100,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # A hybrid model considers two levels: the population and
 # its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'   # the keyword for designing hybrid models
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -122,15 +120,38 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
   individuals:
-    - health_state
+    - age_group: aging
+
+
+#   _____                       _
+#  / ____|                     (_)
+# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
+# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
+# | |__| | | | (_) | |_| | |_) | | | | | (_| |
+#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
+#                        | |             __/ |
+#                        |_|            |___/
+
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+grouping:
+  population:
+    aging: [age_group]
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -141,73 +162,77 @@
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
-  health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+  age_group:
+    desc: 'The state machine which defines the evolution of age
+    groups.'
     # Below, the list of states with their attributes.
     states:
-      - A:
-          name: 'A'
-          desc: 'A'
-          fillcolor: 'wheat'
-          # duration: 10
-      - B:
-          name: 'B'
-          desc: 'B'
-          fillcolor: 'maroon'
-      - C:
-          name: 'C'
-          desc: 'C'
+      - N:
+          name: 'Newborn'
+          desc: 'very young individuals'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
+          duration: 'juvenile_age'
+          default: yes
+      - J:
+          name: 'Juvenile'
+          desc: 'juvenile individuals'
+          fillcolor: 'orange'
+          duration: 'adult_age - juvenile_age'
+      - A:
+          name: 'Adult'
+          desc: 'adult individuals (producing new juveniles)'
+          fillcolor: 'brown'
     transitions:
-      - {from: A, to: C, proba: 0.8}
-      - {from: A, to: B, proba: 0.2}
+      - {from: N, to: J, proba: 1}
+      - {from: J, to: A, proba: 1}
+      # equivalent to:
+      # - {from: N, to: J, amount-all-but: 0}
+      # - {from: J, to: A, amount-all-but: 0}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-
+  juvenile_age:
+    desc: 'age at which newborns become juveniles (days)'
+    value: 20
+  adult_age:
+    desc: 'age at which individuals become adults (days)'
+    value: 'random_uniform(50, 70)'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
-    - default:
-        desc: 'default individuals'
-        health_state: A
+    - newborn:
+        desc: 'newborn individuals'
+        age_group: N
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -221,15 +246,15 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: default
+    - prototype: newborn
       amount: 'initial_population_size'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SEIRS.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SEIRS.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIRS_periodic_risk.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIRS_periodic_risk.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_demo_prototypes.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_demo_prototypes.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_demo_random.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_demo_random.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_metapop.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_metapop.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: IBM_SIR_JA_metapop
+model_name: hybrid_SIR_JA_metapop
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  individual-based SIR model with demography and age structure, at the
+  compartmental SIR model with demography and age structure, at the
   metapopulation scale.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
@@ -100,15 +100,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # Here we introduced a third level, aggregating populations within
 # a metapopulation
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'
+    aggregation_type: 'compartment'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
   metapop:
     desc: 'level of the metapopulation'
     contains:
@@ -143,17 +143,15 @@
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-
+# not used here
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_metapop_data.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_metapop_data.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_JA_struct.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_struct.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_age_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_age_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_aggreg.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_aggreg.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_cumul_inc.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_cumul_inc.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_SIR_struct.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_struct.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -12,20 +59,20 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: IBM_SIR_struct
+model_name: compart_SIR_JA_struct
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  individual-based SIR model with demography and age structure, with
+  compartmental SIR model with demography and age structure, with
   non-exponential durations in state J. Besides, a contact
   structure is added to account for physical separation between
   Juveniles and Adults.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
@@ -55,15 +102,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # An individual-based model (IBM) (or a hybrid model) considers both
 # the individual and the population levels:
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'
+    aggregation_type: 'compartment'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 #  _____
@@ -88,27 +135,15 @@
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-# Groupings are required for defining processes in compartement-based
-# or hybrid models.
-grouping:
-  population:
-    details: [health_state, age_group]
-
+# not used here
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_duration.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_duration.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/IBM_gest.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_gest.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_ABC.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_duration.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -60,23 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_ABC
+model_name: compart_duration
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" model, i.e. with individuals grouped according to
-  relevant variables such as their health state. '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  abstract: 'This model demonstrate how to assign a duration to a state.'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -102,15 +100,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # A hybrid model considers two levels: the population and
 # its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'   # the keyword for designing hybrid models
+    aggregation_type: 'compartment'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -122,15 +120,28 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
   individuals:
-    - health_state
+    - age_group
+
+
+#   _____                       _
+#  / ____|                     (_)
+# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
+# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
+# | |__| | | | (_) | |_| | |_) | | | | | (_| |
+#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
+#                        | |             __/ |
+#                        |_|            |___/
+
+# not used here
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -141,73 +152,76 @@
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
-  health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+  age_group:
+    desc: 'The state machine which defines the evolution of age groups.'
     # Below, the list of states with their attributes.
     states:
-      - A:
-          name: 'A'
-          desc: 'A'
-          fillcolor: 'wheat'
-          # duration: 10
-      - B:
-          name: 'B'
-          desc: 'B'
-          fillcolor: 'maroon'
-      - C:
-          name: 'C'
-          desc: 'C'
+      - N:
+          name: 'Newborn'
+          desc: 'very young individuals'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
+          duration: 'juvenile_age'
+          default: yes
+      - J:
+          name: 'Juvenile'
+          desc: 'juvenile individuals'
+          fillcolor: 'orange'
+          duration: 'adult_age - juvenile_age'
+      - A:
+          name: 'Adult'
+          desc: 'adult individuals (producing new juveniles)'
+          fillcolor: 'brown'
     transitions:
-      - {from: A, to: C, proba: 0.8}
-      - {from: A, to: B, proba: 0.2}
+      - {from: N, to: J, proba: 1}
+      - {from: J, to: A, proba: 1}
+      # equivalent to:
+      # - {from: N, to: J, amount-all-but: 0}
+      # - {from: J, to: A, amount-all-but: 0}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-
+  juvenile_age:
+    desc: 'age at which newborns become juveniles (days)'
+    value: 20
+  adult_age:
+    desc: 'age at which individuals become adults (days)'
+    value: 'random_uniform(50, 70)'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
-    - default:
-        desc: 'default individuals'
-        health_state: A
+    - newborn:
+        desc: 'newborn individuals'
+        age_group: N
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -221,15 +235,15 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: default
+    - prototype: newborn
       amount: 'initial_population_size'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SEIRS.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SEIRS.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIRS_periodic_risk.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIRS_periodic_risk.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_demo_prototypes.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_JA_demo_prototypes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR_JA_demo_prototypes
+model_name: IBM_SIR_JA_demo_prototypes
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with explicit age groups and demography.
+  individual-based SIR model with explicit age groups and demography.
   Data-based prototype collections are used to initialize
   individuals and populations.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
@@ -108,15 +108,15 @@
   metapop:
     desc: 'level of the metapopulation'
     contains:
       - population
     aggregation_type: 'metapopulation'
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'IBM'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -149,17 +149,17 @@
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
-# grouping:
-#   population:
-#     aging: [age_group, health_state]
+grouping:
+  population:
+    aging: [health_state, age_group]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_demo_random.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_demo_random.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_metapop.yaml` & `emulsion-1.3b1/models/features/compart_SIR_JA_metapop.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_metapop_data.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_JA_metapop_data.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_JA_struct.yaml` & `emulsion-1.3b1/models/features/compart_SIR_JA_struct.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_cumul_inc.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_cumul_inc.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SIR_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_lockdown.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SEIRS.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -60,24 +60,22 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR
+model_name: hybrid_SEIRS
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" SIR model, i.e. with individuals grouped according to
-  relevant variables such as their health state. A lockdown occurs
-  during epidemics to flatten the curve.
-  '
+  "hybrid" SEIRS model, i.e. with individuals grouped according to
+  relevant variables such as their health state.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -88,15 +86,15 @@
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
   time_unit: 'days'
   delta_t: 1
   origin: 'January 1'
-  total_duration: '300'
+  total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
@@ -104,15 +102,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # A hybrid model considers two levels: the population and
 # its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'   # the keyword for designing hybrid models
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -124,15 +122,15 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
   individuals:
-    - health_state
+    - health_state: infection
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -144,17 +142,17 @@
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
-#grouping:
-#  population:
-#    infection: [health_state]
+grouping:
+  population:
+    infection: [health_state]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -176,76 +174,74 @@
     '
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
+      - E:
+          name: 'Latent'
+          desc: 'infected but not yet able to transmit the disease'
+          fillcolor: 'orange'
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     # Below, a list of transitions between states, with rate or
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
-      - {from: S, to: I, rate: 'force_of_infection'}
+      - {from: S, to: E, rate: 'force_of_infection'}
+      - {from: E, to: I, rate: '1/incubation'}
       - {from: I, to: R, rate: 'recovery'}
+      - {from: R, to: S, rate: 'waning'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
-    value: 1000
+    value: 100
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
-    value: 10
-  is_lockdown_active:
-    desc: '1 if currently under lockdown, 0 otherwise'
-    value: 'AND(time >= lockdown_start, time <= lockdown_start + lockdown_duration)'
+    value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
-    value: 'IfThenElse(is_lockdown_active, transmission_I_lockdown, transmission_I_default)'
-    # value: 'IfThenElse(AND(total_I > 0.2 * total_population), transmission_I_lockdown, transmission_I_default)'
-  transmission_I_default:
-    desc: 'default transmission rate from infectious individuals (/day)'
-    value: 0.2
-  transmission_I_lockdown:
-    desc: 'transmission rate from infectious individuals during lockdown (/day)'
-    value: 0.02
-  lockdown_start:
-    desc: 'date where lockdown starts after the beginning of the simulation (days)'
-    value: 30
-  lockdown_duration:
-    desc: 'duration of the lockdown (days)'
-    value: 60
+    value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
-    value: '1/15'
+    value: 0.1
+  incubation:
+    desc: 'mean duration of latent state (days, assuming exponential
+    distribution of durations in the state)
+    '
+    value: 5
+  waning:
+    desc: 'rate at which individuals lose immunity (/day)'
+    value: 0.05
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
-    value: '100 * total_I / total_population'
+    value: '100 * (total_I + total_E) / total_population'
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
@@ -305,9 +301,10 @@
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
-      - is_lockdown_active
+      - percentage_prevalence
+      - total_population
 ...
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_metapop.yaml` & `emulsion-1.3b1/models/features/compart_SIR_JA_demo.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -11,109 +58,88 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
+
 # NAME OF THE MODEL
-model_name: compart_SIR_metapop
+model_name: compart_SIR_JA_demo
+
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  compartment-based SIR model with demography and age structure, at
-  the metapopulation scale.
-  '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SIR model with explict age groups and demography.'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: days
+  time_unit: 'days'
   delta_t: 1
-  origin: 'January 1, 2018'
+  origin: 'January 1'
   total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# Here we introduced a third level, aggregating populations within
-# a metapopulation
 levels:
+  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: compartment
-  metapop:
-    desc: 'level of the metapopulation'
+    aggregation_type: 'compartment'
     contains:
-      - population
-    aggregation_type: metapopulation
-
-
-#   _____                       _
-#  / ____|                     (_)
-# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
-# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
-# | |__| | | | (_) | |_| | |_) | | | | | (_| |
-#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
-#                        | |             __/ |
-#                        |_|            |___/
-
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-# Groupings are requimaroon for defining processes in compartement-based
-# or hybrid models.
-grouping:
-  population:
-    infection:
-      machine_name: health_state
-      key_variables: [health_state]
-    aging:
-      machine_name: age_group
-      key_variables: [age_group]
+      - individuals
+  # In a compartment-based model, the individuals level is not simulated explicitly
+  individuals:
+    desc: 'level of individuals'
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model (or in a Hybrid model), processes take
-# place at the population level and are managed by groupings
 processes:
-  population:
-    - infection
-    - aging
+  individuals:
+    - health_state
+    - age_group
 
 
+#   _____                       _
+#  / ____|                     (_)
+# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
+# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
+# | |__| | | | (_) | |_| | |_) | | | | | (_| |
+#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
+#                        | |             __/ |
+#                        |_|            |___/
+
+# not used here
+
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
 
@@ -121,68 +147,58 @@
 # Each state machine is composed at least of several states.
 # The name of a state machine defines an individual variable which
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
-  # Below, the definition of the state machine used by the process
-  # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
-    # Below, the list of states with their attributes.
+    desc: 'The state machine which defines the evolution of health states'
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
           default: yes
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
+
   age_group:
-    desc: 'The state machine which defines the evolution of age groups
-    '
+    desc: 'The state machine which defines the evolution of age groups.'
     states:
       - J:
           name: 'Juvenile'
-          desc: 'Young individuals'
+          desc: 'juvenile individuals'
           fillcolor: 'orange'
-          default: yes
       - A:
           name: 'Adult'
-          desc: 'Adult individuals'
+          desc: 'adult individuals (producing new juveniles)'
           fillcolor: 'brown'
       - D:
           name: 'Dead'
-          desc: 'compartment to represent deceased individuals'
-          fillcolor: 'white'
+          desc: 'compartment to put dead individuals'
+          fillcolor: white
           autoremove: yes
     transitions:
       - {from: J, to: A, rate: 'maturation'}
-      - {from: A, to: D, rate: 'mortality'}
-      - {from: J, to: D, rate: 'mortality'}
+      # death (assuming no disease-induced mortality)
+      - {from: J, to: D, rate: 'death'}
+      - {from: A, to: D, rate: 'death'}
     productions:
-      - {from: A, to: J, rate: 'birth'}
-
+      # births (assuming no vertical transmission)
+      - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
@@ -190,77 +206,63 @@
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
-    value: 'initial_population_size * initial_prevalence'
+    value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
+  birth:
+    desc: 'the birth rate (/day)'
+    value: 0.01
+  death:
+    desc: 'the death rate (/day)'
+    value: 'birth'
   maturation:
     desc: 'rate at which juveniles become adults (/day)'
     value: '1/20'
-  b:
-    desc: 'base mortality rate (/day)'
-    value: 0.05
-  mortality:
-    desc: 'density-dependent mortality rate'
-    value: 'b * total_population / carrying_capacity'
-  birth:
-    desc: 'birth rate (/day)'
-    value: 'b * 2'
-  carrying_capacity:
-    desc: 'carrying capacity of the environment'
-    value: 150
-  nb_populations:
-    desc: 'number of populations in metapopulation'
-    value: 10
-
-#   _____ _        _
-#  / ____| |      | |
-# | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
-#  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
-#  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
-# |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
-
-statevars:
-  initial_prevalence:
-    desc: 'Initial prevalence in the population'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
-  population:
-    - healthy_population:
-        desc: 'population initially without infected individuals'
-        initial_prevalence: 0
-    - infected_population:
-        desc: 'population initially infected individuals'
-        initial_prevalence: 0.1
+  individuals:
+    - healthy:
+        desc: 'healthy individuals'
+        health_state: S
+        age_group: random
+    - infected:
+        desc: 'infected individuals'
+        health_state: I
+        age_group: random
+    - newborn:
+        desc: 'newly created individuals'
+        health_state: default
+        age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -270,31 +272,22 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-
-# In IBM, hybrid models or metapops, initial conditions describe the
-# prototypes involved with the amount of individuals in each of those
-# prototypes
+# In IBM or hybrid models, initial conditions describe the prototypes
+# involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - population:
-        - total: 'initial_population_size'
-        - vars: [S]
-          amount: 'initial_population_size * (1 - initial_prevalence)'
-        - vars: [I]
-          amount: 'initial_population_size * initial_prevalence'
-  metapop:
-    - prototype: infected_population
-      amount: 1
-    - prototype: healthy_population
-      amount: 'nb_populations - 1'
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_SIR_struct.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIRS_periodic_risk.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -11,24 +58,23 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
+
 # NAME OF THE MODEL
-model_name: compart_SIR_struct
+model_name: hybrid_SIRS_periodic_risk
+
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with demography and age structure, with
-  non-exponential durations in state J. Besides, a contact
-  structure is added to account for physical separation between
-  Juveniles and Adults.'
+  hybrid SIRS model exposed to periodic external risk.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -36,67 +82,77 @@
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: days
+  time_unit: 'days'
   delta_t: 1
   origin: 'January 1'
-  total_duration: '200'
+  total_duration: '300'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# An individual-based model (IBM) (or a hybrid model) considers both
-# the individual and the population levels:
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
+
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model (or in a Hybrid model), processes take
-# place at the population level and are managed by groupings
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
   individuals:
-    - health_state
-    - age_group
-
+    - health_state: infection                 # name of a grouping
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+grouping:
+  population:
+    infection: [health_state]
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -115,15 +171,14 @@
     desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
-          default: yes
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
@@ -132,38 +187,15 @@
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
-  age_group:
-    desc: 'The state machine which defines the evolution of age groups'
-    states:
-      - J:
-          name: 'Juvenile'
-          desc: 'Young individuals'
-          fillcolor: 'orange'
-          default: yes
-          duration: '1/maturation'
-      - A:
-          name: 'Adult'
-          desc: 'Adult individuals'
-          fillcolor: 'brown'
-      - D:
-          name: 'Dead'
-          desc: 'compartment to represent deceased individuals'
-          fillcolor: 'white'
-          autoremove: yes
-    transitions:
-      - {from: J, to: A, proba: 1}
-      - {from: A, to: D, rate: 'mortality'}
-      - {from: J, to: D, rate: 'mortality', escape: yes}
-    productions:
-      - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
+      - {from: R, to: S, rate: 'waning'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
@@ -176,62 +208,35 @@
     value: 100
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
     value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
-  transJJ:
-    desc: 'transmission rate within Juveniles age group (/day)'
-    value: 0.2
-  transAA:
-    desc: 'transmission rate within Adults age group (/day)'
-    value: 0.5
-  transJA:
-    desc: 'transmission rate from Juveniles to Adults (/day)'
-    value: 0.3
-  transAJ:
-    desc: 'transmission rate from Adults to Juveniles (/day)'
-    value: 0.05
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
+  waning:
+    desc: 'rate at which individuals lose immunity (/day)'
+    value: 0.01
+  external_risk_period:
+    desc: 'periodicity of the external risk (days)'
+    value: 100
+  external_risk:
+    desc: 'external risk of disease introduction with periodicity'
+    value: 'transmission_I * (1 + sin(time * 2 * pi / external_risk_period))'
+  normalized_external_risk:
+    desc: 'external risk normalized between 0 and 100% of its maximum value'
+    value: '100 * external_risk / (2 * transmission_I)'
   force_of_infection:
     desc: 'infection function'
-    value: 'is_J * force_of_infection_juveniles + is_A * force_of_infection_adults'
-  force_of_infection_juveniles:
-    desc: 'infection function experience by juveniles'
-    value: 'DIV(transJJ * total_I_J, total_J) + DIV(transAJ * total_I_A, total_A)'
-  force_of_infection_adults:
-    desc: 'infection function experience by adults'
-    value: 'DIV(transAA * total_I_A, total_A) + DIV(transJA * total_I_J, total_J)'
+    value: ' (external_risk + transmission_I * total_I) / total_population'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
-  perc_prevalence_A:
-    desc: 'proportion of infected+infectious adults'
-    value: 'DIV(100 * total_I_A, total_A)'
-  perc_prevalence_J:
-    desc: 'proportion of infected+infectious juveniles'
-    value: 'DIV(100 * total_I_J, total_J)'
-  maturation:
-    desc: 'rate at which juveniles become adults (/day)'
-    value: '1/20'
-  b:
-    desc: 'base mortality rate (/day)'
-    value: 0.05
-  mortality:
-    desc: 'density-dependent mortality rate'
-    value: 'b * total_population / carrying_capacity'
-  birth:
-    desc: 'birth rate (/day)'
-    value: 'b * 2'
-  carrying_capacity:
-    desc: 'carrying capacity of the environment'
-    value: 'initial_population_size * 1.5'
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
@@ -242,23 +247,14 @@
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: default
-    - infected:
-        desc: 'infected individuals'
-        health_state: I
-        age_group: default
-    - newborn:
-        desc: 'newborn individuals assuming no vertical transmission'
-        health_state: S
-        age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -273,17 +269,15 @@
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
     - prototype: healthy
-      amount: 'initial_population_size - initial_infected'
-    - prototype: infected
-      amount: 'initial_infected'
+      amount: 'initial_population_size'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -299,10 +293,9 @@
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
       - total_population
-      - perc_prevalence_A
-      - perc_prevalence_J
+      - normalized_external_risk
 ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/compart_duration.yaml` & `emulsion-1.3b1/models/features/compart_duration.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_ABC-old.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_cumul_inc.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -60,24 +60,25 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR
+model_name: hybrid_SIR_cumul_inc
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
   "hybrid" SIR model, i.e. with individuals grouped according to
-  relevant variables such as their health state.
-  '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  relevant variables such as their health state. It records the
+  cumulative incidence (total number of individuals that got
+  infectious over time).'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -122,16 +123,16 @@
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
-  population:
-    - infection                 # name of a grouping
+  individuals:
+    - health_state: infection
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -145,17 +146,15 @@
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
 grouping:
   population:
-    infection:
-      machine_name: health_state
-      key_variables: [health_state]
+    infection: [health_state]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -168,39 +167,39 @@
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+    desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
+          on_enter:
+            - record_change: cumulative_incidence
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     # Below, a list of transitions between states, with rate or
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
-      - {from: S, to: I, proba: 0.9}
-      - {from: S, to: R, proba: 0.1}
+      - {from: S, to: I, rate: 'force_of_infection'}
+      - {from: I, to: R, rate: 'recovery'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
@@ -292,8 +291,9 @@
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
       - total_population
+      - cumulative_incidence
 ...
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_ABC.yaml` & `emulsion-1.3b1/models/features/hybrid_duration.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -60,23 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_ABC
+model_name: hybrid_duration
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" model, i.e. with individuals grouped according to
-  relevant variables such as their health state. '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  abstract: 'This model demonstrate how to assign a duration to a state.'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -122,15 +120,15 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
   individuals:
-    - health_state: infection                 # name of a grouping
+    - age_group: aging
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -144,15 +142,15 @@
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
 grouping:
   population:
-    infection: [health_state]
+    aging: [age_group]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -164,73 +162,77 @@
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
-  health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+  age_group:
+    desc: 'The state machine which defines the evolution of age
+    groups.'
     # Below, the list of states with their attributes.
     states:
-      - A:
-          name: 'A'
-          desc: 'A'
-          fillcolor: 'wheat'
-          # duration: 10
-      - B:
-          name: 'B'
-          desc: 'B'
-          fillcolor: 'maroon'
-      - C:
-          name: 'C'
-          desc: 'C'
+      - N:
+          name: 'Newborn'
+          desc: 'very young individuals'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
+          duration: 'juvenile_age'
+          default: yes
+      - J:
+          name: 'Juvenile'
+          desc: 'juvenile individuals'
+          fillcolor: 'orange'
+          duration: 'adult_age - juvenile_age'
+      - A:
+          name: 'Adult'
+          desc: 'adult individuals (producing new juveniles)'
+          fillcolor: 'brown'
     transitions:
-      - {from: A, to: C, proba: 0.8}
-      - {from: A, to: B, proba: 0.2}
+      - {from: N, to: J, proba: 1}
+      - {from: J, to: A, proba: 1}
+      # equivalent to:
+      # - {from: N, to: J, amount-all-but: 0}
+      # - {from: J, to: A, amount-all-but: 0}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-
+  juvenile_age:
+    desc: 'age at which newborns become juveniles (days)'
+    value: 20
+  adult_age:
+    desc: 'age at which individuals become adults (days)'
+    value: 'random_uniform(50, 70)'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
-    - default:
-        desc: 'default individuals'
-        health_state: A
+    - newborn:
+        desc: 'newborn individuals'
+        age_group: N
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -244,15 +246,15 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: default
+    - prototype: newborn
       amount: 'initial_population_size'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_ABC2.yaml` & `emulsion-1.3b1/models/features/compart_SIR.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -60,23 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_ABC
+model_name: compart_SIR
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" model, i.e. with individuals grouped according to
-  relevant variables such as their health state. '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SIR model.'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -97,65 +95,48 @@
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
-# its components (individuals)
 levels:
+  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
+    aggregation_type: 'compartment'
     contains:
       - individuals
+  # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
-    desc: 'level of the individuals'
-
-
+    desc: 'level of individuals'
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
 processes:
   individuals:
-    - health_state: infection
-    - color: couleur            # name of a grouping
+    - health_state                 # name of a state machine
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-
-grouping:
-  population:
-    infection: [health_state, color]
-    couleur: [color]
-
+# not used here
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -164,90 +145,91 @@
 # Each state machine is composed at least of several states.
 # The name of a state machine defines an individual variable which
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
-  color:
-    desc: ''
-    states:
-      - Blue:
-          name: ''
-          desc: ''
-          fillcolor: 'blue'
-      - Red:
-          name: ''
-          desc: ''
-          fillcolor: 'red'
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+    desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
-      - A:
-          name: 'A'
-          desc: 'A'
+      - S:
+          name: 'Susceptible'
+          desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
-          # duration: 10
-      - B:
-          name: 'B'
-          desc: 'B'
+      - I:
+          name: 'Infectious'
+          desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
-      - C:
-          name: 'C'
-          desc: 'C'
+      - R:
+          name: 'Resistant'
+          desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     # Below, a list of transitions between states, with rate or
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
-      - {from: A, to: C, proba: '0.8'}
-      - {from: A, to: B, proba: '0.2', cond: 'blue'}
+      - {from: S, to: I, rate: 'force_of_infection'}
+      - {from: I, to: R, rate: 'recovery'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-  blue:
-    desc: 'is blue'
-    value: 'is_Blue'
+  initial_infected:
+    desc: 'initial number of infectious individuals in the population'
+    value: 1
+  transmission_I:
+    desc: 'transmission rate from infectious individuals (/day)'
+    value: 0.5
+  recovery:
+    desc: 'recovery rate (/day)'
+    value: 0.1
+  force_of_infection:
+    desc: 'infection function'
+    value: 'transmission_I * total_I / total_population'
+    source: 'classical function assuming frequency dependence'
+  percentage_prevalence:
+    desc: 'proportion of infected+infectious individuals (%)'
+    value: '100 * total_I / total_population'
+
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
-    - default:
-        desc: 'default individuals'
-        health_state: A
-        color: random
-
+    - healthy:
+        desc: 'healthy individuals'
+        health_state: S
+    - infected:
+        desc: 'infected individuals'
+        health_state: I
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
@@ -256,20 +238,22 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
+# Initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: default
-      amount: 'initial_population_size'
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -283,14 +267,10 @@
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
-      - total_B_Blue
-      - total_B_Red
-      - total_A_Blue
-      - total_A_Red
-      - total_C_Blue
-      - total_C_Red
+      - percentage_prevalence
+      - total_population
 ...
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SEIRS.yaml` & `emulsion-1.3b1/models/features/hybrid_SEIRS.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIRS_periodic_risk.yaml` & `emulsion-1.3b1/models/features/hybrid_SIRS_periodic_risk.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_demo_prototypes.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_demo_prototypes.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_demo_random.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_demo_random.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_metapop.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/IBM_SIR_JA_metapop.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR_JA_metapop
+model_name: IBM_SIR_JA_metapop
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  hybrid SIR model with demography and age structure, at the
+  individual-based SIR model with demography and age structure, at the
   metapopulation scale.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
@@ -100,15 +100,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # Here we introduced a third level, aggregating populations within
 # a metapopulation
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: hybrid
+    aggregation_type: 'IBM'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
   metapop:
     desc: 'level of the metapopulation'
     contains:
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_metapop_data.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_metapop_data.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_JA_struct.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_struct.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_age_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_age_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_aggreg.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_aggreg.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_cumul_inc.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_cumul_inc.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_lockdown.yaml` & `emulsion-1.3b1/models/features/IBM_duration.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -13,24 +60,20 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR
+model_name: IBM_duration
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" SIR model, i.e. with individuals grouped according to
-  relevant variables such as their health state. A lockdown occurs
-  during epidemics to flatten the curve.
-  '
+  abstract: 'This model demonstrate how to assign a duration to a state.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -41,31 +84,31 @@
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
   time_unit: 'days'
   delta_t: 1
   origin: 'January 1'
-  total_duration: '300'
+  total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
+# An individual-based model considers two levels: the population and
 # its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
+    aggregation_type: 'IBM'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -73,44 +116,31 @@
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
+# In an Individual-Based Model, processes take place at the individuals
+# level and are thus directly managed by state machines
 processes:
-  population:
-    - infection                 # name of a grouping
+  individuals:
+    - age_group
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-
-grouping:
-  population:
-    infection:
-      machine_name: health_state
-      key_variables: [health_state]
-
+# not used here
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -121,104 +151,78 @@
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
-  health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
+  age_group:
+    desc: 'The state machine which defines the evolution of age
+    groups.
     '
     # Below, the list of states with their attributes.
     states:
-      - S:
-          name: 'Susceptible'
-          desc: 'suceptible of becoming infected'
-          fillcolor: 'wheat'
-      - I:
-          name: 'Infectious'
-          desc: 'infected and able to transmit the disease'
-          fillcolor: 'maroon'
-      - R:
-          name: 'Resistant'
-          desc: 'healthy again and resistant to infection'
+      - N:
+          name: 'Newborn'
+          desc: 'very young individuals'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
+          duration: 'juvenile_age'
+          default: yes
+      - J:
+          name: 'Juvenile'
+          desc: 'juvenile individuals'
+          fillcolor: 'orange'
+          duration: 'adult_age - juvenile_age'
+      - A:
+          name: 'Adult'
+          desc: 'adult individuals (producing new juveniles)'
+          fillcolor: 'brown'
     transitions:
-      - {from: S, to: I, rate: 'force_of_infection'}
-      - {from: I, to: R, rate: 'recovery'}
+      - {from: N, to: J, proba: 1}
+      - {from: J, to: A, proba: 1}
+      # equivalent to:
+      # - {from: N, to: J, amount-all-but: 0}
+      # - {from: J, to: A, amount-all-but: 0}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
-    value: 1000
-  initial_infected:
-    desc: 'initial number of infectious individuals in the population'
-    value: 10
-  transmission_I:
-    desc: 'transmission rate from infectious individuals (/day)'
-    value: 'IfThenElse(AND(time >= lockdown_start, time <= lockdown_start + lockdown_duration), transmission_I_lockdown, transmission_I_default)'
-    # value: 'IfThenElse(AND(total_I > 0.2 * total_population), transmission_I_lockdown, transmission_I_default)'
-  transmission_I_default:
-    desc: 'default transmission rate from infectious individuals (/day)'
-    value: 0.2
-  transmission_I_lockdown:
-    desc: 'transmission rate from infectious individuals during lockdown (/day)'
-    value: 0.02
-  lockdown_start:
-    desc: 'date where lockdown starts after the beginning of the simulation (days)'
-    value: 30
-  lockdown_duration:
-    desc: 'duration of the lockdown (days)'
+    value: 100
+  juvenile_age:
+    desc: 'age at which newborns become juveniles (days)'
     value: 20
-  recovery:
-    desc: 'recovery rate (/day)'
-    value: '1/15'
-  force_of_infection:
-    desc: 'infection function'
-    value: 'transmission_I * total_I / total_population'
-    source: 'classical function assuming frequency dependence'
-  percentage_prevalence:
-    desc: 'proportion of infected+infectious individuals'
-    value: '100 * total_I / total_population'
-
+  adult_age:
+    desc: 'age at which individuals become adults (days)'
+    value: 'random_uniform(50, 70)'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
-    - healthy:
-        desc: 'healthy individuals'
-        health_state: S
-    - infected:
-        desc: 'infected individuals'
-        health_state: I
+    - newborn:
+        desc: 'newborn individuals'
+        age_group: N
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -232,18 +236,16 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: healthy
-      amount: 'initial_population_size - initial_infected'
-    - prototype: infected
-      amount: 'initial_infected'
+    - prototype: newborn
+      amount: 'initial_population_size'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -256,11 +258,8 @@
 # for all state machines each time step during the simulation.
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
-    extra_vars:
-      - percentage_prevalence
-      - total_population
 ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_metapop.yaml` & `emulsion-1.3b1/models/features/compart_SIR_JA_demo_random.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -11,112 +58,93 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
+
 # NAME OF THE MODEL
-model_name: hybrid_SIR_metapop
+model_name: compart_SIR_JA_demo_random
+
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  hybrid SIR model with demography and age structure, at the
-  metapopulation scale.
-  '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  compartmental SIR model with explicit age groups and demography.
+  Initialization uses random multinomial sampling of prototypes
+  (between healthy and infectious) and of states (for age group).'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: days
+  time_unit: 'days'
   delta_t: 1
-  origin: 'January 1, 2018'
+  origin: 'January 1'
   total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# Here we introduced a third level, aggregating populations within
-# a metapopulation
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: hybrid
+    aggregation_type: 'compartment'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
-  metapop:
-    desc: 'level of the metapopulation'
-    contains:
-      - population
-    aggregation_type: metapopulation
-
-
-#   _____                       _
-#  / ____|                     (_)
-# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
-# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
-# | |__| | | | (_) | |_| | |_) | | | | | (_| |
-#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
-#                        | |             __/ |
-#                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-# Groupings are requimaroon for defining processes in compartement-based
-# or hybrid models.
-grouping:
-  population:
-    infection:
-      machine_name: health_state
-      key_variables: [health_state]
-    aging:
-      machine_name: age_group
-      key_variables: [age_group]
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model (or in a Hybrid model), processes take
-# place at the population level and are managed by groupings
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
-  population:
-    - infection
-    - aging
+  individuals:
+    - health_state
+    - age_group
+
 
+#   _____                       _
+#  / ____|                     (_)
+# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
+# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
+# | |__| | | | (_) | |_| | |_) | | | | | (_| |
+#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
+#                        | |             __/ |
+#                        |_|            |___/
+
+# not used here
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -128,17 +156,15 @@
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+    desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
           default: yes
@@ -146,45 +172,41 @@
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
+
   age_group:
-    desc: 'The state machine which defines the evolution of age groups
-    '
+    desc: 'The state machine which defines the evolution of age groups.'
     states:
       - J:
           name: 'Juvenile'
-          desc: 'Young individuals'
+          desc: 'juvenile individuals'
           fillcolor: 'orange'
-          default: yes
       - A:
           name: 'Adult'
-          desc: 'Adult individuals'
+          desc: 'adult individuals (producing new juveniles)'
           fillcolor: 'brown'
       - D:
           name: 'Dead'
-          desc: 'compartment to represent deceased individuals'
-          fillcolor: 'white'
+          desc: 'compartment to put dead individuals'
+          fillcolor: white
           autoremove: yes
     transitions:
       - {from: J, to: A, rate: 'maturation'}
-      - {from: A, to: D, rate: 'mortality'}
-      - {from: J, to: D, rate: 'mortality'}
+      # death (assuming no disease-induced mortality)
+      - {from: J, to: D, rate: 'death'}
+      - {from: A, to: D, rate: 'death'}
     productions:
+      # births (assuming no vertical transmission)
       - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
@@ -192,91 +214,67 @@
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-  initial_infected:
-    desc: 'initial number of infectious individuals in the population'
-    value: 'initial_population_size * initial_prevalence'
+  initial_proba_infection:
+    desc: 'probability that an individual of the population is infectious at t=0'
+    value: 0.1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
+  birth:
+    desc: 'the birth rate (/day)'
+    value: 0.01
+  death:
+    desc: 'the death rate (/day)'
+    value: 'birth'
   maturation:
     desc: 'rate at which juveniles become adults (/day)'
     value: '1/20'
-  b:
-    desc: 'base mortality rate (/day)'
-    value: 0.05
-  mortality:
-    desc: 'density-dependent mortality rate'
-    value: 'b * total_population / carrying_capacity'
-  birth:
-    desc: 'birth rate (/day)'
-    value: 'b * 2'
-  carrying_capacity:
-    desc: 'carrying capacity of the environment'
-    value: 150
-  nb_populations:
-    desc: 'number of populations in metapopulation'
-    value: 10
-
-#   _____ _        _
-#  / ____| |      | |
-# | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
-#  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
-#  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
-# |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
-
-statevars:
-  initial_prevalence:
-    desc: 'Initial prevalence in the population'
+  init_prop_juveniles:
+    desc: 'average proportion of juveniles in the initial population'
+    value: 0.75
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
-  population:
-    - healthy_population:
-        desc: 'population initially without infected individuals'
-        initial_prevalence: 0
-    - infected_population:
-        desc: 'population initially infected individuals'
-        initial_prevalence: 0.1
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: default
+        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
     - infected:
         desc: 'infected individuals'
         health_state: I
-        age_group: default
+        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
     - newborn:
-        desc: 'newborn individuals assuming no vertical transmission'
-        health_state: S
+        desc: 'newly created individuals'
+        health_state: default
         age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
@@ -287,29 +285,26 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-
-# In IBM, hybrid models or metapops, initial conditions describe the
-# prototypes involved with the amount of individuals in each of those
-# prototypes
+# In IBM or hybrid models, initial conditions describe the prototypes
+# involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: healthy
-      amount: 'initial_population_size - initial_infected'
-    - prototype: infected
-      amount: 'initial_infected'
-  metapop:
-    - prototype: infected_population
-      amount: 1
-    - prototype: healthy_population
-      amount: 'nb_populations - 1'
+    - prototype: [infected, healthy]
+      # two possible prototypes for individual initially in the population
+      amount: initial_population_size
+      # drawn among a population of size initial_population_size
+      proba: [initial_proba_infection, 1-initial_proba_infection]
+      # with respective probabilities initial_proba_infection and
+      # 1-initial_proba_infection
+
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_metapop_data.yaml` & `emulsion-1.3b1/models/features/compart_SIR_JA_metapop_data.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -12,23 +59,23 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR_metapop_data
+model_name: compart_SIR_metapop_data
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  hybrid SIR model with demography and age structure, at the
-  metapopulation scale, with data-based trade movements.
-  '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  compartmental SIR model with demography and age structure, at the
+  metapopulation scale, with data-based trade movements responsible
+  for the transmission of infection between populations.'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -54,75 +101,55 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # Here we introduced a third level, aggregating herds within
 # a metapopulation.
 levels:
   herd:
     desc: 'level of the population'
-    aggregation_type: hybrid
+    aggregation_type: 'compartment'
     contains:
       - animals
   animals:
     desc: 'level of the individuals'
   metapop:
     desc: 'level of the metapopulation'
     contains:
       - herd
     aggregation_type: metapopulation
     # The metapopulation is explicitly linked to a specific class in a
     # Python code add-on
-    file: hybrid_SIR_metapop_data.py
+    file: 'compart_SIR_JA_metapop_data.py'
     class_name: Metapopulation
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-
-# # Groupings are required for defining processes in compartement-based
-# # or hybrid models.
-# IBM do not require groupings since processes can be directly
-# associated with state machines.
-grouping:
-  herd:
-    infection:
-      machine_name: health_state
-      key_variables: [health_state]
-    aging:
-      machine_name: age_group
-      key_variables: [age_group]
-
+# not used here
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a Compartment-Based Model (or in a Hybrid model), processes take
 # place at the population level (here, herd) and are managed by groupings
 processes:
-  herd:
-    - infection
-    - aging
+  animals:
+    - health_state
+    - age_group
   metapop:
     # here the process is the name of a procedure defined in the
     # Python code
     - exchange_animals
 
 
 #   _____ _        _         __  __            _     _
@@ -139,17 +166,15 @@
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+    desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
           default: yes
@@ -157,25 +182,19 @@
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
   age_group:
-    desc: 'The state machine which defines the evolution of age groups
-    '
+    desc: 'The state machine which defines the evolution of age groups'
     states:
       - J:
           name: 'Juvenile'
           desc: 'Young animals'
           fillcolor: 'orange'
           default: yes
       - A:
@@ -236,15 +255,15 @@
     desc: 'birth rate (/day)'
     value: 'b * 2'
   carrying_capacity:
     desc: 'carrying capacity of the environment'
     value: 150
   nb_herds:
     desc: 'number of herds in metapopulation'
-    value: 10
+    value: 4
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
@@ -278,17 +297,15 @@
         health_state: I
         age_group: default
     - newborn:
         desc: 'newborn animals assuming no vertical transmission'
         health_state: S
         age_group: J
     - imported_movement:
-        desc: 'animal from outside the metapopulation, assuming no
-        external risk
-        '
+        desc: 'animal from outside the metapopulation, assuming no external risk'
         health_state: S
         age_group: default
 
 #   _____ _        _
 #  / ____| |      | |
 # | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
 #  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
@@ -297,21 +314,18 @@
 
 statevars:
   initial_prevalence:
     desc: 'Initial prevalence in the herd'
   purchased:
     desc: 'Total number of animals purchased by the herd over
     time. This variable is updated by the exchange process in Python
-    file.
-    '
+    file.'
   sold:
     desc: 'Total number of animals sold by the herd over
-    time. This variable is updated by the exchange process in Python
-    file.
-    '
+    time. This variable is updated by the exchange process in Python file.'
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
@@ -335,14 +349,38 @@
       amount: 'initial_infected'
   metapop:
     - prototype: infected_herd
       amount: 1
     - prototype: healthy_herd
       amount: 'nb_herds - 1'
 
+#  _____                   _
+# |_   _|                 | |
+#   | |  _ __  _ __  _   _| |_
+#   | | | '_ \| '_ \| | | | __|
+#  _| |_| | | | |_) | |_| | |_
+# |_____|_| |_| .__/ \__,_|\__|
+#             | |
+#             |_|
+#  _____        _
+# |  __ \      | |
+# | |  | | __ _| |_ __ _
+# | |  | |/ _` | __/ _` |
+# | |__| | (_| | || (_| |
+# |_____/ \__,_|\__\__,_|
+
+input_data:
+  preprocessing:
+    - file: 'compart_SIR_JA_metapop_data.py'
+      class_name: TradeMovementsReader
+      desc: 'A preprocessor class for reading the CSV that describes the trade movements and restructuring it as a dictionary, stored in shared information in the simulation.'
+      input_files:
+        trade_file: 'moves.csv'
+
+
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
 #  \____/ \__,_|\__| .__/ \__,_|\__|___/
 #                  | |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_metapop_params.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_metapop_params.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -235,17 +235,17 @@
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
     value: 'initial_population_size * initial_prevalence'
-#  transmission_I:
-#    desc: 'transmission rate from infectious individuals (/day)'
-#    value: 0.5
+  transmission_I:
+    desc: 'transmission rate from infectious individuals (/day)'
+    value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
@@ -386,10 +386,10 @@
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
-      - birth
-      - transmission_I
+      - percentage_prevalence
+      - total_population
 ...
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_SIR_struct.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_demo_random.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 ---
-# [HEADER]
+
+# EMULSION (Epidemiological Multi-Level Simulation framework)
+# ===========================================================
+# 
+# Contributors and contact:
+# -------------------------
+# 
+#     - Sébastien Picault (sebastien.picault@inrae.fr)
+#     - Yu-Lin Huang
+#     - Vianney Sicard
+#     - Sandie Arnoux
+#     - Gaël Beaunée
+#     - Pauline Ezanno (pauline.ezanno@inrae.fr)
+# 
+#     INRAE, Oniris, BIOEPAR, 44300, Nantes, France
+# 
+# 
+# How to cite:
+# ------------
+# 
+#     S. Picault, Y.-L. Huang, V. Sicard, S. Arnoux, G. Beaunée,
+#     P. Ezanno (2019). "EMULSION: Transparent and flexible multiscale
+#     stochastic models in human, animal and plant epidemiology", PLoS
+#     Computational Biology 15(9): e1007342. DOI:
+#     10.1371/journal.pcbi.1007342
+# 
+# 
+# License:
+# --------
+# 
+#     Copyright 2016 INRAE and Univ. Lille
+# 
+#     Inter Deposit Digital Number: IDDN.FR.001.280043.000.R.P.2018.000.10000
+# 
+#     Agence pour la Protection des Programmes,
+#     54 rue de Paradis, 75010 Paris, France
+# 
+#     Licensed under the Apache License, Version 2.0 (the "License");
+#     you may not use this file except in compliance with the License.
+#     You may obtain a copy of the License at
+# 
+#         http://www.apache.org/licenses/LICENSE-2.0
+# 
+#     Unless required by applicable law or agreed to in writing, software
+#     distributed under the License is distributed on an "AS IS" BASIS,
+#     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#     See the License for the specific language governing permissions and
+#     limitations under the License.
 
 #  __  __           _      _
 # |  \/  |         | |    | |
 # | \  / | ___   __| | ___| |
 # | |\/| |/ _ \ / _` |/ _ \ |
 # | |  | | (_) | (_| |  __/ |
 # |_|  |_|\___/ \__,_|\___|_|
@@ -11,24 +58,25 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
+
 # NAME OF THE MODEL
-model_name: hybrid_SIR_struct
+model_name: hybrid_SIR_JA_demo_random
+
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  hybrid SIR model with demography and age structure, with
-  non-exponential durations in state J. Besides, a contact
-  structure is added to account for physical separation between
-  Juveniles and Adults.'
+  hybrid SIR model with explicit age groups and demography.
+  Initialization uses random multinomial sampling of prototypes
+  (between healthy and infectious) and of states (for age group).'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -36,55 +84,55 @@
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: days
+  time_unit: 'days'
   delta_t: 1
   origin: 'January 1'
-  total_duration: '200'
+  total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# An individual-based model (IBM) (or a hybrid model) considers both
-# the individual and the population levels:
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: hybrid
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
+
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model (or in a Hybrid model), processes take
-# place at the population level and are managed by groupings
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
   individuals:
-    - health_state: details
-    - age_group: details
-
+    - health_state: infection
+    - age_group: aging
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -95,22 +143,19 @@
 # DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
-# Groupings are required for defining processes in compartement-based
-# or hybrid models.
+
 grouping:
   population:
-    # this grouping relies on two variables: the health state but also
-    # the age_group, since the value of variables is_A/is_J used in
-    # the force of infection is determined by the age group
-    details: [health_state, age_group]
+    infection: [health_state]
+    aging: [age_group]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -139,45 +184,41 @@
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
+
   age_group:
-    desc: 'The state machine which defines the evolution of age groups'
+    desc: 'The state machine which defines the evolution of age groups.'
     states:
       - J:
           name: 'Juvenile'
-          desc: 'Young individuals'
+          desc: 'juvenile individuals'
           fillcolor: 'orange'
-          default: yes
-          duration: '1/maturation'
       - A:
           name: 'Adult'
-          desc: 'Adult individuals'
+          desc: 'adult individuals (producing new juveniles)'
           fillcolor: 'brown'
       - D:
           name: 'Dead'
-          desc: 'compartment to represent deceased individuals'
-          fillcolor: 'white'
+          desc: 'compartment to put dead individuals'
+          fillcolor: white
           autoremove: yes
     transitions:
-      - {from: J, to: A, proba: 1}
-      - {from: A, to: D, rate: 'mortality'}
-      - {from: J, to: D, rate: 'mortality', escape: yes}
+      - {from: J, to: A, rate: 'maturation'}
+      # death (assuming no disease-induced mortality)
+      - {from: J, to: D, rate: 'death'}
+      - {from: A, to: D, rate: 'death'}
     productions:
+      # births (assuming no vertical transmission)
       - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
@@ -185,69 +226,42 @@
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-  initial_infected:
-    desc: 'initial number of infectious individuals in the population'
-    value: 1
+  initial_proba_infection:
+    desc: 'probability that an individual of the population is infectious at t=0'
+    value: 0.1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
-  transJJ:
-    desc: 'transmission rate within Juveniles age group (/day)'
-    value: 0.2
-  transAA:
-    desc: 'transmission rate within Adults age group (/day)'
-    value: 0.5
-  transJA:
-    desc: 'transmission rate from Juveniles to Adults (/day)'
-    value: 0.3
-  transAJ:
-    desc: 'transmission rate from Adults to Juveniles (/day)'
-    value: 0.05
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
-    value: 'is_J * force_of_infection_juveniles + is_A * force_of_infection_adults'
-  force_of_infection_juveniles:
-    desc: 'infection function experience by juveniles'
-    value: 'DIV(transJJ * total_I_J, total_J) + DIV(transAJ * total_I_A, total_A)'
-  force_of_infection_adults:
-    desc: 'infection function experience by adults'
-    value: 'DIV(transAA * total_I_A, total_A) + DIV(transJA * total_I_J, total_J)'
+    value: 'transmission_I * total_I / total_population'
+    source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
-  perc_prevalence_A:
-    desc: 'proportion of infected+infectious adults'
-    value: 'DIV(100 * total_I_A, total_A)'
-  perc_prevalence_J:
-    desc: 'proportion of infected+infectious juveniles'
-    value: 'DIV(100 * total_I_J, total_J)'
+  birth:
+    desc: 'the birth rate (/day)'
+    value: 0.01
+  death:
+    desc: 'the death rate (/day)'
+    value: 'birth'
   maturation:
     desc: 'rate at which juveniles become adults (/day)'
     value: '1/20'
-  b:
-    desc: 'base mortality rate (/day)'
-    value: 0.05
-  mortality:
-    desc: 'density-dependent mortality rate'
-    value: 'b * total_population / carrying_capacity'
-  birth:
-    desc: 'birth rate (/day)'
-    value: 'b * 2'
-  carrying_capacity:
-    desc: 'carrying capacity of the environment'
-    value: 'initial_population_size * 1.5'
-
+  init_prop_juveniles:
+    desc: 'average proportion of juveniles in the initial population'
+    value: 0.75
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
@@ -257,22 +271,22 @@
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: default
+        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
     - infected:
         desc: 'infected individuals'
         health_state: I
-        age_group: default
+        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
     - newborn:
-        desc: 'newborn individuals assuming no vertical transmission'
-        health_state: S
+        desc: 'newly created individuals'
+        health_state: default
         age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
@@ -287,18 +301,22 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: healthy
-      amount: 'initial_population_size - initial_infected'
-    - prototype: infected
-      amount: 'initial_infected'
+    - prototype: [infected, healthy]
+      # two possible prototypes for individual initially in the population
+      amount: initial_population_size
+      # drawn among a population of size initial_population_size
+      proba: [initial_proba_infection, 1-initial_proba_infection]
+      # with respective probabilities initial_proba_infection and
+      # 1-initial_proba_infection
+
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -314,10 +332,8 @@
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
       - total_population
-      - perc_prevalence_A
-      - perc_prevalence_J
 ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_duration.yaml` & `emulsion-1.3b1/models/features/compart_SIR_demo.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -60,20 +60,20 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_duration
+model_name: compart_SIR_demo
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model demonstrate how to assign a duration to a state.'
+  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SIR model with demography.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -95,63 +95,50 @@
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
-# its components (individuals)
 levels:
+  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
+    aggregation_type: 'compartment'
     contains:
       - individuals
+  # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
-    desc: 'level of the individuals'
-
+    desc: 'level of individuals'
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
 processes:
   individuals:
-    - age_group: aging
+    - health_state                 # name of a state machine
+
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
-
-grouping:
-  population:
-    aging: [age_group]
-
+# not used here
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -160,79 +147,106 @@
 # Each state machine is composed at least of several states.
 # The name of a state machine defines an individual variable which
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
-  # Below, the definition of the state machine used by the process
-  # 'infection'
-  age_group:
-    desc: 'The state machine which defines the evolution of age
-    groups.'
-    # Below, the list of states with their attributes.
+  health_state:
+    desc: 'The state machine which defines the evolution of health states'
     states:
-      - N:
-          name: 'Newborn'
-          desc: 'very young individuals'
+      - S:
+          name: 'Susceptible'
+          desc: 'suceptible of becoming infected'
+          fillcolor: 'wheat'
+      - I:
+          name: 'Infectious'
+          desc: 'infected and able to transmit the disease'
+          fillcolor: 'maroon'
+      - R:
+          name: 'Resistant'
+          desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-          duration: 'juvenile_age'
-          default: yes
-      - J:
-          name: 'Juvenile'
-          desc: 'juvenile individuals'
-          fillcolor: 'orange'
-          duration: 'adult_age - juvenile_age'
-      - A:
-          name: 'Adult'
-          desc: 'adult individuals (producing new juveniles)'
-          fillcolor: 'brown'
+      - D:
+          name: 'Dead'
+          desc: 'compartment to put dead individuals'
+          fillcolor: white
+          # the autoremove property specifies that this compartment is
+          # automatically emptied
+          autoremove: yes
     transitions:
-      - {from: N, to: J, proba: 1}
-      - {from: J, to: A, proba: 1}
-      # equivalent to:
-      # - {from: N, to: J, amount-all-but: 0}
-      # - {from: J, to: A, amount-all-but: 0}
-
+      - {from: S, to: I, rate: 'force_of_infection'}
+      - {from: I, to: R, rate: 'recovery'}
+      # death (assuming no disease-induced mortality)
+      - {from: S, to: D, rate: death}
+      - {from: I, to: D, rate: death}
+      - {from: R, to: D, rate: death}
+    productions:
+      # births (assuming no vertical transmission)
+      - {from: S, to: S, rate: birth, prototype: newborn}
+      - {from: I, to: S, rate: birth, prototype: newborn}
+      - {from: R, to: S, rate: birth, prototype: newborn}
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-  juvenile_age:
-    desc: 'age at which newborns become juveniles (days)'
-    value: 20
-  adult_age:
-    desc: 'age at which individuals become adults (days)'
-    value: 'random_uniform(50, 70)'
+  initial_infected:
+    desc: 'initial number of infectious individuals in the population'
+    value: 1
+  transmission_I:
+    desc: 'transmission rate from infectious individuals (/day)'
+    value: 0.5
+  recovery:
+    desc: 'recovery rate (/day)'
+    value: 0.1
+  force_of_infection:
+    desc: 'infection function'
+    value: 'transmission_I * total_I / total_population'
+    source: 'classical function assuming frequency dependence'
+  percentage_prevalence:
+    desc: 'proportion of infected+infectious individuals'
+    value: '100 * total_I / total_population'
+  birth:
+    desc: 'the birth rate (/day)'
+    value: 0.01
+  death:
+    desc: 'the death rate (/day)'
+    value: 'birth'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
+    - healthy:
+        desc: 'healthy individuals'
+        health_state: S
+    - infected:
+        desc: 'infected individuals'
+        health_state: I
     - newborn:
-        desc: 'newborn individuals'
-        age_group: N
+        desc: 'newly created individuals'
+        health_state: S
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -246,16 +260,18 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: newborn
-      amount: 'initial_population_size'
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -268,8 +284,11 @@
 # for all state machines each time step during the simulation.
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
+    extra_vars:
+      - percentage_prevalence
+      - total_population
 ...
```

### Comparing `emulsion-1.2rc5/doc/html/_static/models/features/hybrid_gest.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_gest.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/doc/html/_static/models/quickstart/quickstart.yaml` & `emulsion-1.3b1/doc/html/_static/models/quickstart/quickstart.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 # DESCRIPTION OF COMPARTMENTS ASSOCIATED WITH PROCESSES WHICH ARE NOT
 # BASED ON METHODS:
 grouping:
   population:
     infection: [health_state]
     aging: [life_cycle, age_group]
-    
+
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
 
@@ -273,17 +273,17 @@
 parameters:
   initial_population_size:
     desc: 'initial number of animals in the population'
     value: 100
   initial_infected:
     desc: 'initial number of infected animals in the population'
     value: 10
-#  adult_age:
-#    desc: 'minimal age required to produce offspring (days)'
-#    value: '365*2'
+  adult_age:
+    desc: 'minimal age required to produce offspring (days)'
+    value: '365*2'
   init_age_distrib:
     desc: 'distribution of initial ages'
     value: 'randint(0, adult_age)'
   gestation_duration:
     desc: 'duration of the gestation (in days)'
     value: '30*8'
   delay_before_new_gestation:
@@ -336,15 +336,15 @@
     quarantine zone is full)
     '
     value: '0.01*room_in_quarantine'
   room_in_quarantine:
     desc: '1 if number of animals in quarantine < quarantine_size, 0
     otherwise
     '
-    value: 'float(StrictLessThan(total_Q, quarantine_size))'
+    value: 'StrictLessThan(total_Q, quarantine_size)'
   percentage_prevalence:
     desc: '% of animals infected (E+I+Q)'
     value: '100 * (total_E + total_I + total_Q) / total_population'
   view_quarantine:
     desc: 'show quarantine period (*100 for visualization)'
     value: '100 * quarantine_period'
   global_abortion:
```

### Comparing `emulsion-1.2rc5/models/features/IBM_ABC.yaml` & `emulsion-1.3b1/models/features/IBM_SIR.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -60,22 +60,22 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: IBM_ABC
+model_name: IBM_SIR
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" model, i.e. with individuals grouped according to
-  relevant variables such as their health state. '
+  individual-based SIR model.
+  '
   author: 'Sebastien Picault (sebastien.picault@inra.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -97,20 +97,21 @@
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
+# An individual-based model considers two levels: the population and
 # its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'   # the keyword for designing hybrid models
+    aggregation_type: 'IBM'   # the keyword for designing
+                              # invididual-based models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -118,19 +119,34 @@
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
+# In an Individual-Based Model, processes take place at the individuals
+# level and are thus directly managed by state machines
 processes:
   individuals:
-    - health_state
+    - health_state                 # name of a state machine
+
+
+#   _____                       _
+#  / ____|                     (_)
+# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
+# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
+# | |__| | | | (_) | |_| | |_) | | | | | (_| |
+#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
+#                        | |             __/ |
+#                        |_|            |___/
+
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# Individual-Based Models do not use groupings
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -147,49 +163,64 @@
   # 'infection'
   health_state:
     desc: 'The state machine which defines the evolution of health
     states
     '
     # Below, the list of states with their attributes.
     states:
-      - A:
-          name: 'A'
-          desc: 'A'
+      - S:
+          name: 'Susceptible'
+          desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
-          # duration: 10
-      - B:
-          name: 'B'
-          desc: 'B'
+      - I:
+          name: 'Infectious'
+          desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
-      - C:
-          name: 'C'
-          desc: 'C'
+      - R:
+          name: 'Resistant'
+          desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     # Below, a list of transitions between states, with rate or
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
-      - {from: A, to: C, proba: 0.8}
-      - {from: A, to: B, proba: 0.2}
+      - {from: S, to: I, rate: 'force_of_infection'}
+      - {from: I, to: R, rate: 'recovery'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
+  initial_infected:
+    desc: 'initial number of infectious individuals in the population'
+    value: 1
+  transmission_I:
+    desc: 'transmission rate from infectious individuals (/day)'
+    value: 0.5
+  recovery:
+    desc: 'recovery rate (/day)'
+    value: 0.1
+  force_of_infection:
+    desc: 'infection function'
+    value: 'transmission_I * total_I / total_population'
+    source: 'classical function assuming frequency dependence'
+  percentage_prevalence:
+    desc: 'proportion of infected+infectious individuals'
+    value: '100 * total_I / total_population'
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
@@ -197,17 +228,20 @@
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
-    - default:
-        desc: 'default individuals'
-        health_state: A
+    - healthy:
+        desc: 'healthy individuals'
+        health_state: S
+    - infected:
+        desc: 'infected individuals'
+        health_state: I
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -221,16 +255,18 @@
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: default
-      amount: 'initial_population_size'
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -243,8 +279,11 @@
 # for all state machines each time step during the simulation.
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
+    extra_vars:
+      - percentage_prevalence
+      - total_population
 ...
```

### Comparing `emulsion-1.2rc5/models/features/IBM_SEIRS.yaml` & `emulsion-1.3b1/models/features/IBM_SEIRS.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_cumul_inc.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,23 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: IBM_SIR
+model_name: IBM_SIR_cumul_inc
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  individual-based SIR model.
-  '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
+  individual-based SIR model. It records the cumulative incidence
+  (total number of individuals that got infectious over time).'
+  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -118,16 +118,16 @@
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
-# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In an Individual-Based Model, processes take place at the individuals
+# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP In
+# an Individual-Based Model, processes take place at the individuals
 # level and are thus directly managed by state machines
 processes:
   individuals:
     - health_state                 # name of a state machine
 
 
 #   _____                       _
@@ -171,14 +171,16 @@
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
+          on_enter:
+            - record_change: cumulative_incidence
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     # Below, a list of transitions between states, with rate or
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
@@ -282,8 +284,9 @@
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
       - total_population
+      - cumulative_incidence
 ...
```

### Comparing `emulsion-1.2rc5/models/features/IBM_SIRS_periodic_risk.yaml` & `emulsion-1.3b1/models/features/IBM_SIRS_periodic_risk.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_demo.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_JA_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_demo_prototypes.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_demo_prototypes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: IBM_SIR_JA_demo_prototypes
+model_name: hybrid_SIR_JA_demo_prototypes
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  individual-based SIR model with explicit age groups and demography.
+  hybrid SIR model with explicit age groups and demography.
   Data-based prototype collections are used to initialize
   individuals and populations.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
@@ -108,15 +108,15 @@
   metapop:
     desc: 'level of the metapopulation'
     contains:
       - population
     aggregation_type: 'metapopulation'
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
 
@@ -128,16 +128,16 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
   individuals:
-    - health_state
-    - age_group
+    - health_state: infection
+    - age_group: aging
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -151,14 +151,15 @@
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
 grouping:
   population:
+    infection: [health_state]
     aging: [health_state, age_group]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
```

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_demo_random.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_JA_demo_random.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_metapop.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_metapop_params.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -59,21 +59,22 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: IBM_SIR_JA_metapop
+model_name: hybrid_SIR_metapop_data
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  individual-based SIR model with demography and age structure, at the
-  metapopulation scale.'
+  hybrid SIR model with demography and age structure, at the
+  metapopulation scale. Several herd parameters are herd- and time-
+  dependent, specified in a CSV file - see section input_data'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -100,60 +101,64 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # Here we introduced a third level, aggregating populations within
 # a metapopulation
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'
+    aggregation_type: hybrid
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
   metapop:
     desc: 'level of the metapopulation'
     contains:
       - population
     aggregation_type: metapopulation
-    aggregate_vars:
-      - name: metapop_total_population
-        collect: total_population
-        operator: sum
-      - name: metapop_total_I
-        collect: total_I
-        operator: sum
 
 
-#  _____
-# |  __ \
-# | |__) | __ ___   ___ ___  ___ ___  ___  ___
-# |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
-# | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
-# |_|   |_|  \___/ \___\___||___/___/\___||___/
-
-# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model (or in a Hybrid model), processes take
-# place at the population level and are managed by groupings
-processes:
-  individuals:
-    - health_state
-    - age_group
-
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
 # DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
 # DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+# Groupings are required for defining processes in compartement-based
+# or hybrid models.
+grouping:
+  population:
+    infection: [health_state]
+    aging: [age_group]
+
+
+#  _____
+# |  __ \
+# | |__) | __ ___   ___ ___  ___ ___  ___  ___
+# |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
+# | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
+# |_|   |_|  \___/ \___\___||___/___/\___||___/
 
+# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
+# In a Compartment-Based Model (or in a Hybrid model), processes take
+# place at the population level and are managed by groupings
+processes:
+  individuals:
+    - health_state: infection
+    - age_group: aging
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -166,15 +171,17 @@
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health states'
+    desc: 'The state machine which defines the evolution of health
+    states
+    '
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
           default: yes
@@ -191,15 +198,16 @@
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
   age_group:
-    desc: 'The state machine which defines the evolution of age groups'
+    desc: 'The state machine which defines the evolution of age groups
+    '
     states:
       - J:
           name: 'Juvenile'
           desc: 'Young individuals'
           fillcolor: 'orange'
           default: yes
       - A:
@@ -224,90 +232,104 @@
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
-  initial_population_size:
-    desc: 'initial number of individuals in the population'
-    value: 100
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
     value: 'initial_population_size * initial_prevalence'
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
-  transmission_between_populations:
-    desc: 'transmission rate from other infectious individuals situated in other populations of the metapopulation (/day)'
-    value: 0.01
-  force_of_infection_between:
-    desc: 'infection function resulting from possible contacts with other population'
-    value: 'transmission_between_populations * DIV(metapop_total_I - total_I, metapop_total_population - total_population)'
-  force_of_infection_within:
-    desc: 'force of infection within the population'
-    value: 'transmission_I * total_I / total_population'
   force_of_infection:
-    desc: 'total force of infection'
-    value: 'force_of_infection_within + force_of_infection_between'
+    desc: 'infection function'
+    value: 'transmission_I * total_I / total_population'
+    source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
   maturation:
     desc: 'rate at which juveniles become adults (/day)'
     value: '1/20'
   b:
     desc: 'base mortality rate (/day)'
     value: 0.05
   mortality:
     desc: 'density-dependent mortality rate'
     value: 'b * total_population / carrying_capacity'
-  birth:
-    desc: 'birth rate (/day)'
-    value: 'b * 2'
-  carrying_capacity:
-    desc: 'carrying capacity of the environment'
-    value: 150
   nb_populations:
     desc: 'number of populations in metapopulation'
-    value: 4
+    value: 10
 
 #   _____ _        _
 #  / ____| |      | |
 # | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
 #  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
 #  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
 # |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
 
 statevars:
   initial_prevalence:
     desc: 'Initial prevalence in the population'
+  initial_population_size:
+    desc: 'initial number of individuals in the population'
+  carrying_capacity:
+    desc: 'carrying capacity of the environment'
+
+
+#  _____                   _
+# |_   _|                 | |
+#   | |  _ __  _ __  _   _| |_
+#   | | | '_ \| '_ \| | | | __|
+#  _| |_| | | | |_) | |_| | |_
+# |_____|_| |_| .__/ \__,_|\__|
+#             | |
+#             |_|
+#  _____        _
+# |  __ \      | |
+# | |  | | __ _| |_ __ _
+# | |  | |/ _` | __/ _` |
+# | |__| | (_| | || (_| |
+# |_____/ \__,_|\__\__,_|
+
+input_data:
+  data_based_parameters:
+    - level: population
+      file: 'pop_parameters.csv'
+      key_variables: [population_id, step]
+      parameters:
+        transmission_I:
+          desc: 'transmission rate from infectious individuals (/day)'
+          # value: 0.5
+        birth:
+          desc: 'birth rate (/day)'
+
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   population:
-    - healthy_population:
-        desc: 'population initially without infected individuals'
-        initial_prevalence: 0
-    - infected_population:
-        desc: 'population initially infected individuals'
-        initial_prevalence: 0.1
+    - data_based_population:
+        desc: 'population which initial size, carrying capacity and prevalence are driven by data'
+        file: 'pop_structure.csv'
+        select: 'ordered_cycle'
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
         age_group: default
     - infected:
         desc: 'infected individuals'
@@ -341,18 +363,16 @@
 initial_conditions:
   population:
     - prototype: healthy
       amount: 'initial_population_size - initial_infected'
     - prototype: infected
       amount: 'initial_infected'
   metapop:
-    - prototype: infected_population
-      amount: 1
-    - prototype: healthy_population
-      amount: 'nb_populations - 1'
+    - prototype: data_based_population
+      amount: 'nb_populations'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
```

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_metapop_data.py` & `emulsion-1.3b1/models/features/IBM_SIR_JA_metapop_data.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_metapop_data.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_JA_metapop_data.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_JA_struct.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_JA_struct.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_age_demo.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_age_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_aggreg.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_aggreg.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_cumul_inc.yaml` & `emulsion-1.3b1/models/features/compart_SIR_cumul_inc.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: IBM_SIR_cumul_inc
+model_name: compart_SIR_cumul_inc
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  individual-based SIR model. It records the cumulative incidence
+  compartment-based SIR model. It records the cumulative incidence
   (total number of individuals that got infectious over time).'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
@@ -96,57 +96,53 @@
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
+
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# An individual-based model considers two levels: the population and
-# its components (individuals)
 levels:
+  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: 'IBM'   # the keyword for designing
-                              # invididual-based models
+    aggregation_type: 'compartment'
     contains:
       - individuals
+  # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
-    desc: 'level of the individuals'
-
+    desc: 'level of individuals'
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
-# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP In
-# an Individual-Based Model, processes take place at the individuals
-# level and are thus directly managed by state machines
+# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
+# In a Compartment-Based Model, processes take place at the population
+# level and are managed by groupings
 processes:
   individuals:
-    - health_state                 # name of a state machine
+    - health_state
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# Individual-Based Models do not use groupings
-
+# not used here
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -158,17 +154,15 @@
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
+    desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
       - I:
@@ -213,39 +207,39 @@
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
-    desc: 'proportion of infected+infectious individuals'
+    desc: 'proportion of infected+infectious individuals (%)'
     value: '100 * total_I / total_population'
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
+
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
     - infected:
         desc: 'infected individuals'
         health_state: I
 
-
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
 
@@ -253,24 +247,23 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
+# Initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
     - prototype: healthy
       amount: 'initial_population_size - initial_infected'
     - prototype: infected
       amount: 'initial_infected'
 
-
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
 #  \____/ \__,_|\__| .__/ \__,_|\__|___/
 #                  | |
```

### Comparing `emulsion-1.2rc5/models/features/IBM_SIR_demo.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_demo.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/IBM_duration.yaml` & `emulsion-1.3b1/src/emulsion/agent/core/groups.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,17 @@
----
+
+"""
+.. module:: emulsion.agent.core.groups
+
+.. moduleauthor:: Sébastien Picault <sebastien.picault@inra.fr>
+
+Part of this code was adapted from the PADAWAN framework (S. Picault,
+Univ. Lille).
+"""
+
 
 # EMULSION (Epidemiological Multi-Level Simulation framework)
 # ===========================================================
 # 
 # Contributors and contact:
 # -------------------------
 # 
@@ -44,222 +53,171 @@
 # 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-#  __  __           _      _
-# |  \/  |         | |    | |
-# | \  / | ___   __| | ___| |
-# | |\/| |/ _ \ / _` |/ _ \ |
-# | |  | | (_) | (_| |  __/ |
-# |_|  |_|\___/ \__,_|\___|_|
-#
-#  _____        __                           _   _
-# |_   _|      / _|                         | | (_)
-#   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
-#   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
-#  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
-# |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
-
-
-# NAME OF THE MODEL
-model_name: IBM_duration
-
-
-# DESCRIPTION OF THE MODEL
-model_info:
-  abstract: 'This model demonstrate how to assign a duration to a state.'
-  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
-
-
-#  _______ _
-# |__   __(_)
-#    | |   _ _ __ ___   ___
-#    | |  | | '_ ` _ \ / _ \
-#    | |  | | | | | | |  __/
-#    |_|  |_|_| |_| |_|\___|
-
-# TIME INFORMATION
-# This section defines the time unit (used e.g. for expressing
-# durations, rates, etc.), the duration of the time step, the origin
-# date and total duration of the simulation.
-time_info:
-  time_unit: 'days'
-  delta_t: 1
-  origin: 'January 1'
-  total_duration: '100'
-
-
-#  _                    _
-# | |                  | |
-# | |     _____   _____| |___
-# | |    / _ \ \ / / _ \ / __|
-# | |___|  __/\ V /  __/ \__ \
-# |______\___| \_/ \___|_|___/
-
-# ORGANIZATION LEVELS USED IN THE SIMULATION
-# An individual-based model considers two levels: the population and
-# its components (individuals)
-levels:
-  population:
-    desc: 'level of the population'
-    aggregation_type: 'IBM'
-    contains:
-      - individuals
-  individuals:
-    desc: 'level of the individuals'
-
-
-
-#  _____
-# |  __ \
-# | |__) | __ ___   ___ ___  ___ ___  ___  ___
-# |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
-# | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
-# |_|   |_|  \___/ \___\___||___/___/\___||___/
-
-# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In an Individual-Based Model, processes take place at the individuals
-# level and are thus directly managed by state machines
-processes:
-  individuals:
-    - age_group
-
-
-#   _____                       _
-#  / ____|                     (_)
-# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
-# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
-# | |__| | | | (_) | |_| | |_) | | | | | (_| |
-#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
-#                        | |             __/ |
-#                        |_|            |___/
-
-# not used here
-
-#   _____ _        _         __  __            _     _
-#  / ____| |      | |       |  \/  |          | |   (_)
-# | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
-#  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
-#  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
-# |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
-
-# DESCRIPTION OF THE STATE MACHINES INVOLVED IN THE MODEL
-# Each state machine is composed at least of several states.
-# The name of a state machine defines an individual variable which
-# contains the value of the current state in the individual.
-# Transitions define how each change can change to another one.
-# Productions define how individuals in one state can produce
-# new individuals in another state.
-state_machines:
-  # Below, the definition of the state machine used by the process
-  # 'infection'
-  age_group:
-    desc: 'The state machine which defines the evolution of age
-    groups.
-    '
-    # Below, the list of states with their attributes.
-    states:
-      - N:
-          name: 'Newborn'
-          desc: 'very young individuals'
-          fillcolor: 'deepskyblue'
-          duration: 'juvenile_age'
-          default: yes
-      - J:
-          name: 'Juvenile'
-          desc: 'juvenile individuals'
-          fillcolor: 'orange'
-          duration: 'adult_age - juvenile_age'
-      - A:
-          name: 'Adult'
-          desc: 'adult individuals (producing new juveniles)'
-          fillcolor: 'brown'
-    transitions:
-      - {from: N, to: J, proba: 1}
-      - {from: J, to: A, proba: 1}
-      # equivalent to:
-      # - {from: N, to: J, amount-all-but: 0}
-      # - {from: J, to: A, amount-all-but: 0}
-
-
-#  _____                               _
-# |  __ \                             | |
-# | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
-# |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
-# | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
-# |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
-
-# PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
-parameters:
-  initial_population_size:
-    desc: 'initial number of individuals in the population'
-    value: 100
-  juvenile_age:
-    desc: 'age at which newborns become juveniles (days)'
-    value: 20
-  adult_age:
-    desc: 'age at which individuals become adults (days)'
-    value: 'random_uniform(50, 70)'
-
-#  _____           _        _
-# |  __ \         | |      | |
-# | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
-# |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
-# | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
-# |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
-#                                __/ | |
-#                               |___/|_|
-
-# PROTOTYPES describe typical individuals, characterized by specific
-# values of their variables
-prototypes:
-  individuals:
-    - newborn:
-        desc: 'newborn individuals'
-        age_group: N
-
-
-#  _____       _ _   _       _
-# |_   _|     (_) | (_)     | |
-#   | |  _ __  _| |_ _  __ _| |
-#   | | | '_ \| | __| |/ _` | |
-#  _| |_| | | | | |_| | (_| | |
-# |_____|_| |_|_|\__|_|\__,_|_|
-
-#   _____                _ _ _   _
-#  / ____|              | (_) | (_)
-# | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
-# | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
-# | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
-#  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
-
-# INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
-# involved with the amount of individuals in each of those prototypes
-initial_conditions:
-  population:
-    - prototype: newborn
-      amount: 'initial_population_size'
-
-
-#   ____        _               _
-#  / __ \      | |             | |
-# | |  | |_   _| |_ _ __  _   _| |_ ___
-# | |  | | | | | __| '_ \| | | | __/ __|
-# | |__| | |_| | |_| |_) | |_| | |_\__ \
-#  \____/ \__,_|\__| .__/ \__,_|\__|___/
-#                  | |
-#                  |_|
-
-# TYPE AND PERIODICITY OF OUTPUTS
-# The amount of individuals in each state is automatically recorded
-# for all state machines each time step during the simulation.
-# Additional variables (e.g. expressions defined in the 'parameters'
-# section) can be specified below (as 'extra_vars').
-outputs:
-  type: csv
-  population:
-    period: 1
-...
+import abc
+
+from   emulsion.agent.core.emulsion_agent  import EmulsionAgent
+from   emulsion.tools.debug      import debuginfo
+
+#   _____                                               _
+#  / ____|                        /\                   | |
+# | |  __ _ __ ___  _   _ _ __   /  \   __ _  ___ _ __ | |_
+# | | |_ | '__/ _ \| | | | '_ \ / /\ \ / _` |/ _ \ '_ \| __|
+# | |__| | | | (_) | |_| | |_) / ____ \ (_| |  __/ | | | |_
+#  \_____|_|  \___/ \__,_| .__/_/    \_\__, |\___|_| |_|\__|
+#                        | |            __/ |
+#                        |_|           |___/
+
+class GroupAgent(EmulsionAgent):
+    """A GroupAgent is aimed at representing a group of agents. The
+    underlying level may be either explicitly represented (using a
+    ViewCompartment) or aggregated (using an Compartment). Each
+    compartment is associated with keys, i.e. a tuple of state
+    variables (possibly empty) which play a crucial role in this
+    compartment.
+
+    """
+    def __init__(self, keys=(), **others):
+        super().__init__(**others)
+        self.keys = keys
+        self.autoremove = False
+
+
+    @abc.abstractmethod
+    def add(self, population):
+        """Add the specified population to the current compartment."""
+        pass
+
+    @abc.abstractmethod
+    def remove(self, population):
+        """Remove the specified population from the current
+        compartment.
+
+        """
+        pass
+
+    @abc.abstractmethod
+    def _base_move(self, other_unit, **others):
+        pass
+
+    def _before_move(self, state_machine, old_state, new_state, **others):
+        # execute actions when exiting current state (if any)
+        self.do_state_actions('on_exit', state_machine, old_state, **others)
+        # execute actions when crossing edge (if any)
+        self.do_edge_actions(**others)
+        # update states of atom units
+        if 'agents' in others:
+            for unit in others['agents']:
+                unit.change_state(state_machine.machine_name,
+                                  state_machine.states[new_state])
+                # unit.statevars[state_machine.machine_name] =\
+                #   state_machine.states[new_state]
+
+    def _after_move(self, state_machine, new_state, **others):
+        # execute actions when entering new state (if any)
+        self.do_state_actions('on_enter', state_machine, new_state, **others)
+
+
+
+    def move_to(self, target_group, state_machine=None, **others):
+        """Move the specified population from the current group to the target group.
+        If a state machine is provided, executes the corresponding actions when
+        entering/exiting nodes and crossing edges if needed.
+
+        """
+        if state_machine:
+            #old_state = self.get_information(state_machine.machine_name).name
+            old_state = self.statevars[state_machine.machine_name]
+            new_state = target_group.statevars[state_machine.machine_name].name
+            if old_state is not None:
+                self._before_move(state_machine, old_state.name, new_state, **others)
+        # move population from current compartment to other unit
+        self._base_move(target_group, state_machine=state_machine, **others)
+        if state_machine:
+            target_group._after_move(state_machine, new_state, **others)
+
+
+
+#                                           _   _
+#     /\                                   | | (_)
+#    /  \   __ _  __ _ _ __ ___  __ _  __ _| |_ _  ___  _ __
+#   / /\ \ / _` |/ _` | '__/ _ \/ _` |/ _` | __| |/ _ \| '_ \
+#  / ____ \ (_| | (_| | | |  __/ (_| | (_| | |_| | (_) | | | |
+# /_/    \_\__, |\__, |_|  \___|\__, |\__,_|\__|_|\___/|_| |_|
+#           __/ | __/ |          __/ |
+#          |___/ |___/          |___/
+
+
+class Aggregation(GroupAgent):
+    """An Aggregation is aimed at grouping agents from the underlying
+    level. Thus, aggregate information such as the total number of
+    agents in the compartment (population) is calculated from the
+    actual content of the compartment. The evolution of a
+    ViewCompartment, by default, consists in making the units
+    contained in the compartment evolve themselves, unless
+    `recursive=False` is specified during instantiation.
+
+    """
+    def __init__(self, recursive=True, **others):
+        super().__init__(**others)
+        self._content = None
+        self.recursive = recursive
+
+    @property
+    def population(self):
+        """Return the total population of the compartment. It is
+        calculated either using a true 'population' statevar if any,
+        or as the sum of the population of each unit contained in the
+        compartment.
+
+        TAG: USER
+        """
+        return self.statevars.population if 'population' in self.statevars\
+            else sum([unit.get_information('population')
+                      for unit in self])
+
+    def add(self, population):
+        """Add the specified population to the current compartment."""
+        for unit in population:
+            unit.add_host(self)
+
+    def remove(self, population):
+        """Remove the specified population from the current
+        compartment.
+
+        """
+        for unit in population:
+            unit.remove_host(self, keys=self.keys)
+
+    def _base_move(self, other_unit, agents=[], **others):
+        self.remove(agents)
+        other_unit.add(agents)
+
+    @abc.abstractmethod
+    def __iter__(self):
+        pass
+
+    # TODO: shuffle content first
+    def evolve(self, machine=None):
+        """Ask each unit in the current compartment to make its content evolve
+        according to its own capabilities. A specific state machine
+        can be specified if needed.
+
+        """
+        super().evolve(machine=machine)
+        if self.recursive and self.statevars._is_active:
+            for unit in self:
+                unit.evolve(machine=machine)
+                # debuginfo("GROUPS -> STEP", unit)
+
+    def detach_model(self):
+        """Recursively remove the reference to the model in all
+        agents. Required before serialization.
+
+        """
+        super().detach_model()
+        for agent in self:
+            agent.detach_model()
```

### Comparing `emulsion-1.2rc5/models/features/IBM_gest.yaml` & `emulsion-1.3b1/models/features/IBM_gest.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/compart_SEIRS.yaml` & `emulsion-1.3b1/models/features/compart_SEIRS.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/compart_SIR.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -60,21 +60,24 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR
+model_name: hybrid_SIR
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SIR model.'
-  author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
+  abstract: 'This model is a simple discrete-time, stochastic,
+  "hybrid" SIR model, i.e. with individuals grouped according to
+  relevant variables such as their health state.
+  '
+  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
@@ -95,48 +98,63 @@
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
-  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
-  # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
-    desc: 'level of individuals'
+    desc: 'level of the individuals'
+
+
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
   individuals:
-    - health_state                 # name of a state machine
+    - health_state: infection                 # name of a grouping
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+grouping:
+  population:
+    infection: [health_state]
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -148,15 +166,17 @@
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
   # Below, the definition of the state machine used by the process
   # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health states'
+    desc: 'The state machine which defines the evolution of health
+    states
+    '
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
       - I:
@@ -199,15 +219,15 @@
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
-    desc: 'proportion of infected+infectious individuals (%)'
+    desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
@@ -223,14 +243,15 @@
     - healthy:
         desc: 'healthy individuals'
         health_state: S
     - infected:
         desc: 'infected individuals'
         health_state: I
 
+
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
 
@@ -238,15 +259,15 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# Initial conditions describe the prototypes
+# In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
     - prototype: healthy
       amount: 'initial_population_size - initial_infected'
     - prototype: infected
       amount: 'initial_infected'
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIRS_periodic_risk.yaml` & `emulsion-1.3b1/models/features/compart_SIRS_periodic_risk.yaml`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_demo.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/compart_SEIRS_tmp.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -60,20 +60,20 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR_JA_demo
+model_name: compart_SEIRS
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SIR model with explict age groups and demography.'
+  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SEIRS model.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -107,26 +107,26 @@
     contains:
       - individuals
   # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
     desc: 'level of individuals'
 
 
+
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 processes:
   individuals:
-    - health_state
-    - age_group
+    - health_state                 # name of a state machine
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -147,96 +147,84 @@
 # Each state machine is composed at least of several states.
 # The name of a state machine defines an individual variable which
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
+  # Below, the definition of the state machine used by the process
+  # 'infection'
   health_state:
     desc: 'The state machine which defines the evolution of health states'
+    # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
-          default: yes
+      - E:
+          name: 'Latent'
+          desc: 'infected but not yet able to transmit the disease'
+          fillcolor: 'orange'
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
+    # Below, a list of transitions between states, with rate or
+    # probabilities. Rates are automatically converted into
+    # probabilities w.r.t the duration of the time step (delta_t),
+    # assuming a classical exponential distribution of durations in
+    # the states.
     transitions:
-      - {from: S, to: I, rate: 'force_of_infection'}
-      - {from: I, to: R, rate: 'recovery'}
+      - {from: S, to: E, rate: '0.285*total_I'}
+      - {from: E, to: I, rate: '1/3'}
+      - {from: I, to: R, rate: '1/4.5'}
+      - {from: R, to: S, rate: '1/56'}
 
-  age_group:
-    desc: 'The state machine which defines the evolution of age groups.'
-    states:
-      - J:
-          name: 'Juvenile'
-          desc: 'juvenile individuals'
-          fillcolor: 'orange'
-      - A:
-          name: 'Adult'
-          desc: 'adult individuals (producing new juveniles)'
-          fillcolor: 'brown'
-      - D:
-          name: 'Dead'
-          desc: 'compartment to put dead individuals'
-          fillcolor: white
-          autoremove: yes
-    transitions:
-      - {from: J, to: A, rate: 'maturation'}
-      # death (assuming no disease-induced mortality)
-      - {from: J, to: D, rate: 'death'}
-      - {from: A, to: D, rate: 'death'}
-    productions:
-      # births (assuming no vertical transmission)
-      - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
-    value: 100
+    value: '15*9'
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
     value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
+  incubation:
+    desc: 'mean duration of latent state (days, assuming exponential
+    distribution of durations in the state)'
+    value: 5
+  waning:
+    desc: 'rate at which individuals lose immunity (/day)'
+    value: 0.05
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
-    value: '100 * total_I / total_population'
-  birth:
-    desc: 'the birth rate (/day)'
-    value: 0.01
-  death:
-    desc: 'the death rate (/day)'
-    value: 'birth'
-  maturation:
-    desc: 'rate at which juveniles become adults (/day)'
-    value: '1/20'
+    value: '100 * (total_I + total_E) / total_population'
+
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
@@ -246,24 +234,17 @@
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: random
     - infected:
         desc: 'infected individuals'
         health_state: I
-        age_group: random
-    - newborn:
-        desc: 'newly created individuals'
-        health_state: default
-        age_group: J
-
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
@@ -272,15 +253,15 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
+# Initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
     - prototype: healthy
       amount: 'initial_population_size - initial_infected'
     - prototype: infected
       amount: 'initial_infected'
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_demo_prototypes.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_age_demo.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -60,23 +60,21 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR_JA_demo_prototypes
+model_name: hybrid_SIR_age_demo
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with explicit age groups and demography.
-  Data-based prototype collections are used to initialize
-  individuals and populations.'
+  hybrid SIR model with age groups, explicit age and demography.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -101,24 +99,28 @@
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # A hybrid model considers two levels: the population and
 # its components (individuals)
 levels:
-  metapop:
-    desc: 'level of the metapopulation'
-    contains:
-      - population
-    aggregation_type: 'metapopulation'
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'hybrid'
     contains:
       - individuals
+    aggregate_vars:
+      # compute min and max from ages of individuals in subgroups
+      - name: min_age
+        collect: age
+        operator: 'min'
+      - name: max_age
+        collect: age
+        operator: 'max'
+
   individuals:
     desc: 'level of the individuals'
 
 
 
 #  _____
 # |  __ \
@@ -128,16 +130,16 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
 # and are managed by groupings
 processes:
   individuals:
-    - health_state
-    - age_group
+    - health_state: details
+    - age_group: details
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -149,17 +151,17 @@
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
-# grouping:
-#   population:
-#     aging: [age_group, health_state]
+grouping:
+  population:
+    details: [age_group, health_state]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -192,116 +194,129 @@
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
   age_group:
-    desc: 'The state machine which defines the evolution of age groups.'
+    desc: 'The state machine which defines the evolution of age groups'
     states:
       - J:
           name: 'Juvenile'
           desc: 'juvenile individuals'
           fillcolor: 'orange'
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
       - A:
           name: 'Adult'
           desc: 'adult individuals (producing new juveniles)'
           fillcolor: 'brown'
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
       - D:
           name: 'Dead'
           desc: 'compartment to put dead individuals'
           fillcolor: white
           autoremove: yes
     transitions:
-      - {from: J, to: A, rate: 'maturation'}
-      # death (assuming no disease-induced mortality)
-      - {from: J, to: D, rate: 'death'}
-      - {from: A, to: D, rate: 'death'}
+      - {from: J, to: A, cond: 'age >= adult_age', proba: 1}
+      - {from: A, to: D, rate: '1 / avg_adult_death_age'}
     productions:
-      # births (assuming no vertical transmission)
       - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
-  nb_populations:
-    desc: 'number of populations in the metapop'
-    value: 4
+  initial_population_size:
+    desc: 'initial number of individuals in the population'
+    value: 100
+  initial_infected:
+    desc: 'initial number of infectious individuals in the population'
+    value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
-  percentage_prevalence_J:
-    desc: 'proportion of infectious individuals in juvenile group'
-    value: '100 * total_I_J / (total_J + 1e-9)'
-  percentage_prevalence_A:
-    desc: 'proportion of infectious individuals in adult group'
-    value: '100 * total_I_A / (total_A + 1e-9)'
+  percentage_prevalence:
+    desc: 'proportion of infected+infectious individuals'
+    value: '100 * total_I / total_population'
   birth:
     desc: 'the birth rate (/day)'
     value: 0.01
   death:
     desc: 'the death rate (/day)'
     value: 'birth'
-  maturation:
-    desc: 'rate at which juveniles become adults (/day)'
-    value: '1/20'
+  avg_adult_death_age:
+    desc: 'mean longevity of adults (days)'
+    value: 120
+  adult_age:
+    desc: 'age when individuals become adults (days)'
+    value: 30
+  init_age_distrib:
+    desc: 'distribution of initial ages'
+    value: 'random_integers(0, adult_age-1)'
 
 #   _____ _        _
 #  / ____| |      | |
 # | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
 #  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
 #  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
 # |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
 
+
 statevars:
-  initial_population_size:
-    desc: 'initial number of individuals in the population (data-based)'
+  age:
+    desc: 'age of the individual'
+
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
-  population:
-    - data_based_population:
-        desc: 'collection of prototypes specifying several initial population sizes'
-        file: 'population_size.csv'
-        select: 'ordered_cycle(initial_population_size)'
-        exclude_values: ['huge_pop']
   individuals:
-    - data_based_individual:
-        desc: 'collection of prototypes describing typical distributions of individuals based on a CSV data file'
-        file: 'initial_individuals.csv'
-        select: 'random_replace(weight)'
+    - healthy:
+        desc: 'healthy individuals'
+        health_state: S
+        age_group: J
+        age: init_age_distrib
+    - infected:
+        desc: 'infected individuals'
+        health_state: I
+        age_group: J
+        age: init_age_distrib
     - newborn:
         desc: 'newly created individuals'
         health_state: default
         age_group: J
+        age: 0
+
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
@@ -313,20 +328,20 @@
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
-  metapop:
-    - prototype: data_based_population
-      amount: 'nb_populations'
   population:
-    - prototype: data_based_individual
-      amount: 'initial_population_size'
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
+
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
 #  \____/ \__,_|\__| .__/ \__,_|\__|___/
@@ -339,11 +354,15 @@
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
-      - percentage_prevalence_J
-      - percentage_prevalence_A
+      - percentage_prevalence
       - total_population
+      - min_age_A
+      - max_age_J
+      - max_age_A
+      - total_A_I
+      - max_age_A_I
 ...
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_demo_random.yaml` & `emulsion-1.3b1/models/features/compart_SEIRS_tmp.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -60,23 +60,20 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR_JA_demo_random
+model_name: compart_SEIRS
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with explicit age groups and demography.
-  Initialization uses random multinomial sampling of prototypes
-  (between healthy and infectious) and of states (for age group).'
+  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SEIRS model.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -98,41 +95,38 @@
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
-# its components (individuals)
 levels:
+  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
     aggregation_type: 'compartment'
     contains:
       - individuals
+  # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
-    desc: 'level of the individuals'
+    desc: 'level of individuals'
 
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
 processes:
   individuals:
-    - health_state
-    - age_group
+    - health_state                 # name of a state machine
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -163,93 +157,74 @@
     desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
-          default: yes
+      - E:
+          name: 'Latent'
+          desc: 'infected but not yet able to transmit the disease'
+          fillcolor: 'orange'
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
+    # Below, a list of transitions between states, with rate or
+    # probabilities. Rates are automatically converted into
+    # probabilities w.r.t the duration of the time step (delta_t),
+    # assuming a classical exponential distribution of durations in
+    # the states.
     transitions:
-      - {from: S, to: I, rate: 'force_of_infection'}
-      - {from: I, to: R, rate: 'recovery'}
-
-  age_group:
-    desc: 'The state machine which defines the evolution of age groups.'
-    states:
-      - J:
-          name: 'Juvenile'
-          desc: 'juvenile individuals'
-          fillcolor: 'orange'
-      - A:
-          name: 'Adult'
-          desc: 'adult individuals (producing new juveniles)'
-          fillcolor: 'brown'
-      - D:
-          name: 'Dead'
-          desc: 'compartment to put dead individuals'
-          fillcolor: white
-          autoremove: yes
-    transitions:
-      - {from: J, to: A, rate: 'maturation'}
-      # death (assuming no disease-induced mortality)
-      - {from: J, to: D, rate: 'death'}
-      - {from: A, to: D, rate: 'death'}
-    productions:
-      # births (assuming no vertical transmission)
-      - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
+      - {from: S, to: E, rate: '0.285*total_I'}
+      - {from: E, to: I, rate: '1/3'}
+      - {from: I, to: R, rate: '1/4.5'}
+      - {from: R, to: S, rate: '1/56'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
-    value: 100
-  initial_proba_infection:
-    desc: 'probability that an individual of the population is infectious at t=0'
-    value: 0.1
+    value: '15*9'
+  initial_infected:
+    desc: 'initial number of infectious individuals in the population'
+    value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
+  incubation:
+    desc: 'mean duration of latent state (days, assuming exponential
+    distribution of durations in the state)'
+    value: 5
+  waning:
+    desc: 'rate at which individuals lose immunity (/day)'
+    value: 0.05
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
-    value: '100 * total_I / total_population'
-  birth:
-    desc: 'the birth rate (/day)'
-    value: 0.01
-  death:
-    desc: 'the death rate (/day)'
-    value: 'birth'
-  maturation:
-    desc: 'rate at which juveniles become adults (/day)'
-    value: '1/20'
-  init_prop_juveniles:
-    desc: 'average proportion of juveniles in the initial population'
-    value: 0.75
+    value: '100 * (total_I + total_E) / total_population'
+
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
@@ -259,24 +234,17 @@
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
     - infected:
         desc: 'infected individuals'
         health_state: I
-        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
-    - newborn:
-        desc: 'newly created individuals'
-        health_state: default
-        age_group: J
-
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
@@ -285,26 +253,22 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
+# Initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
-    - prototype: [infected, healthy]
-      # two possible prototypes for individual initially in the population
-      amount: initial_population_size
-      # drawn among a population of size initial_population_size
-      proba: [initial_proba_infection, 1-initial_proba_infection]
-      # with respective probabilities initial_proba_infection and
-      # 1-initial_proba_infection
-
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_metapop.yaml` & `emulsion-1.3b1/models/features/IBM_SIR_JA_metapop.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR_JA_metapop
+model_name: IBM_SIR_JA_metapop
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with demography and age structure, at the
+  individual-based SIR model with demography and age structure, at the
   metapopulation scale.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
@@ -100,15 +100,15 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # Here we introduced a third level, aggregating populations within
 # a metapopulation
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'IBM'
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
   metapop:
     desc: 'level of the metapopulation'
     contains:
@@ -131,27 +131,40 @@
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a Compartment-Based Model (or in a Hybrid model), processes take
 # place at the population level and are managed by groupings
 processes:
   individuals:
-    - health_state
-    - age_group
+    - health_state: infection
+    - age_group: aging
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+# Groupings are required for defining processes in compartement-based
+# or hybrid models.
+grouping:
+  population:
+    infection: [health_state]
+    aging: [age_group]
+
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_metapop_data.py` & `emulsion-1.3b1/models/features/compart_SIR_JA_metapop_data.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_metapop_data.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_metapop_data.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 # NAME OF THE MODEL
-model_name: compart_SIR_metapop_data
+model_name: hybrid_SIR_metapop_data
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with demography and age structure, at the
+  hybrid SIR model with demography and age structure, at the
   metapopulation scale, with data-based trade movements responsible
   for the transmission of infection between populations.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
@@ -101,55 +101,71 @@
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # Here we introduced a third level, aggregating herds within
 # a metapopulation.
 levels:
   herd:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: hybrid
     contains:
       - animals
   animals:
     desc: 'level of the individuals'
   metapop:
     desc: 'level of the metapopulation'
     contains:
       - herd
     aggregation_type: metapopulation
     # The metapopulation is explicitly linked to a specific class in a
     # Python code add-on
-    file: 'compart_SIR_JA_metapop_data.py'
+    file: 'hybrid_SIR_JA_metapop_data.py'
     class_name: Metapopulation
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+# # Groupings are required for defining processes in compartement-based
+# # or hybrid models.
+# IBM do not require groupings since processes can be directly
+# associated with state machines.
+grouping:
+  herd:
+    infection: [health_state]
+    aging: [age_group]
+
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a Compartment-Based Model (or in a Hybrid model), processes take
 # place at the population level (here, herd) and are managed by groupings
 processes:
   animals:
-    - health_state
-    - age_group
+    - health_state: infection
+    - age_group: aging
   metapop:
     # here the process is the name of a procedure defined in the
     # Python code
     - exchange_animals
 
 
 #   _____ _        _         __  __            _     _
@@ -366,15 +382,15 @@
 # | |  | | __ _| |_ __ _
 # | |  | |/ _` | __/ _` |
 # | |__| | (_| | || (_| |
 # |_____/ \__,_|\__\__,_|
 
 input_data:
   preprocessing:
-    - file: 'compart_SIR_JA_metapop_data.py'
+    - file: 'hybrid_SIR_JA_metapop_data.py'
       class_name: TradeMovementsReader
       desc: 'A preprocessor class for reading the CSV that describes the trade movements and restructuring it as a dictionary, stored in shared information in the simulation.'
       input_files:
         trade_file: 'moves.csv'
 
 
 #   ____        _               _
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_JA_struct.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_demo.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -58,24 +58,22 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
+
 # NAME OF THE MODEL
-model_name: compart_SIR_JA_struct
+model_name: hybrid_SIR_JA_demo
+
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  compartmental SIR model with demography and age structure, with
-  non-exponential durations in state J. Besides, a contact
-  structure is added to account for physical separation between
-  Juveniles and Adults.'
+  abstract: 'This model is a simple discrete-time, stochastic, hybrid SIR model with explicit age groups and demography.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -83,67 +81,79 @@
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: days
+  time_unit: 'days'
   delta_t: 1
   origin: 'January 1'
-  total_duration: '200'
+  total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# An individual-based model (IBM) (or a hybrid model) considers both
-# the individual and the population levels:
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
+
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model (or in a Hybrid model), processes take
-# place at the population level and are managed by groupings
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
   individuals:
-    - health_state
-    - age_group
-
+    - health_state: infection
+    - age_group: aging
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+grouping:
+  population:
+    infection: [health_state]
+    aging: [age_group]
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -171,45 +181,40 @@
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
   age_group:
-    desc: 'The state machine which defines the evolution of age groups'
+    desc: 'The state machine which defines the evolution of age groups.'
     states:
       - J:
           name: 'Juvenile'
-          desc: 'Young individuals'
+          desc: 'juvenile individuals'
           fillcolor: 'orange'
-          default: yes
-          duration: '1/maturation'
       - A:
           name: 'Adult'
-          desc: 'Adult individuals'
+          desc: 'adult individuals (producing new juveniles)'
           fillcolor: 'brown'
       - D:
           name: 'Dead'
-          desc: 'compartment to represent deceased individuals'
-          fillcolor: 'white'
+          desc: 'compartment to put dead individuals'
+          fillcolor: white
           autoremove: yes
     transitions:
-      - {from: J, to: A, proba: 1}
-      - {from: A, to: D, rate: 'mortality'}
-      - {from: J, to: D, rate: 'mortality', escape: yes}
+      - {from: J, to: A, rate: 'maturation'}
+      # death (assuming no disease-induced mortality)
+      - {from: J, to: D, rate: 'death'}
+      - {from: A, to: D, rate: 'death'}
     productions:
+      # births (assuming no vertical transmission)
       - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
@@ -223,63 +228,36 @@
     value: 100
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
     value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
-  transJJ:
-    desc: 'transmission rate within Juveniles age group (/day)'
-    value: 0.2
-  transAA:
-    desc: 'transmission rate within Adults age group (/day)'
-    value: 0.5
-  transJA:
-    desc: 'transmission rate from Juveniles to Adults (/day)'
-    value: 0.3
-  transAJ:
-    desc: 'transmission rate from Adults to Juveniles (/day)'
-    value: 0.05
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
-    value: 'is_J * force_of_infection_juveniles + is_A * force_of_infection_adults'
-  force_of_infection_juveniles:
-    desc: 'infection function experience by juveniles'
-    value: 'DIV(transJJ * total_I_J, total_J) + DIV(transAJ * total_I_A, total_A)'
-  force_of_infection_adults:
-    desc: 'infection function experience by adults'
-    value: 'DIV(transAA * total_I_A, total_A) + DIV(transJA * total_I_J, total_J)'
+    value: 'transmission_I * total_I / total_population'
+    source: 'classical function assuming frequency dependence'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
-  perc_prevalence_A:
-    desc: 'proportion of infected+infectious adults'
-    value: 'DIV(100 * total_I_A, total_A)'
-  perc_prevalence_J:
-    desc: 'proportion of infected+infectious juveniles'
-    value: 'DIV(100 * total_I_J, total_J)'
+  birth:
+    desc: 'the birth rate (/day)'
+    value: 0.01
+  death:
+    desc: 'the death rate (/day)'
+    value: 'birth'
   maturation:
     desc: 'rate at which juveniles become adults (/day)'
     value: '1/20'
-  b:
-    desc: 'base mortality rate (/day)'
-    value: 0.05
-  mortality:
-    desc: 'density-dependent mortality rate'
-    value: 'b * total_population / carrying_capacity'
-  birth:
-    desc: 'birth rate (/day)'
-    value: 'b * 2'
-  carrying_capacity:
-    desc: 'carrying capacity of the environment'
-    value: 'initial_population_size * 1.5'
-
+  epsilon:
+    desc: 'tiny value to avoid divisions by zero'
+    value: '1e-9'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
@@ -289,22 +267,22 @@
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: default
+        age_group: random
     - infected:
         desc: 'infected individuals'
         health_state: I
-        age_group: default
+        age_group: random
     - newborn:
-        desc: 'newborn individuals assuming no vertical transmission'
-        health_state: S
+        desc: 'newly created individuals'
+        health_state: default
         age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
@@ -346,10 +324,8 @@
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
       - total_population
-      - perc_prevalence_A
-      - perc_prevalence_J
 ...
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_cumul_inc.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_aggreg.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -60,22 +60,20 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR_cumul_inc
+model_name: hybrid_SIR_aggreg
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  compartment-based SIR model. It records the cumulative incidence
-  (total number of individuals that got infectious over time).'
+  abstract: 'SIR model with individual actions and aggregation of variables.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -96,53 +94,71 @@
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
-
 # ORGANIZATION LEVELS USED IN THE SIMULATION
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
-  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
-  # In a compartment-based model, the individuals level is not simulated explicitly
+    aggregate_vars:
+      - name: population_affected_over_time
+        collect: nb_episodes
+        operator: 'sum'
+      - name: average_infection_duration
+        collect: duration_infected
+        operator: 'mean'
   individuals:
-    desc: 'level of individuals'
+    desc: 'level of the individuals'
+
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a Compartment-Based Model, processes take place at the population
-# level and are managed by groupings
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
   individuals:
-    - health_state
+    - health_state: infection
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+grouping:
+  population:
+    infection: [health_state]
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -161,20 +177,28 @@
     desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
+          on_enter:
+            - set_var: duration_infected
+              value: 0
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
           on_enter:
-            - record_change: cumulative_incidence
+            - set_var: nb_episodes
+              value: 1
+            - message: 'I have a bad feeling about this...'
+          on_stay:
+            - set_var: duration_infected
+              value: 'duration_infected + 1'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
     # Below, a list of transitions between states, with rate or
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
@@ -207,38 +231,58 @@
     desc: 'recovery rate (/day)'
     value: 0.1
   force_of_infection:
     desc: 'infection function'
     value: 'transmission_I * total_I / total_population'
     source: 'classical function assuming frequency dependence'
   percentage_prevalence:
-    desc: 'proportion of infected+infectious individuals (%)'
+    desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
 
+#   _____ _        _
+#  / ____| |      | |
+# | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
+#  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
+#  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
+# |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
+
+# STATEVARS describe variables from a level, which are introduced or
+# used in prototypes, actions, or aggregate variables. They are only
+# meant to ensure the simulation engine that they correspond to the
+# modeller's purpose (not e.g. a forgotten parameter)
+
+statevars:
+  duration_infected:
+    desc: 'duration of an infectious episode'
+  nb_episodes:
+    desc: 'number of infectious episodes per individual'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
-
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
+        nb_episodes: 0
+        duration_infected: 0
     - infected:
         desc: 'infected individuals'
         health_state: I
+        nb_episodes: 0
+        duration_infected: 0
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
@@ -247,23 +291,24 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# Initial conditions describe the prototypes
+# In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
     - prototype: healthy
       amount: 'initial_population_size - initial_infected'
     - prototype: infected
       amount: 'initial_infected'
 
+
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
 #  \____/ \__,_|\__| .__/ \__,_|\__|___/
 #                  | |
@@ -276,10 +321,10 @@
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
-      - total_population
-      - cumulative_incidence
+      - population_affected_over_time
+      - average_infection_duration
 ...
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_demo.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_demo.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -60,20 +60,20 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: compart_SIR_demo
+model_name: hybrid_SIR_demo
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic, compartment-based SIR model with demography.'
+  abstract: 'This model is a simple discrete-time, stochastic, hybrid SIR model with demography.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -95,50 +95,63 @@
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
+# A hybrid model considers two levels: the population and
+# its components (individuals)
 levels:
-  # name of the level (arbitrary name)
   population:
     desc: 'level of the population'
-    aggregation_type: 'compartment'
+    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
-  # In a compartment-based model, the individuals level is not simulated explicitly
   individuals:
-    desc: 'level of individuals'
+    desc: 'level of the individuals'
+
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
+# In a hybrid model, processes take place at the population level
+# and are managed by groupings
 processes:
   individuals:
-    - health_state                 # name of a state machine
-
+    - health_state: infection                 # name of a grouping
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
 #                        |_|            |___/
 
-# not used here
+# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# DIRECTLY BASED ON STATE MACHINES
+# A grouping is based on one or more variables. For instance, the
+# grouping for managing the 'infection' process is based on the
+# variable 'health_state' (coming from the state machine with the same
+# name): hence, one group will be defined for all possible values of
+# the health_state variable.
+
+grouping:
+  population:
+    infection: [health_state]
+
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
@@ -147,16 +160,21 @@
 # Each state machine is composed at least of several states.
 # The name of a state machine defines an individual variable which
 # contains the value of the current state in the individual.
 # Transitions define how each change can change to another one.
 # Productions define how individuals in one state can produce
 # new individuals in another state.
 state_machines:
+  # Below, the definition of the state machine used by the process
+  # 'infection'
   health_state:
-    desc: 'The state machine which defines the evolution of health states'
+    desc: 'The state machine which defines the evolution of health
+    states
+    '
+    # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
       - I:
           name: 'Infectious'
@@ -169,27 +187,33 @@
       - D:
           name: 'Dead'
           desc: 'compartment to put dead individuals'
           fillcolor: white
           # the autoremove property specifies that this compartment is
           # automatically emptied
           autoremove: yes
+    # Below, a list of transitions between states, with rate or
+    # probabilities. Rates are automatically converted into
+    # probabilities w.r.t the duration of the time step (delta_t),
+    # assuming a classical exponential distribution of durations in
+    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
       # death (assuming no disease-induced mortality)
       - {from: S, to: D, rate: death}
       - {from: I, to: D, rate: death}
       - {from: R, to: D, rate: death}
     productions:
       # births (assuming no vertical transmission)
       - {from: S, to: S, rate: birth, prototype: newborn}
       - {from: I, to: S, rate: birth, prototype: newborn}
       - {from: R, to: S, rate: birth, prototype: newborn}
 
+
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
@@ -217,14 +241,15 @@
   birth:
     desc: 'the birth rate (/day)'
     value: 0.01
   death:
     desc: 'the death rate (/day)'
     value: 'birth'
 
+
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
```

### Comparing `emulsion-1.2rc5/models/features/compart_SIR_lockdown.yaml` & `emulsion-1.3b1/models/features/hybrid_gest.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -60,24 +60,23 @@
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
 # NAME OF THE MODEL
-model_name: hybrid_SIR
+model_name: hybrid_gest
 
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" SIR model, i.e. with individuals grouped according to
-  relevant variables such as their health state. A lockdown occurs
-  during epidemics to flatten the curve.
-  '
+  hybrid model with explicit gestation and age. Individuals are also
+  grouped automatically by parity, i.e. the number of successful
+  gestations.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -88,51 +87,53 @@
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
   time_unit: 'days'
   delta_t: 1
   origin: 'January 1'
-  total_duration: '300'
+  total_duration: '200'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
 # A hybrid model considers two levels: the population and
 # its components (individuals)
 levels:
-  population:
+  herd:
     desc: 'level of the population'
-    aggregation_type: 'compartment'   # the keyword for designing hybrid models
+    aggregation_type: 'hybrid'
     contains:
-      - individuals
-  individuals:
+      - animals
+  animals:
     desc: 'level of the individuals'
 
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
 # In a hybrid model, processes take place at the population level
-# and are managed by groupings
+# (here, herd) and are managed by groupings
 processes:
-  individuals:
-    - health_state
+  animals:
+    - age_group: age_and_sex
+    - sex: age_and_sex
+    - parity: parities
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -144,129 +145,202 @@
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 
-#grouping:
-#  population:
-#    infection: [health_state]
-
+grouping:
+  herd:
+    age_and_sex: [age_group, sex]
+    parities: [parity]
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
 
 # DESCRIPTION OF THE STATE MACHINES INVOLVED IN THE MODEL
-# Each state machine is composed at least of several states.
-# The name of a state machine defines an individual variable which
-# contains the value of the current state in the individual.
-# Transitions define how each change can change to another one.
-# Productions define how individuals in one state can produce
-# new individuals in another state.
 state_machines:
-  # Below, the definition of the state machine used by the process
-  # 'infection'
-  health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
-    # Below, the list of states with their attributes.
+  sex:
+    desc: 'A state machine without transitions just for representing male/female animals'
+    states:
+      - Female:
+          name: 'Female'
+          desc: 'Female animals'
+          fillcolor: 'orange'
+          default: yes
+      - Male:
+          name: 'Male'
+          desc: 'Male animals'
+          fillcolor: 'deepskyblue'
+  parity:
+    desc: 'A state machine without transitions, just for representing
+    the succession of relevant parities (number of successive
+    farrowings). The order of states defines a predecessor/successor
+    order used by keyword next_state in prototype next_parity'
     states:
-      - S:
-          name: 'Susceptible'
-          desc: 'suceptible of becoming infected'
-          fillcolor: 'wheat'
-      - I:
-          name: 'Infectious'
-          desc: 'infected and able to transmit the disease'
-          fillcolor: 'maroon'
-      - R:
-          name: 'Resistant'
-          desc: 'healthy again and resistant to infection'
+      - P0:
+          name: 'Nulliparous'
+          desc: 'Nulliparous animal (no previous farrowing)'
+          fillcolor: 'orange'
+      - P1:
+          name: 'Parity 1'
+          desc: 'Animal with parity 1 (first farrowing)'
+          fillcolor: 'pink'
+      - P2:
+          name: 'Parity 2'
+          desc: 'Animal with parity 2'
+          fillcolor: 'red'
+      - P3:
+          name: 'Parity 3+'
+          desc: 'Animal with parity 3 and more'
+          fillcolor: 'purple'
+  age_group:
+    desc: 'The state machine which defines the evolution of age groups.'
+    states:
+      - J:
+          name: 'Juvenile'
+          desc: 'juvenile animals'
+          fillcolor: 'orange'
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
+      - A:
+          name: 'Non-gestating Adult'
+          desc: 'adult animals'
+          fillcolor: 'brown'
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
+      - G:
+          name: 'Gestating Adult'
+          desc: 'adult animals (producing new juveniles)'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
+          duration: dur_gestation
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
+      - D:
+          name: 'Dead'
+          desc: 'compartment to put dead animals'
+          fillcolor: white
+          autoremove: yes
     transitions:
-      - {from: S, to: I, rate: 'force_of_infection'}
-      - {from: I, to: R, rate: 'recovery'}
-
+      - from: J
+        to: A
+        cond: 'GreaterThan(age, adult_age)'
+        proba: 1
+        desc: 'all Juveniles with age > adult_age move to Non-gestating Adults'
+      - from: A
+        to: D
+        rate: '1 / avg_adult_death_age'
+        desc: 'all Non-gestating Adults are subject to mortality due to old age'
+      - from: A
+        to: G
+        cond: 'is_Female'
+        rate: 'reproduction'
+        desc: 'non-gestating adult females start gestation at rate "reproduction"'
+      - from: G
+        to: A
+        proba: 1
+        on_cross:
+          - produce_offspring: 'newborn'
+            amount: 1
+          - become: 'next_parity'
+        desc: 'at end of gestation, gestating adult females return to A state and
+        produce offspring. Their parity is updated using the prototype next_parity
+        which increments the value of discrete variable parity'
+      - from: G
+        to: D
+        escape: yes
+        rate: '1 / avg_adult_death_age'
+        desc: 'all Gestating Adults are subject to mortality due to old age -
+        this can occur even during gestation, hence escape is set to yes'
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
-  initial_population_size:
-    desc: 'initial number of individuals in the population'
-    value: 1000
+  initial_herd_size:
+    desc: 'initial number of animals in the herd'
+    value: 100
   initial_infected:
-    desc: 'initial number of infectious individuals in the population'
-    value: 10
-  is_lockdown_active:
-    desc: '1 if currently under lockdown, 0 otherwise'
-    value: 'AND(time >= lockdown_start, time <= lockdown_start + lockdown_duration)'
-  transmission_I:
-    desc: 'transmission rate from infectious individuals (/day)'
-    value: 'IfThenElse(is_lockdown_active, transmission_I_lockdown, transmission_I_default)'
-    # value: 'IfThenElse(AND(total_I > 0.2 * total_population), transmission_I_lockdown, transmission_I_default)'
-  transmission_I_default:
-    desc: 'default transmission rate from infectious individuals (/day)'
-    value: 0.2
-  transmission_I_lockdown:
-    desc: 'transmission rate from infectious individuals during lockdown (/day)'
-    value: 0.02
-  lockdown_start:
-    desc: 'date where lockdown starts after the beginning of the simulation (days)'
-    value: 30
-  lockdown_duration:
-    desc: 'duration of the lockdown (days)'
-    value: 60
-  recovery:
-    desc: 'recovery rate (/day)'
-    value: '1/15'
-  force_of_infection:
-    desc: 'infection function'
-    value: 'transmission_I * total_I / total_population'
-    source: 'classical function assuming frequency dependence'
-  percentage_prevalence:
-    desc: 'proportion of infected+infectious individuals'
-    value: '100 * total_I / total_population'
+    desc: 'initial number of infectious animals in the herd'
+    value: 1
+  death:
+    desc: 'the death rate (/day)'
+    value: 0.01
+  dur_gestation:
+    desc: 'duration of gestation (days)'
+    value: 40
+  reproduction:
+    desc: 'reproduction rate (/days)'
+    value: '1/20'
+  avg_adult_death_age:
+    desc: 'mean longevity of adults (days)'
+    value: 120
+  adult_age:
+    desc: 'age when individuals become adults (days)'
+    value: 20
+  init_age_distrib:
+    desc: 'distribution of initial ages'
+    value: 'adult_age + random_integers(0, 100)'
+
+#   _____ _        _
+#  / ____| |      | |
+# | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
+#  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
+#  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
+# |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
+
+
+statevars:
+  age:
+    desc: 'age of the animal'
+
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
-  individuals:
-    - healthy:
-        desc: 'healthy individuals'
-        health_state: S
-    - infected:
-        desc: 'infected individuals'
-        health_state: I
+  animals:
+    - initial:
+        desc: 'initial animals'
+        age_group: A
+        age: init_age_distrib
+        sex: random
+        parity: random
+    - newborn:
+        desc: 'newly created animals'
+        age_group: J
+        sex: random
+        age: 0
+        parity: P0
+    - next_parity:
+        desc: 'increase the parity of a female at farrowing, based on
+        the order in which parities are defined in the corresponding
+        state machine'
+        parity: next_state
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -279,19 +353,17 @@
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
-  population:
-    - prototype: healthy
-      amount: 'initial_population_size - initial_infected'
-    - prototype: infected
-      amount: 'initial_infected'
+  herd:
+    - prototype: initial
+      amount: 'initial_herd_size'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -302,12 +374,14 @@
 # TYPE AND PERIODICITY OF OUTPUTS
 # The amount of individuals in each state is automatically recorded
 # for all state machines each time step during the simulation.
 # Additional variables (e.g. expressions defined in the 'parameters'
 # section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
-  population:
+  herd:
     period: 1
     extra_vars:
-      - is_lockdown_active
+      - total_herd
+      - total_G_Male
+      - total_G_Female
 ...
```

### Comparing `emulsion-1.2rc5/models/features/data/moves.csv` & `emulsion-1.3b1/models/features/data/moves.csv`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/data/pop_parameters.csv` & `emulsion-1.3b1/models/features/data/pop_parameters.csv`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/models/features/hybrid_ABC-old.yaml` & `emulsion-1.3b1/models/quickstart/quickstart.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -44,256 +44,418 @@
 # 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-#  __  __           _      _
-# |  \/  |         | |    | |
-# | \  / | ___   __| | ___| |
-# | |\/| |/ _ \ / _` |/ _ \ |
-# | |  | | (_) | (_| |  __/ |
-# |_|  |_|\___/ \__,_|\___|_|
-#
+#   _____                           _
+#  / ____|                         | |
+# | |  __  ___ _ __   ___ _ __ __ _| |
+# | | |_ |/ _ \ '_ \ / _ \ '__/ _` | |
+# | |__| |  __/ | | |  __/ | | (_| | |
+#  \_____|\___|_| |_|\___|_|  \__,_|_|
+
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
 
-# NAME OF THE MODEL
-model_name: hybrid_SIR
-
+# NAME OF THE DISEASE
+model_name: Quickstart
 
-# DESCRIPTION OF THE MODEL
 model_info:
-  abstract: 'This model is a simple discrete-time, stochastic,
-  "hybrid" SIR model, i.e. with individuals grouped according to
-  relevant variables such as their health state.
-  '
-  author: 'Sebastien Picault (sebastien.picault@inra.fr)'
-
+  abstract: 'This model is aimed at providing an overview of several EMULSION features.'
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
 #    | |  | | | | | | |  __/
 #    |_|  |_|_| |_| |_|\___|
 
+
 # TIME INFORMATION
-# This section defines the time unit (used e.g. for expressing
-# durations, rates, etc.), the duration of the time step, the origin
-# date and total duration of the simulation.
 time_info:
-  time_unit: 'days'
-  delta_t: 1
+  time_unit: days
+  delta_t: 7
   origin: 'January 1'
-  total_duration: '100'
-
+  total_duration: '2*365'
+  calendars:
+    quarantines:
+      period: {days: 365}
+      events:
+        quarantine_period: {begin: 'April 1', end: 'September 1'}
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
-# ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
-# its components (individuals)
+
+# LEVELS OF AGENTS
 levels:
+  individuals:
+    desc: 'level of individuals'
   population:
     desc: 'level of the population'
-    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
     contains:
       - individuals
-  individuals:
-    desc: 'level of the individuals'
+    aggregation_type: hybrid
+    aggregate_vars:
+      - name: nb_total_abortions
+        collect: nb_abortions
+        operator: 'sum'
+
 
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
-# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
-processes:
-  population:
-    - infection                 # name of a grouping
 
 
-#   _____                       _
-#  / ____|                     (_)
-# | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
-# | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
-# | |__| | | | (_) | |_| | |_) | | | | | (_| |
-#  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
-#                        | |             __/ |
-#                        |_|            |___/
-
-# DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
-# DIRECTLY BASED ON STATE MACHINES
-# A grouping is based on one or more variables. For instance, the
-# grouping for managing the 'infection' process is based on the
-# variable 'health_state' (coming from the state machine with the same
-# name): hence, one group will be defined for all possible values of
-# the health_state variable.
+# LIST OF PROCESSES (IN ORDER)
+processes:
+  individuals:
+    - age_group: aging
+    - life_cycle: aging
+    - health_state: infection
+
+
+#   _____
+#  / ____|
+# | |  __ _ __ ___  _   _ _ __  ___
+# | | |_ | '__/ _ \| | | | '_ \/ __|
+# | |__| | | | (_) | |_| | |_) \__ \
+#  \_____|_|  \___/ \__,_| .__/|___/
+#                        | |
+#                        |_|
 
+# DESCRIPTION OF COMPARTMENTS ASSOCIATED WITH PROCESSES WHICH ARE NOT
+# BASED ON METHODS:
 grouping:
   population:
-    infection:
-      machine_name: health_state
-      key_variables: [health_state]
-
+    infection: [health_state]
+    aging: [life_cycle, age_group]
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
 
 # DESCRIPTION OF THE STATE MACHINES INVOLVED IN THE MODEL
-# Each state machine is composed at least of several states.
-# The name of a state machine defines an individual variable which
-# contains the value of the current state in the individual.
-# Transitions define how each change can change to another one.
-# Productions define how individuals in one state can produce
-# new individuals in another state.
 state_machines:
-  # Below, the definition of the state machine used by the process
-  # 'infection'
+  age_group:
+    desc: 'Age groups in the population'
+    states:
+      - J:
+          name: 'Juvenile'
+          desc: 'juvenile animals'
+          fillcolor: 'orange'
+          default: yes
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
+      - A:
+          name: 'Adult'
+          desc: 'adult animals'
+          fillcolor: 'brown'
+          on_stay:
+            - set_var: age
+              value: 'age + delta_t'
+    transitions:
+      - {from: J, to: A, cond: 'GreaterThan(age, adult_age)', proba: 1}
+  life_cycle:
+    desc: 'Life cycle of animals regarding gestation'
+    states:
+      - G:
+          name: 'Gestating'
+          desc: 'state for gestating animals'
+          fillcolor: 'green'
+          duration: 'gestation_duration'
+      - NG:
+          name: 'NonGestating'
+          desc: 'state for empty animals'
+          fillcolor: 'cyan'
+          duration: 'delay_before_new_gestation'
+          default: yes
+    transitions:
+      - {from: NG, to: G, cond: is_A, rate: reproduction}
+      - desc: 'normal farrowing at end of gestation'
+        from: G
+        to: NG
+        amount-all-but: 0
+        on_cross:
+          - produce_offspring: [infected_newborn, protected_newborn]
+            amount: 1
+            proba:
+              - 'OR(is_E, is_I, is_Q)*proba_vertical_transmission'
+      - desc: 'abortion do tue infection'
+        from: G
+        to: NG
+        # abortions can occur only if animal is infectious
+        escape: is_I
+        proba: daily_abortion
+        on_cross:
+          - set_var: nb_abortions
+            value: 'nb_abortions + 1'
+
+
   health_state:
-    desc: 'The state machine which defines the evolution of health
-    states
-    '
-    # Below, the list of states with their attributes.
+    desc: 'Evolution of health states'
     states:
+      - M:
+          name: 'Maternal protection'
+          desc: 'animal protected by maternal antibodies'
+          fillcolor: 'cyan'
+          duration: 'adult_age'
       - S:
           name: 'Susceptible'
-          desc: 'suceptible of becoming infected'
+          desc: 'suceptible of becoming infectious'
+          default: yes
           fillcolor: 'wheat'
+      - E:
+          name: 'Exposed'
+          desc: 'already infected but not yet able to transmit the disease'
+          fillcolor: 'lightcoral'
+          duration: 'incubation_duration'
       - I:
           name: 'Infectious'
-          desc: 'infected and able to transmit the disease'
+          desc: 'sick and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
-    # Below, a list of transitions between states, with rate or
-    # probabilities. Rates are automatically converted into
-    # probabilities w.r.t the duration of the time step (delta_t),
-    # assuming a classical exponential distribution of durations in
-    # the states.
+      - Q:
+          name: 'Quarantine'
+          desc: 'sick animals that are put aside for a while'
+          fillcolor: 'green'
+          duration: 'quarantine_duration'
+      - D:
+          name: 'Dead'
+          desc: 'dead animals'
+          fillcolor: 'white'
+          autoremove: yes
     transitions:
-      - {from: S, to: I, proba: 0.9}
-      - {from: S, to: R, proba: 0.1}
-
+      - {from: M, to: S, rate: epsilon}
+      - {from: S, to: E, rate: f}
+      - {from: E, to: I, rate: alpha}
+      - {from: I, to: R, rate: gamma}
+      - {from: I, to: Q, rate: detection, when: 'quarantine_period'}
+      - {from: R, to: S, rate: delta}
+      - {from: Q, to: R, proba: 1}
+      - {from: M, to: D, rate: mortality_healthy, escape: yes}
+      - {from: S, to: D, rate: mortality_healthy}
+      - {from: R, to: D, rate: mortality_healthy}
+      - {from: E, to: D, rate: mortality_sick, escape: yes}
+      - {from: I, to: D, rate: mortality_sick}
+      - {from: Q, to: D, rate: mortality_sick, escape: yes}
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
-# PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
-    desc: 'initial number of individuals in the population'
+    desc: 'initial number of animals in the population'
     value: 100
   initial_infected:
-    desc: 'initial number of infectious individuals in the population'
-    value: 1
-  transmission_I:
-    desc: 'transmission rate from infectious individuals (/day)'
-    value: 0.5
-  recovery:
-    desc: 'recovery rate (/day)'
+    desc: 'initial number of infected animals in the population'
+    value: 10
+  adult_age:
+    desc: 'minimal age required to produce offspring (days)'
+    value: '365*2'
+  init_age_distrib:
+    desc: 'distribution of initial ages'
+    value: 'randint(0, adult_age)'
+  gestation_duration:
+    desc: 'duration of the gestation (in days)'
+    value: '30*8'
+  delay_before_new_gestation:
+    desc: 'minimum time to wait before new gestation can start'
+    value: '30*3'
+  reproduction:
+    desc: 'reproduction rate of the animals'
+    value: 0.05
+  mortality_healthy:
+    desc: 'mortality rate for healthy animals'
+    value: 0.002
+  mortality_sick:
+    desc: 'mortality rate for sick animals (E / I / Q)'
+    value: 0.004
+  proba_vertical_transmission:
+    desc: 'probability that the offspring of an infected animal (E/ I /Q) becomes Infectious'
+    value: 0.3
+  adult_age:
+    desc: 'age when individuals become adults (days)'
+    value: 30
+  epsilon:
+    desc: 'maternal antibodies loss rate'
+    value: 0.04
+  incubation_duration:
+    desc: 'minimum duration of the exposed state'
+    value: 10
+  alpha:
+    desc: 'rate for E->I transition'
+    value: 0.3
+  beta:
+    desc: 'contamination rate per sick individual'
     value: 0.1
-  force_of_infection:
-    desc: 'infection function'
-    value: 'transmission_I * total_I / total_population'
-    source: 'classical function assuming frequency dependence'
+  gamma:
+    desc: 'recovery rate'
+    value: 0.01
+  f:
+    desc: 'force of infection'
+    value: 'beta * total_I / total_population'
+  delta:
+    desc: 'resistance loss rate'
+    value: 0.01
+  quarantine_duration:
+    desc: 'duration of the quarantine (days)'
+    value: 30
+  quarantine_size:
+    desc: 'number of animals that can be put simultaneously in the quarantine area'
+    value: 20
+  detection:
+    desc: 'rate at which animals are detected sick (falls to 0 if
+    quarantine zone is full)
+    '
+    value: '0.01*room_in_quarantine'
+  room_in_quarantine:
+    desc: '1 if number of animals in quarantine < quarantine_size, 0
+    otherwise
+    '
+    value: 'StrictLessThan(total_Q, quarantine_size)'
   percentage_prevalence:
-    desc: 'proportion of infected+infectious individuals'
-    value: '100 * total_I / total_population'
+    desc: '% of animals infected (E+I+Q)'
+    value: '100 * (total_E + total_I + total_Q) / total_population'
+  view_quarantine:
+    desc: 'show quarantine period (*100 for visualization)'
+    value: '100 * quarantine_period'
+  global_abortion:
+    desc: 'probability that an infected animal aborts during
+    gestation
+    '
+    value: 0.2
+  daily_abortion:
+    desc: 'daily probability that an infected animal aborts during
+    gestation
+    '
+    value: '1 - (1 - global_abortion)**(1/gestation_duration)'
+#   _____ _        _
+#  / ____| |      | |
+# | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
+#  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
+#  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
+# |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
+
+
+statevars:
+  age:
+    desc: 'age of the animal'
+  nb_abortions:
+    desc: 'number of abortions experienced by the animal'
+
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
-# PROTOTYPES describe typical individuals, characterized by specific
-# values of their variables
 prototypes:
   individuals:
-    - healthy:
-        desc: 'healthy individuals'
+    - protected_newborn:
+        health_state: M
+        life_cycle: NG
+        age_group: J
+        age: 0
+        nb_abortions: 0
+    - infected_newborn:
+        health_state: I
+        life_cycle: NG
+        age_group: J
+        age: 0
+        nb_abortions: 0
+    - default_healthy:
         health_state: S
-    - infected:
-        desc: 'infected individuals'
+        life_cycle: NG
+        age: init_age_distrib
+        age_group: J
+        nb_abortions: 0
+    - default_infected:
         health_state: I
-
+        life_cycle: NG
+        age: init_age_distrib
+        age_group: J
+        nb_abortions: 0
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
 # |_____|_| |_|_|\__|_|\__,_|_|
 
-#   _____                _ _ _   _
-#  / ____|              | (_) | (_)
-# | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
-# | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
-# | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
-#  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
-
-# INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
-# involved with the amount of individuals in each of those prototypes
+#                      _ _ _   _
+#                     | (_) | (_)
+#   ___ ___  _ __   __| |_| |_ _  ___  _ __  ___
+#  / __/ _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
+# | (_| (_) | | | | (_| | | |_| | (_) | | | \__ \
+#  \___\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
+
 initial_conditions:
   population:
-    - prototype: healthy
+    - prototype: default_healthy
       amount: 'initial_population_size - initial_infected'
-    - prototype: infected
+    - prototype: default_infected
       amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
 #  \____/ \__,_|\__| .__/ \__,_|\__|___/
 #                  | |
 #                  |_|
 
-# TYPE AND PERIODICITY OF OUTPUTS
-# The amount of individuals in each state is automatically recorded
-# for all state machines each time step during the simulation.
-# Additional variables (e.g. expressions defined in the 'parameters'
-# section) can be specified below (as 'extra_vars').
 outputs:
   type: csv
+  ## possible alternative: database
+  # database_information:
+  #   database: Quickstart
+  #   dialect: mysql
+  #   driver: mysqldb
+  #   server_name: localhost # 10.0.26.250
+  #   username: EMuLSion
+  #   password: 'EMuLSion'
+  #   # port: '' # 3306
   population:
     period: 1
     extra_vars:
-      - percentage_prevalence
       - total_population
+      - percentage_prevalence
+      - view_quarantine
+      - nb_total_abortions
 ...
```

### Comparing `emulsion-1.2rc5/models/features/hybrid_SIRS_periodic_risk.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_struct.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -58,23 +58,24 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
-
 # NAME OF THE MODEL
-model_name: hybrid_SIRS_periodic_risk
-
+model_name: hybrid_SIR_JA_struct
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  hybrid SIRS model exposed to periodic external risk.'
+  hybrid SIR model with demography and age structure, with
+  non-exponential durations in state J. Besides, a contact
+  structure is added to account for physical separation between
+  Juveniles and Adults.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -82,54 +83,55 @@
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: 'days'
+  time_unit: days
   delta_t: 1
   origin: 'January 1'
-  total_duration: '300'
+  total_duration: '200'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
-# its components (individuals)
+# An individual-based model (IBM) (or a hybrid model) considers both
+# the individual and the population levels:
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
+    aggregation_type: hybrid
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
 
 
-
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
+# In a Compartment-Based Model (or in a Hybrid model), processes take
+# place at the population level and are managed by groupings
 processes:
   individuals:
-    - health_state: infection                 # name of a grouping
+    - health_state: details
+    - age_group: details
+
 
 
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
@@ -140,18 +142,22 @@
 # DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
-
+# Groupings are required for defining processes in compartement-based
+# or hybrid models.
 grouping:
   population:
-    infection: [health_state]
+    # this grouping relies on two variables: the health state but also
+    # the age_group, since the value of variables is_A/is_J used in
+    # the force of infection is determined by the age group
+    details: [health_state, age_group]
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
@@ -171,14 +177,15 @@
     desc: 'The state machine which defines the evolution of health states'
     # Below, the list of states with their attributes.
     states:
       - S:
           name: 'Susceptible'
           desc: 'suceptible of becoming infected'
           fillcolor: 'wheat'
+          default: yes
       - I:
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
@@ -187,15 +194,38 @@
     # probabilities. Rates are automatically converted into
     # probabilities w.r.t the duration of the time step (delta_t),
     # assuming a classical exponential distribution of durations in
     # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
-      - {from: R, to: S, rate: 'waning'}
+  age_group:
+    desc: 'The state machine which defines the evolution of age groups'
+    states:
+      - J:
+          name: 'Juvenile'
+          desc: 'Young individuals'
+          fillcolor: 'orange'
+          default: yes
+          duration: '1/maturation'
+      - A:
+          name: 'Adult'
+          desc: 'Adult individuals'
+          fillcolor: 'brown'
+      - D:
+          name: 'Dead'
+          desc: 'compartment to represent deceased individuals'
+          fillcolor: 'white'
+          autoremove: yes
+    transitions:
+      - {from: J, to: A, proba: 1}
+      - {from: A, to: D, rate: 'mortality'}
+      - {from: J, to: D, rate: 'mortality', escape: yes}
+    productions:
+      - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
 # | |  | (_| | | | (_| | | | | | |  __/ ||  __/ |  \__ \
@@ -208,35 +238,62 @@
     value: 100
   initial_infected:
     desc: 'initial number of infectious individuals in the population'
     value: 1
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
+  transJJ:
+    desc: 'transmission rate within Juveniles age group (/day)'
+    value: 0.2
+  transAA:
+    desc: 'transmission rate within Adults age group (/day)'
+    value: 0.5
+  transJA:
+    desc: 'transmission rate from Juveniles to Adults (/day)'
+    value: 0.3
+  transAJ:
+    desc: 'transmission rate from Adults to Juveniles (/day)'
+    value: 0.05
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
-  waning:
-    desc: 'rate at which individuals lose immunity (/day)'
-    value: 0.01
-  external_risk_period:
-    desc: 'periodicity of the external risk (days)'
-    value: 100
-  external_risk:
-    desc: 'external risk of disease introduction with periodicity'
-    value: 'transmission_I * (1 + sin(time * 2 * pi / external_risk_period))'
-  normalized_external_risk:
-    desc: 'external risk normalized between 0 and 100% of its maximum value'
-    value: '100 * external_risk / (2 * transmission_I)'
   force_of_infection:
     desc: 'infection function'
-    value: ' (external_risk + transmission_I * total_I) / total_population'
+    value: 'is_J * force_of_infection_juveniles + is_A * force_of_infection_adults'
+  force_of_infection_juveniles:
+    desc: 'infection function experience by juveniles'
+    value: 'DIV(transJJ * total_I_J, total_J) + DIV(transAJ * total_I_A, total_A)'
+  force_of_infection_adults:
+    desc: 'infection function experience by adults'
+    value: 'DIV(transAA * total_I_A, total_A) + DIV(transJA * total_I_J, total_J)'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
+  perc_prevalence_A:
+    desc: 'proportion of infected+infectious adults'
+    value: 'DIV(100 * total_I_A, total_A)'
+  perc_prevalence_J:
+    desc: 'proportion of infected+infectious juveniles'
+    value: 'DIV(100 * total_I_J, total_J)'
+  maturation:
+    desc: 'rate at which juveniles become adults (/day)'
+    value: '1/20'
+  b:
+    desc: 'base mortality rate (/day)'
+    value: 0.05
+  mortality:
+    desc: 'density-dependent mortality rate'
+    value: 'b * total_population / carrying_capacity'
+  birth:
+    desc: 'birth rate (/day)'
+    value: 'b * 2'
+  carrying_capacity:
+    desc: 'carrying capacity of the environment'
+    value: 'initial_population_size * 1.5'
 
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
@@ -247,14 +304,23 @@
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
+        age_group: default
+    - infected:
+        desc: 'infected individuals'
+        health_state: I
+        age_group: default
+    - newborn:
+        desc: 'newborn individuals assuming no vertical transmission'
+        health_state: S
+        age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
 #  _| |_| | | | | |_| | (_| | |
@@ -269,15 +335,17 @@
 
 # INITIAL CONDITIONS FOR THE SIMULATION
 # In IBM or hybrid models, initial conditions describe the prototypes
 # involved with the amount of individuals in each of those prototypes
 initial_conditions:
   population:
     - prototype: healthy
-      amount: 'initial_population_size'
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
@@ -293,9 +361,10 @@
 outputs:
   type: csv
   population:
     period: 1
     extra_vars:
       - percentage_prevalence
       - total_population
-      - normalized_external_risk
+      - perc_prevalence_A
+      - perc_prevalence_J
 ...
```

### Comparing `emulsion-1.2rc5/models/features/hybrid_SIR_JA_demo_random.yaml` & `emulsion-1.3b1/doc/html/_static/models/features/hybrid_SIR_JA_metapop.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -58,25 +58,22 @@
 #  _____        __                           _   _
 # |_   _|      / _|                         | | (_)
 #   | |  _ __ | |_ ___  _ __ _ __ ___   __ _| |_ _  ___  _ __
 #   | | | '_ \|  _/ _ \| '__| '_ ` _ \ / _` | __| |/ _ \| '_ \
 #  _| |_| | | | || (_) | |  | | | | | | (_| | |_| | (_) | | | |
 # |_____|_| |_|_| \___/|_|  |_| |_| |_|\__,_|\__|_|\___/|_| |_|
 
-
 # NAME OF THE MODEL
-model_name: hybrid_SIR_JA_demo_random
-
+model_name: hybrid_SIR_JA_metapop
 
 # DESCRIPTION OF THE MODEL
 model_info:
   abstract: 'This model is a simple discrete-time, stochastic,
-  hybrid SIR model with explicit age groups and demography.
-  Initialization uses random multinomial sampling of prototypes
-  (between healthy and infectious) and of states (for age group).'
+  hybrid SIR model with demography and age structure, at the
+  metapopulation scale.'
   author: 'Sebastien Picault (sebastien.picault@inrae.fr)'
 
 
 #  _______ _
 # |__   __(_)
 #    | |   _ _ __ ___   ___
 #    | |  | | '_ ` _ \ / _ \
@@ -84,57 +81,67 @@
 #    |_|  |_|_| |_| |_|\___|
 
 # TIME INFORMATION
 # This section defines the time unit (used e.g. for expressing
 # durations, rates, etc.), the duration of the time step, the origin
 # date and total duration of the simulation.
 time_info:
-  time_unit: 'days'
+  time_unit: days
   delta_t: 1
-  origin: 'January 1'
+  origin: 'January 1, 2018'
   total_duration: '100'
 
 
 #  _                    _
 # | |                  | |
 # | |     _____   _____| |___
 # | |    / _ \ \ / / _ \ / __|
 # | |___|  __/\ V /  __/ \__ \
 # |______\___| \_/ \___|_|___/
 
 # ORGANIZATION LEVELS USED IN THE SIMULATION
-# A hybrid model considers two levels: the population and
-# its components (individuals)
+# Here we introduced a third level, aggregating populations within
+# a metapopulation
 levels:
   population:
     desc: 'level of the population'
-    aggregation_type: 'hybrid'   # the keyword for designing hybrid models
+    aggregation_type: hybrid
     contains:
       - individuals
   individuals:
     desc: 'level of the individuals'
-
+  metapop:
+    desc: 'level of the metapopulation'
+    contains:
+      - population
+    aggregation_type: metapopulation
+    aggregate_vars:
+      - name: metapop_total_population
+        collect: total_population
+        operator: sum
+      - name: metapop_total_I
+        collect: total_I
+        operator: sum
 
 
 #  _____
 # |  __ \
 # | |__) | __ ___   ___ ___  ___ ___  ___  ___
 # |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
 # | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
 # |_|   |_|  \___/ \___\___||___/___/\___||___/
 
 # LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
-# In a hybrid model, processes take place at the population level
-# and are managed by groupings
+# In a Compartment-Based Model (or in a Hybrid model), processes take
+# place at the population level and are managed by groupings
 processes:
   individuals:
     - health_state: infection
     - age_group: aging
 
-
 #   _____                       _
 #  / ____|                     (_)
 # | |  __ _ __ ___  _   _ _ __  _ _ __   __ _
 # | | |_ | '__/ _ \| | | | '_ \| | '_ \ / _` |
 # | |__| | | | (_) | |_| | |_) | | | | | (_| |
 #  \_____|_|  \___/ \__,_| .__/|_|_| |_|\__, |
 #                        | |             __/ |
@@ -143,21 +150,50 @@
 # DESCRIPTION OF GROUPINGS, ASSOCIATED WITH PROCESSES WHICH ARE NOT
 # DIRECTLY BASED ON STATE MACHINES
 # A grouping is based on one or more variables. For instance, the
 # grouping for managing the 'infection' process is based on the
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
-
+# Groupings are required for defining processes in compartement-based
+# or hybrid models.
 grouping:
   population:
+<<<<<<< HEAD:models/features/hybrid_SIR_JA_metapop.yaml
+    infection: [health_state]
+    aging: [age_group]
+
+=======
+    # infection:
+    #   machine_name: health_state
+    #   key_variables: [health_state]
+    # aging:
+    #   machine_name: age_group
+    #   key_variables: [age_group]
     infection: [health_state]
     aging: [age_group]
 
 
+#  _____
+# |  __ \
+# | |__) | __ ___   ___ ___  ___ ___  ___  ___
+# |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
+# | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
+# |_|   |_|  \___/ \___\___||___/___/\___||___/
+
+# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
+# In a Compartment-Based Model (or in a Hybrid model), processes take
+# place at the population level and are managed by groupings
+processes:
+  individuals:
+    - health_state: infection
+    - age_group: aging
+>>>>>>> organization_devel2:models/features/hybrid_SIR_metapop.yaml
+
+
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
 # |_____/ \__\__,_|\__\___| |_|  |_|\__,_|\___|_| |_|_|_| |_|\___||___/
 
@@ -184,41 +220,44 @@
           name: 'Infectious'
           desc: 'infected and able to transmit the disease'
           fillcolor: 'maroon'
       - R:
           name: 'Resistant'
           desc: 'healthy again and resistant to infection'
           fillcolor: 'deepskyblue'
+    # Below, a list of transitions between states, with rate or
+    # probabilities. Rates are automatically converted into
+    # probabilities w.r.t the duration of the time step (delta_t),
+    # assuming a classical exponential distribution of durations in
+    # the states.
     transitions:
       - {from: S, to: I, rate: 'force_of_infection'}
       - {from: I, to: R, rate: 'recovery'}
-
   age_group:
-    desc: 'The state machine which defines the evolution of age groups.'
+    desc: 'The state machine which defines the evolution of age groups'
     states:
       - J:
           name: 'Juvenile'
-          desc: 'juvenile individuals'
+          desc: 'Young individuals'
           fillcolor: 'orange'
+          default: yes
       - A:
           name: 'Adult'
-          desc: 'adult individuals (producing new juveniles)'
+          desc: 'Adult individuals'
           fillcolor: 'brown'
       - D:
           name: 'Dead'
-          desc: 'compartment to put dead individuals'
-          fillcolor: white
+          desc: 'compartment to represent deceased individuals'
+          fillcolor: 'white'
           autoremove: yes
     transitions:
       - {from: J, to: A, rate: 'maturation'}
-      # death (assuming no disease-induced mortality)
-      - {from: J, to: D, rate: 'death'}
-      - {from: A, to: D, rate: 'death'}
+      - {from: A, to: D, rate: 'mortality'}
+      - {from: J, to: D, rate: 'mortality'}
     productions:
-      # births (assuming no vertical transmission)
       - {from: A, to: J, rate: 'birth', prototype: 'newborn'}
 
 
 #  _____                               _
 # |  __ \                             | |
 # | |__) |_ _ _ __ __ _ _ __ ___   ___| |_ ___ _ __ ___
 # |  ___/ _` | '__/ _` | '_ ` _ \ / _ \ __/ _ \ '__/ __|
@@ -226,67 +265,99 @@
 # |_|   \__,_|_|  \__,_|_| |_| |_|\___|\__\___|_|  |___/
 
 # PARAMETERS/FUNCTIONS/EXPRESSIONS USED IN THE MODEL
 parameters:
   initial_population_size:
     desc: 'initial number of individuals in the population'
     value: 100
-  initial_proba_infection:
-    desc: 'probability that an individual of the population is infectious at t=0'
-    value: 0.1
+  initial_infected:
+    desc: 'initial number of infectious individuals in the population'
+    value: 'initial_population_size * initial_prevalence'
   transmission_I:
     desc: 'transmission rate from infectious individuals (/day)'
     value: 0.5
   recovery:
     desc: 'recovery rate (/day)'
     value: 0.1
-  force_of_infection:
-    desc: 'infection function'
+  transmission_between_populations:
+    desc: 'transmission rate from other infectious individuals situated in other populations of the metapopulation (/day)'
+    value: 0.01
+  force_of_infection_between:
+    desc: 'infection function resulting from possible contacts with other population'
+    value: 'transmission_between_populations * DIV(metapop_total_I - total_I, metapop_total_population - total_population)'
+  force_of_infection_within:
+    desc: 'force of infection within the population'
     value: 'transmission_I * total_I / total_population'
-    source: 'classical function assuming frequency dependence'
+  force_of_infection:
+    desc: 'total force of infection'
+    value: 'force_of_infection_within + force_of_infection_between'
   percentage_prevalence:
     desc: 'proportion of infected+infectious individuals'
     value: '100 * total_I / total_population'
-  birth:
-    desc: 'the birth rate (/day)'
-    value: 0.01
-  death:
-    desc: 'the death rate (/day)'
-    value: 'birth'
   maturation:
     desc: 'rate at which juveniles become adults (/day)'
     value: '1/20'
-  init_prop_juveniles:
-    desc: 'average proportion of juveniles in the initial population'
-    value: 0.75
+  b:
+    desc: 'base mortality rate (/day)'
+    value: 0.05
+  mortality:
+    desc: 'density-dependent mortality rate'
+    value: 'b * total_population / carrying_capacity'
+  birth:
+    desc: 'birth rate (/day)'
+    value: 'b * 2'
+  carrying_capacity:
+    desc: 'carrying capacity of the environment'
+    value: 150
+  nb_populations:
+    desc: 'number of populations in metapopulation'
+    value: 4
+
+#   _____ _        _
+#  / ____| |      | |
+# | (___ | |_ __ _| |_ _____   ____ _ _ __ ___
+#  \___ \| __/ _` | __/ _ \ \ / / _` | '__/ __|
+#  ____) | || (_| | ||  __/\ V / (_| | |  \__ \
+# |_____/ \__\__,_|\__\___| \_/ \__,_|_|  |___/
+
+statevars:
+  initial_prevalence:
+    desc: 'Initial prevalence in the population'
 
 #  _____           _        _
 # |  __ \         | |      | |
 # | |__) | __ ___ | |_ ___ | |_ _   _ _ __   ___  ___
 # |  ___/ '__/ _ \| __/ _ \| __| | | | '_ \ / _ \/ __|
 # | |   | | | (_) | || (_) | |_| |_| | |_) |  __/\__ \
 # |_|   |_|  \___/ \__\___/ \__|\__, | .__/ \___||___/
 #                                __/ | |
 #                               |___/|_|
 
 # PROTOTYPES describe typical individuals, characterized by specific
 # values of their variables
 prototypes:
+  population:
+    - healthy_population:
+        desc: 'population initially without infected individuals'
+        initial_prevalence: 0
+    - infected_population:
+        desc: 'population initially infected individuals'
+        initial_prevalence: 0.1
   individuals:
     - healthy:
         desc: 'healthy individuals'
         health_state: S
-        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
+        age_group: default
     - infected:
         desc: 'infected individuals'
         health_state: I
-        age_group: 'random(init_prop_juveniles, 1-init_prop_juveniles)'
+        age_group: default
     - newborn:
-        desc: 'newly created individuals'
-        health_state: default
+        desc: 'newborn individuals assuming no vertical transmission'
+        health_state: S
         age_group: J
 
 
 #  _____       _ _   _       _
 # |_   _|     (_) | (_)     | |
 #   | |  _ __  _| |_ _  __ _| |
 #   | | | '_ \| | __| |/ _` | |
@@ -297,26 +368,29 @@
 #  / ____|              | (_) | (_)
 # | |     ___  _ __   __| |_| |_ _  ___  _ __  ___
 # | |    / _ \| '_ \ / _` | | __| |/ _ \| '_ \/ __|
 # | |___| (_) | | | | (_| | | |_| | (_) | | | \__ \
 #  \_____\___/|_| |_|\__,_|_|\__|_|\___/|_| |_|___/
 
 # INITIAL CONDITIONS FOR THE SIMULATION
-# In IBM or hybrid models, initial conditions describe the prototypes
-# involved with the amount of individuals in each of those prototypes
+
+# In IBM, hybrid models or metapops, initial conditions describe the
+# prototypes involved with the amount of individuals in each of those
+# prototypes
 initial_conditions:
   population:
-    - prototype: [infected, healthy]
-      # two possible prototypes for individual initially in the population
-      amount: initial_population_size
-      # drawn among a population of size initial_population_size
-      proba: [initial_proba_infection, 1-initial_proba_infection]
-      # with respective probabilities initial_proba_infection and
-      # 1-initial_proba_infection
-
+    - prototype: healthy
+      amount: 'initial_population_size - initial_infected'
+    - prototype: infected
+      amount: 'initial_infected'
+  metapop:
+    - prototype: infected_population
+      amount: 1
+    - prototype: healthy_population
+      amount: 'nb_populations - 1'
 
 
 #   ____        _               _
 #  / __ \      | |             | |
 # | |  | |_   _| |_ _ __  _   _| |_ ___
 # | |  | | | | | __| '_ \| | | | __/ __|
 # | |__| | |_| | |_| |_) | |_| | |_\__ \
```

### Comparing `emulsion-1.2rc5/models/features/hybrid_SIR_JA_metapop.yaml` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_metapop.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -154,17 +154,44 @@
 # variable 'health_state' (coming from the state machine with the same
 # name): hence, one group will be defined for all possible values of
 # the health_state variable.
 # Groupings are required for defining processes in compartement-based
 # or hybrid models.
 grouping:
   population:
+<<<<<<< HEAD:models/features/hybrid_SIR_JA_metapop.yaml
     infection: [health_state]
     aging: [age_group]
 
+=======
+    # infection:
+    #   machine_name: health_state
+    #   key_variables: [health_state]
+    # aging:
+    #   machine_name: age_group
+    #   key_variables: [age_group]
+    infection: [health_state]
+    aging: [age_group]
+
+
+#  _____
+# |  __ \
+# | |__) | __ ___   ___ ___  ___ ___  ___  ___
+# |  ___/ '__/ _ \ / __/ _ \/ __/ __|/ _ \/ __|
+# | |   | | | (_) | (_|  __/\__ \__ \  __/\__ \
+# |_|   |_|  \___/ \___\___||___/___/\___||___/
+
+# LIST OF PROCESSES (IN ORDER) TO BE EXECUTED DURING EACH TIME STEP
+# In a Compartment-Based Model (or in a Hybrid model), processes take
+# place at the population level and are managed by groupings
+processes:
+  individuals:
+    - health_state: infection
+    - age_group: aging
+>>>>>>> organization_devel2:models/features/hybrid_SIR_metapop.yaml
 
 
 #   _____ _        _         __  __            _     _
 #  / ____| |      | |       |  \/  |          | |   (_)
 # | (___ | |_ __ _| |_ ___  | \  / | __ _  ___| |__  _ _ __   ___  ___
 #  \___ \| __/ _` | __/ _ \ | |\/| |/ _` |/ __| '_ \| | '_ \ / _ \/ __|
 #  ____) | || (_| | ||  __/ | |  | | (_| | (__| | | | | | | |  __/\__ \
```

### Comparing `emulsion-1.2rc5/models/features/hybrid_SIR_JA_metapop_data.py` & `emulsion-1.3b1/models/features/hybrid_SIR_JA_metapop_data.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/setup.py` & `emulsion-1.3b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Configuration file for distributing the Emulsion package.
 """
 
 # [HEADER]
 
 from   setuptools import setup, find_packages
 
-VERSION = '1.2rc5'
+VERSION = '1.3beta1'
 LICENSE = 'Apache-2.0'
 
 if LICENSE.startswith('Apache'):
     LONG_LICENSE = 'License :: OSI Approved :: Apache Software License'
 elif 'BSD' in LICENSE:
     LONG_LICENSE = 'License :: OSI Approved :: BSD License'
 else:
@@ -31,14 +31,15 @@
 
 Models can use classical modelling paradigms (compartments,
 individual-based models, metapopulations) and multiple scales (from
 individuals to metapopulations), thanks to recent research in
 Artificial Intelligence.
 """
 
+
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
     #
@@ -66,15 +67,15 @@
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     url='https://sourcesup.renater.fr/emulsion-public/',
     download_url='https://pypi.org/project/emulsion/',
     # url='https://github.com/pypa/emulsion',  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
-    author='Sébastien Picault, Yu-Lin Huang, Vianney Sicard and Pauline Ezanno',  # Optional
+    author='Sebastien Picault, Yu-Lin Huang, Vianney Sicard and Pauline Ezanno',  # Optional
     # This should be a valid email address corresponding to the author listed
     # above.
     author_email='sebastien.picault@inrae.fr',  # Optional
     maintainer='Sébastien Picault',
     maintainer_email='sebastien.picault@inrae.fr',  # Optional
     # Classifiers help users find your project by categorizing it.
     #
@@ -97,15 +98,15 @@
         'Topic :: Education',
         # Pick your license as you wish
         LONG_LICENSE,
         # 'License :: The 3-Clause BSD License (BSD-3-Clause)',
         'Natural Language :: English',
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Unix Shell',
         # Specify the Operating Systems supported by your package
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Unix', # not tested in general - report bugs
         'Operating System :: Microsoft :: Windows :: Windows 10', # not tested in general - report bugs,
         # Specify the environment
@@ -183,58 +184,58 @@
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
-        'numpy>=1.23',             # BSD
-        'scipy>=1.9',              # BSD
-        'matplotlib>=3.5',         # Python Software Foundation ## only used in emulsion.tools.views which is not used anywhere now
-        'sympy>=1.11',            # BSD
-        'mpmath>=1.2',             # BSD
-        'pandas>=1.4',            # Simplified BSD
-        'pydot>=1.4',           # MIT
-        'sqlalchemy>=1.4',      # MIT
-        'sortedcontainers>=2.4', # Apache
+        'numpy>=1.18',             # BSD
+        'scipy>=1.1',              # BSD
+        'matplotlib>=2.2',         # Python Software Foundation
+        'sympy==1.1.1',            # BSD
+        'mpmath>=1.1',             # BSD
+        'pandas>=0.23',            # Simplified BSD
+        'sqlalchemy>=1.1.13',      # MIT
+        'sortedcontainers>=1.5.7', # Apache
         'tqdm>=4.23',              # MIT
         'pyyaml>=3.12',            # MIT
         'docopt>=0.6.2',           # MIT
-        'jinja2>=3.1',            # BSD  ## only used to generate .py file templates, soon obsolete
-        'python-dateutil>=2.8',    # BSD
-        # 'utm>=0.7',                # MIT ## no more in use (was used in Qfever model)
-        'bokeh>=2.4',             # BSD 3-Clause
-        'networkx>=2.8',           # BSD
+        'jinja2>=2.10',            # BSD
+        'python-dateutil>=2.7',    # BSD
+        'textx>=1.8',              # MIT
+        'utm>=0.4',                # MIT
+        'bokeh<=3.0',             # BSD 3-Clause
+        'docopt>=0.6',             # MIT
+        'networkx>=2.2',           # BSD
+        'graphviz>=0.8',           # BSD
         'colorama>=0.4',           # BSD
         # 'ggplot',                  # BSD 2-Clause "Simplified" License
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.6',
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
     # projects.
     extras_require={  # Optional
         'doc': [
             # 'doxypypy',              # GPL2
-            'sphinx>=5.1',             # BSD
+            'sphinx>=1.8',             # BSD
             'alabaster',               # BSD
         ],
         'dev': [
-            'setuptools>=63.4',        # MIT
-            'wheel>=0.37',                   # MIT
-            'twine>=4.0',                   # Apache-2.0
-            'pyinstaller>=5',           # GPL2 / Apache-2.0
-            'semantic_version>=2.10',
-            'pylint>=2.14',           # GPL
-            'cython>=0.29',            # Apache
-            'jupyter>=1.0',                 # Modified (3-clause) BSD
+            'setuptools>=38.5',        # MIT
+            'wheel',                   # MIT
+            'twine',                   # Apache-2.0
+            'pylint>=1.8.2',           # GPL
+            'cython>=0.28',            # Apache
+            'jupyter',                 # Modified (3-clause) BSD
             # 'graphviz-python>=2.32', # Eclipse Public License
         ],
     },
 
     include_package_data=True,
 
     # To provide executable scripts, use entry points in preference to the
@@ -243,15 +244,15 @@
     # platform.
     #
     # For example, the following would provide a command called `emulsion` which
     # executes the function `main` from this package when invoked:
     entry_points={  # Optional
         'console_scripts': [
             'emulsion = emulsion.__main__:main',
-            # 'init_emulsion = emulsion.init_emulsion:main',
+            'init_emulsion = emulsion.init_emulsion:main',
         ],
     },
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
@@ -264,10 +265,10 @@
     #     'Funding': 'https://donate.pypi.org',
     #     'Say Thanks!': 'http://saythanks.io/to/example',
     #     'Source': 'https://github.com/pypa/sampleproject/',
     # },
     project_urls={
         # "Bug Tracker": "https://bugs.example.com/HelloWorld/",
         "Documentation": "https://sourcesup.renater.fr/emulsion-public/",
-        "Source Code": "https://forgemia.inra.fr/dynamo/software/emulsion-public",
+        "Source Code": "https://git.renater.fr/emulsion-public.git",
     }
 )
```

### Comparing `emulsion-1.2rc5/src/emulsion/__init__.py` & `emulsion-1.3b1/src/emulsion/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,9 +49,9 @@
 # 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-__version__ = '1.2rc5'
-__all__ = ['tools', 'agent', 'model', 'templates']
+__version__ = '1.3beta1'
+__all__ = ['tools', 'agent', 'model', 'templates', 'organization']
```

### Comparing `emulsion-1.2rc5/src/emulsion/__main__.py` & `emulsion-1.3b1/src/emulsion/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 """Usage:
     emulsion run [--plot] MODEL [options] [(-p KEY=VALUE)...]
-    emulsion diagrams MODEL [options]
     emulsion show MODEL [options] [(-p KEY=VALUE)...]
     emulsion describe MODEL PARAM...
+    emulsion diagrams MODEL [options]
     emulsion plot MODEL [options]
+    emulsion check MODEL [options]
     emulsion generate MODEL
+    emulsion create-project PROJECT
+    emulsion compile MODEL
     emulsion (-h | --help | -V | --version | -L | --license)
 
 Commands:
   run MODEL                   Run simulations based on the specified MODEL
                               (MODEL is the path to the YAML file describing the
                               model to run).
-  diagrams MODEL              Produce model diagrams (as option --view-model
-                              when running/plotting) and open them
   show MODEL                  Print all MODEL parameter values and exit.
   describe MODEL PARAM...     Describe the role of specified PARAMeters in the
                               MODEL and exit.
+  diagrams MODEL              Produce model diagrams (as option --view-model
+                              when running/plotting) and open them
   plot MODEL                  Plot outputs for MODEL (assumed already run) and
                               exit.
+  check MODEL                 Check the syntactic correctness of the given MODEL
+                              (path to YAML file of the model to run), according
+                              to EMULSION meta-model. Option '--meta-tree'
+                              generates a figure representing EMULSION meta-
+                              model. If the model is correct, option
+                              '--model-tree' also generates a figure for the
+                              MODEL structure.
   generate MODEL              Generate a skeleton to help writing specific
                               pieces of code before the MODEL can be run, and
                               exit.
 
+  create-project NAME         Create Emulsion project with templates
+
+  compile                     Compile each YAML parts in a single YAML files
+                              (in the tmp-yaml folder of the project)
+
 Options:
   -h --help                   Display this page and exit.
   -V --version                Display version number and exit.
   -L --license                Display license and exit.
   --plot                      Plot outputs just after running the model.
   -r RUNS --runs RUNS         Specify the number of repetitions of the same
                               model [default: 10].
@@ -48,28 +63,23 @@
   --load FILE                 Use a saved simulation to start the current one.
   --output-dir OUTPUT         Specify a directory for simulation outputs
                               [default: outputs].
   --input-dir INPUT           Specify a directory for simulation inputs
                               [default: data].
   --figure-dir FIG            Specify a directory for graphic outputs (figures)
                               [default: img].
-  --code-path CODE            Specify a path for Python add-ons [default: .].
   --log-params                When producing CSV outputs, insert the name and
                               value of each parameter explicitly changed by
                               option -p/--param. (DEPRECATED)
-  --format FORMAT             Specify an image format for diagram outputs (svg,
-                              pdf, png, jpg) [default: svg].
+  --format FORMAT             Specify an image format for diagram outputs
+                              [default: svg].
   --table-params              Display a table of the parameters and initial
                               conditions.
-  --aggregate                 Together with --plot, force the aggregation of
-                              runs to display median, min-max and 10-90
-                              percentiles instead of the detail of each run.
-                              This is the default behaviour for 20 runs or more.
-  --detail                    Together with --plot, force the display of each
-                              run (default for less than 20 runs).
+
+  --debug                     Display debuginfo
 
 Advanced options:
   --seed SEED                 Set a seed value for random numbers. When not
                               specified, the seed is set according to system
                               time and the process id.
   --show-seed                 Print the seed used for random numbers.
   --start-id ID               ID of the first repetition of the same model
@@ -81,14 +91,19 @@
   --modifiable                Output the list of modifiable parameters and exit.
   --level LEVEL               Specify the LEVEL (scale) for running the model.
                               Valid values are those defined in the 'level'
                               section of the MODEL. The corresponding agent
                               class will be used to manage the simulation of
                               lower-level entities. When no value is given, the
                               highest level (if any) is used.
+  --model-tree                Output a figure or the syntactic tree that
+                              represents the model if it complies to EMULSION
+                              DSL syntax (requires Graphviz).
+  --meta-tree                 Output a figure of the meta-model associated with
+                              EMULSION DSL (requires Graphviz).
 
 
 EMULSION (Epidemiological Multi-Level Simulation framework)
 ===========================================================
 
 Contributors and contact:
 -------------------------
@@ -154,36 +169,55 @@
   # --metamodel META            Specify a metamodel for syntax checking
   #                             [default: ../../scripts/emulsion.tx]
 
 
 import sys
 import os
 import time
+import subprocess
 import datetime                     as dt
 import webbrowser
 
 from   pathlib                      import Path
 
+import yaml
 import numpy                        as np
 
 from   docopt                       import docopt
+from   textx                        import metamodel_from_file
+from   textx.export                 import metamodel_export, model_export
 import colorama
-import pydot
 
+import emulsion
 from   emulsion.model.emulsion_model import EmulsionModel
+# ORGANIZATION PART --------------------------
+from   emulsion.organization        import OrganizationModel
+# --------------------------------------------
 from   emulsion.tools.state         import StateVarDict
 from   emulsion.tools.misc          import load_class
 from   emulsion.tools.plot          import plot_outputs
+# ORGANIZATION PART --------------------------
+from   emulsion.organization.utils  import organization_plot
+# --------------------------------------------
 from   emulsion.tools.simulation    import MultiSimulation
+from   emulsion.tools.debug         import debuginfo
 
-VERSION = '1.2rc5'
+VERSION = '1.3beta1'
 DEFAULT_VERSION = "1.2"
 LICENSE = 'Apache-2.0'
 DEFAULT_LICENSE = "Apache-2.0"
 
+def get_metamodel():
+    """Return the path to the metamodel used for checking syntax of
+    EMULSION YAML files.
+
+    """
+    # retrieve path to EMULSION repository
+    parts = Path(emulsion.__file__).parts[:-1] + ("resources", "emulsion.tx")
+    return Path(*parts)
 
 def get_version():
     """Retrieve the version number of current program.
 
     """
     # try:
     #     proc = subprocess.Popen(["git", "describe",
@@ -226,27 +260,30 @@
             if val in d_params:
                 val = d_params[val]
             # retrieve the value with correct type
             d_params[key] = type(d_params[key])(val)
         elif key in d_modifiable:
             d_model_changes[key] = val
         else:
-            print(colorama.Fore.RED + colorama.Style.BRIGHT + 'Unknown parameter:{}'.format(key) + colorama.Style.RESET_ALL)
+            print(colorama.Fore.RED + colorama.Style.BRIGHT +\
+                  'Unknown parameter:{}'.format(key) + colorama.Style.RESET_ALL)
             sys.exit(-1)
     if any(d_model_changes):
-        d_params.model = EmulsionModel(filename=d_params.filename, input_dir=d_params.input_dir, changed_values=d_model_changes)
+        # d_params.model = EmulsionModel(filename=d_params.filename, input_dir=d_params.input_dir, changed_values=d_model_changes)
+        d_params.model = instanciate_EmulsionModel(filename=d_params.filename, input_dir=d_params.input_dir, changed_values=d_model_changes)
 
 def describe_parameters(params):
     """Display the role of all parameters specified in the PARAM argument
     and exit.
 
     """
     model = params.model
     print(colorama.Style.BRIGHT + '\n{!s: ^72}'.format(params.model))
-    print('{: ^72}'.format('ROLE OF PARAMETERS (AND CURRENT DEFINITION)') + colorama.Style.RESET_ALL)
+    print('{: ^72}'.format('ROLE OF PARAMETERS (AND CURRENT DEFINITION)') +\
+          colorama.Style.RESET_ALL)
     print('-'*72)
     for name in params.to_describe:
         print(model.describe_name(name))
     print('-'*72)
 
 
 def show_parameters(params, short=False):
@@ -292,15 +329,17 @@
         module = '.'.join(mod_path.parent.parts + (mod_path.stem,))
         if mod_path.exists():
             print(colorama.Fore.YELLOW, 'WARNING, file {} already exists, '.format(mod_path))
             mod_path = mod_path.with_suffix('.py.%s' %
                                             (dt.datetime.now().timestamp()))
             print('Writing in {} instead'.format(mod_path) + colorama.Style.RESET_ALL)
         mod_path.parent.mkdir(parents=True, exist_ok=True)
-        print(colorama.Fore.GREEN + colorama.Style.BRIGHT + 'GENERATING CODE SKELETON {}\nFOR MODULE {}'.format(mod_path, module) + colorama.Style.RESET_ALL)
+        print(colorama.Fore.GREEN + colorama.Style.BRIGHT +\
+              'GENERATING CODE SKELETON {}\nFOR MODULE {}'.format(mod_path, module) +\
+              colorama.Style.RESET_ALL)
         with open(mod_path, 'w') as f:
             print(model.generate_skeleton(module), file=f)
 
 
 def run_model(params):
     """Run the model with the specified local parameters.
 
@@ -310,14 +349,15 @@
 
     Returns:
         The instance of MultiSimulation class which carried out the simulations
 
     See also:
         `emulsion.tools.simulation.MultiSimulation`_
     """
+    params.model.organization_model.draw_graph(params.draw_graph)
     count_path = Path(params.output_dir, 'counts.csv')
     if count_path.exists():
         count_path.unlink()
     log_path = Path(params.output_dir, 'log.txt')
     if log_path.exists():
         log_path.unlink()
     multi_simu = MultiSimulation(**params)
@@ -345,38 +385,72 @@
     model = params.model
     model.write_dot(params.output_dir)
     prefix = model.model_name
     for name, _ in model.state_machines.items():
         inpath = Path(params.output_dir, prefix + '_' + name + '.dot')
         outpath = Path(params.figure_dir,
                        prefix + '_' + name + '_machine.' + params.img_format)
-
-        dot_graph = pydot.graph_from_dot_file(inpath)[0]
-        ## bug when reading file (node named "\n" added!)
-        for node in list(dot_graph.get_nodes()):
-            if str(node) == '"\\n";':
-                dot_graph.del_node(node)
-        if params.img_format == "svg":
-            method = dot_graph.write_svg
-        elif params.img_format == "pdf":
-            method = dot_graph.write_pdf
-        elif params.img_format == "png":
-            method = dot_graph.write_png
-        else:
-            method = dot_graph.write_jpg
-        method(outpath)
+        os.system("dot -T%s %s > %s" % (params.img_format, inpath, outpath))
         print(colorama.Fore.GREEN + 'Generated state machine diagram {}'.format(outpath) + colorama.Style.RESET_ALL)
         if view:
             webbrowser.open(outpath.absolute().as_uri())
 
+def check_model(params, filemodel, view_meta=False, view_model=False):
+    """Check the syntax of the model according to the grammar specified in
+    EMULSION metamodel (``src/emulsion/resources/emulsion.tx``). If
+    *show_meta* is True, produce a figure to represent the metamodel
+    in *figure_dir* (requires GraphViz). If the syntax is correct and
+    *show_model* is True, also produce a figure for the model
+    structure.
+
+    """
+    source_path = Path(filemodel)
+    metapath = get_metamodel()
+    if not metapath.exists():
+        print(colorama.Fore.RED + colorama.Style.BRIGHT +\
+              'ERROR, metamodel file not found: {}'.format(metapath) +\
+              colorama.Style.RESET_ALL)
+        sys.exit(-1)
+    meta = metamodel_from_file(metapath)
+    if view_meta:
+        meta_output = Path(params.figure_dir,
+                           'meta_' + metapath.name).with_suffix('.dot')
+        metamodel_export(meta, meta_output)
+        figname = str(meta_output.with_suffix('.' + params.img_format))
+        os.system("dot -T%s %s > %s" % (params.img_format,
+                                        meta_output, figname))
+        print(colorama.Fore.GREEN + 'Produced Metamodel figure: {}'.format(figname) +\
+              colorama.Style.RESET_ALL)
+
+    with open(source_path) as f:
+        content = f.read()
+
+    normalized = yaml.dump(yaml.load(content), default_flow_style=False)
+    with open('tmp.yaml', 'w') as f:
+        print(normalized, file=f)
+    model_check = meta.model_from_str(normalized)
+    if view_model:
+        model_path = Path(params.figure_dir,
+                          'model_%s' % (source_path.name, )).with_suffix('.dot')
+        model_export(model_check, model_path)
+        figname = str(model_path.with_suffix('.' + params.img_format))
+        os.system("dot -T%s %s > %s" % (params.img_format, model_path, figname))
+        print(colorama.Fore.GREEN + 'Produced Model figure {}'.format(figname) + colorama.Style.RESET_ALL)
+    Path('tmp.yaml').unlink()
+    print(colorama.Fore.GREEN + colorama.Style.BRIGHT +\
+          'File {} complies with Emulsion syntax'.format(filemodel)+\
+          colorama.Style.RESET_ALL)
+
+
 def not_implemented(_):
     """Default behavior for unimplemented features.
 
     """
-    print(colorama.Fore.RED + colorama.Style.BRIGHT + 'Feature not implemented in this model.' + colorama.Style.RESET_ALL)
+    print(colorama.Fore.RED + colorama.Style.BRIGHT +\
+          'Feature not implemented in this model.' + colorama.Style.RESET_ALL)
     sys.exit(0)
 
 def set_seed(params, seed=None, show=False):
     """Initialize the numpy's Random Number Generator, either with the
     specified seed, or with a seed calculated from current time and
     process ID.
 
@@ -391,28 +465,34 @@
 
 
 def init_main_level(params):
     """Initialize the upper simulation level, in charge of making all
     sub-levels work properly.
 
     """
+    # debuginfo(params.level)
     if params.level not in params.model.levels:
-        print(colorama.Fore.RED + colorama.Style.BRIGHT + 'ERROR, level {} not found'.format(params.level) + colorama.Style.RESET_ALL)
+        print(colorama.Fore.RED + colorama.Style.BRIGHT + \
+              'ERROR, level {} not found'.format(params.level) + colorama.Style.RESET_ALL)
         sys.exit(-1)
 
     module_name = params.model.levels[params.level]['module']
     class_name = params.model.levels[params.level]['class_name']
     try:
         params.target_agent_class = load_class(module_name,
                                                class_name=class_name)[0]
     except AttributeError:
-        print(colorama.Fore.RED + colorama.Style.BRIGHT + 'ERROR, agent class not found for level {}: {}.{}'.format(params.level, module_name, class_name) + colorama.Style.RESET_ALL)
+        print(colorama.Fore.RED + colorama.Style.BRIGHT + \
+              'ERROR, agent class not found for level {}: {}.{}'.format(
+                  params.level, module_name, class_name) + colorama.Style.RESET_ALL)
         sys.exit(-1)
     except ModuleNotFoundError:
-        print(colorama.Fore.RED + colorama.Style.BRIGHT +  'ERROR, module not found for level {}: {}'.format(params.level, module_name) + colorama.Style.RESET_ALL)
+        print(colorama.Fore.RED + colorama.Style.BRIGHT + \
+              'ERROR, module not found for level {}: {}'.format(params.level, module_name) +\
+              colorama.Style.RESET_ALL)
         sys.exit(-1)
 
 
 def table_param(params):
     """Display a table of parameters and initial conditions.
 
     """
@@ -428,14 +508,67 @@
     initials = params.model._description['initial_conditions']
     strOutput = '\n\nINITIAL CONDITIONS\n__________________\n\n'
     strOutput += '|   name                 |    value\n'
     strOutput += '-' * 200 + '\n'
     strOutput += create_initial(initials)
     print(strOutput)
 
+##############################
+def create_project(params):
+    """
+    Create Emulsion project
+    """
+    print("-------------------------")
+    print(" CREATE EMULSION PROJECT ")
+    print("-------------------------\n")
+    time_unit = input("Enter time_unit [hours|days|weeks]: ")
+    delta_t = input("Enter delta_t (integer): ")
+    total_duration = input("Enter total_duration: ")
+    print("\n-------------------------\n")
+    # create folder for the project
+    if not os.path.isdir(params):
+        os.mkdir(params)
+    else:
+        print("ERROR")
+        print("folder", params, "already exists")
+        return
+    current_path = os.path.dirname(os.path.abspath(__file__))
+    template_path = os.path.join(current_path,"templates")
+    yaml_template_path = os.path.join(template_path,"YAML_templates")
+    main_template_path = os.path.join(template_path,"main_template")
+    from distutils.dir_util import copy_tree
+    yaml_part_path = os.path.join(params,"YAML_parts")
+    os.mkdir(yaml_part_path)
+    copy_tree(yaml_template_path, yaml_part_path)
+    copy_tree(main_template_path, params)
+    os.rename(os.path.join(params,"main.emul"), os.path.join(params,params+".emul"))
+    os.mkdir(os.path.join(params,"tmp_yaml"))
+    head_file_path = os.path.join(yaml_part_path,"head.yaml")
+    f = open(head_file_path,"r")
+    data = ""
+    for line in f:
+        line = line.replace('<time_unit>', time_unit)
+        line = line.replace('<delta_t>', delta_t)
+        line = line.replace('<total_duration>', total_duration)
+        line = line.replace('<name>', params)
+        data += line
+    f.close()
+    f = open(head_file_path, "w")
+    f.write(data)
+    f.close()
+    print("Ready to use !")
+
+def debug():
+    from emulsion.tools.DebugGlobal import DebugGlobal
+    debugglobal = DebugGlobal()
+    debugglobal.debug = True
+
+
+##############################
+
 def create_desc(parameters, p):
     name = p
     result = '| ' + name + ' '*(23 - len(name)) + '| '
 
     val = str(parameters[p]['value'])
     result += val + ' '*(50 - len(val)) + '| '
 
@@ -452,45 +585,100 @@
         for elem in desc:
             for e in elem:
                 result += '  ' + e + ' '*(23 - len(e))
                 result += '| ' + str(elem[e]) + '\n'
             result += '\n'
     return result
 
+globArgs = None
+def instanciate_EmulsionModel(filename=None, description=None, input_dir=None, changed_values=None):
+    model = EmulsionModel(filename=filename, input_dir=input_dir, changed_values=changed_values)
+
+# ORGANIZATION PART -------------------------
+    global globArgs
+    organization_model = OrganizationModel()
+    organization_model.setModel(model)
+    organization_model.set_nb_simu(int(globArgs['--runs']))
+    model.organization_model = organization_model
+    model.run_parse(changed_values=changed_values)
+# -------------------------------------------
+    return model
+
+def compile_yaml(model):
+    """Compile each YAML parts in a signe YAML file into the tmp-yaml folder of the project"""
+    debuginfo("FILE COMPILED :", model['filename'])
 
 def main(args=None):
     """Run EMuLSion's main program according to the command-line
     arguments.
 
     """
     colorama.init()
     if args is None:
         args = docopt(__doc__, version=get_version())
 
     if args['--license']:
         print(colorama.Fore.CYAN + get_license() + colorama.Style.RESET_ALL)
         sys.exit(0)
 
+######################
+    if args["create-project"]:
+        create_project(args['PROJECT'])
+        return
+
+    if '.yaml' not in args['MODEL']:
+        if os.path.isfile("./tmp_yaml/"+args['MODEL']+".yaml"):
+            os.remove("./tmp_yaml/"+args['MODEL']+".yaml")
+        main_file = open(args['MODEL'],'r')
+        # import subprocess
+        new = open("tmp_yaml/"+args["MODEL"]+".yaml", "w+")
+        main_yaml = ""
+        for line in main_file:
+            if not line.startswith('#') and line != "\n":
+                line = line.replace("\n", "")
+                current = open("YAML_parts/"+line)
+                for yaml_line in current:
+                    if "#" not in yaml_line:
+                        main_yaml += yaml_line
+                current.close()
+            # else:
+            #     debuginfo(line)
+        new.write(main_yaml)
+        new.close()
+        main_file.close()
+        args['MODEL'] = 'tmp_yaml/'+args['MODEL']+".yaml"
+        print(args["MODEL"])
+
+#########################
+
     if not Path(args['MODEL']).exists():
-        print(colorama.Fore.RED + colorama.Style.BRIGHT + 'ERROR: file {} not found'.format(args['MODEL']) + colorama.Style.RESET_ALL)
+        print(colorama.Fore.RED + colorama.Style.BRIGHT +\
+              'ERROR: file {} not found'.format(args['MODEL']) + colorama.Style.RESET_ALL)
         sys.exit(-1)
 
+    global globArgs
+    globArgs = args
     params = StateVarDict()
     params.filename = args['MODEL']
     params.input_dir = Path(args['--input-dir'])
-    params.model = EmulsionModel(filename=params.filename, input_dir=params.input_dir)
+
+    params.model = instanciate_EmulsionModel(filename=params.filename, input_dir=params.input_dir)
+#     params.model = EmulsionModel(filename=params.filename, input_dir=params.input_dir)
+
+# # ORGANIZATION PART -------------------------
+#     organization_model = OrganizationModel()
+#     organization_model.setModel(params.model)
+#     organization_model.set_nb_simu(int(args['--runs']))
+#     params.model.organization_model = organization_model
+#     params.model.run_parse()
+# # -------------------------------------------
     params.nb_simu = int(args['--runs'])
     params.stochastic = not args['--deterministic']
     params.to_describe = args['PARAM']
 
-    params.img_format = args['--format']
-    if params.img_format not in ['pdf', 'png', 'svg', 'jpg']:
-        print(colorama.Fore.RED + colorama.Style.BRIGHT + f'Invalid diagram format: {params.img_format}' + colorama.Style.RESET_ALL)
-        sys.exit(-1)
-
     params.save_to_file = args['--save']
     params.load_from_file = args['--load']
 
     params.level = args['--level']
     if params.level is None:
         params.level = params.model.root_level
     if not args['--modifiable']:
@@ -498,19 +686,15 @@
 
     params.silent = args['--silent']
     params.quiet = args['--quiet']
     params.nocount = args['--no-count']
     params.start_id = int(args['--start-id'])
     params.output_dir = Path(args['--output-dir'])
     params.figure_dir = Path(args['--figure-dir'])
-    params.code_path = Path(args['--code-path'])
-    params.aggregate_plot = args['--aggregate']
-    params.detail_plot = args['--detail']
-    sys.path.append(str(params.code_path))
-
+    params.img_format = args['--format']
     if not params.output_dir.exists():
         params.output_dir.mkdir(parents=True)
     if not params.figure_dir.exists():
         params.figure_dir.mkdir(parents=True)
     params.output_dir = str(params.output_dir)
 
     params.log_params = args['--log-params'] ## TODO: WARNING DEPRECATED
@@ -520,51 +704,67 @@
 
     if args['--param']:
         change_parameters(params, args['--param'])
 
     if args['--time']:
         params.steps = int(args['--time'])
     elif 'total_duration' in params.model.parameters:
-        params.steps = int(np.ceil(params.model.get_value('total_duration') / params.model.delta_t))
+        params.steps = int(np.ceil(params.model.get_value('total_duration') \
+                                   / params.model.delta_t))
     else:
         params.steps = 100
 
     if args['--modifiable']:
         show_parameters(params, short=True)
 
     set_seed(params, seed=args['--seed'], show=args['--show-seed'])
 
     if args['--echo']:
         print(args)
         sys.exit(0)
 
     params.view_machines = False
+    params.draw_graph = False
     if args['--view-model']:
         produce_diagrams(params)
         params.view_machines = True
+        params.draw_graph = True
 
     if args['--table-params']:
         table_param(params)
 
-    if args['diagrams']:
+    if args["--debug"]:
+        debug()
+
+    if args['check']:
+        check_model(params, args['MODEL'], args['--meta-tree'], args['--model-tree'])
+    elif args['diagrams']:
         produce_diagrams(params, view=True)
         sys.exit(0)
     elif args['generate']:
         generate_model(params)
     elif args['run']:
         init_main_level(params)
         run_model(params)
         if args['--plot']:
             plot_outputs(params)
+    elif args['compile']:
+        compile_yaml(params)
+# ORGANIZATION PART -------------------------
+            # organization_plot.plot_outputs(params)
+# -------------------------------------------
     elif args['show']:
         show_parameters(params)
     elif args['describe']:
         describe_parameters(params)
     elif args['plot']:
         plot_outputs(params)
+# ORGANIZATION PART -------------------------
+        # organization_plot.plot_outputs(params)
+# -------------------------------------------
     elif args['change']:
         not_implemented(params)
     elif args['sensitivity']:
         not_implemented(params)
     else:
         return params
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/__init__.py` & `emulsion-1.3b1/src/emulsion/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/agent/action.py` & `emulsion-1.3b1/src/emulsion/agent/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         if current_step < 0:
             current_step = 0
         # debuginfo([(current_step, action_performer.get_model_value(self.duration)) for _ in range(population)])
         l_exit_steps = [np.round(current_step + action_performer.get_model_value(self.duration)) for _ in range(population)]
         action_performer.update_time_to_exit({self.state_machine.machine_name: Counter(l_exit_steps)})
 
     def __str__(self):
-        return super().__str__() + ' on {} for state machine {}'.format(self.duration, self.state_machine.machine_name)
+        return super().__str__() + ' on {} for state machine {}'.format(self.duration, self.state_machine)
     __repr__ = __str__
 
 
 class SetVarAction(ValueAction):
     """SetVarAction allows to set the variable of the agent.
 
     """
@@ -278,14 +278,29 @@
 
     def __str__(self):
         return super().__str__() + ' {} <- {}'.format(self.statevar_name,
                                                       self.parameter)
     __repr__ = __str__
 
 
+################## ORGANIZATION PART
+class DepositAction(AbstractAction):
+    def __init__(self, statevar_name=None, parameter=None, model=None, **others):
+        super().__init__(**others)
+        self.parameters = others
+
+    def execute_action(self, unit, population=None, agents=None):
+        space = unit.get_information(self.parameters["target"])
+        info = self.parameters["information"]
+        value = self.parameters["value"]
+        space.informations[info] += unit.get_information(value)
+        # debuginfo(space.informations)
+################## END ORGANIZATION PART
+
+
 class RateAdditiveAction(ValueAction):
     """A RateChangeAction is aimed at increasing or decreasing a
     specific state variable or attribute, according to a specific rate
     (i.e. the actual increase or decrease is the product of the
     `parameter` attribute and a population size).
 
     """
@@ -493,14 +508,15 @@
         if agents is None:
             ## this is the case of IBM and compartment models
             agents = [action_performer]
         for agent in agents:
             l_protos = list(self.prototype_names)
             # compute actual values for probabilities
             l_proba_values = [agent.get_model_value(prob) for prob in self.probas]
+            # debuginfo(l_proba_values)
             total = sum(l_proba_values)
             assert(0 <= total <= 1)
             if total < 1:
                 # add complement
                 l_proba_values.append(1 - total)
                 # if N-1 probabilities were given for N prototypes, no
                 # problem: the last prototype is getting the 1-total
@@ -651,8 +667,9 @@
     'produce_offspring': CloneAction,
     'action': MethodAction,
     'duration': FunctionAction,
     'set_var': SetVarAction,
     'set_upper_var': SetUpperVarAction,
     'record_change': RecordChangeAction,
     'sample_durations': SampleDurationsAction,
+    'deposit': DepositAction
 }
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/atoms.py` & `emulsion-1.3b1/src/emulsion/organization/OrganizationPropagate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-"""A Python implementation of the EMuLSion framework (Epidemiologic
-MUlti-Level SImulatiONs).
-
-Classes and functions for entities management.
+"""
+.. module:: emulsion.organization
+.. moduleauthor:: Vianney Sicard <vianney.sicard@inrae.fr>
 """
 
 
 # EMULSION (Epidemiological Multi-Level Simulation framework)
 # ===========================================================
 # 
 # Contributors and contact:
@@ -49,166 +48,121 @@
 # 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
+import numpy as np
+from    emulsion.organization.Constante     import Constante as const
+from    emulsion.tools.debug                import debuginfo
+
+#   ____                        _          _   _             _____
+#  / __ \                      (_)        | | (_)           |  __ \
+# | |  | |_ __ __ _  __ _ _ __  _ ______ _| |_ _  ___  _ __ | |__) | __ ___
+# | |  | | '__/ _` |/ _` | '_ \| |_  / _` | __| |/ _ \| '_ \|  ___/ '__/ _ \
+# | |__| | | | (_| | (_| | | | | |/ / (_| | |_| | (_) | | | | |   | | | (_) |
+#  \____/|_|  \__, |\__,_|_| |_|_/___\__,_|\__|_|\___/|_| |_|_|   |_|  \___/
+#              __/ |
+#             |___/
+#                          _
+#                         | |
+#  _ __   __ _  __ _  __ _| |_ ___
+# | '_ \ / _` |/ _` |/ _` | __/ _ \
+# | |_) | (_| | (_| | (_| | ||  __/
+# | .__/ \__,_|\__, |\__,_|\__\___|
+# | |           __/ |
+# |_|          |___/
+
+
+class OrganizationPropagate():
+    """create and manage organizational propagate"""
+
+    def __init__(self, manager):
+        self.manager = manager
+
+    def propagate_information(self):
+        self.graph = self.manager.graph
+        self.organization_model = self.manager.organization_model
+        # get adjacency matrix and vector
+        if self.graph is not None:
+            matrix_vector = self.graph.propagate()
+
+            # debuginfo(matrix_vector)
+
+            # get spaces ang managers to update information values in the different nodes
+            dict_space = self.organization_model.dict_space
+            dict_manager = self.organization_model.dict_manager
+
+            # for each information
+            for information in self.graph.informations:
+                # calculate matrix product between adjacency matrix and transposed vector
+                delta = np.matmul(matrix_vector[information]["vector"].T, matrix_vector[information]["adjacency"]).T
+
+                # debuginfo(delta)
+
+                # update information (value + delta) for each node
+                ii=0
+                for key, node in self.graph.graph.nodes.items():
+                    # for atomic_space
+                    if key in dict_space:
+                        # if atomic_space has the information
+                        if information in dict_space[key].informations:
+                            dict_space[key].informations[information] += delta[ii][0]
+                            # debuginfo(key, "->", information, "==>", dict_space[key].informations[information])
+                    # for manager
+                    elif key in dict_manager:
+                        # if the manager has the information
+                        if information in dict_manager[key].informations:
+                            dict_manager[key].informations[informations] = delta[ii][0]
+                    else:
+                        debuginfo("propapagtion of information only in atomic_space or manager")
+                        raise Exception('CANNOT PROGATE')
+                    ii +=1
+
+    def propagate_matter(self):
+        self.graph = self.manager.graph
+        self.organization_model = self.manager.organization_model
+        # get adjacency matrix and vector
+        if self.graph is not None:
+            matrix_vector = self.graph.propagate()
+
+            # get spaces ang managers to update information values in the different nodes
+            dict_space = self.organization_model.dict_space
+            dict_manager = self.organization_model.dict_manager
+
+            # for each information
+            for information in self.graph.informations:
+                # debuginfo("!!", information)
+                adjacency = matrix_vector[information]["adjacency"]
+                vector = matrix_vector[information]["vector"]
+                # normalize each line of the adjacency matrix if superior to 1
+                new_adjacency = []
+                # get sum of the edges
+                sum_line_matrix = np.sum(adjacency, axis=1)
+                # aii = 1-(sum(line)-value(aii))
+                ii=0
+                for line in adjacency:
+                    if sum_line_matrix[ii] > 1:
+                        debuginfo('ERROR: the weight of the line is greater than 1. Check the transmission rates of the graph:', sum_line_matrix[ii])
+                        raise Exception("ERROR sum line greater than 1")
+                    aii = 1-(sum_line_matrix[ii] - adjacency[ii][ii])
+                    # debuginfo(aii)
+                    adjacency[ii][ii] = aii
+                    ii += 1
+
+                product = np.matmul(vector.T, adjacency)
+
+                # debuginfo('-'*50)
+                # debuginfo('\n',adjacency)
+                # debuginfo('-'*50)
+
+                ii = 0
+                for key, node in self.graph.graph.nodes.items():
+                    # for atomic space
+                    if key in dict_space:
+                        # if atomic_space has the information
+                        dict_space[key].informations[information] = product[0][ii]
+                        # debuginfo("info in", key, "---->", product[0][ii])
+                    ii += 1
 
-from   collections               import OrderedDict
-
-from   emulsion.agent.core       import EmulsionAgent
-from   emulsion.agent.process    import StateMachineProcess, MethodProcess
-
-#          _                                           _
-#     /\  | |                    /\                   | |
-#    /  \ | |_ ___  _ __ ___    /  \   __ _  ___ _ __ | |_
-#   / /\ \| __/ _ \| '_ ` _ \  / /\ \ / _` |/ _ \ '_ \| __|
-#  / ____ \ || (_) | | | | | |/ ____ \ (_| |  __/ | | | |_
-# /_/    \_\__\___/|_| |_| |_/_/    \_\__, |\___|_| |_|\__|
-#                                      __/ |
-#                                     |___/
-
-class AtomAgent(EmulsionAgent):
-    """The AtomAgent is aimed at representing an 'individual', i.e. the
-    smallest organization level to be modeled as an entity in the
-    simulation. An AtomAgent may be situated in several hosts, each one
-    associated with a specific tuple of state variables.
-
-    """
-    def __init__(self, **others):
-        super().__init__(**others)
-        self.statevars.population = 1
-        self.stochastic = True
-        self._host = OrderedDict()
-        if 'host' in others:
-            self.add_host(others['host'])
-
-    def __len__(self):
-        return 1
-
-    def get_content(self):
-        """Return the population (1) of the current unit.
-
-        """
-        return ('population', 1)
-
-    def add_host(self, host):
-        """Add the specified host to the current AtomAgent, associated
-        with the specified key.
-
-        """
-        self._host[host.keys] = host
-        if host.simulation is not None:
-            self.simulation = host.simulation
-
-    def remove_host(self, host, keys=None):
-        """Remove the specified host from the current AtomAgent,
-        associated with the specified key.
-
-        """
-        if keys is None:
-            del self._host[host.keys]
-        else:
-            if keys in self._host:
-                del self._host[keys]
-
-    def get_host(self, key='MASTER'):
-        """Retrieve the host of the current AtomAgent identified by the
-        specific key.
-
-        """
-        # DEBUG
-        try:
-            return self._host[key]
-        except Exception:
-            print(self, 'has pb getting host', key)
-            print(self._host)
-            print(self.statevars)
-
-    def clone(self, prototype=None, custom_prototype=None, **others):
-        """Make a copy of the current compartment with the specified
-        observable/value settings. If a prototype is provided, it is
-        applied to the new atom.
-
-        """
-        new_atom = self.__class__.from_dict(self.statevars)
-        new_atom.model = self.model
-        new_atom.level = self.level
-        new_atom._host = dict(self._host)
-        new_atom.statevars.update(**others)
-        if prototype is not None:
-            new_atom.apply_prototype(name=prototype)
-        elif custom_prototype is not None:
-            new_atom.apply_prototype(prototype=custom_prototype)
-        return new_atom
-
-
-#  ______          _       _                     _
-# |  ____|        | |     (_)               /\  | |
-# | |____   _____ | |_   ___ _ __   __ _   /  \ | |_ ___  _ __ ___
-# |  __\ \ / / _ \| \ \ / / | '_ \ / _` | / /\ \| __/ _ \| '_ ` _ \
-# | |___\ V / (_) | |\ V /| | | | | (_| |/ ____ \ || (_) | | | | | |
-# |______\_/ \___/|_| \_/ |_|_| |_|\__, /_/    \_\__\___/|_| |_| |_|
-#                                   __/ |
-#                                  |___/
-
-class EvolvingAtom(AtomAgent):
-    """An EvolvingAtom is able to change state according to its
-    own statemachines.
-
-    """
-    def __init__(self, statemachines=[], **others):
-        super().__init__(**others)
-        self.processes = []
-        self.statemachine_processes = {}
-        self.method_processes = {}
-        if statemachines:
-            self.set_statemachines(statemachines)
-
-    def set_statemachines(self, statemachines):
-        """Define the state machines that this agent is able to execute."""
-        self.statemachine_processes = {
-            sm.machine_name: StateMachineProcess(sm.machine_name, self, sm)
-            for sm in statemachines
-        }
-
-    def init_level_processes(self):
-        """Initialize the level of the agent."""
-        if self.level in self.model.processes:
-            self.processes = self.model.processes[self.level]
-            for d_process in self.processes:
-                for process_name, grouping in d_process.items():
-                    # iterate over items of the dict which should contain only one key:value prepair
-                    if process_name not in self.statemachine_processes:
-                        self.add_method_process(process_name)
-
-    def add_method_process(self, process_name, method=None):
-        """Add a process based on a method name."""
-        if method is None:
-            method = getattr(self, process_name)
-        self.method_processes[process_name] = MethodProcess(process_name, method)
-
-    def get_machine(self, name):
-        """Return the state machine with the specified name."""
-        return self.statemachine_processes[name].state_machine
-
-    def evolve(self, machine=None):
-        super().evolve(machine=machine)
-        self.evolve_states()
-
-    def evolve_states(self, machine=None):
-        """Change the state of the current unit according to the
-        specified state machine name. If no special state machine is
-        provided, executes all the machines.
-
-        """
-        # retrieve the iterable containing the processes to execute
-        if machine is not None:
-            self.statemachine_processes[machine].evolve()
-        else:
-            for d_process in self.processes:
-                for process_name in d_process:
-                    process = self.statemachine_processes[process_name]\
-                                if process_name in self.statemachine_processes\
-                                else self.method_processes[process_name]
-                    process.evolve()
+                # raise
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/comparts.py` & `emulsion-1.3b1/src/emulsion/agent/comparts.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 
 import numpy                     as np
 
 from   emulsion.agent.core       import GroupAgent
-from   emulsion.model.exceptions import SemanticException
 from   emulsion.agent.exceptions import InvalidCompartmentOperation
 from   emulsion.tools.misc       import POPULATION
 from   emulsion.tools.debug      import debuginfo
 
 class Compartment(GroupAgent):
     """An Compartment is a compartment which does not
     represent the underlying level but with aggregate information such
@@ -153,17 +152,15 @@
         else:
             if current_step in self.times_to_exit[machine_name]:
                 return {current_step: min(total_qty, self.times_to_exit[machine_name][current_step])}
             else:
                 return
 
         d_result = {}
-        # debuginfo(self, total_qty, machine_name)
         while total_qty > 0:
-            # debuginfo(l_available_dates, total_qty)
             l_steps, l_qty = zip(*l_available_dates)
             total = sum(l_qty)
             if total == 0:
                 return {}
             l_probas = [qty / total for qty in l_qty]
             l_to_sample = np.random.multinomial(total_qty, l_probas)
             # check that quantities required by multinomial sampling are available
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/core/__init__.py` & `emulsion-1.3b1/src/emulsion/agent/core/__init__.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/agent/core/abstract_agent.py` & `emulsion-1.3b1/src/emulsion/agent/core/abstract_agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,15 +62,16 @@
 
 
 from   emulsion.tools.state       import StateVarDict
 from   emulsion.agent.meta        import MetaAgent
 from   emulsion.agent.exceptions  import StateVarNotFoundException
 from   emulsion.tools.misc        import retrieve_value
 from   emulsion.tools.debug       import debuginfo
-from   emulsion.model.exceptions  import SemanticException
+
+from   emulsion.tools.debug       import debuginfo
 
 
 #           _         _                  _                            _
 #     /\   | |       | |                | |     /\                   | |
 #    /  \  | |__  ___| |_ _ __ __ _  ___| |_   /  \   __ _  ___ _ __ | |_
 #   / /\ \ | '_ \/ __| __| '__/ _` |/ __| __| / /\ \ / _` |/ _ \ '_ \| __|
 #  / ____ \| |_) \__ \ |_| | | (_| | (__| |_ / ____ \ (_| |  __/ | | | |_
@@ -204,14 +205,15 @@
     def get_model_value(self, name):
         """Return the value corresponding to the specified name in the model
         of the agent. If the name refers to a function, apply this
         function to the agent.
 
         TAG: USER
         """
+        # debuginfo(name)
         return retrieve_value(self.model.get_value(name), self)
 
     @property
     def delta_t(self):
         """A shortcut to `self.model.delta_t`."""
         return self.model.delta_t
 
@@ -275,46 +277,91 @@
         #         return self.get_host().get_information(name)
         #     elif name in self.model._values:
         #         return self.get_model_value(name)
         #     else:
         #         raise StateVarNotFoundException(name, self)
 
         ## REWRITTEN (2021, May) to force search of variables in upper levels
-        if name in self.statevars:
-            return self.statevars[name]
-        if name in self._mbr_cache:
-            return getattr(self, name)
+        # debuginfo("get_information -> abstract_agent ----->", self, name, self.model)
+        # raise Exception(self.model.organization_model.l_getters)
+
+
+
+        # if name in self.model.organization_model.l_comb_getters:
+        #     total = self.model.organization_model.get_information(self, name)
+        #     return total
+
+        # debuginfo("==>", self, "for", name)
+
         if name in self.model._values:
             return self.get_model_value(name)
+        if name in self._mbr_cache:
+            # debuginfo(name, "in", self)
+            return getattr(self, name)
+        if name in self.statevars:
+            return self.statevars[name]
+###############ORGANIZATION PART
+        if 'total_' not in name and hasattr(self, 'passport') and self.passport is not None:
+            # debuginfo(name, self.passport.current_locations)
+            ret = self.model.organization_model.get_information(self, name)
+            # debuginfo("RET FOR", self)
+            # debuginfo("\t\tRET ", ret, ret.keys)
+            if ret != -1:
+                return ret
+
+        # if 'my_' in name:
+        #     debuginfo("my_ in", name, "for", self)
+        #     ret = self.model.organization_model.get_information(self, name)
+        #     debuginfo("reload with", ret)
+        #     self.get_information(ret)
+        #     # raise Exception(ret)
+
+        if "info_" in name:
+                        # debuginfo("info")
+            ret = self.model.organization_model.get_information(self, name)
+            # debuginfo(ret)
+            # raise
+            return ret
+        if name in self.model.organization_model.dict_manager:
+            if name in self.passport.current_locations:
+                return self.passport.current_locations[name]['location']
+            else:
+                return None
+###############END ORGANIZATION PART
         if self._host is not None:
             try:
+                # debuginfo("reload !! from", self, name)
+                # debuginfo(self.get_host().get_information(name))
                 return self.get_host().get_information(name)
             except AttributeError:
+                # debuginfo("get upper")
                 return self.upper_level().get_information(name)
-        raise StateVarNotFoundException(name, self)
+
+        # raise StateVarNotFoundException(name, self)
 
     def set_information(self, name, value):
         """Set the specified value for the statevar/attribute.
 
         TAG: USER
         """
         # if hasattr(self, name):
         #     setattr(self, name, value)
         # else:
         #     setattr(self.statevars, name, value)
         # REWRITTEN for efficiency improvement
+        raise Exception("set", name, "for", value)
         if name in self._mbr_cache:
             setattr(self, name, value)
         elif name in self.statevars:
             setattr(self.statevars, name, value)
             # do NOT use self.statevars[name]=value to ensure recursive lookup
         elif self._host is not None:
             self.get_host().set_information(name, value)
         else:
-            debuginfo(str(self), self._mbr_cache)
+            # debuginfo(str(self), self._mbr_cache)
             raise StateVarNotFoundException(name, self)
 
     def init_time_entered(self, machine_name, advance=0, nb_timesteps=0):
         """Initialize the time step value when this agent is entering a new
         state of the specified state machine. A (positive) `advance`
         value can be provided to mimick an earlier entering in the
         state. By default, a `_time_to_exit` value is set according to
@@ -322,47 +369,37 @@
 
         """
         key = '_time_entered_{}'.format(machine_name)
         key_TTE = '_time_to_exit_{}'.format(machine_name)
         self.statevars[key] = self.statevars.step - advance
         self.statevars[key_TTE] = self.statevars[key] + nb_timesteps
 
-    def change_state(self, machine_name, new_state_or_value, do_actions=False):
+    def change_state(self, machine_name, new_state, do_actions=False):
         """Change the state of this agent for the specified state machine to
         `new_state`. The `_time_entered_MACHINE` value for this state machine
         is initialized. If do_actions is True, perform the actions to
         do on_exit from the previous state (if any) and those to do
         on_enter in the new state (if any).
 
         TAG: USER?
         """
         # retrieve the state machine from its name
         state_machine = self.model.state_machines[machine_name]
-        # if value provided, convert to state
-        if new_state_or_value in state_machine.states.__members__:
-            new_state = new_state_or_value
-        else:
-            index = int(new_state_or_value)
-            if index < 1 or index > len(state_machine.states):
-                raise SemanticException('Attempt to change state for state machine {} with incorrect numeric value: {}'.format(machine_name, new_state_or_value))
-            new_state = state_machine.states(index)
-
         # if asked to do actions, first execute the 'on_exit' actions
         # of current state
         if do_actions:
             current_state = self.statevars[machine_name]\
                             if machine_name in self.statevars else None
             if current_state is not None:
                 self.do_state_actions('on_exit', state_machine, current_state.name)
-
         # change the state in the statevar
         self.statevars[machine_name] = new_state
-
         # initialize the _time_entered_STATEMACHINE variable
         self.init_time_entered(machine_name)
+
         # if asked to do actions, execute the 'on_enter' actions of
         # the new state
         if do_actions:
             # do on_enter actions associated to the new value
             self.do_state_actions('on_enter', state_machine, new_state.name, agents=[self])
 
     def update_time_to_exit(self, machine_name, duration):
@@ -425,38 +462,73 @@
         corresponding attributes (mainly _time_entered) ; if
         execute_actions is True, on_enter/on_exit actions are
         performed.
 
         TAG: USER
 
         """
+        # debuginfo("PROTOTYPE:", name)
         # give priority to named prototypes if provided, else
         if name is not None:
             prototype = self.model.get_prototype(self.level, name, self.get_information('simu_id'))
         if prototype is None:
             raise SemanticException("Agent {} was asked to apply inexistent prototype".format(self))
+
         self._last_prototype = prototype
         # if any 'begin_with' sequence is defined, apply immediately in the specified order
         if 'begin_with' in prototype:
             l_tuples = prototype['begin_with']
             for var, value in l_tuples:
                 val = value(self) if callable(value) else value
                 # set the value to the variable depending on the nature of the variable
                 if var in self.model.state_machines:
                     self.change_state(var, val, do_actions=execute_actions)
                 else:
                     self.statevars[var] = val
         # for regular cases:
         # apply changes in states first, then other variables
+        # debuginfo("execute change_state")
         for var, value in prototype.items():
             if var in self.model.state_machines:
                 val = value(self) if callable(value) else value
+                # debuginfo(var, "->", val, "-", execute_actions)
                 self.change_state(var, val, do_actions=execute_actions)
+
+        # debuginfo("apply organization locations")
         for var, value in prototype.items():
             if var not in self.model.state_machines and var != 'in_order':
+# ORGANIZATION_PART-----------
+                # if model has an organization structure,
+                # then add agent to the organization corresponding to the prototype
+                # debuginfo("execute_actions:", execute_actions)
+                if var == "organization":
+                    # debuginfo(name)
+                    # debuginfo(prototype)
+                    self.statevars["tmp_prototype"] = name
+                 # and not execute_actions:
+                    for org in value:
+                        organization = self.model.get_organization(org)
+                        # add agent in organization
+                        organization.add_atom(self)
+                        # add observer from state_machine
+                        for sm in organization.list_state_machine:
+                            self.add_observer(organization, sm)
+                        # add observer from triggers
+                        for obs in organization.list_trigger:
+                            self.add_observer(organization, obs)
+                    # allocate in each organization at initialization
+                    # when all unit are affected -> locate in organization
+                    # in the order of the prototype
+                    for org_name in value:
+                        org = organization.organization_model.dict_roots[org_name]
+                        # debuginfo("check in", org.keys, " -", self)
+                        # debuginfo("\t\t APPLY PROTOTYPE")
+                        org.check_list_indiv()
+                        # debuginfo(self.passport.current_locations)
+# ----------------------------
                 val = value(self) if callable(value) else value
                 self.statevars[var] = val
         # if any 'end_with' sequence is defined, apply finally in the specified order
         if 'end_with' in prototype:
             l_tuples = prototype['end_with']
             for var, value in l_tuples:
                 val = value(self) if callable(value) else value
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/core/emulsion_agent.py` & `emulsion-1.3b1/src/emulsion/agent/core/emulsion_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,19 +56,17 @@
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 import abc
 
 import numpy                      as np
 
-from   sortedcontainers           import SortedSet
 
 from   emulsion.tools.graph       import EdgeTypes
 from   emulsion.model.functions   import EDGE_KEYWORDS
-from   emulsion.model.exceptions  import SemanticException
 from   emulsion.tools.misc        import rates_to_probabilities,\
     aggregate_probabilities, probabilities_to_rates, count_population, AGENTS
 from   emulsion.tools.debug       import debuginfo
 
 from   emulsion.agent.core.abstract_agent  import AbstractAgent
 
 
@@ -344,15 +342,20 @@
             # only edges with condition fulfilled are taken into account
             if cond_result:
                 flux = None
                 for keyword in EDGE_KEYWORDS:
                     if keyword in props:
                         flux = keyword
                         break
-                value = state_machine.get_value(props[flux])
+                try:
+                    value = state_machine.get_value(props[flux])
+                except:
+                    debuginfo('ERROR -->', flux, "in", props)
+                    debuginfo('EDGE_KEYWORDS:', EDGE_KEYWORDS)
+                    raise Exception('keyword EDGE_KEYWORDS not exists in props')
                 actions = props['actions'] if 'actions' in props else []
                 if callable(value):
                     value = value(self)
                 elif type(value) == str:
                     value = self.get_information(value)
                 if value > 0 or flux == 'amount-all-but':
                     result.append((state, flux, value, cond_result, actions))
@@ -467,16 +470,15 @@
         # transformation occurs, 2) probabilities - in that case the
         # values must be converted to rates if the target compartment
         # is deterministic, otherwise the step duration must be taken
         # into account; 3) rates - in that case the values must be
         # converted to probabilities if the target compartment is
         # stochastic
         available_flux = set(flux)
-        if len(available_flux) != 1 and available_flux != set(['amount', 'amount-all-but']):
-            raise SemanticException("Inconsistent transition flux, trying to use simultaneously {}".format(flux))
+        assert len(available_flux) == 1 or available_flux == set(['amount', 'amount-all-but'])
 
         method = None
         if 'amount' in available_flux or 'amount-all-but' in available_flux:
             # handle values as amounts
             method = 'amount'
             total_ref_pop = count_population(reference_pop)
             # check that values are between 0 and the population size,
@@ -601,14 +603,46 @@
         """
         # retrieve name of the state machine associated with the state_name
         varname = self.get_model_value(state_name).state_machine.machine_name
         result = self.statevars[varname].name == state_name\
                  if varname in self.statevars else False
         return result
 
+################## ORGANIZATION PART
+    def is_in_space(self, space_name):
+        """Evaluate if the agent is in the specified space.
+
+        """
+        if hasattr(self, 'passport'):
+            # debuginfo(self, space_name, self.passport.current_locations)
+            space = self.model.organization_model.dict_space[space_name]
+            for loc in self.passport.current_locations.values():
+                if 'reference' not in loc and space in loc['set']:
+                    return True
+            return False
+        else:
+            manager = self.model.organization_model.dict_manager
+            space = self.model.organization_model.dict_space
+            real_space = None
+            if space_name in manager:
+                real_space = manager[space_name]
+            elif space_name in space:
+                real_space = space[space_name]
+            else:
+                raise Exception(self, space_name, self.passport)
+            for k,v in self.statevars.items():
+                if v == real_space:
+                    return True
+            return False
+
+    def get_index(self, space):
+        raise Exception("HERE OK")
+
+################## END ORGANIZATION PART
+
     def get_outbox(self):
         """Return the content of the outbox.
 
         TAG: USER
         """
         return self._outbox
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/exceptions.py` & `emulsion-1.3b1/src/emulsion/agent/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         self.statevar = statevar
         self.source = source
 
     def __str__(self):
         return 'Statevar %s not found in object %s' % (self.statevar,
                                                        self.source)
 
-
 class LevelException(Exception):
     """Exception raised when a semantic error occurs during model parsing.
 
     """
     def __init__(self, cause, level):
         super().__init__()
         self.level = level
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/__init__.py` & `emulsion-1.3b1/src/emulsion/agent/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/abstract_process_manager.py` & `emulsion-1.3b1/src/emulsion/agent/managers/abstract_process_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -66,20 +66,21 @@
 from   sortedcontainers          import SortedSet
 
 import numpy                     as np
 import pandas                    as pd
 
 from   emulsion.agent.views      import StructuredView, AdaptiveView
 from   emulsion.agent.process    import MethodProcess, StateMachineProcess
-from   emulsion.agent.exceptions import StateVarNotFoundException, LevelException
+from   emulsion.agent.exceptions import StateVarNotFoundException
 from   emulsion.tools.misc       import load_class, add_new_property, add_all_test_properties, add_all_relative_population_getters
 from   emulsion.tools.getters    import create_population_getter, create_aggregator, create_group_aggregator, make_information_getter
 from   emulsion.tools.debug      import debuginfo
 
 from   emulsion.agent.managers.group_manager  import  GroupManager
+from   emulsion.tools.debug      import debuginfo
 
 
 #           _         _                  _
 #     /\   | |       | |                | |
 #    /  \  | |__  ___| |_ _ __ __ _  ___| |_
 #   / /\ \ | '_ \/ __| __| '__/ _` |/ __| __|
 #  / ____ \| |_) \__ \ |_| | | (_| | (__| |_
@@ -225,14 +226,15 @@
         ## which are defined at current level (e.g. population)
         for sublevel in self.model.levels_graph.successors(self.level):
             for process in self.model.processes[sublevel]:
                 for process_name, grouping in process.items():
                     ## skip processes not associated with a grouping
                     if grouping is None:
                         continue
+
                     compart_properties = dict(self.model.compartments[self.level][grouping])
                     for keyword in ['compart_manager', 'compart_class']:
                         if keyword in compart_properties:
                             class_desc = compart_properties[keyword]
                             compart_properties[keyword] = load_class(**class_desc)
                     self.add_compart_process(grouping, **compart_properties)
 
@@ -245,14 +247,34 @@
 
         """
         if 'contains' not in self.model.levels[self.level]:
             raise LevelException('not specified for atom creation', '')
         return self.model.levels[self.level]['contains'][0]
 
 
+    # def evolve(self, **others):
+    #     """Make the ProcessManager evolve, i.e. all the registered processes
+    #     in order, starting with the evolution of the sublevels, and
+    #     followed by the evolution inherited from superclasses.
+
+    #     """
+    #     # for key, manager in self.model.organization_model.dict_roots.items():
+    #     #     manager.organization_processes.execute_on_enter()
+    #     # self['MASTER'].evolve()
+    #     # debuginfo(self._content)
+    #     if self.statevars._is_active:
+    #         for process in self:
+    #             process.evolve()
+    #         for name, process in self._content.items():
+    #             if name not in self.no_compart:
+    #                 self.add_new_population(process.new_population)
+    #                 process.update_counts()
+
+    #     super().evolve(**others)
+
     def add_method_process(self, process_name, method=None):
         """Add a process based on a method name."""
         if method is None:
             method = getattr(self, process_name)
         self._content[process_name] = MethodProcess(process_name, method)
         self.no_compart.add(process_name)
 
@@ -277,14 +299,15 @@
         StructuredView or GroupManager). The compartment manager may
         be associated with a specific state machine, and MUST BE
         identified by a tuple of state variables names. Additionally,
         since a first compartment is also instantiated, a specific
         class to do so can be also specified.
 
         """
+
         ## TODO: adapt to multiple state machines per grouping
         args = {'keys': tuple(key_variables), 'host': self,
                 'keep_history': self.keep_history}
         compart_manager_cl, manager_options = compart_manager
         compart_class_cl, compart_options = compart_class
         if any(state_machines):
             l_machines = [self.model.state_machines[machine_name]
@@ -297,14 +320,32 @@
             for machine in l_machines:
                 for state in machine.states:
                     if not state.autoremove:
                         self.create_count_properties_for_state(process_name,
                                                                state.name,
                                                                create_population_getter,
                                                                create_group_aggregator)
+
+####################### ORGANIZATION PART
+        for k in key_variables:
+            if k in self.model.organization_model.dict_level:
+                for space in self.model.organization_model.dict_level[k]["ALL"]:
+                    self.create_count_properties_for_state(process_name,
+                                                           space.name,
+                                                           create_population_getter,
+                                                           create_group_aggregator)
+        # add organization in l_machines for create correct groupings
+        for k in key_variables:
+            # debuginfo(k, "===>", self.model.organization_model.dict_level)
+            if k in self.model.organization_model.dict_level:
+                # debuginfo("OK -->", k, self.model.organization_model.dict_level[k])
+                l_machines.append(k)
+                # l_machines += self.model.organization_model.dict_level[k]['relative_org']
+####################### END ORGANIZATION PART
+
         ## TODO: check if obsolete ?
         if allowed_values:
             args['allowed_values'] = allowed_values
 
         args.update(manager_options)
         dict_comp = compart_manager_cl(**args)
         # update the model of the compartment manager
@@ -319,84 +360,129 @@
             values=init_key,
             host=dict_comp, **compart_options)
         # update the model of views
         dict_comp._content[init_key].model = self.model
         self._content[process_name] = dict_comp
         # dynamically add properties for accessing sub-groups when
         # groupings are based on several states from statemachines
+########################## ORGANIZATION PART
+        # create an imaginary upper concept of state machines and organizations  called <<states_process>>
+        self.all_states_process = dict(self.model.state_machines, **self.model.organization_model.dict_level)
+
+        # old version (only state machines
+        # if len(key_variables) > 1 and\
+        #    all(key in self.model.state_machines for key in key_variables):
+        # substituated by :
         if len(key_variables) > 1 and\
-           all(key in self.model.state_machines for key in key_variables):
+          all(key in self.all_states_process for key in key_variables):
+########################## END ORGANIZATION PART
+            # debuginfo("###", process_name, key_variables)
             self.create_properties_for_groups(process_name, key_variables)
+        # dynamically add properties for testing states in compart_class instances
+        add_all_test_properties(dict_comp._content[init_key])
 
-        ## EXPERIMENTAL - replaced by callable class in the model
-        # # dynamically add properties for testing states in compart_class instances
-        # add_all_test_properties(dict_comp._content[init_key])
 
+        # debuginfo("A --", self.model.compartments)
         # dynamically add properties for relative counts in compart_class instances
+        # debuginfo(self._content)
+        # raise Exception(dict_comp[init_key], dict_comp[init_key].statevars)
         add_all_relative_population_getters(dict_comp._content[init_key], key_variables)
 
+
+        # debuginfo("B --", self.model.compartments)
+
     def create_count_properties_for_state(self, grouping_or_machine_name, state_name,
                                           count_function, aggregation_function):
         """Dynamically add properties of the form ``total_S`` where S can be
         any state of the state machine. Counts are expected to be
         computed by the grouping associated with the specified
         process. The access to counts is defined by
         *count_function*. If aggregated variables such as ``aggvar``
         are defined, corresponding properties of the form
         ``aggvar_S``are also defined with the specified
         *aggregation_function*.
 
         """
+        # debuginfo(grouping_or_machine_name, state_name, count_function, aggregation_function)
         add_new_property(self, 'total_{}'.format(state_name),
                          count_function(grouping_or_machine_name, state_name))
+        # debuginfo("ADD NEW PROPERTY FOR", 'total_{}'.format(state_name))
+
         if self.level in self.model.aggregate_vars:
             for (varname, sourcevar, operator) in self.model.aggregate_vars[self.level]:
+                # debuginfo("COUNT -> ", varname, sourcevar, operator)
                 add_new_property(self, '{}_{}'.format(varname, state_name),
                                  aggregation_function(sourcevar, operator,
                                                       grouping_or_machine_name, state_name))
+        # debuginfo("--------------",self.model.aggregate_vars)
 
     def create_properties_for_groups(self, grouping_name, key_variables):
         """Dynamically add properties of the form `total_S_T` where S, T are a
         valid key in the specified grouping.
 
         """
-        combinations = list(it.product(*[[state.name
-                                          for state in self.model.state_machines[machine_name].states
-                                          if not state.autoremove]
-                                         for machine_name in key_variables]))
+#################### ORGANIZATION PART
+        # old version with only state machines
+        # combinations = list(it.product(*[[state.name
+        #                                   for state in self.model.state_machines[machine_name].states
+        #                                   if not state.autoremove]
+        #                                  for machine_name in key_variables]))
+        # new version taking into account both stet machines and organizations :
+
+        # debuginfo("a --", self.model.compartments)
+        combinations = []
+        for k in key_variables:
+            if k in self.model.organization_model.dict_level:
+                l_tmp = [space.name for space in self.model.organization_model.dict_level[k]['ALL']]
+                combinations.append(l_tmp)
+            else:
+                l_tmp = [state.name for state in self.model.state_machines[k].states]
+                combinations.append(l_tmp)
+        combinations = list(it.product(*combinations))
+        # debuginfo("COMBINATION", combinations)
+        # debuginfo("b --", self.model.compartments)
+#################### END ORGANIZATION PART
+        # debuginfo(self, '->', combinations)
         for group in combinations:
             add_new_property(self, 'total_{}'.format('_'.join(group)),
                              create_population_getter(grouping_name, group))
             if self.level in self.model.aggregate_vars:
                 for (varname, sourcevar, operator) in self.model.aggregate_vars[self.level]:
                     add_new_property(self, '{}_{}'.format(varname, '_'.join(group)),
                                      create_group_aggregator(sourcevar, operator,
                                                              grouping_name, group))
 
+        # debuginfo("c --", self.model.compartments)
+        # debuginfo("--> create properties for groups -->", self._content["infection"]._content[None,None].statevars)
+
 
     def get_group_population(self, grouping_name, t_states):
         """Return the size of the subgroup within the specified *grouping_name*
         associated with the specified tuple of states *t_states*.
 
         """
         complete_key = set(self.get_model_value(state_name)
                            for state_name in t_states)
         groups = self[grouping_name]
         value = 0
         for key, compart in groups._content.items():
+            # debuginfo("complete key ->", complete_key, " -- set key ->", key, "-?", complete_key <= set(key))
             if complete_key <= set(key):
                 value += compart.population
+
+        # debuginfo("TOTAL FOR", complete_key, ":", value)
         return value
 
     @property
     def counts(self):
         """Return a pandas DataFrame containing counts of each process if existing.
         TODO: column steps need to be with one of process
 
         """
+
         res = {}
         for comp in self:
             try:
                 # TODO: BUG with StructuredViewWithCounts, step=0 always !
                 if comp.__class__.__name__ != 'StructuredViewWithCounts':
                     comp.update_counts()
                     res.update(comp.counts)
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/compart_process_manager.py` & `emulsion-1.3b1/src/emulsion/agent/managers/compart_process_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,19 +156,18 @@
                     continue
                 self.create_properties_for_groups('MASTER', d_grouping_desc['key_variables'])
                 add_all_relative_population_getters(self['MASTER']._content[init_key], d_grouping_desc['key_variables'])
 
         for variable_name in t_key_variables_MASTER:
             add_all_relative_population_getters(self['MASTER']._content[init_key], (variable_name,))
 
-        ## EXPERIMENTAL - replaced by callable class in the model
-        # ## ADD is_X and duration_in_machine properties for state
-        # ## machines used as StateMachineProcesses for the current
-        # ## population
-        # add_all_test_properties(self)
+        ## ADD is_X and duration_in_machine properties for state
+        ## machines used as StateMachineProcesses for the current
+        ## population
+        add_all_test_properties(self)
 
     def evolve(self, **others):
         """Make the ProcessManager evolve, i.e. all the registered processes
         in order, starting with the evolution of the sublevels, and
         followed by the evolution inherited from superclasses.
 
         """
@@ -180,15 +179,14 @@
                 if name not in self.no_compart:
                     # debuginfo('>'*20)
                     # debuginfo(process, process.new_population)
                     self.add_new_population(process.new_population)
                     process.update_counts()
         super().evolve(**others)
 
-
     def add_compart_process(self,
                             process_name,
                             key_variables,
                             compart_manager=(GroupManager, {}),
                             state_machines=[],
                             compart_class=(Compartment, {})):
         if process_name not in self._content:
@@ -259,15 +257,15 @@
                         if key not in to_add:
                             to_add[key] = 0
                         to_add[key] += qty
 
             self.add_population(to_add, init=True)
             for proc, group_manager in self._content.items():
                 if proc not in self.no_compart:
-                    # group_manager.do_enter_actions_on_init()
+                    group_manager.do_enter_actions_on_init()
                     group_manager.update_counts()
 
     def add_new_population(self, population):
         """Add new individuals to the appropriate compartments"""
         to_add = {}
         for target_state, amount, proto in population:
             sublevel = self.get_default_sublevel()
@@ -340,22 +338,24 @@
                 else:
                     d_real_population_spec[real_key] += amount
         # debuginfo(d_real_population_spec)
 
         for key, qty in d_real_population_spec.items():
             if key not in group_manager._content:
                 d_statevars = {state.state_machine.machine_name: state for state in key}
-                new_comp = group_manager[default_key].clone(population=0, **d_statevars)
+                new_comp = group_manager[default_key].clone(population=qty, **d_statevars)
                 new_comp.keys = key
                 group_manager._content[key] = new_comp
-            # else:
-            # debuginfo(">"*5, group_manager[key], key, qty)
-            group_manager[key].add(qty)
-            for state in key:
-                group_manager[key].do_state_actions('on_enter', state.state_machine, state.name, population=qty)
+            else:
+                # debuginfo(">"*5, group_manager[key], key, qty)
+                group_manager[key].add(qty)
+                for state in key:
+                    # debuginfo('DOING ACTIONS ON ENTER FOR', group_manager[key], state.name, state.name)
+                    group_manager[key].do_state_actions('on_enter', state.state_machine, state.name, population=qty)
+                    # debuginfo('=>', group_manager[key].times_to_exit)
             nb_added += qty
         self.statevars.population += nb_added
 
         if init:
             group_manager.update_counts()
 
     def remove_population(self, d_population_spec):
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/functions.py` & `emulsion-1.3b1/src/emulsion/agent/managers/functions.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/group_manager.py` & `emulsion-1.3b1/src/emulsion/agent/managers/group_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 from   sortedcontainers          import SortedDict
 
 from   emulsion.agent.views      import StructuredView
 from   emulsion.tools.misc       import count_population, rewrite_keys
 from   emulsion.tools.debug      import debuginfo
 
 from   emulsion.agent.managers.functions import group_and_split_populations
+from   emulsion.tools.debug              import debuginfo
+
+from   emulsion.model.state_machines     import StateMachine
 
 #   _____                       __  __
 #  / ____|                     |  \/  |
 # | |  __ _ __ ___  _   _ _ __ | \  / | __ _ _ __   __ _  __ _  ___ _ __
 # | | |_ | '__/ _ \| | | | '_ \| |\/| |/ _` | '_ \ / _` |/ _` |/ _ \ '__|
 # | |__| | | | (_) | |_| | |_) | |  | | (_| | | | | (_| | (_| |  __/ |
 #  \_____|_|  \___/ \__,_| .__/|_|  |_|\__,_|_| |_|\__,_|\__, |\___|_|
@@ -95,31 +98,48 @@
         self.init_counts()
 
     def init_counts(self, index=0):
         """Initialize the counts."""
         self.counts = {}
         if any(self.l_state_machines):
             for machine in self.l_state_machines:
-                self.counts.update({state.name: [] if self.keep_history else 0
-                                    for state in machine.states})
+                if isinstance(machine, StateMachine):
+                    self.counts.update({state.name: [] if self.keep_history else 0
+                                        for state in machine.states})
+                else:
+                    org_mod = self._host.model.organization_model
+                    level = org_mod.dict_level[machine]["ALL"]
+                    # debuginfo(level)
+                    self.counts.update({space.name: [] if self.keep_history else 0
+                                        for space in level})
             self.counts['step'] = [] if self.keep_history else 0
+
         else:
             super().init_counts()
 
     def update_counts(self):
         """Update the number of atoms for each state of the state
         machine (TODO: for each value of the key[index] enum).
 
         """
         if any(self.l_state_machines):
-            total = {state.name: 0 for machine in self.l_state_machines for state in machine.states}
+            total = {}
+            for machine in self.l_state_machines:
+                # condition for organization
+                if isinstance(machine, StateMachine):
+                    total.update({state.name: 0 for state in machine.states})
+                else:
+                    org_mod = self._host.model.organization_model
+                    level = org_mod.dict_level[machine]["ALL"]
+                    total.update({space.name: 0 for space in level})
             for (key, compartment) in self._content.items():
                 for state in key:
                     if state is not None and state.name in total:
                         total[state.name] += compartment.get_information('population')
+
             if self.keep_history:
                 self.counts['step'].append(self.statevars.step)
                 for state in machine.states:
                     self.counts[state.name].append(total[state.name])
             else:
                 self.counts['step'] = self.statevars.step
                 self.counts.update(total)
@@ -130,22 +150,20 @@
     #     """Force all Compartment agents of this group manager to execute the actions on_enter for each state for their initial population (if any actions on enter). WARNING: this method is intended only for compartment-based models."""
     #     l_states_with_actions_on_enter = []
     #     for state_machine in self.l_state_machines:
     #         for state in state_machine.states:
     #             if state.name in state_machine.state_actions and 'on_enter' in state_machine.state_actions[state.name]:
     #                 l_states_with_actions_on_enter.append(state.name)
 
-    #     debuginfo(l_states_with_actions_on_enter)
     #     for (key, compartment) in self._content.items():
     #         if compartment.statevars.population == 0:
     #             continue
     #         for state in key:
     #             if state.name not in l_states_with_actions_on_enter:
     #                 continue
-    #             debuginfo(self.statevars.step, "ACTIONS ON INIT")
     #             compartment.do_state_actions('on_enter', state.state_machine, state.name, population=compartment.statevars.population)
 
 
     def apply_changes(self, d_transitions, state_machine):
         """Apply modifications to the compartments contained in the current
         GroupManager, according to *d_transitions*. Dictionary *d_transitions*
         is keyed by a tuple of variables and associated with a list of tuples.
@@ -153,57 +171,77 @@
         and a dictionary, either
         {'population': (qty, esc), 'actions': list} or {'agents': list, 'actions': list}.
         Parameter *state_machine* indicates which state machine produced
         d_transitions, in order to perform adequate actions on
         entering/exiting states or on crossing edges.
 
         """
+        # debuginfo("APPLY CHANGES", d_transitions)
         for source, t_evolutions in d_transitions.items():
             for target, d_population_or_agents in t_evolutions:
                 target_group = self.get_or_build(target, source=self[source])
                 self._content[source].move_to(target_group, state_machine=state_machine, **d_population_or_agents)
+                for atom in d_population_or_agents['agents']:
+                    atom.notify()
 
     def evolve(self, machine_index=None):
         """Ask each group to make its content evolve, then remove population or
         agents from autoremove groups and update counts.
 
-        Params:
-        -------
-        machine_index: index of the state machine to run; if None
-          (call from CompartProcessManager), all state machines
-          associated with current group manager are run, in
-          sequence. To avoid multiple calls, super().evolve() is run
-          only if machine_index is None or 0
-
-        This parameter was introduced to run processes in the order specified in the YAML file
-
         """
         if machine_index is None or machine_index == 0:
             super().evolve()
             self.new_population = []
         if self.statevars._is_active:
+            # self.new_population = []
             l_state_machines = [self.l_state_machines[machine_index]] if machine_index is not None else self.l_state_machines
-            for machine in l_state_machines:
-                self.evolve_states(machine=machine)
+            for machine in l_state_machines:  #self.l_state_machines:
+                if isinstance(machine, StateMachine):
+                    self.evolve_states(machine=machine)
+########################## ORGANIZATION PART
+                    # debuginfo("CALL ->", self.statevars.step, "-", machine.machine_name)
+                    # debuginfo(self.model.organization_model.dict_sm_org)
+
+                    # if the machine is in the list of machine linked to an organization
+                    # execute organization processes for all organizations linked to this machine
+                    if machine.machine_name in self.model.organization_model.dict_sm_org:
+                        # debuginfo("BUFFER")
+                        # for manager in self.model.organization_model.dict_sm_org[machine.machine_name]:
+                        #     # move temporarily in the buffer_out of each atomic space
+                        #     manager.to_buffer()
+                        for manager in self.model.organization_model.dict_sm_org[machine.machine_name]:
+                            # allocate in real location
+                            manager.organization_processes.execute_processes(self)
+
+                    self._host.make_all_consistent()
+########################## END ORGANIZATION PART
                 for key, comp in self._content.items():
                     if comp.autoremove:
                         agents_or_population = comp.get_content()
                         ## removing populations in compartment-based models applies
                         ## to 'MASTER' grouping
                         if agents_or_population[0] == 'population':
                             agents_or_population = (
                               agents_or_population[0],
                               { key: agents_or_population[1] }
                               )
                         self._host.remove(agents_or_population)
+######################## ORGANIZATION PART
+                        if self.model.has_organization:
+                            self.model.organization_model.remove_units(agents_or_population)
+                            # !!!!!!! WARNING DEL !!!!!!!!!!!
+                            # del agents_or_population
+######################## END ORGANIZATION PART
                 self.update_counts()
+
         for comp in self._content.values():
-            # debuginfo(self.statevars.step, comp.statevars.step)
             comp.shift_times_to_exit()
 
+        # debuginfo("EVOLVE", self.statevars)
+
     def evolve_states(self, machine):
         """Ask each group to make its content evolve according
         to its current state and the specified state_machine.
 
         List *l_productions* contains tuples (target, {'population': qty}, None)
         or (target, {'agents': list}, prototype), representing individuals
         produced by `productions` edges in the state machine, and to be added to
@@ -214,28 +252,39 @@
         l_productions = self._evolve_productions(machine)
         # apply changes due to transitions for this state machine
         self.apply_changes(d_transitions, machine)
         # add newly created individuals into the list of new populations
         if any(l_productions):
             self.new_population += l_productions
 
+        # debuginfo("-------------!!!!!!!!!!!!!!!!!------------!!!!!!!!!!!!!!------------------")
+        # if machine.machine_name in self.model.organization_model.dict_sm_org:
+        #     for manager in self.model.organization_model.dict_sm_org[machine.machine_name]:
+        #         debuginfo(manager, "->", manager.list_check_last)
+
     def _evolve_transitions(self, machine):
+#######################ORGANIZATION PART
+        # if "key_variables" in self.statevars:
+        #     # debuginfo("YEP")
+        #     return self.model.organization_model.evolve_transitions(self, machine)
+######################END ORGANIZATION PART
         # init empty dictionary for all changes to perform
         future = OrderedDict()
         # iterate over all compartments
         for name, compart in self._content.items():
             future[name] = []
             # compute the current population of each source compartment
             current_pop = compart.get_information('population')
             # no action if current pop <= 0
             if current_pop <= 0:
                 continue
             # compute all possible transitions from the current state
             current_state = compart.get_information(machine.machine_name)
             # execute actions on stay for current state
+            # debuginfo(machine.machine_name, current_state)
             compart.do_state_actions('on_stay', machine, current_state.name, **dict([compart.get_content()]))
             # get the possible transitions from the current state
             # i.e. a list of tuples (state, flux, value, cond_result,
             # actions) where:
             # - state is a possible state reachable from the current state
             # - flux is either 'rate' or 'proba' or 'amount' or 'amount-all-but'
             # - value is the corresponding rate or probability or amount
@@ -261,16 +310,18 @@
                 #
                 values, method = self._compute_values_for_unique_population(
                     values, flux, ref_pop, compart.stochastic)
                 change_list = compart.next_states(states,
                                                   values,
                                                   [ref_pop],
                                                   actions, method=method)
+
                 future[name] += rewrite_keys(name, name.index(current_state),
                                               change_list)
+
         return future
 
 
     def _evolve_productions(self, machine):
         # init empty list for all changes to perform
         future = []
         # iterate over all compartments
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/ibm_process_manager.py` & `emulsion-1.3b1/src/emulsion/agent/managers/ibm_process_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 import numpy                     as np
 import pandas                    as pd
 
 from   emulsion.tools.misc       import select_random, add_all_relative_population_getters
 from   emulsion.tools.getters    import create_counter_getter, create_atoms_aggregator
 
-from   emulsion.tools.debug      import debuginfo
+
 
 from   emulsion.agent.managers.multi_process_manager  import  MultiProcessManager
 
 
 #  _____ ____  __  __ _____
 # |_   _|  _ \|  \/  |  __ \
 #   | | | |_) | \  / | |__) | __ ___   ___ ___  ___ ___
@@ -222,61 +222,39 @@
                 for process_name, grouping in d_process.items():
                     # iterate over items of the dict which should contain only one key:value prepair
                     if process_name in self.model.state_machines:
                         l_state_machines.append(self.model.state_machines[process_name])
         return set(l_state_machines)
 
     def evolve(self, **others):
-        """Make the ProcessManager evolve, i.e. all the registered processes
-        in order, starting with the evolution of the sublevels, and
-        followed by the evolution inherited from superclasses.
+        """Make the agent evolve and update counts based on sub-level
+        agents.
 
         """
         # prepair creation of new agents
         self.new_agents.clear()
-
+        #super().evolve(**others)
         if self.statevars._is_active:
             for process in self:
-                # debuginfo("Evolving", process, self.statevars.step, process.statevars.step)
                 process.evolve()
             for name, process in self._content.items():
-                # debuginfo(name, process)
                 if name not in self.no_compart:
-                    # debuginfo('>'*20)
-                    # debuginfo(process, process.new_population)
                     self.add_new_population(process.new_population)
                     process.update_counts()
         super()._super_evolve(**others)
 
         ## handle autoremove states
         if self.statevars._is_active:
             to_remove = []
             for machine_name, state in self.autoremove_states:
                 to_remove += self.select_atoms(machine_name, value=state)
             self.remove_atoms(set(to_remove))
             self.add_new_population(self.new_agents)
             self.update_counts()
 
-    # def evolve(self, **others):
-    #     """Make the agent evolve and update counts based on sub-level
-    #     agents.
-
-    #     """
-    #     # prepair creation of new agents
-    #     self.new_agents.clear()
-    #     super().evolve(**others)
-    #     ## handle autoremove states
-    #     if self.statevars._is_active:
-    #         to_remove = []
-    #         for machine_name, state in self.autoremove_states:
-    #             to_remove += self.select_atoms(machine_name, value=state)
-    #         self.remove_atoms(set(to_remove))
-    #         self.add_new_population(self.new_agents)
-    #         self.update_counts()
-
     @property
     def counts(self):
         """Return a pandas DataFrame containing counts of each process if
         existing.
 
         """
         res = {}
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/metapop_process_manager.py` & `emulsion-1.3b1/src/emulsion/agent/managers/metapop_process_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 from   collections               import OrderedDict
 
 import pandas                    as pd
 
 
 from   emulsion.agent.managers.multi_process_manager  import  MultiProcessManager
+from   emulsion.tools.debug                           import debuginfo
 
 #  __  __      _
 # |  \/  |    | |
 # | \  / | ___| |_ __ _ _ __   ___  _ __
 # | |\/| |/ _ \ __/ _` | '_ \ / _ \| '_ \
 # | |  | |  __/ || (_| | |_) | (_) | |_) |
 # |_|  |_|\___|\__\__,_| .__/ \___/| .__/
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/managers/multi_process_manager.py` & `emulsion-1.3b1/src/emulsion/agent/managers/multi_process_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,17 +61,19 @@
 from   emulsion.agent.exceptions import LevelException
 from   emulsion.agent.views      import AdaptiveView
 from   emulsion.tools.misc       import load_class, select_random,\
     add_all_test_properties, add_all_relative_population_getters, AGENTS
 from   emulsion.tools.debug      import debuginfo
 from   emulsion.model.exceptions import SemanticException
 
+
 from   emulsion.agent.managers.group_manager  import  GroupManager
 from   emulsion.agent.managers.abstract_process_manager  import  AbstractProcessManager
 
+from   emulsion.tools.debug      import debuginfo
 
 #  __  __       _ _   _ _____
 # |  \/  |     | | | (_)  __ \
 # | \  / |_   _| | |_ _| |__) | __ ___   ___ ___  ___ ___
 # | |\/| | | | | | __| |  ___/ '__/ _ \ / __/ _ \/ __/ __|
 # | |  | | |_| | | |_| | |   | | | (_) | (_|  __/\__ \__ \
 # |_|  |_|\__,_|_|\__|_|_|   |_|  \___/ \___\___||___/___/
@@ -95,15 +97,16 @@
 
     """
     def __init__(self, model=None, level=None, **others):
         view_class, options = load_class(
             **model.levels[level]['super']['master']
         )
         master = view_class(keys='MASTER', host=self, recursive=True, **options)
-        super().__init__(model=model, master=master, level=level, **others)
+        super().__init__(model=model,master=master, level=level, **others)
+        # debuginfo("CREATE HERE", self.model.organization_model, self)
 
     def init_processes(self):
         """Init the processes that the CompartProcessManager will undergo during each
         time step, in order. In a compartment-based process manager, processes may be either:
 
         - method processes based on the execution of the specified method name in a Python add-on
         - state-machine driven processes based on the direct execution of a state machine at the population level
@@ -122,14 +125,15 @@
 
         """
         # a list of tuples (process name, order) for state machine and
         # method processes order can be None otherwise (processes
         # running a state machine on a grouping) order is the index of
         # the state machine to run
         self.l_processes = []
+        # debuginfo("INIT_PROCESS")
         ## TODO: dispatch in sub-classes
         ## 1 - in current level, search for possible method/statemachine processes
         if self.level in self.model.processes:
             # iterate over all process names defined at this level
             for d_process in self.model.processes[self.level]:
                 ## TODO: CHECK
                 process_name, grouping = list(d_process.items())[0]
@@ -142,147 +146,195 @@
                     self.add_method_process(process_name)
                     self.l_processes.append((process_name, None))
 
         ## 2 - in sublevels, search for possible grouping processes
         sublevel = self.get_default_sublevel()
         ## store groupings that are created for real
         self.l_nonsubstituted_groupings = []
+        # debuginfo("model processes", self.model.processes)
         if sublevel in self.model.processes:
             # iterate over all process names defined at sublevel
             for d_process in self.model.processes[sublevel]:
                 # debuginfo("sublevel:", sublevel, " -- d_process:", d_process)
                 # get key and value from a dict which contains only one key...
                 process_name, grouping = list(d_process.items())[0]
                 if process_name not in self.model.state_machines:
                     ## TODO: CHECK
-                    # this must be a method process at the sublevel => ignore
+                    # this should be a method process at the sublevel
                     continue
                 if grouping == 'MASTER':
                     raise SemanticException('Unconsistent grouping MASTER used for level {} with process {} (do not associate processes with special grouping "MASTER" in hybrid models)'.format(sublevel, process_name))
                 if grouping is None:
                     ## TODO: CHECK
-                    # this must be a state machine process at the sublevel => ignore
+                    # this should be a state machine process at the sublevel
                     continue
                 ## add a compart process associated with the MASTER grouping
                 compart_properties = dict(
                     self.model.compartments[self.level][grouping])
-                # debuginfo("compart_properties:", compart_properties)
                 for keyword in ['compart_manager', 'compart_class']:
                     if keyword in compart_properties:
                         class_desc = compart_properties[keyword]
                         compart_properties[keyword] = load_class(**class_desc)
-                # debuginfo(self.level, process_name, grouping, self.model.substitution_dict[self.level])
+
                 if any(compart_properties['state_machines']):
-                    # debuginfo(process_name, '->', compart_properties['state_machines'])
+################## ORGANIZATION PART
+                    for k in compart_properties['key_variables']:
+                        if k in self.model.organization_model.dict_level:
+                            # debuginfo("----------->", k)
+                            self.add_compart_process(grouping, **compart_properties)
+################## END ORGANIZATION PART
+                    # debuginfo("1 --", grouping, ' --> ', compart_properties)
                     self.add_compart_process(grouping, **compart_properties)
                     group_manager = self[grouping]
-                    machine_names = [machine.machine_name for machine in group_manager.l_state_machines]
-                    # debuginfo(process_name, machine_names)
+                    # machine_names = [machine.machine_name for machine in group_manager.l_state_machines]
+                    machine_names = []
+                    for machine in group_manager.l_state_machines:
+                        if isinstance(machine, str):
+                            machine_names.append(machine)
+                        else:
+                            machine_names.append(machine.machine_name)
                     index = machine_names.index(process_name)
                     self.l_processes.append((grouping, index))
                     self.l_nonsubstituted_groupings.append(grouping)
+                    # debuginfo(process_name, '-->', index)
                 else:
                     # process operating on a virtual grouping -> substitute true grouping
+
                     substitution_grouping = self.model.substitution_dict[self.level][grouping]
                     compart_properties = dict(
                         self.model.compartments[self.level][substitution_grouping])
                     machine_names = compart_properties['state_machines']
                     # debuginfo(process_name, machine_names)
                     index = machine_names.index(process_name)
                     self.l_processes.append((substitution_grouping, index))
-
-
+                    # debuginfo(process_name, '-->', index)
 
             self.add_relative_counts()
 
-        # debuginfo('PROCESSES:', self.l_processes)
-
-        ## EXPERIMENTAL - replaced by callable class in the model
-        # ## ADD is_X and duration_in_machine properties for state
-        # ## machines used as StateMachineProcesses for the current
-        # ## population
-        # add_all_test_properties(self)
+        ## ADD is_X and duration_in_machine properties for state
+        ## machines used as StateMachineProcesses for the current
+        ## population
+        add_all_test_properties(self)
 
     def add_relative_counts(self):
         ## once all 'real' groupings are created, add getters for relative population counts (e.g. 'total_my_species_other_health_state')
+        # debuginfo("ADD_RELATIVE_COUNTS -> compartments", self.model.compartments[self.level])
         for grouping_name in self.model.compartments[self.level]:
+            subst_grouping = None
             if grouping_name in self.l_nonsubstituted_groupings:
-                continue
-            compart_properties = dict(
-                self.model.compartments[self.level][grouping_name])
-            t_key_variables = compart_properties['key_variables']
-            ## only add automatically generated variables
-            subst_grouping = self.model.substitution_dict[self.level][grouping_name]
-            # debuginfo("===>", self.model.substitution_dict, '-->', grouping_name)
+                # debuginfo("NON_substituted", self.l_nonsubstituted_groupings)
+                # debuginfo(self.model.substitution_dict)
+                # debuginfo(self.model._description["grouping"])
+                compart_properties = dict(self.model.compartments[self.level][grouping_name])
+                t_key_variables = compart_properties['key_variables']
+                subst_grouping = grouping_name
+                # raise
+                # continue
+            else:
+                compart_properties = dict(
+                    self.model.compartments[self.level][grouping_name])
+                # debuginfo(grouping_name)
+                t_key_variables = compart_properties['key_variables']
+                ## only add automatically generated variables
+                # debuginfo(self.model.substitution_dict)
+                # raise
+                if grouping_name in self.model.substitution_dict[self.level]:
+                    subst_grouping = self.model.substitution_dict[self.level][grouping_name]
+                else:
+                    debuginfo('The grouping name', grouping_name, 'not exists or is not linked to a process')
+                    debuginfo('Please check that the GROUPING exists')
+                    raise Exception('GROUPING NAME ERROR')
+                # debuginfo("===>", self.model.substitution_dict, '-->', grouping_name, "<====>", subst_grouping)
+                # raise
             ## total_X_Y
-            # debuginfo('####', [key in self.model.state_machines for key in t_key_variables])
-            if len(t_key_variables) > 1 and all(key in self.model.state_machines for key in t_key_variables):
-                self.create_properties_for_groups(self.model.substitution_dict[self.level][grouping_name], t_key_variables)
-            # dynamically add properties for relative counts in compart_class instances
-            # debuginfo(self[subst_grouping].keys)
-            init_key = tuple([None] * len(self[subst_grouping].keys))    #l_state_machines))
-            # debuginfo(init_key, '-', subst_grouping, '-', [machine.machine_name for machine in self[subst_grouping].l_state_machines], '-', t_key_variables)
+################## ORGANIZATION PART
+            # create an imaginary upper concept of state machines and organizations  called <<states_process>>
+            self.all_states_process = dict(self.model.state_machines, **self.model.organization_model.dict_level)
+            # old version (only state machines
+            # if len(t_key_variables) > 1 and all(key in self.model.state_machines for key in t_key_variables):
+            #     self.create_properties_for_groups(self.model.substitution_dict[self.level][grouping_name], t_key_variables)
+            # # dynamically add properties for relative counts in compart_class instances
+            # init_key = tuple([None] * len(self[subst_grouping].l_state_machines))
+            # substituated by :
+            # debuginfo(self.all_states_process)
+
+            # debuginfo("all_states\t", self.all_states_process)
+            if len(t_key_variables) > 0 and\
+              all(key in self.all_states_process for key in t_key_variables):
+                # debuginfo("CREATE PROPERTIES", subst_grouping, "WITH", t_key_variables)
+                self.create_properties_for_groups(subst_grouping, t_key_variables)
+                # debuginfo("CREATE PROPERTIES", self.model.substitution_dict[self.level][grouping_name], "WITH", t_key_variables)
+                # self.create_properties_for_groups(self.model.substitution_dict[self.level][grouping_name], t_key_variables)
+
+            # init_key = tuple([None] * len(self.all_states_process))
+            #debuginfo(self[subst_grouping]._content, self[subst_grouping].l_state_machines)
+            init_key = tuple([None] * len(self[subst_grouping].keys))
+            # debuginfo('INIT KEY', init_key)
+
+################# END ORGANIZATION PART
+            # debuginfo(grouping_name, init_key, t_key_variables, subst_grouping)
+            # debuginfo(self._content["s_o_s"].l_state_machines)
+
+            # debuginfo("T_KEY_VARIABLES", t_key_variables)
+
             add_all_relative_population_getters(self[subst_grouping][init_key], t_key_variables)
             for variable_name in t_key_variables:
+                # debuginfo("CREATE GETTER FOR", variable_name)
                 add_all_relative_population_getters(self[subst_grouping][init_key], (variable_name,))
 
 
-
     def add_compart_process(self,
                             process_name,
                             key_variables,
                             compart_manager=(GroupManager, {}),
                             state_machines=[],
                             compart_class=(AdaptiveView, {})):
-        # debuginfo("Adding compart process", process_name, key_variables, state_machines)
+        # debuginfo("ADD COMPART PROCESS", process_name)
         if process_name not in self._content:
             super().add_compart_process(process_name, key_variables, compart_manager=compart_manager, state_machines=state_machines, compart_class=compart_class)
 
 
     def evolve(self, **others):
         """Make the ProcessManager evolve, i.e. all the registered processes
         in order, starting with the evolution of the sublevels, and
         followed by the evolution inherited from superclasses.
 
         """
         if self.statevars._is_active:
-            # for process in self:
-            #     process.evolve()
             self['MASTER'].evolve()
             # debuginfo(self.l_processes)
             for process_or_grouping, index in self.l_processes:
                 process = self[process_or_grouping]
                 if index is None:
-                    # debuginfo("Normal evolution", process_or_grouping, '->', process)
                     process.evolve()
                 else:
-                    # debuginfo("Grouping evolution", process_or_grouping, '->', process, 'SM:', process.l_state_machines[index].machine_name)
-                    process.evolve(index)
+                   process.evolve(index)
             for name, process in self._content.items():
                 if name not in self.no_compart:
-                    # debuginfo('>'*20)
-                    # debuginfo(process, process.new_population)
                     self.add_new_population(process.new_population)
                     process.update_counts()
         super().evolve(**others)
 
     def _super_evolve(self, **others):
-        """Trick for providing subclass a direct access to upper class"""
         super().evolve(**others)
 
+
     def apply_initial_conditions(self):
         """Initialize level with initial conditions specified in the model.
 
         As this agent is aimed at managing individuals in the
         sub-levels, only 'prototypes' are taken into account to
         initialize the sub-levels.
 
         """
-        if self.level in self.model.initial_conditions:
+
+########## HERE TO DEFINE NEW ATOMS !! ############
+        if self.level in self.model.initial_conditions: # and (self.level != "population" and not self.model.has_organisation):
             conds = self.model.initial_conditions[self.level]
+
             for l_protos, qty, l_probas in conds:
                 l_proba_values = [self.get_model_value(p) for p in l_probas]
                 total_value = sum(l_proba_values)
                 if not (0 <= total_value <= 1):
                     raise SemanticException('When building initial conditions for level {}, inconsistent sum of probabilities for prototypes {}, amount {}, probas {}={}'.format(self.level, l_protos, qty, l_probas, l_proba_values))
                 ## if sum of probas < 1 add complement (even if
                 ## proba_values same size as protos) to ensure that
@@ -332,17 +384,16 @@
             prototype = self.model.get_prototype(sublevel, proto, self.get_information('simu_id'))
             prototype[var.machine_name] = val
             to_add = [ self.new_atom(custom_prototype=prototype, execute_actions=False)
                        for _ in range(int(amount)) ]
             # for atom in to_add:
             #     atom.change_state(var, val)
             new_atoms += to_add
-        self.add_atoms(new_atoms)
-        for agent in new_atoms:
-            agent.reapply_prototype(execute_actions=True)
+
+            self.add_atoms(new_atoms)
 
     def select_atoms(self, variable=None, state=None, value=None, process=None):
         """Return a list of atoms selected by specific *value* or *state* of a
         *variable*.
 
         Parameters
         ----------
@@ -413,29 +464,28 @@
 
         """
         if sublevel is None:
             sublevel = self.get_default_sublevel()
         atom_class = self.get_agent_class_for_sublevel(sublevel)
         args.update(model=self.model, simu_id=self.statevars.simu_id,
                     level=sublevel, step=self.statevars.step)
+
         if prototype is not None:
             args.update(prototype=prototype, execute_actions=execute_actions)
         elif custom_prototype is not None:
             args.update(custom_prototype=custom_prototype, execute_actions=execute_actions)
         args['simulation'] = self.simulation
         # args['host'] = self['MASTER']
         new_atom = atom_class(**args)
+
         # initialize MASTER host
         new_atom.add_host(self['MASTER'])
         # maybe to fix strange bugs (step shift for newly introduced populations in metapops ?)
         new_atom.statevars.step = self.statevars.step
-
-        ## EXPERIMENTAL - replaced by callable class in the model
-        # add_all_test_properties(new_atom)
-
+        add_all_test_properties(new_atom)
         # for name, comp in self._content.items():
         #     if name not in self.no_compart:
         #         add_all_relative_population_getters(new_atom, comp.keys)
 
         new_atom.apply_initial_prototype(name=prototype, prototype=custom_prototype,
                                          execute_actions=execute_actions)
         return new_atom
@@ -470,14 +520,15 @@
             for state, atoms in agents_to_init.items():
                 for action in self.model.init_actions[machine][state]:
                     action.execute_action(self['MASTER'], agents=atoms)
 
         # add atoms to appropriate compartments and make them
         # consistent
         for name, comp in self._content.items():
+            # debuginfo(name, comp)
             if name not in self.no_compart:
                 default_key = tuple(None for _ in comp.keys)
                 comp[default_key].add(atom_set)
                 self.make_consistent(comp)
                 if init:
                     comp.update_counts()
 
@@ -508,17 +559,17 @@
         self.remove(self['MASTER'].get_content())
         self.statevars.population = 0
 
     def remove_atoms(self, atom_set):
         """Remove the specified atoms from the current
         MultiProcessManager. Atoms are removed from each of the
         compartment managers (including the 'MASTER' set).
-
         """
         for atom in list(atom_set):
+
             for host in list(atom._host.values()):
                 host.remove([atom])
         self.statevars.population = len(self['MASTER']._content)
 
     def select_randomly(self, proba=0, amount=None, process=None):
         """Select randomly chosen atoms from this ProcessManager. `proba` can
         be either a probability or a dictionary. In that case, the
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/meta.py` & `emulsion-1.3b1/src/emulsion/agent/meta.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/agent/process.py` & `emulsion-1.3b1/src/emulsion/agent/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 #     limitations under the License.
 
 
 from   abc                       import abstractmethod
 import numpy                     as np
 
 from   emulsion.tools.misc       import rates_to_probabilities, aggregate_probabilities, count_population
-from   emulsion.model.exceptions import SemanticException
+from   emulsion.tools.debug      import debuginfo
 
 class AbstractProcess(object):
     """An AbstractProcess is aimed at controlling a specific activity
     in a compartment, and is identified by its name.
 
     """
     def __init__(self, name):
```

### Comparing `emulsion-1.2rc5/src/emulsion/agent/views.py` & `emulsion-1.3b1/src/emulsion/agent/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 from   sortedcontainers          import SortedSet
 
 from   emulsion.agent.core       import Aggregation
 from   emulsion.tools.misc       import select_random, AGENTS
 from   emulsion.model.exceptions import SemanticException
 from   emulsion.tools.debug      import debuginfo
 
+from   emulsion.tools.debug      import debuginfo
+
 #   _____ _                 _   __      ___
 #  / ____(_)               | |  \ \    / (_)
 # | (___  _ _ __ ___  _ __ | | __\ \  / / _  _____      __
 #  \___ \| | '_ ` _ \| '_ \| |/ _ \ \/ / | |/ _ \ \ /\ / /
 #  ____) | | | | | | | |_) | |  __/\  /  | |  __/\ V  V /
 # |_____/|_|_| |_| |_| .__/|_|\___| \/   |_|\___| \_/\_/
 #                    | |
@@ -129,15 +131,20 @@
                 # restart with proportions instead
                 return self.next_states(states,
                                         tuple(v / total_value for v in values) + (0,),
                                         populations, actions, method=None)
             evolution = [int(v) for v in values]
         else:
             # values is expected to be the number of output edges + 1
-            evolution = np.random.multinomial(len(origin), values)[:-1]
+            try:
+                evolution = np.random.multinomial(len(origin), values)[:-1]
+            except Exception as e:
+                debuginfo('ERROR')
+                debuginfo(states, '--', values)
+                raise
 
         ### now select agents corresponding to the amounts
         # init change list
         changes = []
         # track agents already selected
         modified = SortedSet()
         for state, qty, act in zip(states[:-1], evolution, actions[:-1]):
@@ -179,15 +186,14 @@
 
         """
         super().__init__(**others)
         self.statevars.observables = observables
         for (observable, value) in zip(observables, values):
             self.statevars[observable] = value
 
-
     def evaluate_condition(self, condition):
         """Return the population of the compartment if the condition
         is fulfilled, 0 otherwise.
 
         """
         if not callable(condition):
             return self.get_content() if condition else ()
@@ -248,14 +254,18 @@
         changed their value(s) of the compartment-specific
         observable(s). The corresponding units are reported to the
         upper level.
 
         """
         super().evolve(machine=machine)
         if self.statevars._is_active:
+            # if self.statevars.step < 7:
+            #     debuginfo('-'*100)
+            #     debuginfo("Evolve Check", self.statevars)
+            #     debuginfo(self._content)
             self.check_consistency()
 
     def check_consistency(self):
         """Check the value of the observables of the current
         compartment. Units which do not have the expected values are
         notified to the upper level.
 
@@ -263,18 +273,29 @@
         # intruders = [unit for unit in self
         #              if any(unit.get_information(observable)\
         #                       != self.statevars[observable]
         #                     for observable in self.statevars.observables)]
         intruders = SortedSet()
         for unit in self:
             for observable in self.statevars.observables:
+                # if unit.statevars.step > 7:
+                #     raise
+                #     debuginfo("STEP", unit.statevars.step)
+                    # debuginfo(unit, "-->", observable)
+                    # debuginfo(unit.get_information(observable), '->', self.statevars[observable])
                 if unit.get_information(observable) != self.statevars[observable]:
                     intruders.add(unit)
+                    # debuginfo("INTRUDERS ->", unit)
+                    # debuginfo("        ", self.statevars, " \n\tfor", unit.statevars)
                     break
         if intruders:
+            # for e in intruders:
+            #     debuginfo(e, "->", e.get_information("space").keys)
+            # debuginfo("IINNTTRRUUDDEERRSS", intruders, self._host, "-->", self.statevars.step)
+            # print("*"*100)
             self._host.notify_changed_units(self, intruders)
 
     def clone(self, **others):
         """Make a copy of the current compartment with the specified
         observable/value settings. The new content is empty.
 
         """
@@ -315,15 +336,19 @@
 
     def __iter__(self):
         # use a copy of values to allow for modifications during the time step
         return list(self._content.values()).__iter__()
 
     def __getitem__(self, name):
         if name not in self._content: # DEBUG: should not happen !
-            print(name)
+            debuginfo('The grouping name "', name, '" not exists or is not linked to a process')
+            debuginfo('Please check that the GROUPING exists')
+            debuginfo('    This error can occur when the keys of the corresponding GROUPING are misspelled')
+
+            raise Exception('GROUPING NAME ERROR')
         return self._content[name]
 
     def get_content(self):
         """Return the agents contained in the current view.
 
         """
         # raise SemanticException('WARNING, should not enter here (get_content of a StructuredView) !!!')
@@ -343,67 +368,93 @@
 
     def remove(self, population):
         """Remove the specified population from the current
         compartment.  The population is expected to be a dictionary
         with names as keys and compartments as values.
 
         """
+        debuginfo(population)
+        raise
         for key, pop in population.items():
             if key in self._content:
                 self._content[key].remove(pop._content)
 
     def notify_changed_units(self, source_compartment, units):
         """Receive a change notification concerning several units
         which cannot be stored anymore in the source compartment.
 
         """
+        # debuginfo(self, "___________________",source_compartment,  source_compartment.statevars, units)
+################ ORGANIZATION PART
+        # ????
+        self.model.organization_model.add_units(units)
+################ END ORGANIZATION PART
         if source_compartment in self._notifications:
             self._notifications[source_compartment] |= units
         else:
             self._notifications[source_compartment] = SortedSet(units)
 
     def handle_notifications(self):
         """Handle all notifications received during the time step."""
+        # debuginfo("HANDLE ->",self, self.keys, self.statevars.step)
+        # debuginfo(self._notifications)
         for source_compartment, units in self._notifications.items():
+            # debuginfo("COMP :", source_compartment, source_compartment.statevars)
             source_observables = source_compartment.statevars.observables
             new_pop = {}
  #           pop_values = {}
             for unit in units:
+                # debuginfo("HANDLE NOT\n\t", source_observables)
                 key = tuple(unit.get_information(k) for k in source_observables)
+                # debuginfo("\t", key)
                 if key not in new_pop:
+                    # debuginfo("\t\t unit in new_pop")
                     new_pop[key] = [unit]
 #                    pop_values[key] = unit.get_information(source_observable)
                 else:
                     new_pop[key].append(unit)
             for key, unit in new_pop.items():
+                # debuginfo("source_orbservable :", source_observables, key)
+                # debuginfo("CALL from here ->", key)
                 new_comp = self.get_or_build(key, source=source_compartment)
+                # debuginfo("Moving to:", new_comp)
+                # debuginfo('Moving to:', new_comp.keys, '\n\t', unit)
                 source_compartment.move_to(new_comp, agents=unit)
         self._notifications.clear()
+        # debuginfo("CLEAR -->", self, self._content)
 
     def get_or_build(self, key, source=None):
         """Return the compartment with the specified key if any, or
         build one by cloning the source if not found.
 
         """
+
+        # debuginfo("KKKKEEYYY", key, self, source)
         if key not in self._content:
+            # debuginfo("create adaptive ->")
             key_infos = dict(zip(self.keys, key))
+            # debuginfo('    key_infos', key_infos)
             # create a new compartment (Compartment or AdaptiveView) from the specified source
             new_compart = source.clone(host=self, **key_infos)
+            # debuginfo(new_compart.statevars)
             new_compart.keys = key
             # if any key for compart is a state marked "autoremove",
             # then the whole compart is marked "autoremove"
             new_compart.autoremove = any(hasattr(value, 'state_machine') and\
                                   value.state_machine.get_property(value.name, 'autoremove')
                                   for value in key)
             self.add({key: new_compart})
+            # raise Exception(self)
+            # debuginfo(new_compart)
         return self[key]
 
     def evolve(self, machine=None):
         super().evolve(machine=machine)
         if self.statevars._is_active:
+            # debuginfo("EVOLVE -> HANDLE -> PB ->", self)
             self.handle_notifications()
 
 
 
 
 class StructuredViewWithCounts(StructuredView):
     """Same as StructuredView, plus the capability of handling counts for
```

### Comparing `emulsion-1.2rc5/src/emulsion/init_emulsion.py` & `emulsion-1.3b1/src/emulsion/init_emulsion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 #!/usr/bin/env python3
 
 
 # EMULSION (Epidemiological Multi-Level Simulation framework)
 # ===========================================================
 # 
 # Contributors and contact:
@@ -45,43 +46,43 @@
 # 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
+import os
 from   pathlib    import Path
 from   shutil     import copy
 
 from   colorama   import Style
 import emulsion
 
-
-COMMAND = 'source $HOME/.emulsionrc/emulsion-bash-completion.sh'
-# CPATH = 'export PYTHONPATH=$PYTHONPATH:.'
+COMMAND = 'source $HOME/.emulsionrc/emulsion-completion.sh'
+CPATH = 'export PYTHONPATH=$PYTHONPATH:.'
 
 def main():
     # retrieve $HOME and path to EMULSION repository
     parts = Path(emulsion.__file__).parts[:-1] + ("scripts",)
     HOMEDIR = Path.home()
     EMULSION_SCRIPTS = Path(*parts)
     EMULSION_RC = Path(HOMEDIR, '.emulsionrc')
     # create .emulsionrc
     print("Creating $HOME/.emulsionrc with EMULSION init files")
     EMULSION_RC.mkdir(exist_ok=True)
-    # copy emulsion-bash-completion.sh
-    copy(str(Path(EMULSION_SCRIPTS, 'emulsion-bash-completion.sh')),
+    # copy emulsion-completion.sh
+    copy(str(Path(EMULSION_SCRIPTS, 'emulsion-completion.sh')),
          str(EMULSION_RC))
     # change .bashrc
     print("Adding initialization instructions to $HOME/.bashrc")
     with open(Path(HOMEDIR, '.bashrc'), 'a') as f:
         f.write("\n# init EMULSION completion\n")
         f.write(COMMAND + "\n")
-        # f.write("\n# update PYTHONPATH to allow importing local modules\n")
-        # f.write(CPATH + "\n")
+        f.write("\n# update PYTHONPATH to allow importing local modules\n")
+        f.write(CPATH + "\n")
 
     print("Initialization finished.")
     print(Style.BRIGHT + """
     To allow completion for EMULSION in current shell, type:
     source $HOME/.bashrc
     """ + Style.RESET_ALL)
```

### Comparing `emulsion-1.2rc5/src/emulsion/model/__init__.py` & `emulsion-1.3b1/src/emulsion/model/__init__.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/model/emulsion_model.py` & `emulsion-1.3b1/src/emulsion/model/emulsion_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,58 +56,59 @@
 
 
 from   pathlib                 import Path
 from   datetime                import datetime, timedelta
 from   copy                    import deepcopy
 
 import yaml
+import numpy                   as     np
 import dateutil.parser         as     dup
 
 from   sympy                   import sympify, Symbol
 
 from   collections             import OrderedDict
 from   sortedcontainers        import SortedSet, SortedDict
 from   jinja2                  import Environment, PackageLoader
 
 import networkx                as     nx
 
 from   emulsion.tools.state    import StateVarDict
 from   emulsion.tools.misc     import read_csv_prototypes, read_from_file, load_class
-from emulsion.tools.getters import create_new_serial, create_weighted_random, \
-    create_successor_getter, create_predecessor_getter, \
-    make_random_prototype_getter, make_generator_prototype_getter, create_state_indexer, create_my_state_indexer, \
-    create_lazy_ternary, create_lazy_AND, create_lazy_OR, create_duration_getter, create_state_tester
+from   emulsion.tools.getters  import create_new_serial, create_weighted_random,\
+    create_successor_getter, create_predecessor_getter,\
+    make_random_prototype_getter, make_generator_prototype_getter
 from   emulsion.tools.calendar import EventCalendar
 from   emulsion.tools.debug    import debuginfo
 
 from   emulsion.model.functions      import DEFAULT_LEVEL_INFO, DEFAULT_GROUPING_INFO, AGGREG_COMP, AGGREG_HYBRID, AGGREG_METAPOP, AGGREG_IBM, make_function, make_CSV_function, make_when_condition, make_statevar_getter, make_model_value_getter
 from   emulsion.model.exceptions     import SemanticException
 from   emulsion.model.state_machines import StateMachine
 
+from   emulsion.tools.debug          import debuginfo
+
 #  ______                 _     _             __  __           _      _
 # |  ____|               | |   (_)           |  \/  |         | |    | |
 # | |__   _ __ ___  _   _| |___ _  ___  _ __ | \  / | ___   __| | ___| |
 # |  __| | '_ ` _ \| | | | / __| |/ _ \| '_ \| |\/| |/ _ \ / _` |/ _ \ |
 # | |____| | | | | | |_| | \__ \ | (_) | | | | |  | | (_) | (_| |  __/ |
 # |______|_| |_| |_|\__,_|_|___/_|\___/|_| |_|_|  |_|\___/ \__,_|\___|_|
 
-
 class EmulsionModel(object):
     """Class in charge of the description of a multi-level
     epidemiological model. Such models are composed of several
     processes which may take place at different
     organization/observation levels. Some of those processes are
     reified through a function implemented within an agent, while
     others are represented by a state machine. The model is also in
     charge of handling symbolic expressions and pre-computing their
     values, e.g. concerning parameters, transmission functions,
     etc.
 
     """
-    def __init__(self, filename=None, description=None, input_dir=None, changed_values=None):
+    def __init__(self, filename=None, description=None, input_dir=None, changed_values=None, simulation=None):
         """Instantiate the model either from a configuration file or from a
         string. Both must contain a YAML-based description of the model.
 
         Parameters
         ----------
         filename: str
             the path to the YAML file to read
@@ -115,20 +116,49 @@
             a YAML description of the model
         input_dir: Path
             the path to the directory where additional data files can be found if needed (default: 'data')
         changed_values: dict
             changes if parameter values, if any, specified by command-line option '-p' or '--param'
 
         """
-        self.input_dir = input_dir
+# ORGANIZATION PART ---------------------
+        self.simulation = simulation
         self.filename = filename
-        model_description = read_from_file(filename) if self.filename is not None else description
+        self.description = description
+
+        self.input_dir = input_dir
+
+        self.has_organization = False
+        # if filename:
+        #     self.filename = filename
+        #     self.parse(read_from_file(filename))
+        # else:
+        #     self.filename = None
+        #     self.parse(description)
+
+    # def run_parse(self):
+        # if self.filename:
+        #     self.parse(read_from_file(self.filename))
+        # else:
+        #     self.parse(self.description)
+
+        #self.input_dir = input_dir
+        #self.filename = filename
+        self.model_description = read_from_file(filename) if self.filename is not None else description
+        # if changed_values is not None:
+        #     self.model_description = self.change_parameter_values(self.model_description, changed_values)
+
+    def run_parse(self, input_dir=None, changed_values=None):
         if changed_values is not None:
-            model_description = self.change_parameter_values(model_description, changed_values)
-        self.parse(model_description)
+            self.model_description = self.change_parameter_values(self.model_description, changed_values)
+        self.parse(self.model_description)
+
+    def set_simulation(self, simulation):
+        self.simulation = simulation
+# --------------------------------------
 
 
     def __repr__(self):
         return '%s "%s"' % (self.__class__.__name__, self.model_name)
 
     def normalize_format(self):
         """Return a YAML representation of the model, reformatted to to print
@@ -143,15 +173,15 @@
         """Return a copy of object (naif method).
         TODO: Find a way to avoid recharging compartment class when
         intentiate a MultiProcessManager class with a old model.
 
         """
         return deepcopy(self)
 
-    def _reset_all(self):
+    def _reset_all(self, org=True):
         # namespace for all symbols used in the model
         # dict string -> sympy symbol
         self._namespace = {}
         # namespace for calendar periods in the model
         # dict string -> sympy symbol
         self._event_namespace = {}
         # cache for all expressions encountered in the model
@@ -211,14 +241,23 @@
         self.initial_conditions = {}
         # dict of enumerate types used in special variables
         self.types = {}
         # dict of all states existing in state machines
         self.states = StateVarDict()
         # dict of parameters to log when explicitly changed
         self.params_to_log = StateVarDict()
+# ORGANIZATION_PART-----------
+        self.has_organization = False
+        if org:
+            # dict of organizations
+            self.dict_organizations = {"all": {}, "root": {}}
+            self.has_organization = True
+            # organization_model
+            # self.organization_model = None
+# ----------------------------
         # dict of data-based parameters {level -> {filename -> (key variables, parameter names)}}
         self.databased_parameters = {}
         # set of parameters associated with a level-specific value
         # CRUCIAL ROLE in get_information mechanisms (subsumes others)
         self.parameters_by_level = set()
 
 
@@ -267,14 +306,21 @@
         try:
             return self._values[name]
         except KeyError:
             try:
                 return float(sympify(name, locals=self._namespace))
             except TypeError:
                 ### cases of string parameters ?
+################### ORGANIZATION PART
+                if name in self.organization_model.dict_space:
+                    # debuginfo(name)
+                    # debuginfo("!! pass here !!")
+                    # debuginfo(self.organization_model.dict_space[name])
+                    return self.organization_model.dict_space[name]
+################### END ORGANIZATION PART
                 return name
                 # result = sympify(name, locals=self._namespace)
                 # import sys
                 # sys.exit(-1)
 
     def change_parameter_values(self, description, d_changes):
         """Naive method to change several parameter values at the same time.
@@ -345,28 +391,57 @@
         self.build_distributions()
         # parse processes
         self.build_processes()
         # parse compartment description
         self.build_compartment_desc()
         # parse state machines
         self.build_state_machines()
+# ORGANIZATION_PART-----------
+        # parse organizations
+        self.build_organizations()
+# ----------------------------
         # parse prototypes
         self.build_prototypes()
         # parse initial_conditions
         self.build_initial_conds()
+# ORGANIZATION PART-----------
+        # # create atomic space as population
+        # self.create_atomic_population()
+        # self.associate_org_pop()
+# ----------------------------
         # parse actions
         self.build_actions()
         # # calculate expressions from parameters
         # self.calculate_compound_params()
         # replace expressions by values or lambdas
         self.compute_values()
         self._description['parameters']['delta_t'] = {
             'desc': 'duration of the simulation time step',
             'value': self.delta_t
-        }
+            }
+
+
+# ORGANIZATION_PART-----------
+    def build_organizations(self):
+        if "organizations" in self._description:
+            self.organization_model.parse()
+
+    # def create_atomic_population(self):
+    #     if "organizations" in self._description:
+    #         self.organization_model.build_initial_metapop()
+
+    def get_organization(self, name):
+        return self.dict_organizations["all"][name]
+
+    def get_dict_organizations_root(self):
+        return self.dict_organizations["root"]
+
+    # def associate_org_pop(self):
+    #     self.organization_model.associate_population()
+# ---------------------------
 
     def build_outputs_options(self):
         """Parse the outputs options of the model.
         The agents will treat extra variables for outputs (TODO), and
         the simulation classes will treat period outputs.
 
         Example of YAML specification:
@@ -513,22 +588,16 @@
             value: 0.79
 
         """
         if 'modules' in self._description:
             self.modules += self._description['modules']
         if 'parameters' in self._description:
             for (key, val) in self._description['parameters'].items():
-                # experimental
-                if isinstance(val['value'], dict):
-                    self._values[key] = self.parse_dict(key, val['value'])
-                    self._namespace[key] = Symbol(key)
-                else:
-                    self.parameters[key] = sympify(val['value'], locals=self._namespace)
-
-
+                self.parameters[key] = sympify(val['value'],
+                                               locals=self._namespace)
 
     def build_statevars(self):
         """Parse the description of the model and extract the state
         variables that agents running this model must have.
 
         Example of YAML specification:
         ------------------------------
@@ -593,32 +662,37 @@
             - prototype: [healthy_animal, infected_animal]
               amount: 'init_pop'
               proba: ['1 - init_prevalence', 'init_prevalence']
 
         """
         if 'initial_conditions' in self._description:
             for level, desc in self._description['initial_conditions'].items():
-                self.initial_conditions[level] = []
-                for list_items in desc:
-                    l_protos = list_items['prototype']
-                    if not isinstance(l_protos, list):
-                        l_protos = [l_protos]
-                        list_items['prototype'] = l_protos
-                    amount = list_items['amount']
-                    if 'proba' in list_items:
-                        l_probas = list_items['proba']
-                        if not isinstance(l_probas, list):
-                            l_probas = [l_probas]
-                    else:
-                        l_probas = ['1'] * len(l_protos)
-                    list_items['proba'] = l_probas
-                    if not (0 <= len(l_protos) - len(l_probas) <= 1):
-                        raise SemanticException('In initial conditions: inconsistent numbers of prototypes/probabilities\n\tprototypes: {}, probabilities: {}'.format(l_protos, l_probas))
-                    self.initial_conditions[level].append(
-                        (l_protos, self.add_expression(amount), [self.add_expression(p) for p in l_probas]))
+#####################
+# VERIFY IF NOT ORGANIZATION
+#####################
+                if level != "organizations":
+                    self.initial_conditions[level] = []
+                    for list_items in desc:
+                        l_protos = list_items['prototype']
+                        if not isinstance(l_protos, list):
+                            l_protos = [l_protos]
+                            list_items['prototype'] = l_protos
+                        amount = list_items['amount']
+                        if 'proba' in list_items:
+                            l_probas = list_items['proba']
+                            if not isinstance(l_probas, list):
+                                l_probas = [l_probas]
+                        else:
+                            l_probas = ['1'] * len(l_protos)
+                        list_items['proba'] = l_probas
+                        if not (0 <= len(l_protos) - len(l_probas) <= 1):
+                            raise SemanticException('In initial conditions: inconsistent numbers of prototypes/probabilities\n\tprototypes: {}, probabilities: {}'.format(l_protos, l_probas))
+                        self.initial_conditions[level].append(
+                            (l_protos, self.add_expression(amount), [self.add_expression(p) for p in l_probas]))
+
 
     def build_prototypes(self):
         """Parse the description of the model and extract the list of
         prototypes for each level, either with their value, or with
         the expression to compute them. A prototype is a dictionary of
         the form {statevar: value}..
 
@@ -644,14 +718,22 @@
                 for list_item in prototypes:
                     # read all prototypes for a given level
                     for (key, val) in list_item.items():
                         prototype = OrderedDict()
                         # read all variables for prototype named "key"
                         for variable, value in val.items():
                             result = self.parse_prototype_line(variable, value)
+#################### ORGANIZATION PART
+                            if result is not None and 'init_location' in str(result):
+                                self.organization_model.init_location[key] = result["init_location"]
+                                result = None
+                            if result is not None and 'force_location' in str(result):
+                                self.organization_model.force_location[key] = result["force_location"]
+                                result = None
+################### END ORGANIZAION PART
                             if result is not None:
                                 prototype[variable] = result
                         # test if an ordered affectation is defined:
                         # if so, parse the list of variable
                         # assignation as a list of tuples (name of
                         # variable, value)
                         for keyword in ['begin_with', 'end_with']:
@@ -716,14 +798,15 @@
         and return the resulting value.
 
         """
         if variable in ['desc', 'begin_with', 'end_with', 'file', 'filter', 'select', 'include_values', 'exclude_values']:
             return None
         # default case
         result = value
+        # debuginfo(result)
         if value == 'random':
             result = '_random_' + variable
         elif value == 'default':
             result = '_default_' + variable
         elif value == 'next_state':
             result = '_next_state_' + variable
             # associate to a function that returns the successor of
@@ -745,14 +828,25 @@
         elif type(value) == str and value.startswith('serial'):
             result = '_serial_' + variable
             if value != 'serial' and value[6] == '(' and value[-1] == ')':
                 end = self.add_expression(value[7:-1])
             else:
                 start, end = 0, None
             self._values[result] = create_new_serial(end=end, model=self)
+# ORGANIZATION_PART-----------
+        elif variable == "init_location":
+            return {variable: value}
+        elif variable == "force_organization":
+            return {variable: value}
+        elif type(value) != list and value in self.statevars:
+            self._values[result] = lambda agent: agent.statevars[result]#
+            debuginfo(result, "-->", agent.statevars[result])
+            # elif value in self.statevars:
+            #     self._values[result] = lambda agent: agent.statevars[result]
+# ----------------------------
         elif isinstance(value, list):
             result = tuple(value)
         elif value in self.statevars:
             self._values[result] = make_statevar_getter(result)
         elif value in self.parameters:
             self._values[result] = make_model_value_getter(result)
         elif value not in self.states:
@@ -842,15 +936,14 @@
                         if 'statevars' not in self._description:
                             self._description['statevars'] = {}
                         self._description['statevars'][param_name] = {
                             'desc': param_spec['desc'],
                             'source': filename
                         }
         for level in self.databased_parameters:
-            # debuginfo(level)
             for filename, desc in self.databased_parameters[level].items():
                 key_variables, l_params = desc
                 # debuginfo('\t', filename, ':', key_variables, '->', l_params)
 
     def build_levels(self):
         """Parse the description of different level of simulations.
         Most of time, there are tree differents levels:
@@ -956,14 +1049,15 @@
                     for agg_desc in desc['aggregate_vars']:
                         newvar = agg_desc['name']
                         sourcevar = agg_desc['collect']
                         oper = agg_desc['operator'] if 'operator' in agg_desc else 'sum'
                         self.aggregate_vars[level].append((newvar, sourcevar, oper))
 
     def get_agent_class_for_level(self, level):
+        #debuginfo("get", level)
         return load_class(module=self.levels[level]['module'],
                           class_name=self.levels[level]['class_name'])
 
     def build_processes(self):
         """Parse the description of the model and retrieve the list of
         processes with different level.
 
@@ -997,14 +1091,15 @@
                         l_processes.append(process_name)
                 self._description['grouping'][level]['MASTER'] = l_processes
                 ## rewrite list of processes as a list {process_name: grouping}
                 ## where grouping is set to None for processes defined in python add-ons
                 self.processes[sublevel] = [{name: None}
                                             if name not in l_processes else {name: 'MASTER'}
                                             for name in self.processes[sublevel]]
+            # debuginfo(level, self.levels)
         # create a dict to associate each state machine to the appropriate level
         self.statemachines_by_level = {level: [] for level in self.levels}
         for level, l_processes in self.processes.items():
             l_d_processes = []
             for process in l_processes:
                 if isinstance(process, dict):
                     l_d_processes.append(process)
@@ -1021,60 +1116,38 @@
         """Rapidly inspect the name of state machines and of their states to
         pre-register automatically built statevars.
 
         """
         if 'state_machines' in self._description:
             for machine_name, description in self._description['state_machines'].items():
                 self.state_machines[machine_name] = None # to build later
-
-                prop_name = 'duration_in_{}'.format(machine_name)
                 desc = "duration elapsed (time units) in current {} state".format(machine_name)
+                prop_name = 'duration_in_{}'.format(machine_name)
                 # self._description['statevars'][prop_name] = {'desc': desc}
                 self.statevars[prop_name] = {'desc': desc}
                 self._description['statevars'][prop_name] = {'desc': desc}
                 self._namespace[prop_name] = Symbol(prop_name)
-                self._values[prop_name] = create_duration_getter(machine_name)
-
-                prop_name = '_time_entered_{}'.format(machine_name)
                 desc = "time step when agent entered current {} state".format(machine_name)
+                prop_name = '_time_entered_{}'.format(machine_name)
                 self.statevars[prop_name] = {'desc': desc}
                 self._description['statevars'][prop_name] = {'desc': desc}
                 self._namespace[prop_name] = Symbol(prop_name)
-
-                prop_name = '_time_to_exit_{}'.format(machine_name)
                 desc = "time step after which agent is allowed to leave current {} state".format(machine_name)
+                prop_name = '_time_to_exit_{}'.format(machine_name)
                 self.statevars[prop_name] = {'desc': desc}
                 self._description['statevars'][prop_name] = {'desc': desc}
                 self._namespace[prop_name] = Symbol(prop_name)
-
-                desc = "Numeric value associated to current state of state machine {}".format(machine_name)
-                prop_name = 'index_my_{}'.format(machine_name)
-                self._description['statevars'][prop_name] = {'desc': desc}
-                self.statevars[prop_name] = desc
-                self._values[prop_name] = create_my_state_indexer(machine_name)
-                self._namespace[prop_name] = Symbol(prop_name)
-
                 for statedict in description['states']:
                     for state_name in statedict:
-                        ## define "is_X"
                         desc = "Test if {} = {}".format(machine_name, state_name)
                         prop_name = 'is_{}'.format(state_name)
                         self._description['statevars'][prop_name] = {'desc': desc}
                         # self.statevars[prop_name] = desc
                         self._namespace[prop_name] = Symbol(prop_name)
-                        self._values[prop_name] = create_state_tester(state_name)
 
-                        ## same for "index_X"
-                        desc = "Return numeric value of state {} in state machine {}".format(state_name, machine_name)
-                        prop_name = 'index_{}'.format(state_name)
-                        self._description['statevars'][prop_name] = {'desc': desc}
-                        # self.statevars[prop_name] = desc
-                        self._namespace[prop_name] = Symbol(prop_name)
-                        self._values[prop_name] = create_state_indexer(state_name)
-                        
 
     def build_state_machines(self):
         """Parse the description of the model and build all the
         required state machines.
 
         """
         if 'state_machines' in self._description:
@@ -1083,78 +1156,80 @@
                 for level, l_machines in self.statemachines_by_level.items():
                     ## ASSUMING THAT A STATE MACHINE IS USED BY ONLY ONE LEVEL !!!
                     if machine_name in l_machines:
                         level_of_machine = level
                         break
                 if level_of_machine is None:
                     raise SemanticException('Statemachine {} is associated with no level!'.format(machine_name))
-                ## ASSUMING THAT EACH LEVEL HAS AT MOST UPPER LEVEL
-                l_upper_levels = list(self.levels_graph.predecessors(level_of_machine))
-                if any(l_upper_levels):
-                    upper_level = l_upper_levels[0]
-                    aggregation_type = self.levels[upper_level]['aggregation_type']
-                else:
-                    aggregation_type = 'hybrid'
+                ## ASSUMING THAT EACH LEVEL HAS ONLY ONE UPPER LEVEL
+                # debuginfo(list(self.levels_graph.predecessors(level_of_machine)))
+                upper_level = list(self.levels_graph.predecessors(level_of_machine))[0]
+                aggregation_type = self.levels[upper_level]['aggregation_type']
                 self.state_machines[machine_name] = StateMachine(machine_name, description, self, aggregation_type)
 
     def build_compartment_desc(self):
         """Inspect the `grouping` part of the model (if any) in order to store
         the corresponding information.
 
         """
         # create a graph for grouping nesting
         grouping_graphs = { level_name: nx.DiGraph() for level_name in self.levels }
         # susbtitution grouping -> most detailed sub-grouping
         self.substitution_dict = { level_name: {} for level_name in self.levels }
         self.compartments = self._description['grouping'] if 'grouping' in self._description else {}
+        # debuginfo(self.compartments)
         for level in self.levels:
             if level not in self.compartments:
                 self.compartments[level] = {}
             if 'aggregation_type' in self.levels[level]:
                 agg_type = self.levels[level]['aggregation_type']
                 if len(self.compartments[level]) == 0:
                     continue
                 for grouping_name, desc in self.compartments[level].items():
+                    # debuginfo("desc ->", desc)
                     grouping_info = {'key_variables': desc, 'state_machines': []}
                     if agg_type in DEFAULT_GROUPING_INFO:
-
                     # raise SemanticException('Unsupported aggregation_type: {}'.format(agg_type))
                         default = DEFAULT_GROUPING_INFO[agg_type]
                         if 'compart_manager' not in grouping_info:
                             grouping_info['compart_manager'] = default['compart_manager'] if  'state_machines' in grouping_info else default['fallback_view']
                         if 'compart_class' not in grouping_info:
                             grouping_info['compart_class'] = default['compart_class']
                     self.compartments[level][grouping_name] = grouping_info
+                # debuginfo(self.compartments)
 
                 ## identify nesting between groupings
                 for grouping_name1 in self.compartments[level]:
                     grouping_graphs[level].add_node(grouping_name1)
                     for grouping_name2 in self.compartments[level]:
                         if grouping_name1 == grouping_name2:
                             continue
                         key1 = self.compartments[level][grouping_name1]['key_variables']
                         key2 = self.compartments[level][grouping_name2]['key_variables']
                         if set(key1) == set(key2):
                             raise SemanticException('Two groupings with same variables (not allowed): {} and {} (keep only one of them)'.format(grouping_name1, grouping_name2))
                         if set(key1) < set(key2):
                             grouping_graphs[level].add_edge(grouping_name1, grouping_name2)
         # compute substitution in groupings: e.g. if a grouping on var x and a grouping on variables x, y, z exist, the first one must be kept only to define total_X, but state machines must operate only on the grouping based on x, y, z
+
+            # debuginfo(self.compartments)
             leaf_groupings = [grouping_name for grouping_name in grouping_graphs[level].nodes() if grouping_graphs[level].out_degree(grouping_name)==0 and grouping_graphs[level].in_degree(grouping_name)>=1]
             self.substitution_dict[level] = {grouping_name: substitution for substitution in leaf_groupings for grouping_name in grouping_graphs[level].nodes() if grouping_name in nx.ancestors(grouping_graphs[level], substitution)}
         # rewrite grouping section to add relevant state machines
         for level in self.processes:
             for process in self.processes[level]:
                 for process_name, grouping in process.items():
                     if grouping is not None:
                         ## add current process_name to state_machines in groupings
                         for upper_level in self.levels_graph.predecessors(level):
                             ## if any substitution, do it !
                             grouping_name = self.substitution_dict[upper_level][grouping] if grouping in self.substitution_dict[upper_level] else grouping
                             self.compartments[upper_level][grouping_name]['state_machines'].append(process_name)
 
+        # debuginfo(self.compartments)
 
     def get_sublevels(self, level_name):
         """Return the list of sublevels of the given *level_name*"""
         return list(self.levels_graph.successors(level_name))
 
 
     # def calculate_compound_params(self):
@@ -1184,110 +1259,30 @@
         attributes.
 
         """
         ### WARNING: expand_expressions should iterate over all
         ### expressions at the same time (halting when no change
         ### occurs) instead of iterating over each expression one by
         ### one
-
-        # experimental
-        # if isinstance(expression, dict):
-        #     return self.parse_if(expression)
-
         result = sympify(expression, locals=self._namespace)
         expr = result
+        if expr is None:
+            debuginfo("ERROR expression to parse is None")
+            raise
         symbs = {s: self.parameters[s.name]
                  for s in expr.free_symbols
                  if s.name in self.parameters}
         while symbs:
             result = expr.subs(symbs)
             expr = sympify(result, locals=self._namespace)
             symbs = {s: self.parameters[s.name]
                      for s in expr.free_symbols
                      if s.name in self.parameters}
         return result
 
-    # experimental
-    def parse_dict(self, param_name, expression_dict):
-        if 'if' in expression_dict:
-            return self.parse_if(param_name, expression_dict)
-        if 'or' in expression_dict:
-            return self.parse_or(param_name, expression_dict)
-        if 'and' in expression_dict:
-            return self.parse_and(param_name, expression_dict)
-        raise SemanticException('Unknown expression for parameter {}:\n\t{}'.format(param_name, expression_dict))
-
-    # experimental
-    def parse_if(self, param_name, expression_dict):
-        if 'then' not in expression_dict:
-            raise SemanticException('THEN clause missing in expression {}'.format(expression_dict))
-        if 'else' not in expression_dict:
-            raise SemanticException('ELSE clause missing in expression {}'.format(expression_dict))
-
-        cond = expression_dict['if']
-        if_true = expression_dict['then']
-        if_false = expression_dict['else']
-
-        if isinstance(cond, dict):
-            val_cond = self.parse_dict(param_name, cond)
-            self._values[str(cond)] = val_cond
-        else:
-            val_cond = self.add_expression(str(cond))
-
-        if isinstance(if_true, dict):
-            val_true = self.parse_dict(param_name, if_true)
-            self._values[str(if_true)] = val_true
-        else:
-            val_true = self.add_expression(str(if_true))
-
-        if isinstance(if_false, dict):
-            val_false = self.parse_dict(param_name, if_false)
-            self._values[str(if_false)] = val_false
-        else:
-            val_false = self.add_expression(str(if_false))
-
-        return create_lazy_ternary(str(cond), str(if_true), str(if_false))
-
-    # experimental
-    def parse_or(self, param_name, expression_dict):
-        l_conditions = expression_dict['or']
-        if not isinstance(l_conditions, list):
-            raise SemanticException('"or:" clause must be followed by a list, found instead: {}'.format(l_conditions))
-
-        l_expressions = []
-        for condition in l_conditions:
-            if isinstance(condition, dict):
-                val_cond = self.parse_dict(param_name, condition)
-                self._values[str(condition)] = val_cond
-                l_expressions.append(condition)
-            else:
-                val_cond = self.add_expression(str(condition))
-                l_expressions.append(str(val_cond))
-
-        return create_lazy_OR(l_expressions)
-
-    # experimental
-    def parse_and(self, param_name, expression_dict):
-        l_conditions = expression_dict['and']
-        if not isinstance(l_conditions, list):
-            raise SemanticException('"and:" clause must be followed by a list, found instead: {}'.format(l_conditions))
-
-        l_expressions = []
-        for condition in l_conditions:
-            if isinstance(condition, dict):
-                val_cond = self.parse_dict(param_name, condition)
-                self._values[str(condition)] = val_cond
-                l_expressions.append(str(condition))
-            else:
-                val_cond = self.add_expression(str(condition))
-                l_expressions.append(str(val_cond))
-
-        return create_lazy_AND(l_expressions)
-
-
     def build_actions(self):
         """Parse the description of the model and extract the actions
         that agents must have.
 
         Example of YAML specification:
         ------------------------------
         actions:
@@ -1306,28 +1301,23 @@
         compound parameters, expressions corresponding to numbers are
         converted to float values, while other expressions are
         replaced by a function.
 
         """
         # collect 'true' values in the parameters
         for (param, expression) in self.parameters.items():
-            # # experimental
-            # if isinstance(expression, dict):
-            #     self._values[param] = create_lazy_ternary(expression['if'], expression['then'], expression['else'])
-            #     continue
+            if expression is None:
+                debuginfo("ERROR parameters value:", param, "is", expression)
+                raise
             value = self.expand_expression(expression)
             try:
                 self._values[param] = float(value)
             except:
                 self._values[param] = make_function(value, modules=self.modules)
         for (param, expression) in self._expressions.items():
-            # # experimental
-            # if isinstance(expression, dict):
-            #     self._values[param] = create_lazy_ternary(expression['if'], expression['then'], expression['else'])
-            #     continue
             value = self.expand_expression(expression)
             ## DO NOT REALLOCATE EXPRESSIONS ALREADY COMPUTED AS CALLABLE OBJECTS --- NOR STATEVARS !!!
             ## (introduced to support data-based parameters)
             if param in self._values and callable(self._values[param]):
                 debuginfo(param, 'from EXPRESSIONS has value', self._values[param], 'instead of', value)
                 continue
             if param in self.statevars:
@@ -1343,14 +1333,15 @@
         #             for symb in expression.free_symbols]):
         #         self._values[cond] = make_function(value, dtype=bool, modules=self.modules)
         #     else:
         #         self._values[cond] = bool(value)
         for (statename, state) in self.states.items():
             self._values[statename] = state
 
+
     def get_modifiable_parameters(self):
         """Return a dictionary containing all true parameters with their
         value.
 
         """
         d_true_params =  {p: self.get_value(p)
                         for p in self.parameters
```

### Comparing `emulsion-1.2rc5/src/emulsion/model/exceptions.py` & `emulsion-1.3b1/src/emulsion/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/model/functions.py` & `emulsion-1.3b1/src/emulsion/model/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,28 @@
 # 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
+import sys
 from   sympy                   import sympify, lambdify, Symbol
 # BEWARE: using lambdify, by default And and Or fall back to numpy's
 # *binary* operators, so that more than 3 conditions linked by And or
 # Or trigger a TypeError ('return arrays must be of ArrayType')
 # see topic addressed there:
 # https://stackoverflow.com/questions/42045906/typeerror-return-arrays-must-be-of-arraytype-using-lambdify-of-sympy-in-python
 # To avoid problems, please use AND / OR (fully in UPPERCASE) instead
 # of And / Or (Capitalized) in the conditions of Emulsion models
 
 from   emulsion.tools.misc     import load_module
-from   emulsion.tools.debug    import debuginfo
+
+from   emulsion.tools.debug          import debuginfo
+
 
 #  ______                _   _
 # |  ____|              | | (_)
 # | |__ _   _ _ __   ___| |_ _  ___  _ __  ___
 # |  __| | | | '_ \ / __| __| |/ _ \| '_ \/ __|
 # | |  | |_| | | | | (__| |_| | (_) | | | \__ \
 # |_|   \__,_|_| |_|\___|\__|_|\___/|_| |_|___/
@@ -85,14 +88,15 @@
 EDGE_KEYWORDS = ['rate', 'proba', 'amount', 'amount-all-but']
 
 ### NAMES OF AGGREGATION types
 AGGREG_IBM = 'IBM'
 AGGREG_COMP = 'compartment'
 AGGREG_HYBRID = 'hybrid'
 AGGREG_METAPOP = 'metapopulation'
+AGGREG_ORGANIZATION = 'organization'
 
 ### INFORMATION TO ADD TO LEVEL DESCRIPTION WHEN USING aggregation_type
 DEFAULT_LEVEL_INFO = {
     AGGREG_IBM: {
         'level': {
             'class_name': 'IBMProcessManager',
             'module': 'emulsion.agent.managers',
@@ -129,14 +133,27 @@
             'master': {
                 'module': 'emulsion.agent.views',
                 'class_name': 'AutoStructuredView',
                 'options': {'key_variable': 'population_id'}
             }
         },
     },
+#>>>>>>>>>>>>>>>>>ORGANIZATION PART
+    AGGREG_ORGANIZATION: {
+        'level': {
+            'module': 'emulsion.organization.managers',
+            'class_name': 'OrganizationProcessManager',
+            'master': {
+                'module': 'emulsion.organization.views',
+                'class_name': 'OrganizationAutoStructuredView',
+                'options': {'key_variable': 'population_id'}
+            }
+        },
+    },
+#ORGANIZATION PART<<<<<<<<<<<<<<<<<<<<<<
 }
 
 ### INFORMATION TO ADD TO GROUPING DESCRIPTION WHEN USING aggregation_type
 DEFAULT_GROUPING_INFO = {
     AGGREG_HYBRID: {
         'compart_manager': {
             'module': 'emulsion.agent.managers',
@@ -187,22 +204,62 @@
 
         Returns
         -------
         class:
             a callable which can be called on an agent
 
         """
+        self.expression = expression
+
         self.symbs = tuple(expression.free_symbols)
         self.dtype = dtype
         mods = [load_module(m) for m in modules]
         self.lambdified = lambdify(self.symbs, expression, modules=mods)
 
     def __call__(self, agent):
-        vals = [float(agent.get_information(str(s))) for s in self.symbs]
-        return self.dtype(self.lambdified(*vals))
+        # debuginfo("call")
+        for s in self.symbs:
+            try:
+                r = agent.get_information(str(s))
+                if r is None:
+                    debuginfo('-->', r, s, 'in', agent)
+            except RecursionError as err:
+                debuginfo("Maximum recursion depth exceed")
+                debuginfo("\t -> Check if '", str(s), "' exists")
+        try:
+            vals = [float(agent.get_information(str(s))) for s in self.symbs]
+        except Exception:
+            debuginfo('ERROR')
+            debuginfo('Symbs list to call', self.symbs, agent)
+            for s in self.symbs:
+                r = agent.get_information(str(s))
+                if r is None:
+                    debuginfo('The key "', s, '" not exists in', agent)
+                    # debuginfo(agent._content)
+                    # debuginfo(agent.statevars)
+                    debuginfo('MAYBE:')
+                    if 'observables' in agent.statevars:
+                        debuginfo('   the GROUPING', agent.statevars['observables'], 'not exist')
+                        debuginfo('or')
+                    debuginfo('   the key "', s, '" is misspelled')
+            debuginfo("Grouping", str(s), "not exists")
+            raise Exception('KEY GROUPING ERROR', str(s))
+
+
+        try:
+             return self.dtype(self.lambdified(*vals))
+        except Exception:
+            debuginfo("Cannot lambdified expression:")
+            debuginfo(self.expression)
+            for s in self.symbs:
+                debuginfo('    ',s, ' -->', agent.get_information(str(s)))
+
+            raise Exception('LAMBDIFIED ERROR')
+
+        # return self.dtype(self.lambdified(*vals))
 
 class make_CSV_function:
     def __init__(self, expression, modules=['numpy', 'numpy.random', 'math', 'sympy']):
         """Transform the specified sympy expression into a callable class
         which can be called on a CSV line. The transformation uses
         sympy function ``lambdify`` for better performances, with the
         specified modules.
```

### Comparing `emulsion-1.2rc5/src/emulsion/model/state_machines.py` & `emulsion-1.3b1/src/emulsion/model/state_machines.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,16 +60,14 @@
 from   collections             import Counter
 
 import numpy                   as     np
 from   sympy                   import sympify
 
 from   sortedcontainers        import SortedSet
 
-import pydot
-
 import emulsion.tools.graph    as     enx
 from   emulsion.agent.action   import AbstractAction
 from   emulsion.tools.state    import StateVarDict, EmulsionEnum
 
 from   emulsion.model.functions import AGGREG_COMP, ACTION_SYMBOL, WHEN_SYMBOL, ESCAPE_SYMBOL,\
     COND_SYMBOL, CROSS_SYMBOL, EDGE_KEYWORDS, CLOCK_SYMBOL,\
     make_when_condition, make_duration_condition, make_duration_init_action
@@ -434,14 +432,56 @@
         if 'when' in edge_desc:
             expression = sympify(edge_desc['when'],
                                  locals=self.model._event_namespace)
             edge_desc['when'] = str(expression)
             self.model._values[str(expression)] = make_when_condition(
                 expression, modules=self.model.modules)
 
+    # def _parse_conditions_durations(self, from_, edge_desc):
+    #     """Parse the edge description in search for durations,
+    #     escapement and conditions specifications. Durations
+    #     ('duration' clause )are handled as an additional condition
+    #     (agents entering the state are given a 'time to live' in the
+    #     state, then they are not allowed to leave the state until
+    #     their stay reaches that value). Escapements ('escape' clause)
+    #     are also translated as a condition, allowing the agent to
+    #     leave the state when the expression is true, only while the
+    #     stay duration is below its nominal value.
+    #
+    #     """
+    #     cond, escape = None, False
+    #     if 'cond' in edge_desc:
+    #         cond = edge_desc['cond']
+    #     if 'escape' in edge_desc:
+    #         cond = edge_desc['escape']
+    #         escape = True
+    #     if cond is not None:
+    #         ### WARNING the operation below is not completely
+    #         ### safe... it is done to replace conditions of the form
+    #         ### 'x == y' by 'Eq(x, y)', but it is a simple
+    #         ### substitution instead of parsing the syntax
+    #         ### tree... Thus it is *highly* recommended to express
+    #         ### conditions directly with Eq(x, y)
+    #         if '==' in str(cond):
+    #             cond = 'Eq({})'.format(','.join(cond.split('==')))
+    #             # edge_desc['label'] = ', '.join(edge_desc.values()) if
+    #     # duration specified for this state, handle it as an
+    #     # additional condition
+    #     if 'duration' in self._statedesc[from_]:
+    #         duration_cond = make_duration_condition(self.model, self.machine_name)
+    #         if cond is None:
+    #             cond = duration_cond
+    #         elif escape:
+    #             cond = 'AND(Not({}),{})'.format(duration_cond, cond)
+    #         else:
+    #             cond = 'AND({},{})'.format(duration_cond, cond)
+    #         edge_desc['cond'] = cond
+    #     if cond is not None:
+    #         # self.model.conditions[cond] = sympify(cond, locals=self.model._namespace)
+    #         self.model._expressions[cond] = sympify(cond, locals=self.model._namespace)
 
     def build_actions(self):
         """Parse the description of the state machine and extract the
         actions that agents running this state machine must have.
 
         Example of YAML specification:
         ------------------------------
@@ -517,14 +557,17 @@
             self.state_actions[name] = {}
         l_actions = self._parse_action_list(actions)
         self.state_actions[name][event] = l_actions
 
     def _parse_action_list(self, actions):
         """Parse the list of actions associated with a state."""
         l_actions = []
+        if actions is None:
+            debuginfo("actions is None")
+            raise Exception("action cannot be None")
         for d_action in actions:
             if 'action' in d_action:
                 action = d_action['action']
                 l_params = [self.model.add_expression(expr)
                             for expr in d_action['l_params']]\
                                 if 'l_params' in d_action\
                                 else []
@@ -598,14 +641,31 @@
                         l_actions.append(
                             AbstractAction.build_action(
                                 keyword,
                                 parameter=d_action[keyword]
                             )
                         )
                         understood = True
+######################## ORGANIZATION PART
+                for keyword in ['deposit']:
+                    if keyword in d_action:
+                        information = d_action[keyword]['information']
+                        target = d_action[keyword]['target']
+                        value = d_action[keyword]['value']
+                        l_actions.append(
+                            AbstractAction.build_action(
+                                keyword,
+                                information = information,
+                                target = target,
+                                value = value,
+                                model = self.model
+                            )
+                        )
+                        understood = True
+######################## END ORGANIZATION PART
                 if not understood:
                     raise SemanticException('ERROR !!!! action {} not understood'.format(d_action))
         return l_actions
 
 
 
 
@@ -622,41 +682,57 @@
 
     def write_dot(self, filename, view_actions=True):
         """Write the graph of the current state machine in the
         specified filename, according to the dot/graphviz format.
 
         """
 
-        dot_graph = pydot.Dot(self.machine_name, graph_type="digraph", rankdir="LR" if self.graph.edges() else "TB", charset="utf-8")
-        dot_graph.set_node_defaults(fontsize=16, fontname="Arial", shape="box", style='"filled,rounded"')
-        dot_graph.set_edge_defaults(minlen=1.5, penwidth=1.5, tailtooltip="", headtooltip="")
+        rankdir = "LR" if self.graph.edges() else "TB"
+        output = '''digraph {
+          charset="utf-8"
+        '''
+        output += '''\trankdir={};
+        '''.format(rankdir)
+        output += '''
+        \tnode[fontsize=16, fontname=Arial, shape=box, style="filled,rounded"];
+        \tedge[minlen=1.5, fontname=Times, penwidth=1.5, tailtooltip="", headtooltip=""];
 
+        '''
         for state in self.states:
             name = state.name
             name_lab = name
             if 'duration' in self._statedesc[name]:
                 name_lab += '&nbsp;{}'.format(CLOCK_SYMBOL)
-            shape = "Mrecord"
-            label = name_lab
+            actions = 'shape="Mrecord", label="{}", '.format(name_lab)
             nodestyle = "filled,rounded"
             if state.is_default:
                 nodestyle += ",bold"
             if state.autoremove:
                 nodestyle += ",dotted"
             if view_actions:
                 onenter = ACTION_SYMBOL+'|'\
                           if 'on_enter' in self._statedesc[name] else ''
                 onstay = '|'+ACTION_SYMBOL\
                          if 'on_stay' in self._statedesc[name] else ''
                 onexit = '|'+ACTION_SYMBOL\
                          if 'on_exit' in self._statedesc[name] else ''
                 if onenter or onstay or onexit:
-                    label = "{%s{\ %s\ %s}%s}" % (onenter, name_lab, onstay, onexit)
-            new_node = pydot.Node(name=str(name), shape=shape, label=str(label), tooltip=str(self._statedesc[name]['tooltip']), fillcolor=str(self._statedesc[name]['fillcolor']), style=f'"{nodestyle}"')
-            dot_graph.add_node(new_node)
+                    actions = 'shape="Mrecord", label="{%s{\ %s\ %s}%s}", ' % (
+                        onenter, name_lab, onstay, onexit)
+            output += '\t"{}" [{}tooltip="{}", fillcolor="{}", style="{}"] ;\n'.format(
+                name, actions,
+                self._statedesc[name]['tooltip'],
+                # '\n\tON ENTER: {}'.format(self.state_actions[name]['on_enter'])\
+                # if onenter else '' +\
+                # '\n\tON STAY: {}'.format(self.state_actions[name]['on_stay'])\
+                # if onstay else '' +\
+                # '\n\tON EXIT: {}'.format(self.state_actions[name]['on_exit'])\
+                # if onexit else '',
+                self._statedesc[name]['fillcolor'],
+                nodestyle)
         for from_, to_ in SortedSet(self.graph.edges()):
             for desc in self.graph.edge[from_][to_].values():
                 edgetip = ''
                 tail = 'none'
                 if 'when' in desc:
                     tail += WHEN_SYMBOL
                     edgetip += 'WHEN: {}'.format(desc['when'])
@@ -666,10 +742,15 @@
                 if 'truecond' in desc:
                     tail += COND_SYMBOL
                     edgetip += 'COND: {}'.format(desc['truecond'])
                 head = 'normalnone'
                 if 'on_cross' in desc:
                     head += CROSS_SYMBOL
                     # edgetip += 'ON CROSS: {}\\n'.format(desc['on_cross'])
-                new_edge = pydot.Edge(src=str(from_), dst=str(to_), label=str(desc['label']), labeltooltip=str(desc['labeltooltip']), arrowtail=str(tail), arrowhead=str(head), dir="both", tooltip=str(edgetip), minlen=3, style=str(desc['type_id'].linestyle))
-                dot_graph.add_edge(new_edge)
-        dot_graph.write_raw(filename)
+                output += ('\t"{}" -> "{}" [label="{}", labeltooltip="{}", '
+                           'arrowtail="{}", arrowhead="{}", dir=both, '
+                           'tooltip="{}", minlen=3, style="{}"];\n').format(
+                               from_, to_, desc['label'], desc['labeltooltip'],
+                               tail, head, edgetip, desc['type_id'].linestyle)
+        output += '}'
+        with open(filename, 'w', encoding="utf8") as f:
+            f.write(output)
```

### Comparing `emulsion-1.2rc5/src/emulsion/resources/emulsion.tx` & `emulsion-1.3b1/src/emulsion/resources/emulsion.tx`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/__init__.py` & `emulsion-1.3b1/src/emulsion/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/calendar.py` & `emulsion-1.3b1/src/emulsion/tools/calendar.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/debug.py` & `emulsion-1.3b1/src/emulsion/tools/debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 #[HEADER]
 
 from pathlib  import Path
 from inspect  import getframeinfo, stack
 from colorama import Fore, Back, Style, init
+from emulsion.tools.DebugGlobal import DebugGlobal
 
 init()
 
 def debuginfo(*message, **options):
     """Print debug information.
 
     Can be used in the code as a classical `print`
@@ -41,11 +42,13 @@
         debuginfo('Test finished, logging in file test.log')
 
         with open('test.log', 'a') as out:
             debuginfo('values:', *[i for i in range(10)], sep="-", file=out)
 
 
     """
-    caller = getframeinfo(stack()[1][0])
-    options['end'] = Style.RESET_ALL + '\n'
-    prefix = Style.BRIGHT + Fore.BLACK + Back.YELLOW + "{}:{}>".format(Path(caller.filename).name, caller.lineno) + Back.BLACK + Fore.YELLOW + " "
-    print(prefix, *message, **options)
+    debugglobal = DebugGlobal()
+    if True: # debugglobal.debug:
+        caller = getframeinfo(stack()[1][0])
+        options['end'] = Style.RESET_ALL + '\n'
+        prefix = Style.BRIGHT + Fore.BLACK + Back.YELLOW + "{}:{}>".format(Path(caller.filename).name, caller.lineno) + Back.BLACK + Fore.YELLOW + " "
+        print(prefix, *message, **options)
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/functions.py` & `emulsion-1.3b1/src/emulsion/tools/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 
 import numpy as np
-import sympy as sp
 
+from   emulsion.tools.debug          import debuginfo
 
 def IfThenElse(condition, val_if_true, val_if_false):
     """Ternary conditional function: return either *val_if_true* or
     *val_if_false* depending on *condition*.
 
     Example
     -------
@@ -122,15 +122,14 @@
     Returns
     -------
     bool:
         True if **all** values are True, False otherwise.
     """
     return all(values)
 
-
 def OR(*values):
     """Return a logical OR (disjunction) between all the values.
 
     Example
     -------
     To sell animals depending on either their weight or their age::
 
@@ -149,15 +148,14 @@
     Returns
     -------
     bool:
         True if **at least one** of the values is True, False otherwise.
     """
     return any(values)
 
-
 def MIN(*values):
     """Return the minimum of all values.
 
     Parameters
     ----------
     *values: list
         boolean values separated by commas
@@ -165,15 +163,14 @@
     Returns
     -------
     float:
         the lowest value
     """
     return min(values)
 
-
 def MAX(*values):
     """Return the maximum of all values.
 
     Parameters
     ----------
     *values: list
         boolean values separated by commas
@@ -181,45 +178,35 @@
     Returns
     -------
     float:
         the highest value
     """
     return max(values)
 
-
 def DIV(a, b):
     """Return 0 if a=0 without considering b, otherwise a/b.
 
     Parameters
     ----------
     a, b:
         the values to divide
 
     Returns
     -------
     float:
         0 if a is 0, otherwise a/b
     """
-    return 0 if a == 0 else a/b
-
+    if b == 0 and a != 0:
+        debuginfo("ERROR division by 0, with:")
+        debuginfo("a=", a, " b=", b)
 
-def ROUND(value):
-    """Return the integer rounding of the specified value .
+        raise Exception("ERROR division by 0")
 
-    Parameters
-    ----------
-    value:
-        the value to round
+    return 0 if a == 0 else a/b
 
-    Returns
-    -------
-    float:
-        the 0-digit rounding of *value*
-    """
-    return np.round(value)
 
 #   _____ _                _             _         _
 #  / ____| |              | |           | |       | |
 # | (___ | |__   ___  _ __| |_ ___ _   _| |_ ___  | |_ ___
 #  \___ \| '_ \ / _ \| '__| __/ __| | | | __/ __| | __/ _ \
 #  ____) | | | | (_) | |  | || (__| |_| | |_\__ \ | || (_) |
 # |_____/|_| |_|\___/|_|   \__\___|\__,_|\__|___/  \__\___/
@@ -260,15 +247,14 @@
     int:
         either 1 with probability *proba_success*, or 0 with
         probability 1-*proba_success*
 
     """
     return np.random.binomial(1, proba_success)
 
-
 def random_choice(*values):
     """Return a value chosen randomly among those provided (equiprobable
     sampling).
 
     Example
     -------
     To init ``age`` among three typical values::
@@ -287,15 +273,14 @@
     -------
     val:
         one of the values (equiprobable choice)
 
     """
     return np.random.choice(values)
 
-
 def random_choice_weighted(*values):
     """Return a value chosen randomly among those provided (but not
     equiprobably).
 
     Example
     -------
     To init ``age`` among three typical values which respectively
@@ -319,15 +304,14 @@
     """
     choices_and_values = zip(*[iter(values)]*2)
     choices, weights = zip(*choices_and_values)
     total = sum(weights)
     probas = [w / total for w in weights]
     return np.random.choice(choices, p=probas)
 
-
 def random_multinomial(number_of_samples, *probas):
     """Return a multinomial sample based on the specified probabilities.
 
     Parameters
     ----------
     number_of_samples: int
         number of experiments
@@ -337,15 +321,14 @@
     Returns
     -------
     list:
         the drawn samples
     """
     return list(np.random.multinomial(number_of_samples, probas))
 
-
 def random_uniform(low: float, high: float) -> float:
     """Return a random value drawn from a uniform distribution between
     *low* (inclusive) and *high* (exclusive).
 
     Example
     -------
     In a prototype definition::
@@ -368,15 +351,14 @@
     See also
     --------
     numpy.random.uniform
 
     """
     return np.random.uniform(low, high)
 
-
 def random_integers(low: int, high: int) -> int:
     """Return a random integer value drawn from a discrete uniform
     distribution between *low* and *high* (both inclusive).
 
     Example
     -------
     In a prototype definition::
@@ -398,15 +380,14 @@
 
     See also
     --------
     numpy.random.random_integers
     """
     return np.random.random_integers(low, high)
 
-
 def random_exponential(scale: float) -> float:
     """Return a random value drawn from an exponential distribution of
     rate 1/*scale* (thus of mean *scale*).
 
     Example
     -------
     In a prototype definition::
@@ -427,15 +408,14 @@
     See also
     --------
     numpy.random.exponential
 
     """
     return np.random.exponential(scale)
 
-
 def random_beta(a: float, b: float) -> float:
     """Return a random value drawn from a beta distribution of parameters
     *a* and *b*.
 
     Example
     -------
     In a prototype definition::
@@ -457,15 +437,14 @@
 
     See also
     --------
     numpy.random.beta
     """
     return np.random.beta(a, b)
 
-
 def random_gamma(shape: float, scale: float) -> float:
     """Return a random value drawn from a gamma distribution of parameters
     *shape* and *scale*.
 
     Example
     -------
     In a prototype definition::
@@ -487,15 +466,14 @@
 
     See also
     --------
     numpy.random.gamma
     """
     return np.random.gamma(shape, scale)
 
-
 def random_normal(mn: float, sd: float) -> float:
     """Return a random value drawn from a normal distribution of mean *mn*
     and standard deviation *sd*.
 
     Example
     -------
     In a prototype definition::
@@ -518,14 +496,48 @@
     See also
     --------
     numpy.random.normal
 
     """
     return np.random.normal(mn, sd)
 
+def random_truncated_normal(mn: float, sd: float, minval: float, maxval: float) -> float:
+
+    """Return a random value drawn from a truncated normal distribution of mean *mn*
+    and standard deviation *sd*, with minimum value *minval* and maximum value *maxval*
+
+    Example
+    -------
+    In a prototype definition::
+
+      age: 'random_truncated_normal(100, 5, 5, 90)'
+
+    Parameters
+    ----------
+    mn: float
+        the mean of the normal distribution
+    sd: float, positive (>=0)
+        the standard deviation of the normal distribution
+    minval: float
+        the minimum value of the interval
+    maxval: float
+        the maximum value of the interval
+
+    Returns
+    -------
+    float:
+        a random value sampled according to a truncated normal distribution of
+        mean *mn* and standard deviation *sd*
+
+    See also
+    --------
+    numpy.random.normal and np.clip
+
+    """
+    return np.clip(np.random.normal(mn, sd), minval, maxval)
 
 def random_poisson(lam: float) -> int:
     """Return an integer random value drawn from a Poisson distribution of
     mean *lam*.
 
     Example
     -------
@@ -553,154 +565,25 @@
     --------
     numpy.random.poisson
 
     """
     return np.random.poisson(lam)
 
 
-#   _____ _                _             _         _
-#  / ____| |              | |           | |       | |
-# | (___ | |__   ___  _ __| |_ ___ _   _| |_ ___  | |_ ___
-#  \___ \| '_ \ / _ \| '__| __/ __| | | | __/ __| | __/ _ \
-#  ____) | | | | (_) | |  | || (__| |_| | |_\__ \ | || (_) |
-# |_____/|_| |_|\___/|_|   \__\___|\__,_|\__|___/  \__\___/
-
-#   _____
-#  / ____|
-# | (___  _   _ _ __ ___  _ __  _   _
-#  \___ \| | | | '_ ` _ \| '_ \| | | |
-#  ____) | |_| | | | | | | |_) | |_| |
-# |_____/ \__, |_| |_| |_| .__/ \__, |
-#          __/ |         | |     __/ |
-#         |___/          |_|    |___/
-
-
-def Eq(a, b):
-    """Return 1 if *a* and *b* are equals, 0 otherwise.
-
-    Parameters
-    ----------
-    a, b: float
-        the values to compare
-
-    Returns
-    -------
-    float:
-        1 iff a == b, 0 otherwise
-
-    See also
-    --------
-    sympy.Eq
-
-    """
-    return float(sp.Eq(a, b))
-
-
-def GreaterThan(a, b):
-    """Return 1 if *a* is greater than *b* (or equal), 0 otherwise.
-
-    Parameters
-    ----------
-    a, b: float
-        the values to compare
-
-    Returns
-    -------
-    float:
-        1 iff a >= b, 0 otherwise
-
-    See also
-    --------
-    sympy.Eq
-
-    """
-    return float(sp.GreaterThan(a, b))
-
-
-def StrictGreaterThan(a, b):
-    """Return 1 if *a* is strictly greater than *b*, 0 otherwise.
-
-    Parameters
-    ----------
-    a, b: float
-        the values to compare
-
-    Returns
-    -------
-    float:
-        1 iff a > b, 0 otherwise
-
-    See also
-    --------
-    sympy.Eq
-
-    """
-    return float(sp.StrictGreaterThan(a, b))
-
-
-def LessThan(a, b):
-    """Return 1 if *a* is less than *b* (or equal), 0 otherwise.
-
-    Parameters
-    ----------
-    a, b: float
-        the values to compare
-
-    Returns
-    -------
-    float:
-        1 iff a <= b, 0 otherwise
-
-    See also
-    --------
-    sympy.Eq
-
-    """
-    return float(sp.LessThan(a, b))
-
-
-def StrictLessThan(a, b):
-    """Return 1 if *a* is strictly less than *b*, 0 otherwise.
-
-    Parameters
-    ----------
-    a, b: float
-        the values to compare
-
-    Returns
-    -------
-    float:
-        1 iff a < b, 0 otherwise
-
-    See also
-    --------
-    sympy.Eq
-
-    """
-    return float(sp.StrictLessThan(a, b))
-
-
 IfThenElse.__USER_FUNCTION__ = ['Functions Available for Models']
 AND.__USER_FUNCTION__ = ['Functions Available for Models']
 OR.__USER_FUNCTION__ = ['Functions Available for Models']
 MIN.__USER_FUNCTION__ = ['Functions Available for Models']
 MAX.__USER_FUNCTION__ = ['Functions Available for Models']
 DIV.__USER_FUNCTION__ = ['Functions Available for Models']
-ROUND.__USER_FUNCTION__ = ['Functions Available for Models']
 
 random_bool.__USER_FUNCTION__ = ['Functions Available for Models']
 random_choice.__USER_FUNCTION__ = ['Functions Available for Models']
 random_poisson.__USER_FUNCTION__ = ['Functions Available for Models']
 random_choice_weighted.__USER_FUNCTION__ = ['Functions Available for Models']
 random_uniform.__USER_FUNCTION__ = ['Functions Available for Models']
 random_multinomial.__USER_FUNCTION__ = ['Functions Available for Models']
 random_integers.__USER_FUNCTION__ = ['Functions Available for Models']
 random_exponential.__USER_FUNCTION__ = ['Functions Available for Models']
 random_beta.__USER_FUNCTION__ = ['Functions Available for Models']
 random_gamma.__USER_FUNCTION__ = ['Functions Available for Models']
 random_normal.__USER_FUNCTION__ = ['Functions Available for Models']
-
-Eq.__USER_FUNCTION__ = ['Functions Available for Models']
-GreaterThan.__USER_FUNCTION__ = ['Functions Available for Models']
-StrictGreaterThan.__USER_FUNCTION__ = ['Functions Available for Models']
-LessThan.__USER_FUNCTION__ = ['Functions Available for Models']
-StrictLessThan.__USER_FUNCTION__ = ['Functions Available for Models']
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/getters.py` & `emulsion-1.3b1/src/emulsion/tools/getters.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,23 +51,23 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 
+from   importlib                 import import_module
 from   typing                    import List, Iterable, Tuple, Union, Any
 from   collections               import Counter
-from   functools                 import partial
 import itertools                 as it
 
 import numpy                     as np
 
 import emulsion.tools.functions  as em_func
-from   emulsion.model.exceptions import SemanticException
+from   emulsion.tools.debug      import debuginfo
 
 class create_population_getter:
     def __init__(self, grouping_name: str, t_states: Union[str, Tuple]):
         """Build a callable class used as a getter for property of the form
         ``total_X_Y`` where ``X`` and ``Y`` are states of two
         different states machines used in the grouping *grouping_name*.
 
@@ -90,20 +90,25 @@
             population size for the specified group.
 
         """
         if not isinstance(t_states, tuple):
             t_states = (t_states,)
         self.grouping_name = grouping_name
         self.t_states = t_states
+        # debuginfo("CREATE TOTAL GETTER", grouping_name, t_states, len(t_states))
+
 
     def __call__(self, agent):
+        # debuginfo("0000", self.grouping_name, self.t_states, agent.get_group_population(self.grouping_name, self.t_states))
+
         return agent.get_group_population(self.grouping_name, self.t_states)
 
 class create_relative_population_getter:
     def __init__(self, model, t_variables):
+        # debuginfo("HERE with", model, t_variables)
         """Build a callable class used as a getter for property of the form
         ``total_X_Y`` where ``X`` and ``Y`` are either states of two
         different states machines used in the grouping described by *t_variables*,
         or keywords built upon a state machine name ``M`` of the form ``my_M`` or
         ``other_M``.
 
         The functions can handle groupings with an arbitrary number of
@@ -129,41 +134,71 @@
             population size for the specified group.
 
         """
         if not isinstance(t_variables, tuple):
             t_variables = (t_variables,)
         self.model = model
         self.t_variables = t_variables
+        # debuginfo("T_VARIABLE ::: ", self.t_variables)
 
     def __call__(self, agent):
+        test = True
         # build list of total_X_Y where X, Y are only real states
         l_real_states = []
+        # debuginfo("agent",agent.statevars, self.t_variables)
+        # is_org = False
         for field in self.t_variables:
+            # debuginfo("RELATIVE POPULATION",self, "->", self.t_variables)
             if field.startswith("my_"):
                 machine_name = field[len("my_"):]
-                ## replace e.g. 'my_health_state' by the health_state (string) of the agent, e.g. ['I']
-                l_real_states.append([agent.statevars[machine_name].name])
+                # debuginfo('my', field, machine_name )
+########################## ORGANIZATION PART
+                if machine_name in agent.model.state_machines or machine_name in agent.model.organization_model.dict_level:
+                    ## replace e.g. 'my_health_state' by the health_state (string) of the agent, e.g. ['I']
+                    # debuginfo(machine_name, agent, "-", agent.statevars)
+                    if machine_name in agent.statevars and agent.statevars[machine_name] is not None:
+                        l_real_states.append([agent.statevars[machine_name].name])
+                    else:
+                        test = False
+                        debuginfo('Try to find ', machine_name, ' in \n\t\t', agent.statevars)
+                        raise Exception(machine_name, agent.statevars)
+                        # debuginfo
+######################### END ORGANIZATION PART
             elif field.startswith("other_"):
                 machine_name = field[len("other_"):]
                 agent_state_name = agent.statevars[machine_name].name
                 ## replace e.g. 'other_health_state' by all names of non-autoremove states which are not the agent's state, e.g. ['S', 'R']
                 l_state_names = [state.name
                                for state in self.model.state_machines[machine_name].states
                                if not (state.autoremove or state.name == agent_state_name) ]
                 l_real_states.append(l_state_names)
             else:
                 ## add 'true' state as such
                 l_real_states.append([field])
+                if field in agent.model.organization_model.dict_space:
+                    is_org = True
+                # debuginfo("yep", l_real_states)
         # build list of total_X_Y where X, Y are only real states
         l_combinations = list(it.product(*l_real_states))
-        # get corresponding values in agent
+
+        # debuginfo(['total_{}'.format('_'.join(t_group)) for t_group in l_combinations])
         l_totals = [agent.get_information('total_{}'.format('_'.join(t_group)))
                     for t_group in l_combinations]
+        # debuginfo(agent.keys)
+        # for t_group in l_combinations:
+        #     debuginfo('total_{}'.format('_'.join(t_group)))
         # return the sum of values
-
+        # if test is False:
+        #     debuginfo("O for", l_combinations, 'in', agent)
+        #     return 0
+        #     debuginfo(sum(l_totals))
+        #     debuginfo("L_TOTALS", l_totals, "-", l_combinations)
+        #     debuginfo(agent.statevars, '--', self.t_variables)
+        #     raise
+        #debuginfo(sum(l_totals))
         return sum(l_totals)
 
 
 class create_counter_getter:
     def __init__(self, grouping_name, t_states):
         """Build a callable class used as a getter for property of the form
         ``total_X_Y`` where ``X`` and ``Y`` are state names in the
@@ -212,16 +247,51 @@
             agent which returns True if the agent is in state
             *state_name*, False otherwise.
 
         """
         self.state_name = state_name
 
     def __call__(self, agent):
+        # debuginfo("call is", self.state_name)
         return agent.is_in_state(self.state_name)
 
+################ ORGANIZATION PART
+class create_space_tester:
+    def __init__(self, space_name):
+        """Build a callable class used as a getter for property of the form
+        ``isin_X`` where ``X`` is a space of an organization.
+
+        Parameters
+        ----------
+        space_name: str
+            the name of the space
+
+        Returns
+        -------
+        callable:
+            A callable class which can be applied to an ``AtomAgent``
+            agent which returns True if the agent is in the space
+            *space_name*, False otherwise.
+
+        """
+        self.space_name = space_name
+
+    def __call__(self, agent):
+        return agent.is_in_space(self.space_name)
+
+
+class create_index_getter:
+    def __init__(self, space_name):
+        self.space_name = space_name
+
+    def __call__(self, agent):
+        space = agent.model.dict_space[self.space_name]
+        raise Exception(space)
+##################### END ORGANIZATION PART
+
 class create_duration_getter:
     def __init__(self, machine_name):
         """Build a callable class used as a getter for property of the form
         ``duration_in_M`` where ``M`` is a *machine_name*.
 
         Parameters
         ----------
@@ -277,22 +347,17 @@
         #     op = getattr(current_module, operator)
         if hasattr(current_module, operator):
             op = getattr(current_module, operator)
         elif operator.startswith('percentile'):
             # special case of 'percentileXX' where XX is a number (0 to
             # 100) and automatically extracted
             op = partial(np.percentile, q=int(operator[10:]))
-        # otherwise search in numpy
-        elif hasattr(np, operator):
-            op = getattr(np, operator)
-        elif hasattr(np.random, operator):
-            # and finally in numpy.random (e.g. for choice)
-            op = getattr(np.random, operator)
         else:
-            raise SemanticException('No module found to calculate aggregate variable with operator "{}"'.format(operator))
+            # otherwise search in numpy
+            op = getattr(np, operator)
         self.op = op
 
     def __call__(self, *values):
         return self.op(*values)
 
 
 class create_aggregator:
@@ -413,25 +478,14 @@
         try:
             return self.op([sublevel.get_information(self.sourcevar)
                             for sublevel in agent.select_atoms(self.machine_name, state=self.state_name)])
         except ValueError:
             return np.nan
 
 
-def serial(start=0, end=None, model=None):
-    """A very simple serial number generator."""
-    value = start
-    while True:
-        yield value
-        value += 1
-        if end is not None:
-            if value >= model.get_value(end):
-                value = start
-
-
 class create_new_serial:
     def __init__(self, end=None, model=None):
         """Create the serial number generator associated to the specified
         variable.
 
         """
         self.generator = serial(start=0, end=end, model=model)
@@ -653,131 +707,12 @@
 
     Returns
     -------
     class:
         a callable which can be called on an agent
 
     """
-    def __init__(self, value_vame):
-        self.value_vame = value_vame
-
-    def __call__(self, agent):
-        return agent.get_information(self.value_vame)
-
-
-class create_state_indexer:
-    def __init__(self, state_name):
-        """Build a callable class used as a getter for property of the form
-        ``index_X`` where ``X`` is a state of a state machine.
-
-        Parameters
-        ----------
-        state_name: str
-            the name of state
-
-        Returns
-        -------
-        callable:
-            A callable class which can be applied to any agent
-            which returns the index of the specified state.
-
-        """
-        self.state_name = state_name
-
-    def __call__(self, agent):
-        return agent.model.get_value(self.state_name).value
-
-class create_my_state_indexer:
-    def __init__(self, state_machine_name):
-        """Build a callable class used as a getter for property of the form
-        ``index_my_X`` where ``X`` is a state machine.
-
-        Parameters
-        ----------
-        state_machine_name: str
-            the name of state machine
-
-        Returns
-        -------
-        callable:
-            A callable class which can be applied to any agent which returns the index of the current state of the specified state machine if any, 0 otherwise.
-
-        """
-        self.state_machine_name = state_machine_name
-
-    def __call__(self, agent):
-        if self.state_machine_name in agent.statevars:
-            return agent.statevars[self.state_machine_name].value
-        else:
-            return 0
-
-class create_lazy_ternary:
-    def __init__(self, condition, expression_if_true, expression_if_false):
-        """Build a callable class used to return a value depending on the condition. Evaluations of condition and values are delayed until requested, and non-relevant value is not even calculated.
-
-        Parameters
-        ----------
-        condition: str
-            the expression of the condition
-        expression_if_true: str
-            the expression of the value to calculate if the condition is true
-        expression_if_false: str
-            the expression of the value to calculate if the condition is false
-
-        Returns
-        -------
-        callable:
-            A callable class which returns the value of value_value_if_value_if_true if the condition is fulfilled, otherwise the value of value_if_value_if_false.
-
-        """
-        self.condition = condition
-        self.if_true = expression_if_true
-        self.if_false = expression_if_false
-
-    def __call__(self, agent):
-        return agent.get_information(self.if_true) if agent.get_information(self.condition) else agent.get_information(self.if_false)
-
-class create_lazy_OR:
-    def __init__(self, conditions):
-        """Build a callable class used to return a boolean OR on the conditions. Evaluation of conditions is delayed until requested, and returns true as soon as one condition is fulfilled.
-
-        Parameters
-        ----------
-        conditions: str
-            the list of the conditions to test
-
-        Returns
-        -------
-        callable:
-            A callable class which returns the logical true if any condition is fulfilled, false otherwise.
-
-        """
-        self.conditions = conditions
-
-    def __call__(self, agent):
-        for condition in self.conditions:
-            if agent.get_information(condition):
-                return True
-        return False
-
-class create_lazy_AND:
-    def __init__(self, conditions):
-        """Build a callable class used to return a boolean AND on the conditions. Evaluation of conditions is delayed until requested, and returns false as soon as one condition is not fulfilled.
-
-        Parameters
-        ----------
-        conditions: str
-            the list of the conditions to test
-
-        Returns
-        -------
-        callable:
-            A callable class which returns the logical false if any condition is false, true otherwise.
-
-        """
-        self.conditions = conditions
+    def __init__(self, value_name):
+        self.value_name = value_name
 
     def __call__(self, agent):
-        for condition in self.conditions:
-            if not agent.get_information(condition):
-                return False
-        return True
+        return agent.get_information(self.value_name)
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/graph.py` & `emulsion-1.3b1/src/emulsion/tools/graph.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/misc.py` & `emulsion-1.3b1/src/emulsion/tools/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,28 +51,30 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 
+from   functools                 import partial
 from   importlib                 import import_module
 from   typing                    import List, Iterable, Tuple, Union, Any
 from   collections               import OrderedDict
 from   operator                  import itemgetter
 import itertools                 as it
 
 import csv
 import yaml
 
 import numpy                     as np
 
 from   sortedcontainers          import SortedSet
 from   emulsion.model.exceptions import SemanticException
-from   emulsion.tools.getters    import create_duration_getter, create_state_tester, create_relative_population_getter
+from   emulsion.tools.getters    import create_duration_getter, create_state_tester, create_relative_population_getter, create_space_tester, create_index_getter
+from   emulsion.tools.debug      import debuginfo
 
 AGENTS = 1
 """Constant value for the index where list of agents are stored in
 'populations' tuples.
 
 """
 
@@ -102,15 +104,15 @@
     tuple:
         a tuple composed of the class (type) and the options.
 
     Todo
     ----
     - clarify the role of *options*
     """
-    mod = import_module(module)
+    mod = import_module(module, options)
     return getattr(mod, class_name), options
 
 def load_module(module_name: str):
     """Dynamically load the module with the specified *module_name* and
     return it.
 
     Parameters
@@ -257,14 +259,15 @@
 
 # This function is useful to modellers for the following purposes:
 probabilities_to_rates.__USER_FUNCTION__ = ['Rates / probabilities']
 
 
 # internal usage (TODO: make private to relevant module)
 def rewrite_keys(name, position, change_list):
+    # debuginfo("REWRITE KEY !!!!!!!!!!!!!!!!")
     prefix = name[:position]
     suffix = name[position+1:]
     return [(prefix + (key,) + suffix, value)
             for key, value in change_list]
 
 def complement_key(d_initial_key, l_state_machines, prototype=None):
     """Ensure that all values are assigned to build a consistent key based on *d_initial_key* to identify a compartment (values for the variables corresponding to the expected state machines which operate on the compartment) according to the following rules:
@@ -359,15 +362,15 @@
     -------
     object:
         a Python object built by parsing of the YAML file, i.e. either
         a dict, list, or even str/int/etc... (Most YAML document will
         produce dictionaries.)
 
     """
-    with open(filename, 'r', encoding='utf-8', errors='replace') as fil:
+    with open(filename, 'r') as fil:
         description = yaml.safe_load(fil)
     return description
 
 
 def retrieve_value(value_or_function, agent):
     """Return a value either directly given by parameter
     *value_or_function* if it is a true value, or computed from this
@@ -383,15 +386,15 @@
 
     Returns
     -------
     value:
         the expected value (agent-based or not).
 
     """
-
+    # debuginfo(value_or_function, agent)
     return value_or_function(agent)\
         if callable(value_or_function)\
         else value_or_function
 
 
 def moving_average(values, window_size, mode='same'):
     """Compute a moving average of the specified *values* with respect to
@@ -439,45 +442,42 @@
         the name of the property
     getter_function: callable
         the callable class upon which the property is built
 
     """
     setattr(agent.__class__, property_name, property(getter_function))
     agent._mbr_cache.add(property_name)
-    # debuginfo(agent, agent._mbr_cache)
-
     # debuginfo('Agent {} adding property {} to class {}'.format(agent, property_name, agent.__class__))
 
 
 
-## EXPERIMENTAL - replaced by callable class in the model - should not be used anymore in the rest of the code
 def add_all_test_properties(agent):
     """Endow the agent with individuals properties: ``duration_in_<a state
     machine>`` for all state machines, and ``is_X`` for all states.
 
     """
-    pass
-    # determine the list of state machines associated with the level of the agent
-    # if agent.level is not None:
-    #     # if the agent directly represents a model level, the state machines are known by the model
-    #     l_machines = agent.model.statemachines_by_level[agent.level]
-    # else:
-    #     # otherwise, the agent represents a group, hence can be associated with state machines from the underlying level (sublevel of the agent's upper level)
-    #     l_machines = []
-    #     for level in agent.model.get_sublevels(agent.upper_level().level):
-    #         l_machines += agent.model.statemachines_by_level[level]
-    #
-    # # associate
-    # for machine_name in l_machines:
-    #     add_new_property(agent, 'duration_in_{}'.format(machine_name),
-    #                      create_duration_getter(machine_name))
-    #     machine = agent.model.state_machines[machine_name]
-    #     for state in machine.states:
-    #         add_new_property(agent, 'is_{}'.format(state.name),
-    #                          create_state_tester(state.name))
+    if agent.level is not None:
+        l_machines = agent.model.statemachines_by_level[agent.level]
+    else:
+        l_machines = []
+        for level in agent.model.get_sublevels(agent.upper_level().level):
+            l_machines += agent.model.statemachines_by_level[level]
+    for machine_name in l_machines:
+        add_new_property(agent, 'duration_in_{}'.format(machine_name),
+                         create_duration_getter(machine_name))
+        machine = agent.model.state_machines[machine_name]
+        for state in machine.states:
+            add_new_property(agent, 'is_{}'.format(state.name),
+                             create_state_tester(state.name))
+
+################## ORGANIZATION PART
+        for space in agent.model.organization_model.dict_space:
+            agent.model._values['isin_{}'.format(space)] = create_space_tester(space)
+            agent.model._values['get_index_{}'.format(space)] = create_index_getter(space)
+################## END ORGANIZATION PART
 
 def add_all_relative_population_getters(agent, t_key_variables):
     """Endow the agent with individual properties of the form ``total_X_Y``
     where ``X`` and ``Y`` are either states of two different states
     machines used in a grouping, or keywords built upon a state
     machine name ``M`` of the form ``my_M`` or ``other_M``.
 
@@ -487,40 +487,129 @@
         the agent which will be endowed with the new properties
     key_variables: tuple
         string of tuple containing the names of the state machines
     """
     # compute all relevant combinations between states of the state
     # machines and 'my_statemachine', 'other_statemachine'
     ## example: t_key_variables = ('species', 'health_state')
-    s_all_combinations = set(it.product(
-        *[## concatenate the list of states for each state machine, eg. ['Vector', 'Host'] ...
-          [state.name
-           for state in agent.model.state_machines[machine_name].states
-           if not state.autoremove] +\
-           ## ... with ['my_species', 'other_species'] ...
-          ['my_{}'.format(machine_name), 'other_{}'.format(machine_name)]
-          ## ... and do that for all state machines
-          for machine_name in t_key_variables]))
-    ## => provides a set composed e.g. of {('Vector', 'S'), ('Vector', 'I'), ('Vector', 'R'), ('Host', 'S'), ..., ('my_species', 'S'), ..., ('other_species', 'S'), ..., ('Vector', 'my_health_state'), ('Vector', 'other_health_state'), ('Host', 'my_health_state'), ('Host', 'other_health_state'), ('my_species', 'my_health_state'), ('my_species', 'other_health_state'), ('other_species', 'my_health_state'),('other_species', 'other_health_state'),}
-    ## generate set of fully specified combinations e.g. ('Vector', 'S') which are already handled by existing properties
-    s_state_combinations = set(it.product(
-        *[[state.name
-           for state in agent.model.state_machines[machine_name].states
-           if not state.autoremove]
-          for machine_name in t_key_variables]))
+
+########################## ORGANIZATION PART
+    # create combination sets taking into acount state_machines and organizations
+    # debuginfo("M IN --", agent.model.compartments)
+
+
+    l_part_combinations = [] #for reconcstruct s_state_combination
+    l_all_combinations = []  # for reconstruct s_all_combination
+    l_structured_spaces = []
+    key_variables = []
+    has_leaf = False
+    l_all_real_states = []
+    l_real_spaces = []
+    l_all_states = []
+    for k in t_key_variables:
+        # if k is an organization level
+        if k in agent.model.organization_model.dict_level:
+            has_leaf = True
+            # retrieve all spaces for this level
+            l_spaces = []
+            level = agent.model.organization_model.dict_level[k]
+            l_structured_spaces.append(agent.model.organization_model.dict_level[k]['relative_org'])
+            # debuginfo("ALL    ", level["ALL"], " FOR", k)
+            for s in level["ALL"]:
+                l_spaces.append(s.keys)
+                l_real_spaces.append(s)
+            # add spaces
+            l_part_combinations.append(l_spaces)
+            l_spaces2 = []
+            l_spaces2.append("my_{}".format(k))
+            l_spaces2.append("other_{}".format(k))
+            l_spaces2 += l_spaces
+            # debuginfo("L SPACE", l_spaces2)
+            l_all_combinations.append(l_spaces2)
+            l_all_real_states.append(l_real_spaces)
+            # t_key_variables.remove(k)
+            # add key to new list of key variables
+            key_variables.append(k)
+        else:
+            l_states = [state.name
+                        for state in agent.model.state_machines[k].states]
+            l_real_states = [state
+                             for state in agent.model.state_machines[k].states]
+            l_part_combinations.append(l_states)
+            # debuginfo("L_PART WITH STATE MACHINES", l_part_combinations)
+            l_my = ["my_{}".format(k), "other_{}".format(k)]
+            l_states2 = l_states + l_my
+            l_all_combinations.append(l_states2)
+            l_all_real_states.append(l_real_states)
+            l_all_states.append([state.name
+                                 for state in agent.model.state_machines[k].states])
+            key_variables.append(k)
+
+    # debuginfo("COMBINATIONS CREATED")
+    # debuginfo('L_ALL_COMBINATIONS   ', l_all_combinations)
+    # debuginfo('L_PART COMBINATION   ',l_part_combinations)
+    s_all_combinations = set(it.product(*l_all_combinations))
+    s_state_combinations = set(it.product(*l_part_combinations))
     s_combinations = s_all_combinations - s_state_combinations
 
+    # debuginfo("M OUT --", agent.model.compartments)
+    # raise Exception("CORRECTION GROUPING")
+
+
+
+
+#########################END ORGANIZAION PART
+    # replace by lats section ORGANIZAION PART
+
+    # s_all_combinations = set(it.product(
+    #     *[## concatenate the list of states for each state machine, eg. ['Vector', 'Host'] ...
+    #       [state.name
+    #        for state in agent.model.state_machines[machine_name].states
+    #        if not state.autoremove] +\
+    #       ## ... with ['my_species', 'other_species'] ...
+    #       ['my_{}'.format(machine_name), 'other_{}'.format(machine_name)]
+    #       ## ... and do that for all state machines
+    #       for machine_name in t_key_variables]))
+    # ## => provides a set composed e.g. of {('Vector', 'S'), ('Vector', 'I'), ('Vector', 'R'), ('Host', 'S'), ..., ('my_species', 'S'), ..., ('other_species', 'S'), ..., ('Vector', 'my_health_state'), ('Vector', 'other_health_state'), ('Host', 'my_health_state'), ('Host', 'other_health_state'), ('my_species', 'my_health_state'), ('my_species', 'other_health_state'), ('other_species', 'my_health_state'),('other_species', 'other_health_state'),}
+    # ## generate set of fully specified combinations e.g. ('Vector', 'S') which are already handled by existing properties
+    # s_state_combinations = set(it.product(
+    #     *[[state.name
+    #        for state in agent.model.state_machines[machine_name].states
+    #        if not state.autoremove]
+    #       for machine_name in t_key_variables]))
+    # s_combinations = s_all_combinations - s_state_combinations
+
     # add corresponding properties to specified agent
+
+    # debuginfo('          ->', agent)
+    # debuginfo(agent._mbr_cache)
     for t_combination in s_combinations:
         prop_name = 'total_{}'.format('_'.join(t_combination))
-        # debuginfo('Adding property for', t_combination)
+        # if prop_name == "total_my_animal_type":
+        #     debuginfo('                   ', agent, '->', prop_name)
+        #     debuginfo('Adding property for', agent, prop_name, t_combination)
+
         add_new_property(agent, prop_name,
                          create_relative_population_getter(agent.model, t_combination))
 
 
+
+
+
+def serial(start=0, end=None, model=None):
+    """A very simple serial number generator."""
+    value = start
+    while True:
+        yield value
+        value += 1
+        if end is not None:
+            if value >= model.get_value(end):
+                value = start
+
+
 def read_csv_prototypes(collection_name, filename, method=None, condition=None, weight_column=None, include=[], exclude=[]):
     """Read the definitions of prototypes contained in file *filename* and
     return a dictionary representing the collection.
 
     Parameters
     ----------
     collection_name: str
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/parallel.py` & `emulsion-1.3b1/src/emulsion/tools/parallel.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/plot.py` & `emulsion-1.3b1/src/emulsion/tools/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,39 +59,26 @@
 import pandas                       as pd
 import numpy                        as np
 
 # from   scipy.misc                   import imread
 from   PIL                          import Image
 from   xml.etree                    import ElementTree
 from   bokeh.plotting               import figure, output_file, show
-from bokeh.models import Legend, ColumnDataSource, Range1d, Band
+from   bokeh.models                 import Legend, ColumnDataSource, Range1d
 from   bokeh.models.tools           import HoverTool, CrosshairTool
 from   bokeh.models.glyphs          import ImageURL
 from   bokeh.models.widgets         import Div
-from   bokeh.layouts                import gridplot, column
+from   bokeh.layouts                import gridplot, column, widgetbox
 from   bokeh.palettes               import all_palettes
 
 from   emulsion.tools.debug         import debuginfo
 
-# Nth Percentile
-# 10th Percentile
-def q10(x):
-    return x.quantile(0.1)
-
-# 90th Percentile
-def q90(x):
-    return x.quantile(0.9)
-
-def perc(q):
-    def quant(x, q):
-        return x.quantile(q)
-    return quant
 
 def build_state_plot(counts, cols, machine, model, y='quantity', group='state',
-                     ylab='Number of individuals', style=None, aggregate_plot=False, detail_plot=False):
+                     ylab='Number of individuals', style=None):
     """Return a bokeh figure based on the representation of the states in
     the *counts* dataframe, with the associated colors.
 
     Args:
         counts: a Pandas dataframe containing the values to plot
         cols (dict): dictionary which maps state/variable names to colors
         machine: the state machine to which the states are related
@@ -103,24 +90,14 @@
     Returns:
         A bokeh gridplot (reduced to one figure a the herd level, one
         figure per herd at metapopulation level).
 
     """
     WIDTH, HEIGHT = 800, 600
     NB_SIMU = 1 + counts.simu_id.max()
-
-    aggregate = True
-    if NB_SIMU >= 20:
-        if detail_plot and not aggregate_plot:
-            aggregate = False
-    else:
-        if not aggregate_plot:
-            aggregate = False
-
-
     alpha = max(1 /np.sqrt(NB_SIMU), 0.05)
     all_plots = []
     ncols = 1
     leg_pos, leg_orient = 'right', 'vertical'
     metapop = 'population_id' in counts.columns
     if metapop:
         pop_IDs = np.sort(np.unique(counts.population_id.values))
@@ -135,89 +112,52 @@
             df = counts
         time_unit = model.time_unit
         origin = model.origin_date
         dur = model.step_duration
         # df[time_unit] = pd.Series(model.delta_t * df['step'], index=df.index)
         df = df.assign(**{time_unit: pd.Series(model.delta_t * df['step'], index=df.index)})
         # df['date'] = pd.Series(pd.to_datetime(origin + dur * df['step']), index=df.index)
-        plot = figure(width=WIDTH // ncols, height=HEIGHT // ncols)
+        plot = figure(plot_width=WIDTH // ncols, plot_height=HEIGHT // ncols)
         legend_items = []
         for state in cols:
             state_items = []
             line_style = style[state] if style is not None else 'solid'
             subdf = df[df[group] == state]
-            if not aggregate:
-                if NB_SIMU <= 50:   # don't draw points if too many !
-                    ci = plot.circle(x=time_unit, y='quantity', source=ColumnDataSource(subdf),
-                                     size=2, color=cols[state], alpha=alpha)
-                    state_items.append(ci)
-                for simu_id in range(int(1+df['simu_id'].max())):
-                    src = ColumnDataSource(subdf[subdf.simu_id == simu_id])
-                    pl = plot.line(x=time_unit, y='quantity', source=src, color=cols[state], alpha=alpha, line_width=2, line_dash=line_style)
-                    state_items.append(pl)
-            else:
-                df2 = subdf.groupby(time_unit)
-                maxv = df2.quantity.max()
-                minv = df2.quantity.min()
-                upper = df2.quantity.quantile(0.9)
-                lower = df2.quantity.quantile(0.1)
-                med = df2.quantity.quantile(0.5)
-                x = pd.unique(df[time_unit])
-                if group == 'state':
-                    src = ColumnDataSource(data=dict(time=x, median=med, upper=upper, lower=lower, min=minv, max=maxv, state=[group] * len(x)))
-                else:
-                    src = ColumnDataSource(data=dict(time=x, median=med, upper=upper, lower=lower, min=minv, max=maxv, variable=[group] * len(x)))
-
-                pl = plot.line(x='time', y='median', source=src, color=cols[state], alpha=0.9, line_width=2, line_dash=line_style)
-                plmin = plot.line(x='time', y='min', source=src, color=cols[state], alpha=1, line_width=2, line_dash="dotted")
-                plmax = plot.line(x='time', y='max', source=src, color=cols[state], alpha=1, line_width=2, line_dash="dotted")
-                ribbon = plot.varea(x='time', y1='lower', y2='upper', source=src, fill_alpha=0.2, fill_color=cols[state])
+            if NB_SIMU <= 50:   # don't draw points if too many !
+                ci = plot.circle(x=time_unit, y='quantity', source=ColumnDataSource(subdf),
+                                 size=2, color=cols[state], alpha=alpha)
+                state_items.append(ci)
+            for simu_id in range(int(1+df['simu_id'].max())):
+                src = ColumnDataSource(subdf[subdf.simu_id == simu_id])
+                pl = plot.line(x=time_unit, y='quantity', source=src, color=cols[state], alpha=alpha, line_width=2, line_dash=line_style)
                 state_items.append(pl)
-                state_items.append(plmin)
-                state_items.append(plmax)
-                state_items.append(ribbon)
-
             legend_items.append((state, state_items))
-
         plot.title.text = 'Evolution of %s (%s)' % (machine.replace('_', ' '), model.model_name)
-        if aggregate:
-            plot.title.text += ' - median, 10-90 perc., min-max'
         if metapop:
             plot.title.text += ' - population ID: {}'.format(pop_id)
         plot.xaxis.axis_label = 'Time (%s)' % (time_unit,)
         plot.yaxis.axis_label = ylab
         ylim = max(1, df['quantity'].max()*1.1)
         plot.y_range = Range1d(0, ylim)
         hover = HoverTool()
-        if aggregate:
-            hover.tooltips=[
-                (group.capitalize(), '@%s' % (group,)),
-                ('Quantity', '@median'),
-                ('10-90 perc.', '@lower-@upper'),
-                ('Min-Max', '@min-@max'),
-                (time_unit.capitalize(), '@time'),
-                # ('Population ID', pop_id)
-            ]
-        else:
-            hover.tooltips=[
-                (group.capitalize(), '@%s' % (group,)),
-                ('Quantity', '@quantity'),
-                (time_unit.capitalize(), '@%s'%(time_unit,)),
-                ('Step', '@step'),
-                ('Simulation ID', '@simu_id'),
-                # ('Population ID', pop_id)
-            ]
+        hover.tooltips=[
+            (group.capitalize(), '@%s' % (group,)),
+            ('Quantity', '@quantity'),
+            (time_unit.capitalize(), '@%s'%(time_unit,)),
+            ('Step', '@step'),
+            ('Simulation ID', '@simu_id'),
+            # ('Population ID', pop_id)
+        ]
         plot.add_tools(hover)
         plot.add_tools(CrosshairTool())
         legend = Legend(items=legend_items, location=(0, 0))
         legend.click_policy = 'hide'
         legend.orientation = leg_orient
         plot.add_layout(legend, leg_pos)
         all_plots.append(plot)
-
     return gridplot(all_plots, ncols=ncols, toolbar_location="above")
 
 
 def build_machine_plot(machine_name, model, params):
     """Return a bokeh figure based on the representation of the state
     machine, with the associated colors.
 
@@ -249,15 +189,15 @@
 
     div = Div(text='''<h1>State machine for {}</h1>
     <P><IMG SRC="{}"></P>
     <H2>Simulation outputs</H2>
     '''.format(machine_name, machine_url),
               width=width, height=height+100)
 
-    return gridplot([column(div)], ncols=1)
+    return gridplot([widgetbox(div)], ncols=1)
 
 def plot_outputs(params):
     """Read outputs from previous runs and plot the corresponding
     figures. In the *params* dictionary, `output_dir` is expected to
     contain a `counts.csv` file; `figure_dir` is where the plot is
     saved.
 
@@ -286,28 +226,30 @@
         if params.view_machines:
             all_figs.append(build_machine_plot(sm_name, model, params))
         col_dict = state_machine.state_colors
         style_dict = state_machine.state_style
         # col_dict.update(population="black")
         states, cols = zip(*sorted(col_dict.items()))
         vals += [state.name for state in state_machine.states]
-        df2 = pd.melt(df, id_vars=vars, value_vars=states, var_name='state', value_name='quantity')
-        fig = build_state_plot(df2, col_dict, sm_name, model, style=style_dict, aggregate_plot=params.aggregate_plot, detail_plot=params.detail_plot)
+        df2 = pd.melt(df, id_vars=vars, value_vars=states,
+                      var_name='state', value_name='quantity')
+        fig = build_state_plot(df2, col_dict, sm_name, model, style=style_dict)
         all_figs.append(fig)
         # figpath = Path(params.figure_dir,
         #                model.model_name + '_' + sm_name + '.png')
         # plot = build_state_plot(df2, cols, sm_name, model.model_name)
         # plot.save(str(figpath))
         # print('Saved figure %s' % (figpath, ))
     extras = [variable for variable in df.columns if variable not in vars + vals]
     if extras:
         df2 = pd.melt(df, id_vars=vars, value_vars=extras, value_name='quantity')
         idx = [(256 // len(extras))*i for i in range(len(extras))]
         cols=dict(zip(extras, [all_palettes['Plasma'][256][i] for i in idx]))
-        fig = build_state_plot(df2, cols, 'Additional variables', model, y='value', group='variable', ylab='Value', aggregate_plot=params.aggregate_plot, detail_plot=params.detail_plot)
+        fig = build_state_plot(df2, cols, 'Additional variables', model,
+                               y='value', group='variable', ylab='Value')
         # plot = build_state_plot(df2, [], 'Additional variables',
         #                         model.model_name, y='value', group='variable')
         # plot.save(str(figpath))
         # print('Saved figure %s' % (figpath, ))
         all_figs.append(fig)
     # print(all_figs)
     print('Outputs plot in file: %s' % (figpath,))
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/preprocessor.py` & `emulsion-1.3b1/src/emulsion/tools/preprocessor.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/simulation.py` & `emulsion-1.3b1/src/emulsion/tools/simulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 import pandas         as     pd
 
 from   tqdm           import trange, tqdm   # a nice replacement for progressbar2
 
 from   sqlalchemy     import create_engine
 
 from   emulsion.model.emulsion_model import EmulsionModel
-from   emulsion.model.exceptions     import SemanticException
 from   emulsion.tools.misc           import load_class
 from   emulsion.tools.debug          import debuginfo
 
+from   emulsion.tools.debug  import debuginfo
+
 #   ____        _               _   __  __
 #  / __ \      | |             | | |  \/  |
 # | |  | |_   _| |_ _ __  _   _| |_| \  / | __ _ _ __   __ _  __ _  ___ _ __
 # | |  | | | | | __| '_ \| | | | __| |\/| |/ _` | '_ \ / _` |/ _` |/ _ \ '__|
 # | |__| | |_| | |_| |_) | |_| | |_| |  | | (_| | | | | (_| | (_| |  __/ |
 #  \____/ \__,_|\__| .__/ \__,_|\__|_|  |_|\__,_|_| |_|\__,_|\__, |\___|_|
 #                  | |                                        __/ |
@@ -148,14 +149,15 @@
             shared_data: dict containing pre-loaded input data to be shared
               between several simulations (without reloading them)
 
         """
         # ID of simulation
         self.start_id = start_id
         self.model = EmulsionModel(filename=model_path, input_dir=input_dir) if model is None else model
+        self.model.set_simulation(self)
         self.stock_agent = stock_agent
         self.target_agent_class = target_agent_class
         self.output_manager = OutputManager(model=self.model, output_dir=output_dir)
         self.save_results = save_results
         self.save_to_file = save_to_file
         self.load_from_file = load_from_file
 
@@ -271,14 +273,15 @@
 
         See Also:
             `emulsion.tools.simulation.AbstractSimulation`_
         """
         super().__init__(**others)
         self.simu_id = simu_id
         self.steps = steps
+        self.current_step = 0
         self.silent = silent
         self.quiet = quiet
         self.nocount = nocount
 
         del(others['target_agent_class'])
         others['simu_id'] = self.simu_id
         others['simulation'] = self
@@ -308,30 +311,82 @@
     def run(self, dparams: dict = {}):
         """Make the simulation progress."""
         if self.silent or self.quiet:
             progress = range(self.steps)
         else:
             progress = trange(self.steps, desc=f'[Run {self.simu_id}]',
                               bar_format='{l_bar}{bar}| {n_fmt}/{total_fmt}')
+# ORGANIZATION_PART-----------
+        if self.model.organization_model is not None:
+            # self.model.organization_model.create_output_df()
+            self.model.organization_model.set_simu_id(self.simu_id)
+            self.model.organization_model.set_simulation(self)
+            # self.model.organization_model.init_population()
+# ----------------------------
         if not self.nocount:
             self.update_csv_counts(self.counts, dparams=dparams)
+
         for step in progress:
+            self.current_step = step
+# ORGANIZATION PART----------
+            if self.model.organization_model is not None:
+                self.start_of_step_actions(step)
+                self.org_counters(step)
+# --------------------------
             self.agent.evolve()
+            # debuginfo(step, "-->", self.agent)
+# ORGANIZATION_PART-----------
+            # if self.model.organization_model is not None:
+            #     self.end_of_step_actions(step)
+            # if self.model.organization_model is not None:
+            #     self.start_of_step_actions(step)
+            #     self.org_counters(step)
+# ---------------------------
             if step % self.outputs_period == 0 and not self.nocount:
                 self.update_csv_counts(self.counts,
                                        # header=not exists(self.counts_path),
                                        dparams=dparams)
             if self.model.conditional_stop and self.agent.get_model_value('stop_condition'):
                 debuginfo('Stop condition fulfilled: {}'.format(self.model._description['time_info']['stop_condition']))
                 break
         ## make main level agent run a "finalization" procedure if any
         self.agent.finalize_level(simulation=self)
         if self.save_to_file:
             self.agent.save_state_to_file(self.simu_id, self.save_to_file)
 
+# ORGANIZATION_PART-----------
+        # write outputs organization to csv
+        # if self.model.organization_model is not None:
+        #     output_path = self.output_manager.output_dir
+        #     # for key,df in self.model.organization_model.dict_output.items():
+        #     #     path = "%s/%s.csv"%(output_path,key)
+        #     #     df.to_csv(path, header=True, index=False)
+
+        #     path = "%s/%s.csv"%(output_path,"output_organization")
+        #     self.model.organization_model.create_csv(path)
+# ---------------------------
+
+
+# ORGANIZATION_PART-----------
+    def org_counters(self, step):
+        # DEPRECATED ?
+        pass
+        # self.model.organization_model.save_counts(step)
+
+    def start_of_step_actions(self, step):
+        """actions executed at the end of each step"""
+        self.model.organization_model.set_step(step)
+        # debuginfo(self.model.organization_model.ordered_list_execute)
+        # debuginfo(self.model.organization_model.dict_roots)
+        # for organization in self.model.organization_model.ordered_list_execute:
+        #     organization.end_of_step_actions(step)
+        for organization_name, organization_object in self.model.organization_model.dict_roots.items():
+            organization_object.end_of_step_actions(step)
+# ---------------------------
+
     @property
     def counts(self):
         """Return a pandas DataFrame contains counts of each process if existing.
         TODO: column steps need to be with one of process
         and NO column steps for inter herd
 
         """
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/state.py` & `emulsion-1.3b1/src/emulsion/tools/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """This class represents enumerations for states of state machines in
     EMULSION. They are endowed with some special features:
 
     #. They provide total ordering between items (based on ``__lt__``
        and ``__eq__`` methods).
     #. A comparison with ``None`` is provided (any state is always
        greater than ``None``).
-    #. Underlying values can be used to get/set states
+    #. Other features will be developed soon.
 
     """
 
     def __lt__(self, other):
         """Return a less-than comparison for enumeration items. An enum item
         is always greater than ``None``and than any other item of
         another enumeration. Then, the ``value`` attribute of the item
```

### Comparing `emulsion-1.2rc5/src/emulsion/tools/timing.py` & `emulsion-1.3b1/src/emulsion/tools/timing.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion/tools/view.py` & `emulsion-1.3b1/src/emulsion/tools/view.py`

 * *Files identical despite different names*

### Comparing `emulsion-1.2rc5/src/emulsion.egg-info/PKG-INFO` & `emulsion-1.3b1/src/emulsion.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: emulsion
-Version: 1.2rc5
+Version: 1.3b1
 Summary: Epidemiological Multi-Level Simulation framework
 Home-page: https://sourcesup.renater.fr/emulsion-public/
-Download-URL: https://pypi.org/project/emulsion/
-Author: Sébastien Picault, Yu-Lin Huang, Vianney Sicard and Pauline Ezanno
+Author: Sebastien Picault, Yu-Lin Huang, Vianney Sicard and Pauline Ezanno
 Author-email: sebastien.picault@inrae.fr
 Maintainer: Sébastien Picault
 Maintainer-email: sebastien.picault@inrae.fr
 License: Apache-2.0
+Download-URL: https://pypi.org/project/emulsion/
 Project-URL: Documentation, https://sourcesup.renater.fr/emulsion-public/
-Project-URL: Source Code, https://forgemia.inra.fr/dynamo/software/emulsion-public
+Project-URL: Source Code, https://git.renater.fr/emulsion-public.git
+Description: 
+        Framework EMULSION is intended for modellers in epidemiology, to help
+        them design, simulate, and revise complex mechanistic stochastic
+        models, without having to write or rewrite huge amounts of code.
+        
+        It comes with a *Domain-Specific Language* to represent all components
+        of epidemiological models (assumptions, model structure,
+        parameters...) in an explicit, intelligible and revisable way, and
+        thus facilitate interactions with other scientists (biologists,
+        veterinarians, economists...) throughout the modelling
+        process. EMULSION models are automatically processed by a modular
+        simulation engine, which, if needed, can also incorporate small code
+        add-ons for representing very specific features of a model.
+        
+        Models can use classical modelling paradigms (compartments,
+        individual-based models, metapopulations) and multiple scales (from
+        individuals to metapopulations), thanks to recent research in
+        Artificial Intelligence.
+        
 Keywords: epidemiological modelling,computational epidemiology,multilevel modelling,compartment-based models,individual-based models,metapopulations,agent-based simulation,animal health,artificial intelligence,stochastic models,mechanistic models
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Unix Shell
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Provides-Extra: doc
 Provides-Extra: dev
-License-File: LICENSE
-License-File: NOTICE
-
-
-Framework EMULSION is intended for modellers in epidemiology, to help
-them design, simulate, and revise complex mechanistic stochastic
-models, without having to write or rewrite huge amounts of code.
-
-It comes with a *Domain-Specific Language* to represent all components
-of epidemiological models (assumptions, model structure,
-parameters...) in an explicit, intelligible and revisable way, and
-thus facilitate interactions with other scientists (biologists,
-veterinarians, economists...) throughout the modelling
-process. EMULSION models are automatically processed by a modular
-simulation engine, which, if needed, can also incorporate small code
-add-ons for representing very specific features of a model.
-
-Models can use classical modelling paradigms (compartments,
-individual-based models, metapopulations) and multiple scales (from
-individuals to metapopulations), thanks to recent research in
-Artificial Intelligence.
```

### Comparing `emulsion-1.2rc5/src/emulsion.egg-info/SOURCES.txt` & `emulsion-1.3b1/src/emulsion.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,76 +17,58 @@
 doc/html/_static/benchmark/model4.yaml
 doc/html/_static/benchmark/model5-short.yaml
 doc/html/_static/benchmark/model5.yaml
 doc/html/_static/benchmark/model6-short.yaml
 doc/html/_static/benchmark/model6.yaml
 doc/html/_static/benchmark/model7-short.yaml
 doc/html/_static/benchmark/model7.yaml
-doc/html/_static/models/features/IBM_ABC.yaml
 doc/html/_static/models/features/IBM_SEIRS.yaml
 doc/html/_static/models/features/IBM_SIR.yaml
 doc/html/_static/models/features/IBM_SIRS_periodic_risk.yaml
 doc/html/_static/models/features/IBM_SIR_JA_demo.yaml
 doc/html/_static/models/features/IBM_SIR_JA_demo_prototypes.yaml
 doc/html/_static/models/features/IBM_SIR_JA_demo_random.yaml
 doc/html/_static/models/features/IBM_SIR_JA_metapop.yaml
 doc/html/_static/models/features/IBM_SIR_JA_metapop_data.yaml
 doc/html/_static/models/features/IBM_SIR_JA_struct.yaml
 doc/html/_static/models/features/IBM_SIR_age_demo.yaml
 doc/html/_static/models/features/IBM_SIR_aggreg.yaml
 doc/html/_static/models/features/IBM_SIR_cumul_inc.yaml
 doc/html/_static/models/features/IBM_SIR_demo.yaml
-doc/html/_static/models/features/IBM_SIR_struct.yaml
 doc/html/_static/models/features/IBM_duration.yaml
 doc/html/_static/models/features/IBM_gest.yaml
-doc/html/_static/models/features/compart_ABC.yaml
 doc/html/_static/models/features/compart_SEIRS.yaml
+doc/html/_static/models/features/compart_SEIRS_tmp.yaml
 doc/html/_static/models/features/compart_SIR.yaml
 doc/html/_static/models/features/compart_SIRS_periodic_risk.yaml
 doc/html/_static/models/features/compart_SIR_JA_demo.yaml
-doc/html/_static/models/features/compart_SIR_JA_demo_prototypes.yaml
 doc/html/_static/models/features/compart_SIR_JA_demo_random.yaml
 doc/html/_static/models/features/compart_SIR_JA_metapop.yaml
 doc/html/_static/models/features/compart_SIR_JA_metapop_data.yaml
 doc/html/_static/models/features/compart_SIR_JA_struct.yaml
 doc/html/_static/models/features/compart_SIR_cumul_inc.yaml
 doc/html/_static/models/features/compart_SIR_demo.yaml
-doc/html/_static/models/features/compart_SIR_lockdown.yaml
-doc/html/_static/models/features/compart_SIR_metapop.yaml
-doc/html/_static/models/features/compart_SIR_struct.yaml
 doc/html/_static/models/features/compart_duration.yaml
-doc/html/_static/models/features/hybrid_ABC-old.yaml
-doc/html/_static/models/features/hybrid_ABC.yaml
-doc/html/_static/models/features/hybrid_ABC2.yaml
 doc/html/_static/models/features/hybrid_SEIRS.yaml
 doc/html/_static/models/features/hybrid_SIR.yaml
 doc/html/_static/models/features/hybrid_SIRS_periodic_risk.yaml
 doc/html/_static/models/features/hybrid_SIR_JA_demo.yaml
 doc/html/_static/models/features/hybrid_SIR_JA_demo_prototypes.yaml
 doc/html/_static/models/features/hybrid_SIR_JA_demo_random.yaml
 doc/html/_static/models/features/hybrid_SIR_JA_metapop.yaml
 doc/html/_static/models/features/hybrid_SIR_JA_metapop_data.yaml
 doc/html/_static/models/features/hybrid_SIR_JA_struct.yaml
 doc/html/_static/models/features/hybrid_SIR_age_demo.yaml
 doc/html/_static/models/features/hybrid_SIR_aggreg.yaml
 doc/html/_static/models/features/hybrid_SIR_cumul_inc.yaml
 doc/html/_static/models/features/hybrid_SIR_demo.yaml
-doc/html/_static/models/features/hybrid_SIR_lockdown.yaml
-doc/html/_static/models/features/hybrid_SIR_metapop.yaml
-doc/html/_static/models/features/hybrid_SIR_metapop_data.yaml
 doc/html/_static/models/features/hybrid_SIR_metapop_params.yaml
-doc/html/_static/models/features/hybrid_SIR_struct.yaml
 doc/html/_static/models/features/hybrid_duration.yaml
 doc/html/_static/models/features/hybrid_gest.yaml
 doc/html/_static/models/quickstart/quickstart.yaml
-doc/html/_static/models/transition/compart_SIR_JA_demo-1.1.yaml
-doc/html/_static/models/transition/compart_SIR_JA_demo-1.2.yaml
-doc/html/_static/models/transition/hybrid_SIR_JA_demo-1.1.yaml
-doc/html/_static/models/transition/hybrid_SIR_JA_demo-1.2.yaml
-models/features/IBM_ABC.yaml
 models/features/IBM_SEIRS.yaml
 models/features/IBM_SIR.yaml
 models/features/IBM_SIRS_periodic_risk.yaml
 models/features/IBM_SIR_JA_demo.yaml
 models/features/IBM_SIR_JA_demo_prototypes.yaml
 models/features/IBM_SIR_JA_demo_random.yaml
 models/features/IBM_SIR_JA_metapop.yaml
@@ -95,32 +77,27 @@
 models/features/IBM_SIR_JA_struct.yaml
 models/features/IBM_SIR_age_demo.yaml
 models/features/IBM_SIR_aggreg.yaml
 models/features/IBM_SIR_cumul_inc.yaml
 models/features/IBM_SIR_demo.yaml
 models/features/IBM_duration.yaml
 models/features/IBM_gest.yaml
-models/features/compart_ABC.yaml
 models/features/compart_SEIRS.yaml
+models/features/compart_SEIRS_tmp.yaml
 models/features/compart_SIR.yaml
 models/features/compart_SIRS_periodic_risk.yaml
 models/features/compart_SIR_JA_demo.yaml
-models/features/compart_SIR_JA_demo_prototypes.yaml
 models/features/compart_SIR_JA_demo_random.yaml
 models/features/compart_SIR_JA_metapop.yaml
 models/features/compart_SIR_JA_metapop_data.py
 models/features/compart_SIR_JA_metapop_data.yaml
 models/features/compart_SIR_JA_struct.yaml
 models/features/compart_SIR_cumul_inc.yaml
 models/features/compart_SIR_demo.yaml
-models/features/compart_SIR_lockdown.yaml
 models/features/compart_duration.yaml
-models/features/hybrid_ABC-old.yaml
-models/features/hybrid_ABC.yaml
-models/features/hybrid_ABC2.yaml
 models/features/hybrid_SEIRS.yaml
 models/features/hybrid_SIR.yaml
 models/features/hybrid_SIRS_periodic_risk.yaml
 models/features/hybrid_SIR_JA_demo.yaml
 models/features/hybrid_SIR_JA_demo_prototypes.yaml
 models/features/hybrid_SIR_JA_demo_random.yaml
 models/features/hybrid_SIR_JA_metapop.yaml
@@ -171,22 +148,65 @@
 src/emulsion/agent/managers/metapop_process_manager.py
 src/emulsion/agent/managers/multi_process_manager.py
 src/emulsion/model/__init__.py
 src/emulsion/model/emulsion_model.py
 src/emulsion/model/exceptions.py
 src/emulsion/model/functions.py
 src/emulsion/model/state_machines.py
+src/emulsion/organization/AbstractParse.py
+src/emulsion/organization/AtomicSpace.py
+src/emulsion/organization/Constante.py
+src/emulsion/organization/OrganizationAction.py
+src/emulsion/organization/OrganizationConstraint.py
+src/emulsion/organization/OrganizationException.py
+src/emulsion/organization/OrganizationGraph.py
+src/emulsion/organization/OrganizationManager.py
+src/emulsion/organization/OrganizationModel.py
+src/emulsion/organization/OrganizationPosition.py
+src/emulsion/organization/OrganizationProcess.py
+src/emulsion/organization/OrganizationPropagate.py
+src/emulsion/organization/Passport.py
+src/emulsion/organization/__init__.py
+src/emulsion/organization/organization_function.py
+src/emulsion/organization/managers/OrganizationProcessManager.py
+src/emulsion/organization/managers/__init__.py
+src/emulsion/organization/utils/__init__.py
+src/emulsion/organization/utils/organization_plot.py
 src/emulsion/resources/emulsion.tx
+src/emulsion/scripts/emulsion-completion.sh
+src/emulsion/templates/EMUL_templates/groups.yaml
+src/emulsion/templates/EMUL_templates/head.yaml
+src/emulsion/templates/EMUL_templates/initials.yaml
+src/emulsion/templates/EMUL_templates/levels.yaml
+src/emulsion/templates/EMUL_templates/organizations.yaml
+src/emulsion/templates/EMUL_templates/outputs.yaml
+src/emulsion/templates/EMUL_templates/parameters.yaml
+src/emulsion/templates/EMUL_templates/prototypes.yaml
+src/emulsion/templates/EMUL_templates/state_machines.yaml
+src/emulsion/templates/EMUL_templates/statevars.yaml
+src/emulsion/templates/YAML_templates/groups.yaml
+src/emulsion/templates/YAML_templates/head.yaml
+src/emulsion/templates/YAML_templates/initials.yaml
+src/emulsion/templates/YAML_templates/levels.yaml
+src/emulsion/templates/YAML_templates/organizations.yaml
+src/emulsion/templates/YAML_templates/outputs.yaml
+src/emulsion/templates/YAML_templates/parameters.yaml
+src/emulsion/templates/YAML_templates/prototypes.yaml
+src/emulsion/templates/YAML_templates/state_machines.yaml
+src/emulsion/templates/YAML_templates/statevars.yaml
+src/emulsion/templates/main_template/main.emul
+src/emulsion/tools/DebugGlobal.py
 src/emulsion/tools/__init__.py
 src/emulsion/tools/calendar.py
 src/emulsion/tools/debug.py
 src/emulsion/tools/functions.py
 src/emulsion/tools/getters.py
 src/emulsion/tools/graph.py
 src/emulsion/tools/misc.py
 src/emulsion/tools/parallel.py
+src/emulsion/tools/persist.py
 src/emulsion/tools/plot.py
 src/emulsion/tools/preprocessor.py
 src/emulsion/tools/simulation.py
 src/emulsion/tools/state.py
 src/emulsion/tools/timing.py
 src/emulsion/tools/view.py
```

