# Comparing `tmp/robotools-1.5.3.tar.gz` & `tmp/robotools-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotools-1.5.3.tar", last modified: Wed Mar 22 13:58:11 2023, max compression
+gzip compressed data, was "robotools-1.6.1.tar", last modified: Wed Jun  7 12:53:36 2023, max compression
```

## Comparing `robotools-1.5.3.tar` & `robotools-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:58:11.000000 robotools-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-03-22 13:57:46.000000 robotools-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-22 13:58:11.000000 robotools-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-22 13:57:46.000000 robotools-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-22 13:57:46.000000 robotools-1.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-22 13:57:46.000000 robotools-1.5.3/robotools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools/evotools/
--rw-r--r--   0 runner    (1001) docker     (123)    66701 2023-03-22 13:57:46.000000 robotools-1.5.3/robotools/evotools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools/liquidhandling/
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-03-22 13:57:46.000000 robotools-1.5.3/robotools/liquidhandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   134018 2023-03-22 13:57:46.000000 robotools-1.5.3/robotools/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-03-22 13:57:46.000000 robotools-1.5.3/robotools/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-03-22 13:57:46.000000 robotools-1.5.3/robotools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-22 13:58:11.000000 robotools-1.5.3/robotools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:58:11.000000 robotools-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-22 13:57:46.000000 robotools-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-07 12:53:10.000000 robotools-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-07 12:53:36.287405 robotools-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 12:53:10.000000 robotools-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 12:53:10.000000 robotools-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.283405 robotools-1.6.1/robotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/test_transform.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/transform.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/utils.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/evotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/evotools/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    26749 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/commands.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)   172857 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/types.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    52678 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/worklist.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59566 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/test_worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45274 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/worklist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/liquidhandling/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/liquidhandling/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/composition.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/labware.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    56943 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    44659 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/labware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/test_labware.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.283405 robotools-1.6.1/robotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:53:36.287405 robotools-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-07 12:53:10.000000 robotools-1.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `robotools-1.5.3/LICENSE` & `robotools-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotools-1.5.3/README.md` & `robotools-1.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [![PyPI version](https://img.shields.io/pypi/v/robotools)](https://pypi.org/project/robotools)
 [![pipeline](https://github.com/jubiotech/robotools/workflows/pipeline/badge.svg)](https://github.com/jubiotech/robotools/actions)
 [![coverage](https://codecov.io/gh/jubiotech/robotools/branch/master/graph/badge.svg)](https://codecov.io/gh/jubiotech/robotools)
 [![documentation](https://readthedocs.org/projects/robotools/badge/?version=latest)](https://robotools.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/358629210.svg)](https://zenodo.org/badge/latestdoi/358629210)
 
 # `robotools`
+
 This is a package for debugging and planning liquid handling operations, writing worklist files for the Tecan FreedomEVO platform on the fly.
 
 You can visit the documentation at https://robotools.readthedocs.io, where the [notebooks](https://github.com/jubiotech/robotools/tree/master/notebooks)
 are rendered next to auto-generated API documentation.
 
 # Installation
+
 `robotools` is available through [PyPI](https://pypi.org/project/robotools/):
 
 ```
 pip install robotools
 ```
 
 # Contributing
+
 The easiest way to contribute is to report bugs by opening [Issues](https://github.com/JuBiotech/robotools/issues).
 
 We apply automated code style normalization using `black`.
 This is done with a `pre-commit`, which you can set up like this:
 1. `pip install pre-commit`
 2. `pre-commit install`
 3. `pre-commit run --all`
 
 Step 2.) makes sure that the `pre-commit` runs automatically before you make a commit.
 
 Step 3.) runs it manually.
 
 # Usage and Citing
+
 `robotools` is licensed under the [GNU Affero General Public License v3.0](https://github.com/JuBiotech/robotools/blob/master/LICENSE).
 
 When using `robotools` in your work, please cite the [corresponding software version](https://doi.org/10.5281/zenodo.4697605).
 
 ```bibtex
 @software{robotools,
   author       = {Michael Osthege and
```

### Comparing `robotools-1.5.3/robotools/evotools/__init__.py` & `robotools-1.6.1/robotools/evotools/worklist.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,27 @@
 """ Creating worklist files for the Tecan Freedom EVO.
 """
 import collections
-import enum
 import logging
 import math
 import os
 import typing
+import warnings
 
 import numpy
 
-from .. import liquidhandling, transform
+from robotools.evotools import commands
+from robotools.evotools.exceptions import InvalidOperationError
+from robotools.evotools.types import Tip, int_to_tip
 
-logger = logging.getLogger("evotools")
-
-
-class Labwares(str, enum.Enum):
-    """Built-in EVOware labware identifiers."""
-
-    SystemLiquid = "Systemliquid"
-
-
-class Tip(enum.IntEnum):
-    Any = -1
-    T1 = 1
-    T2 = 2
-    T3 = 4
-    T4 = 8
-    T5 = 16
-    T6 = 32
-    T7 = 64
-    T8 = 128
-
-
-class InvalidOperationError(Exception):
-    pass
+from .. import liquidhandling
 
+__all__ = ("Worklist",)
 
-def _int_to_tip(tip_int: int):
-    """Asserts a Tecan Tip class to an int between 1 and 8."""
-    if not 1 <= tip_int <= 8:
-        raise ValueError(
-            f"Tip is {tip_int} with type {type(tip_int)}, but should be an int between 1 and 8 for _int_to_tip conversion."
-        )
-    if tip_int == 1:
-        return Tip.T1
-    elif tip_int == 2:
-        return Tip.T2
-    elif tip_int == 3:
-        return Tip.T3
-    elif tip_int == 4:
-        return Tip.T4
-    elif tip_int == 5:
-        return Tip.T5
-    elif tip_int == 6:
-        return Tip.T6
-    elif tip_int == 7:
-        return Tip.T7
-    elif tip_int == 8:
-        return Tip.T8
+logger = logging.getLogger("evotools")
 
 
 def _prepare_aspirate_dispense_parameters(
     rack_label: str,
     position: int,
     volume: float,
     liquid_class: str = "",
@@ -144,21 +104,21 @@
 
     # optional parameters
     if not isinstance(liquid_class, str) or ";" in liquid_class:
         raise ValueError(f"Invalid liquid_class: {liquid_class}")
 
     if isinstance(tip, int) and not isinstance(tip, Tip):
         # User-specified integers from 1-8 need to be converted to Tecan logic
-        tip = _int_to_tip(tip)
+        tip = int_to_tip(tip)
 
     if isinstance(tip, collections.abc.Iterable):
         tips = []
         for element in tip:
             if isinstance(element, int) and not isinstance(element, Tip):
-                tips.append(_int_to_tip(element))
+                tips.append(int_to_tip(element))
             elif isinstance(element, Tip):
                 if element == -1:
                     raise ValueError(
                         "When Iterables are used, no Tip.Any elements are allowed. Pass just one Tip.Any instead."
                     )
                 tips.append(element)
             else:
@@ -178,305 +138,14 @@
 
     # apply rounding and corrections for the right string formatting
     volume = f"{numpy.round(volume, decimals=2):.2f}"
     tip = "" if tip == -1 else tip
     return rack_label, position, volume, liquid_class, tip, rack_id, tube_id, rack_type, forced_rack_type
 
 
-def _prepare_evo_aspirate_dispense_parameters(
-    labware: liquidhandling.Labware,
-    wells: typing.Union[str, typing.Sequence[str], numpy.ndarray],
-    *,
-    labware_position: typing.Tuple[int, int],
-    volume: typing.Union[float, typing.List[float], int],
-    liquid_class: str,
-    tips: typing.Union[typing.List[Tip], typing.List[int]],
-    max_volume: typing.Optional[int] = None,
-) -> typing.Tuple[str, list, tuple, float, str, list]:
-    """Validates and prepares aspirate/dispense parameters.
-
-    Parameters
-    ----------
-    labware : liquidhandling.Labware
-        Source labware
-    wells : list of str
-        List with target well ID(s)
-    labware_position : tuple
-        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
-    volume : int, float or list
-        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
-    liquid_class : str, optional
-        Overwrites the liquid class for this step (max 32 characters)
-    tips : list of int
-        Tip(s) that will be selected (out of tips 1-8)
-    max_volume : int, optional
-        Maximum allowed volume
-
-    Returns
-    -------
-    labware : liquidhandling.Labware
-        Source labware
-    wells : list of str
-        List with target well ID(s)
-    labware_position : tuple
-        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
-    volume : list
-        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
-    liquid_class : str, optional
-        Overwrites the liquid class for this step (max 32 characters)
-    tips : list of int
-        Tip(s) that will be selected (out of tips 1-8)
-    """
-    if labware is None:
-        raise ValueError("Missing required parameter: labware")
-    if not isinstance(labware, liquidhandling.Labware):
-        raise ValueError(f"Invalid labware: {labware}")
-
-    if wells is None:
-        raise ValueError("Missing required parameter: wells")
-    if not isinstance(wells, (str, list, tuple, numpy.ndarray)):
-        raise ValueError(f"Invalid wells: {wells}")
-    if not len(wells) == len(tips):
-        raise ValueError(f"Invalid wells: wells and tips need to have the same length.")
-    if labware_position is None:
-        raise ValueError("Missing required parameter: position")
-    if not all(isinstance(position, int) for position in labware_position) or any(
-        position < 0 for position in labware_position
-    ):
-        raise ValueError(f"Invalid position: {labware_position}")
-
-    if volume is None:
-        raise ValueError("Missing required parameter: volume")
-    if isinstance(volume, list):
-        for vol in volume:
-            try:
-                vol = float(vol)
-            except:
-                raise ValueError(f"Invalid volume: {vol}")
-            if vol < 0 or vol > 7158278 or numpy.isnan(vol):
-                raise ValueError(f"Invalid volume: {vol}")
-            if max_volume is not None and vol > max_volume:
-                raise InvalidOperationError(f"Invalid volume: volume of {vol} exceeds max_volume.")
-        if not len(volume) == len(tips) == len(wells):
-            raise Exception(
-                f"Invalid volume: Tips, wells, and volume lists have different lengths ({len(tips)}, {len(wells)} and {len(volume)}, respectively)."
-            )
-    elif isinstance(volume, (float, int)):
-        # test volume like in the list section
-        if volume < 0 or volume > 7158278 or numpy.isnan(volume):
-            raise ValueError(f"Invalid volume: {volume}")
-        if max_volume is not None and volume > max_volume:
-            raise InvalidOperationError(f"Invalid volume: volume of {volume} exceeds max_volume.")
-        # convert volume to list and multiply list to reach identical length as wells
-        volume = [float(volume)] * len(wells)
-    else:
-        raise ValueError(f"Invalid volume: {volume}")
-
-    # apply rounding and corrections for the right string formatting
-    volume = numpy.round(volume, decimals=2).tolist()
-
-    if liquid_class is None:
-        raise ValueError(f"Missing required parameter: liquid_class")
-    if not isinstance(liquid_class, str) or ";" in liquid_class:
-        raise ValueError(f"Invalid liquid_class: {liquid_class}")
-
-    if tips is None:
-        raise ValueError(f"Missing required parameter: tips")
-    for tip in tips:
-        if not isinstance(tip, (int, Tip)):
-            raise ValueError(f"Invalid type of tips: {type(tip)}. Has to be int or Tip.")
-    tecan_tips = []
-    for tip in tips:
-        if isinstance(tip, int) and not isinstance(tip, Tip):
-            # User-specified integers from 1-8 need to be converted to Tecan logic
-            tip = _int_to_tip(tip)
-        tecan_tips.append(tip)
-
-    return labware, wells, labware_position, volume, liquid_class, tecan_tips
-
-
-def _prepare_evo_wash_parameters(
-    *,
-    tips: typing.Union[typing.List[Tip], typing.List[int]],
-    waste_location: typing.Tuple[int, int],
-    cleaner_location: typing.Tuple[int, int],
-    arm: int = 0,
-    waste_vol: float = 3.0,
-    waste_delay: int = 500,
-    cleaner_vol: float = 4.0,
-    cleaner_delay: int = 500,
-    airgap: int = 10,
-    airgap_speed: int = 70,
-    retract_speed: int = 30,
-    fastwash: int = 1,
-    low_volume: int = 0,
-) -> typing.Tuple[list, tuple, tuple, int, float, int, float, int, int, int, int, int, int]:
-    """Validates and prepares aspirate/dispense parameters.
-
-    Parameters
-    ----------
-    tips : list
-        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
-    waste_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of waste as integers
-    cleaner_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers
-    arm : int
-        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2
-    waste_vol: float
-        Volume in waste in mL (0-100)
-    waste_delay : int
-        Delay before closing valves in waste in ms (0-1000)
-    cleaner_vol: float
-        Volume in cleaner in mL (0-100)
-    cleaner_delay : int
-        Delay before closing valves in cleaner in ms (0-1000)
-    airgap : int
-        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)
-    airgap_speed : int
-        Speed of airgap aspiration in µL/s (1-1000)
-    retract_speed : int
-        Retract speed in mm/s (1-100)
-    fastwash : int
-        Use fast-wash module = 1, don't use it = 0
-    low_volume : int
-        Use pinch valves = 1, don't use them = 0
-
-    Returns
-    -------
-    tips : list
-        Tip(s) that will be selected; have been converted to tip.T1 - tip.T8 here if they weren't originally formatted that way
-    waste_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of waste as integers
-    cleaner_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers
-    arm : int
-        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2
-    waste_vol: float
-        Volume in waste in mL (0-100)
-    waste_delay : int
-        Delay before closing valves in waste in ms (0-1000)
-    cleaner_vol: float
-        Volume in cleaner in mL (0-100)
-    cleaner_delay : int
-        Delay before closing valves in cleaner in ms (0-1000)
-    airgap : int
-        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)
-    airgap_speed : int
-        Speed of airgap aspiration in µL/s (1-1000)
-    retract_speed : int
-        Retract speed in mm/s (1-100)
-    fastwash : int
-        Use fast-wash module = 1, don't use it = 0
-    low_volume : int
-        Use pinch valves = 1, don't use them = 0
-    """
-    if tips is None:
-        raise ValueError("Missing required parameter: tips")
-
-    tecan_tips = []
-    for tip in tips:
-        if isinstance(tip, int) and not isinstance(tip, Tip):
-            # User-specified integers from 1-8 need to be converted to Tecan logic
-            tip = _int_to_tip(tip)
-        tecan_tips.append(tip)
-
-    if waste_location is None:
-        raise ValueError("Missing required parameter: waste_location")
-    grid, site = waste_location
-    if not isinstance(grid, int) or not 1 <= grid <= 67:
-        raise ValueError("Grid (first number in waste_location tuple) has to be an int from 1 - 67.")
-    if not isinstance(site, int) or not 0 <= site <= 127:
-        raise ValueError("Site (second number in waste_location tuple) has to be an int from 0 - 127.")
-
-    if cleaner_location is None:
-        raise ValueError("Missing required parameter: cleaner_location")
-    grid, site = cleaner_location
-    if not isinstance(grid, int) or not 1 <= grid <= 67:
-        raise ValueError("Grid (first number in cleaner_location tuple) has to be an int from 1 - 67.")
-    if not isinstance(site, int) or not 0 <= site <= 127:
-        raise ValueError("Site (second number in cleaner_location tuple) has to be an int from 0 - 127.")
-
-    if arm is None:
-        raise ValueError("Missing required paramter: arm")
-    if not isinstance(arm, int):
-        raise ValueError("Parameter arm is not int.")
-    if not arm == 0 and not arm == 1:
-        raise ValueError("Parameter arm has to be 0 (LiHa 1) or 1 (LiHa 2).")
-
-    if waste_vol is None:
-        raise ValueError("Missing required parameter: waste_vol")
-    if not isinstance(waste_vol, float) or not 0 <= waste_vol <= 100:
-        raise ValueError("waste_vol has to be a float from 0 - 100.")
-    # round waste_vol to the first decimal (pre-requisite for Tecan's wash command)
-    waste_vol = numpy.round(waste_vol, 1)
-
-    if waste_delay is None:
-        raise ValueError("Missing required parameter: waste_delay")
-    if not isinstance(waste_delay, int) or not 0 <= waste_delay <= 1000:
-        raise ValueError("waste_delay has to be an int from 0 - 1000.")
-
-    if cleaner_vol is None:
-        raise ValueError("Missing required parameter: cleaner_vol")
-    if not isinstance(cleaner_vol, float) or not 0 <= cleaner_vol <= 100:
-        raise ValueError("cleaner_vol has to be a float from 0 - 100.")
-    # round cleaner_vol to the first decimal (pre-requisite for Tecan's wash command)
-    cleaner_vol = numpy.round(cleaner_vol, 1)
-
-    if cleaner_delay is None:
-        raise ValueError("Missing required parameter: cleaner_delay")
-    if not isinstance(cleaner_delay, int) or not 0 <= cleaner_delay <= 1000:
-        raise ValueError("cleaner_delay has to be an int from 0 - 1000.")
-
-    if airgap is None:
-        raise ValueError("Missing required parameter: airgap")
-    if not isinstance(airgap, int) or not 0 <= airgap <= 100:
-        raise ValueError("airgap has to be an int from 0 - 100.")
-
-    if airgap_speed is None:
-        raise ValueError("Missing required parameter: airgap_speed")
-    if not isinstance(airgap_speed, int) or not 1 <= airgap_speed <= 1000:
-        raise ValueError("airgap_speed has to be an int from 1 - 1000.")
-
-    if retract_speed is None:
-        raise ValueError("Missing required parameter: retract_speed")
-    if not isinstance(retract_speed, int) or not 1 <= retract_speed <= 100:
-        raise ValueError("retract_speed has to be an int from 1 - 100.")
-
-    if fastwash is None:
-        raise ValueError("Missing required paramter: fastwash")
-    if not isinstance(fastwash, int):
-        raise ValueError("Parameter fastwash is not int.")
-    if not fastwash == 0 and not fastwash == 1:
-        raise ValueError("Parameter fastwash has to be 0 (no fast-wash) or 1 (use fast-wash).")
-
-    if low_volume is None:
-        raise ValueError("Missing required paramter: low_volume")
-    if not isinstance(low_volume, int):
-        raise ValueError("Parameter low_volume is not int.")
-    if not low_volume == 0 and not low_volume == 1:
-        raise ValueError("Parameter low_volume has to be 0 (no fast-wash) or 1 (use fast-wash).")
-
-    return (
-        tecan_tips,
-        waste_location,
-        cleaner_location,
-        arm,
-        waste_vol,
-        waste_delay,
-        cleaner_vol,
-        cleaner_delay,
-        airgap,
-        airgap_speed,
-        retract_speed,
-        fastwash,
-        low_volume,
-    )
-
-
 def _optimize_partition_by(
     source: liquidhandling.Labware,
     destination: liquidhandling.Labware,
     partition_by: str,
     label: typing.Optional[str] = None,
 ) -> str:
     """Determines optimal partitioning settings.
@@ -596,101 +265,14 @@
             list(numpy.array(srcs)[order]),
             list(numpy.array(dsts)[order]),
             list(numpy.array(vols)[order]),
         )
     return column_groups
 
 
-def to_hex(dec: int):
-    """Method from stackoverflow to convert decimal to hex.
-    Link: https://stackoverflow.com/questions/5796238/python-convert-decimal-to-hex
-    Solution posted by user "Chunghee Kim" on 21.11.2020.
-    """
-    digits = "0123456789ABCDEF"
-    x = dec % 16
-    rest = dec // 16
-    if rest == 0:
-        return digits[x]
-    return to_hex(rest) + digits[x]
-
-
-def evo_make_selection_array(rows: int, columns: int, wells: numpy.ndarray):
-    """Translate well IDs to a numpy array with 1s (selected) and 0s (not selected).
-
-    Parameters
-    ----------
-    rows : int
-        Number of rows of target labware object
-    cols : int
-        Number of columns of target labware object
-    wells : List[str]
-        Selected wells by well IDs as strings (e.g. ["A01", "B01"])
-
-    Returns
-    -------
-    selection_array : numpy.ndarray
-        Numpy array in labware dimensions with selected wells as 1 and others as 0
-    """
-    # create array with a shape beffiting the labware dimensions
-    selection_array = numpy.zeros((rows, columns))
-    # get a dictionary with the "coordinates" of well IDs (A01, B01 etc) as tuples
-    well_index_dict = transform.make_well_index_dict(rows, columns)
-    # insert 1s for all selected wells
-    for well in wells:
-        selection_array[well_index_dict[well]] = 1
-    return selection_array
-
-
-def evo_get_selection(rows: int, cols: int, selected: numpy.ndarray):
-    """Function to generate the code string for the well selection of pipetting actions in EvoWare scripts (.esc).
-    Adapted from the C++ function detailed in the EvoWare manual to Python by Martin Beyß (except the test at the end).
-
-    Parameters
-    ----------
-    rows : int
-        Number of rows of target labware object
-    cols : int
-        Number of columns of target labware object
-    selected : numpy.ndarray
-        Numpy array in labware dimensions with selected wells as 1 and others as 0 (from evo_make_selection_array)
-
-    Returns
-    -------
-    selection : str
-        Code string for well selection of pipetting actions in EvoWare scripts (.esc)
-    """
-    # apply bit mask with 7 bits, adapted from function detailed in EvoWare manual
-    selection = f"0{to_hex(cols)}{rows:02d}"
-    bit_counter = 0
-    bit_mask = 0
-    for x in range(cols):
-        for y in range(rows):
-            if selected[y, x] == 1:
-                bit_mask |= 1 << bit_counter
-            bit_counter += 1
-            if bit_counter > 6:
-                selection += chr(bit_mask + 48)
-                bit_counter = 0
-                bit_mask = 0
-    if bit_counter > 0:
-        selection += chr(bit_mask + 48)
-
-    # check if wells from more than one column are selected and raise Exception if so
-    check = 0
-    for column in selected.transpose():
-        if sum(column) >= 1:
-            check += 1
-    if check >= 2:
-        raise Exception(
-            "Wells from more than one column are selected.\nSelect only wells from one column per pipetting action."
-        )
-
-    return selection
-
-
 class Worklist(list):
     """Context manager for the creation of Worklists."""
 
     def __init__(self, filepath: str = None, max_volume: int = 950, auto_split: bool = True) -> None:
         """Creates a worklist writer.
 
         Parameters
@@ -895,72 +477,30 @@
         labware: liquidhandling.Labware,
         wells: typing.Union[str, typing.List[str]],
         labware_position: typing.Tuple[int, int],
         volume: typing.Union[float, typing.List[float], int],
         liquid_class: str,
         tips: typing.Union[typing.List[Tip], typing.List[int]],
     ) -> None:
-        """Command for aspirating with the EvoWARE aspirate command. As many wells in one column may be selected as your liquid handling arm has pipettes.
-        This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string
-        specifying the target wells.
-
-        Parameters
-        ----------
-        labware : liquidhandling.Labware
-            Source labware
-        wells : list of str
-            List with target well ID(s)
-        labware_position : tuple
-            Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
-        volume : int, float or list
-            Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
-        liquid_class : str, optional
-            Overwrites the liquid class for this step (max 32 characters)
-        tips : list
-            Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
-        """
-        # perform consistency checks
-        kwargs = dict(
+        warnings.warn(
+            "The `evo_aspirate_well` method is deprecated because it's just a wrapper for the `evo_aspirate` function."
+            "Replace your `evo_aspirate_well(...)` call with `wl.append(robotools.evotools.evo_aspirate(...))`.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        cmd = commands.evo_aspirate(
             labware=labware,
             wells=wells,
             labware_position=labware_position,
             volume=volume,
             liquid_class=liquid_class,
             tips=tips,
+            max_volume=self.max_volume,
         )
-        (
-            labware,
-            wells,
-            labware_position,
-            volume,
-            liquid_class,
-            tips,
-        ) = _prepare_evo_aspirate_dispense_parameters(**kwargs, max_volume=self.max_volume)
-
-        # calculate tip_selection based on tips argument (tips are converted to evotools.Tip in _prepare_evo_aspirate_dispense_parameters)
-        tip_selection = 0
-        for tip in tips:
-            tip_selection += tip.value
-
-        # prepare volume section (volume is converted to list in _prepare_evo_aspirate_dispense_parameters)
-        tip_volumes = ""
-        for tip in [1, 2, 4, 8, 16, 32, 64, 128]:
-            if tip in [tecantip.value for tecantip in tips]:
-                tip_volumes += f'"{volume[0]}",'
-                volume.pop(0)
-            else:
-                tip_volumes += "0,"
-
-        # convert selection from list of well ids to numpy array with same dimensions as target labware (1: well is selected, 0: well is not selected)
-        selected = evo_make_selection_array(labware.n_rows, labware.n_columns, wells)
-        # create code string containing information about target well(s)
-        code_string = evo_get_selection(labware.n_rows, labware.n_columns, selected)
-        self.append(
-            f'B;Aspirate({tip_selection},"{liquid_class}",{tip_volumes}0,0,0,0,{labware_position[0]},{labware_position[1]},1,"{code_string}",0,0);'
-        )
+        self.append(cmd)
         return
 
     def dispense_well(
         self,
         rack_label: str,
         position: int,
         volume: float,
@@ -1033,72 +573,30 @@
         labware: liquidhandling.Labware,
         wells: typing.Union[str, typing.List[str]],
         labware_position: typing.Tuple[int, int],
         volume: typing.Union[float, typing.List[float], int],
         liquid_class: str,
         tips: typing.Union[typing.List[Tip], typing.List[int]],
     ) -> None:
-        """Command for dispensing using the EvoWARE dispense command. As many wells in one column may be selected as your liquid handling arm has pipettes.
-        This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string
-        specifying the target wells.
-
-        Parameters
-        ----------
-        labware : liquidhandling.Labware
-            Source labware
-        wells : list of str
-            List with target well ID(s)
-        labware_position : tuple
-            Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
-        volume : int, float or list
-            Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
-        liquid_class : str, optional
-            Overwrites the liquid class for this step (max 32 characters)
-        tips : list
-            Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
-        """
-        # perform consistency checks
-        kwargs = dict(
+        warnings.warn(
+            "The `evo_dispense_well` method is deprecated because it's just a wrapper for the `evo_dispense` function."
+            "Replace your `evo_dispense_well(...)` call with `wl.append(robotools.evotools.evo_dispense(...))`.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        cmd = commands.evo_dispense(
             labware=labware,
             wells=wells,
             labware_position=labware_position,
             volume=volume,
             liquid_class=liquid_class,
             tips=tips,
+            max_volume=self.max_volume,
         )
-        (
-            labware,
-            wells,
-            labware_position,
-            volume,
-            liquid_class,
-            tips,
-        ) = _prepare_evo_aspirate_dispense_parameters(**kwargs, max_volume=self.max_volume)
-
-        # calculate tip_selection based on tips argument (tips are converted to evotools.Tip in _prepare_evo_aspirate_dispense_parameters)
-        tip_selection = 0
-        for tip in tips:
-            tip_selection += tip.value
-
-        # prepare volume section (volume is converted to list in _prepare_evo_aspirate_dispense_parameters)
-        tip_volumes = ""
-        for tip in [1, 2, 4, 8, 16, 32, 64, 128]:
-            if tip in [tecantip.value for tecantip in tips]:
-                tip_volumes += f'"{volume[0]}",'
-                volume.pop(0)
-            else:
-                tip_volumes += "0,"
-
-        # convert selection from list of well ids to numpy array with same dimensions as target labware (1: well is selected, 0: well is not selected)
-        selected = evo_make_selection_array(labware.n_rows, labware.n_columns, wells)
-        # create code string containing information about target well(s)
-        code_string = evo_get_selection(labware.n_rows, labware.n_columns, selected)
-        self.append(
-            f'B;Dispense({tip_selection},"{liquid_class}",{tip_volumes}0,0,0,0,{labware_position[0]},{labware_position[1]},1,"{code_string}",0,0);'
-        )
+        self.append(cmd)
         return
 
     def evo_wash(
         self,
         *,
         tips: typing.Union[typing.List[Tip], typing.List[int]],
         waste_location: typing.Tuple[int, int],
@@ -1143,54 +641,30 @@
         retract_speed : int
             Retract speed in mm/s (1-100)
         fastwash : int
             Use fast-wash module = 1, don't use it = 0
         low_volume : int
             Use pinch valves = 1, don't use them = 0
         """
-
-        # perform consistency checks
-        kwargs = dict(
+        cmd = commands.evo_wash(
             tips=tips,
             waste_location=waste_location,
             cleaner_location=cleaner_location,
             arm=arm,
             waste_vol=waste_vol,
             waste_delay=waste_delay,
             cleaner_vol=cleaner_vol,
             cleaner_delay=cleaner_delay,
             airgap=airgap,
             airgap_speed=airgap_speed,
             retract_speed=retract_speed,
             fastwash=fastwash,
             low_volume=low_volume,
         )
-        (
-            tips,
-            waste_location,
-            cleaner_location,
-            arm,
-            waste_vol,
-            waste_delay,
-            cleaner_vol,
-            cleaner_delay,
-            airgap,
-            airgap_speed,
-            retract_speed,
-            fastwash,
-            low_volume,
-        ) = _prepare_evo_wash_parameters(**kwargs)
-        # calculate tip_selection based on tips argument
-        tip_selection = 0
-        for tip in tips:
-            tip_selection += tip.value
-
-        self.append(
-            f'B;Wash({tip_selection},{waste_location[0]},{waste_location[1]},{cleaner_location[0]},{cleaner_location[1]},"{waste_vol}",{waste_delay},"{cleaner_vol}",{cleaner_delay},{airgap},{airgap_speed},{retract_speed},{fastwash},{low_volume},1000,{arm});'
-        )
+        self.append(cmd)
         return
 
     def reagent_distribution(
         self,
         src_rack_label: str,
         src_start: int,
         src_end: int,
@@ -1376,22 +850,24 @@
         # diferentiate between what is needed for volume calculation and for pipetting commands
         wells_calc = numpy.array(wells).flatten("F")
         volumes_calc = numpy.array(volumes).flatten("F")
         if len(volumes_calc) == 1:
             volumes_calc = numpy.repeat(volumes_calc, len(wells_calc))
         labware.remove(wells_calc, volumes_calc, label)
         self.comment(label)
-        self.evo_aspirate_well(
+        cmd = commands.evo_aspirate(
             labware=labware,
             wells=wells,
             labware_position=labware_position,
             volume=volumes,
             liquid_class=liquid_class,
             tips=tips,
+            max_volume=self.max_volume,
         )
+        self.append(cmd)
         return
 
     def dispense(
         self,
         labware: liquidhandling.Labware,
         wells: typing.Union[str, typing.Sequence[str], numpy.ndarray],
         volumes: typing.Union[float, typing.Sequence[float], numpy.ndarray],
@@ -1462,22 +938,23 @@
         # diferentiate between what is needed for volume calculation and for pipetting commands
         wells_calc = numpy.array(wells).flatten("F")
         volumes_calc = numpy.array(volumes).flatten("F")
         if len(volumes_calc) == 1:
             volumes_calc = numpy.repeat(volumes_calc, len(wells_calc))
         labware.remove(wells_calc, volumes_calc, label)
         self.comment(label)
-        self.evo_dispense_well(
+        cmd = commands.evo_dispense(
             labware=labware,
             wells=wells,
             labware_position=labware_position,
             volume=volumes,
             liquid_class=liquid_class,
             tips=tips,
         )
+        self.append(cmd)
         return
 
     def transfer(
         self,
         source: liquidhandling.Labware,
         source_wells: typing.Union[str, typing.Sequence[str], numpy.ndarray],
         destination: liquidhandling.Labware,
```

### Comparing `robotools-1.5.3/robotools/liquidhandling/__init__.py` & `robotools-1.6.1/robotools/liquidhandling/labware.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,183 +1,62 @@
-import logging
-import typing
-import warnings
-
-import numpy
-
-logger = logging.getLogger("liquidhandling")
-
+"""Object-oriented, stateful labware representations."""
 
-class VolumeOverflowError(Exception):
-    """Error that indicates the planned overflow of a well."""
 
-    def __init__(
-        self,
-        labware: str,
-        well: str,
-        current: float,
-        change: float,
-        threshold: float,
-        label: typing.Optional[str] = None,
-    ) -> None:
-        if label:
-            super().__init__(
-                f'Too much volume for "{labware}".{well}: {current} + {change} > {threshold} in step {label}'
-            )
-        else:
-            super().__init__(f'Too much volume for "{labware}".{well}: {current} + {change} > {threshold}')
-
-
-class VolumeUnderflowError(Exception):
-    """Error that indicates the planned underflow of a well."""
-
-    def __init__(
-        self,
-        labware: str,
-        well: str,
-        current: float,
-        change: float,
-        threshold: float,
-        label: typing.Optional[str] = None,
-    ) -> None:
-        if label:
-            super().__init__(
-                f'Too little volume in "{labware}".{well}: {current} - {change} < {threshold} in step {label}'
-            )
-        else:
-            super().__init__(f'Too little volume in "{labware}".{well}: {current} - {change} < {threshold}')
+import warnings
+from typing import Dict, List, Optional, Sequence, Tuple, Union
 
+import numpy as np
 
-def _combine_composition(
-    volume_A: float,
-    composition_A: typing.Optional[typing.Dict[str, float]],
-    volume_B: float,
-    composition_B: typing.Optional[typing.Dict[str, float]],
-) -> typing.Optional[typing.Dict[str, float]]:
-    """Computes the composition of a liquid, created by the mixing of two liquids (A and B).
-
-    Parameters
-    ----------
-    volume_A : float
-        Volume of liquid A
-    composition_A : dict
-        Relative composition of liquid A
-    volume_B : float
-        Volume of liquid B
-    composition_B : dict
-        Relative composition of liquid B
-
-    Returns
-    -------
-    composition : dict
-        Composition of the new liquid created by mixing the given volumes of A and B
-    """
-    if composition_A is None or composition_B is None:
-        return None
-    # convert to volumetric fractions
-    volumetric_fractions = {k: f * volume_A for k, f in composition_A.items()}
-    # volumetrically add incoming fractions
-    for k, f in composition_B.items():
-        if not k in volumetric_fractions:
-            volumetric_fractions[k] = 0
-        volumetric_fractions[k] += f * volume_B
-    # convert back to relative fractions
-    new_composition = {k: v / (volume_A + volume_B) for k, v in volumetric_fractions.items()}
-    return new_composition
-
-
-def _get_initial_composition(
-    name: str,
-    real_wells: numpy.ndarray,
-    component_names: typing.Dict[str, typing.Union[str, None]],
-    initial_volumes: numpy.ndarray,
-) -> typing.Dict[str, typing.Union[str, None]]:
-    """Creates a dictionary of initial composition arrays.
-
-    Parameters
-    ----------
-    name : str
-        Name of the labware - used for default component names.
-    real_wells : array-like
-        2D array of non-virtual wells in the labware.
-    component_names : dict
-        User-provided dictionary that maps real well IDs to component names.
-    initial_volumes : numpy.ndarray
-        Initial volumes of real wells.
-
-    Returns
-    -------
-    composition : dict
-        The component-wise dictionary of numpy arrays that describe the composition of real wells.
-    """
-    possible_component_wells = set(numpy.unique(real_wells))
-    illegal_component_wells = set(component_names.keys()) - possible_component_wells
-    if illegal_component_wells:
-        raise ValueError(f"Invalid component name keys: {illegal_component_wells}")
-
-    is_multiwell = len(real_wells) > 1
-    composition = {}
-    for idx, w in numpy.ndenumerate(real_wells):
-        # Ignore None-valued component names, but don't allow naming of empty wells.
-        if initial_volumes[idx] == 0:
-            if component_names.get(w, None) is not None:
-                raise ValueError(
-                    f"A component name '{component_names[w]}' was specified for {name}.{w}, but the corresponding initial volume is 0."
-                )
-            continue
-
-        # Fetch a name for identifying the liquid from this non-empty well
-        default_name = f"{name}.{w}" if is_multiwell else name
-        cname = component_names.get(w, default_name)
-
-        # Make sure that a composition array exists
-        if cname not in composition:
-            composition[cname] = numpy.zeros_like(real_wells, dtype=float)
-
-        # Mark this well as filled by this component
-        composition[cname][idx] = 1
-    return composition
+from robotools.liquidhandling.composition import (
+    combine_composition,
+    get_initial_composition,
+    get_trough_component_names,
+)
+from robotools.liquidhandling.exceptions import (
+    VolumeOverflowError,
+    VolumeUnderflowError,
+)
 
 
 class Labware:
     """Represents an array of liquid cavities."""
 
     @property
-    def history(self) -> typing.List[typing.Tuple[typing.Optional[str], numpy.ndarray]]:
+    def history(self) -> List[Tuple[Optional[str], np.ndarray]]:
         """List of label/volumes history."""
         return list(zip(self._labels, self._history))
 
     @property
     def report(self) -> str:
         """A printable report of the labware history."""
         report = self.name
         for label, state in self.history:
             if label:
                 report += f"\n{label}"
-            report += f"\n{numpy.round(state, decimals=1)}"
+            report += f"\n{np.round(state, decimals=1)}"
             report += "\n"
         return report
 
     @property
-    def volumes(self) -> numpy.ndarray:
+    def volumes(self) -> np.ndarray:
         """Current volumes in the labware."""
         return self._volumes.copy()
 
     @property
-    def wells(self) -> numpy.ndarray:
+    def wells(self) -> np.ndarray:
         """Array of well ids."""
         return self._wells
 
     @property
-    def indices(self) -> typing.Dict[str, typing.Tuple[int, int]]:
+    def indices(self) -> Dict[str, Tuple[int, int]]:
         """Mapping of well-ids to numpy indices."""
         return self._indices
 
     @property
-    def positions(self) -> typing.Dict[str, int]:
+    def positions(self) -> Dict[str, int]:
         """Mapping of well-ids to EVOware-compatible position numbers."""
         return self._positions
 
     @property
     def n_rows(self) -> int:
         return len(self.row_ids)
 
@@ -186,32 +65,32 @@
         return len(self.column_ids)
 
     @property
     def is_trough(self) -> bool:
         return self.virtual_rows != None
 
     @property
-    def composition(self) -> typing.Dict[str, numpy.ndarray]:
+    def composition(self) -> Dict[str, np.ndarray]:
         """Relative composition of the liquids.
 
         This dictionary maps liquid names (keys) to arrays of relative amounts in each well.
         """
         return self._composition
 
     def __init__(
         self,
         name: str,
         rows: int,
         columns: int,
         *,
         min_volume: float,
         max_volume: float,
-        initial_volumes: typing.Optional[typing.Union[float, numpy.ndarray]] = None,
-        virtual_rows: typing.Optional[int] = None,
-        component_names: typing.Optional[typing.Dict[str, str]] = None,
+        initial_volumes: Optional[Union[float, np.ndarray]] = None,
+        virtual_rows: Optional[int] = None,
+        component_names: Optional[Dict[str, str]] = None,
     ) -> None:
         """Creates a `Labware` object.
 
         Parameters
         ----------
         name : str
             Label that the labware is identified by.
@@ -252,40 +131,38 @@
                 UserWarning,
                 stacklevel=2,
             )
 
         # explode convenience parameters
         if initial_volumes is None:
             initial_volumes = 0
-        initial_volumes = numpy.array(initial_volumes)
+        initial_volumes = np.array(initial_volumes)
         if initial_volumes.shape == ():
-            initial_volumes = numpy.full((rows, columns), initial_volumes)
+            initial_volumes = np.full((rows, columns), initial_volumes)
         else:
             initial_volumes = initial_volumes.reshape((rows, columns))
         assert initial_volumes.shape == (
             rows,
             columns,
         ), f"Invalid shape of initial_volumes: {initial_volumes.shape}"
-        if numpy.any(initial_volumes < 0):
+        if np.any(initial_volumes < 0):
             raise ValueError("initial_volume cannot be negative")
-        if numpy.any(initial_volumes > max_volume):
+        if np.any(initial_volumes > max_volume):
             raise ValueError("initial_volume cannot be above max_volume")
 
         # initialize properties
         self.name = name
         self.row_ids = tuple("ABCDEFGHIJKLMNOPQRSTUVWXYZ"[: rows if not virtual_rows else virtual_rows])
         self.column_ids = list(range(1, columns + 1))
         self.min_volume = min_volume
         self.max_volume = max_volume
         self.virtual_rows = virtual_rows
 
         # generate arrays/mappings of well ids
-        self._wells = numpy.array(
-            [[f"{row}{column:02d}" for column in self.column_ids] for row in self.row_ids]
-        )
+        self._wells = np.array([[f"{row}{column:02d}" for column in self.column_ids] for row in self.row_ids])
         if virtual_rows is None:
             self._indices = {
                 f"{row}{column:02d}": (r, c)
                 for r, row in enumerate(self.row_ids)
                 for c, column in enumerate(self.column_ids)
             }
             self._positions = {
@@ -303,25 +180,25 @@
                 f"{vrow}{column:02d}": 1 + c * virtual_rows + vr
                 for vr, vrow in enumerate(self.row_ids)
                 for c, column in enumerate(self.column_ids)
             }
 
         # initialize state variables
         self._volumes = initial_volumes.copy().astype(float)
-        self._history: typing.List[numpy.ndarray] = [self.volumes]
-        self._labels: typing.List[typing.Optional[str]] = ["initial"]
-        self._composition = _get_initial_composition(
+        self._history: List[np.ndarray] = [self.volumes]
+        self._labels: List[Optional[str]] = ["initial"]
+        self._composition = get_initial_composition(
             name,
             real_wells=self.wells[[0], :] if virtual_rows else self.wells,
             component_names=component_names or {},
             initial_volumes=initial_volumes,
         )
         super().__init__()
 
-    def get_well_composition(self, well: str) -> typing.Dict[str, float]:
+    def get_well_composition(self, well: str) -> Dict[str, float]:
         """Retrieves the relative composition of a well.
 
         Parameters
         ----------
         well : str
             ID of the well for which to retrieve the composition.
 
@@ -335,38 +212,38 @@
             return None
         idx = self.indices[well]
         well_comp = {k: f[idx] for k, f in self.composition.items() if f[idx] > 0}
         return well_comp
 
     def add(
         self,
-        wells: typing.Sequence[str],
-        volumes: typing.Union[float, typing.Sequence[float], numpy.ndarray],
-        label: typing.Optional[str] = None,
-        compositions: typing.Optional[typing.List[typing.Optional[typing.Dict[str, float]]]] = None,
+        wells: Sequence[str],
+        volumes: Union[float, Sequence[float], np.ndarray],
+        label: Optional[str] = None,
+        compositions: Optional[List[Optional[Dict[str, float]]]] = None,
     ) -> None:
         """Adds volumes to wells.
 
         Parameters
         ----------
         wells : iterable of str
             Well ids
         volumes : float, iterable of float
             Scalar or iterable of volumes
         label : str
             Description of the operation
         compositions : iterable
             List of composition dictionaries ({ name : relative amount })
         """
-        wells = numpy.array(wells).flatten("F")
-        volumes = numpy.array(volumes).flatten("F")
+        wells = np.array(wells).flatten("F")
+        volumes = np.array(volumes).flatten("F")
         if len(volumes) == 1:
-            volumes = numpy.repeat(volumes, len(wells))
+            volumes = np.repeat(volumes, len(wells))
         assert len(volumes) == len(wells), "Number of volumes must equal the number of wells"
-        assert numpy.all(volumes >= 0), "Volumes must be positive or zero."
+        assert np.all(volumes >= 0), "Volumes must be positive or zero."
         if compositions is not None:
             assert len(compositions) == len(
                 wells
             ), "Well compositions must be given for either all or none of the wells."
         else:
             compositions = [None] * len(wells)
 
@@ -380,72 +257,72 @@
 
             self._volumes[idx] = v_new
 
             if composition is not None and self._composition is not None:
                 assert isinstance(composition, dict), "Well compositions must be given as dicts"
                 # update the volumentric composition for this well
                 original_composition = self.get_well_composition(well)
-                new_composition = _combine_composition(v_original, original_composition, volume, composition)
+                new_composition = combine_composition(v_original, original_composition, volume, composition)
                 for k, f in new_composition.items():
                     if not k in self._composition:
                         # a new liquid is being added
-                        self._composition[k] = numpy.zeros_like(self.volumes)
+                        self._composition[k] = np.zeros_like(self.volumes)
                     self._composition[k][idx] = f
 
         self.log(label)
         return
 
     def remove(
         self,
-        wells: typing.Sequence[str],
-        volumes: typing.Union[float, typing.Sequence[float], numpy.ndarray],
-        label: typing.Optional[str] = None,
+        wells: Sequence[str],
+        volumes: Union[float, Sequence[float], np.ndarray],
+        label: Optional[str] = None,
     ) -> None:
         """Removes volumes from wells.
 
         Parameters
         ----------
         wells : iterable of str
             Well ids
         volumes : float, iterable of float
             Scalar or iterable of volumes
         label : str
             Description of the operation
         """
-        wells = numpy.array(wells).flatten("F")
-        volumes = numpy.array(volumes).flatten("F")
+        wells = np.array(wells).flatten("F")
+        volumes = np.array(volumes).flatten("F")
         if len(volumes) == 1:
-            volumes = numpy.repeat(volumes, len(wells))
+            volumes = np.repeat(volumes, len(wells))
         assert len(volumes) == len(wells), "Number of volumes must number of wells"
-        assert numpy.all(volumes >= 0), "Volumes must be positive or zero."
+        assert np.all(volumes >= 0), "Volumes must be positive or zero."
         for well, volume in zip(wells, volumes):
             idx = self.indices[well]
             v_original = self._volumes[idx]
             v_new = v_original - volume
 
             if v_new < self.min_volume:
                 raise VolumeUnderflowError(self.name, well, v_original, volume, self.min_volume, label)
 
             self._volumes[idx] -= volume
         self.log(label)
         return
 
-    def log(self, label: typing.Optional[str]) -> None:
+    def log(self, label: Optional[str]) -> None:
         """Logs the current volumes to the history.
 
         Parameters
         ----------
         label : str
             A label to insert in the history.
         """
         self._history.append(self.volumes)
         self._labels.append(label)
         return
 
-    def condense_log(self, n: int, label: typing.Optional[str] = "last") -> None:
+    def condense_log(self, n: int, label: Optional[str] = "last") -> None:
         """Condense the last n log entries.
 
         Parameters
         ----------
         n : int
             Number of log entries to condense
         label : str
@@ -461,88 +338,33 @@
         self._history = self._history[:-n]
         # append the last state
         self._labels.append(label)
         self._history.append(state)
         return
 
     def __repr__(self) -> None:
-        return f"{self.name}\n{numpy.round(self.volumes, decimals=1)}"
+        return f"{self.name}\n{np.round(self.volumes, decimals=1)}"
 
     def __str__(self) -> None:
         return self.__repr__()
 
 
-def _get_trough_component_names(
-    name: str,
-    columns: int,
-    column_names: typing.Sequence[typing.Union[str, None]],
-    initial_volumes: typing.Sequence[typing.Union[int, float]],
-) -> typing.Dict[str, typing.Union[str, None]]:
-    """Determines a fully-specified component name dictionary for a trough.
-
-    This helper function exists to provide a different default naming pattern for troughs.
-    Instead of "stocks.A01" this function defaults to "stocks.column_01" with 1-based column numbering.
-
-    Parameters
-    ----------
-    name : str
-        Name of the trough - used for default component names.
-    columns : int
-        Number of trough columns.
-    column_names : array-like
-        Column-wise component names.
-        Must be given for all columns, but can contain None elements.
-    initial_volumes : array-like
-        Column-wise initial volumes.
-        Used to determine if a default component name is needed.
-
-    Returns
-    -------
-    component_names : dict
-        The component name dictionary that maps all row A well IDs to component names.
-    """
-    if numpy.shape(column_names) != (columns,):
-        raise ValueError(f"The column names {column_names} don't match the number of columns ({columns}).")
-    if numpy.shape(initial_volumes) != (columns,):
-        raise ValueError(
-            f"The initial volumes {initial_volumes} don't match the number of columns ({columns})."
-        )
-
-    if any([cname is not None and ivol == 0 for cname, ivol in zip(column_names, initial_volumes)]):
-        raise ValueError(
-            f"Empty columns must be unnamed."
-            f"\n\tcolumn_names: {column_names}"
-            f"\n\tinitial_volumes: {initial_volumes}"
-        )
-
-    component_names = {}
-    for c, (cname, ivol) in enumerate(zip(column_names, initial_volumes)):
-        if ivol > 0 and cname is None:
-            # Determine default name
-            if columns > 1:
-                cname = f"{name}.column_{c+1:02d}"
-            else:
-                cname = name
-        component_names[f"A{c+1:02d}"] = cname
-    return component_names
-
-
 class Trough(Labware):
     """Special type of labware that can be accessed by many pipette tips in parallel."""
 
     def __init__(
         self,
         name: str,
         virtual_rows: int,
         columns: int,
         *,
         min_volume: float,
         max_volume: float,
-        initial_volumes: typing.Union[float, numpy.ndarray] = 0,
-        column_names: typing.Optional[typing.Sequence[typing.Union[str, None]]] = None,
+        initial_volumes: Union[float, np.ndarray] = 0,
+        column_names: Optional[Sequence[Union[str, None]]] = None,
     ) -> None:
         """Creates a `Labware` object.
 
         Parameters
         ----------
         name : str
             Label that the labware is identified by.
@@ -568,15 +390,15 @@
         if isinstance(column_names, str):
             column_names = [column_names]
 
         if isinstance(initial_volumes, (int, float)):
             initial_volumes = [initial_volumes] * columns
 
         # Determine component names with a different default pattern compared to Labware
-        component_names = _get_trough_component_names(name, columns, column_names, initial_volumes)
+        component_names = get_trough_component_names(name, columns, column_names, initial_volumes)
 
         super().__init__(
             name=name,
             rows=1,
             columns=columns,
             min_volume=min_volume,
             max_volume=max_volume,
```

### Comparing `robotools-1.5.3/robotools/transform.py` & `robotools-1.6.1/robotools/transform.py`

 * *Files identical despite different names*

### Comparing `robotools-1.5.3/robotools/utils.py` & `robotools-1.6.1/robotools/utils.py`

 * *Files identical despite different names*

### Comparing `robotools-1.5.3/setup.py` & `robotools-1.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,25 +47,28 @@
 __version__ = get_version()
 
 setuptools.setup(
     name=__packagename__,
     packages=setuptools.find_packages(),  # this must be the same as the name above
     version=__version__,
     description="Pythonic in-silico liquid handling and creation of Tecan FreedomEVO worklists.",
+    long_description=open(pathlib.Path(__file__).parent / "README.md").read(),
+    long_description_content_type="text/markdown",
     url="https://github.com/jubiotech/robotools",
     download_url="https://github.com/jubiotech/robotools/tarball/%s" % __version__,
     author="Michael Osthege",
     author_email="m.osthege@fz-juelich.de",
     license="GNU Affero General Public License v3",
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
     ],
     install_requires=[
         "numpy",
         "pandas",
```

