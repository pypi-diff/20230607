# Comparing `tmp/tcex-3.0.8.tar.gz` & `tmp/tcex-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcex-3.0.8.tar", last modified: Mon Apr 10 17:48:24 2023, max compression
+gzip compressed data, was "tcex-3.0.9.tar", last modified: Wed Jun  7 19:48:12 2023, max compression
```

## Comparing `tcex-3.0.8.tar` & `tcex-3.0.9.tar`

### file list

```diff
@@ -1,426 +1,426 @@
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.428491 tcex-3.0.8/
--rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2019-02-12 17:08:25.000000 tcex-3.0.8/LICENSE
--rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-04-10 17:48:24.428624 tcex-3.0.8/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)     2211 2022-11-14 21:07:06.000000 tcex-3.0.8/README.md
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.266764 tcex-3.0.8/bin/
--rw-rw-r--   0 bsummers   (503) staff       (20)    15774 2023-04-10 17:48:00.000000 tcex-3.0.8/bin/tcex
--rw-rw-r--   0 bsummers   (503) staff       (20)     1006 2023-04-10 17:48:00.000000 tcex-3.0.8/pyproject.toml
--rw-rw-r--   0 bsummers   (503) staff       (20)      772 2023-04-10 17:48:24.429189 tcex-3.0.8/setup.cfg
--rw-rw-r--   0 bsummers   (503) staff       (20)     3081 2023-04-10 17:48:00.000000 tcex-3.0.8/setup.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.267810 tcex-3.0.8/tcex/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1139 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      432 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/__metadata__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.270634 tcex-3.0.8/tcex/api/
--rw-rw-r--   0 bsummers   (503) staff       (20)       76 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      765 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/api.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.271340 tcex-3.0.8/tcex/api/tc/
--rw-rw-r--   0 bsummers   (503) staff       (20)       91 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/tc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.272600 tcex-3.0.8/tcex/api/tc/ti_transform/
--rw-rw-r--   0 bsummers   (503) staff       (20)      141 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      196 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/formatters.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.273255 tcex-3.0.8/tcex/api/tc/ti_transform/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)      353 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7541 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/ti_transform/model/transform_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6377 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/ti_transform.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    25131 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/ti_transform/transform_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.274002 tcex-3.0.8/tcex/api/tc/utils/
--rw-rw-r--   0 bsummers   (503) staff       (20)       39 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/utils/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14736 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/utils/threat_intel_utils.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.274944 tcex-3.0.8/tcex/api/tc/v2/
--rw-rw-r--   0 bsummers   (503) staff       (20)      100 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.279547 tcex-3.0.8/tcex/api/tc/v2/batch/
--rw-rw-r--   0 bsummers   (503) staff       (20)      228 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/batch/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2671 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    44500 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/batch.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18746 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/batch/batch_submit.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    51366 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/batch/batch_writer.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    23538 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    29032 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/batch/indicator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1768 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1161 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/tag.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.280722 tcex-3.0.8/tcex/api/tc/v2/datastore/
--rw-rw-r--   0 bsummers   (503) staff       (20)      114 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/datastore/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7077 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/datastore/cache.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11000 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/datastore/datastore.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.281589 tcex-3.0.8/tcex/api/tc/v2/metrics/
--rw-rw-r--   0 bsummers   (503) staff       (20)       84 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/metrics/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6543 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/metrics/metrics.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.282287 tcex-3.0.8/tcex/api/tc/v2/notifications/
--rw-rw-r--   0 bsummers   (503) staff       (20)      102 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/notifications/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3187 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/notifications/notifications.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.284247 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/
--rw-rw-r--   0 bsummers   (503) staff       (20)      118 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.287626 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2386 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/filters.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.288142 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3731 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.293445 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8796 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1625 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      953 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4495 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1112 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2339 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2340 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      951 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      867 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3710 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1564 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      841 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      843 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      831 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.293961 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10357 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.295909 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2166 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2041 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7612 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3127 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2103 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22774 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2241 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/owner.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2945 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2545 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tag.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1249 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tags.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8676 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/task.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15032 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/victim.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    57009 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    35065 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7064 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/v2.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.299481 tcex-3.0.8/tcex/api/tc/v3/
--rw-rw-r--   0 bsummers   (503) staff       (20)       53 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.303442 tcex-3.0.8/tcex/api/tc/v3/_gen/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9764 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    19062 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3450 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_args_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18924 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_filter_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16667 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_model_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    38886 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_object_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.305610 tcex-3.0.8/tcex/api/tc/v3/_gen/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)      176 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4059 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/models/_filter_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14547 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/models/_property_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.306174 tcex-3.0.8/tcex/api/tc/v3/adversary_assets/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/adversary_assets/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1003 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/api_endpoints.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.308694 tcex-3.0.8/tcex/api/tc/v3/artifact_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3157 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2770 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2982 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.311367 tcex-3.0.8/tcex/api/tc/v3/artifacts/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6810 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6061 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8747 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.313621 tcex-3.0.8/tcex/api/tc/v3/attribute_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3206 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3261 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.314731 tcex-3.0.8/tcex/api/tc/v3/attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2234 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/attributes/attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.316429 tcex-3.0.8/tcex/api/tc/v3/case_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4753 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6577 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4834 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.317595 tcex-3.0.8/tcex/api/tc/v3/case_management/
--rw-rw-r--   0 bsummers   (503) staff       (20)       63 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/case_management/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22368 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/case_management/case_management.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.320006 tcex-3.0.8/tcex/api/tc/v3/cases/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/cases/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12920 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/cases/case.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16300 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/cases/case_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12033 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/cases/case_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.321175 tcex-3.0.8/tcex/api/tc/v3/file_actions/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_actions/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1797 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_actions/file_action_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.322333 tcex-3.0.8/tcex/api/tc/v3/file_occurrences/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_occurrences/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1641 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1371 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/filter_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.324563 tcex-3.0.8/tcex/api/tc/v3/group_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4856 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7370 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5255 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.326684 tcex-3.0.8/tcex/api/tc/v3/groups/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/groups/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15307 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/groups/group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22742 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/groups/group_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16799 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/groups/group_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.328321 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4980 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7466 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5383 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.330509 tcex-3.0.8/tcex/api/tc/v3/indicators/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14868 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/indicator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20183 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17137 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.332776 tcex-3.0.8/tcex/api/tc/v3/notes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/notes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3463 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/notes/note.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4852 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/notes/note_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6026 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/notes/note_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12632 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/object_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8527 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/object_collection_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.335300 tcex-3.0.8/tcex/api/tc/v3/security/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1393 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/assignee_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      741 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_group_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      716 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.336885 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3600 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3530 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.338234 tcex-3.0.8/tcex/api/tc/v3/security/owners/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2761 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/owner.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10858 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7508 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2266 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/security.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.339741 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2905 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2697 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2650 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/task_assignee_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.340983 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1411 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2739 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.342361 tcex-3.0.8/tcex/api/tc/v3/security/users/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2734 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/user.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6970 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/user_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2021 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/user_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.343758 tcex-3.0.8/tcex/api/tc/v3/security_labels/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4337 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6009 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3134 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.345015 tcex-3.0.8/tcex/api/tc/v3/tags/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tags/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3980 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/tags/tag.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6091 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/tags/tag_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4349 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tags/tag_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.346187 tcex-3.0.8/tcex/api/tc/v3/tasks/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6646 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/task.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9537 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/task_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7442 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/task_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.347004 tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/
--rw-rw-r--   0 bsummers   (503) staff       (20)       67 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17553 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.348438 tcex-3.0.8/tcex/api/tc/v3/tql/
--rw-rw-r--   0 bsummers   (503) staff       (20)       51 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tql/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2222 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/tql/tql.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      520 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tql/tql_operator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      251 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tql/tql_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1321 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/v3.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18104 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/v3_model_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/v3_types.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.349700 tcex-3.0.8/tcex/api/tc/v3/victim_assets/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5821 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5222 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5177 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.350860 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4815 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7027 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4879 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.352488 tcex-3.0.8/tcex/api/tc/v3/victims/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victims/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7916 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/victims/victim.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9140 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/victims/victim_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6561 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victims/victim_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.355097 tcex-3.0.8/tcex/api/tc/v3/workflow_events/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4550 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4075 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5484 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.357693 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3611 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3449 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5159 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.364794 tcex-3.0.8/tcex/app_config/
--rw-rw-r--   0 bsummers   (503) staff       (20)      327 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    21393 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9324 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6004 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/install_json_update.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1485 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/install_json_validate.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2061 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4484 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/layout_json.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.368857 tcex-3.0.8/tcex/app_config/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)      464 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13834 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/app_config/models/app_spec_yml_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    29279 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/models/install_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2993 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/models/job_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2853 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/layout_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1833 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/tcex_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      914 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/template_config_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20625 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/app_config/permutation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2973 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3222 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/tcex_json_update.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.369779 tcex-3.0.8/tcex/app_feature/
--rw-rw-r--   0 bsummers   (503) staff       (20)      135 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_feature/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5615 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_feature/advanced_request.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.370248 tcex-3.0.8/tcex/backports/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1066 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/backports/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.378474 tcex-3.0.8/tcex/bin/
--rw-rw-r--   0 bsummers   (503) staff       (20)      284 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/bin/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6525 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/bin_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17417 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/bin/dep.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5090 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/bin/deploy.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9593 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/package.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11318 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22766 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_app_input.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8530 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_app_input_static.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11155 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5739 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1587 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      981 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/spec_tool_layout_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14062 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_readme_md.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1057 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/spec_tool_tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    21485 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/bin/template.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    21765 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/validate.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.382766 tcex-3.0.8/tcex/decorators/
--rw-rw-r--   0 bsummers   (503) staff       (20)      360 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/decorators/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2335 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/decorators/benchmark.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/decorators/debug.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4525 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/decorators/fail_on_output.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3681 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/decorators/on_exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1828 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/decorators/on_success.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/decorators/output.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.384490 tcex-3.0.8/tcex/exit/
--rw-rw-r--   0 bsummers   (503) staff       (20)      192 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/exit/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5374 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/exit/error_codes.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6516 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/exit/exit.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.385575 tcex-3.0.8/tcex/input/
--rw-rw-r--   0 bsummers   (503) staff       (20)       92 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.395011 tcex-3.0.8/tcex/input/field_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1242 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3532 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/binary.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3129 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/case_management_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1581 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/choice.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      866 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/datetime.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3764 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/edit_choice.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3073 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2995 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/group_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2725 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/indicator_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3505 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/input/field_types/integer.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2336 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/ip_address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1270 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/key_value.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5151 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/input/field_types/sensitive.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4111 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/string.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1251 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/tc_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8590 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/validators.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15693 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/input/input.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.402222 tcex-3.0.8/tcex/input/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1012 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2575 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/input/models/advanced_request_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      999 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/aot_execution_enabled_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2935 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/input/models/api_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1525 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/batch_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      893 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/cal_settings_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1567 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/input/models/create_config_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1595 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/logging_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2736 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/input/models/model_map.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      428 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/organization_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1162 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/path_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1151 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/playbook_common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      929 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1350 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/proxy_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2716 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1174 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/smtp_settings_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.405595 tcex-3.0.8/tcex/key_value_store/
--rw-rw-r--   0 bsummers   (503) staff       (20)      224 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/key_value_store/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      873 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/key_value_store/key_value_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2499 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/key_value_store/key_value_api.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1801 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/key_value_store/key_value_mock.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2777 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/key_value_store/key_value_redis.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1669 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/key_value_store/redis_client.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.410599 tcex-3.0.8/tcex/logger/
--rw-rw-r--   0 bsummers   (503) staff       (20)      293 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/logger/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3780 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/logger/api_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      862 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/logger/cache_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13964 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/logger/logger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3112 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/pattern_file_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2001 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/rotating_file_handler_custom.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      974 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/sensitive_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/thread_file_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1206 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/logger/trace_logger.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.414162 tcex-3.0.8/tcex/playbook/
--rw-rw-r--   0 bsummers   (503) staff       (20)       88 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/playbook/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3467 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/playbook/playbook.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20899 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/playbook/playbook_create.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1027 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/playbook/playbook_delete.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      668 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/playbook/playbook_output.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22857 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/playbook/playbook_read.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.417968 tcex-3.0.8/tcex/pleb/
--rw-rw-r--   0 bsummers   (503) staff       (20)       26 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/pleb/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1599 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/env_path.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      737 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      536 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/none_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1178 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/pleb/proxies.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7213 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/pleb/registry.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2311 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/pleb/scoped_property.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      412 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/pleb/singleton.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      731 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/threading.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.420337 tcex-3.0.8/tcex/services/
--rw-rw-r--   0 bsummers   (503) staff       (20)      324 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/services/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11874 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/services/api_service.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16230 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/services/common_service.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17548 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/services/common_service_trigger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10563 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/services/mqtt_message_broker.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15948 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/services/webhook_trigger_service.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.421797 tcex-3.0.8/tcex/sessions/
--rw-rw-r--   0 bsummers   (503) staff       (20)       40 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/sessions/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.423269 tcex-3.0.8/tcex/sessions/auth/
--rw-rw-r--   0 bsummers   (503) staff       (20)       31 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/sessions/auth/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1706 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/auth/hmac_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1539 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/sessions/auth/tc_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1835 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/auth/token_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12891 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/external_session.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4923 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/rate_limit_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4420 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/tc_session.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    19749 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/tcex.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.424030 tcex-3.0.8/tcex/tokens/
--rw-rw-r--   0 bsummers   (503) staff       (20)       80 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/tokens/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12245 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/tokens/tokens.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.427409 tcex-3.0.8/tcex/utils/
--rw-rw-r--   0 bsummers   (503) staff       (20)       78 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/utils/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/utils/aes_operations.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10144 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/utils/datetime_operations.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7272 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/utils/file_operations.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.428128 tcex-3.0.8/tcex/utils/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)      127 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/utils/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      667 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/utils/models/playbook_variable_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4889 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/utils/requests_to_curl.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7751 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/utils/string_operations.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6165 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/utils/utils.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7352 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/utils/variables.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.269885 tcex-3.0.8/tcex.egg-info/
--rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)    14001 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/SOURCES.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/dependency_links.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)     1019 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/requires.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        5 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/top_level.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/zip-safe
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.249093 tcex-3.0.9/
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2019-02-12 17:08:25.000000 tcex-3.0.9/LICENSE
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-06-07 19:48:12.249252 tcex-3.0.9/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2211 2022-11-14 21:07:06.000000 tcex-3.0.9/README.md
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.610228 tcex-3.0.9/bin/
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15774 2023-04-10 17:48:00.000000 tcex-3.0.9/bin/tcex
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1006 2023-04-10 17:48:00.000000 tcex-3.0.9/pyproject.toml
+-rw-rw-r--   0 bsummers   (503) staff       (20)      772 2023-06-07 19:48:12.250251 tcex-3.0.9/setup.cfg
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3081 2023-04-10 17:48:00.000000 tcex-3.0.9/setup.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.614649 tcex-3.0.9/tcex/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1139 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      432 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/__metadata__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.627344 tcex-3.0.9/tcex/api/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       76 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      765 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/api.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.648466 tcex-3.0.9/tcex/api/tc/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       91 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/tc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.664446 tcex-3.0.9/tcex/api/tc/ti_transform/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      141 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/ti_transform/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      196 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/ti_transform/formatters.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.669095 tcex-3.0.9/tcex/api/tc/ti_transform/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      353 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/ti_transform/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7765 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/api/tc/ti_transform/model/transform_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6377 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/ti_transform/ti_transform.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    25333 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/api/tc/ti_transform/transform_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.698110 tcex-3.0.9/tcex/api/tc/utils/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       39 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/utils/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14736 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/utils/threat_intel_utils.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.704815 tcex-3.0.9/tcex/api/tc/v2/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      100 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.756918 tcex-3.0.9/tcex/api/tc/v2/batch/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      228 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/batch/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2671 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/batch/attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    44500 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/batch/batch.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18746 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v2/batch/batch_submit.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    51366 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v2/batch/batch_writer.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    23538 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/batch/group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    29032 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v2/batch/indicator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1768 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/batch/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1161 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/batch/tag.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.764767 tcex-3.0.9/tcex/api/tc/v2/datastore/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      114 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/datastore/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7077 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/datastore/cache.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11000 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/datastore/datastore.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.774834 tcex-3.0.9/tcex/api/tc/v2/metrics/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       84 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/metrics/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6543 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/metrics/metrics.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.797834 tcex-3.0.9/tcex/api/tc/v2/notifications/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      102 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/notifications/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3187 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/notifications/notifications.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.812399 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      118 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.852736 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2386 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/filters.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.855627 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3731 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.917885 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8796 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1625 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      953 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4495 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1112 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2339 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2340 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      951 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      867 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3710 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1564 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      841 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      843 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      831 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.921709 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10357 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.956068 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2166 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2041 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7612 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3127 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2103 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22774 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2241 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/owner.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2945 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2545 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/tag.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1249 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/tags.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8676 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/task.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15032 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/victim.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    57009 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    35065 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7064 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v2/v2.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.975525 tcex-3.0.9/tcex/api/tc/v3/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       53 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.021919 tcex-3.0.9/tcex/api/tc/v3/_gen/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9764 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/_gen.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    19062 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3450 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_args_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18924 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_filter_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16667 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_model_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    38886 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_object_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.048371 tcex-3.0.9/tcex/api/tc/v3/_gen/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      176 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4059 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/models/_filter_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14547 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/_gen/models/_property_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.049595 tcex-3.0.9/tcex/api/tc/v3/adversary_assets/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/adversary_assets/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1003 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/api_endpoints.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.063296 tcex-3.0.9/tcex/api/tc/v3/artifact_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/artifact_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3157 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/artifact_types/artifact_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2770 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/artifact_types/artifact_type_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2982 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/artifact_types/artifact_type_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.078235 tcex-3.0.9/tcex/api/tc/v3/artifacts/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/artifacts/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6810 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/artifacts/artifact.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6061 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/artifacts/artifact_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8747 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/artifacts/artifact_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.104121 tcex-3.0.9/tcex/api/tc/v3/attribute_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/attribute_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/attribute_types/attribute_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3206 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/attribute_types/attribute_type_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3261 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/attribute_types/attribute_type_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.108087 tcex-3.0.9/tcex/api/tc/v3/attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2234 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/attributes/attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.116248 tcex-3.0.9/tcex/api/tc/v3/case_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/case_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4753 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/case_attributes/case_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6577 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/case_attributes/case_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4834 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/case_attributes/case_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.124009 tcex-3.0.9/tcex/api/tc/v3/case_management/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       63 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/case_management/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22368 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/case_management/case_management.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.154033 tcex-3.0.9/tcex/api/tc/v3/cases/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/cases/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12920 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/cases/case.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16300 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/cases/case_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12033 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/cases/case_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.159405 tcex-3.0.9/tcex/api/tc/v3/file_actions/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/api/tc/v3/file_actions/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1797 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/api/tc/v3/file_actions/file_action_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.164123 tcex-3.0.9/tcex/api/tc/v3/file_occurrences/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/api/tc/v3/file_occurrences/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1641 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1371 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/filter_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.179108 tcex-3.0.9/tcex/api/tc/v3/group_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/group_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4856 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/group_attributes/group_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7370 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/group_attributes/group_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5255 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/group_attributes/group_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.212084 tcex-3.0.9/tcex/api/tc/v3/groups/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/groups/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15307 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/groups/group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22742 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/groups/group_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16799 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/groups/group_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.225332 tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4980 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7466 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5383 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.255868 tcex-3.0.9/tcex/api/tc/v3/indicators/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/indicators/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14868 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/indicators/indicator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20183 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/indicators/indicator_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17137 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/indicators/indicator_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.267026 tcex-3.0.9/tcex/api/tc/v3/notes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/notes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3463 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/notes/note.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4852 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/notes/note_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6026 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/notes/note_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12632 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/object_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8527 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/object_collection_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.304405 tcex-3.0.9/tcex/api/tc/v3/security/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1393 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/assignee_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      741 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/assignee_user_group_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      716 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/assignee_user_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.318135 tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/owner_role.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3600 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3530 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/owner_role_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.330014 tcex-3.0.9/tcex/api/tc/v3/security/owners/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/owners/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2761 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/owners/owner.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10858 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/owners/owner_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7508 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/owners/owner_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2266 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/security.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.359325 tcex-3.0.9/tcex/api/tc/v3/security/system_roles/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/system_roles/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2905 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/system_roles/system_role.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/system_roles/system_role_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2697 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/system_roles/system_role_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2650 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/task_assignee_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.373994 tcex-3.0.9/tcex/api/tc/v3/security/user_groups/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/user_groups/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/user_groups/user_group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1411 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/user_groups/user_group_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2739 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/user_groups/user_group_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.401226 tcex-3.0.9/tcex/api/tc/v3/security/users/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/users/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2734 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security/users/user.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6970 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/api/tc/v3/security/users/user_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2021 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/security/users/user_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.414277 tcex-3.0.9/tcex/api/tc/v3/security_labels/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/security_labels/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4337 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/security_labels/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6009 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/security_labels/security_label_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3134 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/security_labels/security_label_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.425752 tcex-3.0.9/tcex/api/tc/v3/tags/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/tags/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3980 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/tags/tag.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6091 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/tags/tag_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4349 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/tags/tag_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.453058 tcex-3.0.9/tcex/api/tc/v3/tasks/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/tasks/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6646 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/tasks/task.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9537 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/tasks/task_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7442 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/api/tc/v3/tasks/task_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.457931 tcex-3.0.9/tcex/api/tc/v3/threat_intelligence/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       67 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/threat_intelligence/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17553 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.477032 tcex-3.0.9/tcex/api/tc/v3/tql/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       51 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/tql/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2222 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/tql/tql.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      520 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/tql/tql_operator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      251 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/tql/tql_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1321 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/v3.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18129 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/api/tc/v3/v3_model_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/v3_types.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.504598 tcex-3.0.9/tcex/api/tc/v3/victim_assets/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/victim_assets/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5821 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/api/tc/v3/victim_assets/victim_asset.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5222 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/victim_assets/victim_asset_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5177 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/victim_assets/victim_asset_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.516699 tcex-3.0.9/tcex/api/tc/v3/victim_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/victim_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4815 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/victim_attributes/victim_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7027 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4879 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.529872 tcex-3.0.9/tcex/api/tc/v3/victims/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/victims/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7916 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/victims/victim.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9140 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/victims/victim_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6561 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/victims/victim_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.562685 tcex-3.0.9/tcex/api/tc/v3/workflow_events/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_events/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4550 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_events/workflow_event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4075 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_events/workflow_event_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5484 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_events/workflow_event_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.574990 tcex-3.0.9/tcex/api/tc/v3/workflow_templates/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_templates/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3611 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_templates/workflow_template.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3449 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5159 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/api/tc/v3/workflow_templates/workflow_template_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.630508 tcex-3.0.9/tcex/app_config/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      327 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21393 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/app_config/app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9324 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/app_config/install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6004 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/app_config/install_json_update.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1485 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/install_json_validate.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2061 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4484 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/layout_json.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.676131 tcex-3.0.9/tcex/app_config/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      464 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/app_config/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13834 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/app_config/models/app_spec_yml_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    29279 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/app_config/models/install_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2993 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/models/job_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2853 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/app_config/models/layout_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1833 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/app_config/models/tcex_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      914 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/app_config/models/template_config_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20625 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/app_config/permutation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2973 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3222 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_config/tcex_json_update.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.698781 tcex-3.0.9/tcex/app_feature/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      135 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/app_feature/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5615 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/app_feature/advanced_request.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.705058 tcex-3.0.9/tcex/backports/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1066 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/backports/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.780656 tcex-3.0.9/tcex/bin/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      284 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/bin/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6525 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/bin/bin_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17417 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/bin/dep.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5090 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/bin/deploy.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9593 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/package.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11318 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22766 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool_app_input.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8530 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool_app_input_static.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11155 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool_app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5739 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool_install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1587 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool_job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      981 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/bin/spec_tool_layout_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14062 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/bin/spec_tool_readme_md.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1057 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/bin/spec_tool_tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21485 2023-04-10 17:48:00.000000 tcex-3.0.9/tcex/bin/template.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21765 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/bin/validate.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.829023 tcex-3.0.9/tcex/decorators/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      360 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/decorators/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2335 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/decorators/benchmark.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2020-09-04 22:24:44.000000 tcex-3.0.9/tcex/decorators/debug.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4525 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/decorators/fail_on_output.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3681 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/decorators/on_exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1828 2020-09-04 22:24:44.000000 tcex-3.0.9/tcex/decorators/on_success.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2020-09-04 22:24:44.000000 tcex-3.0.9/tcex/decorators/output.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.858251 tcex-3.0.9/tcex/exit/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      192 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/exit/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5374 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/exit/error_codes.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6516 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/exit/exit.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.866540 tcex-3.0.9/tcex/input/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       92 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:11.954798 tcex-3.0.9/tcex/input/field_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1242 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/input/field_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3532 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/binary.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3129 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/input/field_types/case_management_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1581 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/choice.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      866 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/datetime.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3764 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/edit_choice.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3073 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2995 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/group_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2725 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/indicator_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3505 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/input/field_types/integer.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2336 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/input/field_types/ip_address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1270 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/key_value.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5151 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/input/field_types/sensitive.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4111 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/input/field_types/string.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1251 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/field_types/tc_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8590 2022-03-23 20:18:24.000000 tcex-3.0.9/tcex/input/field_types/validators.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15693 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/input/input.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.012168 tcex-3.0.9/tcex/input/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1012 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2575 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/input/models/advanced_request_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      999 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/aot_execution_enabled_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2935 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/input/models/api_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1525 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/batch_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      893 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/cal_settings_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1567 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/input/models/create_config_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1595 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/logging_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2736 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/input/models/model_map.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      428 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/organization_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1162 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/path_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1577 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/input/models/playbook_common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      929 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1350 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/proxy_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2716 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1174 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/input/models/smtp_settings_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.025595 tcex-3.0.9/tcex/key_value_store/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      224 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/key_value_store/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      873 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/key_value_store/key_value_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2499 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/key_value_store/key_value_api.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1801 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/key_value_store/key_value_mock.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2777 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/key_value_store/key_value_redis.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1860 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/key_value_store/redis_client.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.073325 tcex-3.0.9/tcex/logger/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      293 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/logger/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3780 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/logger/api_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      862 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/logger/cache_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13964 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/logger/logger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3112 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/logger/pattern_file_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2001 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/logger/rotating_file_handler_custom.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1099 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/logger/sensitive_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/logger/thread_file_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1206 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/logger/trace_logger.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.106971 tcex-3.0.9/tcex/playbook/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       88 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/playbook/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3467 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/playbook/playbook.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20899 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/playbook/playbook_create.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1027 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/playbook/playbook_delete.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      668 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/playbook/playbook_output.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22857 2022-08-26 17:57:26.000000 tcex-3.0.9/tcex/playbook/playbook_read.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.128115 tcex-3.0.9/tcex/pleb/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       26 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/pleb/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1599 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/pleb/env_path.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      737 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/pleb/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      536 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/pleb/none_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1178 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/pleb/proxies.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7213 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/pleb/registry.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2311 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/pleb/scoped_property.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      412 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/pleb/singleton.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      731 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/pleb/threading.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.161856 tcex-3.0.9/tcex/services/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      324 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/services/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11874 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/services/api_service.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16230 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/services/common_service.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17548 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/services/common_service_trigger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10563 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/services/mqtt_message_broker.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15948 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/services/webhook_trigger_service.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.172666 tcex-3.0.9/tcex/sessions/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       40 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/sessions/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.198304 tcex-3.0.9/tcex/sessions/auth/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       31 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/sessions/auth/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1706 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/sessions/auth/hmac_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1539 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/sessions/auth/tc_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1835 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/sessions/auth/token_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12891 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/sessions/external_session.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4923 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/sessions/rate_limit_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4420 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/sessions/tc_session.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20160 2023-06-07 19:48:06.000000 tcex-3.0.9/tcex/tcex.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.203927 tcex-3.0.9/tcex/tokens/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       80 2020-09-04 22:24:44.000000 tcex-3.0.9/tcex/tokens/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12245 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/tokens/tokens.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.226880 tcex-3.0.9/tcex/utils/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       78 2020-09-04 22:24:44.000000 tcex-3.0.9/tcex/utils/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/utils/aes_operations.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10144 2022-06-29 14:32:21.000000 tcex-3.0.9/tcex/utils/datetime_operations.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7272 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/utils/file_operations.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:12.248646 tcex-3.0.9/tcex/utils/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      127 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/utils/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      667 2022-03-08 20:24:00.000000 tcex-3.0.9/tcex/utils/models/playbook_variable_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4889 2023-02-02 18:36:54.000000 tcex-3.0.9/tcex/utils/requests_to_curl.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7751 2023-02-07 21:10:46.000000 tcex-3.0.9/tcex/utils/string_operations.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6165 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/utils/utils.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7352 2022-11-14 21:07:06.000000 tcex-3.0.9/tcex/utils/variables.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-06-07 19:48:10.618128 tcex-3.0.9/tcex.egg-info/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-06-07 19:48:09.000000 tcex-3.0.9/tcex.egg-info/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14001 2023-06-07 19:48:10.000000 tcex-3.0.9/tcex.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-06-07 19:48:09.000000 tcex-3.0.9/tcex.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1019 2023-06-07 19:48:09.000000 tcex-3.0.9/tcex.egg-info/requires.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        5 2023-06-07 19:48:09.000000 tcex-3.0.9/tcex.egg-info/top_level.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-06-07 19:48:09.000000 tcex-3.0.9/tcex.egg-info/zip-safe
```

### Comparing `tcex-3.0.8/LICENSE` & `tcex-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/PKG-INFO` & `tcex-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tcex
-Version: 3.0.8
+Version: 3.0.9
 Summary: ThreatConnect Exchange App Framework
 Home-page: https://github.com/ThreatConnect-Inc/tcex
-Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.8
+Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.9
 Author: ThreatConnect (support@threatconnect.com)
 Author-email: support@threatconnect.com
 License: Apache License, Version 2
 Project-URL: Documentation, https://github.com/ThreatConnect-Inc/tcex
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `tcex-3.0.8/README.md` & `tcex-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/bin/tcex` & `tcex-3.0.9/bin/tcex`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/pyproject.toml` & `tcex-3.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/setup.cfg` & `tcex-3.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/setup.py` & `tcex-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/__init__.py` & `tcex-3.0.9/tcex/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/api.py` & `tcex-3.0.9/tcex/api/api.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/tc.py` & `tcex-3.0.9/tcex/api/tc/tc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/ti_transform/model/transform_model.py` & `tcex-3.0.9/tcex/api/tc/ti_transform/model/transform_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,17 @@
     # document
     malware: Optional[MetadataTransformModel] = Field(None, description='')
     password: Optional[MetadataTransformModel] = Field(None, description='')
     # email
     from_addr: Optional[MetadataTransformModel] = Field(None, description='')
     score: Optional[MetadataTransformModel] = Field(None, description='')
     to_addr: Optional[MetadataTransformModel] = Field(None, description='')
+    subject: Optional[MetadataTransformModel] = Field(None, description='')
+    body: Optional[MetadataTransformModel] = Field(None, description='')
+    header: Optional[MetadataTransformModel] = Field(None, description='')
     # event, incident
     event_date: Optional[DatetimeTransformModel] = Field(None, description='')
     status: Optional[MetadataTransformModel] = Field(None, description='')
     # report
     publish_date: Optional[DatetimeTransformModel] = Field(None, description='')
     # signature
     file_type: Optional[MetadataTransformModel] = Field(None, description='')
