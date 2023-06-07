# Comparing `tmp/xocto-3.1.4.tar.gz` & `tmp/xocto-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xocto-3.1.4.tar", last modified: Fri Mar 24 14:43:07 2023, max compression
+gzip compressed data, was "xocto-3.2.0.tar", last modified: Wed Jun  7 08:36:17 2023, max compression
```

## Comparing `xocto-3.1.4.tar` & `xocto-3.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:07.967107 xocto-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-24 14:42:58.000000 xocto-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-24 14:43:07.967107 xocto-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-24 14:42:58.000000 xocto-3.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-24 14:42:58.000000 xocto-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-24 14:43:07.967107 xocto-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-03-24 14:42:58.000000 xocto-3.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:07.963107 xocto-3.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-24 14:42:58.000000 xocto-3.1.4/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-03-24 14:42:58.000000 xocto-3.1.4/tests/test_localtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-24 14:42:58.000000 xocto-3.1.4/tests/test_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-03-24 14:42:58.000000 xocto-3.1.4/tests/test_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-03-24 14:42:58.000000 xocto-3.1.4/tests/test_settlement_periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:07.963107 xocto-3.1.4/xocto/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:07.967107 xocto-3.1.4/xocto/events/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/events/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/events/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    24033 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/localtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/pact_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29205 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/settlement_periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:07.967107 xocto-3.1.4/xocto/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/storage/s3_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    60238 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-24 14:42:58.000000 xocto-3.1.4/xocto/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:07.967107 xocto-3.1.4/xocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-24 14:43:07.000000 xocto-3.1.4/xocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-24 14:43:07.000000 xocto-3.1.4/xocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:43:07.000000 xocto-3.1.4/xocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:43:07.000000 xocto-3.1.4/xocto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-24 14:43:07.000000 xocto-3.1.4/xocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-24 14:43:07.000000 xocto-3.1.4/xocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-07 08:36:06.000000 xocto-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 08:36:17.789391 xocto-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 08:36:06.000000 xocto-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-07 08:36:06.000000 xocto-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 08:36:17.789391 xocto-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-07 08:36:06.000000 xocto-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_settlement_periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/events/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/events/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/pact_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29680 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/settlement_periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/s3_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60238 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/top_level.txt
```

### Comparing `xocto-3.1.4/LICENSE` & `xocto-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/PKG-INFO` & `xocto-3.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: xocto
-Version: 3.1.4
+Version: 3.2.0
 Summary: Kraken Technologies Python service utilities
 Home-page: https://github.com/octoenergy/xocto
 Author: Kraken Technologies
 Author-email: talent@octopus.energy
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # xocto - utilities for Python services
 
