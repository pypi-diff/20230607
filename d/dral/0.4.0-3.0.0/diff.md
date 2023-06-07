# Comparing `tmp/dral-0.4.0.tar.gz` & `tmp/dral-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dral-0.4.0.tar", max compression
+gzip compressed data, was "dral-3.0.0.tar", max compression
```

## Comparing `dral-0.4.0.tar` & `dral-3.0.0.tar`

### file list

```diff
@@ -1,58 +1,46 @@
--rw-r--r--   0        0        0     1065 2023-06-07 19:37:27.581011 dral-0.4.0/LICENSE
--rw-r--r--   0        0        0      656 2023-06-07 19:37:27.581011 dral-0.4.0/README.md
--rw-r--r--   0        0        0      223 2023-06-07 19:37:27.581011 dral-0.4.0/dral/__init__.py
--rw-r--r--   0        0        0      110 2023-06-07 19:37:27.581011 dral-0.4.0/dral/adapter/__init__.py
--rw-r--r--   0        0        0      521 2023-06-07 19:37:27.581011 dral-0.4.0/dral/adapter/base.py
--rw-r--r--   0        0        0     3281 2023-06-07 19:37:27.581011 dral-0.4.0/dral/adapter/svd.py
--rw-r--r--   0        0        0     1858 2023-06-07 19:37:27.581011 dral-0.4.0/dral/adapter/white_black_list.py
--rw-r--r--   0        0        0     5833 2023-06-07 19:37:27.581011 dral-0.4.0/dral/app.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.581011 dral-0.4.0/dral/devices/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.581011 dral-0.4.0/dral/devices/arm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.581011 dral-0.4.0/dral/devices/arm/example/__init__.py
--rw-r--r--   0        0        0    33134 2023-06-07 19:37:27.581011 dral-0.4.0/dral/devices/arm/example/example1.svd
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.581011 dral-0.4.0/dral/devices/stm32/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.581011 dral-0.4.0/dral/devices/stm32/f4/__init__.py
--rw-r--r--   0        0        0   930253 2023-06-07 19:37:27.589012 dral-0.4.0/dral/devices/stm32/f4/stm32f411.svd
--rw-r--r--   0        0        0  1949938 2023-06-07 19:37:27.589012 dral-0.4.0/dral/devices/stm32/f4/stm32f446.svd
--rw-r--r--   0        0        0    33867 2023-06-07 19:37:27.589012 dral-0.4.0/dral/devices/trinamic/tmc22xx/tmc2209.svd
--rw-r--r--   0        0        0      216 2023-06-07 19:37:27.589012 dral-0.4.0/dral/filter/__init__.py
--rw-r--r--   0        0        0     5236 2023-06-07 19:37:27.589012 dral-0.4.0/dral/filter/banks.py
--rw-r--r--   0        0        0      251 2023-06-07 19:37:27.589012 dral-0.4.0/dral/filter/base.py
--rw-r--r--   0        0        0      300 2023-06-07 19:37:27.589012 dral-0.4.0/dral/filter/black_list.py
--rw-r--r--   0        0        0      306 2023-06-07 19:37:27.589012 dral-0.4.0/dral/filter/exclude.py
--rw-r--r--   0        0        0     1386 2023-06-07 19:37:27.589012 dral-0.4.0/dral/filter/white_list.py
--rw-r--r--   0        0        0      191 2023-06-07 19:37:27.589012 dral-0.4.0/dral/format/__init__.py
--rw-r--r--   0        0        0      699 2023-06-07 19:37:27.589012 dral-0.4.0/dral/format/base.py
--rw-r--r--   0        0        0     1848 2023-06-07 19:37:27.589012 dral-0.4.0/dral/format/cmake_lib.py
--rw-r--r--   0        0        0     2313 2023-06-07 19:37:27.589012 dral-0.4.0/dral/format/mbedautomatify.py
--rw-r--r--   0        0        0     1375 2023-06-07 19:37:27.589012 dral-0.4.0/dral/format/single_file.py
--rw-r--r--   0        0        0     1110 2023-06-07 19:37:27.589012 dral-0.4.0/dral/generator.py
--rw-r--r--   0        0        0     9674 2023-06-07 19:37:27.589012 dral-0.4.0/dral/template.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/c/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/__init__.py
--rw-r--r--   0        0        0      455 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/bank.dral
--rw-r--r--   0        0        0      138 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/bank.field.dral
--rw-r--r--   0        0        0      112 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/bitfield.dral
--rw-r--r--   0        0        0      126 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/field.dral
--rw-r--r--   0        0        0     1284 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/header.dral
--rw-r--r--   0        0        0      725 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/peripheral.dral
--rw-r--r--   0        0        0      497 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/mcu/register.dral
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/serial/__init__.py
--rw-r--r--   0        0        0      112 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/serial/bitfield.dral
--rw-r--r--   0        0        0     1284 2023-06-07 19:37:27.589012 dral-0.4.0/dral/templates/cpp/serial/header.dral
--rw-r--r--   0        0        0      514 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/cpp/serial/peripheral.dral
--rw-r--r--   0        0        0      290 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/cpp/serial/register.dral
--rw-r--r--   0        0        0     4454 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/model/cpp.dral
--rw-r--r--   0        0        0     1284 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/model/header.dral
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/python/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/python/mcu/__init__.py
--rw-r--r--   0        0        0      267 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/python/mcu/field.dral
--rw-r--r--   0        0        0      550 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/python/mcu/peripheral.dral
--rw-r--r--   0        0        0      463 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/python/mcu/register.dral
--rw-r--r--   0        0        0      132 2023-06-07 19:37:27.593012 dral-0.4.0/dral/templates/python/mcu/register.simple.dral
--rw-r--r--   0        0        0     5993 2023-06-07 19:37:27.593012 dral-0.4.0/dral/types.py
--rw-r--r--   0        0        0     1692 2023-06-07 19:37:27.593012 dral-0.4.0/dral/utils.py
--rw-r--r--   0        0        0     1742 2023-06-07 19:37:27.593012 dral-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1494 1970-01-01 00:00:00.000000 dral-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-01 18:02:04.626572 dral-3.0.0/LICENSE
+-rw-r--r--   0        0        0      656 2022-10-01 18:02:04.626572 dral-3.0.0/README.md
+-rw-r--r--   0        0        0      126 2022-10-01 18:02:04.626572 dral-3.0.0/dral/__init__.py
+-rw-r--r--   0        0        0      110 2022-10-01 18:02:04.626572 dral-3.0.0/dral/adapter/__init__.py
+-rw-r--r--   0        0        0      485 2022-10-01 18:02:04.626572 dral-3.0.0/dral/adapter/base.py
+-rw-r--r--   0        0        0     3286 2022-10-01 18:02:04.626572 dral-3.0.0/dral/adapter/svd.py
+-rw-r--r--   0        0        0     1804 2022-10-01 18:02:04.626572 dral-3.0.0/dral/adapter/white_black_list.py
+-rw-r--r--   0        0        0     4232 2022-10-01 18:02:04.626572 dral-3.0.0/dral/app.py
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.626572 dral-3.0.0/dral/devices/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.626572 dral-3.0.0/dral/devices/arm/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.626572 dral-3.0.0/dral/devices/arm/example/__init__.py
+-rw-r--r--   0        0        0    33134 2022-10-01 18:02:04.626572 dral-3.0.0/dral/devices/arm/example/example1.svd
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.626572 dral-3.0.0/dral/devices/stm32/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.626572 dral-3.0.0/dral/devices/stm32/f4/__init__.py
+-rw-r--r--   0        0        0   930253 2022-10-01 18:02:04.630572 dral-3.0.0/dral/devices/stm32/f4/stm32f411.svd
+-rw-r--r--   0        0        0  1949205 2022-10-01 18:02:04.634572 dral-3.0.0/dral/devices/stm32/f4/stm32f446.svd
+-rw-r--r--   0        0        0      164 2022-10-01 18:02:04.634572 dral-3.0.0/dral/filter/__init__.py
+-rw-r--r--   0        0        0     5195 2022-10-01 18:02:04.634572 dral-3.0.0/dral/filter/banks.py
+-rw-r--r--   0        0        0      215 2022-10-01 18:02:04.634572 dral-3.0.0/dral/filter/base.py
+-rw-r--r--   0        0        0      264 2022-10-01 18:02:04.634572 dral-3.0.0/dral/filter/black_list.py
+-rw-r--r--   0        0        0     1399 2022-10-01 18:02:04.634572 dral-3.0.0/dral/filter/white_list.py
+-rw-r--r--   0        0        0      191 2022-10-01 18:02:04.634572 dral-3.0.0/dral/format/__init__.py
+-rw-r--r--   0        0        0      533 2022-10-01 18:02:04.634572 dral-3.0.0/dral/format/base.py
+-rw-r--r--   0        0        0     1534 2022-10-01 18:02:04.634572 dral-3.0.0/dral/format/cmake_lib.py
+-rw-r--r--   0        0        0     2212 2022-10-01 18:02:04.634572 dral-3.0.0/dral/format/mbedautomatify.py
+-rw-r--r--   0        0        0     1317 2022-10-01 18:02:04.634572 dral-3.0.0/dral/format/single_file.py
+-rw-r--r--   0        0        0      938 2022-10-01 18:02:04.634572 dral-3.0.0/dral/generator.py
+-rw-r--r--   0        0        0    12348 2022-10-01 18:02:04.634572 dral-3.0.0/dral/objects.py
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/__init__.py
+-rw-r--r--   0        0        0      369 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/bank.dral
+-rw-r--r--   0        0        0      129 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/bank.field.dral
+-rw-r--r--   0        0        0      117 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/field.dral
+-rw-r--r--   0        0        0     3009 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/model.dral
+-rw-r--r--   0        0        0      558 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/peripheral.dral
+-rw-r--r--   0        0        0      314 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/dral/register.dral
+-rw-r--r--   0        0        0        0 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/mbedAutomatify/__init__.py
+-rw-r--r--   0        0        0      226 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/mbedAutomatify/field.dral
+-rw-r--r--   0        0        0      458 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/mbedAutomatify/peripheral.dral
+-rw-r--r--   0        0        0      383 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/mbedAutomatify/register.dral
+-rw-r--r--   0        0        0      116 2022-10-01 18:02:04.634572 dral-3.0.0/dral/templates/mbedAutomatify/register.simple.dral
+-rw-r--r--   0        0        0     8159 2022-10-01 18:02:04.634572 dral-3.0.0/dral/types.py
+-rw-r--r--   0        0        0      988 2022-10-01 18:02:04.634572 dral-3.0.0/dral/utils.py
+-rw-r--r--   0        0        0     1646 2022-10-01 18:02:04.638572 dral-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 dral-3.0.0/setup.py
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dral-3.0.0/PKG-INFO
```

### Comparing `dral-0.4.0/LICENSE` & `dral-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dral-0.4.0/README.md` & `dral-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dral-0.4.0/dral/adapter/svd.py` & `dral-3.0.0/dral/adapter/svd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import re
 from pathlib import Path
 from typing import Any, Dict, List
 
 import svd2py
 
 from ..types import Device, Field, Peripheral, Register
