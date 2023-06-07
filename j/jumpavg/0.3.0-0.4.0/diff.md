# Comparing `tmp/jumpavg-0.3.0.tar.gz` & `tmp/jumpavg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jumpavg-0.3.0.tar", last modified: Mon Aug 15 11:20:15 2022, max compression
+gzip compressed data, was "jumpavg-0.4.0.tar", last modified: Wed Jun  7 12:53:41 2023, max compression
```

## Comparing `jumpavg-0.3.0.tar` & `jumpavg-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2022-08-15 11:20:15.904952 jumpavg-0.3.0/
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)    11357 2022-06-29 11:41:29.000000 jumpavg-0.3.0/LICENSE.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)       89 2022-06-29 11:41:29.000000 jumpavg-0.3.0/MANIFEST.in
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2195 2022-08-15 11:20:15.904952 jumpavg-0.3.0/PKG-INFO
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     1251 2022-08-15 11:14:17.000000 jumpavg-0.3.0/README.rst
-drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2022-08-15 11:20:15.904952 jumpavg-0.3.0/jumpavg/
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3454 2022-08-15 11:14:17.000000 jumpavg-0.3.0/jumpavg/AvgStdevStats.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     5502 2022-08-15 11:14:17.000000 jumpavg-0.3.0/jumpavg/BitCountingGroup.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     7223 2022-08-15 11:14:17.000000 jumpavg-0.3.0/jumpavg/BitCountingGroupList.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     6188 2022-08-15 11:14:17.000000 jumpavg-0.3.0/jumpavg/BitCountingStats.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      870 2022-08-11 08:24:17.000000 jumpavg-0.3.0/jumpavg/__init__.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2983 2022-08-15 11:14:17.000000 jumpavg-0.3.0/jumpavg/classify.py
-drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2022-08-15 11:20:15.904952 jumpavg-0.3.0/jumpavg.egg-info/
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2195 2022-08-15 11:20:15.000000 jumpavg-0.3.0/jumpavg.egg-info/PKG-INFO
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      330 2022-08-15 11:20:15.000000 jumpavg-0.3.0/jumpavg.egg-info/SOURCES.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        1 2022-08-15 11:20:15.000000 jumpavg-0.3.0/jumpavg.egg-info/dependency_links.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        8 2022-08-15 11:20:15.000000 jumpavg-0.3.0/jumpavg.egg-info/top_level.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      106 2022-08-15 11:20:15.904952 jumpavg-0.3.0/setup.cfg
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     1958 2022-08-15 11:14:17.000000 jumpavg-0.3.0/setup.py
+drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-06-07 12:53:41.683740 jumpavg-0.4.0/
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)    11357 2023-06-07 12:43:39.000000 jumpavg-0.4.0/LICENSE
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2317 2023-06-07 12:53:41.683740 jumpavg-0.4.0/PKG-INFO
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     1363 2023-06-07 12:19:55.000000 jumpavg-0.4.0/README.md
+drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-06-07 12:53:41.683740 jumpavg-0.4.0/jumpavg/
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      879 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/__init__.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3454 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/avg_stdev_stats.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     5703 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/bit_counting_group.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     7440 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/bit_counting_group_list.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     6493 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/bit_counting_stats.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3928 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/classify.py
+drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-06-07 12:53:41.683740 jumpavg-0.4.0/jumpavg.egg-info/
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2317 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/PKG-INFO
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      318 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/SOURCES.txt
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        1 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/dependency_links.txt
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        8 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/top_level.txt
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      995 2023-06-07 12:53:37.000000 jumpavg-0.4.0/pyproject.toml
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)       38 2023-06-07 12:53:41.683740 jumpavg-0.4.0/setup.cfg
```

### Comparing `jumpavg-0.3.0/LICENSE.txt` & `jumpavg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpavg-0.3.0/jumpavg/AvgStdevStats.py` & `jumpavg-0.4.0/jumpavg/avg_stdev_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Cisco and/or its affiliates.
+# Copyright (c) 2023 Cisco and/or its affiliates.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at:
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
```

### Comparing `jumpavg-0.3.0/jumpavg/BitCountingGroup.py` & `jumpavg-0.4.0/jumpavg/bit_counting_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Cisco and/or its affiliates.
+# Copyright (c) 2023 Cisco and/or its affiliates.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at:
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -13,16 +13,16 @@
 
 """Module holding BitCountingGroup class."""
 
 import collections
 import dataclasses
 import typing
 
