# Comparing `tmp/PyEventEngine-0.1.4.tar.gz` & `tmp/PyEventEngine-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEventEngine-0.1.4.tar", last modified: Fri Sep 16 03:20:48 2022, max compression
+gzip compressed data, was "PyEventEngine-0.2.1.tar", last modified: Wed Jun  7 19:56:04 2023, max compression
```

## Comparing `PyEventEngine-0.1.4.tar` & `PyEventEngine-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2022-09-16 03:20:49.878538 PyEventEngine-0.1.4/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2022-09-16 03:20:49.718558 PyEventEngine-0.1.4/EventEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2022-09-16 03:20:49.787952 PyEventEngine-0.1.4/EventEngine/Core/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    12094 2022-09-16 03:18:28.000000 PyEventEngine-0.1.4/EventEngine/Core/_Event.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3613 2022-09-09 07:00:56.000000 PyEventEngine-0.1.4/EventEngine/Core/_Topic.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3065 2022-09-14 03:36:07.000000 PyEventEngine-0.1.4/EventEngine/Core/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       46 2022-09-16 03:18:28.000000 PyEventEngine-0.1.4/EventEngine/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2022-09-09 09:50:11.000000 PyEventEngine-0.1.4/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2001 2022-09-16 03:20:49.879540 PyEventEngine-0.1.4/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2022-09-16 03:20:49.859537 PyEventEngine-0.1.4/PyEventEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2001 2022-09-16 03:20:47.000000 PyEventEngine-0.1.4/PyEventEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      291 2022-09-16 03:20:48.000000 PyEventEngine-0.1.4/PyEventEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2022-09-16 03:20:47.000000 PyEventEngine-0.1.4/PyEventEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2022-09-16 03:20:47.000000 PyEventEngine-0.1.4/PyEventEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2022-09-13 02:50:04.000000 PyEventEngine-0.1.4/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2022-09-16 03:20:49.883537 PyEventEngine-0.1.4/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1443 2022-09-09 09:58:03.000000 PyEventEngine-0.1.4/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:04.152082 PyEventEngine-0.2.1/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:03.840799 PyEventEngine-0.2.1/EventEngine/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:03.967363 PyEventEngine-0.2.1/EventEngine/Core/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    11736 2023-05-29 07:51:43.000000 PyEventEngine-0.2.1/EventEngine/Core/_Event.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3488 2023-05-29 09:31:15.000000 PyEventEngine-0.2.1/EventEngine/Core/_Topic.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     5821 2023-06-07 19:47:58.000000 PyEventEngine-0.2.1/EventEngine/Core/_Topic_c.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3128 2023-06-07 19:32:17.000000 PyEventEngine-0.2.1/EventEngine/Core/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       43 2023-06-07 18:11:39.000000 PyEventEngine-0.2.1/EventEngine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:03.999337 PyEventEngine-0.2.1/EventEngine/cpp/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9038 2023-06-07 19:15:36.000000 PyEventEngine-0.2.1/EventEngine/cpp/topic_api.cpp
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-05-27 08:57:55.000000 PyEventEngine-0.2.1/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2001 2023-06-07 19:56:04.154077 PyEventEngine-0.2.1/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:04.115557 PyEventEngine-0.2.1/PyEventEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2001 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      350 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2023-05-27 08:57:55.000000 PyEventEngine-0.2.1/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2023-06-07 19:56:04.163074 PyEventEngine-0.2.1/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1633 2023-06-07 19:02:25.000000 PyEventEngine-0.2.1/setup.py
```

### Comparing `PyEventEngine-0.1.4/EventEngine/Core/_Topic.py` & `PyEventEngine-0.2.1/EventEngine/Core/_Topic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from __future__ import annotations
-
-import re
-from enum import Enum
-from string import Formatter
-
-
-class Topic(dict):
-    """
-    topic for event hook. e.g. "TickData.002410.SZ.Realtime"
-    """
-
-    class Error(Exception):
-        def __init__(self, msg):
-            super().__init__(msg)
-
-    def __init__(self, topic: str, *args, **kwargs):
-        self._value = topic
-        super().__init__(*args, **kwargs)
-
-    def __repr__(self):
-        return f'<{self.__class__.__name__}>({self._value}){super().__repr__()}'
-
-    def __str__(self):
-        return self.value
-
-    def __bool__(self):
-        return True
-
-    def __hash__(self):
-        return self.value.__hash__()
-
-    def match(self, topic: str) -> Topic | None:
-        if self._value == topic:
-            return self.__class__(topic=topic)
-        else:
-            return None
-
-    @classmethod
-    def cast(cls, topic: Topic | str | Enum, dtype=None) -> Topic:
-        if isinstance(topic, Enum):
-            topic = topic.value
-        elif isinstance(topic, Topic):
-            return topic
-
-        if dtype is None:
-            if re.search(r'{(.+?)}', topic):
-                t = PatternTopic(pattern=topic)
-            elif '*' in topic or '+' in topic or '|' in topic:
-                re.compile(pattern=topic)
-                t = RegularTopic(pattern=topic)
-            else:
-                t = Topic(topic=topic)
-        else:
-            t = dtype(topic)
-
-        return t
-
-    @property
-    def value(self) -> str:
-        return self._value
-
-
-class RegularTopic(Topic):
-    """
-    topic in regular expression. e.g. "TickData.(.+).((SZ)|(SH)).((Realtime)|(History))"
-    """
-
-    def __init__(self, pattern: str):
-        super().__init__(topic=pattern)
-
-    def match(self, topic: str) -> Topic | None:
-        if re.match(self._value, topic):
-            match = Topic(topic=topic)
-            match['pattern'] = self._value
-            return match
-        else:
-            return None
-
-
-class PatternTopic(Topic):
-    """
-    topic for event hook. e.g. "TickData.{symbol}.{market}.{flag}"
-    """
-
-    def __init__(self, pattern: str):
-        super().__init__(topic=pattern)
-
-    def __call__(self, **kwargs):
-        return self.format_map(kwargs)
-
-    @classmethod
-    def string_to_dict(cls, target: str, pattern: str):
-        pattern = re.escape(pattern)
-        regex = re.sub(r'\\{(.+?)\\}', r'(?P<_\1>.+)', pattern)
-        match = re.match(regex, target)
-        if match:
-            values = list(match.groups())
-            keys = re.findall(r'\\{(.+?)\\}', pattern)
-            m = dict(zip(keys, values))
-            return m
-        else:
-            raise Topic.Error(f'pattern {pattern} not in string {target} found!')
-
-    def format_map(self, mapping: dict) -> Topic:
-        for key in self.keys():
-            if key not in mapping:
-                mapping[key] = f'{{{key}}}'
-
-        return Topic.cast(self._value.format_map(mapping))
-
-    def keys(self):
-        keys = [i[1] for i in Formatter().parse(self._value) if i[1] is not None]
-        return keys
-
-    def match(self, topic: str) -> Topic | None:
-        try:
-            keyword_dict = self.string_to_dict(target=topic, pattern=self._value)
-            match = Topic(topic=topic)
-            match.update(keyword_dict)
-            return match
-        except self.Error as _:
-            return None
-
-    @property
-    def value(self) -> str:
-        return self._value.format_map({_: '*' for _ in self.keys()})
+from __future__ import annotations
+
+import re
+from enum import Enum
+from string import Formatter
+
+
+class Topic(dict):
+    """
+    topic for event hook. e.g. "TickData.002410.SZ.Realtime"
+    """
+
+    class Error(Exception):
+        def __init__(self, msg):
+            super().__init__(msg)
+
+    def __init__(self, topic: str, *args, **kwargs):
+        self._value = topic
+        super().__init__(*args, **kwargs)
+
+    def __repr__(self):
+        return f'<{self.__class__.__name__}>({self._value}){super().__repr__()}'
+
+    def __str__(self):
+        return self.value
+
+    def __bool__(self):
+        return True
+
+    def __hash__(self):
+        return self.value.__hash__()
+
+    def match(self, topic: str) -> Topic | None:
+        if self._value == topic:
+            return self.__class__(topic=topic)
+        else:
+            return None
+
+    @classmethod
+    def cast(cls, topic: Topic | str | Enum, dtype=None) -> Topic:
+        if isinstance(topic, Enum):
+            topic = topic.value
+        elif isinstance(topic, Topic):
+            return topic
+
+        if dtype is None:
+            if re.search(r'{(.+?)}', topic):
+                t = PatternTopic(pattern=topic)
+            elif '*' in topic or '+' in topic or '|' in topic:
+                re.compile(pattern=topic)
+                t = RegularTopic(pattern=topic)
+            else:
+                t = Topic(topic=topic)
+        else:
+            t = dtype(topic)
+
+        return t
+
+    @property
+    def value(self) -> str:
+        return self._value
+
+
+class RegularTopic(Topic):
+    """
+    topic in regular expression. e.g. "TickData.(.+).((SZ)|(SH)).((Realtime)|(History))"
+    """
+
+    def __init__(self, pattern: str):
+        super().__init__(topic=pattern)
+
+    def match(self, topic: str) -> Topic | None:
+        if re.match(self._value, topic):
+            match = Topic(topic=topic)
+            match['pattern'] = self._value
+            return match
+        else:
+            return None
+
+
+class PatternTopic(Topic):
+    """
+    topic for event hook. e.g. "TickData.{symbol}.{market}.{flag}"
+    """
+
+    def __init__(self, pattern: str):
+        super().__init__(topic=pattern)
+
+    def __call__(self, **kwargs):
+        return self.format_map(kwargs)
+
+    @classmethod
+    def extract_mapping(cls, target: str, pattern: str):
+        pattern = re.escape(pattern)
+        regex = re.sub(r'\\{(.+?)\\}', r'(?P<_\1>.+)', pattern)
+        match = re.match(regex, target)
+        if match:
+            values = list(match.groups())
+            keys = re.findall(r'\\{(.+?)\\}', pattern)
+            m = dict(zip(keys, values))
+            return m
+        else:
+            raise Topic.Error(f'pattern {pattern} not in string {target} found!')
+
+    def format_map(self, mapping: dict) -> Topic:
+        for key in self.keys():
+            if key not in mapping:
+                mapping[key] = f'{{{key}}}'
+
+        return Topic.cast(self._value.format_map(mapping))
+
+    def keys(self):
+        keys = [i[1] for i in Formatter().parse(self._value) if i[1] is not None]
+        return keys
+
+    def match(self, topic: str) -> Topic | None:
+        try:
+            keyword_dict = self.extract_mapping(target=topic, pattern=self._value)
+            match = Topic(topic=topic)
+            match.update(keyword_dict)
+            return match
+        except self.Error as _:
+            return None
+
+    @property
+    def value(self) -> str:
+        return self._value.format_map({_: '*' for _ in self.keys()})
```

### Comparing `PyEventEngine-0.1.4/EventEngine/Core/__init__.py` & `PyEventEngine-0.2.1/EventEngine/Core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,97 @@
-from __future__ import annotations
-
-import logging
-import sys
-import time
-
-__all__ = ['set_logger', 'LOG_LEVEL_EVENT', 'Topic', 'RegularTopic', 'PatternTopic', 'EventHook', 'EventEngine']
-LOGGER: logging.Logger | None = None
-LOG_LEVEL = logging.INFO
-LOG_LEVEL_EVENT = LOG_LEVEL - 1
-
-
-class ColoredFormatter(logging.Formatter):
-    """Logging Formatter to add colors and count warning / errors"""
-
-    def __init__(self, fmt=None, datefmt=None, style='{', validate=True):
-        self.format_str = '[{asctime} {name} - {threadName} - {module}:{lineno} - {levelname}] {message}' if fmt is None else fmt
-        self.date_fmt = '%Y-%m-%d %H:%M:%S' if datefmt is None else datefmt
-        self.style = style
-
-        super().__init__(fmt=fmt, datefmt=datefmt, style=style, validate=validate)
-
-    def _get_format(self, level: int, select=False):
-        bold_red = f"\33[31;1;3;4{';7' if select else ''}m"
-        red = f"\33[31;1{';7' if select else ''}m"
-        green = f"\33[32;1{';7' if select else ''}m"
-        yellow = f"\33[33;1{';7' if select else ''}m"
-        blue = f"\33[34;1{';7' if select else ''}m"
-        reset = "\33[0m"
-
-        if level <= logging.NOTSET:
-            fmt = self.format_str
-        elif level <= logging.DEBUG:
-            fmt = blue + self.format_str + reset
-        elif level <= logging.INFO:
-            fmt = green + self.format_str + reset
-        elif level <= logging.WARNING:
-            fmt = yellow + self.format_str + reset
-        elif level <= logging.ERROR:
-            fmt = red + self.format_str + reset
-        else:
-            fmt = bold_red + self.format_str + reset
-
-        return fmt
-
-    def format(self, record):
-        log_fmt = self._get_format(level=record.levelno)
-        formatter = logging.Formatter(log_fmt, datefmt=self.date_fmt, style=self.style)
-        return formatter.format(record)
-
-
-def get_logger(**kwargs) -> logging.Logger:
-    level = kwargs.get('level', LOG_LEVEL)
-    stream_io = kwargs.get('stream_io', sys.stdout)
-    formatter = kwargs.get('formatter', ColoredFormatter())
-    global LOGGER
-
-    if LOGGER is not None:
-        return LOGGER
-
-    LOGGER = logging.getLogger('EventEngine')
-    LOGGER.setLevel(level)
-    logging.Formatter.converter = time.gmtime
-
-    if stream_io:
-        have_handler = False
-        for handler in LOGGER.handlers:
-            # noinspection PyUnresolvedReferences
-            if type(handler) == logging.StreamHandler and handler.stream == stream_io:
-                have_handler = True
-                break
-
-        if not have_handler:
-            logger_ch = logging.StreamHandler(stream=stream_io)
-            logger_ch.setLevel(level=level)
-            logger_ch.setFormatter(fmt=formatter)
-            LOGGER.addHandler(logger_ch)
-
-    return LOGGER
-
-
-def set_logger(logger: logging.Logger):
-    global LOGGER
-    LOGGER = logger
-
-
-_ = get_logger()
-
-from ._Topic import Topic, RegularTopic, PatternTopic
-from ._Event import EventHook, EventEngine
+from __future__ import annotations
+
+import logging
+import sys
+import time
+
+__all__ = ['set_logger', 'LOG_LEVEL_EVENT', 'Topic', 'RegularTopic', 'PatternTopic', 'EventHook', 'EventEngine', 'LOGGER']
+LOGGER: logging.Logger | None = None
+LOG_LEVEL = logging.INFO
+LOG_LEVEL_EVENT = LOG_LEVEL - 1
+
+
+class ColoredFormatter(logging.Formatter):
+    """Logging Formatter to add colors and count warning / errors"""
+
+    def __init__(self, fmt=None, datefmt=None, style='{', validate=True):
+        self.format_str = '[{asctime} {name} - {threadName} - {module}:{lineno} - {levelname}] {message}' if fmt is None else fmt
+        self.date_fmt = '%Y-%m-%d %H:%M:%S' if datefmt is None else datefmt
+        self.style = style
+
+        super().__init__(fmt=fmt, datefmt=datefmt, style=style, validate=validate)
+
+    def _get_format(self, level: int, select=False):
+        bold_red = f"\33[31;1;3;4{';7' if select else ''}m"
+        red = f"\33[31;1{';7' if select else ''}m"
+        green = f"\33[32;1{';7' if select else ''}m"
+        yellow = f"\33[33;1{';7' if select else ''}m"
+        blue = f"\33[34;1{';7' if select else ''}m"
+        reset = "\33[0m"
+
+        if level <= logging.NOTSET:
+            fmt = self.format_str
+        elif level <= logging.DEBUG:
+            fmt = blue + self.format_str + reset
+        elif level <= logging.INFO:
+            fmt = green + self.format_str + reset
+        elif level <= logging.WARNING:
+            fmt = yellow + self.format_str + reset
+        elif level <= logging.ERROR:
+            fmt = red + self.format_str + reset
+        else:
+            fmt = bold_red + self.format_str + reset
+
+        return fmt
+
+    def format(self, record):
+        log_fmt = self._get_format(level=record.levelno)
+        formatter = logging.Formatter(log_fmt, datefmt=self.date_fmt, style=self.style)
+        return formatter.format(record)
+
+
+def get_logger(**kwargs) -> logging.Logger:
+    level = kwargs.get('level', LOG_LEVEL)
+    stream_io = kwargs.get('stream_io', sys.stdout)
+    formatter = kwargs.get('formatter', ColoredFormatter())
+    global LOGGER
+
+    if LOGGER is not None:
+        return LOGGER
+
+    LOGGER = logging.getLogger('EventEngine')
+    LOGGER.setLevel(level)
+    logging.Formatter.converter = time.gmtime
+
+    if stream_io:
+        have_handler = False
+        for handler in LOGGER.handlers:
+            # noinspection PyUnresolvedReferences
+            if type(handler) == logging.StreamHandler and handler.stream == stream_io:
+                have_handler = True
+                break
+
+        if not have_handler:
+            logger_ch = logging.StreamHandler(stream=stream_io)
+            logger_ch.setLevel(level=level)
+            logger_ch.setFormatter(fmt=formatter)
+            LOGGER.addHandler(logger_ch)
+
+    return LOGGER
+
+
+def set_logger(logger: logging.Logger):
+    global LOGGER
+    LOGGER = logger
+
+
+_ = get_logger()
+
+# use c++ optimized module
+try:
+    from ._Topic_c import Topic, RegularTopic, PatternTopic
+except Exception as _:
+    from ._Topic import Topic, RegularTopic, PatternTopic
+
+    LOGGER.warning(_)
+
+from ._Event import EventHook, EventEngine
```

### Comparing `PyEventEngine-0.1.4/LICENSE` & `PyEventEngine-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyEventEngine-0.1.4/PKG-INFO` & `PyEventEngine-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.1.4
+Version: 0.2.1
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyEventEngine-0.1.4/PyEventEngine.egg-info/PKG-INFO` & `PyEventEngine-0.2.1/PyEventEngine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.1.4
+Version: 0.2.1
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyEventEngine-0.1.4/README.md` & `PyEventEngine-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PyEventEngine-0.1.4/setup.py` & `PyEventEngine-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import setuptools
-import os
 import codecs
+import os
+
+import setuptools.extension
 
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
@@ -39,10 +40,12 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     license='MIT',
-    install_requires=[
-    ]
+    install_requires=[],
+    ext_modules=[
+        setuptools.extension.Extension(r'EventEngine.topic_api', sources=[r'EventEngine/cpp/topic_api.cpp'], include_dirs=[], language='c++', optional=True),
+    ],
 )
```