@@ -33,14 +31,15 @@
             else:
                 position = field["bitOffset"]
                 width = field["bitWidth"]
             new_field = Field(
                 name=field["name"],
                 description=field["description"],
                 position=position,
+                mask=((1 << width) - 1),
                 width=width,
             )
             fields_list.append(new_field)
         return fields_list
 
     def _get_registers(self, svd_registers: List[Dict[str, Any]]) -> List[Register]:
         registers_list = []
```

### Comparing `dral-0.4.0/dral/adapter/white_black_list.py` & `dral-3.0.0/dral/adapter/white_black_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from pathlib import Path
 from typing import Any, Dict, List
 
 import yaml
 
 from ..types import Device, Field, Peripheral, Register
 from .base import BaseAdapter
@@ -37,13 +35,13 @@
             new_peripheral = Peripheral(**peripheral)
             peripherals_list.append(new_peripheral)
         return peripherals_list
 
     def _list_to_dral(self, _list: Dict[str, Any]) -> Device:
         if "peripherals" in _list:
             _list.update({"peripherals": self._get_peripherals(_list["peripherals"])})
-        return Device(name="WhiteList", **_list)
+        return Device(**_list)
 
     def convert(self) -> Device:
         with open(self._list_file, "r", encoding="UTF-8") as list_file:
             _list = yaml.load(list_file, Loader=yaml.FullLoader)
         return self._list_to_dral(_list)