-from .AvgStdevStats import AvgStdevStats
-from .BitCountingStats import BitCountingStats
+from .avg_stdev_stats import AvgStdevStats
+from .bit_counting_stats import BitCountingStats
 
 
 @dataclasses.dataclass
 class BitCountingGroup(collections.abc.Sequence):
     """Group of runs which tracks bit count in an efficient manner.
 
     This class contains methods that mutate the internal state,
@@ -42,15 +42,17 @@
 
     run_list: typing.List[typing.Union[float, AvgStdevStats]]
     """List of run to compose into this group.
     The init call takes ownership of the list,
     so the caller should clone it to avoid unexpected muations."""
     max_value: float
     """Maximal sample value to expect."""
-    comment: str = "unknown"
+    unit: float = 1.0
+    """Typical resolution of the values"""
+    comment: str = "normal"
     """Any string giving more info, e.g. "regression"."""
     prev_avg: typing.Optional[float] = None
     """Average of the previous group, if any."""
     stats: AvgStdevStats = None
     """Stats object used for computing bits.
     Almost always recomputed, except when non-None in init."""
     cached_bits: typing.Optional[float] = None
@@ -60,28 +62,31 @@
     def __post_init__(self):
         """Recompute stats is None.
 
         It is not verified whether the user provided values are valid,
         e.g. whether the stats and bits values reflect the runs.
         """
         if self.stats is None:
-            self.stats = AvgStdevStats.for_runs(self.run_list)
+            self.stats = AvgStdevStats.for_runs(runs=self.run_list)
 
     @property
     def bits(self) -> float:
         """Return overall bit content of the group list.
 
         If not cached, compute from stats and cache.
 
         :returns: The overall information content in bits.
         :rtype: float
         """
         if self.cached_bits is None:
-            self.cached_bits = BitCountingStats.for_runs(
-                [self.stats], self.max_value, self.prev_avg
+            self.cached_bits = BitCountingStats.for_runs_and_params(
+                runs=[self.stats],
+                max_value=self.max_value,
+                unit=self.unit,
+                prev_avg=self.prev_avg,
             ).bits
         return self.cached_bits
 
     def __getitem__(self, index: int) -> typing.Union[float, AvgStdevStats]:
         """Return the run at the index.
 
         :param index: Index of the run to return.
@@ -111,14 +116,15 @@
         """
         stats = AvgStdevStats.for_runs([self.stats])
         return self.__class__(
             run_list=list(self.run_list),
             stats=stats,
             cached_bits=self.cached_bits,
             max_value=self.max_value,
+            unit=self.unit,
             prev_avg=self.prev_avg,
             comment=self.comment,
         )
 
     def append(
         self, run: typing.Union[float, AvgStdevStats]
     ) -> "BitCountingGroup":
```

### Comparing `jumpavg-0.3.0/jumpavg/BitCountingGroupList.py` & `jumpavg-0.4.0/jumpavg/bit_counting_group_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Cisco and/or its affiliates.
+# Copyright (c) 2023 Cisco and/or its affiliates.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at:
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -13,16 +13,16 @@
 
 """Module holding BitCountingGroupList class."""
 
 import collections
 import dataclasses
 import typing
 
-from .AvgStdevStats import AvgStdevStats  # Just for type hints.
-from .BitCountingGroup import BitCountingGroup
+from .avg_stdev_stats import AvgStdevStats  # Just for type hints.
+from .bit_counting_group import BitCountingGroup
 
 
 @dataclasses.dataclass
 class BitCountingGroupList(collections.abc.Sequence):
     """List of data groups which tracks overall bit count.
 
     The Sequence-like access is related to the list of groups,
