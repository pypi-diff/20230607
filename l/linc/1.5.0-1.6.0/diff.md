# Comparing `tmp/linc-1.5.0.tar.gz` & `tmp/linc-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linc-1.5.0.tar", max compression
+gzip compressed data, was "linc-1.6.0.tar", max compression
```

## Comparing `linc-1.5.0.tar` & `linc-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      136 2023-02-20 02:18:41.067533 linc-1.5.0/README.md
--rw-r--r--   0        0        0      316 2023-02-22 15:13:25.251690 linc-1.5.0/linc/__init__.py
--rw-r--r--   0        0        0     1065 2023-02-15 15:29:59.756081 linc-1.5.0/linc/cli.py
--rw-r--r--   0        0        0       92 2023-02-15 15:29:59.756081 linc-1.5.0/linc/config/__init__.py
--rw-r--r--   0        0        0       34 2023-02-15 17:30:56.063904 linc-1.5.0/linc/config/default-config.toml
--rw-r--r--   0        0        0     1188 2023-04-11 02:58:40.653993 linc-1.5.0/linc/config/models.py
--rw-r--r--   0        0        0      931 2023-02-16 02:55:41.005378 linc-1.5.0/linc/config/read.py
--rw-r--r--   0        0        0     3037 2023-04-10 00:00:05.393895 linc-1.5.0/linc/convertion.py
--rw-r--r--   0        0        0     2727 2023-02-19 01:05:47.201474 linc-1.5.0/linc/models.py
--rw-r--r--   0        0        0       77 2023-02-15 15:29:59.756081 linc-1.5.0/linc/parse/__init__.py
--rw-r--r--   0        0        0       41 2023-02-18 22:47:13.181551 linc-1.5.0/linc/parse/constants.py
--rw-r--r--   0        0        0      983 2023-02-16 21:11:51.157824 linc-1.5.0/linc/parse/dataset.py
--rw-r--r--   0        0        0      247 2023-02-15 15:29:59.756081 linc-1.5.0/linc/parse/file.py
--rw-r--r--   0        0        0     2767 2023-02-15 15:29:59.756081 linc-1.5.0/linc/parse/header.py
--rw-r--r--   0        0        0      344 2023-02-19 00:12:32.110253 linc-1.5.0/linc/parse/utils.py
--rw-r--r--   0        0        0     1762 2023-04-09 23:59:51.673896 linc-1.5.0/linc/reader.py
--rw-r--r--   0        0        0     1413 2023-04-15 01:59:49.664279 linc-1.5.0/linc/utils.py
--rw-r--r--   0        0        0     1293 2023-02-18 17:19:25.786396 linc-1.5.0/linc/write/common.py
--rw-r--r--   0        0        0     6044 2023-04-11 15:37:40.743083 linc-1.5.0/linc/write/writer_nc.py
--rw-r--r--   0        0        0      629 2023-04-11 15:36:38.533097 linc-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 linc-1.5.0/setup.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 linc-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-06-07 01:03:22.218726 linc-1.6.0/linc/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-07 01:03:22.218726 linc-1.6.0/linc/cli.py
+-rw-r--r--   0        0        0       96 2023-06-07 01:03:22.232840 linc-1.6.0/linc/config/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-07 01:03:22.232840 linc-1.6.0/linc/config/default-config.toml
+-rw-r--r--   0        0        0     1276 2023-06-07 13:28:15.945042 linc-1.6.0/linc/config/models.py
+-rw-r--r--   0        0        0      967 2023-06-07 01:03:22.232840 linc-1.6.0/linc/config/read.py
+-rw-r--r--   0        0        0     3183 2023-06-07 13:34:35.874796 linc-1.6.0/linc/convertion.py
+-rw-r--r--   0        0        0     2846 2023-06-07 01:03:22.234945 linc-1.6.0/linc/models.py
+-rw-r--r--   0        0        0       80 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/constants.py
+-rw-r--r--   0        0        0     1016 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/dataset.py
+-rw-r--r--   0        0        0      256 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/file.py
+-rw-r--r--   0        0        0     2860 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/header.py
+-rw-r--r--   0        0        0      355 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/utils.py
+-rw-r--r--   0        0        0     1810 2023-06-07 13:25:10.157503 linc-1.6.0/linc/reader.py
+-rw-r--r--   0        0        0     1468 2023-06-07 01:03:22.236254 linc-1.6.0/linc/utils.py
+-rw-r--r--   0        0        0     1332 2023-06-07 01:03:22.239644 linc-1.6.0/linc/write/common.py
+-rw-r--r--   0        0        0     6259 2023-06-07 01:03:22.239644 linc-1.6.0/linc/write/writer_nc.py
+-rw-r--r--   0        0        0      659 2023-06-07 13:38:53.822694 linc-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-06-07 01:03:22.218726 linc-1.6.0/README.md
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 linc-1.6.0/PKG-INFO
```

### Comparing `linc-1.5.0/linc/config/models.py` & `linc-1.6.0/linc/config/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-from typing import Any
-
-from pydantic import BaseModel, Field
-
-
-DEFAULT_ATTRS: dict[str, Any] = {"generated_by": "linc-python"}
-
-class OptionalVariable(BaseModel):
-    name: str
-    type: str
-
-class Options(BaseModel):
-    channel_not_present_all_ok: bool = False
-    time_lidar_variables: list[OptionalVariable] = []
-    time_channel_variables: list[OptionalVariable] = []
-
-class LidarChannel(BaseModel):
-    name: str
-    link_to: str # The device ID
-
-
-class LidarConfig(BaseModel):
-    bin_width: float 
-    bin_count: int
-    attrs: dict[str, Any] = DEFAULT_ATTRS
-    channels: list[LidarChannel] = Field(default_factory=list)
-
-
-class Config(BaseModel):
-    lidar: LidarConfig = Field()
-    options: Options = Field()
-
-
-"""
-DEFAULT_CONFIG: Config = {
-    "lidar": {
-        "attrs": {"converter": "linc"},
-        "channels": [
-            # {"wavelength": 532, "link_to": "BT0"},
-            # {"wavelength": 532, "link_to": "S2A0"},
-            # {"wavelength": 532, "link_to": "BT1"},
-            # {"wavelength": 532, "link_to": "S2A1"},
-        ],
-    },
-    "config": {
-        "include_undefined_channels": True,
-        "default_channel_name_format": r"%wx%p%a",
-    },
-}
-"""
+from typing import Any
+
+from pydantic import BaseModel, Field
+
+
+DEFAULT_ATTRS: dict[str, Any] = {"generated_by": "linc-python"}
+
+class OptionalVariable(BaseModel):
+    name: str
+    type: str
+
+class Options(BaseModel):
+    channel_not_present_all_ok: bool = False
+    time_lidar_variables: list[OptionalVariable] = []
+    time_channel_variables: list[OptionalVariable] = []
+
+class LidarChannel(BaseModel):
+    name: str
+    link_to: str # The device ID
+
+
+class LidarConfig(BaseModel):
+    bin_width: float 
+    bin_count: int
+    bins_per_microsecond: float = 20
+    attrs: dict[str, Any] = DEFAULT_ATTRS
+    channels: list[LidarChannel] = Field(default_factory=list)
+
+
+class Config(BaseModel):
+    lidar: LidarConfig = Field()
+    options: Options = Field()
+
+
+"""
+DEFAULT_CONFIG: Config = {
+    "lidar": {
+        "attrs": {"converter": "linc"},
+        "channels": [
+            # {"wavelength": 532, "link_to": "BT0"},
+            # {"wavelength": 532, "link_to": "S2A0"},
+            # {"wavelength": 532, "link_to": "BT1"},
+            # {"wavelength": 532, "link_to": "S2A1"},
+        ],
+    },
+    "config": {
+        "include_undefined_channels": True,
+        "default_channel_name_format": r"%wx%p%a",
+    },
+}
+"""
```

### Comparing `linc-1.5.0/linc/config/read.py` & `linc-1.6.0/linc/config/read.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from functools import lru_cache
-from pathlib import Path
-
-from pydantic import BaseModel
-
-from tomli import load
-from .models import Config
-
-FALLBACK_CONFIG = Path(__file__).parent / "default-config.toml"
-CURRENT_DIR_CONFIG = Path("./lidar-conf.toml")
-
-
-@lru_cache
-def get_config(file: Path | str | None = None, use_default: bool = False) -> Config:
-
-    if file is not None:
-        _cf = Path(file)
-        if _cf.exists():
-            config_path = _cf
-        elif CURRENT_DIR_CONFIG.exists():
-            config_path = CURRENT_DIR_CONFIG
-        else:
-            if use_default:
-                config_path = FALLBACK_CONFIG
-            else:
-                raise FileNotFoundError()
-    else:
-        if use_default:
-                config_path = FALLBACK_CONFIG
-        else:
-            raise FileNotFoundError()
-
-    with open(config_path, "rb") as f:
-        settings_dict = load(f)
-
-    return Config(**settings_dict)
+from functools import lru_cache
+from pathlib import Path
+
+from pydantic import BaseModel
+
+from tomli import load
+from .models import Config
+
+FALLBACK_CONFIG = Path(__file__).parent / "default-config.toml"
+CURRENT_DIR_CONFIG = Path("./lidar-conf.toml")
+
+
+@lru_cache
+def get_config(file: Path | str | None = None, use_default: bool = False) -> Config:
+
+    if file is not None:
+        _cf = Path(file)
+        if _cf.exists():
+            config_path = _cf
+        elif CURRENT_DIR_CONFIG.exists():
+            config_path = CURRENT_DIR_CONFIG
+        else:
+            if use_default:
+                config_path = FALLBACK_CONFIG
+            else:
+                raise FileNotFoundError()
+    else:
+        if use_default:
+                config_path = FALLBACK_CONFIG
+        else:
+            raise FileNotFoundError()
+
+    with open(config_path, "rb") as f:
+        settings_dict = load(f)
+
+    return Config(**settings_dict)
```

### Comparing `linc-1.5.0/linc/convertion.py` & `linc-1.6.0/linc/convertion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-import numpy as np
-import pandas as pd
-
-
-from .models import Channel, DataFile, DataFileU32, MeasurementTypeEnum
-from .utils import device_id_to_str
-
-SQUARED_CHANNELS = [
-    MeasurementTypeEnum.ANALOG_SQUARED,
-    MeasurementTypeEnum.PHOTONCOUNTING_SQUARED,
-]
-
-
-def convert_to_physical_units(data_file: DataFileU32) -> DataFile:
-    final_dataset = data_file.dataset.copy()
-
-    squared_channels = list(
-        filter(
-            lambda c: c.device_id.type in SQUARED_CHANNELS,
-            data_file.header.channels,
-        )
-    )
-
-    measurement_channels = list(
-        filter(
-            lambda c: c.device_id.type not in SQUARED_CHANNELS,
-            data_file.header.channels,
-        )
-    )
-
-    # First iterate over normal channels
-    for channel in measurement_channels:
-        channel_str = device_id_to_str(channel.device_id)
-        final_dataset[channel_str] = _to_physical(channel, final_dataset[channel_str])
-
-    for channel in squared_channels:
-        channel_str = device_id_to_str(channel.device_id)
-        final_dataset[channel_str] = _to_standard_deviation(
-            channel,
-            final_dataset[channel_str],
-            # data_file.dataset[measurement_dataset_idx].astype(np.float64),
-        )
-
-    return DataFile(header=data_file.header, dataset=final_dataset)
-
-
-def _to_physical(channel: Channel, dataset: pd.Series) -> pd.Series:
-    match channel.device_id.type:
-        case MeasurementTypeEnum.ANALOG:
-            _d = (1000 * dataset * channel.dc_dr) / (
-                channel.shots * (2**channel.adc_bits - 1)
-            )
-        case MeasurementTypeEnum.PHOTONCOUNTING:
-            _d = (dataset) / (
-                channel.shots
-                * 1e6
-                * channel.binwidth  # Microseconds conversion output in MHz
-            )
-        case MeasurementTypeEnum.POWERMETER:
-            _d = dataset / channel.shots  # Just apply normalization
-        case MeasurementTypeEnum.POWERMETER_PHOTODIODE:
-            _d = dataset / channel.shots  # Just apply normalization
-        case default:
-            # _d = (dataset) / (channel.shots * (2**channel.adc_bits - 1))
-            raise ValueError(f"Channel not handled: {default}")
-    return _d
-
-
-def _to_standard_deviation(
-    channel: Channel,
-    dataset: pd.Series,
-    # measurement_dataset: npt.NDArray[np.float64],
-) -> pd.Series:
-    match channel.device_id.type:
-        case MeasurementTypeEnum.ANALOG_SQUARED:
-            _s = (
-                (1000 * dataset * channel.dc_dr)
-                / (channel.shots * (2**channel.adc_bits - 1))
-                / np.sqrt(channel.shots - 1)
-            )
-        case MeasurementTypeEnum.PHOTONCOUNTING_SQUARED:
-            _s = (
-                (1000 * dataset * channel.dc_dr)
-                / (channel.shots * (2**channel.adc_bits - 1))
-                / np.sqrt(channel.shots)
-            )
-        case default:
-            raise ValueError(f"Channel not handled: {default}")
-
-    _s[channel.bins:] = np.nan # Remove other non-square-mean
-
-    return _s
+import numpy as np
+import pandas as pd
+
+
+from .models import Channel, DataFile, DataFileU32, MeasurementTypeEnum
+from .utils import device_id_to_str
+from .config import Config
+
+SQUARED_CHANNELS = [
+    MeasurementTypeEnum.ANALOG_SQUARED,
+    MeasurementTypeEnum.PHOTONCOUNTING_SQUARED,
+]
+
+
+def convert_to_physical_units(data_file: DataFileU32, config: Config) -> DataFile:
+    final_dataset = data_file.dataset.copy()
+
+    squared_channels = list(
+        filter(
+            lambda c: c.device_id.type in SQUARED_CHANNELS,
+            data_file.header.channels,
+        )
+    )
+
+    measurement_channels = list(
+        filter(
+            lambda c: c.device_id.type not in SQUARED_CHANNELS,
+            data_file.header.channels,
+        )
+    )
+
+    # First iterate over normal channels
+    for channel in measurement_channels:
+        channel_str = device_id_to_str(channel.device_id)
+        final_dataset[channel_str] = _to_physical(channel, final_dataset[channel_str], config = config)
+
+    for channel in squared_channels:
+        channel_str = device_id_to_str(channel.device_id)
+        final_dataset[channel_str] = _to_standard_deviation(
+            channel,
+            final_dataset[channel_str],
+            # data_file.dataset[measurement_dataset_idx].astype(np.float64),
+        )
+
+    return DataFile(header=data_file.header, dataset=final_dataset)
+
+
+def _to_physical(channel: Channel, dataset: pd.Series, config: Config) -> pd.Series:
+    match channel.device_id.type:
+        case MeasurementTypeEnum.ANALOG:
+            _d = (1000 * dataset * channel.dc_dr) / (
+                channel.shots * (2**channel.adc_bits - 1)
+            )
+        case MeasurementTypeEnum.PHOTONCOUNTING:
+            _d = (dataset * config.lidar.bins_per_microsecond) / (
+                channel.shots  # Microseconds conversion output in MHz
+            )
+        case MeasurementTypeEnum.POWERMETER:
+            _d = dataset / channel.shots  # Just apply normalization
+        case MeasurementTypeEnum.POWERMETER_PHOTODIODE:
+            _d = dataset / channel.shots  # Just apply normalization
+        case default:
+            # _d = (dataset) / (channel.shots * (2**channel.adc_bits - 1))
+            raise ValueError(f"Channel not handled: {default}")
+    return _d
+
+
+def _to_standard_deviation(
+    channel: Channel,
+    dataset: pd.Series,
+    # measurement_dataset: npt.NDArray[np.float64],
+) -> pd.Series:
+    match channel.device_id.type:
+        case MeasurementTypeEnum.ANALOG_SQUARED:
+            _s = (
+                (1000 * dataset * channel.dc_dr)
+                / (channel.shots * (2**channel.adc_bits - 1))
+                / np.sqrt(channel.shots - 1)
+            )
+        case MeasurementTypeEnum.PHOTONCOUNTING_SQUARED:
+            _s = (
+                (1000 * dataset * channel.dc_dr)
+                / (channel.shots * (2**channel.adc_bits - 1))
+                / np.sqrt(channel.shots)
+            )
+        case default:
+            raise ValueError(f"Channel not handled: {default}")
+
+    _s[channel.bins:] = np.nan # Remove other non-square-mean
+
+    return _s
```

### Comparing `linc-1.5.0/linc/parse/dataset.py` & `linc-1.6.0/linc/parse/dataset.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import numpy as np
-import pandas as pd
-import numpy.typing as npt
-
-from linc.utils import device_id_to_str
-
-from ..models import Header
-
-
-def parse_dataset(dataset: bytes, header: Header) -> pd.DataFrame:
-    dt = np.dtype(np.uint32)
-    dt = dt.newbyteorder("<")
-
-    max_length = max(map(lambda x: x.bins, header.channels))
-    parsed = np.full((len(header.channels), max_length), fill_value=np.nan)
-    _parsed = pd.DataFrame()
-
-    for channel in header.channels:
-        bytes_size = channel.bins * 4
-        current_array = np.frombuffer(dataset, dtype=dt, count=channel.bins)
-        _parsed[device_id_to_str(channel.device_id)] = np.pad(
-            current_array, (0, max_length - current_array.shape[0]), "empty"
-        )
-        # parsed[idx, : current_array.shape[0]] = current_array
-
-        *_, dataset = dataset[bytes_size:].partition(b"\r\n")
-        # print("parsed: ")
-        # print(parsed)
-        # print(before, symbol)
-
-    # set_trace()
-
-    return _parsed
+import numpy as np
+import pandas as pd
+import numpy.typing as npt
+
+from linc.utils import device_id_to_str
+
+from ..models import Header
+
+
+def parse_dataset(dataset: bytes, header: Header) -> pd.DataFrame:
+    dt = np.dtype(np.uint32)
+    dt = dt.newbyteorder("<")
+
+    max_length = max(map(lambda x: x.bins, header.channels))
+    parsed = np.full((len(header.channels), max_length), fill_value=np.nan)
+    _parsed = pd.DataFrame()
+
+    for channel in header.channels:
+        bytes_size = channel.bins * 4
+        current_array = np.frombuffer(dataset, dtype=dt, count=channel.bins)
+        _parsed[device_id_to_str(channel.device_id)] = np.pad(
+            current_array, (0, max_length - current_array.shape[0]), "empty"
+        )
+        # parsed[idx, : current_array.shape[0]] = current_array
+
+        *_, dataset = dataset[bytes_size:].partition(b"\r\n")
+        # print("parsed: ")
+        # print(parsed)
+        # print(before, symbol)
+
+    # set_trace()
+
+    return _parsed
```

### Comparing `linc-1.5.0/linc/reader.py` & `linc-1.6.0/linc/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-
-from .convertion import convert_to_physical_units
-from .models import DataFileU32, DataFile
-from .config import Config
-from .parse.header import parse_header
-from .parse.dataset import parse_dataset
-from .parse.file import read_file_header_dataset
-
-
-def read_file(file_path: str | Path, config: Config | None = None) -> DataFile:
-    _p = Path(file_path)
-    h, d = read_file_header_dataset(_p)
-    header = parse_header(h.split(b"\r\n"))
-    dataset = parse_dataset(d, header=header)
-
-    file_u32 = DataFileU32(header=header, dataset=dataset)
-    file = convert_to_physical_units(file_u32)
-
-    if config is not None:
-        new_dataset = replace_with_names(file.dataset, config)
-        file = DataFile(header=header, dataset=new_dataset)
-
-    return file
-
-
-def replace_with_names(dataset: pd.DataFrame | pd.Series, config: Config) -> pd.DataFrame | pd.Series:
-    final_columns = list(map(lambda ch: ch.link_to, config.lidar.channels))
-    # set_trace()
-
-    if config.options.channel_not_present_all_ok:
-        select_columns = list(filter(lambda ch: ch in dataset.columns, final_columns))
-    else:
-        select_columns = final_columns
-
-    dataset = dataset[select_columns]
-    
-
-    for channel in config.lidar.channels:
-        if channel.link_to in dataset.columns:
-            if isinstance(dataset, pd.DataFrame):
-                dataset = dataset.rename(columns={channel.link_to: channel.name})
-            else:
-                dataset = dataset.rename({channel.link_to: channel.name})
-        else:
-            if isinstance(dataset, pd.DataFrame):
-                dataset.loc[:, channel.name] = np.nan
-            else:
-                dataset[:] = np.nan
-
-    return dataset
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+
+from .convertion import convert_to_physical_units
+from .models import DataFileU32, DataFile
+from .config import Config
+from .parse.header import parse_header
+from .parse.dataset import parse_dataset
+from .parse.file import read_file_header_dataset
+
+
+def read_file(file_path: str | Path, config: Config) -> DataFile:
+    _p = Path(file_path)
+    h, d = read_file_header_dataset(_p)
+    header = parse_header(h.split(b"\r\n"))
+    dataset = parse_dataset(d, header=header)
+
+    file_u32 = DataFileU32(header=header, dataset=dataset)
+    file = convert_to_physical_units(file_u32, config)
+
+    if config is not None:
+        new_dataset = replace_with_names(file.dataset, config)
+        file = DataFile(header=header, dataset=new_dataset)
+
+    return file
+
+
+def replace_with_names(dataset: pd.DataFrame | pd.Series, config: Config) -> pd.DataFrame | pd.Series:
+    final_columns = list(map(lambda ch: ch.link_to, config.lidar.channels))
+    # set_trace()
+
+    if config.options.channel_not_present_all_ok:
+        select_columns = list(filter(lambda ch: ch in dataset.columns, final_columns))
+    else:
+        select_columns = final_columns
+
+    dataset = dataset[select_columns]
+    
+
+    for channel in config.lidar.channels:
+        if channel.link_to in dataset.columns:
+            if isinstance(dataset, pd.DataFrame):
+                dataset = dataset.rename(columns={channel.link_to: channel.name})
+            else:
+                dataset = dataset.rename({channel.link_to: channel.name})
+        else:
+            if isinstance(dataset, pd.DataFrame):
+                dataset.loc[:, channel.name] = np.nan
+            else:
+                dataset[:] = np.nan
+
+    return dataset
```

### Comparing `linc-1.5.0/linc/utils.py` & `linc-1.6.0/linc/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import pkg_resources
-from typing import TypeVar, Iterator
-
-from .models import DeviceId, MeasurementTypeEnum
-
-
-U = TypeVar("U")
-T = TypeVar("T", str, bytes)
-
-
-def split_seq(seq: list[T], sep: T) -> Iterator[list[T]]:
-    start = 0
-    while start < len(seq):
-        try:
-            stop = start + seq[start:].index(sep)
-            yield seq[start:stop]
-            start = stop + 1
-        except ValueError:
-            yield seq[start:]
-            break
-
-
-def safe_get_list(l: list[U], idx: int, default: U | None) -> U | None:
-    try:
-        return l[idx]
-    except IndexError:
-        return default
-
-
-def to_acquisition_type_string(type: MeasurementTypeEnum) -> str:
-    match type:
-        case MeasurementTypeEnum.ANALOG:
-            return "a"
-        case MeasurementTypeEnum.ANALOG_SQUARED:
-            return "A"
-        case MeasurementTypeEnum.PHOTONCOUNTING:
-            return "p"
-        case MeasurementTypeEnum.PHOTONCOUNTING_SQUARED:
-            return "P"
-        case _:
-            raise ValueError("Input type not supported")
-
-
-def device_id_to_str(device_id: DeviceId) -> str:
-    return f"{device_id.type}{device_id.number}"
-
-
-def str_to_device_id(device_id: str) -> DeviceId:
-    sep_index = 3 if device_id.startswith("S2") else 2
-
-    # set_trace()
-    return DeviceId(
-        type=device_id[:sep_index], # type: ignore
-        number=device_id[sep_index:] # type: ignore
-    )
+import pkg_resources
+from typing import TypeVar, Iterator
+
+from .models import DeviceId, MeasurementTypeEnum
+
+
+U = TypeVar("U")
+T = TypeVar("T", str, bytes)
+
+
+def split_seq(seq: list[T], sep: T) -> Iterator[list[T]]:
+    start = 0
+    while start < len(seq):
+        try:
+            stop = start + seq[start:].index(sep)
+            yield seq[start:stop]
+            start = stop + 1
+        except ValueError:
+            yield seq[start:]
+            break
+
+
+def safe_get_list(l: list[U], idx: int, default: U | None) -> U | None:
+    try:
+        return l[idx]
+    except IndexError:
+        return default
+
+
+def to_acquisition_type_string(type: MeasurementTypeEnum) -> str:
+    match type:
+        case MeasurementTypeEnum.ANALOG:
+            return "a"
+        case MeasurementTypeEnum.ANALOG_SQUARED:
+            return "A"
+        case MeasurementTypeEnum.PHOTONCOUNTING:
+            return "p"
+        case MeasurementTypeEnum.PHOTONCOUNTING_SQUARED:
+            return "P"
+        case _:
+            raise ValueError("Input type not supported")
+
+
+def device_id_to_str(device_id: DeviceId) -> str:
+    return f"{device_id.type}{device_id.number}"
+
+
+def str_to_device_id(device_id: str) -> DeviceId:
+    sep_index = 3 if device_id.startswith("S2") else 2
+
+    # set_trace()
+    return DeviceId(
+        type=device_id[:sep_index], # type: ignore
+        number=device_id[sep_index:] # type: ignore
+    )
```

### Comparing `linc-1.5.0/linc/write/common.py` & `linc-1.6.0/linc/write/common.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from ..config import Config
-from ..models import Channel, Header
-from ..utils import device_id_to_str, safe_get_list, to_acquisition_type_string
-
-
-def compare_joinable_dataset(header1: Header, header2: Header) -> None:
-    assert (
-        header1.channels == header2.channels
-    ), "While parsing a same dataset, channels most remain identical"
-
-    assert (
-        header1.location == header2.location
-    ), "While parsing a same dataset, channels most remain identical"
-
-
-
-def get_merged_channel_config(channel: Channel, config: Config) -> Channel:
-    channel_as_str = device_id_to_str(channel.device_id)
-    channel_config = safe_get_list(
-        list(filter(lambda c: c.link_to == channel_as_str, config.lidar.channels)),
-        0,
-        None,
-    )
-
-    if channel_config is None:
-        return channel
-
-    return Channel(**channel.copy(update=channel_config).dict())  # type: ignore
-
-
-def format_channel(channel: Channel, format: str) -> str:
-    format = format.replace(r"%w", str(channel.wavelength))
-    format = format.replace(r"%p", channel.polarization.value)
-    format = format.replace(r"%a", to_acquisition_type_string(channel.device_id.type))
-    format = format.replace(
-        r"%i", f"{channel.device_id.type}{channel.device_id.number}"
-    )
-
-    return format
+from ..config import Config
+from ..models import Channel, Header
+from ..utils import device_id_to_str, safe_get_list, to_acquisition_type_string
+
+
+def compare_joinable_dataset(header1: Header, header2: Header) -> None:
+    assert (
+        header1.channels == header2.channels
+    ), "While parsing a same dataset, channels most remain identical"
+
+    assert (
+        header1.location == header2.location
+    ), "While parsing a same dataset, channels most remain identical"
+
+
+
+def get_merged_channel_config(channel: Channel, config: Config) -> Channel:
+    channel_as_str = device_id_to_str(channel.device_id)
+    channel_config = safe_get_list(
+        list(filter(lambda c: c.link_to == channel_as_str, config.lidar.channels)),
+        0,
+        None,
+    )
+
+    if channel_config is None:
+        return channel
+
+    return Channel(**channel.copy(update=channel_config).dict())  # type: ignore
+
+
+def format_channel(channel: Channel, format: str) -> str:
+    format = format.replace(r"%w", str(channel.wavelength))
+    format = format.replace(r"%p", channel.polarization.value)
+    format = format.replace(r"%a", to_acquisition_type_string(channel.device_id.type))
+    format = format.replace(
+        r"%i", f"{channel.device_id.type}{channel.device_id.number}"
+    )
+
+    return format
```

### Comparing `linc-1.5.0/linc/write/writer_nc.py` & `linc-1.6.0/linc/write/writer_nc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,181 +1,182 @@
-import time
-import warnings
-import pkg_resources
-from pathlib import Path
-from typing import Any
-from collections.abc import Iterable
-
-import numpy as np
-from rich.progress import Progress
-from cftime import date2num
-
-from ..models import DataFile
-from ..reader import read_file
-from ..config import Config
-from ..config.models import LidarChannel
-from ..parse.utils import parse_date_from_filename
-
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore")
-    from netCDF4 import Dataset  # type: ignore
-
-
-def write_nc_legacy(
-    files: Iterable[Path | str],
-    output_file: Path | str,
-    config: Config,
-) -> None:
-    _f = sorted(list(files), key=lambda p: Path(p).name)
-
-    nc = Dataset(output_file, "w")
-    nc.history = "Created " + time.ctime(time.time())
-    nc.generated_with = str(pkg_resources.get_distribution("linc").egg_name())
-
-    bin_width = config.lidar.bin_width
-    bin_count = config.lidar.bin_count
-    channel_array = np.array(filter_real_channels(config.lidar.channels))
-    first_time = parse_date_from_filename(Path(_f[0]).name)
-
-    time_dim = nc.createDimension("time", None)
-    range_dim = nc.createDimension("range", config.lidar.bin_count)
-    channel_dim = nc.createDimension("channel", channel_array.shape[0])
-
-    time_var = nc.createVariable("time", "i4", ("time",), compression="zlib")
-    time_var.units = f"milliseconds since {first_time.isoformat().replace('T', ' ')}"
-    time_var.calendar = "proleptic_gregorian"
-
-    range_var = nc.createVariable("range", "f4", ("range",), compression="zlib")
-    range_var[:] = np.arange(bin_width, bin_width * (bin_count + 1), bin_width)
-
-    channel_var = nc.createVariable("channel", "S8", ("channel",))
-    channel_var[:] = channel_array
-
-    signal_vars = create_signal_variables(nc, config)  # Raw signal
-    lidar_vars = create_lidar_vars(nc, config)
-    # channels_vars = create_channels_vars(nc, config)
-
-    progress = Progress()
-
-    total_files = len(_f)
-    total_digits = len(str(total_files))
-    task1 = progress.add_task("[red]Processing...", total=len(_f))
-
-    with progress:
-        for idx_f, iter_file in enumerate(_f):
-            current_file = read_file(iter_file, config=config)
-
-            write_signal_vars(current_file, time_var, signal_vars, idx_f)
-            write_lidar_vars(current_file, lidar_vars, idx_f)
-
-            progress.update(
-                task1,
-                advance=1,
-                description=f"[blue]Converting {idx_f + 1:0{total_digits}d}/{total_files} file",  # noqa: E501
-            )
-            # write_channels_vars(current_file, channel_array, channels_vars, idx_f)
-        
-
-    # progress.remove_task(task1)
-
-    write_attrs(nc, config)
-
-    nc.close()
-
-
-def write_signal_vars(
-    current_file: DataFile, time_var: Any, signal_vars: list[Any], index: int
-) -> None:
-    time_var[index] = date2num(
-        current_file.header.start_date, units=time_var.units, calendar=time_var.calendar
-    )
-    for (channel_str, channel_var) in signal_vars:
-        channel_var[index, :] = current_file.dataset[channel_str].values  # type: ignore
-
-
-def write_attrs(nc: Any, config: Config) -> None:
-    for k, v in config.lidar.attrs.items():
-        set_or_create_attr(nc, attr_name=k, attr_value=v)
-
-
-def create_signal_variables(nc: Any, config: Config) -> list[Any]:
-    signal_vars: list[tuple[str, Any]] = []
-    for channel in list(map(lambda x: x.name, config.lidar.channels)):
-        channel_str = channel
-        try:
-            signal_var = nc.createVariable(
-                f"{channel_str}",
-                "f8",
-                ("time", "range"),
-                compression="zlib",
-            )
-        except Exception:
-            raise ValueError(f"problem creating variable: {channel_str}")
-
-        signal_vars.append((channel_str, signal_var))
-    return signal_vars
-
-
-def set_or_create_attr(var, attr_name, attr_value):
-    if attr_name in var.ncattrs():
-        var.setncattr(attr_name, attr_value)
-        return
-    try:
-        var.UnusedNameAttribute = attr_value
-        var.renameAttribute("UnusedNameAttribute", attr_name)
-    except TypeError:
-        raise TypeError(
-            f"Type of attribute {attr_name} is {type(attr_value)} which cannot be written in netCDF"  # noqa: E501
-        )
-    return
-
-
-def filter_real_channels(lidar_channels: list[LidarChannel]) -> list[str]:
-    """This function retrieves the lidar channel regardless if stderr or signal.
-    For example, if there are two LidarChannel signal_532xpa and stderr_532xpa, it only returns 532xpa to channels list
-
-    Args:
-        lidar_channels (list[LidarChannel]): list of config sourced channels
-
-    Returns:
-        list[str]: strings with the convention wavelenght|telescope|polarization|aq_type. Ej: 532xpa
-    """  # noqa: E501
-    channels: set[str] = set({})
-
-    for lidar_channel in lidar_channels:
-        channels |= {lidar_channel.name.split("_")[1]}
-
-    return list(channels)
-
-
-def create_lidar_vars(nc, config: Config) -> list[tuple[str, Any]]:
-    lidar_vars: list[tuple[str, Any]] = []
-    for opt_var in config.options.time_lidar_variables:
-        lidar_var = nc.createVariable(
-            opt_var.name,
-            opt_var.type,
-            ("time",),
-            compression="zlib",
-        )
-        lidar_vars.append((opt_var.name, lidar_var))
-    return lidar_vars
-
-
-# def create_channels_vars(nc: Any, config: Config) -> list[tuple[str, Any]]:
-#     channels_vars: list[tuple[str, Any]] = []
-#     for opt_var in config.options.time_channel_variables:
-#         channels_var = nc.createVariable(
-#             opt_var.name,
-#             opt_var.type,
-#             ("time", "channel"),
-#             compression="zlib",
-#         )
-#         channels_vars.append((opt_var.name, channels_var))
-#     return channels_vars
-
-
-def write_lidar_vars(
-    current_file: DataFile, lidar_vars: list[tuple[str, Any]], index: int
-) -> None:
-    for lidar_var in lidar_vars:
-        value = getattr(current_file.header, lidar_var[0])
-        lidar_var[1][index] = value
+import time
+import warnings
+import pkg_resources
+from pathlib import Path
+from typing import Any
+from collections.abc import Iterable
+
+import numpy as np
+from rich.progress import Progress
+from rich.console import Console
+from cftime import date2num
+
+from ..models import DataFile
+from ..reader import read_file
+from ..config import Config
+from ..config.models import LidarChannel
+from ..parse.utils import parse_date_from_filename
+
+with warnings.catch_warnings():
+    warnings.filterwarnings("ignore")
+    from netCDF4 import Dataset  # type: ignore
+
+
+def write_nc_legacy(
+    files: Iterable[Path | str],
+    output_file: Path | str,
+    config: Config,
+) -> None:
+    _f = sorted(list(files), key=lambda p: Path(p).name)
+
+    nc = Dataset(output_file, "w")
+    nc.history = "Created " + time.ctime(time.time())
+    nc.generated_with = str(pkg_resources.get_distribution("linc").egg_name())
+
+    bin_width = config.lidar.bin_width
+    bin_count = config.lidar.bin_count
+    channel_array = np.array(filter_real_channels(config.lidar.channels))
+    first_time = parse_date_from_filename(Path(_f[0]).name)
+
+    time_dim = nc.createDimension("time", None)
+    range_dim = nc.createDimension("range", config.lidar.bin_count)
+    channel_dim = nc.createDimension("channel", channel_array.shape[0])
+
+    time_var = nc.createVariable("time", "i4", ("time",), compression="zlib")
+    time_var.units = f"milliseconds since {first_time.isoformat().replace('T', ' ')}"
+    time_var.calendar = "proleptic_gregorian"
+
+    range_var = nc.createVariable("range", "f4", ("range",), compression="zlib")
+    range_var[:] = np.arange(bin_width, bin_width * (bin_count + 1), bin_width)
+
+    channel_var = nc.createVariable("channel", "S8", ("channel",))
+    channel_var[:] = channel_array
+
+    signal_vars = create_signal_variables(nc, config)  # Raw signal
+    lidar_vars = create_lidar_vars(nc, config)
+    # channels_vars = create_channels_vars(nc, config)
+
+    progress = Progress()
+
+    total_files = len(_f)
+    total_digits = len(str(total_files))
+    task1 = progress.add_task("[red]Processing...", total=len(_f))
+
+    with progress:
+        for idx_f, iter_file in enumerate(_f):
+            current_file = read_file(iter_file, config=config)
+
+            write_signal_vars(current_file, time_var, signal_vars, idx_f)
+            write_lidar_vars(current_file, lidar_vars, idx_f)
+
+            progress.update(
+                task1,
+                advance=1,
+                description=f"[blue]Converting {idx_f + 1:0{total_digits}d}/{total_files} file",  # noqa: E501
+            )
+            # write_channels_vars(current_file, channel_array, channels_vars, idx_f)
+        
+
+    # progress.remove_task(task1)
+
+    write_attrs(nc, config)
+
+    nc.close()
+
+
+def write_signal_vars(
+    current_file: DataFile, time_var: Any, signal_vars: list[Any], index: int
+) -> None:
+    time_var[index] = date2num(
+        current_file.header.start_date, units=time_var.units, calendar=time_var.calendar
+    )
+    for (channel_str, channel_var) in signal_vars:
+        channel_var[index, :] = current_file.dataset[channel_str].values  # type: ignore
+
+
+def write_attrs(nc: Any, config: Config) -> None:
+    for k, v in config.lidar.attrs.items():
+        set_or_create_attr(nc, attr_name=k, attr_value=v)
+
+
+def create_signal_variables(nc: Any, config: Config) -> list[Any]:
+    signal_vars: list[tuple[str, Any]] = []
+    for channel in list(map(lambda x: x.name, config.lidar.channels)):
+        channel_str = channel
+        try:
+            signal_var = nc.createVariable(
+                f"{channel_str}",
+                "f8",
+                ("time", "range"),
+                compression="zlib",
+            )
+        except Exception:
+            raise ValueError(f"problem creating variable: {channel_str}")
+
+        signal_vars.append((channel_str, signal_var))
+    return signal_vars
+
+
+def set_or_create_attr(var, attr_name, attr_value):
+    if attr_name in var.ncattrs():
+        var.setncattr(attr_name, attr_value)
+        return
+    try:
+        var.UnusedNameAttribute = attr_value
+        var.renameAttribute("UnusedNameAttribute", attr_name)
+    except TypeError:
+        raise TypeError(
+            f"Type of attribute {attr_name} is {type(attr_value)} which cannot be written in netCDF"  # noqa: E501
+        )
+    return
+
+
+def filter_real_channels(lidar_channels: list[LidarChannel]) -> list[str]:
+    """This function retrieves the lidar channel regardless if stderr or signal.
+    For example, if there are two LidarChannel signal_532xpa and stderr_532xpa, it only returns 532xpa to channels list
+
+    Args:
+        lidar_channels (list[LidarChannel]): list of config sourced channels
+
+    Returns:
+        list[str]: strings with the convention wavelenght|telescope|polarization|aq_type. Ej: 532xpa
+    """  # noqa: E501
+    channels: set[str] = set({})
+
+    for lidar_channel in lidar_channels:
+        channels |= {lidar_channel.name.split("_")[1]}
+
+    return list(channels)
+
+
+def create_lidar_vars(nc, config: Config) -> list[tuple[str, Any]]:
+    lidar_vars: list[tuple[str, Any]] = []
+    for opt_var in config.options.time_lidar_variables:
+        lidar_var = nc.createVariable(
+            opt_var.name,
+            opt_var.type,
+            ("time",),
+            compression="zlib",
+        )
+        lidar_vars.append((opt_var.name, lidar_var))
+    return lidar_vars
+
+
+# def create_channels_vars(nc: Any, config: Config) -> list[tuple[str, Any]]:
+#     channels_vars: list[tuple[str, Any]] = []
+#     for opt_var in config.options.time_channel_variables:
+#         channels_var = nc.createVariable(
+#             opt_var.name,
+#             opt_var.type,
+#             ("time", "channel"),
+#             compression="zlib",
+#         )
+#         channels_vars.append((opt_var.name, channels_var))
+#     return channels_vars
+
+
+def write_lidar_vars(
+    current_file: DataFile, lidar_vars: list[tuple[str, Any]], index: int
+) -> None:
+    for lidar_var in lidar_vars:
+        value = getattr(current_file.header, lidar_var[0])
+        lidar_var[1][index] = value
```

### Comparing `linc-1.5.0/PKG-INFO` & `linc-1.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linc
-Version: 1.5.0
+Version: 1.6.0
 Summary: A package to handle LICEL Binary format
 License: MIT
 Author: Juan Diego
 Author-email: jdlar@eafit.edu.co
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

