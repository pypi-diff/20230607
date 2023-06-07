# Comparing `tmp/fileformats-0.5.2.tar.gz` & `tmp/fileformats-0.6.tar.gz`

## Comparing `fileformats-0.5.2.tar` & `fileformats-0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/_version.py
--rw-r--r--   0        0        0    35322 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/base.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/converter.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/mark.py
--rw-r--r--   0        0        0    23709 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/mixin.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/utils.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_qualifiers.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/base.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/raster.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.5.2/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.5.2/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.5.2/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.5.2/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.5.2/README.rst
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 fileformats-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    22552 2020-02-02 00:00:00.000000 fileformats-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/_version.py
+-rw-r--r--   0        0        0    41119 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/base.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/converter.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6/README.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6/pyproject.toml
+-rw-r--r--   0        0        0    22510 2020-02-02 00:00:00.000000 fileformats-0.6/PKG-INFO
```

### Comparing `fileformats-0.5.2/fileformats/archive/__init__.py` & `fileformats-0.6/fileformats/archive/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from fileformats.core import __version__
 from warnings import warn
 from fileformats.core import FileSet
-from fileformats.core.mixin import WithQualifiers
+from fileformats.core.mixin import WithClassifiers
 from fileformats.generic import File
 from fileformats.core.mixin import WithMagicNumber
 
 
-class Archive(WithQualifiers, File):
+class Archive(WithClassifiers, File):
     "Base class for compressed archives"
 
-    qualifiers_attr_name = "archived_type"
+    classifiers_attr_name = "archived_type"
     archived_type = None
-    multiple_qualifiers = False
-    allowed_qualifiers = (FileSet,)
+    multiple_classifiers = False
+    allowed_classifiers = (FileSet,)
     generically_qualifies = True
 
     binary = True
     iana_mime = None
 
 
 # Compressed formats
```

### Comparing `fileformats-0.5.2/fileformats/archive/converters.py` & `fileformats-0.6/fileformats/archive/converters.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,33 +54,27 @@
 @mark.converter(source_format=Compressed, target_format=Tar[Compressed])
 @mark.converter(
     source_format=Compressed, target_format=TarGzip[Compressed], compression="gz"
 )
 @pydra.mark.task
 @pydra.mark.annotate(
     {
-        "in_file": PathLike,
-        "out_file": str,
-        "filter": str,
-        "compression": str,  # TAR_COMPRESSION_ANNOT,
-        "format": int,
-        "ignore_zeros": bool,
         "return": {"out_file": Path},
     }
 )
 def create_tar(
-    in_file,
-    out_file=None,
-    base_dir=None,
-    filter=None,
-    compression=None,
-    format=tarfile.DEFAULT_FORMAT,
-    ignore_zeros=False,
-    encoding=tarfile.ENCODING,
-):
+    in_file: FileSet,
+    out_file: ty.Optional[Path] = None,
+    base_dir: ty.Optional[Path] = None,
+    filter: ty.Optional[str] = None,
+    compression: ty.Optional[str] = None,
+    format: int = tarfile.DEFAULT_FORMAT,
+    ignore_zeros: bool = False,
+    encoding: str = tarfile.ENCODING,
+) -> Path:
     return _create_tar(
         in_file=in_file,
         out_file=out_file,
         base_dir=base_dir,
         filter=filter,
         compression=compression,
         format=format,
@@ -166,16 +160,16 @@
 @mark.converter(source_format=Tar, target_format=FsObject)
 @mark.converter(source_format=TarGzip, target_format=FsObject)
 @mark.converter(source_format=Tar[Compressed], target_format=Compressed)
 @mark.converter(source_format=TarGzip[Compressed], target_format=Compressed)
 @pydra.mark.task
 @pydra.mark.annotate({"return": {"out_file": pydra.engine.specs.MultiOutputObj}})
 def extract_tar(
-    in_file: PathLike,
-    extract_dir: PathLike,
+    in_file: FileSet,
+    extract_dir: Path,
     bufsize: int = 10240,
     compression_type: str = "*",
 ) -> ty.Iterable[Path]:
 
     if extract_dir == attrs.NOTHING:
         extract_dir = tempfile.mkdtemp()
     else:
@@ -193,29 +187,25 @@
 
 
 @mark.converter(source_format=FsObject, target_format=Zip)
 @mark.converter(source_format=Compressed, target_format=Zip[Compressed])
 @pydra.mark.task
 @pydra.mark.annotate(
     {
-        "in_file": PathLike,
-        "out_file": str,
-        "compression": int,  # ZIP_COMPRESSION_ANNOT,
-        "allowZip64": bool,
         "return": {"out_file": PathLike},
     }
 )
 def create_zip(
-    in_file,
-    out_file,
-    base_dir,
-    compression=zipfile.ZIP_DEFLATED,
-    allowZip64=True,
-    compresslevel=None,
-    strict_timestamps=True,
+    in_file: FileSet,
+    out_file: Path,
+    base_dir: Path,
+    compression: int = zipfile.ZIP_DEFLATED,
+    allowZip64: bool = True,
+    compresslevel: ty.Optional[int] = None,
+    strict_timestamps: bool = True,
 ):
     return _create_zip(
         in_file=in_file,
         out_file=out_file,
         base_dir=base_dir,
         compression=compression,
         allowZip64=allowZip64,
```

### Comparing `fileformats-0.5.2/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6/fileformats/archive/tests/test_archive_converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 def test_tar_gz_roundtrip(archive_input):
     _roundtrip(archive_input, TarGzip)
 
 
 def _roundtrip(input, archive_klass):
     archive_klass.convert(input)  # test generic archive
-    # Create qualified archive that can be reversed
+    # Create classified archive that can be reversed
     compressed_type = Directory if input.is_dir else PlainText
     archive = archive_klass[compressed_type].convert(input)
     assert isinstance(archive, archive_klass)
     output = compressed_type.convert(archive)
     if isinstance(input, File):
         assert filecmp.cmp(output.fspath, input.fspath)
     else:
```

### Comparing `fileformats-0.5.2/fileformats/audio/__init__.py` & `fileformats-0.6/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/base.py` & `fileformats-0.6/fileformats/core/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+from __future__ import annotations
 import os
 from copy import copy
+import struct
 from inspect import isclass
 from warnings import warn
 import traceback
 import typing as ty
 import importlib
 import shutil
 from operator import itemgetter
 import itertools
+import functools
 from pathlib import Path
 import hashlib
 import logging
 import attrs
 from .utils import (
     subpackages,
     classproperty,
     fspaths_converter,
     to_mime_format_name,
     from_mime_format_name,
     STANDARD_NAMESPACES,
-    hash_file,
-    hash_dir,
     add_exc_note,
     describe_task,
 )
 from .converter import SubtypeVar
 from .exceptions import (
     FileFormatsError,
     FormatMismatchError,
@@ -33,14 +34,16 @@
 )
 
 # Tools imported from Arcana, will remove again once file-formats and "cells"
 # have been split
 REQUIRED_ANNOTATION = "__fileformats_required__"
 CHECK_ANNOTATION = "__fileformats_check__"
 
+FILE_CHUNK_LEN_DEFAULT = 8192
+
 
 logger = logging.getLogger("fileformats")
 
 
 class DataType:
     is_fileset = False
     is_field = False
@@ -73,16 +76,16 @@
 
     @classmethod
     def issubtype(cls, super_type: type, allow_same: bool = True):
         """Check to see whether datatype class is a subtype of a given super class.
         In this case the subtype is expected to be able to be treated as if it was
         the super class.
 
-        Overridden in the ``WithQualifiers`` mixin to add support for
-        qualified subtypes
+        Overridden in the ``WithClassifiers`` mixin to add support for
+        classified subtypes
 
         Parameters
         ----------
         super_type : type
             the class to check whether the given class is a subtype of
         allow_same : bool, optional
             whether there is a match if the classes are the same, by default True
@@ -120,14 +123,23 @@
         """Iterate over all installed subclasses"""
         for subpkg in subpackages():
             for attr_name in dir(subpkg):
                 attr = getattr(subpkg, attr_name)
                 if isclass(attr) and issubclass(attr, cls):
                     yield attr
 
+    @classmethod
+    def get_converter(cls, source_format: type, name: str = "converter", **kwargs):
+        if source_format.issubtype(cls):
+            return None
+        else:
+            raise FormatConversionError(
+                f"Cannot converter between '{cls.mime_like}' and '{source_format.mime_like}'"
+            )
+
     @classproperty
     def mime_like(cls):
         """Generates a "MIME-like" identifier from a format class (i.e.
         an identifier for a non-MIME class in the MIME style), e.g.
 
             fileformats.text.Plain to "text/plain"
 
@@ -179,15 +191,20 @@
             MIME identifier
 
         Returns
         -------
         type
             the corresponding file format class
         """
-        namespace, format_name = mime_string.split("/")
+        try:
+            namespace, format_name = mime_string.split("/")
+        except ValueError:
+            raise FormatRecognitionError(
+                f"Format '{mime_string}' is not a valid MIME-like format of <namespace>/<format>"
+            )
         try:
             return FileSet.formats_by_iana_mime[mime_string]
         except KeyError:
             pass
         if namespace == "application":
             # We treat the "application" namespace as a catch-all for any formats that are
             # not explicitly covered by the IANA standard (which is kind of how the IANA
@@ -230,43 +247,43 @@
                     f"try installing the namespace package with "
                     f"'python3 -m pip install fileformats-{namespace}'."
                 ) from None
             try:
                 klass = getattr(module, class_name)
             except AttributeError:
                 if "+" in format_name:
-                    qualifier_names, qualified_name = format_name.split("+")
+                    qualifier_names, classified_name = format_name.split("+")
                     try:
-                        qualifiers = [
+                        classifiers = [
                             getattr(module, from_mime_format_name(q))
                             for q in qualifier_names.split(".")
                         ]
                     except AttributeError:
                         raise FormatRecognitionError(
-                            f"Could not load qualifiers [{qualifier_names}] from "
+                            f"Could not load classifiers [{qualifier_names}] from "
                             f"fileformats.{namespace}, corresponding to MIME, "
                             f"or MIME-like, type {mime_string}"
                         ) from None
                     try:
-                        qualified = getattr(
-                            module, from_mime_format_name(qualified_name)
+                        classified = getattr(
+                            module, from_mime_format_name(classified_name)
                         )
                     except AttributeError:
                         try:
-                            qualified = cls.generically_qualifies_by_name[
-                                qualified_name
+                            classified = cls.generically_qualifies_by_name[
+                                classified_name
                             ]
                         except KeyError:
                             raise FormatRecognitionError(
-                                f"Could not load qualified class '{qualified_name}' from "
+                                f"Could not load classified class '{classified_name}' from "
                                 f"fileformats.{namespace} or list of generic types "
                                 f"({list(cls.generically_qualifies_by_name)}), "
                                 f"corresponding to MIME, or MIME-like, type {mime_string}"
                             ) from None
-                    klass = qualified[qualifiers]
+                    klass = classified[classifiers]
                 else:
                     raise FormatRecognitionError(
                         f"Did not find '{class_name}' class in fileformats.{namespace} "
                         f"corresponding to MIME, or MIME-like, type {mime_string}"
                     ) from None
         return klass
 
@@ -276,15 +293,15 @@
             cls._generically_qualifies_by_name = {
                 to_mime_format_name(f.__name__): f
                 for f in FileSet.all_formats
                 if getattr(f, "generically_qualifies", False)
             }
         return cls._generically_qualifies_by_name
 
-    _generically_qualifies_by_name = None  # Register all generically qualified types
+    _generically_qualifies_by_name = None  # Register all generically classified types
 
 
 @attrs.define
 class FileSet(DataType):
     """
     The base class for all format types within the fileformats package. A generic
     representation of a collection of files related to a single data resource. A
@@ -319,14 +336,17 @@
     converters = {}
 
     is_fileset = True
 
     def __hash__(self):
         return hash(sorted(self.fspaths))
 
+    def __repr__(self):
+        return f"{type(self).__name__}('" + "', '".join(self.fspaths) + "')"
+
     def __attrs_post_init__(self):
         # Check required properties don't raise errors
         for prop_name in self.required_properties():
             getattr(self, prop_name)
         # Loop through all attributes and find methods marked by CHECK_ANNOTATION
         for check in self.checks():
             getattr(self, check)()
@@ -452,47 +472,68 @@
                 pass
             else:
                 yield attr_name
 
     def copy_to(
         self,
         dest_dir: Path,
-        stem: str = None,
-        symlink: bool = False,
+        stem: ty.Optional[str] = None,
+        link_type: ty.Optional[str] = None,
         trim: bool = True,
         make_dirs: bool = False,
         overwrite: bool = False,
     ):
         """Copies the file-set to a new directory, optionally renaming the files
         to have consistent name-stems.
 
         Parameters
         ----------
         dest_dir : str
             Path to the parent directory to save the file-set
         stem: str, optional
             the file name excluding file extensions, to give the files/dirs in the parent
             directory, by default the original file name is used
-        symlink : bool, optional
-            Use symbolic links instead of copying files to new location, false by default
+        link_type : str, optional
+            Whether to use hard ('hard') or symbolic ('symbolic') links instead of
+            copying files to the new location. If None then the files are copied,
+            None by default.
         trim : bool, optional
-            Only copy the paths in the file-set that are "required" by the format, true by default
+            Only copy the paths in the file-set that are "required" by the format,
+            true by default
         make_dirs : bool, optional
-            Make the parent destination and all missing ancestors if they are missing, false by default
+            Make the parent destination and all missing ancestors if they are missing,
+            false by default
         overwrite : bool, optional
             whether to overwrite existing files/directories if present
         """
         dest_dir = Path(dest_dir)  # ensure a Path not a string
         if make_dirs:
             dest_dir.mkdir(parents=True, exist_ok=True)
-        if symlink:
-            copy_dir = copy_file = os.symlink
-        else:
+        if link_type is None:
             copy_dir = shutil.copytree
             copy_file = shutil.copyfile
+        elif link_type == "hard":
+            copy_file = os.link
+
+            def hardlink_dir(src: Path, dest: Path):
+                for dpath, _, fpaths in os.walk(src):
+                    dpath = Path(dpath)
+                    relpath = dpath.relative_to(src)
+                    (dest / relpath).mkdir()
+                    for fpath in fpaths:
+                        os.link(dpath / fpath, dest / relpath / fpath)
+
+            copy_dir = hardlink_dir
+        elif link_type == "symbolic":
+            copy_dir = copy_file = os.symlink
+        else:
+            raise FileFormatsError(
+                f"Unrecognised link_type option {link_type}, can be 'hard', 'symbolic' "
+                "or None"
+            )
         new_paths = []
         if trim and self.required_paths():
             fspaths_to_copy = self.required_paths()
         else:
             fspaths_to_copy = self.fspaths
         if not fspaths_to_copy:
             raise FileFormatsError(
@@ -519,15 +560,17 @@
             if fspath.is_dir():
                 copy_dir(fspath, new_path)
             else:
                 copy_file(fspath, new_path)
             new_paths.append(new_path)
         return type(self)(new_paths)
 
-    def select_by_ext(self, fileformat: type = None, allow_none: bool = False) -> Path:
+    def select_by_ext(
+        self, fileformat: ty.Optional[type] = None, allow_none: bool = False
+    ) -> Path:
         """Selects a single path from a set of file-system paths based on the file
         extension
 
         Parameters
         ----------
         fileformat : type
             the format class of the path to select
@@ -653,19 +696,19 @@
             return None
         converters = (
             cls.get_converters_dict()
         )  # triggers loading of standard converters for target format
         # Ensure standard converters from source format are loaded
         source_format.import_standard_converters()
         try:
-            unqualified = source_format.unqualified
+            unclassified = source_format.unclassified
         except AttributeError:
             pass
         else:
-            unqualified.import_standard_converters()
+            unclassified.import_standard_converters()
         try:
             converter_tuple = converters[source_format]
         except KeyError:
             # If no direct mapping check for mapping from source super types and wildcard
             # matches
             available_converters = cls.get_converter_tuples(source_format)
             if len(available_converters) > 1:
@@ -747,28 +790,28 @@
         """
         converters_dict = cls.get_converters_dict()
         available = []
         for src_frmt, converter in converters_dict.items():
             if len(converter) == 2:  # Ignore converters with wildcards at this point
                 if source_format.issubtype(src_frmt):
                     available.append(converter)
-        if not available and hasattr(source_format, "unqualified"):
+        if not available and hasattr(source_format, "unclassified"):
             available = SubtypeVar.get_converter_tuples(
                 source_format, target_format=cls
             )
         return available
 
     @classmethod
     def register_converter(
         cls,
         source_format: type,
         converter_tuple: ty.Tuple[ty.Callable, ty.Dict[str, ty.Any]],
     ):
-        """Registers a converter task within a class attribute. Called by the @fileformats.mark.converter
-        decorator.
+        """Registers a converter task within a class attribute. Called by the
+        @fileformats.mark.converter decorator.
 
         Parameters
         ----------
         source_format : type
             the source format to register a converter from
         task_spec : ty.Callable
             a callable that resolves to a Pydra task
@@ -788,15 +831,15 @@
             raise FormatConversionError(
                 f"There is already a converter registered between {source_format.__name__} "
                 f"and {cls.__name__}: {describe_task(prev)}"
             )
         converters_dict[source_format] = converter_tuple
 
     @classproperty
-    def all_formats(cls):
+    def all_formats(cls) -> set:
         """Iterate over all FileSet formats in fileformats.* namespaces"""
         if cls._all_formats is None:
             cls._all_formats = set(
                 f for f in FileSet.subclasses() if f.__dict__.get("iana_mime", True)
             )
         return cls._all_formats
 
@@ -833,125 +876,231 @@
                         key=itemgetter(0),
                     ),
                     key=itemgetter(0),
                 )
             }
         return cls._formats_by_name
 