```

### Comparing `tcex-3.0.8/tcex/api/tc/ti_transform/ti_transform.py` & `tcex-3.0.9/tcex/api/tc/ti_transform/ti_transform.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/ti_transform/transform_abc.py` & `tcex-3.0.9/tcex/api/tc/ti_transform/transform_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,17 @@
             self._process_metadata('fileName', self.transform.file_name)
             self._process_metadata('malware', self.transform.malware)
             self._process_metadata('password', self.transform.confidence)
 
         if self.transformed_item['type'] == 'Email':
             self._process_metadata('from', self.transform.from_addr)
             self._process_metadata('to', self.transform.to_addr)
+            self._process_metadata('subject', self.transform.subject)
+            self._process_metadata('body', self.transform.body)
+            self._process_metadata('header', self.transform.header)
 
         if self.transformed_item['type'] in ('Event', 'Incident'):
             self._process_metadata_datetime('eventDate', self.transform.event_date)
             self._process_metadata('status', self.transform.status)
 
         if self.transformed_item['type'] == 'Report':
             self._process_metadata('fileName', self.transform.file_name)
```

### Comparing `tcex-3.0.8/tcex/api/tc/utils/threat_intel_utils.py` & `tcex-3.0.9/tcex/api/tc/utils/threat_intel_utils.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/attribute.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/batch.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/batch.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/batch_submit.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/batch_submit.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/batch_writer.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/batch_writer.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/group.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/indicator.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/security_label.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/batch/tag.py` & `tcex-3.0.9/tcex/api/tc/v2/batch/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/datastore/cache.py` & `tcex-3.0.9/tcex/api/tc/v2/datastore/cache.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/datastore/datastore.py` & `tcex-3.0.9/tcex/api/tc/v2/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/metrics/metrics.py` & `tcex-3.0.9/tcex/api/tc/v2/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/notifications/notifications.py` & `tcex-3.0.9/tcex/api/tc/v2/notifications/notifications.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/filters.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/filters.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/owner.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/owner.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tag.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tags.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/tags.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/task.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/task.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/victim.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/mappings/victim.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py` & `tcex-3.0.9/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v2/v2.py` & `tcex-3.0.9/tcex/api/tc/v2/v2.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/_gen.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_args_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_args_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_filter_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_filter_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_model_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_model_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_object_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/_gen_object_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/models/_filter_model.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/models/_filter_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/_gen/models/_property_model.py` & `tcex-3.0.9/tcex/api/tc/v3/_gen/models/_property_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/api_endpoints.py` & `tcex-3.0.9/tcex/api/tc/v3/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type.py` & `tcex-3.0.9/tcex/api/tc/v3/artifact_types/artifact_type.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/artifact_types/artifact_type_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_model.py` & `tcex-3.0.9/tcex/api/tc/v3/artifact_types/artifact_type_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact.py` & `tcex-3.0.9/tcex/api/tc/v3/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/artifacts/artifact_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_model.py` & `tcex-3.0.9/tcex/api/tc/v3/artifacts/artifact_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type.py` & `tcex-3.0.9/tcex/api/tc/v3/attribute_types/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/attribute_types/attribute_type_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_model.py` & `tcex-3.0.9/tcex/api/tc/v3/attribute_types/attribute_type_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/attributes/attribute_model.py` & `tcex-3.0.9/tcex/api/tc/v3/attributes/attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute.py` & `tcex-3.0.9/tcex/api/tc/v3/case_attributes/case_attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/case_attributes/case_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_model.py` & `tcex-3.0.9/tcex/api/tc/v3/case_attributes/case_attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/case_management/case_management.py` & `tcex-3.0.9/tcex/api/tc/v3/case_management/case_management.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/cases/case.py` & `tcex-3.0.9/tcex/api/tc/v3/cases/case.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/cases/case_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/cases/case_model.py` & `tcex-3.0.9/tcex/api/tc/v3/cases/case_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/file_actions/file_action_model.py` & `tcex-3.0.9/tcex/api/tc/v3/file_actions/file_action_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py` & `tcex-3.0.9/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/filter_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/filter_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute.py` & `tcex-3.0.9/tcex/api/tc/v3/group_attributes/group_attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/group_attributes/group_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_model.py` & `tcex-3.0.9/tcex/api/tc/v3/group_attributes/group_attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/groups/group.py` & `tcex-3.0.9/tcex/api/tc/v3/groups/group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/groups/group_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/groups/group_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/groups/group_model.py` & `tcex-3.0.9/tcex/api/tc/v3/groups/group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py` & `tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py` & `tcex-3.0.9/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/indicators/indicator.py` & `tcex-3.0.9/tcex/api/tc/v3/indicators/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/indicators/indicator_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_model.py` & `tcex-3.0.9/tcex/api/tc/v3/indicators/indicator_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/notes/note.py` & `tcex-3.0.9/tcex/api/tc/v3/notes/note.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/notes/note_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/notes/note_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/notes/note_model.py` & `tcex-3.0.9/tcex/api/tc/v3/notes/note_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/object_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/object_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/object_collection_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/object_collection_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/assignee_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/assignee_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_group_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/assignee_user_group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/assignee_user_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role.py` & `tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/owner_role.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/owner_roles/owner_role_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/owners/owner.py` & `tcex-3.0.9/tcex/api/tc/v3/security/owners/owner.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/security/owners/owner_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/owners/owner_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/security.py` & `tcex-3.0.9/tcex/api/tc/v3/security/security.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role.py` & `tcex-3.0.9/tcex/api/tc/v3/security/system_roles/system_role.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/security/system_roles/system_role_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/system_roles/system_role_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/task_assignee_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/task_assignee_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group.py` & `tcex-3.0.9/tcex/api/tc/v3/security/user_groups/user_group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/security/user_groups/user_group_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/user_groups/user_group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/users/user.py` & `tcex-3.0.9/tcex/api/tc/v3/security/users/user.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/users/user_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/security/users/user_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security/users/user_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security/users/user_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label.py` & `tcex-3.0.9/tcex/api/tc/v3/security_labels/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/security_labels/security_label_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_model.py` & `tcex-3.0.9/tcex/api/tc/v3/security_labels/security_label_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tags/tag.py` & `tcex-3.0.9/tcex/api/tc/v3/tags/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tags/tag_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/tags/tag_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tags/tag_model.py` & `tcex-3.0.9/tcex/api/tc/v3/tags/tag_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tasks/task.py` & `tcex-3.0.9/tcex/api/tc/v3/tasks/task.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tasks/task_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/tasks/task_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tasks/task_model.py` & `tcex-3.0.9/tcex/api/tc/v3/tasks/task_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py` & `tcex-3.0.9/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tql/tql.py` & `tcex-3.0.9/tcex/api/tc/v3/tql/tql.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/tql/tql_operator.py` & `tcex-3.0.9/tcex/api/tc/v3/tql/tql_operator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/v3.py` & `tcex-3.0.9/tcex/api/tc/v3/v3.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/v3_model_abc.py` & `tcex-3.0.9/tcex/api/tc/v3/v3_model_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         #    PUT methods instead of the POST fields.  This handles not sending owner field
         #    for tag.
         if method == 'POST' and nested is True and self._shared_type is True:
             method = 'PUT'
 
         # METHOD RULE: If the current method is in the property "methods" list the
         #     field should be included when available.
