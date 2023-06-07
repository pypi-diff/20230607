# Comparing `tmp/django_workflow_engine-0.1.1.tar.gz` & `tmp/django_workflow_engine-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_workflow_engine-0.1.1.tar", max compression
+gzip compressed data, was "django_workflow_engine-0.2.0.tar", max compression
```

## Comparing `django_workflow_engine-0.1.1.tar` & `django_workflow_engine-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1091 2022-10-21 12:03:38.269790 django_workflow_engine-0.1.1/LICENSE
--rw-r--r--   0        0        0      903 2022-10-21 12:03:38.270132 django_workflow_engine-0.1.1/django_workflow_engine/__init__.py
--rw-r--r--   0        0        0      162 2022-10-21 12:03:38.270209 django_workflow_engine-0.1.1/django_workflow_engine/apps.py
--rw-r--r--   0        0        0     2897 2022-10-21 12:03:38.270294 django_workflow_engine-0.1.1/django_workflow_engine/dataclass.py
--rw-r--r--   0        0        0      238 2022-10-21 12:03:38.270370 django_workflow_engine-0.1.1/django_workflow_engine/exceptions.py
--rw-r--r--   0        0        0     7366 2023-05-04 12:21:29.108299 django_workflow_engine-0.1.1/django_workflow_engine/executor.py
--rw-r--r--   0        0        0     2412 2022-10-21 12:03:38.270560 django_workflow_engine-0.1.1/django_workflow_engine/generate_urls.py
--rw-r--r--   0        0        0        0 2023-05-04 12:21:29.106950 django_workflow_engine-0.1.1/django_workflow_engine/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:21:29.107024 django_workflow_engine-0.1.1/django_workflow_engine/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-05-04 12:21:29.108598 django_workflow_engine-0.1.1/django_workflow_engine/management/commands/cleanup_workflow_engine.py
--rw-r--r--   0        0        0     4162 2022-10-21 12:03:38.270677 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0001_initial.py
--rw-r--r--   0        0        0      428 2022-10-21 12:03:38.270765 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0002_alter_flow_workflow_name.py
--rw-r--r--   0        0        0      416 2022-10-21 12:03:38.270829 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0003_taskrecord_broke_flow.py
--rw-r--r--   0        0        0     1259 2022-10-21 12:03:38.270912 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0004_auto_20211116_0823.py
--rw-r--r--   0        0        0      400 2022-10-21 12:03:38.270991 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0005_rename_finished_at_taskrecord_executed_at.py
--rw-r--r--   0        0        0      427 2022-10-21 12:03:38.271064 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0006_taskrecord_done.py
--rw-r--r--   0        0        0      398 2022-10-21 12:03:38.271129 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0007_flow_running.py
--rw-r--r--   0        0        0      345 2022-10-21 12:03:38.271203 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0008_remove_taskrecord_broke_flow.py
--rw-r--r--   0        0        0     1211 2023-03-16 11:13:49.239841 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0009_rename_taskrecord_taskrecordexecution_and_create_new_taskstatus.py
--rw-r--r--   0        0        0     3924 2023-05-04 12:21:29.109390 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0010_create_replacement_task_record.py
--rw-r--r--   0        0        0     2940 2023-05-04 12:21:29.108775 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0011_migrate_from_taskrecordexecutions.py
--rw-r--r--   0        0        0     1169 2023-05-04 12:21:29.108693 django_workflow_engine-0.1.1/django_workflow_engine/migrations/0012_alter_target_unique_together.py
--rw-r--r--   0        0        0        0 2022-10-21 12:03:38.271234 django_workflow_engine-0.1.1/django_workflow_engine/migrations/__init__.py
--rw-r--r--   0        0        0     4935 2023-05-04 12:21:29.108852 django_workflow_engine-0.1.1/django_workflow_engine/models.py
--rw-r--r--   0        0        0      193 2022-10-21 12:03:38.271436 django_workflow_engine-0.1.1/django_workflow_engine/tasks/__init__.py
--rw-r--r--   0        0        0      717 2023-03-16 11:13:49.240056 django_workflow_engine-0.1.1/django_workflow_engine/tasks/email_form.py
--rw-r--r--   0        0        0     1229 2023-03-16 11:13:49.240145 django_workflow_engine-0.1.1/django_workflow_engine/tasks/previous_tasks_complete.py
--rw-r--r--   0        0        0      761 2023-03-16 11:13:49.240923 django_workflow_engine-0.1.1/django_workflow_engine/tasks/send_email.py
--rw-r--r--   0        0        0     1972 2023-03-16 11:13:49.241001 django_workflow_engine-0.1.1/django_workflow_engine/tasks/task.py
--rw-r--r--   0        0        0      260 2022-10-21 12:03:38.271905 django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow-continue.html
--rw-r--r--   0        0        0      804 2023-03-16 11:13:49.241105 django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_detail.html
--rw-r--r--   0        0        0     2694 2022-10-21 12:03:38.272045 django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_diagram.html
--rw-r--r--   0        0        0       97 2022-10-21 12:03:38.272108 django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_form.html
--rw-r--r--   0        0        0      870 2022-10-21 12:03:38.272176 django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_list.html
--rw-r--r--   0        0        0      666 2023-03-16 11:13:49.241229 django_workflow_engine-0.1.1/django_workflow_engine/templates/includes/requirement_summary.html
--rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272344 django_workflow_engine-0.1.1/django_workflow_engine/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272379 django_workflow_engine-0.1.1/django_workflow_engine/tests/conftest.py
--rw-r--r--   0        0        0      542 2022-10-21 12:03:38.272450 django_workflow_engine-0.1.1/django_workflow_engine/tests/factories.py
--rw-r--r--   0        0        0     1662 2022-10-21 12:03:38.272525 django_workflow_engine-0.1.1/django_workflow_engine/tests/tasks.py
--rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272562 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_create_view.py
--rw-r--r--   0        0        0      400 2022-10-21 12:03:38.272661 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_creation.py
--rw-r--r--   0        0        0       91 2022-10-21 12:03:38.272730 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_django.py
--rw-r--r--   0        0        0     1392 2022-10-21 12:03:38.272824 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_task_info.py
--rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272891 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_views/__init__.py
--rw-r--r--   0        0        0       90 2022-10-21 12:03:38.272967 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_views/test_continue_view.py
--rw-r--r--   0        0        0       64 2022-10-21 12:03:38.273028 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_views/test_delete_view.py
--rw-r--r--   0        0        0       78 2022-10-21 12:03:38.273091 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_views/test_diagram_view.py
--rw-r--r--   0        0        0       66 2022-10-21 12:03:38.273148 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_views/test_list_view.py
--rw-r--r--   0        0        0       82 2022-10-21 12:03:38.273218 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_views/test_view.py
--rw-r--r--   0        0        0        0 2022-10-21 12:03:38.273277 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/__init__.py
--rw-r--r--   0        0        0      648 2023-03-16 11:13:49.241343 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_linear_workflow.py
--rw-r--r--   0        0        0     3407 2023-03-08 14:10:13.489432 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_loops.py
--rw-r--r--   0        0        0     1443 2023-03-16 11:13:49.241440 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_pause_task.py
--rw-r--r--   0        0        0     2832 2023-03-16 11:13:49.241594 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_previous_tasks_complete.py
--rw-r--r--   0        0        0     1661 2023-03-16 11:13:49.241749 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_reminder_workflow.py
--rw-r--r--   0        0        0      713 2023-03-16 11:13:49.241939 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_split_and_join_workflow.py
--rw-r--r--   0        0        0      711 2023-03-16 11:13:49.242400 django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_split_workflow.py
--rw-r--r--   0        0        0      549 2022-10-21 12:03:38.273913 django_workflow_engine-0.1.1/django_workflow_engine/tests/utils.py
--rw-r--r--   0        0        0     7263 2022-10-21 12:03:38.273998 django_workflow_engine-0.1.1/django_workflow_engine/tests/workflows.py
--rw-r--r--   0        0        0     2416 2023-03-16 14:24:24.282527 django_workflow_engine-0.1.1/django_workflow_engine/utils.py
--rw-r--r--   0        0        0     7753 2023-03-16 11:13:49.242074 django_workflow_engine-0.1.1/django_workflow_engine/views.py
--rw-r--r--   0        0        0     2155 2023-05-04 12:44:00.549513 django_workflow_engine-0.1.1/docs/index.md
--rw-r--r--   0        0        0      996 2023-05-30 14:08:54.160614 django_workflow_engine-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 django_workflow_engine-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-10-21 12:03:38.269790 django_workflow_engine-0.2.0/LICENSE
+-rw-r--r--   0        0        0      903 2022-10-21 12:03:38.270132 django_workflow_engine-0.2.0/django_workflow_engine/__init__.py
+-rw-r--r--   0        0        0      162 2022-10-21 12:03:38.270209 django_workflow_engine-0.2.0/django_workflow_engine/apps.py
+-rw-r--r--   0        0        0     2897 2022-10-21 12:03:38.270294 django_workflow_engine-0.2.0/django_workflow_engine/dataclass.py
+-rw-r--r--   0        0        0      238 2022-10-21 12:03:38.270370 django_workflow_engine-0.2.0/django_workflow_engine/exceptions.py
+-rw-r--r--   0        0        0     7554 2023-06-06 13:34:31.443353 django_workflow_engine-0.2.0/django_workflow_engine/executor.py
+-rw-r--r--   0        0        0     2412 2022-10-21 12:03:38.270560 django_workflow_engine-0.2.0/django_workflow_engine/generate_urls.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:21:29.106950 django_workflow_engine-0.2.0/django_workflow_engine/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:21:29.107024 django_workflow_engine-0.2.0/django_workflow_engine/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-05-04 12:21:29.108598 django_workflow_engine-0.2.0/django_workflow_engine/management/commands/cleanup_workflow_engine.py
+-rw-r--r--   0        0        0     4162 2022-10-21 12:03:38.270677 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0001_initial.py
+-rw-r--r--   0        0        0      428 2022-10-21 12:03:38.270765 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0002_alter_flow_workflow_name.py
+-rw-r--r--   0        0        0      416 2022-10-21 12:03:38.270829 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0003_taskrecord_broke_flow.py
+-rw-r--r--   0        0        0     1259 2022-10-21 12:03:38.270912 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0004_auto_20211116_0823.py
+-rw-r--r--   0        0        0      400 2022-10-21 12:03:38.270991 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0005_rename_finished_at_taskrecord_executed_at.py
+-rw-r--r--   0        0        0      427 2022-10-21 12:03:38.271064 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0006_taskrecord_done.py
+-rw-r--r--   0        0        0      398 2022-10-21 12:03:38.271129 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0007_flow_running.py
+-rw-r--r--   0        0        0      345 2022-10-21 12:03:38.271203 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0008_remove_taskrecord_broke_flow.py
+-rw-r--r--   0        0        0     1211 2023-03-16 11:13:49.239841 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0009_rename_taskrecord_taskrecordexecution_and_create_new_taskstatus.py
+-rw-r--r--   0        0        0     3924 2023-05-04 12:21:29.109390 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0010_create_replacement_task_record.py
+-rw-r--r--   0        0        0     2940 2023-05-04 12:21:29.108775 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0011_migrate_from_taskrecordexecutions.py
+-rw-r--r--   0        0        0     1169 2023-05-04 12:21:29.108693 django_workflow_engine-0.2.0/django_workflow_engine/migrations/0012_alter_target_unique_together.py
+-rw-r--r--   0        0        0        0 2022-10-21 12:03:38.271234 django_workflow_engine-0.2.0/django_workflow_engine/migrations/__init__.py
+-rw-r--r--   0        0        0     4935 2023-05-04 12:21:29.108852 django_workflow_engine-0.2.0/django_workflow_engine/models.py
+-rw-r--r--   0        0        0      193 2022-10-21 12:03:38.271436 django_workflow_engine-0.2.0/django_workflow_engine/tasks/__init__.py
+-rw-r--r--   0        0        0      717 2023-03-16 11:13:49.240056 django_workflow_engine-0.2.0/django_workflow_engine/tasks/email_form.py
+-rw-r--r--   0        0        0     1229 2023-03-16 11:13:49.240145 django_workflow_engine-0.2.0/django_workflow_engine/tasks/previous_tasks_complete.py
+-rw-r--r--   0        0        0      761 2023-03-16 11:13:49.240923 django_workflow_engine-0.2.0/django_workflow_engine/tasks/send_email.py
+-rw-r--r--   0        0        0     1972 2023-03-16 11:13:49.241001 django_workflow_engine-0.2.0/django_workflow_engine/tasks/task.py
+-rw-r--r--   0        0        0      260 2022-10-21 12:03:38.271905 django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow-continue.html
+-rw-r--r--   0        0        0      804 2023-03-16 11:13:49.241105 django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_detail.html
+-rw-r--r--   0        0        0     2694 2022-10-21 12:03:38.272045 django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_diagram.html
+-rw-r--r--   0        0        0       97 2022-10-21 12:03:38.272108 django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_form.html
+-rw-r--r--   0        0        0      870 2022-10-21 12:03:38.272176 django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_list.html
+-rw-r--r--   0        0        0      666 2023-03-16 11:13:49.241229 django_workflow_engine-0.2.0/django_workflow_engine/templates/includes/requirement_summary.html
+-rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272344 django_workflow_engine-0.2.0/django_workflow_engine/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272379 django_workflow_engine-0.2.0/django_workflow_engine/tests/conftest.py
+-rw-r--r--   0        0        0      542 2022-10-21 12:03:38.272450 django_workflow_engine-0.2.0/django_workflow_engine/tests/factories.py
+-rw-r--r--   0        0        0     1801 2023-06-06 13:31:01.256066 django_workflow_engine-0.2.0/django_workflow_engine/tests/tasks.py
+-rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272562 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_create_view.py
+-rw-r--r--   0        0        0      400 2022-10-21 12:03:38.272661 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_creation.py
+-rw-r--r--   0        0        0       91 2022-10-21 12:03:38.272730 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_django.py
+-rw-r--r--   0        0        0     1392 2022-10-21 12:03:38.272824 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_task_info.py
+-rw-r--r--   0        0        0        0 2022-10-21 12:03:38.272891 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_views/__init__.py
+-rw-r--r--   0        0        0       90 2022-10-21 12:03:38.272967 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_views/test_continue_view.py
+-rw-r--r--   0        0        0       64 2022-10-21 12:03:38.273028 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_views/test_delete_view.py
+-rw-r--r--   0        0        0       78 2022-10-21 12:03:38.273091 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_views/test_diagram_view.py
+-rw-r--r--   0        0        0       66 2022-10-21 12:03:38.273148 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_views/test_list_view.py
+-rw-r--r--   0        0        0       82 2022-10-21 12:03:38.273218 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_views/test_view.py
+-rw-r--r--   0        0        0        0 2022-10-21 12:03:38.273277 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/__init__.py
+-rw-r--r--   0        0        0     1204 2023-06-06 13:41:34.719063 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_linear_workflow.py
+-rw-r--r--   0        0        0     3407 2023-03-08 14:10:13.489432 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_loops.py
+-rw-r--r--   0        0        0     1443 2023-03-16 11:13:49.241440 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_pause_task.py
+-rw-r--r--   0        0        0     2832 2023-03-16 11:13:49.241594 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_previous_tasks_complete.py
+-rw-r--r--   0        0        0     1661 2023-03-16 11:13:49.241749 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_reminder_workflow.py
+-rw-r--r--   0        0        0     1397 2023-06-06 13:40:48.382572 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_split_and_join_workflow.py
+-rw-r--r--   0        0        0     1368 2023-06-06 13:40:34.598898 django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_split_workflow.py
+-rw-r--r--   0        0        0      549 2022-10-21 12:03:38.273913 django_workflow_engine-0.2.0/django_workflow_engine/tests/utils.py
+-rw-r--r--   0        0        0     7263 2022-10-21 12:03:38.273998 django_workflow_engine-0.2.0/django_workflow_engine/tests/workflows.py
+-rw-r--r--   0        0        0     2416 2023-03-16 14:24:24.282527 django_workflow_engine-0.2.0/django_workflow_engine/utils.py
+-rw-r--r--   0        0        0     7753 2023-03-16 11:13:49.242074 django_workflow_engine-0.2.0/django_workflow_engine/views.py
+-rw-r--r--   0        0        0     2155 2023-05-04 12:44:00.549513 django_workflow_engine-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      996 2023-06-07 15:28:16.025153 django_workflow_engine-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 django_workflow_engine-0.2.0/PKG-INFO
```

### Comparing `django_workflow_engine-0.1.1/LICENSE` & `django_workflow_engine-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/__init__.py` & `django_workflow_engine-0.2.0/django_workflow_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/dataclass.py` & `django_workflow_engine-0.2.0/django_workflow_engine/dataclass.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/executor.py` & `django_workflow_engine-0.2.0/django_workflow_engine/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import TYPE_CHECKING, List, Tuple, Type
+from typing import TYPE_CHECKING, List, Optional, Tuple, Type
 
 from django.contrib.auth import get_user_model
 from django.utils import timezone
 
 from django_workflow_engine import COMPLETE
 from django_workflow_engine.exceptions import WorkflowError, WorkflowNotAuthError
 from django_workflow_engine.models import Target, TaskStatus