-    def hash_files(
+    @property
+    def all_file_paths(self) -> ty.Iterable[Path]:
+        """Paths of all files within the fileset"""
+        for fspath in self.fspaths:
+            if fspath.is_file():
+                yield fspath
+            else:
+                for dpath, _, file_paths in os.walk(fspath):
+                    for file_path in file_paths:
+                        yield Path(dpath) / file_path
+
+    def byte_chunks(
         self,
-        crypto=None,
-        chunk_len=8192,
-        relative_to: os.PathLike = None,
-        **kwargs,
-    ):
-        """Calculate hashes for all files within the file set within a dictionary.
-        Hashes for files within directories are nested within separate dictionaries
-        for each (sub)directory.
+        mtime: bool = False,
+        chunk_len=FILE_CHUNK_LEN_DEFAULT,
+        relative_to: ty.Optional[os.PathLike] = None,
+        ignore_hidden_files: bool = False,
+        ignore_hidden_dirs: bool = False,
+    ) -> ty.Generator[str, ty.Generator[bytes]]:
+        """Yields relative paths for all files within the file-set along with iterators
+        over their byte-contents. To be used when generating hashes for the file set.
 
         Parameters
         ----------
-        crypto : function, optional
-            the cryptography method used to hash the files, by default hashlib.sha256
+        mtime : bool, optional
+            instead of iterating over the entire contents of the file-set, simply yield
+            a bytes repr of the last modification time.
         chunk_len : int, optional
             the chunk length to break up the file and calculate the hash over, by default 8192
         relative_to : Path, optional
             the base path by which to record the file system paths in the dictionary keys
             to, by default None
-        **kwargs
-            keyword args passed directly through to the ``hash_dir`` function
+        ignore_hidden_files : bool
+            whether to ignore hidden files within nested directories (i.e. those
+            starting with '.')
+        ignore_hidden_dirs : bool
+            whether to ignore hidden directories within nested directories (i.e. those
+            starting with '.')
 
-        Returns
+        Yields
         -------
-        file_hashes : dict[str, str]
-            hashes for all files in the file-set, addressed by their directory relative
-            to the ``relative_to`` path
+        rel_path: str
+            relative path to either 'relative_to' arg or common base path for each file
+            in the file set
+        byte_iter : Generator[bytes]
+            an iterator over the bytes contents of the file, chunked into 'chunk_len'
+            chunks
         """
+        # If "relative_to" is not provided, get the common path between
         if relative_to is None:
             relative_to = Path(os.path.commonpath(self.fspaths))
             if all(p.is_file() and p.parent == relative_to for p in self.fspaths):
                 relative_to /= os.path.commonprefix(
                     [p.name for p in self.fspaths]
                 ).rstrip(".")
+        # yield the absolute base path if using mtimes instead of contents
+        if mtime:
+            yield ("<base-path>", iter([str(relative_to.absolute()).encode()]))
+
         relative_to = str(relative_to)
         if Path(relative_to).is_dir() and not relative_to.endswith(os.path.sep):
             relative_to += os.path.sep
-        if crypto is None:
-            crypto = hashlib.sha256
 
-        file_hashes = {}
+        if mtime:
+
+            def chunk_file(fspath: Path):
+                """Yields a byte representation of the last modified time for the file"""
+                yield bytes(struct.pack("<d", os.stat(fspath).st_mtime))
+
+        else:
+
+            def chunk_file(fspath: Path):
+                """Yields the contents of the file in byte chunks"""
+                if not fspath.is_file():
+                    assert fspath.is_symlink()  # broken symlink
+                    yield b"\x00"
+                else:
+                    with open(fspath, "rb") as fp:
+                        for chunk in iter(functools.partial(fp.read, chunk_len), b""):
+                            yield chunk
+
+        def chunk_dir(fspath):
+            for dpath, _, filenames in sorted(os.walk(fspath)):
+                # Sort in-place to guarantee order.
+                filenames.sort()
+                dpath = Path(dpath)
+                if (
+                    ignore_hidden_dirs
+                    and dpath.name.startswith(".")
+                    and str(dpath) != fspath
+                ):
+                    continue
+                for filename in filenames:
+                    if ignore_hidden_files and filename.startswith("."):
+                        continue
+                    yield (
+                        str((dpath / filename).relative_to(relative_to)),
+                        chunk_file(dpath / filename),
+                    )
+
         for key, fspath in sorted(
             ((str(p)[len(relative_to) :], p) for p in self.fspaths),
             key=itemgetter(0),
         ):
-            if fspath.is_file():
-                file_hashes[key] = hash_file(fspath, chunk_len=chunk_len, crypto=crypto)
-            elif fspath.is_dir():
-                file_hashes.update(
-                    hash_dir(
-                        fspath,
-                        chunk_len=chunk_len,
-                        crypto=crypto,
-                        relative_to=relative_to,
-                        **kwargs,
-                    )
-                )
+            if fspath.is_dir():
+                yield from chunk_dir(fspath)
             else:
-                raise RuntimeError(f"Cannot hash {self} as {fspath} no longer exists")
-        return file_hashes
+                yield (key, chunk_file(fspath))
 
-    def hash(self, crypto=None, *args, **kwargs):
+    def hash(self, crypto=None, **kwargs) -> bytes:
         """Calculate a unique hash for the file-set based on the relative paths and
         contents of its constituent files
 
         Parameters
         ----------
         crypto : function, optional
             the cryptography method used to hash the files, by default hashlib.sha256
-        chunk_len : int, optional
-            the chunk length to break up the file and calculate the hash over, by default 8192
-        relative_to : Path, optional
-            the base path by which to record the file system paths in the dictionary keys
-            to, by default None
         **kwargs
             keyword args passed directly through to the ``hash_dir`` function
 
         Returns
         -------
         hash : str
             unique hash for the file-set
         """
         if crypto is None:
             crypto = hashlib.sha256
         crytpo_obj = crypto()
-        for path, hash in self.hash_files(crypto=crypto, *args, **kwargs).items():
+        for path, bytes_iter in self.byte_chunks(**kwargs):
             crytpo_obj.update(path.encode())
-            crytpo_obj.update(hash.encode())
+            for bytes_str in bytes_iter:
+                crytpo_obj.update(bytes_str)
         return crytpo_obj.hexdigest()
 
+    def hash_files(self, crypto=None, **kwargs) -> dict[str, bytes]:
+        """Calculate hashes for all files in the file-set based on the relative paths and
+        contents of its constituent files
+
+        Parameters
+        ----------
+        crypto : function, optional
+            the cryptography method used to hash the files, by default hashlib.sha256
+        **kwargs
+            keyword args passed directly through to the ``hash_dir`` function
+
+        Returns
+        -------
+        file_hashes : dict[str, bytes]
+            unique hashes for each file in the file-set
+        """
+        if crypto is None:
+            crypto = hashlib.sha256
+        file_hashes = {}
+        for path, bytes_iter in self.byte_chunks(**kwargs):
+            crypto_obj = crypto()
+            for bytes_str in bytes_iter:
+                crypto_obj.update(bytes_str)
+            file_hashes[str(path)] = crypto_obj.hexdigest()
+        return file_hashes
+
+    def __bytes_repr__(self, cache, mode=None):  # pylint: disable=unused-argument
+        """Provided for compatibility with Pydra's hashing function, return the contents
+        of all the files in the file-set in chunks
+
+        Parameters
+        ----------
+        cache : pydra.utils.hash.Cache
+            an object passed around by Pydra's hashing function to store cached versions
+            of previously hashed objects, to allow recursive structures
+        mode : int, optional
+            a flag used to specify the mode used to generate the bytes representation
+
+        Yields
+        ------
+        bytes
+            a chunk of bytes of length FILE_CHUNK_LEN_DEFAULT from the contents of all
+            files in the file-set.
+        """
+        cls = type(self)
+        yield f"{cls.__module__}.{cls.__name__}:".encode()
+        for key, chunk_iter in self.byte_chunks():
+            yield (",'" + key + "'=").encode()
+            yield from chunk_iter
+
     _all_formats = None
     _formats_by_iana_mime = None
     _formats_by_name = None
 
 
 @attrs.define
 class Field(DataType):
     value = attrs.field()
 
     type = None
     is_field = True
+    primitive = None
 
     def __str__(self):
         return str(self.value)
 
     @property
     def metadata(self):
         return {}
 
     @classproperty
-    def all_fields(cls):
+    def all_fields(cls) -> list[ty.Type[Field]]:  # pylint: disable=no-self-argument
         """Iterate over all field formats in fileformats.* namespaces"""
-        if cls._all_fields is None:
-            cls._all_fields = [f for f in Field.subclasses() if f.type is not None]
-        return cls._all_fields
+        import fileformats.field  # noqa
+
+        return [f for f in Field.subclasses() if f.primitive is not None]
+
+    @classmethod
+    def from_primitive(cls, dtype: type):
+        try:
+            datatype = next(iter(f for f in cls.all_fields if f.primitive is dtype))
+        except StopIteration as e:
+            field_types_str = ", ".join(t.__name__ for t in cls.all_fields)
+            raise FileFormatsError(
+                f"{dtype} doesn't not correspond to a valid fileformats field type "
+                f"({field_types_str})"
+            ) from e
+        return datatype
 
     _all_fields = None
```

### Comparing `fileformats-0.5.2/fileformats/core/converter.py` & `fileformats-0.6/fileformats/core/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 @attrs.define
 class ConverterWrapper:
     """Wraps a converter task in a workflow so that the in_file and out_file names can
     be mapped onto their standardised names, "in_file" and "out_file" if necessary
     """
 
     task_spec: ty.Callable
-    in_file: str = None
-    out_file: str = None
+    in_file: ty.Optional[str] = None
+    out_file: ty.Optional[str] = None
 
     def __call__(self, name=None, **kwargs):
         from pydra.engine import Workflow
 
         if name is None:
             name = f"{self.task_spec.__name__}_wrapper"
         wf = Workflow(
@@ -59,16 +59,16 @@
         return self.name
 
     def issubtype(self, super_type: type, allow_same: bool = True):
         """Check to see whether datatype class is a subtype of a given super class.
         In this case the subtype is expected to be able to be treated as if it was
         the super class.
 
-        Overridden in the ``WithQualifiers`` mixin to add support for
-        qualified subtypes
+        Overridden in the ``WithClassifiers`` mixin to add support for
+        classified subtypes
 
         Parameters
         ----------
         super_type : type
             the class to check whether the given class is a subtype of
         allow_same : bool, optional
             whether there is a match if the classes are the same, by default True
@@ -84,26 +84,26 @@
     @classmethod
     def get_converter_tuples(
         cls, source_format: type, target_format: type
     ) -> ty.List[ty.Tuple[ty.Callable, ty.Dict[str, ty.Any]]]:
         # check to see whether there are converters from a base class of the source
         # format
         available_converters = []
-        if source_format.is_qualified:
+        if source_format.is_classified:
             for template_source_format, converter in cls.converters.items():
-                if not template_source_format.unqualified.issubtype(
-                    source_format.unqualified
+                if not template_source_format.unclassified.issubtype(
+                    source_format.unclassified
                 ):
                     continue
-                assert len(template_source_format.wildcard_qualifiers()) == 1
-                non_wildcards = template_source_format.non_wildcard_qualifiers()
-                if not non_wildcards.issubset(source_format.qualifiers):
+                assert len(template_source_format.wildcard_classifiers()) == 1
+                non_wildcards = template_source_format.non_wildcard_classifiers()
+                if not non_wildcards.issubset(source_format.classifiers):
                     continue
                 from_types = tuple(
-                    set(source_format.qualifiers).difference(non_wildcards)
+                    set(source_format.classifiers).difference(non_wildcards)
                 )
                 if any(q.issubtype(target_format) for q in from_types):
                     available_converters.append(converter)
         return available_converters
 
     @classmethod
     def register_converter(
@@ -126,32 +126,32 @@
 
         Raises
         ------
         FormatConversionError
             if there is already a converter registered between the two types
         """
         # Ensure "converters" dict is defined in the target class and not in a superclass
-        if len(source_format.wildcard_qualifiers()) > 1:
+        if len(source_format.wildcard_classifiers()) > 1:
             raise FileFormatsError(
                 "Cannot register a conversion to a generic type from a type with more "
-                f"than one wildcard {source_format} ({list(source_format.wildcard_qualifiers())})"
+                f"than one wildcard {source_format} ({list(source_format.wildcard_classifiers())})"
             )
         prev_registered = [
             f
             for f in cls.converters
             if (
-                f.unqualified is source_format.unqualified
-                and f.non_wildcard_qualifiers()
-                == source_format.non_wildcard_qualifiers()
+                f.unclassified is source_format.unclassified
+                and f.non_wildcard_classifiers()
+                == source_format.non_wildcard_classifiers()
             )
         ]
         assert len(prev_registered) <= 1
         if prev_registered:
             prev = prev_registered[0]
             prev_task = cls.converters[prev][0]
             raise FileFormatsError(
                 f"There is already a converter registered from {prev} "
-                f"to the generic type '{tuple(prev.wildcard_qualifiers())[0]}':"
+                f"to the generic type '{tuple(prev.wildcard_classifiers())[0]}':"
                 f"{describe_task(prev_task)}"
             )
 
         cls.converters[source_format] = converter_tuple
```

### Comparing `fileformats-0.5.2/fileformats/core/mark.py` & `fileformats-0.6/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/mixin.py` & `fileformats-0.6/fileformats/core/mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         if the file-format is a binary type then this flag needs to be set in order to
         read the contents properly
     magic_number_offset : int, optional
         the offset in bytes from the start of the file that the magic number is stored
     """
 
     magic_number_offset = 0
+    binary: bool
+    magic_number: ty.Union[str, int]
 
     @mark.check
     def check_magic_number(self):
         if self.binary and isinstance(self.magic_number, str):
             magic_bytes = bytes.fromhex(self.magic_number)
         else:
             magic_bytes = self.magic_number
@@ -66,31 +68,32 @@
     post_init_super : type
         the format class the WithAdjacentFiles mixin is mixed with that defines the
         __attrs_post_init__ method that should be called once the adjacent files
         are added to the self.fspaths attribute to run checks.
     """
 
     post_init_super = FileSet
+    fspaths: ty.FrozenSet[Path]
 
     def __attrs_post_init__(self):
         if len(self.fspaths) == 1:
             self.fspaths |= self.get_adjacent_files()
             trim = True
         else:
             trim = False
         self.post_init_super.__attrs_post_init__(self)
         if trim:
             self.trim_paths()
 
     def get_adjacent_files(self) -> ty.Set[Path]:
-        stem = self.stem
+        stem = self.stem  # pylint: disable=no-member
         adjacents = set()
-        for sibling in self.fspath.parent.iterdir():
+        for sibling in self.fspath.parent.iterdir():  # pylint: disable=no-member
             if (
-                sibling != self.fspath
+                sibling != self.fspath  # pylint: disable=no-member
                 and sibling.is_file()
                 and sibling.name.startswith(stem + ".")
             ):
                 adjacents.add(sibling)
         return adjacents
 
 
@@ -157,15 +160,15 @@
             else:
                 metadata[
                     to_mime_format_name(type(side_car).__name__)
                 ] = side_car_metadata
         return metadata
 
 
-class WithQualifiers:
+class WithClassifiers:
     """Mixin class for adding the ability to qualify the format class to designate the
     type of information stored within the format, e.g. ``DirectoryContaining[Png, Gif]`` for a
     directory containing PNG and GIF files, ``Zip[DataFile]`` for a zipped data file,
     ``Array[Integer]`` for an array containing integers, or DicomDir[T1w, Brain] for a
     T1-weighted MRI scan of the brain in DICOM format.
 
         class MyFormatWithContents(WithContents, File):
@@ -177,218 +180,226 @@
             ...
 
     A unique class will be returned (i.e. multiple calls with the same arguments will
     return the same class)
 
     Class Attrs
     -----------
-    qualifiers_attr_name : str, optional
-        an attribute name to store the qualifiers at within the qualified class. This
-        should be used if you need to reference the ``qualifiers`` attribute directly
+    classifiers_attr_name : str, optional
+        an attribute name to store the classifiers at within the classified class. This
+        should be used if you need to reference the ``classifiers`` attribute directly
         in any validation/other methods (i.e. in most cases), to handle the case of
-        diamond inheritance between two classes that can be qualified.
-        A default value should also be set in the unqualified base for this attribute,
-        which is either ``()`` if ``multiple_qualifiers`` is true and ``None`` otherwise
-    <qualifiers-attr-name> : tuple[type, ...] or None, optional
-        pass a default value to the attribute referenced by 'qualifiers_attr_name'
-    multiple_qualifiers : bool, optional
+        diamond inheritance between two classes that can be classified.
+        A default value should also be set in the unclassified base for this attribute,
+        which is either ``()`` if ``multiple_classifiers`` is true and ``None`` otherwise
+    <classifiers-attr-name> : tuple[type, ...] or None, optional
+        pass a default value to the attribute referenced by 'classifiers_attr_name'
+    multiple_classifiers : bool, optional
         whether or not multiple content types are permitted for the container type, True
-    allowed_qualifiers : tuple[type,...], optional
+    allowed_classifiers : tuple[type,...], optional
         the allowable types (+ subclasses) for the content types. If None all types
         are allowed
-    ordered_qualifiers : bool, optional
+    ordered_classifiers : bool, optional
         whether the order of the content types is important or not, by default false
-    genericly_qualified : bool, optional
-        whether the class can be qualified by qualifiers in any namespace (true) or just the
+    genericly_classified : bool, optional
+        whether the class can be classified by classifiers in any namespace (true) or just the
         namespace it belongs to (false). If true, then the namespace of the genericly
-        qualified class is omitted from the "mime-like" string. Note that the
+        classified class is omitted from the "mime-like" string. Note that the
         class' name therefore needs to be globally unique amongst all other genericly
-        qualified classes and so it should be used sparingly, i.e., highly generic
+        classified classes and so it should be used sparingly, i.e., highly generic
         formats that are unambiguous across all namespaces, such as "directory", "zip",
         "gzip", "json", "yaml", etc...
     """
 
-    qualifiers = ()  # qualifiers set in the current class
-    _qualified_subtypes = {}
-    # dict of previously created qualified subtypes. If an existing class with matching
-    # qualifiers has been created it is returned instead of creating a new type. This
+    classifiers = ()  # classifiers set in the current class
+    _classified_subtypes = {}
+    # dict of previously created classified subtypes. If an existing class with matching
+    # classifiers has been created it is returned instead of creating a new type. This
     # ensures that ``assert MyFormat[Qualifier] is MyFormat[Qualifier]``
 
     # Default values for class attrs
-    multiple_qualifiers = True
-    allowed_qualifiers = None
-    ordered_qualifiers = False
+    multiple_classifiers = True
+    allowed_classifiers: ty.Optional[ty.Tuple[ty.Type[ty.Any]]] = None
+    ordered_classifiers = False
     generically_qualifies = False
 
     def __attrs_pre_init__(self):
-        if self.wildcard_qualifiers():
+        if self.wildcard_classifiers():
             raise FileFormatsError(
-                f"Can instantiate {type(self)} class as it has wildcard qualifiers "
+                f"Can instantiate {type(self)} class as it has wildcard classifiers "
                 "and therefore should only be used for converter specifications"
             )
 
     @classproperty
-    def is_qualified(cls):
-        return "unqualified" in cls.__dict__
+    def is_classified(cls):  # pylint: disable=no-self-argument
+        return "unclassified" in cls.__dict__
 
     @classmethod
-    def wildcard_qualifiers(cls, qualifiers=None):
-        if qualifiers is None:
-            qualifiers = cls.qualifiers if cls.is_qualified else ()
-        return frozenset(t for t in qualifiers if isinstance(t, SubtypeVar))
+    def wildcard_classifiers(cls, classifiers=None):
+        if classifiers is None:
+            classifiers = cls.classifiers if cls.is_classified else ()
+        return frozenset(t for t in classifiers if isinstance(t, SubtypeVar))
 
     @classmethod
-    def non_wildcard_qualifiers(cls, qualifiers=None):
-        if qualifiers is None:
-            qualifiers = cls.qualifiers if cls.is_qualified else ()
-        return frozenset(q for q in qualifiers if not isinstance(q, SubtypeVar))
+    def non_wildcard_classifiers(cls, classifiers=None):
+        if classifiers is None:
+            classifiers = cls.classifiers if cls.is_classified else ()
+        return frozenset(q for q in classifiers if not isinstance(q, SubtypeVar))
 
     @classmethod
-    def __class_getitem__(cls, qualifiers):
+    def __class_getitem__(cls, classifiers):
         """Set the content types for a newly created dynamically type"""
-        if isinstance(qualifiers, ty.Iterable):
-            qualifiers = tuple(qualifiers)
+        if isinstance(classifiers, ty.Iterable):
+            classifiers = tuple(classifiers)
         else:
-            qualifiers = (qualifiers,)
-        if cls.allowed_qualifiers:
+            classifiers = (classifiers,)
+        if cls.allowed_classifiers:
             not_allowed = [
                 q
-                for q in qualifiers
-                if not any(q.issubtype(t) for t in cls.allowed_qualifiers)
+                for q in classifiers
+                if not any(q.issubtype(t) for t in cls.allowed_classifiers)
             ]
             if not_allowed:
                 raise FileFormatsError(
                     f"Invalid content types provided to {cls} (must be subclasses of "
-                    f"{cls.allowed_qualifiers}): {not_allowed}"
+                    f"{cls.allowed_classifiers}): {not_allowed}"
                 )
         # Sort content types if order isn't important
-        if cls.multiple_qualifiers:
-            if not cls.ordered_qualifiers:
-                # TODO: should check to see if qualifiers are subclasses of each other
-                repetitions = [t for t, c in Counter(qualifiers).items() if c > 1]
+        if cls.multiple_classifiers:
+            if not cls.ordered_classifiers:
+                # TODO: should check to see if classifiers are subclasses of each other
+                repetitions = [t for t, c in Counter(classifiers).items() if c > 1]
                 if repetitions:
                     raise FileFormatsError(
                         f"Cannot have more than one occurrence of a qualifier "
                         f"({repetitions}) for {cls} class when "
-                        f"{cls.__name__}.ordered_qualifiers is false"
+                        f"{cls.__name__}.ordered_classifiers is false"
                     )
-                qualifiers = frozenset(qualifiers)
+                classifiers = frozenset(classifiers)
         else:
-            if len(qualifiers) > 1:
+            if len(classifiers) > 1:
                 raise FileFormatsError(
-                    f"Multiple qualifiers not permitted for {cls} types, provided: ({qualifiers})"
+                    f"Multiple classifiers not permitted for {cls} types, provided: ({classifiers})"
                 )
-        # Make sure that the "qualified" dictionary is present in this class not super
+        # Make sure that the "classified" dictionary is present in this class not super
         # classes
-        if "_qualified_subtypes" not in cls.__dict__:
-            cls._qualified_subtypes = {}
+        if "_classified_subtypes" not in cls.__dict__:
+            cls._classified_subtypes = {}
         try:
             # Load previously created type so we can do ``assert MyType[Integer] is MyType[Integer]``
-            qualified = cls._qualified_subtypes[qualifiers]
+            classified = cls._classified_subtypes[classifiers]
         except KeyError:
-            if not hasattr(cls, "qualifiers_attr_name"):
+            if not hasattr(cls, "classifiers_attr_name"):
                 raise FileFormatsError(
-                    f"{cls} needs to define the 'qualifiers_attr_name' class attribute "
+                    f"{cls} needs to define the 'classifiers_attr_name' class attribute "
                     "with the name of the (different) class attribute to hold the "
-                    "qualified types"
+                    "classified types"
                 )
-            if cls.qualifiers_attr_name is None:
+            if cls.classifiers_attr_name is None:
                 raise FileFormatsError(
-                    f"Inherited qualifiers have been disabled in {cls} (by setting "
-                    f'"qualifiers_attr_name)" to None)'
+                    f"Inherited classifiers have been disabled in {cls} (by setting "
+                    f'"classifiers_attr_name)" to None)'
                 )
             try:
-                qualifiers_attr = getattr(cls, cls.qualifiers_attr_name)
+                classifiers_attr = getattr(cls, cls.classifiers_attr_name)
             except AttributeError:
                 raise FileFormatsError(
-                    f"Default value for qualifiers attribute "
-                    f"'{cls.qualifiers_attr_name}' needs to be set in {cls}"
+                    f"Default value for classifiers attribute "
+                    f"'{cls.classifiers_attr_name}' needs to be set in {cls}"
                 )
             else:
-                if qualifiers_attr:
+                if classifiers_attr:
                     raise FileFormatsError(
-                        f"Default value for qualifiers attribute "
-                        f"'{cls.qualifiers_attr_name}' needs to be set in {cls}"
+                        f"Default value for classifiers attribute "
+                        f"'{cls.classifiers_attr_name}' needs to be set in {cls}"
                     )
             class_attrs = {
-                "unqualified": cls,
-                "qualifiers": qualifiers,
+                "unclassified": cls,
+                "classifiers": classifiers,
             }
-            class_attrs[cls.qualifiers_attr_name] = (
-                qualifiers if cls.multiple_qualifiers else qualifiers[0]
+            class_attrs[cls.classifiers_attr_name] = (
+                classifiers if cls.multiple_classifiers else classifiers[0]
             )
-            qualifier_names = [t.__name__ for t in qualifiers]
-            if not cls.ordered_qualifiers:
+            qualifier_names = [t.__name__ for t in classifiers]
+            if not cls.ordered_classifiers:
                 qualifier_names.sort()
-            qualified = type(
+            classified = type(
                 f"{'_'.join(qualifier_names)}__{cls.__name__}",
                 (cls,),
                 class_attrs,
             )
-            cls._qualified_subtypes[qualifiers] = qualified
-        return qualified
+            cls._classified_subtypes[classifiers] = classified
+        return classified
 
     @classmethod
     def get_converter_tuples(
         cls, source_format: type
     ) -> ty.List[ty.Tuple[ty.Callable, ty.Dict[str, ty.Any]]]:
         """Search the registered converters to find an appropriate task and associated
         key-word args to perform the conversion between source and target formats
 
         Parameters
         ----------
         source_format : type(FileSet)
             the source format to convert from
         """
         # Try to see if a converter has been defined to the exact type
-        available_converters = super().get_converter_tuples(source_format)
+        available_converters = super().get_converter_tuples(
+            source_format
+        )  # pylint: disable=no-member
         # Failing that, see if there is a generic conversion between the container type
         # the source format (or subclass of) defined with matching wildcards in the source
         # and target formats
-        if not available_converters and cls.is_qualified:
-            converters_dict = FileSet.get_converters_dict(cls.unqualified)
+        if not available_converters and cls.is_classified:
+            converters_dict = FileSet.get_converters_dict(
+                cls.unclassified
+            )  # pylint: disable=no-member
             for template_source_format, converter in converters_dict.items():
-                if len(converter) == 3:  # was defined with wildcard qualifiers
-                    converter, conv_kwargs, template_qualifiers = converter
+                if len(converter) == 3:  # was defined with wildcard classifiers
+                    converter, conv_kwargs, template_classifiers = converter
                     # Attempt conversion from generic type to template match
                     if isinstance(template_source_format, SubtypeVar):
-                        assert tuple(cls.wildcard_qualifiers(template_qualifiers)) == (
-                            template_source_format,
+                        assert tuple(
+                            cls.wildcard_classifiers(template_classifiers)
+                        ) == (template_source_format,)
+                        non_wildcards = cls.non_wildcard_classifiers(
+                            template_classifiers
                         )
-                        non_wildcards = cls.non_wildcard_qualifiers(template_qualifiers)
-                        to_match = tuple(set(cls.qualifiers).difference(non_wildcards))
+                        to_match = tuple(set(cls.classifiers).difference(non_wildcards))
                         if len(to_match) > 1:
                             wildcard_match = False
                         else:
                             wildcard_match = source_format.issubtype(to_match[0])
                     # Attempt template to template conversion match
                     elif getattr(
-                        source_format, "is_qualified", False
-                    ) and source_format.unqualified.issubtype(
-                        template_source_format.unqualified
+                        source_format, "is_classified", False
+                    ) and source_format.unclassified.issubtype(
+                        template_source_format.unclassified
                     ):
-                        assert cls.wildcard_qualifiers(
-                            template_qualifiers
-                        ) == cls.wildcard_qualifiers(template_source_format.qualifiers)
-                        if cls.ordered_qualifiers:
-                            if len(cls.qualifiers) != len(template_qualifiers) or len(
-                                source_format.qualifiers
-                            ) != len(template_source_format.qualifiers):
+                        assert cls.wildcard_classifiers(
+                            template_classifiers
+                        ) == cls.wildcard_classifiers(
+                            template_source_format.classifiers
+                        )
+                        if cls.ordered_classifiers:
+                            if len(cls.classifiers) != len(template_classifiers) or len(
+                                source_format.classifiers
+                            ) != len(template_source_format.classifiers):
                                 wildcard_match = False
                             else:
                                 wildcard_map = {}
                                 for actual, template in zip(
-                                    source_format.qualifiers,
-                                    template_source_format.qualifiers,
+                                    source_format.classifiers,
+                                    template_source_format.classifiers,
                                 ):
                                     if isinstance(template, SubtypeVar):
                                         wildcard_map[template] = actual
                                 wildcard_match = True
                                 for actual, template in zip(
-                                    cls.qualifiers, template_qualifiers
+                                    cls.classifiers, template_classifiers
                                 ):
                                     if isinstance(template, SubtypeVar):
                                         try:
                                             reference = wildcard_map[template]
                                         except KeyError:
                                             wildcard_match = False
                                             break
@@ -396,64 +407,68 @@
                                             if not actual.issubtype(reference):
                                                 wildcard_match = False
                                                 break
                                     elif not actual.issubtype(template):
                                         wildcard_match = False
                                         break
                         else:
-                            non_wildcards = cls.non_wildcard_qualifiers(
-                                template_qualifiers
+                            non_wildcards = cls.non_wildcard_classifiers(
+                                template_classifiers
                             )
-                            src_non_wildcards = cls.non_wildcard_qualifiers(
-                                template_source_format.qualifiers
+                            src_non_wildcards = cls.non_wildcard_classifiers(
+                                template_source_format.classifiers
                             )
                             if not non_wildcards.issubset(
-                                set(cls.qualifiers)
+                                set(cls.classifiers)
                             ) or not src_non_wildcards.issubset(
-                                set(source_format.qualifiers)
+                                set(source_format.classifiers)
                             ):
                                 wildcard_match = False
                             else:
-                                to_match = set(cls.qualifiers).difference(non_wildcards)
-                                from_types = set(source_format.qualifiers).difference(
+                                to_match = set(cls.classifiers).difference(
+                                    non_wildcards
+                                )
+                                from_types = set(source_format.classifiers).difference(
                                     src_non_wildcards
                                 )
                                 wildcard_match = to_match.issubset(from_types)
                     else:
                         wildcard_match = False
                     if wildcard_match:
                         available_converters.append((converter, conv_kwargs))
         return available_converters
 
     @classmethod
     def issubtype(cls, super_type: type):
-        if super().issubtype(super_type):
+        if super().issubtype(super_type):  # pylint: disable=no-member
             return True
-        # Check to see whether the unqualified types are equivalent
+        # Check to see whether the unclassified types are equivalent
         if (
-            not cls.is_qualified
-            or not getattr(super_type, "is_qualified", False)
-            or not cls.unqualified.issubtype(super_type.unqualified)
+            not cls.is_classified
+            or not getattr(super_type, "is_classified", False)
+            or not cls.unclassified.issubtype(
+                super_type.unclassified
+            )  # pylint: disable=no-member
         ):
             return False
-        if cls.ordered_qualifiers:
-            if len(cls.qualifiers) != len(super_type.qualifiers):
+        if cls.ordered_classifiers:
+            if len(cls.classifiers) != len(super_type.classifiers):
                 is_subtype = False
             else:
                 is_subtype = all(
                     q.issubtype(s)
-                    for q, s in zip(cls.qualifiers, super_type.qualifiers)
+                    for q, s in zip(cls.classifiers, super_type.classifiers)
                 )
         else:
-            if super_type.qualifiers.issubset(cls.qualifiers):
+            if super_type.classifiers.issubset(cls.classifiers):
                 is_subtype = True
             else:
                 is_subtype = all(
-                    any(q.issubtype(s) for q in cls.qualifiers)
-                    for s in super_type.qualifiers
+                    any(q.issubtype(s) for q in cls.classifiers)
+                    for s in super_type.classifiers
                 )
         return is_subtype
 
     @classmethod
     def register_converter(
         cls,
         source_format: type,
@@ -474,72 +489,72 @@
 
         Raises
         ------
         FormatConversionError
             if there is already a converter registered between the two types
         """
         # Ensure "converters" dict is defined in the target class and not in a superclass
-        if cls.wildcard_qualifiers():
+        if cls.wildcard_classifiers():
             if isinstance(source_format, SubtypeVar):
-                if len(cls.wildcard_qualifiers()) > 1:
+                if len(cls.wildcard_classifiers()) > 1:
                     raise FileFormatsError(
                         "Can only have one wildcard qualifier when registering a converter "
-                        f"to {cls} from a generic type, found {cls.wildcard_qualifiers()}"
+                        f"to {cls} from a generic type, found {cls.wildcard_classifiers()}"
                     )
-            elif not source_format.is_qualified:
+            elif not source_format.is_classified:
                 raise FileFormatsError(
-                    "Can only use wildcard qualifiers when registering a converter "
-                    f"from a generic type or similarly qualified type, not {source_format}"
+                    "Can only use wildcard classifiers when registering a converter "
+                    f"from a generic type or similarly classified type, not {source_format}"
                 )
             else:
-                if cls.wildcard_qualifiers() != source_format.wildcard_qualifiers():
+                if cls.wildcard_classifiers() != source_format.wildcard_classifiers():
                     raise FileFormatsError(
                         f"Mismatching wildcards between source format, {source_format} "
-                        f"({list(source_format.wildcard_qualifiers())}), and target "
-                        f"{cls} ({cls.wildcard_qualifiers()})"
+                        f"({list(source_format.wildcard_classifiers())}), and target "
+                        f"{cls} ({cls.wildcard_classifiers()})"
                     )
                 prev_registered = [
                     f
                     for f in cls.converters
                     if (
-                        source_format.unqualified.issubtype(f.unqualified)
-                        and f.non_wildcard_qualifiers()
-                        == source_format.non_wildcard_qualifiers()
+                        source_format.unclassified.issubtype(f.unclassified)
+                        and f.non_wildcard_classifiers()
+                        == source_format.non_wildcard_classifiers()
                     )
                 ]
                 assert len(prev_registered) <= 1
                 prev = prev_registered[0] if prev_registered else None
                 if prev:
                     raise FileFormatsError(
-                        f"There is already a converter registered from {prev.unqualified} "
-                        f"to {cls.unqualified} with non-wildcard qualifiers "
-                        f"{list(prev.non_wildcard_qualifiers())}: "
+                        f"There is already a converter registered from {prev.unclassified} "
+                        f"to {cls.unclassified} with non-wildcard classifiers "
+                        f"{list(prev.non_wildcard_classifiers())}: "
                         + describe_task(cls.converters[prev][0])
                     )
-            converters_dict = cls.unqualified.get_converters_dict()
-            converters_dict[source_format] = converter_tuple + (cls.qualifiers,)
+            converters_dict = cls.unclassified.get_converters_dict()
+            converters_dict[source_format] = converter_tuple + (cls.classifiers,)
         else:
             super().register_converter(source_format, converter_tuple)
 
     @classproperty
-    def namespace(cls):
+    def namespace(cls):  # pylint: disable=no-self-argument
         """The "namespace" the format belongs to under the "fileformats" umbrella
         namespace"""
-        if cls.is_qualified:
-            namespaces = set(t.namespace for t in cls.qualifiers)
+        if cls.is_classified:
+            namespaces = set(t.namespace for t in cls.classifiers)
             if not cls.generically_qualifies:
-                namespaces.add(cls.unqualified.namespace)
+                namespaces.add(cls.unclassified.namespace)
             if len(namespaces) == 1:
                 return next(iter(namespaces))
             else:
                 msg = (
                     "Cannot create reversible MIME type for because did not find a "
-                    f"common namespace between all qualifiers {list(cls.qualifiers)}"
+                    f"common namespace between all classifiers {list(cls.classifiers)}"
                 )
                 if cls.generically_qualifies:
                     msg += (
-                        f" and (non genericly qualified) base class {cls.unqualified}"
+                        f" and (non genericly classified) base class {cls.unclassified}"
                     )
                 raise FormatRecognitionError(msg + f", found:\n{list(namespaces)}")
         else:
             namespace = super().namespace
         return namespace
```

### Comparing `fileformats-0.5.2/fileformats/core/utils.py` & `fileformats-0.6/fileformats/core/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,49 @@
+from __future__ import annotations
 import importlib
 from pathlib import Path
 import inspect
 import typing as ty
 import re
 import os
+import logging
 import pkgutil
 from contextlib import contextmanager
 from fileformats.core.exceptions import (
     MissingExtendedDepenciesError,
     FileFormatsError,
 )
 import fileformats.core
 
+logger = logging.getLogger("fileformats")
 
-def find_matching(fspaths: ty.List[Path], standard_only: bool = False):
+
+def find_matching(
+    fspaths: ty.List[Path], standard_only: bool = False, include_generic: bool = False
+):
     """Detect the corresponding file format from a set of file-system paths
 
     Parameters
     ----------
     fspaths : list[Path]
         file-system paths to detect the format of
     standard_only : bool, optional
-        If you only want to return matches from the "standard" IANA types
+        If you only want to return matches from the "standard" IANA types, by default False
+    include_generic : bool, optional
+        Include generic file-set types (i.e ones within the fileformats.generic package),
+        by default False
     """
     fspaths = fspaths_converter(fspaths)
     matches = []
     for frmt in fileformats.core.FileSet.all_formats:
-        if frmt.matches(fspaths) and (
-            not standard_only or frmt.namespace in STANDARD_NAMESPACES
+        namespace = frmt.namespace
+        if (
+            frmt.matches(fspaths)
+            and (not standard_only or namespace in STANDARD_NAMESPACES)
+            and (include_generic or namespace != "generic")
         ):
             matches.append(frmt)
     return matches
 
 
 def from_mime(mime_str: str):
     return fileformats.core.DataType.from_mime(mime_str)
@@ -97,17 +109,23 @@
         yield path
     finally:
         os.chdir(pwd)
 
 
 def fspaths_converter(
     fspaths: ty.Union[
-        ty.Iterable[ty.Union[str, os.PathLike, bytes]], str, os.PathLike, bytes
+        ty.Iterable[ty.Union[str, os.PathLike, bytes]],
+        str,
+        os.PathLike,
+        bytes,
+        fileformats.core.FileSet,
     ]
 ):
+    import fileformats.core
+
     """Ensures fs-paths are a set of pathlib.Path"""
     if isinstance(fspaths, fileformats.core.FileSet):
         fspaths = fspaths.fspaths
     elif isinstance(fspaths, (str, os.PathLike, bytes)):
         fspaths = [fspaths]
     return frozenset(Path(p).absolute() for p in fspaths)
 
@@ -182,46 +200,46 @@
     format_name = format_name.capitalize()
     format_name = re.sub(r"(\.)(\w)", lambda m: "_" + m.group(2).upper(), format_name)
     format_name = re.sub(r"(\+)(\w)", lambda m: "__" + m.group(2).upper(), format_name)
     format_name = re.sub(r"(-)(\w)", lambda m: m.group(2).upper(), format_name)
     return format_name
 
 
-def hash_file(fspath: Path, chunk_len: int, crypto: ty.Callable):
-    crypto_obj = crypto()
-    with open(fspath, "rb") as fp:
-        for chunk in iter(lambda: fp.read(chunk_len), b""):
-            crypto_obj.update(chunk)
-    return crypto_obj.hexdigest()
-
-
-def hash_dir(
-    fspath: Path,
-    chunk_len: int,
-    crypto: ty.Callable,
-    ignore_hidden_files: bool = False,
-    ignore_hidden_dirs: bool = False,
-    relative_to: Path = None,
-):
-    if relative_to is None:
-        relative_to = fspath
-    file_hashes = {}
-    for dpath, _, filenames in sorted(os.walk(fspath)):
-        # Sort in-place to guarantee order.
-        filenames.sort()
-        dpath = Path(dpath)
-        if ignore_hidden_dirs and dpath.name.startswith(".") and str(dpath) != fspath:
-            continue
-        for filename in filenames:
-            if ignore_hidden_files and filename.startswith("."):
-                continue
-            file_hashes[str((dpath / filename).relative_to(relative_to))] = hash_file(
-                dpath / filename, crypto=crypto, chunk_len=chunk_len
-            )
-    return file_hashes
+# def hash_file(fspath: Path, chunk_len: int, crypto: ty.Callable):
+#     crypto_obj = crypto()
+#     with open(fspath, "rb") as fp:
+#         for chunk in iter(lambda: fp.read(chunk_len), b""):
+#             crypto_obj.update(chunk)
+#     return crypto_obj.hexdigest()
+
+
+# def hash_dir(
+#     fspath: Path,
+#     chunk_len: int,
+#     crypto: ty.Callable,
+#     ignore_hidden_files: bool = False,
+#     ignore_hidden_dirs: bool = False,
+#     relative_to: ty.Optional[Path] = None,
+# ):
+#     if relative_to is None:
+#         relative_to = fspath
+#     file_hashes = {}
+#     for dpath, _, filenames in sorted(os.walk(fspath)):
+#         # Sort in-place to guarantee order.
+#         filenames.sort()
+#         dpath = Path(dpath)
+#         if ignore_hidden_dirs and dpath.name.startswith(".") and str(dpath) != fspath:
+#             continue
+#         for filename in filenames:
+#             if ignore_hidden_files and filename.startswith("."):
+#                 continue
+#             file_hashes[str((dpath / filename).relative_to(relative_to))] = hash_file(
+#                 dpath / filename, crypto=crypto, chunk_len=chunk_len
+#             )
+#     return file_hashes
 
 
 def add_exc_note(e, note):
     """Adds a note to an exception in a Python <3.11 compatible way
 
     Parameters
     ----------
@@ -257,7 +275,81 @@
     if inspect.isfunction(task):
         import cloudpickle
 
         task = cloudpickle.loads(task().inputs._func)
     src_file = inspect.getsourcefile(task)
     src_line = inspect.getsourcelines(task)[-1]
     return f"{task} (defined at line {src_line} of {src_file})"
+
+
+# def on_cifs(fname):
+#     """
+#     Check whether a file path is on a CIFS filesystem mounted in a POSIX host.
+
+#     POSIX hosts are assumed to have the ``mount`` command.
+
+#     On Windows, Docker mounts host directories into containers through CIFS
+#     shares, which has support for Minshall+French symlinks, or text files that
+#     the CIFS driver exposes to the OS as symlinks.
+#     We have found that under concurrent access to the filesystem, this feature
+#     can result in failures to create or read recently-created symlinks,
+#     leading to inconsistent behavior and ``FileNotFoundError`` errors.
+
+#     This check is written to support disabling symlinks on CIFS shares.
+
+#     NB: This function and sub-functions are copied from the nipype.utils.filemanip module
+
+#     """
+#     # Only the first match (most recent parent) counts
+#     for fspath, fstype in _cifs_table:
+#         if fname.startswith(fspath):
+#             return fstype == "cifs"
+#     return False
+
+
+# def _generate_cifs_table():
+#     """
+#     Construct a reverse-length-ordered list of mount points that fall under a CIFS mount.
+
+#     This precomputation allows efficient checking for whether a given path
+#     would be on a CIFS filesystem.
+#     On systems without a ``mount`` command, or with no CIFS mounts, returns an
+#     empty list.
+
+#     """
+#     exit_code, output = sp.getstatusoutput("mount")
+
+#     # Not POSIX
+#     if exit_code != 0:
+#         return []
+
+#     # Linux mount example:  sysfs on /sys type sysfs (rw,nosuid,nodev,noexec)
+#     #                          <PATH>^^^^      ^^^^^<FSTYPE>
+#     # OSX mount example:    /dev/disk2 on / (hfs, local, journaled)
+#     #                               <PATH>^  ^^^<FSTYPE>
+#     pattern = re.compile(r".*? on (/.*?) (?:type |\()([^\s,\)]+)")
+
+#     # Keep line and match for error reporting (match == None on failure)
+#     # Ignore empty lines
+#     matches = [(ll, pattern.match(ll)) for ll in output.strip().splitlines() if ll]
+
+#     # (path, fstype) tuples, sorted by path length (longest first)
+#     mount_info = sorted(
+#         (match.groups() for _, match in matches if match is not None),
+#         key=lambda x: len(x[0]),
+#         reverse=True,
+#     )
+#     cifs_paths = [path for path, fstype in mount_info if fstype.lower() == "cifs"]
+
+#     # Report failures as warnings
+#     for line, match in matches:
+#         if match is None:
+#             logger.debug("Cannot parse mount line: '%s'", line)
+
+#     return [
+#         mount
+#         for mount in mount_info
+#         if any(mount[0].startswith(path) for path in cifs_paths)
+#     ]
+
+
+# _cifs_table = _generate_cifs_table()
```

### Comparing `fileformats-0.5.2/fileformats/core/tests/test_converter.py` & `fileformats-0.6/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/tests/test_detection.py` & `fileformats-0.6/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/tests/test_general.py` & `fileformats-0.6/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/tests/test_mime.py` & `fileformats-0.6/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/tests/test_mixin.py` & `fileformats-0.6/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/core/tests/test_qualifiers.py` & `fileformats-0.6/fileformats/core/tests/test_classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 )
 
 
 SpecificDataType = DataType.type_var("SpecificDataType")
 SpecificFileSet = FileSet.type_var("SpecificFileSet")
 
 
-def test_qualified_equivalence():
+def test_classified_equivalence():
     assert F is F
     assert F[A] is F[A]
     assert F[A, B] is F[B, A]
     assert K[A, B] is not K[B, A]  # ordered qualifers
     assert F[A] is not F[B]
     assert F[SpecificDataType] is F[SpecificDataType]
     assert F[SpecificDataType] is not F[A]
@@ -80,26 +80,26 @@
         H[D]
     assert "Invalid content types provided to" in str(e)
 
     with pytest.raises(FileFormatsError) as e:
         H[A, B, A]
     assert "Cannot have more than one occurrence of a qualifier" in str(e)
 
-    K[A, B, A]  # ordered qualifiers allow repeats
+    K[A, B, A]  # ordered classifiers allow repeats
 
     with pytest.raises(FileFormatsError) as e:
         Q[A]
     assert (
-        "Default value for qualifiers attribute 'new_qualifiers_attr' needs to be set"
+        "Default value for classifiers attribute 'new_classifiers_attr' needs to be set"
         in str(e)
     )
 
     with pytest.raises(FileFormatsError) as e:
         M[A, B]
-    assert "Multiple qualifiers not permitted for " in str(e)
+    assert "Multiple classifiers not permitted for " in str(e)
 
 
 # (source_format=F, target_format=H)
 
 
 @converter
 @converter(source_format=F[A], target_format=H[A])  # Additional converter
@@ -145,29 +145,29 @@
     L[C, A].get_converter(K[A, E, B])  # E is a subtype of C
 
 
 def test_mime_rountrips():
     assert DirectoryContaining[F].mime_like == "testing/f+directory-containing"
     assert from_mime("testing/f+directory-containing") is DirectoryContaining[F]
 
-    # Directory is unordered so sort qualifiers to create unique mime
+    # Directory is unordered so sort classifiers to create unique mime
     assert DirectoryContaining[H, F].mime_like == "testing/f.h+directory-containing"
     assert from_mime("testing/f.h+directory-containing") is DirectoryContaining[F, H]
 
     # K is ordered
     assert K[B, A].mime_like == "testing/b.a+k"
     assert from_mime("testing/b.a+k") is K[B, A]
     assert from_mime("testing/b.a+k") is not K[A, B]
 
     with pytest.raises(FormatRecognitionError) as e:
         Array[TestField].mime_like
     assert "Cannot create reversible MIME type for " in str(e)
 
 
-def test_inherited_qualifiers():
+def test_inherited_classifiers():
     assert Zip[G].mime_like == "testing/g+zip"
     assert from_mime("testing/g+zip") is Zip[G]
 
 
 def test_arrays():
     Array[Integer]([1, 2, 3, 4])
     with pytest.raises(FormatMismatchError) as e:
```

### Comparing `fileformats-0.5.2/fileformats/document/__init__.py` & `fileformats-0.6/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/field/__init__.py` & `fileformats-0.6/fileformats/field/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import attrs
 import decimal
-from ..core import Field
-from ..core.mixin import WithQualifiers
-from ..core.exceptions import FormatMismatchError
+import typing as ty
+import attrs
+from fileformats.core import Field
+from fileformats.core.mixin import WithClassifiers
+from fileformats.core.exceptions import FormatMismatchError
 
 
 @attrs.define
-class Singluar(Field):
+class Singular(Field):
     pass
 
 
 class LogicalMixin:
     def __bool__(self):
         return bool(self.value)
 
@@ -59,36 +60,36 @@
         return abs(self.value)
 
 
 def text_converter(value):
     try:
         return str(value)
     except ValueError as e:
-        raise FormatMismatchError(str(e))
+        raise FormatMismatchError(str(e)) from None
 
 
 def integer_converter(value):
     if isinstance(value, float):
         raise FormatMismatchError(
             f"Cannot convert float ({value}) to integer field without potential loss "
             "of information"
         )
     try:
         return int(value)
     except ValueError as e:
-        raise FormatMismatchError(str(e))
+        raise FormatMismatchError(str(e)) from None
 
 
 def decimal_converter(value):
     if isinstance(value, Decimal):
         return value.value
     try:
         return decimal.Decimal(value)
     except decimal.InvalidOperation as e:
-        raise FormatMismatchError(str(e))
+        raise FormatMismatchError(str(e)) from None
 
 
 def boolean_converter(value):
     if isinstance(value, str):
         if value.lower() in ("true", "1", "yes"):
             value = True
         elif value.lower() in ("false", "0", "no"):
@@ -97,109 +98,111 @@
             raise FormatMismatchError(
                 f"Cannot convert string '{value}' to boolean value"
             )
     else:
         try:
             value = bool(value)
         except ValueError as e:
-            raise FormatMismatchError(str(e))
+            raise FormatMismatchError(str(e)) from None
     return value
 
 
 def array_converter(value):
     if isinstance(value, str):
         if value.startswith("[") and value.endswith("]"):
             value = value[1:-1]
         elif value.startswith("[") or value.endswith("]"):
             raise FormatMismatchError(f"Unmatched brackets in array field {value}")
         value = [v.strip() for v in value.split(",")]
     else:
         try:
             value = list(value)
         except ValueError as e:
-            raise FormatMismatchError(str(e))
+            raise FormatMismatchError(str(e)) from None
     return value
 
 
 @attrs.define
-class Text(Singluar):
+class Text(Singular):
 
     value: str = attrs.field(converter=text_converter)
 
-    raw_type = str
+    primitive = str
 
 
 @attrs.define
-class Integer(Singluar, ScalarMixin):
+class Integer(Singular, ScalarMixin):
 
     value: int = attrs.field(converter=integer_converter)
 
-    raw_type = int
+    primitive = int
 
     def __int__(self):
         return self.value
 
     def __float__(self):
         return float(self.value)
 
     def __bool__(self):
         return bool(self.value)
 
 
 @attrs.define
-class Decimal(Singluar, ScalarMixin):
+class Decimal(Singular, ScalarMixin):
 
     value: decimal.Decimal = attrs.field(converter=decimal_converter)
 
-    raw_type = float
+    primitive = float
 
     def __float__(self):
         return float(self.value)
 
     def __bool__(self):
         return bool(self.value)
 
 
 @attrs.define
-class Boolean(Singluar, LogicalMixin):
+class Boolean(Singular, LogicalMixin):
 
-    raw_type = bool
+    primitive = bool
 
     value: bool = attrs.field(converter=boolean_converter)
 
     def __str__(self):
         return str(self.value).lower()
 
     def __bool__(self):
         return self.value
 
 
-@attrs.define
-class Array(WithQualifiers, Field):
+@attrs.define(auto_attribs=False)
+class Array(WithClassifiers, Field):
 
-    # WithQualifiers class attrs
-    qualifiers_attr_name = "item_type"
-    multiple_qualifiers = False
-    allowed_qualifiers = (Singluar,)
-    item_type = None
+    # WithClassifiers class attrs
+    classifiers_attr_name: str = "item_type"
+    multiple_classifiers: bool = False
+    allowed_classifiers: ty.Tuple[ty.Type[Singular]] = (Singular,)
+    item_type: ty.Union[ty.Type[Singular], None] = None
 
-    raw_type = list
+    primitive = list
 
     value: list = attrs.field(converter=array_converter)
 
     def __attrs_post_init__(self):
         # Ensure items are of the correct type
         if self.item_type is not None:
             self.value = [self.item_type(i).value for i in self.value]
 
     def __str__(self):
         return (
             "["
             + ",".join(
-                str(self.item_type(i)) if self.item_type is not None else i
+                str(self.item_type(i))
+                if self.item_type is not None
+                else i  # pylint: disable=not-callable
                 for i in self.value
             )
             + "]"
         )
 
     def __iter__(self):
         return iter(self.value)
```

### Comparing `fileformats-0.5.2/fileformats/field/tests/test_fields.py` & `fileformats-0.6/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/generic/__init__.py` & `fileformats-0.6/fileformats/generic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 import attrs
-from ..core.base import FileSet
-from ..core.exceptions import FormatMismatchError, FileFormatsError
-from ..core import mark
-from ..core.utils import splitext, classproperty
-from ..core.mixin import WithQualifiers
+from fileformats.core.base import FileSet
+from fileformats.core.exceptions import FormatMismatchError, FileFormatsError
+from fileformats.core import mark
+from fileformats.core.utils import splitext, classproperty
+from fileformats.core.mixin import WithClassifiers
 
 
 @attrs.define
 class FsObject(FileSet, os.PathLike):
     "Generic file-system object, can be either a file or a directory"
 
     @mark.required
@@ -26,14 +26,18 @@
         return str(self.fspath)
 
     def __fspath__(self):
         """Render to string, so can be treated as any other file-system path, i.e. passed
         to functions like file 'open'"""
         return str(self)
 
+    @property
+    def stem(self):
+        return self.fspath.with_suffix("").name
+
 
 @attrs.define
 class File(FsObject):
     """Generic file type"""
 
     binary = False
     is_dir = False
@@ -111,15 +115,15 @@
         if not matching:
             assert False, (
                 f"extension of fspath {self.fspath} is not in possible extensions for "
                 f"{type(self)} class: {self.possible_exts}. This should have been "
                 "checked at initialisation"
             )
         # Return the longest matching extension, useful for optional extensions
-        return sorted(matching, key=lambda x: len(x))[-1]
+        return sorted(matching, key=len)[-1]
 
     @property
     def stem(self):
         return self.fspath.name[: -len(self.actual_ext)]
 
 
 @attrs.define
@@ -133,15 +137,15 @@
 
     @mark.required
     @property
     def fspath(self):
         dirs = [p for p in self.fspaths if p.is_dir()]
         if not dirs:
             raise FormatMismatchError(f"No directory paths provided {repr(self)}")
-        elif len(dirs) > 1:
+        if len(dirs) > 1:
             raise FormatMismatchError(
                 f"More than one directory path provided {dirs} to {repr(self)}"
             )
         fspath = dirs[0]
         missing = []
         for content_type in self.content_types:
             match = False
@@ -222,22 +226,22 @@
         assert not_found
         raise FormatMismatchError(
             f"Did not find the required content types, {not_found}, within the "
             f"given list {self.fspaths}"
         )
 
 
-class DirectoryContaining(WithQualifiers, Directory):
-    """Generic directory qualified by the formats of its contents"""
+class DirectoryContaining(WithClassifiers, Directory):
+    """Generic directory classified by the formats of its contents"""
 
-    # WithQualifiers-required class attrs
-    qualifiers_attr_name = "content_types"
-    allowed_qualifiers = (FileSet,)
+    # WithClassifiers-required class attrs
+    classifiers_attr_name = "content_types"
+    allowed_classifiers = (FileSet,)
     generically_qualifies = True
 
 
-class SetOf(WithQualifiers, TypedSet):
+class SetOf(WithClassifiers, TypedSet):
 
-    # WithQualifiers-required class attrs
-    qualifiers_attr_name = "content_types"
-    allowed_qualifiers = (FileSet,)
+    # WithClassifiers-required class attrs
+    classifiers_attr_name = "content_types"
+    allowed_classifiers = (FileSet,)
     generically_qualifies = True
```

### Comparing `fileformats-0.5.2/fileformats/image/converters.py` & `fileformats-0.6/fileformats/image/converters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from pathlib import Path
+import typing as ty
 import tempfile
 import pydra.mark
 import pydra.engine.specs
 from fileformats.core import mark
 from .raster import RasterImage, Bitmap, Gif, Jpeg, Png, Tiff
 
 
 @mark.converter(target_format=Bitmap, output_format=Bitmap)
 @mark.converter(target_format=Gif, output_format=Gif)
 @mark.converter(target_format=Jpeg, output_format=Jpeg)
 @mark.converter(target_format=Png, output_format=Png)
 @mark.converter(target_format=Tiff, output_format=Tiff)
 @pydra.mark.task
 @pydra.mark.annotate({"return": {"out_file": RasterImage}})
-def convert_image(in_file: RasterImage, output_format: type, out_dir: Path = None):
+def convert_image(
+    in_file: RasterImage, output_format: type, out_dir: ty.Optional[Path] = None
+):
     data_array = in_file.load()
     if out_dir is None:
         out_dir = Path(tempfile.mkdtemp())
     output_path = out_dir / (in_file.fspath.stem + output_format.ext)
     return output_format.save_new(output_path, data_array)
```

### Comparing `fileformats-0.5.2/fileformats/image/raster.py` & `fileformats-0.6/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/serialization/__init__.py` & `fileformats-0.6/fileformats/serialization/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 import json
 from ..core import __version__, mark, DataType
-from ..core.mixin import WithQualifiers
+from ..core.mixin import WithClassifiers
 from ..generic import File
 from ..core.utils import MissingExtendedDependency
 
 try:
     import yaml
 except ImportError:
     yaml = MissingExtendedDependency("yaml", __name__)
@@ -26,22 +26,22 @@
     pass
 
 
 class InformalSchema(Schema):
     "Not actually a strict schema, just a set of conventions on how to structure the serialization"
 
 
-class DataSerialization(WithQualifiers, File):
+class DataSerialization(WithClassifiers, File):
     "Base class for text-based hierarchical data-serialization formats, e.g. JSON, YAML"
 
-    # Qualifiers class attrs
-    qualifiers_attr_name = "schema"
+    # Classifiers class attrs
+    classifiers_attr_name = "schema"
     schema = None
-    multiple_qualifiers = False
-    allowed_qualifiers = (Schema,)
+    multiple_classifiers = False
+    allowed_classifiers = (Schema,)
     generically_qualifies = True
 
     iana_mime = None
 
     @mark.check
     def load(self):
         """Load the contents of the file into a dictionary"""
@@ -51,20 +51,20 @@
     def save_new(fspath: Path, dct: dict):
         """Serialise a dictionary to a new file"""
         raise NotImplementedError
 
 
 class Xml(DataSerialization):
     ext = ".xml"
-    allowed_qualifiers = (XmlSchema, InformalSchema)
+    allowed_classifiers = (XmlSchema, InformalSchema)
 
 
 class Json(DataSerialization):
     ext = ".json"
-    allowed_qualifiers = (JsonSchema, InformalSchema)
+    allowed_classifiers = (JsonSchema, InformalSchema)
 
     @mark.check
     def load(self):
         with open(self.fspath) as f:
             dct = json.load(f)
         return dct
```

### Comparing `fileformats-0.5.2/fileformats/serialization/converters.py` & `fileformats-0.6/fileformats/serialization/converters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
+import typing as ty
 import tempfile
 import pydra.mark
 import pydra.engine.specs
 from fileformats.core import mark
 from . import DataSerialization, Json, Yaml
 
 
 @mark.converter(target_format=Json, output_format=Json)
 @mark.converter(target_format=Yaml, output_format=Yaml)
 @pydra.mark.task
 @pydra.mark.annotate({"return": {"out_file": DataSerialization}})
 def convert_data_serialization(
-    in_file: DataSerialization, output_format: type, out_dir: Path = None
+    in_file: DataSerialization, output_format: type, out_dir: ty.Optional[Path] = None
 ):
     dct = in_file.load()
     if out_dir is None:
         out_dir = Path(tempfile.mkdtemp())
     output_path = out_dir / (in_file.fspath.stem + output_format.ext)
     return output_format.save_new(output_path, dct)
```

### Comparing `fileformats-0.5.2/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/fileformats/text/__init__.py` & `fileformats-0.6/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/LICENSE` & `fileformats-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/README.rst` & `fileformats-0.6/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.5.2/pyproject.toml` & `fileformats-0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "fileformats[extended]",
     "fileformats[test]",
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
-    "codecov",
     "fileformats-testing",
 ]
 docs = [
     "packaging",
     "docutils>=0.10",
     "mock>1.0",
     "sphinx >=2.1.2",
```

### Comparing `fileformats-0.5.2/PKG-INFO` & `fileformats-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.5.2
+Version: 0.6
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -132,15 +132,14 @@
 Requires-Dist: sphinx-click>=3.1; extra == 'docs'
 Requires-Dist: sphinx>=2.1.2; extra == 'docs'
 Provides-Extra: extended
 Requires-Dist: imageio>=2.24.0; extra == 'extended'
 Requires-Dist: pydra>=0.20.0; extra == 'extended'
 Requires-Dist: pyyaml>=6.0; extra == 'extended'
 Provides-Extra: test
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: fileformats-testing; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats
```

