# Comparing `tmp/pytest_localstack-0.6.0.tar.gz` & `tmp/pytest_localstack-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_localstack-0.6.0.tar", max compression
+gzip compressed data, was "pytest_localstack-0.6.1.tar", max compression
```

## Comparing `pytest_localstack-0.6.0.tar` & `pytest_localstack-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1885 2022-10-17 22:28:55.302325 pytest_localstack-0.6.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1073 2019-10-04 18:42:05.412310 pytest_localstack-0.6.0/LICENSE
--rw-r--r--   0        0        0     3170 2020-09-22 14:57:02.276233 pytest_localstack-0.6.0/README.rst
--rw-r--r--   0        0        0     2303 2022-10-17 23:06:33.339054 pytest_localstack-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5767 2022-10-17 19:04:18.938432 pytest_localstack-0.6.0/pytest_localstack/__init__.py
--rw-r--r--   0        0        0     1422 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/constants.py
--rw-r--r--   0        0        0     1777 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/container.py
--rw-r--r--   0        0        0        0 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/contrib/__init__.py
--rw-r--r--   0        0        0     2380 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/contrib/boto3.py
--rw-r--r--   0        0        0    21840 2022-02-25 21:38:47.930949 pytest_localstack-0.6.0/pytest_localstack/contrib/botocore.py
--rw-r--r--   0        0        0     2040 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/exceptions.py
--rw-r--r--   0        0        0     1577 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/hookspecs.py
--rw-r--r--   0        0        0      872 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/plugin.py
--rw-r--r--   0        0        0     5767 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/service_checks.py
--rw-r--r--   0        0        0    15923 2022-10-17 22:28:08.102234 pytest_localstack-0.6.0/pytest_localstack/session.py
--rw-r--r--   0        0        0     2739 2022-02-25 21:30:34.233161 pytest_localstack-0.6.0/pytest_localstack/utils.py
--rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 pytest_localstack-0.6.0/setup.py
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 pytest_localstack-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1983 2023-06-07 04:29:41.259314 pytest_localstack-0.6.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1073 2019-10-04 18:42:05.412310 pytest_localstack-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3170 2020-09-22 14:57:02.276233 pytest_localstack-0.6.1/README.rst
+-rw-r--r--   0        0        0     2393 2023-06-06 20:59:57.441646 pytest_localstack-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5767 2022-10-17 19:04:18.938432 pytest_localstack-0.6.1/pytest_localstack/__init__.py
+-rw-r--r--   0        0        0     1422 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/constants.py
+-rw-r--r--   0        0        0     1777 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/container.py
+-rw-r--r--   0        0        0        0 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/contrib/__init__.py
+-rw-r--r--   0        0        0     2380 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/contrib/boto3.py
+-rw-r--r--   0        0        0    21840 2022-02-25 21:38:47.930949 pytest_localstack-0.6.1/pytest_localstack/contrib/botocore.py
+-rw-r--r--   0        0        0     2040 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/exceptions.py
+-rw-r--r--   0        0        0     1577 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/hookspecs.py
+-rw-r--r--   0        0        0      872 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/plugin.py
+-rw-r--r--   0        0        0     5767 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/service_checks.py
+-rw-r--r--   0        0        0    15922 2023-06-07 04:28:31.459221 pytest_localstack-0.6.1/pytest_localstack/session.py
+-rw-r--r--   0        0        0     2739 2022-02-25 21:30:34.233161 pytest_localstack-0.6.1/pytest_localstack/utils.py
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 pytest_localstack-0.6.1/setup.py
+-rw-r--r--   0        0        0     4723 1970-01-01 00:00:00.000000 pytest_localstack-0.6.1/PKG-INFO
```

### Comparing `pytest_localstack-0.6.0/CHANGELOG.rst` & `pytest_localstack-0.6.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change Log
 ==========
 
+0.6.1 (2023-06-06)
+------------------
+
+- Update to docker >= v6 to address deprecation warnings.
+
 0.6.0 (2022-10-17)
 ------------------
 
 - Get the default Localstack hostname from the `DOCKER_HOST` env var, if set.
 - Protect starting/stopping the Localstack container with a lock.
 
 0.5.0 (2022-10-13)
