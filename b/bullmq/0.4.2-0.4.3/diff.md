# Comparing `tmp/bullmq-0.4.2.tar.gz` & `tmp/bullmq-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.4.2.tar", last modified: Thu Jun  1 17:08:40 2023, max compression
+gzip compressed data, was "bullmq-0.4.3.tar", last modified: Wed Jun  7 09:21:39 2023, max compression
```

## Comparing `bullmq-0.4.2.tar` & `bullmq-0.4.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.790743 bullmq-0.4.2/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-01 17:08:40.790384 bullmq-0.4.2/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.2/README.md
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.746573 bullmq-0.4.2/bullmq/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/backoffs.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.784465 bullmq-0.4.2/bullmq/commands/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/addJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/drain-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getState-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveJobFromActiveToWait-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/pause-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/promote-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/reprocessJob-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/takeLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/updateData-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.2/bullmq/error_code.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.2/bullmq/event_emitter.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7343 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/job.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4847 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/queue.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1356 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/redis_connection.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    15741 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/scripts.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.2/bullmq/timer.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.789564 bullmq-0.4.2/bullmq/types/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      314 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      207 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/backoff_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1920 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/job_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      395 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/keep_jobs.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      189 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/queue_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      129 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/retry_job_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1190 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/worker_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      144 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/utils.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7490 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/worker.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.748326 bullmq-0.4.2/bullmq.egg-info/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1574 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       21 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/requires.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/top_level.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-06-01 17:08:40.790854 bullmq-0.4.2/setup.cfg
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1177 2023-06-01 17:06:57.000000 bullmq-0.4.2/setup.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.733139 bullmq-0.4.3/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-07 09:21:39.732783 bullmq-0.4.3/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.3/README.md
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.705716 bullmq-0.4.3/bullmq/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/backoffs.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.729548 bullmq-0.4.3/bullmq/commands/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/drain-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getState-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveJobFromActiveToWait-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/pause-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/promote-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/reprocessJob-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/takeLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.3/bullmq/error_code.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.3/bullmq/event_emitter.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7488 2023-06-06 19:07:05.000000 bullmq-0.4.3/bullmq/job.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4847 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/queue.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1356 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/redis_connection.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    16376 2023-06-06 19:07:05.000000 bullmq-0.4.3/bullmq/scripts.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.3/bullmq/timer.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.732302 bullmq-0.4.3/bullmq/types/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      314 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      207 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/backoff_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1920 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/job_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      395 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/keep_jobs.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      189 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/queue_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      129 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/retry_job_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1190 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/worker_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      144 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/utils.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7490 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/worker.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.707876 bullmq-0.4.3/bullmq.egg-info/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1574 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       21 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/requires.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-06-07 09:21:39.733258 bullmq-0.4.3/setup.cfg
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1177 2023-06-07 09:15:53.000000 bullmq-0.4.3/setup.py
```

### Comparing `bullmq-0.4.2/PKG-INFO` & `bullmq-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.2
+Version: 0.4.3
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.4.2/README.md` & `bullmq-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/backoffs.py` & `bullmq-0.4.3/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/addJob-8.lua` & `bullmq-0.4.3/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/changeDelay-3.lua` & `bullmq-0.4.3/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.4.3/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/drain-4.lua` & `bullmq-0.4.3/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/getCounts-1.lua` & `bullmq-0.4.3/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/getRanges-1.lua` & `bullmq-0.4.3/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/getState-7.lua` & `bullmq-0.4.3/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/getStateV2-7.lua` & `bullmq-0.4.3/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/isFinished-3.lua` & `bullmq-0.4.3/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/moveJobFromActiveToWait-4.lua` & `bullmq-0.4.3/bullmq/commands/moveJobFromActiveToWait-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.4.3/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/moveToActive-9.lua` & `bullmq-0.4.3/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.4.3/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.4.3/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.4.3/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/obliterate-2.lua` & `bullmq-0.4.3/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/pause-4.lua` & `bullmq-0.4.3/bullmq/commands/pause-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/promote-6.lua` & `bullmq-0.4.3/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/removeJob-1.lua` & `bullmq-0.4.3/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.4.3/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/reprocessJob-4.lua` & `bullmq-0.4.3/bullmq/commands/reprocessJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/retryJob-8.lua` & `bullmq-0.4.3/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/commands/retryJobs-6.lua` & `bullmq-0.4.3/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/event_emitter.py` & `bullmq-0.4.3/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/job.py` & `bullmq-0.4.3/bullmq/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         self.processedOn = None
         self.returnvalue = None
         return self.scripts.reprocessJob(self, state)
 
     def getState(self):
         return self.scripts.getState(self.id)
 
