# Comparing `tmp/dapla_toolbelt_pseudo-0.2.8.tar.gz` & `tmp/dapla_toolbelt_pseudo-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-0.2.8.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-0.2.9.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-0.2.8.tar` & `dapla_toolbelt_pseudo-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-06-06 06:55:57.690538 dapla_toolbelt_pseudo-0.2.8/LICENSE
--rw-r--r--   0        0        0     4899 2023-06-06 06:55:57.690538 dapla_toolbelt_pseudo-0.2.8/README.md
--rw-r--r--   0        0        0     2460 2023-06-06 06:56:08.254712 dapla_toolbelt_pseudo-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1214 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      833 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      455 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0      888 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      377 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0     5529 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/builder.py
--rw-r--r--   0        0        0    11256 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0     5248 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/models.py
--rw-r--r--   0        0        0    12949 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/ops.py
--rw-r--r--   0        0        0      668 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.8/setup.py
--rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-07 08:47:01.077868 dapla_toolbelt_pseudo-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4899 2023-06-07 08:47:01.077868 dapla_toolbelt_pseudo-0.2.9/README.md
+-rw-r--r--   0        0        0     2460 2023-06-07 08:47:15.313956 dapla_toolbelt_pseudo-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1214 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      833 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      455 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0      888 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      377 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0     6617 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/builder.py
+-rw-r--r--   0        0        0    11256 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     5248 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/models.py
+-rw-r--r--   0        0        0    12949 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/ops.py
+-rw-r--r--   0        0        0      668 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.9/setup.py
+-rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.9/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-0.2.8/LICENSE` & `dapla_toolbelt_pseudo-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/README.md` & `dapla_toolbelt_pseudo-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/pyproject.toml` & `dapla_toolbelt_pseudo-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "0.2.8"
+version = "0.2.9"
 description = "Pseudonymization extensions for Dapla Toolbelt"
 authors = ["Team Skyinfrastruktur <dapla@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/builder.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,29 +39,55 @@
     @staticmethod
     def from_pandas(dataframe: pd.DataFrame) -> "_FieldSelector":
         """Initialize a pseudonymization request from a pandas DataFrame."""
         return PseudoData._FieldSelector(dataframe)
 
     @staticmethod
     def from_file(file_path_str: str, **kwargs: Any) -> "_FieldSelector":
-        """Initialize a pseudonymization request from a pandas dataframe read from file."""
+        """Initialize a pseudonymization request from a pandas dataframe read from file.
+
+        Args:
+            file_path_str (str): The path to the file to be read.
+            kwargs (dict): Additional keyword arguments to be passed to the file reader.
+
+        Raises:
+            FileNotFoundError: If no file is found at the specified local path.
+            NoFileExtensionError: If the file has no extension.
+
+        Returns:
+            _FieldSelector: An instance of the _FieldSelector class.
+
+        Examples:
+            # Read from bucket
+            from dapla import AuthClient
+            from dapla_pseudo import PseudoData
+            bucket_path = "gs://ssb-staging-dapla-felles-data-delt/felles/smoke-tests/fruits/data.parquet"
+            storage_options = {"token": AuthClient.fetch_google_credentials()}
+            field_selector = PseudoData.from_file(bucket_path, storage_options=storage_options)
+
+            # Read from local filesystem
+            from dapla_pseudo import PseudoData
+
+            local_path = "some_file.csv"
+            field_selector = PseudoData.from_file(local_path)
+        """
         file_path = Path(file_path_str)
 
-        if not file_path.is_file():
-            raise FileNotFoundError(f"No file found at path: {file_path}")
+        if not file_path.is_file() and "storage_options" not in kwargs:
+            raise FileNotFoundError(f"No local file found in path: {file_path}")
 
         file_extension = file_path.suffix[1:]
 
         if file_extension == "":
             raise NoFileExtensionError(f"The file {file_path_str!r} has no file extension.")
 
         file_format = SupportedFileFormat(file_extension)
 
         pandas_function = getattr(pd, file_format.get_pandas_function_name())
-        return PseudoData._FieldSelector(pandas_function(file_path, **kwargs))
+        return PseudoData._FieldSelector(pandas_function(file_path_str, **kwargs))
 
     class _FieldSelector:
         """Select one or multiple fields to be pseudonymized."""
 
         def __init__(self, dataframe: pd.DataFrame):
             """Initialize the class."""
             self._dataframe = dataframe
```

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/models.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/ops.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/ops.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.8/setup.py` & `dapla_toolbelt_pseudo-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pyhumps>=3.8.0,<4.0.0',
  'pylibmagic>=0.2.2,<0.3.0',
  'python-magic>=0.4.27,<0.5.0',
  'types-requests>=2.28.11,<3.0.0']
 
 setup_kwargs = {
     'name': 'dapla-toolbelt-pseudo',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Pseudonymization extensions for Dapla Toolbelt',
     'long_description': '# Pseudonymization extensions for Dapla Toolbelt\n\n[![PyPI](https://img.shields.io/pypi/v/dapla-toolbelt-pseudo.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/dapla-toolbelt-pseudo.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/dapla-toolbelt-pseudo)][python version]\n[![License](https://img.shields.io/pypi/l/dapla-toolbelt-pseudo)][license]\n\n[![Tests](https://github.com/statisticsnorway/dapla-toolbelt-pseudo/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[status]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[python version]: https://pypi.org/project/dapla-toolbelt-pseudo\n[tests]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nPseudonymize, repseudonymize and depseudonymize data on Dapla.\n\n## Usage\n\nSee the [command-line reference] for details.\n\n### Pseudonymize\n\n```python\nfrom dapla_pseudo import pseudonymize\n\n# Pseudonymize fields in a local file using the default key:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"])\n\n# Pseudonymize fields in a local file, explicitly denoting the key to use:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n\n# Pseudonymize a local file using a custom key:\nimport json\ncustom_keyset = json.dumps(    {\n    "encryptedKeyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",\n    "keysetInfo": {\n        "primaryKeyId": 1234567890,\n        "keyInfo": [\n            {\n                "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",\n                "status": "ENABLED",\n                "keyId": 1234567890,\n                "outputPrefixType": "TINK",\n            }\n        ],\n    },\n    "kekUri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1",\n})\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key=custom_keyset)\n\n# Operate on data in a streaming manner:\nimport shutil\nwith pseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:\n    with open("./data/personer_deid.json", \'wb\') as f:\n        res.raw.decode_content = True\n        shutil.copyfileobj(res.raw, f)\n\n# Map certain fields to stabil ID\npseudonymize(file_path="./data/personer.json", fields=["fornavn"], sid_fields=["fnr"])\n```\n\n### Repseudonymize\n\n```python\nfrom dapla_pseudo import repseudonymize\n\n# Repseudonymize fields in a local file, denoting source and target keys to use:\nrepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], source_key="ssb-common-key-1", target_key="ssb-common-key-2")\n```\n\n### Depseudonymize\n\n```python\nfrom dapla_pseudo import depseudonymize\n\n# Depseudonymize fields in a local file using the default key:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"])\n\n# Depseudonymize fields in a local file, explicitly denoting the key to use:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n```\n\n_Note that depseudonymization requires elevated access privileges._\n\n## Requirements\n\n- [Dapla Toolbelt](https://github.com/statisticsnorway/dapla-toolbelt)\n\n## Installation\n\nYou can install _dapla-toolbelt-pseudo_ via [pip] from [PyPI]:\n\n```console\npip install dapla-toolbelt-pseudo\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Pseudonymization extensions for Dapla Toolbelt_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/LICENSE\n[contributor guide]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/CONTRIBUTING.md\n[command-line reference]: https://statisticsnorway.github.io/dapla-toolbelt-pseudo\n',
     'author': 'Team Skyinfrastruktur',
     'author_email': 'dapla@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/dapla-toolbelt-pseudo',
```

### Comparing `dapla_toolbelt_pseudo-0.2.8/PKG-INFO` & `dapla_toolbelt_pseudo-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Pseudonymization extensions for Dapla Toolbelt
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Team Skyinfrastruktur
 Author-email: dapla@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

