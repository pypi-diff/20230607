# Comparing `tmp/pagure-messages-1.0.0.tar.gz` & `tmp/pagure-messages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagure-messages-1.0.0.tar", last modified: Thu May 25 09:17:59 2023, max compression
+gzip compressed data, was "pagure-messages-1.1.0.tar", last modified: Wed Jun  7 08:13:34 2023, max compression
```

## Comparing `pagure-messages-1.0.0.tar` & `pagure-messages-1.1.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/
--rw-r--r--   0 abompard  (1000) abompard  (1000)    18092 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/LICENSE
--rw-r--r--   0 abompard  (1000) abompard  (1000)       24 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/MANIFEST.in
--rw-r--r--   0 abompard  (1000) abompard  (1000)      970 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/PKG-INFO
--rw-r--r--   0 abompard  (1000) abompard  (1000)      202 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/README.md
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.569225 pagure-messages-1.0.0/pagure_messages/
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2549 2023-05-24 11:23:39.000000 pagure-messages-1.0.0/pagure_messages/__init__.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    11945 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/base.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     9683 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/git_schema.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    16131 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/issue_schema.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     6481 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/misc_schema.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    17528 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/project_schema.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    22019 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/pull_requests_schema.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/pagure_messages/tests/
--rw-r--r--   0 abompard  (1000) abompard  (1000)        0 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/pagure_messages/tests/__init__.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2485 2023-05-24 11:43:37.000000 pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2496 2023-05-24 11:43:45.000000 pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_updated.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     1743 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/tests/test_common.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     4132 2023-05-24 11:44:01.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_creation.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     3383 2023-05-24 11:44:08.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_deletion.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     6039 2023-05-24 11:44:14.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_receive.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     3356 2023-05-24 11:44:19.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_creation.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     3356 2023-05-24 11:44:24.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_deletion.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2393 2023-05-24 11:44:28.000000 pagure-messages-1.0.0/pagure_messages/tests/test_group_edit.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2682 2023-05-24 11:44:36.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2380 2023-05-24 11:44:41.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_reset.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2391 2023-05-24 11:44:45.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_comment_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2550 2023-05-24 11:44:49.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2608 2023-05-24 11:44:54.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_removed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2401 2023-05-24 11:45:00.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_drop.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2496 2023-05-24 11:45:04.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_edit.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2347 2023-05-24 11:45:09.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_new.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2486 2023-05-24 11:45:15.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2538 2023-05-24 11:45:20.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_removed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     1559 2023-05-24 11:23:39.000000 pagure-messages-1.0.0/pagure_messages/tests/test_object_from_topic.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2219 2023-05-24 11:45:31.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_deleted.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2405 2023-05-24 11:45:37.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_edit.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2192 2023-05-24 11:45:43.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_forked.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2543 2023-05-24 11:45:48.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_group_access_updated.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2484 2023-05-24 11:45:53.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_group_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2501 2023-05-24 11:45:58.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_group_removed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2195 2023-05-24 11:46:04.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_new.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2360 2023-05-24 11:46:08.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_edited.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2369 2023-05-24 11:46:12.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_removed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2500 2023-05-24 11:46:16.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_user_access_updated.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2318 2023-05-24 11:46:22.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_user_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2371 2023-05-24 11:46:29.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_user_removed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2578 2023-05-24 11:46:34.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2429 2023-05-24 11:46:38.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_reset.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     3172 2023-05-24 11:46:43.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_closed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2336 2023-05-24 11:46:49.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2346 2023-05-24 11:46:53.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_edited.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2412 2023-05-24 11:46:58.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2427 2023-05-24 11:47:02.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_updated.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2494 2023-05-24 11:47:06.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_initial_comment_edited.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2306 2023-05-24 11:47:10.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_new.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2260 2023-05-24 11:47:17.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_rebased.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2269 2023-05-24 11:47:22.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_reopened.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2531 2023-05-24 11:47:26.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_added.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2564 2023-05-24 11:47:29.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_removed.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2260 2023-05-24 11:47:33.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_updated.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     1929 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/pagure_messages/tests/test_test_notification.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    19998 2023-05-15 10:25:11.000000 pagure-messages-1.0.0/pagure_messages/tests/utils.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.570225 pagure-messages-1.0.0/pagure_messages.egg-info/
--rw-r--r--   0 abompard  (1000) abompard  (1000)      970 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/PKG-INFO
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2958 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/SOURCES.txt
--rw-r--r--   0 abompard  (1000) abompard  (1000)        1 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/dependency_links.txt
--rw-r--r--   0 abompard  (1000) abompard  (1000)     3666 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/entry_points.txt
--rw-r--r--   0 abompard  (1000) abompard  (1000)        1 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/not-zip-safe
--rw-r--r--   0 abompard  (1000) abompard  (1000)       17 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/requires.txt
--rw-r--r--   0 abompard  (1000) abompard  (1000)       16 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/top_level.txt
--rw-r--r--   0 abompard  (1000) abompard  (1000)     4965 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/setup.cfg
--rw-r--r--   0 abompard  (1000) abompard  (1000)       61 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/setup.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)      564 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/tox.ini
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-06-07 08:13:34.314773 pagure-messages-1.1.0/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    18092 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/LICENSE
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       24 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/MANIFEST.in
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      970 2023-06-07 08:13:34.314773 pagure-messages-1.1.0/PKG-INFO
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      202 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/README.md
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-06-07 08:13:34.309773 pagure-messages-1.1.0/pagure_messages/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2549 2023-05-24 11:23:39.000000 pagure-messages-1.1.0/pagure_messages/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    11945 2023-05-24 11:50:07.000000 pagure-messages-1.1.0/pagure_messages/base.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    10503 2023-06-07 07:58:19.000000 pagure-messages-1.1.0/pagure_messages/git_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    16131 2023-05-24 11:50:07.000000 pagure-messages-1.1.0/pagure_messages/issue_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6481 2023-05-24 11:50:07.000000 pagure-messages-1.1.0/pagure_messages/misc_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    17528 2023-05-24 11:50:07.000000 pagure-messages-1.1.0/pagure_messages/project_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    22019 2023-05-24 11:50:07.000000 pagure-messages-1.1.0/pagure_messages/pull_requests_schema.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-06-07 08:13:34.314773 pagure-messages-1.1.0/pagure_messages/tests/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)        0 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/pagure_messages/tests/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2485 2023-05-24 11:43:37.000000 pagure-messages-1.1.0/pagure_messages/tests/test_commit_flag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2496 2023-05-24 11:43:45.000000 pagure-messages-1.1.0/pagure_messages/tests/test_commit_flag_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1743 2023-05-24 11:50:07.000000 pagure-messages-1.1.0/pagure_messages/tests/test_common.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     4132 2023-05-24 11:44:01.000000 pagure-messages-1.1.0/pagure_messages/tests/test_git_branch_creation.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3383 2023-05-24 11:44:08.000000 pagure-messages-1.1.0/pagure_messages/tests/test_git_branch_deletion.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     5221 2023-06-07 07:58:19.000000 pagure-messages-1.1.0/pagure_messages/tests/test_git_receive.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3356 2023-05-24 11:44:19.000000 pagure-messages-1.1.0/pagure_messages/tests/test_git_tag_creation.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3356 2023-05-24 11:44:24.000000 pagure-messages-1.1.0/pagure_messages/tests/test_git_tag_deletion.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2393 2023-05-24 11:44:28.000000 pagure-messages-1.1.0/pagure_messages/tests/test_group_edit.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2682 2023-05-24 11:44:36.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_assigned_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2380 2023-05-24 11:44:41.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_assigned_reset.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2391 2023-05-24 11:44:45.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_comment_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2550 2023-05-24 11:44:49.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_dependency_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2608 2023-05-24 11:44:54.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_dependency_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2401 2023-05-24 11:45:00.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_drop.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2496 2023-05-24 11:45:04.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_edit.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2347 2023-05-24 11:45:09.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_new.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2486 2023-05-24 11:45:15.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_tag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2538 2023-05-24 11:45:20.000000 pagure-messages-1.1.0/pagure_messages/tests/test_issue_tag_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1559 2023-05-24 11:23:39.000000 pagure-messages-1.1.0/pagure_messages/tests/test_object_from_topic.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2219 2023-05-24 11:45:31.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_deleted.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2405 2023-05-24 11:45:37.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_edit.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2192 2023-05-24 11:45:43.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_forked.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2543 2023-05-24 11:45:48.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_group_access_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2484 2023-05-24 11:45:53.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_group_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2501 2023-05-24 11:45:58.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_group_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2195 2023-05-24 11:46:04.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_new.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2360 2023-05-24 11:46:08.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_tag_edited.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2369 2023-05-24 11:46:12.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_tag_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2500 2023-05-24 11:46:16.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_user_access_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2318 2023-05-24 11:46:22.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_user_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2371 2023-05-24 11:46:29.000000 pagure-messages-1.1.0/pagure_messages/tests/test_project_user_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2578 2023-05-24 11:46:34.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_assigned_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2429 2023-05-24 11:46:38.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_assigned_reset.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3172 2023-05-24 11:46:43.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_closed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2336 2023-05-24 11:46:49.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_comment_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2346 2023-05-24 11:46:53.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_comment_edited.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2412 2023-05-24 11:46:58.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_flag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2427 2023-05-24 11:47:02.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_flag_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2494 2023-05-24 11:47:06.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_initial_comment_edited.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2306 2023-05-24 11:47:10.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_new.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2260 2023-05-24 11:47:17.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_rebased.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2269 2023-05-24 11:47:22.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_reopened.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2531 2023-05-24 11:47:26.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_tag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2564 2023-05-24 11:47:29.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_tag_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2260 2023-05-24 11:47:33.000000 pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1929 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/pagure_messages/tests/test_test_notification.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    19998 2023-05-15 10:25:11.000000 pagure-messages-1.1.0/pagure_messages/tests/utils.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-06-07 08:13:34.309773 pagure-messages-1.1.0/pagure_messages.egg-info/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      970 2023-06-07 08:13:33.000000 pagure-messages-1.1.0/pagure_messages.egg-info/PKG-INFO
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2958 2023-06-07 08:13:34.000000 pagure-messages-1.1.0/pagure_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)        1 2023-06-07 08:13:33.000000 pagure-messages-1.1.0/pagure_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3666 2023-06-07 08:13:33.000000 pagure-messages-1.1.0/pagure_messages.egg-info/entry_points.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)        1 2023-05-25 09:17:59.000000 pagure-messages-1.1.0/pagure_messages.egg-info/not-zip-safe
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       17 2023-06-07 08:13:34.000000 pagure-messages-1.1.0/pagure_messages.egg-info/requires.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       16 2023-06-07 08:13:34.000000 pagure-messages-1.1.0/pagure_messages.egg-info/top_level.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     4965 2023-06-07 08:13:34.314773 pagure-messages-1.1.0/setup.cfg
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       61 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/setup.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      564 2023-05-15 10:07:56.000000 pagure-messages-1.1.0/tox.ini
```

### Comparing `pagure-messages-1.0.0/LICENSE` & `pagure-messages-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/PKG-INFO` & `pagure-messages-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagure-messages
-Version: 1.0.0
+Version: 1.1.0
 Summary: A schema package for messages sent by pagure
 Home-page: https://pagure.io/pagure
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
 License: GPLv2+
 Keywords: fedora
 Platform: Fedora