-        if method in property_.get('methods', []) and value:
+        if method in property_.get('methods', []) and (value or value in [0, False]):
             return True
 
         # DEFAULT RULE -> Fields should not be included unless the match a previous rule.
         return False
 
     # pylint: disable=too-many-return-statements
     def _calculate_nested_inclusion(self, method: str, mode: str, model: 'BaseModel') -> str:
```

### Comparing `tcex-3.0.8/tcex/api/tc/v3/v3_types.py` & `tcex-3.0.9/tcex/api/tc/v3/v3_types.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset.py` & `tcex-3.0.9/tcex/api/tc/v3/victim_assets/victim_asset.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/victim_assets/victim_asset_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_model.py` & `tcex-3.0.9/tcex/api/tc/v3/victim_assets/victim_asset_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute.py` & `tcex-3.0.9/tcex/api/tc/v3/victim_attributes/victim_attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py` & `tcex-3.0.9/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victims/victim.py` & `tcex-3.0.9/tcex/api/tc/v3/victims/victim.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victims/victim_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/victims/victim_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/victims/victim_model.py` & `tcex-3.0.9/tcex/api/tc/v3/victims/victim_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event.py` & `tcex-3.0.9/tcex/api/tc/v3/workflow_events/workflow_event.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/workflow_events/workflow_event_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_model.py` & `tcex-3.0.9/tcex/api/tc/v3/workflow_events/workflow_event_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template.py` & `tcex-3.0.9/tcex/api/tc/v3/workflow_templates/workflow_template.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py` & `tcex-3.0.9/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_model.py` & `tcex-3.0.9/tcex/api/tc/v3/workflow_templates/workflow_template_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/app_spec_yml.py` & `tcex-3.0.9/tcex/app_config/app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/install_json.py` & `tcex-3.0.9/tcex/app_config/install_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/install_json_update.py` & `tcex-3.0.9/tcex/app_config/install_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/install_json_validate.py` & `tcex-3.0.9/tcex/app_config/install_json_validate.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/job_json.py` & `tcex-3.0.9/tcex/app_config/job_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/layout_json.py` & `tcex-3.0.9/tcex/app_config/layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/models/app_spec_yml_model.py` & `tcex-3.0.9/tcex/app_config/models/app_spec_yml_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/models/install_json_model.py` & `tcex-3.0.9/tcex/app_config/models/install_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/models/job_json_model.py` & `tcex-3.0.9/tcex/app_config/models/job_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/models/layout_json_model.py` & `tcex-3.0.9/tcex/app_config/models/layout_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/models/tcex_json_model.py` & `tcex-3.0.9/tcex/app_config/models/tcex_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/models/template_config_model.py` & `tcex-3.0.9/tcex/app_config/models/template_config_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/permutation.py` & `tcex-3.0.9/tcex/app_config/permutation.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/tcex_json.py` & `tcex-3.0.9/tcex/app_config/tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_config/tcex_json_update.py` & `tcex-3.0.9/tcex/app_config/tcex_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/app_feature/advanced_request.py` & `tcex-3.0.9/tcex/app_feature/advanced_request.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/backports/__init__.py` & `tcex-3.0.9/tcex/backports/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/bin_abc.py` & `tcex-3.0.9/tcex/bin/bin_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/dep.py` & `tcex-3.0.9/tcex/bin/dep.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/deploy.py` & `tcex-3.0.9/tcex/bin/deploy.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/package.py` & `tcex-3.0.9/tcex/bin/package.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool.py` & `tcex-3.0.9/tcex/bin/spec_tool.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_app_input.py` & `tcex-3.0.9/tcex/bin/spec_tool_app_input.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_app_input_static.py` & `tcex-3.0.9/tcex/bin/spec_tool_app_input_static.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_app_spec_yml.py` & `tcex-3.0.9/tcex/bin/spec_tool_app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_install_json.py` & `tcex-3.0.9/tcex/bin/spec_tool_install_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_job_json.py` & `tcex-3.0.9/tcex/bin/spec_tool_job_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_layout_json.py` & `tcex-3.0.9/tcex/bin/spec_tool_layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_readme_md.py` & `tcex-3.0.9/tcex/bin/spec_tool_readme_md.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/spec_tool_tcex_json.py` & `tcex-3.0.9/tcex/bin/spec_tool_tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/template.py` & `tcex-3.0.9/tcex/bin/template.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/bin/validate.py` & `tcex-3.0.9/tcex/bin/validate.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/decorators/benchmark.py` & `tcex-3.0.9/tcex/decorators/benchmark.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/decorators/debug.py` & `tcex-3.0.9/tcex/decorators/debug.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/decorators/fail_on_output.py` & `tcex-3.0.9/tcex/decorators/fail_on_output.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/decorators/on_exception.py` & `tcex-3.0.9/tcex/decorators/on_exception.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/decorators/on_success.py` & `tcex-3.0.9/tcex/decorators/on_success.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/decorators/output.py` & `tcex-3.0.9/tcex/decorators/output.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/exit/error_codes.py` & `tcex-3.0.9/tcex/exit/error_codes.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/exit/exit.py` & `tcex-3.0.9/tcex/exit/exit.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/__init__.py` & `tcex-3.0.9/tcex/input/field_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/binary.py` & `tcex-3.0.9/tcex/input/field_types/binary.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/case_management_entity.py` & `tcex-3.0.9/tcex/input/field_types/case_management_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/choice.py` & `tcex-3.0.9/tcex/input/field_types/choice.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/datetime.py` & `tcex-3.0.9/tcex/input/field_types/datetime.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/edit_choice.py` & `tcex-3.0.9/tcex/input/field_types/edit_choice.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/exception.py` & `tcex-3.0.9/tcex/input/field_types/exception.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/group_entity.py` & `tcex-3.0.9/tcex/input/field_types/group_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/indicator_entity.py` & `tcex-3.0.9/tcex/input/field_types/indicator_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/integer.py` & `tcex-3.0.9/tcex/input/field_types/integer.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/ip_address.py` & `tcex-3.0.9/tcex/input/field_types/ip_address.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/key_value.py` & `tcex-3.0.9/tcex/input/field_types/key_value.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/sensitive.py` & `tcex-3.0.9/tcex/input/field_types/sensitive.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/string.py` & `tcex-3.0.9/tcex/input/field_types/string.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/tc_entity.py` & `tcex-3.0.9/tcex/input/field_types/tc_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/field_types/validators.py` & `tcex-3.0.9/tcex/input/field_types/validators.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/input.py` & `tcex-3.0.9/tcex/input/input.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/__init__.py` & `tcex-3.0.9/tcex/input/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/advanced_request_model.py` & `tcex-3.0.9/tcex/input/models/advanced_request_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/aot_execution_enabled_model.py` & `tcex-3.0.9/tcex/input/models/aot_execution_enabled_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/api_model.py` & `tcex-3.0.9/tcex/input/models/api_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/batch_model.py` & `tcex-3.0.9/tcex/input/models/batch_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/cal_settings_model.py` & `tcex-3.0.9/tcex/input/models/cal_settings_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/create_config_model.py` & `tcex-3.0.9/tcex/input/models/create_config_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/logging_model.py` & `tcex-3.0.9/tcex/input/models/logging_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/model_map.py` & `tcex-3.0.9/tcex/input/models/model_map.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/path_model.py` & `tcex-3.0.9/tcex/input/models/path_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/playbook_common_model.py` & `tcex-3.0.9/tcex/input/models/playbook_common_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 """Playbook Common Model"""
+# standard library
+from typing import Optional
+
 # third-party
 from pydantic import BaseModel, Field
 
