# Comparing `tmp/python-hostingde-0.9.0.tar.gz` & `tmp/python-hostingde-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hostingde-0.9.0.tar", last modified: Thu May 25 19:25:06 2023, max compression
+gzip compressed data, was "python-hostingde-0.9.1.tar", last modified: Wed Jun  7 07:11:11 2023, max compression
```

## Comparing `python-hostingde-0.9.0.tar` & `python-hostingde-0.9.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.304829 python-hostingde-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1064 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8368 2023-05-25 19:25:06.304829 python-hostingde-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7347 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.296829 python-hostingde-0.9.0/hostingde/
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-25 19:25:04.000000 python-hostingde-0.9.0/hostingde/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/account/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/account/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/account/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/account/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/account/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/billing/billing.py
--rw-r--r--   0 root         (0) root         (0)      762 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/dns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22828 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/dns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/dns/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/requests/create_new_zone.py
--rw-r--r--   0 root         (0) root         (0)      206 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/requests/delete_zone.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/requests/update_records_request.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/dns/requests/update_zone_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5563 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/domain/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.300829 python-hostingde-0.9.0/hostingde/domain/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/domain/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      920 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/domain/requests/check_availability.py
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/domain/requests/register_domain.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/hostingde.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/job_waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.304829 python-hostingde-0.9.0/hostingde/model/
--rw-r--r--   0 root         (0) root         (0)     2854 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/account.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/billing.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/domain.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/domain_contact.py
--rw-r--r--   0 root         (0) root         (0)    12691 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/filter.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/job.py
--rw-r--r--   0 root         (0) root         (0)     4779 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/record.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/soa_values.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/sort.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/ssl.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/zone.py
--rw-r--r--   0 root         (0) root         (0)     6620 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/model/zone_config.py
--rw-r--r--   0 root         (0) root         (0)     4779 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/paginator.py
--rw-r--r--   0 root         (0) root         (0)     3095 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.304829 python-hostingde-0.9.0/hostingde/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/ssl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/hostingde/ssl/ssl.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 19:25:06.304829 python-hostingde-0.9.0/python_hostingde.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8368 2023-05-25 19:25:06.000000 python-hostingde-0.9.0/python_hostingde.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1446 2023-05-25 19:25:06.000000 python-hostingde-0.9.0/python_hostingde.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 19:25:06.000000 python-hostingde-0.9.0/python_hostingde.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-25 19:25:06.000000 python-hostingde-0.9.0/python_hostingde.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-25 19:25:06.000000 python-hostingde-0.9.0/python_hostingde.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-25 19:25:06.304829 python-hostingde-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1719 2023-05-25 19:25:03.000000 python-hostingde-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.694719 python-hostingde-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8368 2023-06-07 07:11:11.694719 python-hostingde-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7347 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.686719 python-hostingde-0.9.1/hostingde/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-07 07:11:09.000000 python-hostingde-0.9.1/hostingde/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.686719 python-hostingde-0.9.1/hostingde/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/account/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.686719 python-hostingde-0.9.1/hostingde/account/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/account/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.686719 python-hostingde-0.9.1/hostingde/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/billing/billing.py
+-rw-r--r--   0 root         (0) root         (0)      762 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.686719 python-hostingde-0.9.1/hostingde/dns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22828 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/dns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.690719 python-hostingde-0.9.1/hostingde/dns/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/requests/create_new_zone.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/requests/delete_zone.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/requests/update_records_request.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/dns/requests/update_zone_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.690719 python-hostingde-0.9.1/hostingde/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5563 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/domain/domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.690719 python-hostingde-0.9.1/hostingde/domain/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/domain/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      920 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/domain/requests/check_availability.py
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/domain/requests/register_domain.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/hostingde.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/job_waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.690719 python-hostingde-0.9.1/hostingde/model/
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/account.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/billing.py
+-rw-r--r--   0 root         (0) root         (0)     6012 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/domain.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/domain_contact.py
+-rw-r--r--   0 root         (0) root         (0)    12691 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/filter.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     4779 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/record.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/soa_values.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/sort.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/ssl.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/zone.py
+-rw-r--r--   0 root         (0) root         (0)     6620 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/model/zone_config.py
+-rw-r--r--   0 root         (0) root         (0)     4779 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/paginator.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.690719 python-hostingde-0.9.1/hostingde/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/ssl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/hostingde/ssl/ssl.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:11:11.694719 python-hostingde-0.9.1/python_hostingde.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8368 2023-06-07 07:11:11.000000 python-hostingde-0.9.1/python_hostingde.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-06-07 07:11:11.000000 python-hostingde-0.9.1/python_hostingde.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 07:11:11.000000 python-hostingde-0.9.1/python_hostingde.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-07 07:11:11.000000 python-hostingde-0.9.1/python_hostingde.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 07:11:11.000000 python-hostingde-0.9.1/python_hostingde.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-07 07:11:11.694719 python-hostingde-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-06-07 07:11:08.000000 python-hostingde-0.9.1/setup.py
```

### Comparing `python-hostingde-0.9.0/LICENSE` & `python-hostingde-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/PKG-INFO` & `python-hostingde-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hostingde
-Version: 0.9.0
+Version: 0.9.1
 Summary: Interact with HostingDe API
 Home-page: https://github.com/cancom/python-hostingde
 Author: CANCOM OpenSource
 Author-email: opensource@cancom.de
 License: MIT
 Project-URL: Source, https://github.com/cancom/python-hostingde
 Project-URL: Bug Reports, https://github.com/cancom/python-hostingde/issues