```

### Comparing `pytest_localstack-0.6.0/LICENSE` & `pytest_localstack-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/README.rst` & `pytest_localstack-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pyproject.toml` & `pytest_localstack-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-localstack"
-version = "0.6.0"
+version = "0.6.1"
 description = "Pytest plugin for AWS integration tests"
 authors = ["Mintel Group Ltd."]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/mintel/pytest-localstack"
 documentation = "https://pytest-localstack.readthedocs.io/"
 keywords = ["pytest", "localstack", "aws"]
@@ -26,17 +26,18 @@
 ]
 include = ["CHANGELOG.rst", "LICENSE"]
 
 [tool.poetry.plugins.pytest11]
 localstack = "pytest_localstack"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-botocore = "^1.4.31,!=1.4.45"
-docker = "^4.0.0"
+python = "^3.7.0"
+botocore = "!=1.4.45"
+urllib3 = "<2" # https://github.com/orgs/python-poetry/discussions/7937#discussioncomment-5921842
+docker = "^6.0.0"
 pluggy = "^0.12.0"
 pytest = "^6.0.0"  # need caplog (+ warnings for tests)
 
 [tool.poetry.dev-dependencies]
 boto3 = "*"
 hypothesis = "*"
 black = "*"
```

### Comparing `pytest_localstack-0.6.0/pytest_localstack/__init__.py` & `pytest_localstack-0.6.1/pytest_localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/constants.py` & `pytest_localstack-0.6.1/pytest_localstack/constants.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/container.py` & `pytest_localstack-0.6.1/pytest_localstack/container.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/contrib/boto3.py` & `pytest_localstack-0.6.1/pytest_localstack/contrib/boto3.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/contrib/botocore.py` & `pytest_localstack-0.6.1/pytest_localstack/contrib/botocore.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/exceptions.py` & `pytest_localstack-0.6.1/pytest_localstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/hookspecs.py` & `pytest_localstack-0.6.1/pytest_localstack/hookspecs.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/plugin.py` & `pytest_localstack-0.6.1/pytest_localstack/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/service_checks.py` & `pytest_localstack-0.6.1/pytest_localstack/service_checks.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/pytest_localstack/session.py` & `pytest_localstack-0.6.1/pytest_localstack/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         hostname,
         services=None,
         region_name=None,
         use_ssl=False,
         localstack_version="latest",
         **kwargs,
     ):