```

### Comparing `dral-0.4.0/dral/app.py` & `dral-3.0.0/dral/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-from __future__ import annotations
-
-import glob
 from pathlib import Path
 from typing import Any
 
 import click
-import yaml
 from rich.console import Console
 from rich.traceback import install as traceback
 
 from .adapter.svd import SvdAdapter
 from .adapter.white_black_list import WhiteBlackListAdapter
-from .filter import BanksFilter, BlackListFilter, ExcludeFilter, WhiteListFilter
+from .filter import BanksFilter, BlackListFilter, WhiteListFilter
 from .format import CMakeLibFormat, MbedAutomatifyFormat
-from .generator import DralGenerator, DralOutputFile
-from .template import DralTemplate
+from .generator import Generator
 from .utils import Utils
 
 
 def print_supported_devices(ctx: Any, param: Any, value: Any) -> None:
     del param
     if not value or ctx.resilient_parsing:
         return
-    devices_path = Path(__file__).parent / "devices"
-    svd = glob.glob(f"{devices_path}/**/*.svd", recursive=True)
-    svd.sort()
-    for device in svd:
-        chip, family, brand = Utils.get_device_info(Path(device))
-        click.echo(f"{brand}::{family}::{chip}")
+    click.echo("TODO")
     ctx.exit()
 
 
 def validate_svd(ctx: Any, param: Any, value: Any) -> Any:
     del ctx, param
     if Path(value).exists():
         return Path(value).resolve()