@@ -42,14 +42,16 @@
 
     The data can be only added, and there is some logic to skip
     recalculations if the bit count is not needed.
     """
 
     max_value: float
     """Maximal sample value to base bits computation on."""
+    unit: float = 1.0
+    """Typical resolution of the values."""
     group_list: typing.List[BitCountingGroup] = None
     """List of groups to compose this group list.
     Init also accepts None standing for an empty list.
     This class takes ownership of the list,
     so caller of init should clone their copy to avoid unexpected mutations.
     """
     bits_except_last: float = 0.0
@@ -58,15 +60,15 @@
     def __post_init__(self):
         """Turn possible None into an empty list.
 
         It is not verified whether the user provided values are valid,
         e.g. whether the cached bits values (and bits_except_last) make sense.
         """
         if self.group_list is None:
-            self.group_list = list()
+            self.group_list = []
 
     def __getitem__(self, index: int) -> BitCountingGroup:
         """Return the group at the index.
 
         :param index: Index of the group to return.
         :type index: int
         :returns: The group at the index.
@@ -86,14 +88,15 @@
         """Return a new instance with copied internal state.
 
         :returns: The copied instance.
         :rtype: BitCountingGroupList
         """
         return self.__class__(
             max_value=self.max_value,
+            unit=self.unit,
             group_list=[group.copy() for group in self.group_list],
             bits_except_last=self.bits_except_last,
         )
 
     def copy_fast(self) -> "BitCountingGroupList":
         """Return a new instance with minimaly copied internal state.
 
@@ -110,14 +113,15 @@
             # Further speedup is possible by keeping the last group
             # as a singly linked (from end) list,
             # but for CSIT sample sizes, copy of whole Python list is faster.
             # TODO: Implement linked list as an option
             # for users with many samples.
         return self.__class__(
             max_value=self.max_value,
+            unit=self.unit,
             group_list=group_list,
             bits_except_last=self.bits_except_last,
         )
 
     @property
     def bits(self) -> float:
         """Return overall bit content of the group list.
@@ -148,19 +152,23 @@
         :rtype: BitCountingGroupList
         """
         prev_avg = self.group_list[-1].stats.avg if self.group_list else None
         if isinstance(runs, BitCountingGroup):
             # It is faster to avoid stats recalculation.
             new_group = runs.copy()
             new_group.max_value = self.max_value
+            # Unit is common.
             new_group.prev_avg = prev_avg
             new_group.cached_bits = None
         else:
             new_group = BitCountingGroup(
-                run_list=runs, max_value=self.max_value, prev_avg=prev_avg
+                run_list=runs,
+                max_value=self.max_value,
+                unit=self.unit,
+                prev_avg=prev_avg,
             )
         self.bits_except_last = self.bits
         self.group_list.append(new_group)
         return self
 
     def append_run_to_to_last_group(
         self, run: typing.Union[float, AvgStdevStats]
```

### Comparing `jumpavg-0.3.0/jumpavg/BitCountingStats.py` & `jumpavg-0.4.0/jumpavg/bit_counting_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Cisco and/or its affiliates.
+# Copyright (c) 2023 Cisco and/or its affiliates.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at:
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -13,15 +13,15 @@
 
 """Module holding BitCountingStats class."""
 
 import dataclasses
 import math
 import typing
 
-from .AvgStdevStats import AvgStdevStats
+from .avg_stdev_stats import AvgStdevStats
 
 
 @dataclasses.dataclass
 class BitCountingStats(AvgStdevStats):
     """Class for statistics which include information content of a group.
 
     The information content is based on an assumption that the data