```

### Comparing `pagure-messages-1.0.0/pagure_messages/__init__.py` & `pagure-messages-1.1.0/pagure_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/base.py` & `pagure-messages-1.1.0/pagure_messages/base.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/git_schema.py` & `pagure-messages-1.1.0/pagure_messages/git_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -174,39 +174,58 @@
             "start_commit",
             "end_commit",
         ],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New commit: {count} commits\nBy: {agent_name}".format(
-            count=self.body["total_commits"],
-            agent_name=self.agent_name,
+        author = self.body["authors"][0]
+        force_prefix = "forced-" if self.body["forced"] else ""
+        plural_suffix = "s" if self.body["total_commits"] > 1 else ""
+        branch_short = self.body["branch"].replace("refs/heads/", "")
+        tpl = (
+            "{author[fullname]} ({author[name]}) {force_prefix}pushed {total_commits} "
+            "commit{plural_suffix} on {repo[fullname]}.\n"
+            "Branch: {branch_short}\n"
+        )
+        return tpl.format(
+            **self.body,
+            author=author,
+            force_prefix=force_prefix,
+            plural_suffix=plural_suffix,
+            branch_short=branch_short,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
+        branch = self.body["branch"].replace("refs/heads/", "")
         return "{agent_name} pushed {count} commits on {fullname} (branch: {branch})".format(
             agent_name=self.agent_name,
             fullname=self.body["repo"]["fullname"],
             count=self.body["total_commits"],
-            branch=self.body["branch"],
+            branch=branch,
         )
 
     @property
     def url(self):
-        base_url = self.body["repo"]["full_url"]
+        if self.body["total_commits"] == 1:
+            return "{base_url}/c/{rev}".format(
+                base_url=self.body["repo"]["full_url"], rev=self.body["end_commit"]
+            )
+        else:
+            return "{base_url}/c/{old}..{end}".format(
+                base_url=self.body["repo"]["full_url"],
+                old=self.body["old_commit"],
+                end=self.body["end_commit"],
+            )
 
-        item = self.body["branch"]
-        if "refs/heads/" in item:
-            item = item.replace("refs/heads/", "")
-
-        tmpl = "{base_url}/tree/{item}"
-        return tmpl.format(base_url=base_url, item=item)
+    @property
+    def patch_url(self):
+        return f"{self.url}.patch" if self.body["total_commits"] == 1 else None
 
 
 class GitTagCreationV1(GitMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
```

### Comparing `pagure-messages-1.0.0/pagure_messages/issue_schema.py` & `pagure-messages-1.1.0/pagure_messages/issue_schema.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/misc_schema.py` & `pagure-messages-1.1.0/pagure_messages/misc_schema.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/project_schema.py` & `pagure-messages-1.1.0/pagure_messages/project_schema.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/pull_requests_schema.py` & `pagure-messages-1.1.0/pagure_messages/pull_requests_schema.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_commit_flag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_updated.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_commit_flag_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_common.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_creation.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_git_branch_creation.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_deletion.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_git_branch_deletion.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_git_receive.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_git_receive.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,157 +20,131 @@
 
 import pytest
 
 from .utils import PROJECT
 from ..git_schema import GitReceiveV1
 
 
-def test_minimal():
-    """
-    Assert the message schema validates a message with the required fields.
-    """
-    body = {
+@pytest.fixture
+def body():
+    return {
         "agent": "dummy-user",
         "forced": False,
         "repo": PROJECT,
         "old_commit": "hash_commit_old",
         "branch": "refs/heads/develop",
         "authors": [
             {
-                "fullname": "dummy-user",
+                "fullname": "Dummy User",
                 "url_path": "user/dummy-user",
                 "name": "dummy-user",
-                "email": None,
+                "email": "dummy-user@example.com",
             }
         ],
         "total_commits": 42,
         "start_commit": "hash_commit_start",
         "end_commit": "hash_commit_stop",
     }
+
+
+def test_minimal(body):
+    """
+    Assert the message schema validates a message with the required fields.
+    """
     message = GitReceiveV1(body=body)
     message.validate()
-    assert (
-        message.url
-        == "http://localhost.localdomain/fedora-infra/fedocal-messages/tree/develop"
+    assert message.url == (
+        "http://localhost.localdomain/fedora-infra/fedocal-messages"
+        "/c/hash_commit_old..hash_commit_stop"
     )
     assert message.packages == []
     assert message.containers == []
     assert message.modules == []
     assert message.flatpaks == []
 
 
-def test_minimal_short_branch():
+def test_minimal_short_branch(body):
     """
     Assert the message schema validates a message with the required fields.
     """
-    body = {
-        "agent": "dummy-user",
-        "forced": False,
-        "repo": PROJECT,
-        "old_commit": "hash_commit_old",
-        "branch": "develop",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": None,
-                "name": None,
-                "email": "dummy-user@example.com",
-            }
-        ],
-        "total_commits": 42,
-        "start_commit": "hash_commit_start",
-        "end_commit": "hash_commit_stop",
-    }
+    body["branch"] = "develop"
     message = GitReceiveV1(body=body)
     message.validate()
-    assert (
-        message.url
-        == "http://localhost.localdomain/fedora-infra/fedocal-messages/tree/develop"
+    assert message.url == (
+        "http://localhost.localdomain/fedora-infra/fedocal-messages/"
+        "c/hash_commit_old..hash_commit_stop"
     )
 
 
-def test_missing_fields():
+def test_missing_fields(body):
     """Assert an exception is actually raised on validation failure."""
-    minimal_message = {
-        "forced": False,
-        "repo": PROJECT,
-        "old_commit": "hash_commit_old",
-        "branch": "develop",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
-        "total_commits": 42,
-        "start_commit": "hash_commit_start",
-        "end_commit": "hash_commit_stop",
-    }
-    message = GitReceiveV1(body=minimal_message)
+    del body["agent"]
+    message = GitReceiveV1(body=body)
     with pytest.raises(ValidationError):
         message.validate()
 
 
-def test_str():
+def test_str(body):
     """Assert __str__ produces a human-readable message."""
-    body = {
-        "agent": "dummy-user",
-        "forced": False,
-        "repo": PROJECT,
-        "old_commit": "hash_commit_old",
-        "branch": "develop",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
-        "total_commits": 42,
-        "start_commit": "hash_commit_start",
-        "end_commit": "hash_commit_stop",
-    }
-    expected_str = "New commit: 42 commits\nBy: dummy-user"
+    expected_str = (
+        "Dummy User (dummy-user) pushed 42 commits on "
+        "fedora-infra/fedocal-messages.\n"
+        "Branch: develop\n"
+    )
     message = GitReceiveV1(body=body)
     message.validate()
     assert expected_str == str(message)
 
 
-def test_summary():
+def test_summary(body):
     """Assert the summary is correct."""
-    body = {
-        "agent": "dummy-user",
-        "forced": False,
-        "repo": PROJECT,
-        "old_commit": "hash_commit_old",
-        "branch": "develop",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
-        "total_commits": 42,
-        "start_commit": "hash_commit_start",
-        "end_commit": "hash_commit_stop",
-    }
     expected_summary = (
         "dummy-user pushed 42 commits on "
         "fedora-infra/fedocal-messages (branch: develop)"
     )
     message = GitReceiveV1(body=body)
     message.validate()
     assert expected_summary == message.summary
 
 
+def test_url_one_commit(body):
+    """
+    Assert the URL is correct when a single commit was received.
+    """
+    body["total_commits"] = 1
+    message = GitReceiveV1(body=body)
+    message.validate()
+    assert message.url == (
+        "http://localhost.localdomain/fedora-infra/fedocal-messages"
+        "/c/hash_commit_stop"
+    )
+
+
+def test_patch_url(body):
+    """
+    Assert the patch URL is correct when a single commit was received.
+    """
+    body["total_commits"] = 1
+    message = GitReceiveV1(body=body)
+    message.validate()
+    assert message.patch_url == (
+        "http://localhost.localdomain/fedora-infra/fedocal-messages"
+        "/c/hash_commit_stop.patch"
+    )
+
+
+def test_patch_url_multiple_commits(body):
+    """
+    Assert the patch URL is correct when a single commit was received.
+    """
+    message = GitReceiveV1(body=body)
+    message.validate()
+    assert message.patch_url is None
+
+
 @pytest.mark.parametrize(
     "namespace,msg_attr",
     [
         ("rpms", "packages"),
         ("containers", "containers"),
         ("modules", "modules"),
         ("flatpaks", "flatpaks"),
```

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_creation.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_git_tag_creation.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_deletion.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_git_tag_deletion.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_group_edit.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_group_edit.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_assigned_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_reset.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_assigned_reset.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_comment_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_comment_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_dependency_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_removed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_dependency_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_drop.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_drop.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_edit.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_edit.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_new.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_new.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_tag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_removed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_issue_tag_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_object_from_topic.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_object_from_topic.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_deleted.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_deleted.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_edit.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_edit.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_forked.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_forked.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_group_access_updated.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_group_access_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_group_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_group_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_group_removed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_group_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_new.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_new.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_edited.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_tag_edited.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_removed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_tag_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_user_access_updated.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_user_access_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_user_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_user_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_project_user_removed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_project_user_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_assigned_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_reset.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_assigned_reset.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_closed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_closed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_comment_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_edited.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_comment_edited.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_flag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_updated.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_flag_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_initial_comment_edited.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_initial_comment_edited.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_new.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_new.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_rebased.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_rebased.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_reopened.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_reopened.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_added.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_tag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_removed.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_tag_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_updated.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_pull_request_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/test_test_notification.py` & `pagure-messages-1.1.0/pagure_messages/tests/test_test_notification.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages/tests/utils.py` & `pagure-messages-1.1.0/pagure_messages/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages.egg-info/PKG-INFO` & `pagure-messages-1.1.0/pagure_messages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagure-messages
-Version: 1.0.0
+Version: 1.1.0
 Summary: A schema package for messages sent by pagure
 Home-page: https://pagure.io/pagure
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
 License: GPLv2+
 Keywords: fedora
 Platform: Fedora
```

### Comparing `pagure-messages-1.0.0/pagure_messages.egg-info/SOURCES.txt` & `pagure-messages-1.1.0/pagure_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/pagure_messages.egg-info/entry_points.txt` & `pagure-messages-1.1.0/pagure_messages.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pagure-messages-1.0.0/setup.cfg` & `pagure-messages-1.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pagure-messages
-version = 1.0.0
+version = 1.1.0
 description = A schema package for messages sent by pagure
 long_description = file: README.md
 url = https://pagure.io/pagure
 maintainer = Fedora Infrastructure Team
 maintainer_email = infrastructure@lists.fedoraproject.org
 keywords = fedora
 platforms = Fedora, GNU/Linux
```

### Comparing `pagure-messages-1.0.0/tox.ini` & `pagure-messages-1.1.0/tox.ini`

 * *Files identical despite different names*