+# first-party
+from tcex.input.field_types.sensitive import Sensitive
+
 
 class PlaybookCommonModel(BaseModel):
     """Playbook Common Model
 
     Supported for the following runtimeLevel:
     * ApiService
     * Playbook
@@ -20,20 +26,30 @@
     )
     tc_kvstore_host: str = Field(
         'localhost',
         alias='tc_playbook_db_path',
         description='The KV Store hostname.',
         inclusion_reason='runtimeLevel',
     )
+    tc_kvstore_pass: Optional[Sensitive] = Field(
+        None,
+        description='The KV Store password.',
+        inclusion_reason='runtimeLevel',
+    )
     tc_kvstore_port: int = Field(
         6379,
         alias='tc_playbook_db_port',
         description='The KV Store port number.',
         inclusion_reason='runtimeLevel',
     )
+    tc_kvstore_user: Optional[str] = Field(
+        None,
+        description='The KV Store username.',
+        inclusion_reason='runtimeLevel',
+    )
     tc_kvstore_type: str = Field(
         'Redis',
         alias='tc_playbook_db_type',
         description='The KV Store type (Redis or TCKeyValueAPI).',
         inclusion_reason='runtimeLevel',
     )
     tc_playbook_kvstore_id: int = Field(
```

### Comparing `tcex-3.0.8/tcex/input/models/playbook_model.py` & `tcex-3.0.9/tcex/input/models/playbook_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/proxy_model.py` & `tcex-3.0.9/tcex/input/models/proxy_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/service_model.py` & `tcex-3.0.9/tcex/input/models/service_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/input/models/smtp_settings_model.py` & `tcex-3.0.9/tcex/input/models/smtp_settings_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/key_value_store/key_value_abc.py` & `tcex-3.0.9/tcex/key_value_store/key_value_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/key_value_store/key_value_api.py` & `tcex-3.0.9/tcex/key_value_store/key_value_api.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/key_value_store/key_value_mock.py` & `tcex-3.0.9/tcex/key_value_store/key_value_mock.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/key_value_store/key_value_redis.py` & `tcex-3.0.9/tcex/key_value_store/key_value_redis.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/key_value_store/redis_client.py` & `tcex-3.0.9/tcex/key_value_store/redis_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""TcEx Framework Redis Module"""
-# standard library
-from typing import Optional
-
+"""TcEx Framework Module"""
 # third-party
 import redis
 
 # first-party
 from tcex.backports import cached_property
 
 