@@ -36,14 +36,16 @@
     Only for_runs method calls the parent implementation, without using super().
     """
 
     max_value: float = None
     """Maximal sample value (real or estimated).
     Default value is there just for argument ordering reasons,
     leaving None leads to exceptions."""
+    unit: float = 1.0
+    """Typical resolution of the values."""
     prev_avg: typing.Optional[float] = None
     """Population average of the previous group (if any)."""
     bits: float = None
     """The computed information content of the group.
     It is formally an argument to init function, just to keep repr string
     a valid call. ut the init value is ignored and always recomputed.
     """
@@ -70,52 +72,55 @@
         # Zero size should in principle have non-zero bits (coding zero size),
         # but zero allows users to add empty groups without affecting bits.
         self.bits = 0.0
         if self.size < 1:
             return
         if self.max_value <= 0.0:
             raise ValueError(f"Invalid max value: {self!r}")
+        max_value = self.max_value / self.unit
+        avg = self.avg / self.unit
         # Length of the sequence must be also counted in bits,
         # otherwise the message would not be decodable.
         # Model: probability of k samples is 1/k - 1/(k+1) == 1/k/(k+1)
         # This is compatible with zero size leading to zero bits.
         self.bits += math.log(self.size * (self.size + 1), 2)
         if self.prev_avg is None:
             # Avg is considered to be uniformly distributed
             # from zero to max_value.
-            self.bits += math.log(self.max_value + 1.0, 2)
+            self.bits += math.log(max_value + 1, 2)
         else:
             # Opposite triangle distribution with minimum.
-            self.bits += math.log(
-                (self.max_value * (self.max_value + 1))
-                / (abs(self.avg - self.prev_avg) + 1),
-                2,
-            )
+            prev_avg = self.prev_avg / self.unit
+            norm = prev_avg * prev_avg
+            norm -= (prev_avg - 1) * max_value
+            norm += max_value * max_value / 2
+            self.bits -= math.log((abs(avg - prev_avg) + 1) / norm, 2)
         if self.size < 2:
             return
+        stdev = self.stdev / self.unit
         # Stdev is considered to be uniformly distributed
         # from zero to max_value. That is quite a bad expectation,
         # but resilient to negative samples etc.
-        self.bits += math.log(self.max_value + 1.0, 2)
+        self.bits += math.log(max_value + 1, 2)
         # Now we know the samples lie on sphere in size-1 dimensions.
         # So it is (size-2)-sphere, with radius^2 == stdev^2 * size.
         # https://en.wikipedia.org/wiki/N-sphere
         sphere_area_ln = math.log(2)
-        sphere_area_ln += math.log(math.pi) * ((self.size - 1) / 2.0)
-        sphere_area_ln -= math.lgamma((self.size - 1) / 2.0)
-        sphere_area_ln += math.log(self.stdev + 1.0) * (self.size - 2)
-        sphere_area_ln += math.log(self.size) * ((self.size - 2) / 2.0)
+        sphere_area_ln += math.log(math.pi) * ((self.size - 1) / 2)
+        sphere_area_ln -= math.lgamma((self.size - 1) / 2)
+        sphere_area_ln += math.log(stdev + 1) * (self.size - 2)
+        sphere_area_ln += math.log(self.size) * ((self.size - 2) / 2)
         self.bits += sphere_area_ln / math.log(2)
 
-    # TODO: Rename, so pylint stops complaining about signature change.
     @classmethod
-    def for_runs(
+    def for_runs_and_params(
         cls,
         runs: typing.Iterable[typing.Union[float, AvgStdevStats]],
         max_value: float,
+        unit: float = 1.0,
         prev_avg: typing.Optional[float] = None,
     ):
         """Return new stats instance describing the sequence of runs.
 
         If you want to append data to existing stats object,
         you can simply use the stats object as the first run.
 
@@ -127,23 +132,26 @@
         The max_value cannot be None for non-zero size data.
         The implementation does not check if no datapoint exceeds max_value.
 
         TODO: Document the behavior for zero size result.
 
         :param runs: Sequence of data to describe by the new metadata.
         :param max_value: Maximal expected value.
+        :param unit: Typical resolution of the values.
         :param prev_avg: Population average of the previous group, if any.
         :type runs: Iterable[Union[float, AvgStdevStats]]
         :type max_value: Union[float, NoneType]
+        :type unit: float
         :type prev_avg: Union[float, NoneType]
         :returns: The new stats instance.
         :rtype: cls
         """
         asd = AvgStdevStats.for_runs(runs)
         ret_obj = cls(
             size=asd.size,
             avg=asd.avg,
             stdev=asd.stdev,
             max_value=max_value,
+            unit=unit,
             prev_avg=prev_avg,
         )
         return ret_obj
```