-Proven utilities used on Python services at Kraken Technologies. This library works with Python 3.8 and above.
+Proven utilities used on Python services at Kraken Technologies. This library
+works with Python 3.9 and above.
 
 CI status:
 
 [![CircleCI](https://circleci.com/gh/octoenergy/xocto/tree/main.svg?style=svg)](https://circleci.com/gh/octoenergy/xocto/tree/main)
 
 - PyPI detail page: <https://pypi.python.org/pypi/xocto>
 - Documentation: <https://xocto.readthedocs.io/>
```

### Comparing `xocto-3.1.4/pyproject.toml` & `xocto-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/setup.py` & `xocto-3.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from codecs import open
 from os import path
 
 from setuptools import setup
 
 REPO_ROOT = path.abspath(path.dirname(__file__))
 
-VERSION = "3.1.4"
+VERSION = "3.2.0"
 
 with open(path.join(REPO_ROOT, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xocto",
     version=VERSION,
@@ -21,15 +21,17 @@
     author_email="talent@octopus.energy",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=["xocto", "xocto.events", "xocto.storage"],
     package_data={"xocto": ["py.typed"]},
     zip_safe=False,
     install_requires=[
         "ddtrace>=1.9.0",
         "django>=3.2,<5.0",
@@ -48,14 +50,15 @@
             "black==22.12.0",
             "boto3==1.26.53",
             "botocore==1.29.53",
             "isort==5.11.4",
             "mypy-boto3-s3==1.26.0.post1",
             "mypy==0.991",
             "numpy==1.22.2",
+            "pre-commit>=3.2.0",
             "twine==4.0.2",
             "types-openpyxl==3.0.4.5",
             "types-python-dateutil==2.8.19.6",
             "types-pytz==2022.7.1.0",
             "types-requests==2.28.11.8",
             "wheel==0.38.4",
         ],
```

### Comparing `xocto-3.1.4/tests/test_localtime.py` & `xocto-3.2.0/tests/test_localtime.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/tests/test_numbers.py` & `xocto-3.2.0/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/tests/test_ranges.py` & `xocto-3.2.0/tests/test_ranges.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,7 +557,44 @@
             period.start + ONE_DAY,
         ]
         assert ranges.get_finite_datetime_ranges_from_timestamps(period, splits) == [
             ranges.FiniteDatetimeRange(period.start, splits[1]),
             ranges.FiniteDatetimeRange(splits[1], splits[0]),
             ranges.FiniteDatetimeRange(splits[0], period.end),
         ]
+
+
+class TestAnyOverlapping:
+    @pytest.mark.parametrize(
+        "ranges_",
+        [
+            [
+                ranges.Range(0, 2),
+                ranges.Range(1, 3),
+            ],
+            [
+                ranges.Range(0, 2, boundaries=ranges.RangeBoundaries.INCLUSIVE_INCLUSIVE),
+                ranges.Range(2, 4),
+            ],
+        ],
+    )
+    def test_returns_true_if_and_ranges_overlap(self, ranges_):
+        assert ranges.any_overlapping(ranges_)
+
+    @pytest.mark.parametrize(
+        "ranges_",
+        [
+            [
+                ranges.Range(0, 2),
+                ranges.Range(2, 4),
+            ],
+            [
+                ranges.Range(0, 2),
+                ranges.Range(2, 4, boundaries=ranges.RangeBoundaries.EXCLUSIVE_INCLUSIVE),
+            ],
+        ],
+    )
+    def test_returns_false_if_no_ranges_overlap(self, ranges_):
+        assert not ranges.any_overlapping(ranges_)
+
+    def test_returns_false_for_empty_set_of_ranges(self):
+        assert not ranges.any_overlapping([])
```

### Comparing `xocto-3.1.4/tests/test_settlement_periods.py` & `xocto-3.2.0/tests/test_settlement_periods.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/events/core.py` & `xocto-3.2.0/xocto/events/core.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/health.py` & `xocto-3.2.0/xocto/health.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/localtime.py` & `xocto-3.2.0/xocto/localtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,18 +166,24 @@
     calling `.date()` on it and subtracting a day. If `tz` is not provided, the function will
     return the date before `dt` in the local time zone.
     """
     return day_before(date(dt, tz))
 
 
 def day_before(d: datetime_.date) -> datetime_.date:
+    """
+    Return the date of the day before the passed date.
+    """
     return d - datetime_.timedelta(days=1)
 
 
 def day_after(d: datetime_.date) -> datetime_.date:
+    """
+    Return the date of the day after the passed date.
+    """
     return d + datetime_.timedelta(days=1)
 
 
 # Returning datetimes
 
 
 def seconds_in_the_future(n: int, dt: Optional[datetime_.datetime] = None) -> datetime_.datetime:
@@ -212,15 +218,15 @@
     if date_or_datetime is None:
         date_: Date = today(tz)
     elif isinstance(date_or_datetime, datetime_.datetime):
         # Although this function is meant to be used on dates, we want to handle datetimes
         # properly as well, as these are frequently passed in as a way of 'truncating' them to
         # midnight on that date.
         if timezone.is_naive(date_or_datetime):
-            # Default to localtime if no tz provided, as_localtime takes tz aware args
+            # Default to localtime if no tz provided, as_localtime takes tz aware args.
             date_ = date(timezone.make_aware(date_or_datetime), tz)
         else:
             date_ = date(date_or_datetime, tz)
     else:
         date_ = date_or_datetime
 
     naive_midnight = datetime_.datetime.combine(date_, datetime_.datetime.min.time())
@@ -275,14 +281,17 @@
     naive_datetime = datetime_.datetime.combine(_date, datetime_.time(hour))
     return timezone.make_aware(naive_datetime, timezone=tz)
 
 
 def datetime_from_epoch_timestamp(
     timestamp: int | float, tz: timezone.zoneinfo.ZoneInfo | None = None
 ) -> datetime_.datetime:
+    """
+    Return a TZ-aware datetime for the passed epoch timestamp.
+    """
     naive_datetime_in_utc = datetime_.datetime.utcfromtimestamp(timestamp)
     utc_dt = timezone.make_aware(naive_datetime_in_utc, timezone=UTC)
     return timezone.localtime(utc_dt, timezone=tz)
 
 
 def latest(
     _date: datetime_.date | None = None, tz: timezone.zoneinfo.ZoneInfo | None = None
@@ -295,14 +304,19 @@
     if _date is None:
         _date = today()
     naive_midnight = datetime_.datetime.combine(_date, datetime_.datetime.max.time())
     return timezone.make_aware(naive_midnight, timezone=tz)
 
 
 def combine(_date: datetime_.date, _time: datetime_.time, tz: timezone.zone) -> datetime_.datetime:
+    """
+    Return a TZ-aware datetime obtained by combining the given date and time.
+
+    It's a TZ-aware wrapper around datetime.datetime.combine.
+    """
     combined_dt = datetime_.datetime.combine(_date, _time)
     if tz is datetime_.timezone.utc:
         return combined_dt.replace(tzinfo=tz)
     return tz.localize(combined_dt)
 
 
 # Converting dates into datetime pairs
@@ -319,14 +333,21 @@
     """
     return midnight(_date, tz), next_midnight(_date, tz)
 
 
 def month_boundaries(month: int, year: int) -> Tuple[datetime_.datetime, datetime_.datetime]:
     """
     Return the boundary datetimes of a given month.
+
+    The boundary consists of a 2-tuple of: midnight of the first day of the month and midnight of the first day of the next month.
+
+    For example:
+
+        >>> month_boundaries(1, 2020)
+        ((datetime.datetime(2020, 1, 1, 0, 0), datetime.datetime(2020, 2, 1, 0, 0))
     """
     start_date = datetime_.date(year, month, 1)
     end_date = start_date + relativedelta(months=1)
     return (midnight(start_date), midnight(end_date))
 
 
 def as_range(
@@ -406,18 +427,24 @@
         dt_as_timestamp, timedelta_seconds, rounding=rounding
     )
     quantised_dt = datetime_.datetime.fromtimestamp(quantised_dt_timestamp, tz=dt.tzinfo)
     return as_localtime(quantised_dt)
 
 
 def nearest_half_hour(dt: datetime_.datetime) -> datetime_.datetime:
+    """
+    Return the nearest half-hour datetime to the passed datetime.
+    """
     return quantise(dt, datetime_.timedelta(minutes=30))
 
 
 def is_last_day_of_month(_date: datetime_.date) -> bool:
+    """
+    Return True if the given date is the last day of the month.
+    """
     next_day = _date + datetime_.timedelta(days=1)
     if _date.month != next_day.month:
         return True
     return False
 
 
 def start_of_month(dt: datetime_.datetime | None = None) -> datetime_.datetime:
@@ -427,15 +454,15 @@
     if not dt:
         dt = now()
     return midnight(dt + relativedelta(day=1))
 
 
 def end_of_month(dt: datetime_.datetime | None = None) -> datetime_.datetime:
     """
-    Return the start datetime of the month for dt passed - or of current month.
+    Return the start datetime of the next month for dt passed - or of next month.
     """
     if not dt:
         dt = now()
     return midnight(dt + relativedelta(day=1, months=1))
 
 
 def first_day_of_month(dt: datetime_.datetime | None = None) -> datetime_.date:
```

### Comparing `xocto-3.1.4/xocto/numbers.py` & `xocto-3.2.0/xocto/numbers.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/pact_testing.py` & `xocto-3.2.0/xocto/pact_testing.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/ranges.py` & `xocto-3.2.0/xocto/ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,25 @@
     * The `is_disjoint` function will tell you if two ranges are disjoint
         >>> Range(0, 2).is_disjoint(Range(3, 5))
         True
         >>> Range(0, 2).is_disjoint(Range(2, 5))  # Since the default is not right-inclusive
         True
 
     * The `union` function (which is aliased to the or (|) operator), will return a range which
-      covers two overlapping (or adjacent) ranges, or None if they are disjoint.
+      covers two overlapping (or touching) ranges, or None if they are disjoint.
         >>> Range(0, 2).union(Range(1, 3))
         <Range: [0,3)>
         >>> Range(0, 2) | Range(2, 4)
         <Range: [0,4)>
         >>> Range(0, 2) | Range(3, 4)
         None
         >>> Range(0, 2) | Range(2, 4, boundaries="(]")
         None
+        >>> Range(0, 2, boundaries="[]") | Range(3, 4)  # Since Range doesn't understand that 2 and 3 are adjacent.
+        None
 
     * The `difference` function (which is aliased to the subtraction (-) operator), will return a
       range which contains the bit of this range which is not covered by the other range, or a
       rangeset which contains the bits of this range which are not covered (or None if the other
       range covers this one).
         >>> Range(0, 4) - Range(2, 4)
         <Range: [0,2)>
@@ -168,15 +170,15 @@
         self._is_right_inclusive = not self._is_right_exclusive
 
         if self.start is None:
             if self._is_left_inclusive:
                 raise ValueError("Range with unbounded start must be left-exclusive")
         elif self.end is None:
             if self._is_right_inclusive:
-                raise ValueError("Ranges with unbounded ends must be right-inclusive")
+                raise ValueError("Range with unbounded end must be right-exclusive")
         else:
             check_op = {
                 RangeBoundaries.EXCLUSIVE_EXCLUSIVE: operator.lt,
                 RangeBoundaries.EXCLUSIVE_INCLUSIVE: operator.lt,
                 RangeBoundaries.INCLUSIVE_EXCLUSIVE: operator.lt,
                 RangeBoundaries.INCLUSIVE_INCLUSIVE: operator.le,
             }[self.boundaries]
@@ -826,7 +828,19 @@
             [finite_datetime_range.start, *timestamps_in_range],
             [*timestamps_in_range, finite_datetime_range.end],
         )
         # We don't need to split when a timestamp is exactly at the start
         # or end of the period.
         if start != end
     ]
+
+
+def any_overlapping(ranges: Sequence[Range[T]]) -> bool:
+    """Return true if any of the passed Ranges are overlapping."""
+    if not ranges:
+        return False
+    range_set = RangeSet[T]([ranges[0]])
+    for range in ranges[1:]:
+        if range_set.intersection(range):
+            return True
+        range_set.add(range)
+    return False
```

### Comparing `xocto-3.1.4/xocto/settlement_periods.py` & `xocto-3.2.0/xocto/settlement_periods.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/storage/files.py` & `xocto-3.2.0/xocto/storage/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import csv
 import hashlib
 import io
 import os
 import tempfile
 from typing import IO, Any, AnyStr, Callable
 
-import openpyxl
 import pandas as pd
 import xlrd
 
 XLRD_FLOAT_TYPE = 2
 
 
 def size(file: IO[AnyStr]) -> int:
@@ -65,14 +64,16 @@
         encoding:           Encoding scheme for csv file.
         errors:             How file object should handle encoding errors.
         quoting:            The type of quoting the output CSV file should have
         delimiter:          The delimiter the output CSV file should have
 
     """
     # data_only to extract values from formulae and not formulas themselves
+    import openpyxl
+
     workbook = openpyxl.load_workbook(xlsx_filepath, data_only=True, read_only=True)
     sheet = workbook.active
 
     csv_file, wr = _get_csv_file_and_writer(csv_filepath, encoding, errors, quoting, delimiter)
 
     for row in sheet.rows:
         wr.writerow([cell.value for cell in row])
```

### Comparing `xocto-3.1.4/xocto/storage/s3_select.py` & `xocto-3.2.0/xocto/storage/s3_select.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/storage/storage.py` & `xocto-3.2.0/xocto/storage/storage.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/tracing.py` & `xocto-3.2.0/xocto/tracing.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto/types.py` & `xocto-3.2.0/xocto/types.py`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto.egg-info/PKG-INFO` & `xocto-3.2.0/xocto.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: xocto
-Version: 3.1.4
+Version: 3.2.0
 Summary: Kraken Technologies Python service utilities
 Home-page: https://github.com/octoenergy/xocto
 Author: Kraken Technologies
 Author-email: talent@octopus.energy
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # xocto - utilities for Python services
 
-Proven utilities used on Python services at Kraken Technologies. This library works with Python 3.8 and above.
+Proven utilities used on Python services at Kraken Technologies. This library
+works with Python 3.9 and above.
 
 CI status:
 
 [![CircleCI](https://circleci.com/gh/octoenergy/xocto/tree/main.svg?style=svg)](https://circleci.com/gh/octoenergy/xocto/tree/main)
 
 - PyPI detail page: <https://pypi.python.org/pypi/xocto>
 - Documentation: <https://xocto.readthedocs.io/>
```

### Comparing `xocto-3.1.4/xocto.egg-info/SOURCES.txt` & `xocto-3.2.0/xocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xocto-3.1.4/xocto.egg-info/requires.txt` & `xocto-3.2.0/xocto.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 black==22.12.0
 boto3==1.26.53
 botocore==1.29.53
 isort==5.11.4
 mypy-boto3-s3==1.26.0.post1
 mypy==0.991
 numpy==1.22.2
+pre-commit>=3.2.0
 twine==4.0.2
 types-openpyxl==3.0.4.5
 types-python-dateutil==2.8.19.6
 types-pytz==2022.7.1.0
 types-requests==2.28.11.8
 wheel==0.38.4
```