```

### Comparing `python-hostingde-0.9.0/README.md` & `python-hostingde-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/account/account.py` & `python-hostingde-0.9.1/hostingde/account/account.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/api.py` & `python-hostingde-0.9.1/hostingde/api.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/billing/billing.py` & `python-hostingde-0.9.1/hostingde/billing/billing.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/client.py` & `python-hostingde-0.9.1/hostingde/client.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/dns/dns.py` & `python-hostingde-0.9.1/hostingde/dns/dns.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/dns/requests/update_records_request.py` & `python-hostingde-0.9.1/hostingde/dns/requests/update_records_request.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/dns/requests/update_zone_request.py` & `python-hostingde-0.9.1/hostingde/dns/requests/update_zone_request.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/domain/domain.py` & `python-hostingde-0.9.1/hostingde/domain/domain.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/domain/requests/check_availability.py` & `python-hostingde-0.9.1/hostingde/domain/requests/check_availability.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/exceptions.py` & `python-hostingde-0.9.1/hostingde/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/hostingde.py` & `python-hostingde-0.9.1/hostingde/hostingde.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/job_waiter.py` & `python-hostingde-0.9.1/hostingde/job_waiter.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/__init__.py` & `python-hostingde-0.9.1/hostingde/model/__init__.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/account.py` & `python-hostingde-0.9.1/hostingde/model/account.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/billing.py` & `python-hostingde-0.9.1/hostingde/model/billing.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/domain.py` & `python-hostingde-0.9.1/hostingde/model/domain.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,14 +57,19 @@
     create_date: Optional[str]
     current_contract_period_end: Optional[str]
     next_contract_period_start: Optional[str]
     deletion_type: Optional[str]
     deletion_date: Optional[str]
     add_date: Optional[str]
     last_change_date: Optional[str]