@@ -41,32 +31,20 @@
     raise click.BadParameter("SVD must be a path to external SVD file or name of the already supported device")
 
 
 @click.command()
 @click.argument("svd", type=click.UNPROCESSED, callback=validate_svd)
 @click.argument("output", type=click.Path(resolve_path=True, path_type=Path))
 @click.option(
-    "-l",
-    "--language",
-    default="cpp",
-    show_default=True,
-    type=click.Choice(["c", "cpp", "python"], case_sensitive=False),
-    help="Specify the programming language for which you want to generate files.",
-)
-@click.option(
     "-t",
     "--template",
-    type=click.Path(exists=True, resolve_path=True, path_type=Path),
-    help="Specify path to template files used to generate files.",
-)
-@click.option(
-    "-m",
-    "--mapping",
-    type=click.Path(exists=True, resolve_path=True, path_type=Path),
-    help="Specify mapping file to overwrite values with constants.",
+    default="dral",
+    show_default=True,
+    type=click.Choice(["dral", "mbedAutomatify"], case_sensitive=False),
+    help="Specify template used to generate files.",
 )
 @click.option(
     "-e",
     "--exclude",
     multiple=True,
     type=click.Choice(["peripherals", "registers", "banks", "fields"], case_sensitive=False),
     help="Exclude items from generation.",
@@ -89,15 +67,15 @@
     is_flag=True,
     is_eager=True,
     expose_value=False,
     callback=print_supported_devices,
     help="Show list of the supported devices and exit.",
 )
 @click.version_option()
