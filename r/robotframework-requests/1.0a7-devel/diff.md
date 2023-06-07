# Comparing `tmp/robotframework-requests-1.0a7.tar.gz` & `tmp/robotframework-requests-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requests-1.0a7.tar", last modified: Tue Jun  6 23:54:03 2023, max compression
+gzip compressed data, was "dist/robotframework-requests-0.1.tar", last modified: Fri Sep  2 05:56:17 2011, max compression
```

## Comparing `robotframework-requests-1.0a7.tar` & `robotframework-requests-0.1.tar`

### file list

```diff
@@ -1,25 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:54:03.795446 robotframework-requests-1.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-06 23:54:03.795446 robotframework-requests-1.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:54:03.795446 robotframework-requests-1.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:54:03.791445 robotframework-requests-1.0a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:54:03.791445 robotframework-requests-1.0a7/src/RequestsLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)    15887 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/RequestsKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/RequestsOnSessionKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    26195 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/SessionKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 23:53:55.000000 robotframework-requests-1.0a7/src/RequestsLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:54:03.795446 robotframework-requests-1.0a7/src/robotframework_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-06 23:54:03.000000 robotframework-requests-1.0a7/src/robotframework_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-06 23:54:03.000000 robotframework-requests-1.0a7/src/robotframework_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:54:03.000000 robotframework-requests-1.0a7/src/robotframework_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 23:54:03.000000 robotframework-requests-1.0a7/src/robotframework_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 23:54:03.000000 robotframework-requests-1.0a7/src/robotframework_requests.egg-info/top_level.txt
+drwxr-xr-x   0 bulkan     (501) staff       (20)        0 2011-09-02 05:56:17.000000 robotframework-requests-0.1/
+-rw-r--r--   0 bulkan     (501) staff       (20)      718 2011-09-02 05:56:17.000000 robotframework-requests-0.1/PKG-INFO
+-rw-r--r--   0 bulkan     (501) staff       (20)       62 2011-09-01 05:42:38.000000 robotframework-requests-0.1/setup.cfg
+-rw-r--r--   0 bulkan     (501) staff       (20)     1168 2011-09-02 05:56:14.000000 robotframework-requests-0.1/setup.py
+drwxr-xr-x   0 bulkan     (501) staff       (20)        0 2011-09-02 05:56:17.000000 robotframework-requests-0.1/src/
+drwxr-xr-x   0 bulkan     (501) staff       (20)        0 2011-09-02 05:56:17.000000 robotframework-requests-0.1/src/RequestsLibrary/
+-rw-r--r--   0 bulkan     (501) staff       (20)      116 2011-09-02 04:21:50.000000 robotframework-requests-0.1/src/RequestsLibrary/__init__.py
+-rw-r--r--   0 bulkan     (501) staff       (20)     3784 2011-09-02 04:14:39.000000 robotframework-requests-0.1/src/RequestsLibrary/keywords.py
+-rw-r--r--   0 bulkan     (501) staff       (20)       16 2011-09-02 05:55:00.000000 robotframework-requests-0.1/src/RequestsLibrary/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