-
         self.kwargs = kwargs
         self.use_ssl = use_ssl
         self.region_name = region_name
         self._hostname = hostname
         self.localstack_version = localstack_version
 
         if self.localstack_version != "latest" and utils.get_version_tuple(
```

### Comparing `pytest_localstack-0.6.0/pytest_localstack/utils.py` & `pytest_localstack-0.6.1/pytest_localstack/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_localstack-0.6.0/setup.py` & `pytest_localstack-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 packages = \
 ['pytest_localstack', 'pytest_localstack.contrib']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['botocore>=1.4.31,<2.0.0,!=1.4.45',
- 'docker>=4.0.0,<5.0.0',
+['botocore!=1.4.45',
+ 'docker>=6.0.0,<7.0.0',
  'pluggy>=0.12.0,<0.13.0',
- 'pytest>=6.0.0,<7.0.0']
+ 'pytest>=6.0.0,<7.0.0',
+ 'urllib3<2']
 
 entry_points = \
 {'pytest11': ['localstack = pytest_localstack']}
 
 setup_kwargs = {
     'name': 'pytest-localstack',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Pytest plugin for AWS integration tests',
     'long_description': 'pytest-localstack\n=================\n\n.. image:: https://img.shields.io/pypi/v/pytest-localstack.svg\n    :alt: PyPI\n    :target: https://pypi.org/project/pytest-localstack/\n\n.. image:: https://img.shields.io/travis/mintel/pytest-localstack/master.svg\n    :alt: Travis-CI\n    :target: https://travis-ci.org/mintel/pytest-localstack\n\n.. image:: https://img.shields.io/codecov/c/github/mintel/pytest-localstack.svg\n    :alt: Codecov\n    :target: https://codecov.io/gh/mintel/pytest-localstack\n\n.. image:: https://img.shields.io/github/license/mintel/pytest-localstack.svg\n    :target: https://github.com/mintel/pytest-localstack/blob/master/LICENSE\n\n.. image:: https://img.shields.io/github/issues/mintel/pytest-localstack.svg\n    :target: https://github.com/mintel/pytest-localstack/issues\n\n.. image:: https://img.shields.io/github/forks/mintel/pytest-localstack.svg\n    :target: https://github.com/mintel/pytest-localstack/network\n\n.. image:: https://img.shields.io/github/stars/mintel/pytest-localstack.svg\n    :target: https://github.com/mintel/pytest-localstack/stargazers\n\npytest-localstack is a plugin for pytest_ to create AWS_ integration tests\nvia a Localstack_ Docker container.\n\n`Read The Docs`_\n\n**Requires:**\n\n- pytest >= 3.3.0\n- Docker\n\nTested against Python >= 3.6.\n\n.. _pytest: http://docs.pytest.org/\n.. _AWS: https://aws.amazon.com/\n.. _Localstack: https://github.com/localstack/localstack\n.. _Read the Docs: https://pytest-localstack.readthedocs.io/\n\n\nFeatures\n--------\n* Create `pytest fixtures`_ that start and stop a Localstack container.\n* Temporarily patch botocore to redirect botocore/boto3 API calls to Localstack container.\n* Plugin system to easily extend supports to other AWS client libraries such as aiobotocore_.\n\n.. _pytest fixtures: https://docs.pytest.org/en/stable/fixture.html\n\nExample\n-------\n.. code-block:: python\n\n    import boto3\n    import pytest_localstack\n\n    localstack = pytest_localstack.patch_fixture(\n        services=["s3"],  # Limit to the AWS services you need.\n        scope=\'module\',  # Use the same Localstack container for all tests in this module.\n        autouse=True,  # Automatically use this fixture in tests.\n    )\n\n    def test_s3_bucket_creation():\n        s3 = boto3.resource(\'s3\')  # Botocore/boto3 will be patched to use Localstack\n        assert len(list(s3.buckets.all())) == 0\n        bucket = s3.Bucket(\'foobar\')\n        bucket.create()\n        assert len(list(s3.buckets.all())) == 1\n\nServices\n--------\n* apigateway\n* cloudformation\n* cloudwatch\n* dynamodb\n* dynamodbstreams\n* ec2\n* es\n* firehose\n* iam\n* kinesis\n* lambda\n* logs\n* redshift\n* route53\n* s3\n* secretsmanager\n* ses\n* sns\n* sqs\n* ssm\n* stepfunctions\n* sts\n\nInstallation\n------------\n.. code-block:: bash\n\n    $ pip install pytest-localstack\n\n\nTODO\n----\n\n* More detailed docs.\n* Break Docker container running out of LocalstackSession.\n* Make botocore patching more comprehensible.\n* Add common test resource fixture factories i.e. S3 buckets, SQS queues, SNS topics, etc.\n* Test this works for non-localhost Docker containers.\n* Add other client libraries such as aiobotocore_.\n\n.. _aiobotocore: https://github.com/aio-libs/aiobotocore\n',
     'author': 'Mintel Group Ltd.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mintel/pytest-localstack',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4.0.0',
+    'python_requires': '>=3.7.0,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pytest_localstack-0.6.0/PKG-INFO` & `pytest_localstack-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-localstack
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pytest plugin for AWS integration tests
 Home-page: https://github.com/mintel/pytest-localstack
 License: MIT
 Keywords: pytest,localstack,aws
 Author: Mintel Group Ltd.
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
@@ -23,18 +23,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Dist: botocore (>=1.4.31,<2.0.0,!=1.4.45)
-Requires-Dist: docker (>=4.0.0,<5.0.0)
+Requires-Dist: botocore (!=1.4.45)
+Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: pluggy (>=0.12.0,<0.13.0)
 Requires-Dist: pytest (>=6.0.0,<7.0.0)
+Requires-Dist: urllib3 (<2)
 Project-URL: Documentation, https://pytest-localstack.readthedocs.io/
 Project-URL: Repository, https://github.com/mintel/pytest-localstack
 Description-Content-Type: text/x-rst
 
 pytest-localstack
 =================
```