+    product_code: Optional[str]
+    renew_on: Optional[str]
+    restorable_until: Optional[str]
+    latest_deletion_date_without_renew: Optional[str]
+    paid_until: Optional[str]
     status: Optional[DomainStatus] = EnumField(DomainStatus)
     contacts: List[DomainContactRef] = field(default_factory=list)
     nameservers: List[Nameserver] = field(default_factory=list)
 
     def __init__(
             self,
             name: str,
@@ -77,14 +82,19 @@
             contacts: Optional[List[DomainContactRef]] = None,
             nameservers: Optional[List[Nameserver]] = None,
             create_date: Optional[str] = None,
             current_contract_period_end: Optional[str] = None,
             next_contract_period_start: Optional[str] = None,
             deletion_type: Optional[str] = None,
             deletion_date: Optional[str] = None,
+            product_code: Optional[str] = None,
+            renew_on: Optional[str] = None,
+            restorable_until: Optional[str] = None,
+            latest_deletion_date_without_renew: Optional[str] = None,
+            paid_until: Optional[str] = None,
             add_date: Optional[str] = None,
             last_change_date: Optional[str] = None,
             **kwargs: Any
     ):
         """
         Represents a domain object
         :param name: Domain name. (Unicode or ASCII format). The name will always be returned in ASCII/ACE format.
@@ -102,14 +112,19 @@
                             getting the original creation date, it will be the date of the transfer.
         :param current_contract_period_end:  End date of current contract period
         :param next_contract_period_start: 	Start date of next contract period
         :param deletion_type: Removal mode (delete or withdraw). Empty when domain is not scheduled for removal.
         :param deletion_date: 	Date the domain is scheduled for deletion or withdrawal. Is empty if domain is not
                                 scheduled for removal.
         :param add_date: Date and time this domain was created in or transferred into our system.
+        :param renew_on: Next renewal date
+        :param product_code: Code of the product, e.g. domain-co.uk-renewal
+        :param restorable_until: Latest possible restoration date
+        :param latest_deletion_date_without_renew: Last time to cancel the renewal process
+        :param paid_until: How long is the domain paid for
         :param last_change_date: Date and time of last modification of any domain data in our system.
         :param kwargs:
         """
         super().__init__(**kwargs)
         self.name = name
         self.transfer_lock_enabled = transfer_lock_enabled
         self.id = id
@@ -122,9 +137,12 @@
         self.create_date = create_date
         self.current_contract_period_end = current_contract_period_end
         self.next_contract_period_start = next_contract_period_start
         self.deletion_type = deletion_type
         self.deletion_date = deletion_date
         self.add_date = add_date
         self.last_change_date = last_change_date
-
-
+        self.renew_on = renew_on
+        self.product_code = product_code
+        self.restorable_until = restorable_until
+        self.latest_deletion_date_without_renew = latest_deletion_date_without_renew
+        self.paid_until = paid_until
```

### Comparing `python-hostingde-0.9.0/hostingde/model/domain_contact.py` & `python-hostingde-0.9.1/hostingde/model/domain_contact.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/filter.py` & `python-hostingde-0.9.1/hostingde/model/filter.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/job.py` & `python-hostingde-0.9.1/hostingde/model/job.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/record.py` & `python-hostingde-0.9.1/hostingde/model/record.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/soa_values.py` & `python-hostingde-0.9.1/hostingde/model/soa_values.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/sort.py` & `python-hostingde-0.9.1/hostingde/model/sort.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/ssl.py` & `python-hostingde-0.9.1/hostingde/model/ssl.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/zone.py` & `python-hostingde-0.9.1/hostingde/model/zone.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/model/zone_config.py` & `python-hostingde-0.9.1/hostingde/model/zone_config.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/paginator.py` & `python-hostingde-0.9.1/hostingde/paginator.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/session.py` & `python-hostingde-0.9.1/hostingde/session.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/hostingde/ssl/ssl.py` & `python-hostingde-0.9.1/hostingde/ssl/ssl.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/python_hostingde.egg-info/PKG-INFO` & `python-hostingde-0.9.1/python_hostingde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hostingde
-Version: 0.9.0
+Version: 0.9.1
 Summary: Interact with HostingDe API
 Home-page: https://github.com/cancom/python-hostingde
 Author: CANCOM OpenSource
 Author-email: opensource@cancom.de
 License: MIT
 Project-URL: Source, https://github.com/cancom/python-hostingde
 Project-URL: Bug Reports, https://github.com/cancom/python-hostingde/issues
```

### Comparing `python-hostingde-0.9.0/python_hostingde.egg-info/SOURCES.txt` & `python-hostingde-0.9.1/python_hostingde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.9.0/setup.py` & `python-hostingde-0.9.1/setup.py`

 * *Files identical despite different names*

