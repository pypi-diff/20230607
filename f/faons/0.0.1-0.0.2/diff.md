# Comparing `tmp/faons-0.0.1.tar.gz` & `tmp/faons-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faons-0.0.1.tar", last modified: Wed Jun  7 05:54:14 2023, max compression
+gzip compressed data, was "faons-0.0.2.tar", last modified: Wed Jun  7 07:50:40 2023, max compression
```

## Comparing `faons-0.0.1.tar` & `faons-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 05:54:14.693297 faons-0.0.1/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      111 2023-06-07 05:54:14.688296 faons-0.0.1/PKG-INFO
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:43.000000 faons-0.0.1/README.md
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 05:54:14.294566 faons-0.0.1/faons/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:06.000000 faons-0.0.1/faons/__init__.py
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     3178 2023-06-07 05:48:37.000000 faons-0.0.1/faons/cli.py
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 05:54:14.651296 faons-0.0.1/faons.egg-info/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      111 2023-06-07 05:54:12.000000 faons-0.0.1/faons.egg-info/PKG-INFO
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      225 2023-06-07 05:54:14.000000 faons-0.0.1/faons.egg-info/SOURCES.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        1 2023-06-07 05:54:12.000000 faons-0.0.1/faons.egg-info/dependency_links.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       49 2023-06-07 05:54:13.000000 faons-0.0.1/faons.egg-info/entry_points.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       61 2023-06-07 05:54:13.000000 faons-0.0.1/faons.egg-info/requires.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        6 2023-06-07 05:54:13.000000 faons-0.0.1/faons.egg-info/top_level.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       38 2023-06-07 05:54:14.695297 faons-0.0.1/setup.cfg
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      412 2023-06-07 05:53:32.000000 faons-0.0.1/setup.py
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 07:50:40.083656 faons-0.0.2/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      111 2023-06-07 07:50:40.065762 faons-0.0.2/PKG-INFO
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     1609 2023-06-07 07:50:27.000000 faons-0.0.2/README.md
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 07:50:39.543567 faons-0.0.2/faons/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:06.000000 faons-0.0.2/faons/__init__.py
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     5748 2023-06-07 07:28:21.000000 faons-0.0.2/faons/cli.py
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 07:50:40.025657 faons-0.0.2/faons.egg-info/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      111 2023-06-07 07:50:37.000000 faons-0.0.2/faons.egg-info/PKG-INFO
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      225 2023-06-07 07:50:39.000000 faons-0.0.2/faons.egg-info/SOURCES.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        1 2023-06-07 07:50:37.000000 faons-0.0.2/faons.egg-info/dependency_links.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       42 2023-06-07 07:50:38.000000 faons-0.0.2/faons.egg-info/entry_points.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       61 2023-06-07 07:50:38.000000 faons-0.0.2/faons.egg-info/requires.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        6 2023-06-07 07:50:38.000000 faons-0.0.2/faons.egg-info/top_level.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       38 2023-06-07 07:50:40.085654 faons-0.0.2/setup.cfg
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      405 2023-06-07 07:12:42.000000 faons-0.0.2/setup.py
```

