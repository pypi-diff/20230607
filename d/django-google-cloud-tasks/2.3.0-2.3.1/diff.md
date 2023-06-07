# Comparing `tmp/django_google_cloud_tasks-2.3.0.tar.gz` & `tmp/django_google_cloud_tasks-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.3.0.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.3.1.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.3.0.tar` & `django_google_cloud_tasks-2.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/LICENSE.md
--rw-r--r--   0        0        0      153 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1870 2023-05-24 18:43:03.594293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0        0 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4364 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2704 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2522 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2853 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0    10404 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      871 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3014 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/django_cloud_tasks/views.py
--rw-r--r--   0        0        0     1172 2023-05-24 18:43:03.598293 django_google_cloud_tasks-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2693 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     3026 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2853 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0    10404 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      871 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0     1192 2023-06-07 13:13:43.090976 django_google_cloud_tasks-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.3.1/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.3.0/LICENSE.md` & `django_google_cloud_tasks-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Self
 
 from django.db import models, transaction
 from django.utils import timezone
-
+from drf_kit.models import ModelDiffMixin
 from django_cloud_tasks import serializers
 from django_cloud_tasks.field import TaskField
 
 
 class Pipeline(models.Model):
     name = models.CharField(max_length=100)
 
@@ -26,15 +26,15 @@
         for routine in routines:
             routine.revert()
 
     def add_routine(self, routine: dict) -> "Routine":
         return self.routines.create(**routine)
 
 
-class Routine(models.Model):
+class Routine(models.Model, ModelDiffMixin):
     class Statuses(models.TextChoices):
         PENDING = ("pending", "Pending")
         SCHEDULED = ("scheduled", "Scheduled")
         RUNNING = ("running", "Running")
         COMPLETED = ("completed", "Completed")
         FAILED = ("failed", "Failed")
         REVERTING = ("reverting", "Reverting")
```

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from django.core.exceptions import ValidationError
-from django.db.models.signals import pre_save
+from django.db.models import Model
+from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 
 from django_cloud_tasks import models
 
 
-def _is_status_changing(instance: models.Routine) -> bool:
-    if not instance.pk:
-        return False
-
-    current_routine = models.Routine.objects.get(pk=instance.pk)
-    return current_routine.status != instance.status
+def _is_status_changing(instance: Model) -> bool:
+    previous_status, current_status = instance._diff.get("status", (None, None))
+    return previous_status != current_status
 
 
 def enqueue_next_routines(instance: models.Routine):
     for routine in instance.next_routines.all():
         routine.enqueue()
 
 
@@ -39,15 +37,15 @@
     models.Routine.Statuses.COMPLETED: enqueue_next_routines,
     models.Routine.Statuses.REVERTED: revert_previous_routines,
     models.Routine.Statuses.SCHEDULED: enqueue_routine_scheduled,
     models.Routine.Statuses.REVERTING: enqueue_revert_task,
 }
 
 
-@receiver(pre_save, sender=models.Routine)
+@receiver(post_save, sender=models.Routine)
 def handle_status_changed(sender, instance: models.Routine, **kwargs):
     if not _is_status_changing(instance=instance):
         return
 
     if action := STATUS_ACTION.get(instance.status):
         action(instance=instance)
 
@@ -56,23 +54,23 @@
 def ensure_status_machine(sender, instance: models.Routine, **kwargs):
     if not instance.pk and instance.status != models.Routine.Statuses.PENDING:
         raise ValidationError(f"The initial routine's status must be 'pending' not '{instance.status}'")
 
     if not _is_status_changing(instance=instance):
         return
 
-    current_routine = models.Routine.objects.get(pk=instance.pk)
+    previous_status, _ = instance._diff.get("status", (None, None))
 
     statuses = models.Routine.Statuses
     machine_statuses = {
         statuses.PENDING: [None],
         statuses.SCHEDULED: [statuses.PENDING, statuses.FAILED],
         statuses.RUNNING: [statuses.SCHEDULED],
         statuses.COMPLETED: [statuses.RUNNING],
         statuses.FAILED: [statuses.RUNNING, statuses.SCHEDULED],
         statuses.REVERTING: [statuses.COMPLETED, statuses.PENDING, statuses.SCHEDULED, statuses.FAILED],
         statuses.REVERTED: [statuses.REVERTING],
     }
     available_statuses = machine_statuses[instance.status]
 
-    if current_routine.status not in available_statuses:
-        raise ValidationError(f"Status update from '{current_routine.status}' to '{instance.status}' is not allowed")
+    if previous_status not in available_statuses:
+        raise ValidationError(f"Status update from '{previous_status}' to '{instance.status}' is not allowed")
```

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/routine_task.py`

 * *Files 21% similar despite different names*

```diff
@@ -52,14 +52,22 @@
             routine.pipeline.revert()
             return
 
         routine.attempt_count += 1
         routine.status = models.Routine.Statuses.RUNNING
         routine.save(update_fields=("attempt_count", "status", "updated_at"))
 
+        # we are adding this to re-instantiate this object due to
+        # a bug that are happening with _diff field from ModelDiffMixin.
+        # the complete method called below is triggering the ensure_status_machine
+        # with wrong previous_status. when we call complete(), we had previous status
+        # scheduled, but we just changed it to running. this was raising an error:
+        # changing from scheduled to complete is not allowed.
+        routine = models.Routine(**routine._dict)
+
         try:
             logger.info(f"Routine #{routine.pk} is running")
             task_response = routine.task_class(metadata=self._metadata).sync(**routine.body)
         except Exception as error:
             logger.info(f"Routine #{routine.pk} has failed")
             routine.fail(output={"error": str(error)})
             routine.enqueue()
```

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.3.1/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.0/pyproject.toml` & `django_google_cloud_tasks-2.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.3.0"
+version = "2.3.1"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 django = ">=4,<5"
 gcp-pilot = {version = "*", extras = ["tasks", "pubsub"]}
+drf-kit = "^1.21.6"
 
 
 [tool.poetry.dev-dependencies]
 ruff = "*"
 black = "*"
 coverage = "*"
 factory-boy = "*"
```