-def cli(svd, output, language, template, mapping, exclude, single, white_list, black_list):  # type: ignore[no-untyped-def] # noqa: C901
+def cli(svd, output, template, exclude, single, white_list, black_list):  # type: ignore[no-untyped-def]
     """D-RAL - Device Register Access Layer
 
     Generate D-RAL files in the OUTPUT from SVD.
 
     \b
     SVD    - can be a path to external SVD file or name of the already supported device.
              Type 'dral --list' to see all supported devices.
@@ -117,63 +95,44 @@
     if black_list:
         black_list_adapter = WhiteBlackListAdapter(black_list)
         black_list = black_list_adapter.convert()
     else:
         black_list = None
 
     exclude = exclude if exclude else []
-
-    if template:
-        template_dir = template
-    else:
-        template = Utils.get_device_template(svd)
-        template_dir = Utils.get_template_dir(language, template)
-    template_object = DralTemplate(template_dir)
-
-    if mapping:
-        with open(mapping, "r", encoding="utf-8") as mapping_file:
-            mapping = yaml.load(mapping_file, Loader=yaml.FullLoader)
+    adapter = SvdAdapter(svd)
+    generator = Generator(template)
 
     info = "[bold green]Generating D-Ral files..."
     with console.status(info):
         # Convert data using adapter
-        adapter = SvdAdapter(svd)
         device = adapter.convert()
 
         # Apply filters
         filters: Any = []
         if black_list is not None:
             filters.append(BlackListFilter(black_list))
         if white_list is not None:
             filters.append(WhiteListFilter(white_list))
         filters.append(BanksFilter())
-        if exclude:
-            filters.append(ExcludeFilter(exclude))
         for item in filters:
             device = item.apply(device)
 
         # Generate D-RAL data
-        generator = DralGenerator(template_object)
-        objects = generator.generate(device, mapping=mapping)
-
-        # Get D-RAL register model file
-        model_dir = Utils.get_model_dir()
-        model_template = DralTemplate(model_dir)
-        model_content = model_template.parse_from_template(f"{language}.dral", mapping={})
-        dral_model_file = DralOutputFile("register_model", "".join(model_content))
+        objects = generator.generate(device, exclude=exclude)
 
         # Make output
         output = output / "dralOutput"
 
-        chip, family, brand = Utils.get_device_info(svd)
-        output_format: Any = CMakeLibFormat(output, "dral", chip)
-        if language == "cpp":
-            output_format = CMakeLibFormat(output, "dral", chip)
-        elif language == "python":
+        output_format: Any = CMakeLibFormat(output, "dral")
+        if template == "dral":
+            output_format = CMakeLibFormat(output, "dral")
+        elif template == "mbedAutomatify":
+            chip, family, brand = Utils.get_device_info(svd)
             output_format = MbedAutomatifyFormat(output, chip, family, brand)
-        output_format.make(objects, model=dral_model_file, single=single)
+        output_format.make(objects, single)
 
     console.print(f"Successfully generated D-Ral files to {output}", style="green")
 
 
 if __name__ == "__main__":
     cli()  # noqa
```

### Comparing `dral-0.4.0/dral/devices/arm/example/example1.svd` & `dral-3.0.0/dral/devices/arm/example/example1.svd`

 * *Files identical despite different names*

### Comparing `dral-0.4.0/dral/devices/stm32/f4/stm32f411.svd` & `dral-3.0.0/dral/devices/stm32/f4/stm32f411.svd`

 * *Files identical despite different names*

### Comparing `dral-0.4.0/dral/devices/stm32/f4/stm32f446.svd` & `dral-3.0.0/dral/devices/stm32/f4/stm32f446.svd`

 * *Files 0% similar despite different names*

#### Comparing `dral-0.4.0/dral/devices/stm32/f4/stm32f446.svd` & `dral-3.0.0/dral/devices/stm32/f4/stm32f446.svd`

```diff
@@ -18941,15 +18941,15 @@
               accesses</description>
               <bitOffset>0</bitOffset>
               <bitWidth>16</bitWidth>
             </field>
           </fields>
         </register>
         <register>
-          <name>_OR</name>
+          <name>OR</name>
           <displayName>OR</displayName>
           <description>TIM5 option register</description>
           <addressOffset>0x50</addressOffset>
           <size>0x20</size>
           <access>read-write</access>
           <resetValue>0x0000</resetValue>
           <fields>
@@ -20815,15 +20815,15 @@
               accesses</description>
               <bitOffset>0</bitOffset>
               <bitWidth>16</bitWidth>
             </field>
           </fields>
         </register>
         <register>
-          <name>_OR</name>
+          <name>OR</name>
           <displayName>OR</displayName>
           <description>TIM5 option register</description>
           <addressOffset>0x50</addressOffset>
           <size>0x20</size>
           <access>read-write</access>
           <resetValue>0x0000</resetValue>
           <fields>
@@ -22265,35 +22265,14 @@
               <name>SRQ</name>
               <description>Session request</description>
               <bitOffset>1</bitOffset>
               <bitWidth>1</bitWidth>
               <access>read-write</access>
             </field>
             <field>
-              <name>AVALOEN</name>
-              <description>AVALOEN</description>
-              <bitOffset>4</bitOffset>
-              <bitWidth>1</bitWidth>
-              <access>read-write</access>
-            </field>
-            <field>
-              <name>BVALOEN</name>
-              <description>BVALOEN</description>
-              <bitOffset>6</bitOffset>
-              <bitWidth>1</bitWidth>
-              <access>read-write</access>
-            </field>
-            <field>
-              <name>BVALOVAL</name>
-              <description>BVALOVAL</description>
-              <bitOffset>7</bitOffset>
-              <bitWidth>1</bitWidth>
-              <access>read-write</access>
-            </field>
-            <field>
               <name>HNGSCS</name>
               <description>Host negotiation success</description>
               <bitOffset>8</bitOffset>
               <bitWidth>1</bitWidth>
               <access>read-only</access>
             </field>
             <field>
```

### Comparing `dral-0.4.0/dral/filter/banks.py` & `dral-3.0.0/dral/filter/banks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import sys
 from typing import Any, List, Tuple
 
 from rich.console import Console
 
 from ..types import Bank, Device, Register
 from .base import BaseFilter
@@ -81,15 +79,15 @@
         if len(set(diff)) != 1:
             console = Console()
             console.print(f"[red]ERROR: Register banks offset not consistent: {offsets}")
             console.print("Registers dump:")
             console.print(registers)
             sys.exit()
         min_offset = min(offsets)  # type: ignore[type-var]
-        return min_offset, abs(diff[0])
+        return min_offset, diff[0]
 
     def _get_register_bank_name(self, bank: List[Register]) -> str:
         from difflib import SequenceMatcher
 
         differ = SequenceMatcher(None, bank[0].name, bank[1].name)
         replace = differ.get_opcodes()[1]
         if replace[0] == "replace":
```

### Comparing `dral-0.4.0/dral/format/cmake_lib.py` & `dral-3.0.0/dral/format/cmake_lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from __future__ import annotations
-
 from pathlib import Path
-from typing import List, Optional
+from typing import Dict, List
 
-from ..generator import DralOutputFile
 from .base import BaseFormat
 
 
 class CMakeLibFormat(BaseFormat):
-    def __init__(self, directory: Path, name: str, chip: str):
+    def __init__(self, directory: Path, name: str):
         self._directory = directory
         self._name = name
-        self._chip = chip
         self._cmake_content = (
             f"add_library({self._name} INTERFACE)\n"
             f"\n"
             f"target_include_directories({self._name}\n"
             f"  INTERFACE\n"
             f"    ${{CMAKE_CURRENT_SOURCE_DIR}}/inc\n"
             f")"
@@ -23,25 +19,23 @@
 
     def _create_file(self, name: str, directory: Path, content: str) -> None:
         file_path = directory / name
         with open(file_path, "w", encoding="UTF-8") as new_file:
             new_file.writelines(content)
 
     def _create_output_directory(self, output: Path) -> Path:
-        directory_path = output / f"{self._name}/inc/{self._name}" / self._chip
+        directory_path = output / f"{self._name}/inc/{self._name}"
         Path.mkdir(directory_path, parents=True, exist_ok=True)
         return directory_path
 
-    def _make_default(self, objects: List[DralOutputFile], model: Optional[DralOutputFile] = None) -> None:
+    def _make_default(self, objects: List[Dict[str, str]]) -> None:
         directory = self._create_output_directory(self._directory)
         for item in objects:
-            self._create_file(f"{item.name.lower()}.h", directory, item.content)
+            self._create_file("%s.h" % item["name"].lower(), directory, item["content"])
         self._create_file("CMakeLists.txt", self._directory / self._name, self._cmake_content)
-        if model is not None:
-            self._create_file(f"{model.name.lower()}.h", self._directory / self._name / "inc" / self._name, model.content)
 
-    def _make_single(self, objects: List[DralOutputFile]) -> None:
+    def _make_single(self, objects: List[Dict[str, str]]) -> None:
         # TODO refactor
         from .single_file import SingleFileFormat
 
         single = SingleFileFormat(self._directory, "dral.h")
         single.make(objects)
```

### Comparing `dral-0.4.0/dral/format/mbedautomatify.py` & `dral-3.0.0/dral/format/mbedautomatify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from __future__ import annotations
-
 from pathlib import Path
-from typing import List, Optional
+from typing import Dict, List
 
-from ..generator import DralOutputFile
 from .base import BaseFormat
 
 
 class MbedAutomatifyFormat(BaseFormat):
     def __init__(self, directory: Path, device: str, family: str, brand: str):
         self._directory = directory
         self._device = device
@@ -21,34 +18,34 @@
             new_file.writelines(content)
 
     def _create_output_directory(self, output: Path) -> Path:
         directory_path = output / f"{self._brand}" / f"{self._family}" / f"{self._device}"
         directory_path.mkdir(parents=True, exist_ok=True)
         return directory_path
 
-    def _create_device_file(self, name: str, directory: Path, objects: List[DralOutputFile]) -> None:
+    def _create_device_file(self, name: str, directory: Path, objects: List[Dict[str, str]]) -> None:
         content = ""
         for item in objects:
-            content += f"from .{item.name.lower()} import {item.name.capitalize()}\n"
+            content += f"from .{item['name'].lower()} import {item['name'].capitalize()}\n"
         content += "\n" * 2
         content += self._device_file_content
         for item in objects:
-            content += f"{' ' * 8}self.{item.name.lower()} = {item.name.capitalize()}(proxy)\n"
+            content += f"{' ' * 8}self.{item['name'].lower()} = {item['name'].capitalize()}(proxy)\n"
         self._create_file(name, directory, content)
 
     def _create_init_files(self, directory: Path) -> None:
         with open(directory / "__init__.py", "w", encoding="UTF-8") as init:
             init.write("from .dral import dral")
         directory = directory.parent
         while directory != self._directory:
             open(directory / "__init__.py", "w", encoding="UTF-8").close()
             directory = directory.parent
 
-    def _make_default(self, objects: List[DralOutputFile], model: Optional[DralOutputFile] = None) -> None:
+    def _make_default(self, objects: List[Dict[str, str]]) -> None:
         directory = self._create_output_directory(self._directory)
         for item in objects:
-            self._create_file("%s.py" % item.name.lower(), directory, item.content)
+            self._create_file("%s.py" % item["name"].lower(), directory, item["content"])
         self._create_device_file("dral.py", directory, objects)
         self._create_init_files(directory)
 
-    def _make_single(self, objects: List[DralOutputFile]) -> None:
+    def _make_single(self, objects: List[Dict[str, str]]) -> None:
         pass
```

### Comparing `dral-0.4.0/dral/format/single_file.py` & `dral-3.0.0/dral/format/single_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from __future__ import annotations
-
 from pathlib import Path
-from typing import List
-
-from ..generator import DralOutputFile
+from typing import Dict, List
 
 
 class SingleFileFormat:
     def __init__(self, directory: Path, name: str, includeRegModel: bool = False):
         self._directory = directory
         self._name = name
         self._includeRegModel = includeRegModel
@@ -17,20 +13,20 @@
         with open(file_path, "w", encoding="UTF-8") as new_file:
             new_file.writelines(content)
 
     def _create_output_directory(self, output: Path) -> Path:
         output.mkdir(parents=True, exist_ok=True)
         return self._directory
 
-    def make(self, objects: List[DralOutputFile]) -> None:
+    def make(self, objects: List[Dict[str, str]]) -> None:
         directory = self._create_output_directory(self._directory)
         file_path = self._directory / f"{self._name}"
         self._create_file(file_path.name, directory, "")
 
         for i, item in enumerate(objects):
-            if item.name == "register_model" and not self._includeRegModel:
-                self._create_file(f"{item.name.lower()}.h", directory, item.content)
+            if item["name"] == "register_model" and not self._includeRegModel:
+                self._create_file(f"{item['name'].lower()}.h", directory, item["content"])
             else:
                 with open(file_path, "a", encoding="UTF-8") as new_file:
                     if i > 0:
                         new_file.write("\n\n")
-                    new_file.writelines(item.content)
+                    new_file.writelines(item["content"])
```

### Comparing `dral-0.4.0/pyproject.toml` & `dral-3.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "dral"
 homepage = "https://github.com/gembcior/d-ral"
-version = "0.4.0"
+version = "3.0.0"
 description = "D-RAL - Device Register Access Layer"
 authors = ["Gembcior <gembcior@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
 ]
 packages = [{ include = "dral" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 svd2py = "^0.1"
 rich = "^12.5"
 click = "^8.1"
-pyyaml = "^6.0"
 pylama = { extras = ["all"], version = "^8.4.1" }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-sugar = "^0.9.5"
 pytest-cov = "^3.0.0"
 pytest-clarity = "^1.0.1"
@@ -43,15 +41,14 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 files = ["dral"]
 show_error_codes = true
 strict = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
-disable_error_code = ["union-attr"]
 
 [[tool.mypy.overrides]]
 module = ["rich.*", "click.*", "svd2py.*"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `dral-0.4.0/PKG-INFO` & `dral-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: dral
-Version: 0.4.0
+Version: 3.0.0
 Summary: D-RAL - Device Register Access Layer
 Home-page: https://github.com/gembcior/d-ral
 License: MIT
 Author: Gembcior
 Author-email: gembcior@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: pylama[all] (>=8.4.1,<9.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=12.5,<13.0)
 Requires-Dist: svd2py (>=0.1,<0.2)
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/gembcior/d-ral/main/doc/logo.svg)
 
 <h1 align="center">D-RAL - Device Register Access Layer</h1>
```