+    def changePriority(self, opts: dict):
+        return self.scripts.changePriority(self.id, opts.get("priority", 0), opts.get("lifo", False))
+
     def updateProgress(self, progress):
         self.progress = progress
         return self.scripts.updateProgress(self.id, progress)
 
     async def moveToFailed(self, err, token:str, fetchNext:bool = False):
         error_message = str(err)
         self.failedReason = error_message
```

### Comparing `bullmq-0.4.2/bullmq/queue.py` & `bullmq-0.4.3/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/redis_connection.py` & `bullmq-0.4.3/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/scripts.py` & `bullmq-0.4.3/bullmq/scripts.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,24 +27,25 @@
         self.prefix = prefix
         self.queueName = queueName
         self.keys = {}
         self.redisConnection = redisConnection
         self.redisClient = redisConnection.conn
         self.commands = {
             "addJob": self.redisClient.register_script(self.getScript("addJob-8.lua")),
+            "changePriority": self.redisClient.register_script(self.getScript("changePriority-4.lua")),
             "extendLock": self.redisClient.register_script(self.getScript("extendLock-2.lua")),
             "getCounts": self.redisClient.register_script(self.getScript("getCounts-1.lua")),
             "getState": self.redisClient.register_script(self.getScript("getState-7.lua")),
             "getStateV2": self.redisClient.register_script(self.getScript("getStateV2-7.lua")),
             "moveToActive": self.redisClient.register_script(self.getScript("moveToActive-9.lua")),
             "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
             "moveToFinished": self.redisClient.register_script(self.getScript("moveToFinished-12.lua")),
             "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
-            "pause": self.redisClient.register_script(self.getScript("pause-4.lua")),
             "obliterate": self.redisClient.register_script(self.getScript("obliterate-2.lua")),
+            "pause": self.redisClient.register_script(self.getScript("pause-4.lua")),
             "reprocessJob": self.redisClient.register_script(self.getScript("reprocessJob-6.lua")),
             "retryJob": self.redisClient.register_script(self.getScript("retryJob-8.lua")),
             "retryJobs": self.redisClient.register_script(self.getScript("retryJobs-6.lua")),
             "saveStacktrace": self.redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
             "updateData": self.redisClient.register_script(self.getScript("updateData-1.lua")),
             "updateProgress": self.redisClient.register_script(self.getScript("updateProgress-2.lua")),
         }
@@ -164,14 +165,29 @@
         if isRedisVersionLowerThan(redis_version, '6.0.6'):
             result = await self.commands["getState"](keys=keys, args=args)
             return result
 
         result = await self.commands["getStateV2"](keys=keys, args=args)
         return result
 
+    async def changePriority(self, job_id: str, priority:int = 0, lifo:bool = False):
+        keys = [self.keys['wait'],
+            self.keys['paused'],
+            self.keys['meta'],
+            self.keys['priority']]
+        
+        args = [priority, self.toKey(job_id), job_id, 1 if lifo else 0]
+
+        result = await self.commands["changePriority"](keys=keys, args=args)
+
+        if result is not None:
+            if result < 0:
+                raise self.finishedErrors(result, job_id, 'updateData')
+        return None
+
     async def updateData(self, job_id: str, data):
         keys = [self.toKey(job_id)]
         data_json = json.dumps(data, separators=(',', ':'))
         args = [data_json]
 
         result = await self.commands["updateData"](keys=keys, args=args)
```

### Comparing `bullmq-0.4.2/bullmq/timer.py` & `bullmq-0.4.3/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/types/job_options.py` & `bullmq-0.4.3/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/types/worker_options.py` & `bullmq-0.4.3/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq/worker.py` & `bullmq-0.4.3/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/bullmq.egg-info/PKG-INFO` & `bullmq-0.4.3/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.2
+Version: 0.4.3
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.4.2/bullmq.egg-info/SOURCES.txt` & `bullmq-0.4.3/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.2/setup.py` & `bullmq-0.4.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(".", 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bullmq',
-    version='0.4.2',    
+    version='0.4.3',    
     description='BullMQ for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bullmq.io',
     author='Taskforce.sh Inc.',
     author_email='manast@taskforce.sh',
     license='MIT',
```