@@ -78,15 +78,22 @@
 
         # If there is nothing to execute, then we are done.
         if not current_steps:
             return break_flow
 
         # Execute the steps.
         for current_step in current_steps:
-            current_step_break_flow = self.execute_step(user=user, step=current_step)
+            try:
+                current_step_break_flow = self.execute_step(
+                    user=user, step=current_step
+                )
+            except Exception as e:
+                logger.exception(e)
+                current_step_break_flow = True
+
             # We want to toggle break_flow to True, but not back to False.
             if current_step_break_flow:
                 break_flow = True
 
         # If we have broken the flow, then we are done, any remaining tasks will
         # be picked up next time.
         if break_flow:
```

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/generate_urls.py` & `django_workflow_engine-0.2.0/django_workflow_engine/generate_urls.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/management/commands/cleanup_workflow_engine.py` & `django_workflow_engine-0.2.0/django_workflow_engine/management/commands/cleanup_workflow_engine.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/migrations/0001_initial.py` & `django_workflow_engine-0.2.0/django_workflow_engine/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/migrations/0004_auto_20211116_0823.py` & `django_workflow_engine-0.2.0/django_workflow_engine/migrations/0004_auto_20211116_0823.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/migrations/0009_rename_taskrecord_taskrecordexecution_and_create_new_taskstatus.py` & `django_workflow_engine-0.2.0/django_workflow_engine/migrations/0009_rename_taskrecord_taskrecordexecution_and_create_new_taskstatus.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/migrations/0010_create_replacement_task_record.py` & `django_workflow_engine-0.2.0/django_workflow_engine/migrations/0010_create_replacement_task_record.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/migrations/0011_migrate_from_taskrecordexecutions.py` & `django_workflow_engine-0.2.0/django_workflow_engine/migrations/0011_migrate_from_taskrecordexecutions.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/migrations/0012_alter_target_unique_together.py` & `django_workflow_engine-0.2.0/django_workflow_engine/migrations/0012_alter_target_unique_together.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/models.py` & `django_workflow_engine-0.2.0/django_workflow_engine/models.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tasks/email_form.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tasks/email_form.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tasks/previous_tasks_complete.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tasks/previous_tasks_complete.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tasks/send_email.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tasks/send_email.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tasks/task.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_detail.html` & `django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_detail.html`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_diagram.html` & `django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_diagram.html`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/templates/django_workflow_engine/flow_list.html` & `django_workflow_engine-0.2.0/django_workflow_engine/templates/django_workflow_engine/flow_list.html`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/templates/includes/requirement_summary.html` & `django_workflow_engine-0.2.0/django_workflow_engine/templates/includes/requirement_summary.html`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/factories.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/tasks.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.contrib.auth import get_user_model
+
 from django_workflow_engine.tasks.task import Task
 
 User = get_user_model()
 
 """
 Test Task definitions
 
@@ -22,14 +23,22 @@
     task_name = "pause_task"
     auto = True
 
     def execute(self, task_info):
         return [], False
 
 
+class ErrorTask(Task):
+    task_name = "error_task"
+    auto = True
+
+    def execute(self, task_info):
+        raise Exception("Error")
+
+
 class SelfReferencingPauseTask(Task):
     task_name = "self_ref_pause_task"
     auto = True
 
     def execute(self, task_info):
         return ["self_ref_pause_task"], False
```

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/test_task_info.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/test_task_info.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_loops.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_loops.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_pause_task.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_pause_task.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_previous_tasks_complete.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_previous_tasks_complete.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/test_workflows/test_reminder_workflow.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/test_workflows/test_reminder_workflow.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/utils.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/tests/workflows.py` & `django_workflow_engine-0.2.0/django_workflow_engine/tests/workflows.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/utils.py` & `django_workflow_engine-0.2.0/django_workflow_engine/utils.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/django_workflow_engine/views.py` & `django_workflow_engine-0.2.0/django_workflow_engine/views.py`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/docs/index.md` & `django_workflow_engine-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_workflow_engine-0.1.1/pyproject.toml` & `django_workflow_engine-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-workflow-engine"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = [
     "Cameron Lamb <cameron.lamb@digital.trade.gov.uk>",
     "Ross Miller <ross.miller@digital.trade.gov.uk>"
 ]
 license = "MIT"
 readme = "docs/index.md"
```

### Comparing `django_workflow_engine-0.1.1/PKG-INFO` & `django_workflow_engine-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-workflow-engine
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Cameron Lamb
 Author-email: cameron.lamb@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