@@ -25,24 +22,33 @@
         password (str, kwargs): The REDIS password.
         socket_timeout (int, kwargs): The REDIS socket timeout.
         timeout (int, kwargs): The REDIS Blocking Connection Pool timeout value.
     """
 
     def __init__(
         self,
-        host: Optional[str] = 'localhost',
-        port: Optional[int] = 6379,
-        db: Optional[int] = 0,
-        blocking_pool: Optional[bool] = False,
-        **kwargs
+        host: str = 'localhost',
+        port: int = 6379,
+        db: int = 0,
+        blocking_pool: bool = False,
+        **kwargs,
     ):
         """Initialize class properties"""
+        password = kwargs.pop('password', None)
+        username = kwargs.pop('username', None)
+
         pool = redis.ConnectionPool
         if blocking_pool:
             kwargs.pop('blocking_pool')  # remove blocking_pool key
             pool = redis.BlockingConnectionPool
-        self.pool = pool(host=host, port=port, db=db, **kwargs)
+
+        if username and password:
+            self.pool = pool(
+                host=host, port=port, db=db, username=username, password=password, **kwargs
+            )
+        else:
+            self.pool = pool(host=host, port=port, db=db, **kwargs)
 
     @cached_property
-    def client(self) -> 'redis.Redis':
+    def client(self) -> redis.Redis:
         """Return an instance of redis.client.Redis."""
         return redis.Redis(connection_pool=self.pool)
```

### Comparing `tcex-3.0.8/tcex/logger/api_handler.py` & `tcex-3.0.9/tcex/logger/api_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/logger/cache_handler.py` & `tcex-3.0.9/tcex/logger/cache_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/logger/logger.py` & `tcex-3.0.9/tcex/logger/logger.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/logger/pattern_file_handler.py` & `tcex-3.0.9/tcex/logger/pattern_file_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/logger/rotating_file_handler_custom.py` & `tcex-3.0.9/tcex/logger/rotating_file_handler_custom.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/logger/sensitive_filter.py` & `tcex-3.0.9/tcex/logger/sensitive_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """TcEx logging filter module"""
 # standard library
 import logging
+from threading import Lock
 
 
 class SensitiveFilter(logging.Filter):
     """Sensitive Log Filter"""
 
     def __init__(self, name=''):
         """Plug in a new filter to an existing formatter"""
         super().__init__(name)
         self._sensitive_registry = set()
+        self._lock = Lock()
 
     def add(self, value: str):
         """Add sensitive value to registry."""
         if value:
-            # don't add empty string
-            self._sensitive_registry.add(str(value))
+            with self._lock:
+                # don't add empty string
+                self._sensitive_registry.add(str(value))
 
     def filter(self, record: logging.LogRecord) -> bool:
         """Filter the record"""
         # have to sniff the msg and args values of the LogRecord
         record.msg = self.replace(record.getMessage())
         record.args = {}
         return True
 
     def replace(self, obj: str):
         """Replace any sensitive data in the object if its a string"""
-        for replacement in self._sensitive_registry:
-            obj = obj.replace(replacement, '***')
+        with self._lock:
+            for replacement in self._sensitive_registry:
+                obj = obj.replace(replacement, '***')
         return obj
```

### Comparing `tcex-3.0.8/tcex/logger/thread_file_handler.py` & `tcex-3.0.9/tcex/logger/thread_file_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/logger/trace_logger.py` & `tcex-3.0.9/tcex/logger/trace_logger.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/playbook/playbook.py` & `tcex-3.0.9/tcex/playbook/playbook.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/playbook/playbook_create.py` & `tcex-3.0.9/tcex/playbook/playbook_create.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/playbook/playbook_delete.py` & `tcex-3.0.9/tcex/playbook/playbook_delete.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/playbook/playbook_output.py` & `tcex-3.0.9/tcex/playbook/playbook_output.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/playbook/playbook_read.py` & `tcex-3.0.9/tcex/playbook/playbook_read.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/env_path.py` & `tcex-3.0.9/tcex/pleb/env_path.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/event.py` & `tcex-3.0.9/tcex/pleb/event.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/none_model.py` & `tcex-3.0.9/tcex/pleb/none_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/proxies.py` & `tcex-3.0.9/tcex/pleb/proxies.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/registry.py` & `tcex-3.0.9/tcex/pleb/registry.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/scoped_property.py` & `tcex-3.0.9/tcex/pleb/scoped_property.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/pleb/threading.py` & `tcex-3.0.9/tcex/pleb/threading.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/services/api_service.py` & `tcex-3.0.9/tcex/services/api_service.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/services/common_service.py` & `tcex-3.0.9/tcex/services/common_service.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/services/common_service_trigger.py` & `tcex-3.0.9/tcex/services/common_service_trigger.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/services/mqtt_message_broker.py` & `tcex-3.0.9/tcex/services/mqtt_message_broker.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/services/webhook_trigger_service.py` & `tcex-3.0.9/tcex/services/webhook_trigger_service.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/sessions/auth/hmac_auth.py` & `tcex-3.0.9/tcex/sessions/auth/hmac_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/sessions/auth/tc_auth.py` & `tcex-3.0.9/tcex/sessions/auth/tc_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/sessions/auth/token_auth.py` & `tcex-3.0.9/tcex/sessions/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/sessions/external_session.py` & `tcex-3.0.9/tcex/sessions/external_session.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/sessions/rate_limit_handler.py` & `tcex-3.0.9/tcex/sessions/rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/sessions/tc_session.py` & `tcex-3.0.9/tcex/sessions/tc_session.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/tcex.py` & `tcex-3.0.9/tcex/tcex.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 import os
 import platform
 import signal
 import threading
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 # third-party
+from redis import Redis
 from requests import Session
 
 # first-party
 from tcex.api import API
 from tcex.api.tc.utils.threat_intel_utils import ThreatIntelUtils
 from tcex.api.tc.v2.v2 import V2
 from tcex.api.tc.v3.v3 import V3
 from tcex.app_config.install_json import InstallJson
 from tcex.app_feature import AdvancedRequest
 from tcex.backports import cached_property
 from tcex.exit.exit import ExitCode, ExitService
+from tcex.input.field_types.sensitive import Sensitive
 from tcex.input.input import Input
 from tcex.key_value_store import KeyValueApi, KeyValueMock, KeyValueRedis, RedisClient
 from tcex.logger.logger import Logger  # pylint: disable=no-name-in-module
 from tcex.playbook import Playbook
 from tcex.pleb.proxies import proxies
 from tcex.pleb.registry import registry
 from tcex.pleb.scoped_property import scoped_property
@@ -194,33 +196,37 @@
                 startup, but for service Apps each request gets different outputs.
         """
         return Playbook(self.key_value_store, context, output_variables)
 
     @staticmethod
     def get_redis_client(
         host: str, port: int, db: int = 0, blocking_pool: bool = False, **kwargs
-    ) -> 'RedisClient':
+    ) -> Redis:
         """Return a *new* instance of Redis client.
 
         For a full list of kwargs see https://redis-py.readthedocs.io/en/latest/#redis.Connection.
 
         Args:
             host: The REDIS host. Defaults to localhost.
             port: The REDIS port. Defaults to 6379.
             db: The REDIS db. Defaults to 0.
             blocking_pool: Use BlockingConnectionPool instead of ConnectionPool.
-            errors (str, kwargs): The REDIS errors policy (e.g. strict).
-            max_connections (int, kwargs): The maximum number of connections to REDIS.
-            password (str, kwargs): The REDIS password.
-            socket_timeout (int, kwargs): The REDIS socket timeout.
-            timeout (int, kwargs): The REDIS Blocking Connection Pool timeout value.
+            **kwargs: Additional keyword arguments.
 
-        Returns:
-            Redis.client: An instance of redis client.
+        Keyword Args:
+            errors (str): The REDIS errors policy (e.g. strict).
+            max_connections (int): The maximum number of connections to REDIS.
+            password (Sensitive): The REDIS password.
+            socket_timeout (int): The REDIS socket timeout.
+            timeout (int): The REDIS Blocking Connection Pool timeout value.
+            username (str): The REDIS username.
         """
