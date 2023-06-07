# Comparing `tmp/reportseff-2.7.4.tar.gz` & `tmp/reportseff-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportseff-2.7.4.tar", max compression
+gzip compressed data, was "reportseff-2.7.5.tar", max compression
```

## Comparing `reportseff-2.7.4.tar` & `reportseff-2.7.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-03-31 18:26:17.799181 reportseff-2.7.4/LICENSE
--rw-r--r--   0        0        0    13013 2023-03-31 18:26:17.799181 reportseff-2.7.4/README.md
--rw-r--r--   0        0        0     1357 2023-03-31 18:26:17.799181 reportseff-2.7.4/pyproject.toml
--rw-r--r--   0        0        0      370 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/__init__.py
--rw-r--r--   0        0        0     7435 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/console.py
--rw-r--r--   0        0        0    14142 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/db_inquirer.py
--rw-r--r--   0        0        0    14445 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/job.py
--rw-r--r--   0        0        0     9184 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/job_collection.py
--rw-r--r--   0        0        0    14553 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/output_renderer.py
--rw-r--r--   0        0        0     2726 2023-03-31 18:26:17.799181 reportseff-2.7.4/src/reportseff/parameters.py
--rw-r--r--   0        0        0    14264 1970-01-01 00:00:00.000000 reportseff-2.7.4/setup.py
--rw-r--r--   0        0        0    13824 1970-01-01 00:00:00.000000 reportseff-2.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-07 17:01:21.953909 reportseff-2.7.5/LICENSE
+-rw-r--r--   0        0        0    13013 2023-06-07 17:01:21.953909 reportseff-2.7.5/README.md
+-rw-r--r--   0        0        0     1358 2023-06-07 17:01:21.957909 reportseff-2.7.5/pyproject.toml
+-rw-r--r--   0        0        0      370 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/__init__.py
+-rw-r--r--   0        0        0     7435 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/console.py
+-rw-r--r--   0        0        0    14210 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/db_inquirer.py
+-rw-r--r--   0        0        0    14445 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/job.py
+-rw-r--r--   0        0        0     9184 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/job_collection.py
+-rw-r--r--   0        0        0    14553 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/output_renderer.py
+-rw-r--r--   0        0        0     2726 2023-06-07 17:01:21.957909 reportseff-2.7.5/src/reportseff/parameters.py
+-rw-r--r--   0        0        0    14264 1970-01-01 00:00:00.000000 reportseff-2.7.5/setup.py
+-rw-r--r--   0        0        0    13824 1970-01-01 00:00:00.000000 reportseff-2.7.5/PKG-INFO
```

### Comparing `reportseff-2.7.4/LICENSE` & `reportseff-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/README.md` & `reportseff-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/pyproject.toml` & `reportseff-2.7.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reportseff"
-version = "2.7.4"
+version = "2.7.5"
 description= "Tablular seff output"
 authors = ["Troy Comi <troycomi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage= "https://github.com/troycomi/reportseff"
 repository= "https://github.com/troycomi/reportseff"
 keywords= ["slurm","seff"]
@@ -18,27 +18,27 @@
 pytest = "^7.2.0"
 pytest-mock = "^3.6.1"
 coverage = {extras = ["toml"], version = "^6.0.2"}
 pytest-cov = "^3.0.0"
 black = { version = "^22.1.0", allow-prereleases = true }
 flake8 = "^3.7.9"
 flake8-bandit = "^2.1.2"
-flake8-black = "^0.2.5"
+flake8-black = "^0.3.6"
 flake8-bugbear = "^21.9.2"
 flake8-import-order = "^0.18.1"
 safety = "^2.2.0"
 mypy = "^0.910"
 types-click = "^7.1.7"
 pytype = {version = "^2021.10.11", python = "3.7"}
 typeguard = "^2.13.0"
 flake8-annotations = "^2.0.0"
 flake8-docstrings = ">=1.6.0"
 darglint = ">=1.8.1"
 Sphinx = "^4.2.0"
-codecov = "^2.1.12"
+codecov = ">=2.1.13"
 
 [tool.poetry.scripts]
 reportseff = "reportseff.console:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reportseff-2.7.4/src/reportseff/console.py` & `reportseff-2.7.5/src/reportseff/console.py`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/src/reportseff/db_inquirer.py` & `reportseff-2.7.5/src/reportseff/db_inquirer.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 
 class SacctInquirer(BaseInquirer):
     """Implementation of BaseInquirer for the sacct slurm function."""
 
     def __init__(self) -> None:
         """Initialize a new inquirer."""
-        self.default_args = "sacct -P -n".split()
+        self.default_args = "sacct -P -n --delimiter=^|^".split()
         self.user: Optional[str] = None
         self.state: Optional[Set] = None
         self.not_state: Optional[Set] = None
         self.since: Optional[str] = None
         self.until: Optional[str] = None
         self.query_all_users: bool = False
         self.partition: Optional[str] = None
@@ -254,15 +254,16 @@
         except subprocess.CalledProcessError as error:
             raise RuntimeError(f"Error running sacct!\n{error.stderr}") from error
 
         lines = cmd_result.stdout.split("\n")
         if debug_cmd is not None:
             debug_cmd("\n".join(lines))
 
-        result = [dict(zip(columns, line.split("|"))) for line in lines if line]
+        sacct_split = re.compile(r"\^\|\^")
+        result = [dict(zip(columns, sacct_split.split(line))) for line in lines if line]
 
         if self.state:
             # split to get first word in entries like "CANCELLED BY X"
             result = [r for r in result if r["State"].split()[0] in self.state]
 
         if self.not_state:
             # split to get first word in entries like "CANCELLED BY X"
```

### Comparing `reportseff-2.7.4/src/reportseff/job.py` & `reportseff-2.7.5/src/reportseff/job.py`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/src/reportseff/job_collection.py` & `reportseff-2.7.5/src/reportseff/job_collection.py`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/src/reportseff/output_renderer.py` & `reportseff-2.7.5/src/reportseff/output_renderer.py`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/src/reportseff/parameters.py` & `reportseff-2.7.5/src/reportseff/parameters.py`

 * *Files identical despite different names*

### Comparing `reportseff-2.7.4/setup.py` & `reportseff-2.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {':python_version < "3.8"': ['importlib-metadata>=4.8.2,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['reportseff = reportseff.console:main']}
 
 setup_kwargs = {
     'name': 'reportseff',
-    'version': '2.7.4',
+    'version': '2.7.5',
     'description': 'Tablular seff output',
     'long_description': '[![Tests](https://github.com/troycomi/reportseff/workflows/Tests/badge.svg)](https://github.com/troycomi/reportseff/actions?workflow=Tests)\n[![codecov](https://codecov.io/gh/troycomi/reportseff/branch/main/graph/badge.svg)](https://codecov.io/gh/troycomi/reportseff)\n[![PyPI](https://img.shields.io/pypi/v/reportseff.svg)](https://pypi.org/project/reportseff/)\n\n# `reportseff`\n\n> A python script for tabular display of slurm efficiency information\n\n![Example](https://github.com/troycomi/reportseff/raw/main/imgs/example.png)\n\n## About\n\n### Motivation\n\nWhether a sys admin or cluster user, knowing how well you are estimating job\nresources can help streamline job scheduling and maximize your priority. If you\nhave ever tried to use `sacct` you probably had some trouble interpreting the\noutput.  While `seff` or `jobstats` can provide detailed summaries, they don\'t\nscale easily to array jobs or offer a way to see all the jobs from a single\nuser.  `reportseff` aims to fill this role.  Read more about the [motivation\nfor reportseff](https://github.com/troycomi/reportseff/blob/main/ABOUT.md).\n\n### Audience\n\nIf you are running more than one slurm job at a time, you should try\n`reportseff`.  Users of HPC systems can get an idea how well they estimate\nresource usage.  By tuning these values, you can get scheduled earlier and not\nbe penalized for unused allocations.  Since `reportseff` can parse job ids from\nslurm output files, it simplifies the task of identifying which jobs have\nfailed and why. Sys admins can pipe `reportseff` output to identify users with\npoor utilization or produce summaries at the end of a billing cycle.\n\n### Implementation\n\n`reportseff` is a wrapper around `sacct` that provides more complex option\nparsing, simpler options, and cleaner, colored outputs.  All querying is\nperformed in a single call to `sacct` and should have similar performance.\nMulti-node and GPU utilization is acquired from information contained in the\n`AdminComment` field, as generated by `jobstats`.\n\n## Usage\n\n### Installation\n\n`reportseff` runs on python >= 3.6.\nThe only external dependency is click (>= 6.7).\nCalling\n\n```sh\npip install --user reportseff\n# OR\npipx install reportseff\n```\n\nwill create command line bindings and install click.\n\n### Sample Usage\n\nTry `reportseff -u $USER` or just `reportseff` in a directory with some slurm\noutputs.  You may be surprised by your results!\n\n#### Single job\n\nCalling `reportseff` with a single jobid will provide equivalent information to\nseff for that job. `reportseff 24371789` and `reportseff map_fastq_24371789`\nproduce the following output:\n\n```txt\n   JobID      State          Elapsed   CPUEff   MemEff\n24371789    COMPLETED       03:08:03   71.2%    45.7%\n```\n\n#### Single array job\n\nProviding either the raw job id or the array job id will get efficiency\ninformation for a single element of the array job. `reportseff 24220929_421`\nand `reportseff 24221219` generate:\n\n```txt\n       JobID      State          Elapsed    CPUEff   MemEff\n24220929_421    COMPLETED       00:09:34    99.0%    34.6%\n```\n\n#### Array job group\n\nIf the base job id of an array is provided, all elements of the array will\nbe added to the output. `reportseff 24220929`\n\n```txt\n          JobID      State          Elapsed    CPUEff   MemEff\n     24220929_1    COMPLETED       00:10:43    99.2%    33.4%\n    24220929_11    COMPLETED       00:10:10    99.2%    37.5%\n    24220929_21    COMPLETED       00:09:25    98.8%    36.1%\n    24220929_31    COMPLETED       00:09:19    98.9%    33.3%\n    24220929_41    COMPLETED       00:09:23    98.9%    33.3%\n    24220929_51    COMPLETED       00:08:02    98.5%    36.3%\n    ...\n   24220929_951    COMPLETED       00:25:12    99.5%    33.5%\n   24220929_961    COMPLETED       00:39:26    99.7%    34.1%\n   24220929_971    COMPLETED       00:24:11    99.5%    34.2%\n   24220929_981    COMPLETED       00:24:50    99.5%    44.3%\n   24220929_991    COMPLETED       00:13:05    98.7%    33.7%\n```\n\n#### Glob expansion of slurm outputs\n\nBecause slurm output files can act as job id inputs, the following can\nget all seff information for a given job name:\n\n```txt\nslurm_out  ❯❯❯ reportseff split_ubam_24*\n              JobID      State          Elapsed   CPUEff   MemEff\nsplit_ubam_24342816    COMPLETED       23:30:32   99.9%    4.5%\nsplit_ubam_24342914    COMPLETED       22:40:51   99.9%    4.6%\nsplit_ubam_24393599    COMPLETED       23:43:36   99.4%    4.4%\nsplit_ubam_24393655    COMPLETED       21:36:58   99.3%    4.5%\nsplit_ubam_24418960     RUNNING        02:53:11    ---      ---\nsplit_ubam_24419972     RUNNING        01:26:26    ---      ---\n```\n\n#### No arguments\n\nWithout arguments, reportseff will try to find slurm output files in the\ncurrent directory. Combine with `watch` to monitor job progress:\n`watch -cn 300 reportseff --color --modified-sort`\n\n```txt\n                JobID           State          Elapsed   CPUEff   MemEff\n   split_ubam_24418960          RUNNING        02:56:14    ---      ---\nfastq_to_ubam_24419971          RUNNING        01:29:29    ---      ---\n   split_ubam_24419972          RUNNING        01:29:29    ---      ---\nfastq_to_ubam_24393600         COMPLETED     1-02:00:47   58.3%    41.1%\n    map_fastq_24419330          RUNNING        02:14:53    ---      ---\n    map_fastq_24419323          RUNNING        02:15:24    ---      ---\n    map_fastq_24419324          RUNNING        02:15:24    ---      ---\n    map_fastq_24419322          RUNNING        02:15:24    ---      ---\nmark_adapters_24418437         COMPLETED       01:29:23   99.8%    48.2%\nmark_adapters_24418436         COMPLETED       01:29:03   99.9%    47.4%\n```\n\n#### Filtering slurm output files\n\nOne useful application of `reportseff` is filtering a directory of slurm output\nfiles based on the state or time since running. Additionally, if only the\n`jobid` is specified as a format output, the filenames will be returned in a\npipe-friendly manner:\n\n```txt\nold_runs   ❯❯❯ reportseff --since d=4 --state Timeout\n\n                 JobID   State      Elapsed  CPUEff   MemEff\ncall_variants_31550458  TIMEOUT    20:05:17  99.5%     0.0%\ncall_variants_31550474  TIMEOUT    20:05:17  99.6%     0.0%\ncall_variants_31550500  TIMEOUT    20:05:08  99.7%     0.0%\nold_runs   ❯❯❯ reportseff --since d=4 --state Timeout --format jobid\ncall_variants_31550458\ncall_variants_31550474\ncall_variants_31550500\n```\n\nTo find all lines with `output:` in jobs which have timed out or failed\nin the last 4 days:\n\n```sh\nreportseff --since \'d=4\' --state TO,F --format jobid | xargs grep output:\n```\n\n### Arguments\n\nJobs can be passed as arguments in the following ways:\n\n- Job ID such as 1234567.  If the id is part of an array job, only the element\nfor that ID will be displayed.  If the id is the base part of an array job,\nall elements in the array will be displayed.\n- Array Job ID such as 1234567\\_89.  Will display only the element specified.\n- Slurm output file.  Format must be BASE\\_%A\\_%a.  BASE is optional as is a\n\'.out\' suffix.  Unix glob expansions can also be used to filter which jobs\nare displayed.\n- From current directory.  If no argument is supplied, `reportseff` will attempt\nto find slurm output files in the current directory as described above.\nIf a user is provided, instead `reportseff` will show recent jobs for that user.\nIf only `since` is set, all recent jobs for all users will be shown (if allowed).\n- Supplying a directory as a single argument will override the current\ndirectory to check for slurm outputs.\n\n### Options\n\n- `--color/--no-color`: Force color output or not.  By default, will force color\n  output.  With the no-color flag, click will strip color codes for everything\n  besides stdout.\n- `--modified-sort`: Instead of sorting by filename/jobid, sort by last\n  modification time of the slurm output file.\n- `--debug`: Write sacct result to stderr.\n- `--user/-u`: Ignore job arguments and instead query sacct with provided user.\n  Returns all jobs from the last week.\n- `--state/-s`: Output only jobs with states matching one of the provided options.\n  Accepts comma separated values of job codes (e.g. \'R\') or full names\n  (e.g. RUNNING).  Case insensitive.\n- `--not-state/-S`: Output only jobs with states not matching any of the provided options.\n  Accepts comma separated values of job codes (e.g. \'R\') or full names\n  (e.g. RUNNING).  Case insensitive.\n- `--format`: Provide a comma separated list of columns to produce. Prefixing the\n  argument with `+` adds the specified values to the defaults.  Values can\n  be any valid column name to sacct and the custom efficiency values: TimeEff,\n  cpuEff, MemEff.  Can also optionally set alignment (<, ^, >) and maximum width.\n  Default is center-aligned with a width of the maximum column entry.  For\n  example, `--format \'jobid%>,state%10,memeff%<5\'` produces 3 columns with:\n  - JobId aligned right, width set automatically\n  - State with width 10 (center aligned by default)\n  - MemEff aligned left, width 5\n- `--slurm-format`: The filename pattern passed to sbatch during job submission.\n  Overrides the default regex for job id parsing from filenames.  E.g. to match\n  filenames like `123456.out` set `--slurm-format %j.out`.\n- `--since`: Limit results to those occurring after the specified time.  Accepts\n  sacct formats and a comma separated list of key/value pairs.  To get jobs in\n  the last hour and a half, can pass `h=1,m=30`.\n-`--until`: Limit results to those occurring before the specified time. Accepts\n  sacct formats and a comma separated list of key/value pairs.\n  Useful in combination with the \'since\' option to query a specific range.\n- `--partition`: Limit results to a specific partition.\n- `--node/-n`: Display information for multi-node jobs; requires additional\n  sacct fields from jobstats.\n- `--node-and-gpu/-g`: Display information for multi-node jobs and GPU information;\n  requires additional sacct fields from jobstats.\n- `--parsable/-p`: Ignore formatting and output as a `|` delimited table.  Useful\n  for piping into more complex analyses.\n\n## Status, Contributions, and Support\n\n`reportseff` is actively maintained but currently feature complete.  If there\nis a function missing, please open an issue to discuss its merit!\n\nBug reports, pull requests, and any feedback are welcome! Prior to submitting\na pull request, be sure any new features have been tested and all unit tests\nare passing. In the cloned repo with\n[poetry](https://github.com/python-poetry/poetry#installation) installed:\n\n```sh\npoetry install\npoetry run pytest\npoetry run pre-commit install\nnox\n```\n\n## Troubleshooting\n\n### I can\'t install, what is pip?\n\n[pip](https://pip.pypa.io/en/stable/) is the package installer for python.  If\nyou get an error that pip isn\'t found, look for a python/anaconda/conda module.\n[pipx](https://pypa.github.io/pipx/) ensures that each application is installed\nin an isolated environment.  This resolves issues of dependency versions and\nallows applications to be run from any environment.\n\n### The output has no color with many jobs!\n\nClick should determine if the output supports color display and react automatically\nin a way you expect.  Check that your terminal is setup to display colors and\nthat your pager (probably less) will display color by default.  Some commands,\ne.g. `watch` aren\'t handled properly even when invoked to support color.  Here\nare some useful settings for your `.bashrc`:\n```\n# have less display colors by default.  Will fix `reportseff` not showing colors\nexport LESS="-R"\n# for watch aliases, include the `--color` option\nwatch -cn 300 reportseff --color --modified-sort\n#      ^                 ^^^^^^^\n```\nYou can always for display of color (or suppress it) with the `--color/--no-color`\noptions\n\n### I get an error about broken pipes when chaining to other commands\n\nPython will report that the consumer of process output has closed the stream\n(i.e. the pipe) while still attempting to write.  Newer versions of click\nshould suppress the warning output, but it seems to not always work.  Besides\nsome extra printing on stderr, the output is not affected.\n\n### My jobs don\'t have any information about multiple nodes or GPU efficiency\n\nBecause `sacct` doesn\'t currently record this information, `reportseff`\nretrieves it from a custom field from `jobstats`, developed at Princeton\nUniversity.  If you are outside a Research Computing cluster, that information\nwill likely be absent.  Node-level reporting is only shown for jobs which use\nmultiple nodes or GPUs.  If you need a list of where jobs were run, you can add\n`--format +NodeList`.\n\n## Acknowledgments\n\nThe code for calling sacct and parsing the returning information was taken\nfrom [Slurmee](https://github.com/PrincetonUniversity/slurmee).\n\nStyle and tooling from [hypermodern python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)\n\nCode review provided from a [repo-review](https://researchcomputing.princeton.edu/services/repo-review-consultations)\nwhich vastly improved this readme.\n',
     'author': 'Troy Comi',
     'author_email': 'troycomi@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/troycomi/reportseff',
```

### Comparing `reportseff-2.7.4/PKG-INFO` & `reportseff-2.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportseff
-Version: 2.7.4
+Version: 2.7.5
 Summary: Tablular seff output
 Home-page: https://github.com/troycomi/reportseff
 License: MIT
 Keywords: slurm,seff
 Author: Troy Comi
 Author-email: troycomi@gmail.com
 Requires-Python: >=3.7.0,<4.0
```