+        # get value from Sensitive value before passing to Redis
+        password = kwargs.get('password')
+        kwargs['password'] = password.value if isinstance(password, Sensitive) else password
         return RedisClient(
             host=host, port=port, db=db, blocking_pool=blocking_pool, **kwargs
         ).client
 
     def get_session_tc(
         self,
         auth: Optional[Union['HmacAuth', 'TokenAuth', 'TcAuth']] = None,
@@ -401,20 +407,22 @@
             proxy_port=self.inputs.model_unresolved.tc_proxy_port,
             proxy_user=self.inputs.model_unresolved.tc_proxy_username,
             proxy_pass=self.inputs.model_unresolved.tc_proxy_password,
         )
 
     @registry.factory(RedisClient)
     @scoped_property
-    def redis_client(self) -> 'RedisClient':
+    def redis_client(self) -> Redis:
         """Return redis client instance configure for Playbook/Service Apps."""
         return self.get_redis_client(
             host=self.inputs.contents.get('tc_kvstore_host'),
             port=self.inputs.contents.get('tc_kvstore_port'),
             db=0,
+            username=self.inputs.contents.get('tc_kvstore_user'),
+            password=self.inputs.contents.get('tc_kvstore_pass'),
         )
 
     def results_tc(self, key: str, value: str):
         """Write data to results_tc file in TcEX specified directory.
 
         The TcEx platform support persistent values between executions of the App.  This
         method will store the values for TC to read and put into the Database.
```

### Comparing `tcex-3.0.8/tcex/tokens/tokens.py` & `tcex-3.0.9/tcex/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/aes_operations.py` & `tcex-3.0.9/tcex/utils/aes_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/datetime_operations.py` & `tcex-3.0.9/tcex/utils/datetime_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/file_operations.py` & `tcex-3.0.9/tcex/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/models/playbook_variable_model.py` & `tcex-3.0.9/tcex/utils/models/playbook_variable_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/requests_to_curl.py` & `tcex-3.0.9/tcex/utils/requests_to_curl.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/string_operations.py` & `tcex-3.0.9/tcex/utils/string_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/utils.py` & `tcex-3.0.9/tcex/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex/utils/variables.py` & `tcex-3.0.9/tcex/utils/variables.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex.egg-info/PKG-INFO` & `tcex-3.0.9/tcex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tcex
-Version: 3.0.8
+Version: 3.0.9
 Summary: ThreatConnect Exchange App Framework
 Home-page: https://github.com/ThreatConnect-Inc/tcex
-Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.8
+Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.9
 Author: ThreatConnect (support@threatconnect.com)
 Author-email: support@threatconnect.com
 License: Apache License, Version 2
 Project-URL: Documentation, https://github.com/ThreatConnect-Inc/tcex
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `tcex-3.0.8/tcex.egg-info/SOURCES.txt` & `tcex-3.0.9/tcex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tcex-3.0.8/tcex.egg-info/requires.txt` & `tcex-3.0.9/tcex.egg-info/requires.txt`

 * *Files identical despite different names*

