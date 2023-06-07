# Comparing `tmp/pycarl-2.0.4.tar.gz` & `tmp/pycarl-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycarl-2.0.4.tar", last modified: Fri Dec 13 15:51:33 2019, max compression
+gzip compressed data, was "pycarl-2.2.0.tar", last modified: Wed Jun  7 20:03:46 2023, max compression
```

## Comparing `pycarl-2.0.4.tar` & `pycarl-2.2.0.tar`

### file list

```diff
@@ -1,290 +1,113 @@
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:33.000000 pycarl-2.0.4/
--rw-r--r--   0 mvolk      (502) staff       (20)     3867 2019-06-19 13:51:37.000000 pycarl-2.0.4/CMakeLists.txt
--rw-r--r--   0 mvolk      (502) staff       (20)      136 2019-06-19 13:51:37.000000 pycarl-2.0.4/MANIFEST.in
--rw-r--r--   0 mvolk      (502) staff       (20)     1353 2019-12-13 15:51:33.000000 pycarl-2.0.4/PKG-INFO
--rw-r--r--   0 mvolk      (502) staff       (20)      491 2018-03-26 09:50:05.000000 pycarl-2.0.4/README.md
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/cmake/
--rw-r--r--   0 mvolk      (502) staff       (20)      589 2019-06-19 13:51:37.000000 pycarl-2.0.4/cmake/CMakeLists.txt
--rw-r--r--   0 mvolk      (502) staff       (20)      192 2019-06-19 13:51:37.000000 pycarl-2.0.4/cmake/config.py.in
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/
--rw-r--r--   0 mvolk      (502) staff       (20)     1234 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)      124 2019-12-13 14:16:27.000000 pycarl-2.0.4/lib/pycarl/_config.py
--rw-r--r--   0 mvolk      (502) staff       (20)       22 2019-12-13 15:50:34.000000 pycarl-2.0.4/lib/pycarl/_version.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/cln/
--rw-r--r--   0 mvolk      (502) staff       (20)      951 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/cln/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)       77 2019-12-13 14:16:28.000000 pycarl-2.0.4/lib/pycarl/cln/_config.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/cln/formula/
--rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-17 15:23:55.000000 pycarl-2.0.4/lib/pycarl/cln/formula/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)       77 2019-12-13 14:16:33.000000 pycarl-2.0.4/lib/pycarl/cln/formula/_config.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/cln/parse/
--rw-r--r--   0 mvolk      (502) staff       (20)      148 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/cln/parse/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)       80 2019-12-13 14:16:40.000000 pycarl-2.0.4/lib/pycarl/cln/parse/_config.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/convert/
--rw-r--r--   0 mvolk      (502) staff       (20)      513 2018-04-17 15:23:55.000000 pycarl-2.0.4/lib/pycarl/convert/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)     7260 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/convert/cln_converter.py
--rw-r--r--   0 mvolk      (502) staff       (20)     7840 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/convert/gmp_converter.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/formula/
--rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-17 15:23:55.000000 pycarl-2.0.4/lib/pycarl/formula/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/gmp/
--rw-r--r--   0 mvolk      (502) staff       (20)      769 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/gmp/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/gmp/formula/
--rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-17 15:23:55.000000 pycarl-2.0.4/lib/pycarl/gmp/formula/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/gmp/parse/
--rw-r--r--   0 mvolk      (502) staff       (20)      148 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/gmp/parse/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)       80 2019-12-13 14:16:38.000000 pycarl-2.0.4/lib/pycarl/gmp/parse/_config.py
--rw-r--r--   0 mvolk      (502) staff       (20)     1920 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/infinity.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl/parse/
--rw-r--r--   0 mvolk      (502) staff       (20)     1586 2019-06-19 13:51:37.000000 pycarl-2.0.4/lib/pycarl/parse/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)       80 2019-12-13 14:16:37.000000 pycarl-2.0.4/lib/pycarl/parse/_config.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl.egg-info/
--rw-r--r--   0 mvolk      (502) staff       (20)     1353 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl.egg-info/PKG-INFO
--rw-r--r--   0 mvolk      (502) staff       (20)     9565 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl.egg-info/SOURCES.txt
--rw-r--r--   0 mvolk      (502) staff       (20)        1 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl.egg-info/dependency_links.txt
--rw-r--r--   0 mvolk      (502) staff       (20)        1 2019-11-05 10:12:07.000000 pycarl-2.0.4/lib/pycarl.egg-info/not-zip-safe
--rw-r--r--   0 mvolk      (502) staff       (20)       78 2019-12-13 15:51:32.000000 pycarl-2.0.4/lib/pycarl.egg-info/top_level.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1638 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/.appveyor.yml
--rwxr-xr-x   0 mvolk      (502) staff       (20)      360 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/.gitignore
--rwxr-xr-x   0 mvolk      (502) staff       (20)      100 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/.gitmodules
--rwxr-xr-x   0 mvolk      (502) staff       (20)       62 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/.readthedocs.yml
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7295 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/.travis.yml
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5827 2019-10-04 12:42:29.000000 pycarl-2.0.4/resources/pybind11/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1896 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/CONTRIBUTING.md
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1271 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/ISSUE_TEMPLATE.md
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2190 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/LICENSE
--rwxr-xr-x   0 mvolk      (502) staff       (20)       71 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/MANIFEST.in
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5896 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/README.md
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/docs/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      535 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/Doxyfile
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/docs/_static/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      254 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3895 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/chrono.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3189 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/custom.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    14276 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/eigen.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3889 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/functional.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1534 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/index.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11482 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/overview.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7236 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/stl.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9240 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/cast/strings.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    22719 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/classes.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8052 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/embedding.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7091 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/exceptions.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    22211 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/functions.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9187 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/pycpp/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      278 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/pycpp/index.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    14118 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/pycpp/numpy.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2922 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/pycpp/object.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2601 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/pycpp/utilities.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     6366 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/advanced/smart_ptrs.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8214 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/basics.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2920 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/benchmark.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3170 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/benchmark.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    27212 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/changelog.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    13014 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/classes.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9042 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/compiling.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10618 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/conf.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10045 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/faq.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)      693 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/index.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4243 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/intro.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)      879 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/limitations.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    58510 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/pybind11-logo.png
--rwxr-xr-x   0 mvolk      (502) staff       (20)    44653 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/pybind11_vs_boost_python1.png
--rwxr-xr-x   0 mvolk      (502) staff       (20)    87708 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/pybind11_vs_boost_python1.svg
--rwxr-xr-x   0 mvolk      (502) staff       (20)    41121 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/pybind11_vs_boost_python2.png
--rwxr-xr-x   0 mvolk      (502) staff       (20)    85853 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/pybind11_vs_boost_python2.svg
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1622 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/reference.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1127 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/docs/release.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)       17 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/docs/requirements.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/include/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/
--rwxr-xr-x   0 mvolk      (502) staff       (20)    18071 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/attr.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4299 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/buffer_info.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    86469 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/cast.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     6596 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/chrono.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    23813 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/class_support.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    40584 2019-10-04 12:23:52.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/common.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1949 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/complex.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7693 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/descr.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    29215 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/eigen.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7425 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/embed.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3845 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/eval.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2934 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/functional.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    65466 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/numpy.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8651 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/operators.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2004 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/options.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    81353 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/pybind11.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    48451 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/pytypes.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    12223 2019-10-04 12:26:30.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/stl.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    20849 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/stl_bind.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1402 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/include/pybind11/typeid.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/pybind11/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      336 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/pybind11/__init__.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)      791 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/pybind11/__main__.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)       77 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/pybind11/_version.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)      238 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/setup.cfg
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3646 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/setup.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7408 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)     6526 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/conftest.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11150 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/constructor_stats.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5389 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/object.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3626 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/pybind11_tests.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1252 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/pybind11_tests.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)      530 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/pytest.ini
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5830 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_buffers.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2430 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_buffers.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7020 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_builtin_casters.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7948 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_builtin_casters.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3337 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_call_policies.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5118 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_call_policies.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5769 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_callbacks.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4380 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_callbacks.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2100 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_chrono.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3402 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_chrono.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10033 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_class.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4550 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_class.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2042 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      654 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/installed_embed/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      686 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/installed_function/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      474 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/installed_target/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1056 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      152 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/subdirectory_embed/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      327 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/subdirectory_function/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      373 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/subdirectory_target/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      695 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      142 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_cmake_build/test.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3330 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_constants_and_functions.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1100 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_constants_and_functions.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8897 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_copy_move.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5103 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_copy_move.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2284 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_docstring_options.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1705 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_docstring_options.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16268 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_eigen.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    28676 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tests/test_embed/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1234 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_embed/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      414 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_embed/catch.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7675 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_embed/test_interpreter.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)      195 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_embed/test_interpreter.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1863 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_enum.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4144 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_enum.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2377 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_eval.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)      560 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_eval.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)      119 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tests/test_eval_call.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5889 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_exceptions.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2897 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_exceptions.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3026 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_kwargs_and_defaults.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4618 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_kwargs_and_defaults.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    17753 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_methods_and_attributes.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16018 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_methods_and_attributes.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3283 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_modules.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2208 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_modules.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7853 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_multiple_inheritance.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9277 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_multiple_inheritance.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    12169 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_numpy_array.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16119 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_numpy_array.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    15916 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_numpy_dtypes.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11824 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_numpy_dtypes.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3440 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_numpy_vectorize.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8887 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_numpy_vectorize.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2241 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_opaque_types.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1869 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_opaque_types.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5350 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_operator_overloading.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3442 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_operator_overloading.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2945 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_pickling.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)      834 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_pickling.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8189 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_pytypes.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5777 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_pytypes.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11959 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_sequences_and_iterators.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5189 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_sequences_and_iterators.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    12371 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_smart_ptr.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8732 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_smart_ptr.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5883 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_stl.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5124 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_stl.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3780 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_stl_binders.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4850 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_stl_binders.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16682 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_virtual_functions.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11020 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tests/test_virtual_functions.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/resources/pybind11/tools/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2100 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tools/FindCatch.cmake
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2995 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tools/FindEigen3.cmake
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7998 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2308 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tools/check-style.sh
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1098 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tools/libsize.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10341 2018-03-26 09:50:05.000000 pycarl-2.0.4/resources/pybind11/tools/mkdoc.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3978 2019-06-19 13:51:37.000000 pycarl-2.0.4/resources/pybind11/tools/pybind11Config.cmake.in
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8321 2019-10-04 12:26:04.000000 pycarl-2.0.4/resources/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/setup/
--rw-r--r--   0 mvolk      (502) staff       (20)       26 2019-06-19 13:51:37.000000 pycarl-2.0.4/setup/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)     2469 2019-06-19 13:51:37.000000 pycarl-2.0.4/setup/config.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1936 2019-06-19 13:51:37.000000 pycarl-2.0.4/setup/helper.py
--rw-r--r--   0 mvolk      (502) staff       (20)      226 2019-12-13 15:51:33.000000 pycarl-2.0.4/setup.cfg
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10271 2019-08-06 08:19:59.000000 pycarl-2.0.4/setup.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/src/
--rw-r--r--   0 mvolk      (502) staff       (20)     1218 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/common.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/src/core/
--rw-r--r--   0 mvolk      (502) staff       (20)      313 2018-05-02 15:31:42.000000 pycarl-2.0.4/src/core/bound_type.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       77 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/core/bound_type.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2011 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/core/monomial.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      241 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/core/monomial.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3891 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/core/variable.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      282 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/core/variable.h
--rw-r--r--   0 mvolk      (502) staff       (20)       27 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/definitions.h.in
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:32.000000 pycarl-2.0.4/src/formula/
--rw-r--r--   0 mvolk      (502) staff       (20)     1028 2018-05-02 15:31:30.000000 pycarl-2.0.4/src/formula/formula_type.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       79 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/formula/formula_type.h
--rw-r--r--   0 mvolk      (502) staff       (20)      496 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/formula/relation.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       76 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/formula/relation.h
--rw-r--r--   0 mvolk      (502) staff       (20)      279 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/helpers.h
--rw-r--r--   0 mvolk      (502) staff       (20)      745 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/mod_cln.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      348 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/mod_core.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      296 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/mod_formula.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      745 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/mod_gmp.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      896 2018-05-02 15:35:54.000000 pycarl-2.0.4/src/mod_parse.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      362 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/mod_typed_formula.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)     1093 2018-05-02 15:35:42.000000 pycarl-2.0.4/src/mod_typed_parse.cpp
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:33.000000 pycarl-2.0.4/src/typed_core/
--rw-r--r--   0 mvolk      (502) staff       (20)     1352 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/factorization.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      232 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/factorization.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2793 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/factorizedpolynomial.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      213 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/factorizedpolynomial.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2358 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/factorizedrationalfunction.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      331 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/factorizedrationalfunction.h
--rw-r--r--   0 mvolk      (502) staff       (20)     8606 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/integer.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      118 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/integer.h
--rw-r--r--   0 mvolk      (502) staff       (20)     4248 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/interval.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       76 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/interval.h
--rw-r--r--   0 mvolk      (502) staff       (20)     5596 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/polynomial.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      251 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/polynomial.h
--rw-r--r--   0 mvolk      (502) staff       (20)    13726 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/rational.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      286 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/rational.h
--rw-r--r--   0 mvolk      (502) staff       (20)     5512 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/rationalfunction.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      281 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/rationalfunction.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3437 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_core/term.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      221 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_core/term.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:33.000000 pycarl-2.0.4/src/typed_formula/
--rw-r--r--   0 mvolk      (502) staff       (20)      236 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_formula/common.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3589 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_formula/constraint.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      202 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_formula/constraint.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3152 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_formula/formula.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       75 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_formula/formula.h
--rw-r--r--   0 mvolk      (502) staff       (20)      375 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_formula/types.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:33.000000 pycarl-2.0.4/src/typed_parse/
--rw-r--r--   0 mvolk      (502) staff       (20)      214 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/typed_parse/parser.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)     1456 2019-06-19 13:51:37.000000 pycarl-2.0.4/src/typed_parse/parser.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-13 15:51:33.000000 pycarl-2.0.4/src/types/
--rw-r--r--   0 mvolk      (502) staff       (20)      132 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/types/cln_types.h
--rw-r--r--   0 mvolk      (502) staff       (20)      103 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/types/gmp_types.h
--rw-r--r--   0 mvolk      (502) staff       (20)      919 2018-03-26 09:50:05.000000 pycarl-2.0.4/src/types.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.647215 pycarl-2.2.0/
+-rw-r--r--   0 mvolk      (502) staff       (20)     6173 2023-04-03 19:03:27.000000 pycarl-2.2.0/CMakeLists.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)      136 2022-03-15 21:58:32.000000 pycarl-2.2.0/MANIFEST.in
+-rw-r--r--   0 mvolk      (502) staff       (20)     1562 2023-06-07 20:03:46.647593 pycarl-2.2.0/PKG-INFO
+-rw-r--r--   0 mvolk      (502) staff       (20)      838 2023-05-01 11:59:57.000000 pycarl-2.2.0/README.md
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.553657 pycarl-2.2.0/cmake/
+-rw-r--r--   0 mvolk      (502) staff       (20)      588 2023-04-03 19:03:28.000000 pycarl-2.2.0/cmake/CMakeLists.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)       60 2022-09-01 17:21:45.000000 pycarl-2.2.0/cmake/cln_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)      192 2022-08-02 14:46:05.000000 pycarl-2.2.0/cmake/config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)      166 2022-09-07 21:39:00.000000 pycarl-2.2.0/cmake/core_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)       66 2022-09-01 17:21:45.000000 pycarl-2.2.0/cmake/parser_config.py.in
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.543318 pycarl-2.2.0/lib/
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.556575 pycarl-2.2.0/lib/pycarl/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1234 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      122 2023-05-01 11:58:58.000000 pycarl-2.2.0/lib/pycarl/_config.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       22 2023-06-07 19:38:50.000000 pycarl-2.2.0/lib/pycarl/_version.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.563741 pycarl-2.2.0/lib/pycarl/cln/
+-rw-r--r--   0 mvolk      (502) staff       (20)      951 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/cln/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       49 2023-04-05 08:21:06.000000 pycarl-2.2.0/lib/pycarl/cln/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.565141 pycarl-2.2.0/lib/pycarl/cln/formula/
+-rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-17 15:23:55.000000 pycarl-2.2.0/lib/pycarl/cln/formula/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       49 2023-04-05 08:21:06.000000 pycarl-2.2.0/lib/pycarl/cln/formula/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.567301 pycarl-2.2.0/lib/pycarl/cln/parse/
+-rw-r--r--   0 mvolk      (502) staff       (20)      148 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/cln/parse/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       52 2023-04-05 08:21:06.000000 pycarl-2.2.0/lib/pycarl/cln/parse/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.570518 pycarl-2.2.0/lib/pycarl/convert/
+-rw-r--r--   0 mvolk      (502) staff       (20)      513 2018-04-17 15:23:55.000000 pycarl-2.2.0/lib/pycarl/convert/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     7260 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/convert/cln_converter.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     7840 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/convert/gmp_converter.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.571418 pycarl-2.2.0/lib/pycarl/formula/
+-rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-17 15:23:55.000000 pycarl-2.2.0/lib/pycarl/formula/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.572327 pycarl-2.2.0/lib/pycarl/gmp/
+-rw-r--r--   0 mvolk      (502) staff       (20)      769 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/gmp/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.573333 pycarl-2.2.0/lib/pycarl/gmp/formula/
+-rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-17 15:23:55.000000 pycarl-2.2.0/lib/pycarl/gmp/formula/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.575451 pycarl-2.2.0/lib/pycarl/gmp/parse/
+-rw-r--r--   0 mvolk      (502) staff       (20)      148 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/gmp/parse/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       52 2023-04-05 08:21:06.000000 pycarl-2.2.0/lib/pycarl/gmp/parse/_config.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     1920 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/infinity.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.578929 pycarl-2.2.0/lib/pycarl/parse/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1586 2022-03-15 21:58:32.000000 pycarl-2.2.0/lib/pycarl/parse/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       52 2023-04-05 08:21:06.000000 pycarl-2.2.0/lib/pycarl/parse/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.562318 pycarl-2.2.0/lib/pycarl.egg-info/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1562 2023-06-07 20:03:46.000000 pycarl-2.2.0/lib/pycarl.egg-info/PKG-INFO
+-rw-r--r--   0 mvolk      (502) staff       (20)     2317 2023-06-07 20:03:46.000000 pycarl-2.2.0/lib/pycarl.egg-info/SOURCES.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)        1 2023-06-07 20:03:46.000000 pycarl-2.2.0/lib/pycarl.egg-info/dependency_links.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)        1 2023-04-05 08:21:04.000000 pycarl-2.2.0/lib/pycarl.egg-info/not-zip-safe
+-rw-r--r--   0 mvolk      (502) staff       (20)       37 2023-06-07 20:03:46.000000 pycarl-2.2.0/lib/pycarl.egg-info/requires.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)       78 2023-06-07 20:03:46.000000 pycarl-2.2.0/lib/pycarl.egg-info/top_level.txt
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.580029 pycarl-2.2.0/resources/
+-rw-r--r--   0 mvolk      (502) staff       (20)      496 2022-09-07 21:39:00.000000 pycarl-2.2.0/resources/include_pybind11.cmake
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.585188 pycarl-2.2.0/setup/
+-rw-r--r--   0 mvolk      (502) staff       (20)       26 2022-03-15 21:58:32.000000 pycarl-2.2.0/setup/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     2502 2022-09-07 21:39:00.000000 pycarl-2.2.0/setup/config.py
+-rwxr-xr-x   0 mvolk      (502) staff       (20)     1936 2022-03-15 21:58:32.000000 pycarl-2.2.0/setup/helper.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      226 2023-06-07 20:03:46.649655 pycarl-2.2.0/setup.cfg
+-rwxr-xr-x   0 mvolk      (502) staff       (20)     9798 2023-06-07 19:34:04.000000 pycarl-2.2.0/setup.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.605785 pycarl-2.2.0/src/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1218 2022-03-15 21:58:32.000000 pycarl-2.2.0/src/common.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.611445 pycarl-2.2.0/src/core/
+-rw-r--r--   0 mvolk      (502) staff       (20)      313 2018-05-02 15:31:42.000000 pycarl-2.2.0/src/core/bound_type.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       77 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/core/bound_type.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2110 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/core/monomial.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      241 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/core/monomial.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3670 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/core/variable.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      282 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/core/variable.h
+-rw-r--r--   0 mvolk      (502) staff       (20)       27 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/definitions.h.in
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.615099 pycarl-2.2.0/src/formula/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1028 2018-05-02 15:31:30.000000 pycarl-2.2.0/src/formula/formula_type.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       79 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/formula/formula_type.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      567 2023-03-22 15:20:12.000000 pycarl-2.2.0/src/formula/relation.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       76 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/formula/relation.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      279 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/helpers.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      745 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/mod_cln.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      348 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/mod_core.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      296 2022-03-15 21:58:32.000000 pycarl-2.2.0/src/mod_formula.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      745 2022-03-15 21:58:32.000000 pycarl-2.2.0/src/mod_gmp.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      896 2018-05-02 15:35:54.000000 pycarl-2.2.0/src/mod_parse.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      362 2022-03-15 21:58:32.000000 pycarl-2.2.0/src/mod_typed_formula.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)     1093 2018-05-02 15:35:42.000000 pycarl-2.2.0/src/mod_typed_parse.cpp
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.633011 pycarl-2.2.0/src/typed_core/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1560 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/factorization.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      232 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/factorization.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2875 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/factorizedpolynomial.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      213 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/factorizedpolynomial.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2440 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/factorizedrationalfunction.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      331 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/factorizedrationalfunction.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     8313 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/integer.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      118 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/integer.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     4330 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/interval.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       76 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/interval.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     5678 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/polynomial.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      251 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/polynomial.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    13020 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/rational.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      286 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/rational.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     5606 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/rationalfunction.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      281 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/rationalfunction.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3519 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_core/term.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      221 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_core/term.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.638249 pycarl-2.2.0/src/typed_formula/
+-rw-r--r--   0 mvolk      (502) staff       (20)      236 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_formula/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3835 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_formula/constraint.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      202 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_formula/constraint.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3232 2022-07-31 14:16:03.000000 pycarl-2.2.0/src/typed_formula/formula.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       75 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_formula/formula.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      375 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_formula/types.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.640616 pycarl-2.2.0/src/typed_parse/
+-rw-r--r--   0 mvolk      (502) staff       (20)      214 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/typed_parse/parser.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)     1456 2022-03-15 21:58:32.000000 pycarl-2.2.0/src/typed_parse/parser.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-07 20:03:46.646025 pycarl-2.2.0/src/types/
+-rw-r--r--   0 mvolk      (502) staff       (20)      132 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/types/cln_types.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      103 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/types/gmp_types.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      919 2018-03-26 09:50:05.000000 pycarl-2.2.0/src/types.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycarl-2.0.4/PKG-INFO` & `pycarl-2.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pycarl
-Version: 2.0.4
+Version: 2.2.0
 Summary: pycarl - Python Bindings for CArL
 Home-page: https://github.com/moves-rwth/pycarl/
 Author: S. Junges
 Author-email: sebastian.junges@cs.rwth-aachen.de
 Maintainer: M. Volk
 Maintainer-email: matthias.volk@cs.rwth-aachen.de
-License: UNKNOWN
 Project-URL: Documentation, https://moves-rwth.github.io/pycarl/
 Project-URL: Source, https://github.com/moves-rwth/pycarl/
 Project-URL: Bug reports, https://github.com/moves-rwth/pycarl/issues
-Description: Pycarl - Python Bindings for CArL
-        =================================
-        
-        [![Build Status](https://travis-ci.org/moves-rwth/pycarl.svg?branch=master)](https://travis-ci.org/moves-rwth/pycarl)
-        
-        Python bindings for [CArL](https://github.com/smtrat/carl), created using [PyBind11](http://pybind11.readthedocs.io/en/stable/intro.html).
-        
-        For more information, please check the [documentation](https://moves-rwth.github.io/pycarl/).
-        
-        ### Authors:
-        
-        - Harold Bruintjes
-        - Sebastian Junges
-        - Matthias Volk
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: doc
+
+Pycarl - Python Bindings for CArL
+=================================
+
+[![Build Status](https://github.com/moves-rwth/pycarl/workflows/Build%20Test/badge.svg)](https://github.com/moves-rwth/pycarl/actions)
+[![GitHub release](https://img.shields.io/github/release/moves-rwth/pycarl.svg)](https://github.com/moves-rwth/pycarl/releases/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7763164.svg)](https://doi.org/10.5281/zenodo.7763164)
+
+Python bindings for [CArL](https://github.com/moves-rwth/carl-storm), created using [PyBind11](http://pybind11.readthedocs.io/en/stable/intro.html).
+
+For more information, please check the [documentation](https://moves-rwth.github.io/pycarl/).
+
+### Authors:
+
+Main developers:
+- Sebastian Junges
+- Matthias Volk
+
+The development of pycarl received significant contributions from:
+- Harold Bruintjes
```

### Comparing `pycarl-2.0.4/cmake/CMakeLists.txt` & `pycarl-2.2.0/cmake/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 find_package(carlparser QUIET)
 
 
 # Set configuration
 set(CARL_DIR ${carl_DIR})
 set(CARL_VERSION ${carl_VERSION})
 if(carlparser_FOUND)
-    set(CARL_PARSER_DIR ${carl_parser_DIR})
+    set(CARL_PARSER_DIR ${carlparser_DIR})
     set(CARL_WITH_PARSER "True")
 else()
     set(CARL_PARSER_DIR "")
     set(CARL_WITH_PARSER "False")
 endif()
 if(CARL_USE_CLN_NUMBERS)
     set(CARL_WITH_CLN "True")
```

### Comparing `pycarl-2.0.4/lib/pycarl/__init__.py` & `pycarl-2.2.0/lib/pycarl/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/cln/__init__.py` & `pycarl-2.2.0/lib/pycarl/cln/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/convert/__init__.py` & `pycarl-2.2.0/lib/pycarl/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/convert/cln_converter.py` & `pycarl-2.2.0/lib/pycarl/convert/cln_converter.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/convert/gmp_converter.py` & `pycarl-2.2.0/lib/pycarl/convert/gmp_converter.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/gmp/__init__.py` & `pycarl-2.2.0/lib/pycarl/gmp/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/infinity.py` & `pycarl-2.2.0/lib/pycarl/infinity.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl/parse/__init__.py` & `pycarl-2.2.0/lib/pycarl/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/lib/pycarl.egg-info/PKG-INFO` & `pycarl-2.2.0/lib/pycarl.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pycarl
-Version: 2.0.4
+Version: 2.2.0
 Summary: pycarl - Python Bindings for CArL
 Home-page: https://github.com/moves-rwth/pycarl/
 Author: S. Junges
 Author-email: sebastian.junges@cs.rwth-aachen.de
 Maintainer: M. Volk
 Maintainer-email: matthias.volk@cs.rwth-aachen.de
-License: UNKNOWN
 Project-URL: Documentation, https://moves-rwth.github.io/pycarl/
 Project-URL: Source, https://github.com/moves-rwth/pycarl/
 Project-URL: Bug reports, https://github.com/moves-rwth/pycarl/issues
-Description: Pycarl - Python Bindings for CArL
-        =================================
-        
-        [![Build Status](https://travis-ci.org/moves-rwth/pycarl.svg?branch=master)](https://travis-ci.org/moves-rwth/pycarl)
-        
-        Python bindings for [CArL](https://github.com/smtrat/carl), created using [PyBind11](http://pybind11.readthedocs.io/en/stable/intro.html).
-        
-        For more information, please check the [documentation](https://moves-rwth.github.io/pycarl/).
-        
-        ### Authors:
-        
-        - Harold Bruintjes
-        - Sebastian Junges
-        - Matthias Volk
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: doc
+
+Pycarl - Python Bindings for CArL
+=================================
+
+[![Build Status](https://github.com/moves-rwth/pycarl/workflows/Build%20Test/badge.svg)](https://github.com/moves-rwth/pycarl/actions)
+[![GitHub release](https://img.shields.io/github/release/moves-rwth/pycarl.svg)](https://github.com/moves-rwth/pycarl/releases/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7763164.svg)](https://doi.org/10.5281/zenodo.7763164)
+
+Python bindings for [CArL](https://github.com/moves-rwth/carl-storm), created using [PyBind11](http://pybind11.readthedocs.io/en/stable/intro.html).
+
+For more information, please check the [documentation](https://moves-rwth.github.io/pycarl/).
+
+### Authors:
+
+Main developers:
+- Sebastian Junges
+- Matthias Volk
+
+The development of pycarl received significant contributions from:
+- Harold Bruintjes
```

### Comparing `pycarl-2.0.4/setup/config.py` & `pycarl-2.2.0/setup/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         return {
             "carl_dir": "",
             "carl_parser_dir": "",
             "disable_cln": False,
             "disable_parser": False,
             "debug": False,
             "jobs": str(no_jobs),
+            "pybind_version": ""
         }
 
     def load_from_file(self, path):
         """
         Load config from file.
         :param path Path to config file.
         """
```

### Comparing `pycarl-2.0.4/setup/helper.py` & `pycarl-2.2.0/setup/helper.py`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/setup.py` & `pycarl-2.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import os
 import sys
 import subprocess
 import datetime
 
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
-from distutils.version import StrictVersion
 
 import setup.helper as setup_helper
 from setup.config import SetupConfig
 
 if sys.version_info[0] == 2:
     sys.exit('Sorry, Python 2.x is not supported')
 
 # Minimal carl version required
-carl_min_version = "17.12"
-carl_max_version = "19.12"
-carl_master14_version = "14."
+carl_min_version = "14.23"
+carl_storm_version_prefix = "14."
+pybind_version_default = "2.10.0"
 
 # Get the long description from the README file
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 class CMakeExtension(Extension):
-    def __init__(self, name, sourcedir='', subdir=''):
+    def __init__(self, name, sourcedir=''):
         Extension.__init__(self, name, sources=[])
         self.sourcedir = os.path.abspath(sourcedir)
-        self.subdir = subdir
 
 
 class CMakeBuild(build_ext):
     user_options = build_ext.user_options + [
         ('carl-dir=', None, 'Path to carl root (binary) location'),
         ('carl-parser-dir=', None, 'Path to carl-parser root (binary) location'),
         ('disable-cln', None, 'Disable support for CLN'),
         ('disable-parser', None, 'Disable parsing support'),
         ('debug', None, 'Build in Debug mode'),
         ('jobs=', 'j', 'Number of jobs to use for compiling'),
+        ('pybind-version=', None, 'Pybind11 version to use'),
     ]
 
     config = SetupConfig()
 
     def _extdir(self, extname):
         return os.path.abspath(os.path.dirname(self.get_ext_fullpath(extname)))
 
@@ -49,141 +48,136 @@
         try:
             _ = subprocess.check_output(['cmake', '--version'])
         except OSError:
             raise RuntimeError("CMake must be installed to build the following extensions: " +
                                ", ".join(e.name for e in self.extensions))
 
         # Build cmake version info
+        print("Pycarl - Building into {}".format(self.build_temp))
         build_temp_version = self.build_temp + "-version"
         setup_helper.ensure_dir_exists(build_temp_version)
 
         # Write config
-        setup_helper.ensure_dir_exists("build")
-        self.config.write_config("build/build_config.cfg")
+        setup_helper.ensure_dir_exists(self.build_temp)
+        self.config.write_config(os.path.join(self.build_temp, "build_config.cfg"))
 
         cmake_args = []
         carl_dir = os.path.expanduser(self.config.get_as_string("carl_dir"))
         carl_parser_dir = os.path.expanduser(self.config.get_as_string("carl_parser_dir"))
         if carl_dir:
             cmake_args += ['-Dcarl_DIR=' + carl_dir]
         if carl_parser_dir:
-            cmake_args += ['-Dcarl_parser_DIR=' + carl_parser_dir]
-        output = subprocess.check_output(['cmake', os.path.abspath("cmake")] + cmake_args, cwd=build_temp_version)
+            cmake_args += ['-Dcarlparser_DIR=' + carl_parser_dir]
+        _ = subprocess.check_output(['cmake', os.path.abspath("cmake")] + cmake_args, cwd=build_temp_version)
         cmake_conf = setup_helper.load_cmake_config(os.path.join(build_temp_version, 'generated/config.py'))
 
         # Set carl directory
         if carl_dir == "":
             carl_dir = cmake_conf.CARL_DIR
         if carl_dir != cmake_conf.CARL_DIR:
-            print("Pycarl - Warning: Using different carl directory {} instead of given {}!".format(cmake_conf.CARL_DIR,
-                                                                                                    carl_dir))
+            print("Pycarl - WARNING: Using different carl directory {} instead of given {}!".format(cmake_conf.CARL_DIR, carl_dir))
             carl_dir = cmake_conf.CARL_DIR
         # Set carl-parser directory
         if carl_parser_dir == "":
             carl_parser_dir = cmake_conf.CARL_PARSER_DIR
         if carl_parser_dir != cmake_conf.CARL_PARSER_DIR:
-            print("Pycarl - Warning: Using different carl-parser directory {} instead of given {}!".format(
-                cmake_conf.CARL_PARSER_DIR, carl_parser_dir))
+            print("Pycarl - WARNING: Using different carl-parser directory {} instead of given {}!".format(cmake_conf.CARL_PARSER_DIR, carl_parser_dir))
             carl_parser_dir = cmake_conf.CARL_PARSER_DIR
 
         # Check version
+        from packaging.version import Version  # Need to import here because otherwise packaging cannot be automatically installed as required dependency
         carl_version, carl_commit = setup_helper.parse_carl_version(cmake_conf.CARL_VERSION)
-        if carl_version.startswith(carl_master14_version):
-            print("Pycarl - Using carl with master14 branch.")
-        elif StrictVersion(carl_version) < StrictVersion(carl_min_version):
+        if not carl_version.startswith(carl_storm_version_prefix):
+            print("Pycarl - We only support carl-storm (https://github.com/moves-rwth/carl-storm) indicated by version 14.x. On this system, we only found version {} at {}".format(
+                carl_version, carl_dir))
+        elif Version(carl_version) < Version(carl_min_version):
             sys.exit("Pycarl - Error: carl version {} from '{}' is not supported anymore!".format(carl_version, carl_dir))
-        elif StrictVersion(carl_version) > StrictVersion(carl_max_version):
-            sys.exit("Pycarl - Error: carl version {} from '{}' is not supported!".format(carl_version, carl_dir))
 
         # Check additional support
-        use_cln = cmake_conf.CARL_WITH_CLN and not self.config.get_as_bool("disable_cln")
-        use_parser = cmake_conf.CARL_WITH_PARSER and not self.config.get_as_bool("disable_parser")
+        enable_parser = not self.config.get_as_bool("disable_parser")
+        enable_cln = not self.config.get_as_bool("disable_cln")
+        use_parser = enable_parser and cmake_conf.CARL_WITH_PARSER
+        use_cln = enable_cln and cmake_conf.CARL_WITH_CLN
+
+        # Set pybind version
+        pybind_version = self.config.get_as_string("pybind_version")
+        if pybind_version == "":
+            pybind_version = pybind_version_default
 
         # Print build info
         print("Pycarl - Using carl {} from {}".format(carl_version, carl_dir))
+        print("Pycarl - Using pybind11 version {}".format(pybind_version))
         if use_parser:
             print("Pycarl - carl parser extension from {} included.".format(carl_parser_dir))
         else:
-            print("Pycarl - Warning: No parser support!")
+            print("Pycarl - WARNING: No parser support!")
         if use_cln:
             print("Pycarl - Support for CLN found and included.")
         else:
-            print("Pycarl - Warning: No support for CLN!")
+            print("Pycarl - WARNING: No support for CLN!")
 
-        # Set general cmake build options
         build_type = 'Debug' if self.config.get_as_bool("debug") else 'Release'
-        cmake_args = ['-DPYTHON_EXECUTABLE=' + sys.executable]
+        # Set cmake build options
+        cmake_args = ['-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + self._extdir("core")]
+        cmake_args += ['-DPYTHON_EXECUTABLE=' + sys.executable]
         cmake_args += ['-DCMAKE_BUILD_TYPE=' + build_type]
+        cmake_args += ['-DPYBIND_VERSION=' + pybind_version]
         if carl_dir is not None:
             cmake_args += ['-Dcarl_DIR=' + carl_dir]
         if use_parser and carl_parser_dir:
-            cmake_args += ['-Dcarl_parser_DIR=' + carl_parser_dir]
+            cmake_args += ['-Dcarlparser_DIR=' + carl_parser_dir]
+        cmake_args += ['-DUSE_PARSER=' + ('ON' if enable_parser else 'OFF')]
+        cmake_args += ['-DUSE_CLN_NUMBERS=' + ('ON' if enable_cln else 'OFF')]
+
+        # Configure extensions
+        env = os.environ.copy()
+        env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(env.get('CXXFLAGS', ''), self.distribution.get_version())
+        setup_helper.ensure_dir_exists(self.build_temp)
+        print("Pycarl - CMake args={}".format(cmake_args))
+        # Call cmake
+        subprocess.check_call(['cmake', os.path.abspath("")] + cmake_args, cwd=self.build_temp, env=env)
+
+        # Set build args
         build_args = ['--config', build_type]
         build_args += ['--', '-j{}'.format(self.config.get_as_int("jobs"))]
-
         # Build extensions
         for ext in self.extensions:
-            setup_helper.ensure_dir_exists(os.path.join(self._extdir(ext.name), ext.subdir))
-            if "core" in ext.name:
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-                    f.write('CARL_VERSION = "{}"\n'.format(carl_version))
-                    f.write("CARL_WITH_PARSER = {}\n".format(use_parser))
-                    f.write("CARL_WITH_CLN = {}\n".format(use_cln))
-            if "cln" in ext.name:
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-                    f.write("CARL_WITH_CLN = {}\n".format(use_cln))
-                if not use_cln:
-                    print("Pycarl - CLN bindings skipped")
-                    continue
-            if "parse" in ext.name:
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-                    f.write("CARL_WITH_PARSER = {}\n".format(use_parser))
-                if not use_parser:
-                    print("Pycarl - Parser bindings skipped")
-                    continue
-            self.build_extension(ext, cmake_args, build_args)
+            if "cln" in ext.name and not use_cln:
+                print("Pycarl - Skipped CLN bindings")
+                continue
+            if "parse" in ext.name and not use_parser:
+                print("Pycarl - Skipped parser bindings")
+                continue
+            # Call make
+            subprocess.check_call(['cmake', '--build', '.', '--target', ext.name] + build_args, cwd=self.build_temp)
 
     def initialize_options(self):
         build_ext.initialize_options(self)
-        # Load setup config
-        self.config.load_from_file("build/build_config.cfg")
         # Set default values for custom cmdline flags
         self.carl_dir = None
         self.carl_parser_dir = None
         self.disable_cln = None
         self.disable_parser = None
         self.debug = None
         self.jobs = None
+        self.pybind_version = None
 
     def finalize_options(self):
         build_ext.finalize_options(self)
+        # Load setup config
+        # This can only be done after the finalization step, because otherwise build_temp is not initialized yet.
+        self.config.load_from_file(os.path.join(self.build_temp, "build_config.cfg"))
         # Update setup config
         self.config.update("carl_dir", self.carl_dir)
         self.config.update("carl_parser_dir", self.carl_parser_dir)
         self.config.update("disable_cln", self.disable_cln)
         self.config.update("disable_parser", self.disable_parser)
         self.config.update("debug", self.debug)
         self.config.update("jobs", self.jobs)
-
-    def build_extension(self, ext, general_cmake_args, general_build_args):
-        extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
-        cmake_args = ['-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + os.path.join(extdir, ext.subdir)] + general_cmake_args
-        build_args = general_build_args
-
-        env = os.environ.copy()
-        env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(env.get('CXXFLAGS', ''),
-                                                              self.distribution.get_version())
-        setup_helper.ensure_dir_exists(self.build_temp)
-        print("Pycarl - CMake args={}".format(cmake_args))
-        # Call cmake
-        subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
-        subprocess.check_call(['cmake', '--build', '.', '--target', ext.name] + build_args, cwd=self.build_temp)
+        self.config.update("pybind_version", self.pybind_version)
 
 
 setup(
     name='pycarl',
     version=setup_helper.obtain_version(),
     author="S. Junges",
     author_email="sebastian.junges@cs.rwth-aachen.de",
@@ -203,24 +197,29 @@
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     include_package_data=True,
+    package_data={'pycarl.examples': ['examples/files/*']},
     ext_package='pycarl',
-    ext_modules=[CMakeExtension('core', subdir=''),
-                 CMakeExtension('cln', subdir='cln'),
-                 CMakeExtension('gmp', subdir='gmp'),
-                 CMakeExtension('formula', subdir='formula'),
-                 CMakeExtension('formula-cln', subdir='cln/formula'),
-                 CMakeExtension('formula-gmp', subdir='gmp/formula'),
-                 CMakeExtension('parse', subdir='parse'),
-                 CMakeExtension('parse-gmp', subdir='gmp/parse'),
-                 CMakeExtension('parse-cln', subdir='cln/parse')],
-
+    ext_modules=[CMakeExtension('core'),
+                 CMakeExtension('cln'),
+                 CMakeExtension('gmp'),
+                 CMakeExtension('formula'),
+                 CMakeExtension('formula-cln'),
+                 CMakeExtension('formula-gmp'),
+                 CMakeExtension('parse'),
+                 CMakeExtension('parse-gmp'),
+                 CMakeExtension('parse-cln')
+                 ],
     cmdclass={'build_ext': CMakeBuild},
     zip_safe=False,
-    setup_requires=['pytest-runner'],
+    setup_requires=['pytest-runner',
+                    'packaging'],
     tests_require=['pytest'],
-    python_requires='>=3',
+    extras_require={
+        "doc": ["Sphinx", "sphinx-bootstrap-theme"]
+    },
+    python_requires='>=3.7',  # required by packaging
 )
```

### Comparing `pycarl-2.0.4/src/common.h` & `pycarl-2.2.0/src/common.h`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/core/monomial.cpp` & `pycarl-2.2.0/src/core/monomial.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,22 @@
         .def_property_readonly("exponents", [](const Monomial::Arg& arg) { return arg->exponents();} )
         .def("__str__", &streamToString<const Monomial::Arg&>)
 
         .def("__len__", [](const Monomial::Arg& m) { return m->nrVariables(); })
         .def("__getitem__", [](const Monomial::Arg& m, std::size_t index) { return *(m->begin()+index); })
         .def("__iter__", [](const Monomial::Arg& m) { return py::make_iterator(m->begin(), m->end()); },
                             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */)
-        .def("__getstate__", [](const Monomial& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Monomial& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Monomial& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> std::shared_ptr<Monomial> {
+                    throw NoPickling();
+                }
+            ))
         .def("__hash__", [](const Monomial& v) { std::hash<Monomial> h; return h(v);})
     ;
 
 
     m.def("create_monomial", [] (const carl::Variable& v, carl::exponent e){
         return carl::createMonomial(v, e);
     }, "Create monomial", py::arg("variable"), py::arg("exponent"));
```

### Comparing `pycarl-2.0.4/src/core/variable.cpp` & `pycarl-2.2.0/src/core/variable.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,22 @@
         .value("INT", carl::VariableType::VT_INT)
         .value("REAL", carl::VariableType::VT_REAL);
 }
 
 void define_variable(py::module& m) {
 
     py::class_<carl::Variable>(m, "Variable")
-        .def("__init__", [](carl::Variable &instance, carl::Variable const& other) {
-                new(&instance) carl::Variable(other);
-            })
-        .def("__init__", [](carl::Variable &instance, std::string name, carl::VariableType type) {
-                carl::Variable tmp = freshVariable(name, type);
-                new(&instance) carl::Variable(tmp);
-            }, py::arg("name"), py::arg("type") = carl::VariableType::VT_REAL)
-        .def("__init__", [](carl::Variable &instance, carl::VariableType type) {
-                carl::Variable tmp = freshVariable(type);
-                new (&instance) carl::Variable(tmp);
-            }, py::arg("type") = carl::VariableType::VT_REAL)
-
+        .def(py::init<carl::Variable>(), py::arg("other"))
+        .def(py::init([] (std::string name, carl::VariableType type) {
+                return freshVariable(name, type);
+            }), py::arg("name"), py::arg("type") = carl::VariableType::VT_REAL)
+        .def(py::init([] (carl::VariableType type) {
+                return freshVariable(type);
+                //return std::unique_ptr<carl::Variable>(new carl::Variable(tmp));
+            }), py::arg("type") = carl::VariableType::VT_REAL)
         .def("__mul__",  static_cast<Monomial::Arg (*)(carl::Variable, carl::Variable)>(&carl::operator*))
 
 
         .def(py::self == py::self)
         .def(py::self != py::self)
         .def(py::self < py::self)
         .def(py::self <= py::self)
@@ -60,20 +56,22 @@
         .def_property_readonly("type", &carl::Variable::type)
         .def_property_readonly("id", &carl::Variable::id)
         .def_property_readonly("rank", &carl::Variable::rank)
         .def("__repr__", [](const carl::Variable& r)  { if (r != carl::Variable::NO_VARIABLE) { return "<Variable " + r.name() + " [id = " + std::to_string(r.id()) + "]>"; } else { return std::string("<NOVARIABLE>");} })
         .def("__str__", &streamToString<carl::Variable>)
         .def_property_readonly("is_no_variable", [](const carl::Variable& v) {return v == carl::Variable::NO_VARIABLE;})
             // TODO get state has an issue if there are several variables with the same name; they cannot be distinguished afterwards
-        .def("__getstate__", [](const carl::Variable& v) { return std::make_tuple<std::string, std::string>(v.name(), carl::to_string(v.type()));})
-
-        .def("__setstate__", [](carl::Variable& v, const std::tuple<std::string, std::string>& data ) {
-                carl::Variable tmp = getOrCreateVariable(std::get<0>(data), carl::variableTypeFromString(std::get<1>(data)));
-                new(&v) carl::Variable(tmp);
-            })
+        .def(py::pickle(
+                [](const carl::Variable& v) {
+                    return std::make_tuple<std::string, std::string>(v.name(), carl::to_string(v.type()));
+                },
+                [](const std::tuple<std::string, std::string>& data ) {
+                    return getOrCreateVariable(std::get<0>(data), carl::variableTypeFromString(std::get<1>(data)));
+                }
+            ))
         .def("__hash__", [](const carl::Variable& v) { std::hash<carl::Variable> h; return h(v);})
 
     ;
 
     m.def("variable_with_name", [](std::string const& name){
             return carl::VariablePool::getInstance().findVariableWithName(name);
         }, "Get a variable from the pool with the given name.");
```

### Comparing `pycarl-2.0.4/src/formula/formula_type.cpp` & `pycarl-2.2.0/src/formula/formula_type.cpp`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/mod_cln.cpp` & `pycarl-2.2.0/src/mod_cln.cpp`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/mod_gmp.cpp` & `pycarl-2.2.0/src/mod_gmp.cpp`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/mod_parse.cpp` & `pycarl-2.2.0/src/mod_parse.cpp`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/mod_typed_parse.cpp` & `pycarl-2.2.0/src/mod_typed_parse.cpp`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/typed_core/factorization.cpp` & `pycarl-2.2.0/src/typed_core/factorization.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 #include "src/types.h"
 #include "src/helpers.h"
 
 
 void define_factorizationcache(py::module& m) {
     py::class_<carl::Cache<FactorizationPair>, std::shared_ptr<carl::Cache<FactorizationPair>>>(m, "_FactorizationCache", "Cache storing all factorized polynomials")
         .def(py::init(), "Constructor")
-        .def("__getstate__", [](const FactorizationPair& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](FactorizationPair& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const carl::Cache<FactorizationPair>& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> std::shared_ptr<carl::Cache<FactorizationPair>> {
+                    throw NoPickling();
+                }
+            ))
     ;
 }
 
 void define_factorization(py::module& m) {
     py::class_<Factorization, std::shared_ptr<Factorization>>(m, "Factorization", "Factorization")
         .def("__str__", &streamToString<Factorization>)
         .def(py::self == py::self)
@@ -20,11 +26,17 @@
         .def("__len__", [](const Factorization& f) {
                 return f.size();
             })
         .def("__iter__", [](const Factorization& f) {
                 return py::make_iterator(f.begin(), f.end());
             }, py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */)
 
-        .def("__getstate__", [](const Factorization& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Factorization& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Factorization& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> Factorization {
+                    throw NoPickling();
+                }
+            ))
     ;
-}
+}
```

### Comparing `pycarl-2.0.4/src/typed_core/factorizedpolynomial.cpp` & `pycarl-2.2.0/src/typed_core/factorizedpolynomial.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -44,12 +44,18 @@
                 return pol.pow(exp);
             }, py::arg("exponent"), "Raise polynomial to the power")
 
         .def(py::self == py::self)
         .def(py::self != py::self)
         .def(py::self == Rational())
         .def(py::self != Rational())
-        .def("__getstate__", [](const FactorizedPolynomial& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](FactorizedPolynomial& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const FactorizedPolynomial& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> FactorizedPolynomial {
+                    throw NoPickling();
+                }
+            ))
         .def("__hash__", [](const FactorizedPolynomial& v) { std::hash<FactorizedPolynomial> h; return h(v);})
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_core/factorizedrationalfunction.cpp` & `pycarl-2.2.0/src/typed_core/factorizedrationalfunction.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -33,12 +33,18 @@
         .def(py::self - py::self)
         .def(py::self + py::self)
         .def(py::self * py::self)
         .def(py::self / py::self)
         .def(py::self == py::self)
         .def(py::self != py::self)
         .def(py::self + Rational())
-        .def("__getstate__", [](const FactorizedRationalFunction& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](FactorizedRationalFunction& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const FactorizedRationalFunction& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> FactorizedRationalFunction {
+                    throw NoPickling();
+                }
+            ))
         .def("__hash__", [](const FactorizedRationalFunction& v) { std::hash<FactorizedRationalFunction> h; return h(v);})
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_core/integer.cpp` & `pycarl-2.2.0/src/typed_core/integer.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 #include "carl/numbers/numbers.h"
 #include "carl/numbers/conversion/cln_gmp.h"
 
 
 void define_cln_integer(py::module& m) {
 #ifdef PYCARL_USE_CLN
     py::class_<cln::cl_I>(m, "Integer", "Class wrapping cln-integers")
-        .def("__init__", [](cln::cl_I &instance, int val) -> void { new (&instance) cln::cl_I(val); })
-        .def("__init__", [](cln::cl_I &instance, std::string val) -> void {
-            cln::cl_I tmp;
-            bool suc = carl::try_parse<cln::cl_I>(val, tmp);
-            if(!suc) {
-                throw std::invalid_argument("Cannot translate " + val + " into an integer.");
-            }
-             new (&instance) cln::cl_I(tmp); })
-        .def("__init__", [](cln::cl_I &instance, mpz_class const& val) -> void { auto tmp = carl::convert<mpz_class, cln::cl_I>(val); new (&instance) cln::cl_I(tmp);})
+        .def(py::init<int>())
+        .def(py::init([](std::string const& val) {
+                cln::cl_I tmp;
+                bool suc = carl::try_parse<cln::cl_I>(val, tmp);
+                if(!suc) {
+                    throw std::invalid_argument("Cannot translate " + val + " into an integer.");
+                }
+                return tmp;
+            }))
+        .def(py::init(&carl::convert<mpz_class, cln::cl_I>))
 
         .def(py::self + py::self)
         .def(py::self + int())
         .def(int() + py::self)
         .def("__add__", [](const cln::cl_I& lhs, carl::Variable::Arg rhs) -> Polynomial { return cln::cl_RA(lhs) + rhs; })
         .def("__add__", [](const cln::cl_I& lhs, const Monomial::Arg& rhs) -> Polynomial { return cln::cl_RA(lhs) + rhs; })
         .def("__radd__", [](const cln::cl_I& rhs, carl::Variable::Arg lhs) -> Polynomial { return cln::cl_RA(rhs) + lhs; })
@@ -63,36 +64,41 @@
         .def(py::self >= int())
         .def(py::self <= int())
 
 
         .def("__float__", static_cast<double (*)(cln::cl_I const&)>(&carl::toDouble))
         .def("__str__", &streamToString<cln::cl_I>)
         .def("__repr__", [](const cln::cl_I& r) { return "<Integer (cln) " + streamToString<cln::cl_I>(r) + ">"; })
-        .def("__getstate__", [](const cln::cl_I& val) {
-            return std::tuple<std::string>(carl::toString(val));})
-
-        .def("__setstate__", [](cln::cl_I& val, std::tuple<std::string> data) {cln::cl_I res = carl::parse<cln::cl_I>(std::get<0>(data)); new (&val) cln::cl_I(res); })
+        .def(py::pickle(
+                [](const cln::cl_I& val) {
+                    return std::tuple<std::string>(carl::toString(val));
+                },
+                [](std::tuple<std::string> data) {
+                    return carl::parse<cln::cl_I>(std::get<0>(data));
+                }
+            ))
         .def("__hash__", [](const cln::cl_I& v) { std::hash<cln::cl_I> h; return h(v);})
     ;
 #endif
 }
 
 void define_gmp_integer(py::module& m) {
 #ifndef PYCARL_USE_CLN
     py::class_<mpz_class>(m, "Integer", "Class wrapping gmp-integers")
-        .def("__init__", [](mpz_class &instance, int val) -> void { new (&instance) mpz_class(val); })
-        .def("__init__", [](mpz_class &instance, std::string const& val)  -> void {
-            mpz_class tmp;
-            bool suc = carl::try_parse<mpz_class>(val, tmp);
-            if(!suc) {
-                throw std::invalid_argument("Cannot translate " + val + " into an integer.");
-            }
-            new (&instance) mpz_class(tmp); })
+        .def(py::init<int>())
+        .def(py::init([](std::string const& val) {
+                mpz_class tmp;
+                bool suc = carl::try_parse<mpz_class>(val, tmp);
+                if(!suc) {
+                    throw std::invalid_argument("Cannot translate " + val + " into an integer.");
+                }
+                return tmp;
+            }))
 #ifdef PYCARL_HAS_CLN
-        .def("__init__", [](mpz_class &instance, cln::cl_I const& val) -> void { auto tmp = carl::convert<cln::cl_I, mpz_class>(val); new (&instance) mpz_class(tmp);})
+        .def(py::init(&carl::convert<cln::cl_I, mpz_class>))
 #endif
 
         .def("__add__", [](const mpz_class& lhs, const mpz_class& rhs) -> mpz_class { return lhs + rhs; })
         .def("__add__", [](const mpz_class& lhs, int rhs) -> mpz_class { return lhs + rhs; })
         .def("__radd__", [](const mpz_class& lhs, int rhs) -> mpz_class { return lhs + rhs; })
         .def("__add__", [](const mpz_class& lhs, carl::Variable::Arg rhs) -> Polynomial { return mpq_class(lhs) + rhs; })
         .def("__add__", [](const mpz_class& lhs, const Monomial::Arg& rhs) -> Polynomial { return mpq_class(lhs) + rhs; })
@@ -137,17 +143,22 @@
         .def(py::self >= int())
         .def(py::self <= int())
 
 
         .def("__float__", static_cast<double (*)(mpz_class const&)>(&carl::toDouble))
         .def("__str__", &streamToString<mpz_class>)
         .def("__repr__", [](const mpz_class& r) { return "<Integer (gmp) " + streamToString<mpz_class>(r) + ">"; })
-        .def("__getstate__", [](const mpz_class& val) {
-            return std::tuple<std::string>(carl::toString(val));})
-        .def("__setstate__", [](mpz_class& val, std::tuple<std::string> data) {mpz_class res = carl::parse<mpz_class>(std::get<0>(data)); new (&val) mpz_class(res); })
+        .def(py::pickle(
+                [](const mpz_class& val) -> std::tuple<std::string> {
+                    return std::tuple<std::string>(carl::toString(val));
+                },
+                [](const std::tuple<std::string>& data) -> mpz_class {
+                    return carl::parse<mpz_class>(std::get<0>(data));
+                }
+            ))
         .def("__hash__", [](const mpz_class& v) { std::hash<mpz_class> h; return h(v);})
     ;
 #endif
 
 }
```

### Comparing `pycarl-2.0.4/src/typed_core/interval.cpp` & `pycarl-2.2.0/src/typed_core/interval.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -93,16 +93,22 @@
 		.def(Rational() < py::self)
 		.def(py::self > py::self)
 		.def(py::self > Rational())
 		.def(Rational() > py::self)
 		
 		.def("__str__", &streamToString<Interval>)
 		.def("__repr__", [](const Interval& i) { return "<Interval " + streamToString<Interval>(i) + ">"; })
-        .def("__getstate__", [](const Interval& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Interval& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Interval& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> Interval {
+                    throw NoPickling();
+                }
+            ))
 	;
 	
 	m.def("isInteger", [](const Interval& i){ return carl::isInteger(i); });
 	m.def("div", [](const Interval& l, const Interval& r){ return carl::div(l, r); });
 	m.def("quotient", [](const Interval& l, const Interval& r){ return carl::quotient(l, r); });
 	m.def("abs", [](const Interval& i){ return carl::abs(i); });
 	m.def("pow", [](const Interval& i, carl::uint exp){ return carl::pow(i, exp); });
```

### Comparing `pycarl-2.0.4/src/typed_core/polynomial.cpp` & `pycarl-2.2.0/src/typed_core/polynomial.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -87,12 +87,18 @@
         .def("__ne__", [](const Polynomial& lhs, const Integer& rhs) -> bool {return lhs != Rational(rhs);})
 
         .def("__len__", &Polynomial::size)
         .def("__getitem__", [](const Polynomial& p, std::size_t index) { return *(p.begin()+index); })
         .def("__iter__", [](const Polynomial& p) {
                 return py::make_iterator(p.begin(), p.end());
             }, py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */)
-        .def("__getstate__", [](const Polynomial& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Polynomial& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Polynomial& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> Polynomial {
+                    throw NoPickling();
+                }
+            ))
         .def("__hash__", [](const Polynomial& v) { std::hash<Polynomial> h; return h(v);})
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_core/rational.cpp` & `pycarl-2.2.0/src/typed_core/rational.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,26 @@
 
 #include "carl/numbers/numbers.h"
 #include "carl/numbers/conversion/cln_gmp.h"
 
 void define_cln_rational(py::module& m) {
 #ifdef PYCARL_USE_CLN
     py::class_<cln::cl_RA>(m, "Rational", "Class wrapping cln-rational numbers")
-        .def("__init__", [](cln::cl_RA &instance, double val) -> void { auto tmp = carl::rationalize<cln::cl_RA>(val); new (&instance) cln::cl_RA(tmp); })
-        .def("__init__", [](cln::cl_RA &instance, carl::sint val) -> void { auto tmp = carl::rationalize<cln::cl_RA>(val); new (&instance) cln::cl_RA(tmp); })
-        .def("__init__", [](cln::cl_RA &instance, const cln::cl_I& numerator, const cln::cl_I& denominator) -> void { new (&instance) cln::cl_RA(cln::cl_RA(numerator)/cln::cl_RA(denominator)); })
-        .def("__init__", [](cln::cl_RA &instance, const std::string& val) -> void {
+        .def(py::init([](double val) { return carl::rationalize<cln::cl_RA>(val); }))
+        .def(py::init([](carl::sint val) { return carl::rationalize<cln::cl_RA>(val); }))
+        .def(py::init([](const cln::cl_I& numerator, const cln::cl_I& denominator) { return cln::cl_RA(numerator)/cln::cl_RA(denominator); }))
+        .def(py::init([](const std::string& val) {
                 cln::cl_RA tmp;
                 bool suc = carl::try_parse<cln::cl_RA>(val, tmp);
                 if(!suc) {
                    throw std::invalid_argument("Cannot translate " + val + " into a rational.");
                 }
-                new (&instance) cln::cl_RA(tmp);
-            })
-        .def("__init__", [](cln::cl_RA &instance, mpq_class const& val) -> void {
-                auto tmp = carl::convert<mpq_class, cln::cl_RA>(val);
-                new (&instance) cln::cl_RA(tmp);
-            })
-
+                return tmp;
+            }))
+        .def(py::init(&carl::convert<mpq_class, cln::cl_RA>))
 
         .def("__add__", [](const cln::cl_RA& lhs, const cln::cl_RA& rhs) -> cln::cl_RA { return lhs + rhs; })
         .def("__add__", [](const cln::cl_RA& lhs, carl::sint rhs) -> cln::cl_RA { return lhs + carl::rationalize<cln::cl_RA>(rhs); })
         .def("__add__", [](const cln::cl_RA& lhs, const Polynomial& rhs) -> Polynomial { return lhs + rhs; })
         .def("__add__", [](const cln::cl_RA& lhs, const FactorizedRationalFunction& rhs) -> FactorizedRationalFunction { return rhs + lhs; })
         .def("__radd__", [](const cln::cl_RA& rhs, carl::sint lhs) -> cln::cl_RA { return carl::rationalize<cln::cl_RA>(lhs) + rhs; })
         .def("__radd__", [](const cln::cl_RA& rhs, carl::Variable::Arg lhs) -> Polynomial { return lhs + rhs; })
@@ -115,45 +111,49 @@
         .def_property_readonly("numerator", [](const cln::cl_RA& val) ->  cln::cl_I {
                 return carl::getNum(val);
             })
         .def_property_readonly("denominator", [](const cln::cl_RA& val) ->  cln::cl_I {
                 return carl::getDenom(val);
             })
 
-        .def("__getstate__", [](const cln::cl_RA& val) {
-                return std::pair<std::string, std::string>(carl::toString(carl::getNum(val)), carl::toString(carl::getDenom(val)));
-            })
-
-        .def("__setstate__", [](cln::cl_RA& val, std::pair<std::string, std::string> data) {
-                cln::cl_RA res = carl::parse<cln::cl_RA>(data.first) / carl::parse<cln::cl_RA>(data.second);
-                new (&val) cln::cl_RA(res);
-            })
+        .def(py::pickle(
+                [](const cln::cl_RA& val) {
+                    return std::pair<std::string, std::string>(carl::toString(carl::getNum(val)), carl::toString(carl::getDenom(val)));
+                },
+                [](std::pair<std::string, std::string> data) {
+                    return carl::parse<cln::cl_RA>(data.first) / carl::parse<cln::cl_RA>(data.second);
+                }
+            ))
         .def("__hash__", [](const cln::cl_RA& v) { std::hash<cln::cl_RA> h; return h(v);})
     ;
 
 	py::implicitly_convertible<carl::uint, cln::cl_RA>();
 #endif
 }
 
 
 
 void define_gmp_rational(py::module& m) {
 #ifndef PYCARL_USE_CLN
     py::class_<mpq_class>(m, "Rational", "Class wrapping gmp-rational numbers")
-        .def("__init__", [](mpq_class &instance, double val) -> void { auto tmp = carl::rationalize<mpq_class>(val); new (&instance) mpq_class(tmp); })
-        .def("__init__", [](mpq_class &instance, carl::sint val) -> void { auto tmp = carl::rationalize<mpq_class>(val); new (&instance) mpq_class(tmp); })
-        .def("__init__", [](mpq_class &instance, const mpz_class& numerator, const mpz_class& denominator) -> void { new (&instance) mpq_class(mpq_class(numerator)/mpq_class(denominator)); })
-        .def("__init__", [](mpq_class &instance, const std::string& val) -> void {
+        .def(py::init([](double val) { return carl::rationalize<mpq_class>(val); }))
+        .def(py::init([](carl::sint val) { return carl::rationalize<mpq_class>(val); }))
+        .def(py::init<const mpz_class&, const mpz_class&>())
+        .def(py::init([](const std::string& val) {
                 mpq_class tmp;
                 bool suc = carl::try_parse<mpq_class>(val, tmp);
                 if(!suc) {
                     throw std::invalid_argument("Cannot translate " + val + " into a rational.");
                 }
-                new (&instance) mpq_class(tmp);
-            })
+                return tmp;
+            }))
+#ifdef PYCARL_HAS_CLN
+        .def(py::init(&carl::convert<cln::cl_RA, mpq_class>))
+#endif
+
         .def("__add__", [](const mpq_class& lhs, const mpq_class& rhs) -> mpq_class { return lhs + rhs; })
         .def("__add__", [](const mpq_class& lhs, carl::sint rhs) -> mpq_class { return lhs + carl::rationalize<mpq_class>(rhs); })
         .def("__radd__", [](const mpq_class& rhs, carl::sint lhs) -> mpq_class { return carl::rationalize<mpq_class>(lhs) + rhs; })
         .def("__radd__", [](const mpq_class& rhs, carl::Variable::Arg lhs) -> Polynomial { return lhs + rhs; })
 
 
         .def("__sub__", [](const mpq_class& lhs, const mpq_class& rhs) -> mpq_class { return lhs - rhs; })
@@ -232,21 +232,21 @@
         .def_property_readonly("numerator", [](const mpq_class& val) -> mpz_class {
                 return carl::getNum(val);
             })
         .def_property_readonly("denominator", [](const mpq_class& val) -> mpz_class {
                 return carl::getDenom(val);
             })
 
-        .def("__getstate__", [](const mpq_class& val) {
-                return std::pair<std::string, std::string>(carl::toString(carl::getNum(val)), carl::toString(carl::getDenom(val)));
-            })
-
-        .def("__setstate__", [](mpq_class& val, std::pair<std::string, std::string> data) {
-                mpq_class res = carl::parse<mpq_class>(data.first) / carl::parse<mpq_class>(data.second);
-                new (&val) mpq_class(res);
-            })
+        .def(py::pickle(
+                [](const mpq_class& val) {
+                    return std::pair<std::string, std::string>(carl::toString(carl::getNum(val)), carl::toString(carl::getDenom(val)));
+                },
+                [](std::pair<std::string, std::string> data) {
+                    return carl::parse<mpq_class>(data.first) / carl::parse<mpq_class>(data.second);
+                }
+            ))
         .def("__hash__", [](const mpq_class& v) { std::hash<mpq_class> h; return h(v);})
     ;
 
     py::implicitly_convertible<carl::uint, mpq_class>();
 #endif
 }
```

### Comparing `pycarl-2.0.4/src/typed_core/rationalfunction.cpp` & `pycarl-2.2.0/src/typed_core/rationalfunction.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -68,12 +68,18 @@
             })
 
         .def(py::self == py::self)
         .def(py::self != py::self)
         .def("__eq__", [](const RationalFunction& lhs, const Polynomial& rhs) -> bool {return lhs == RationalFunction(rhs);})
         .def("__ne__", [](const RationalFunction& lhs, const Polynomial& rhs) -> bool {return lhs != RationalFunction(rhs);})
 
-        .def("__getstate__", [](const RationalFunction&) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](RationalFunction&, const  std::tuple<std::string>&) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const RationalFunction& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> RationalFunction {
+                    throw NoPickling();
+                }
+            ))
         .def("__hash__", [](const RationalFunction& v) { std::hash<RationalFunction> h; return h(v);})
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_core/term.cpp` & `pycarl-2.2.0/src/typed_core/term.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -47,12 +47,18 @@
         .def_property_readonly("tdeg", [](const Term& arg) { return arg.tdeg();} )
 
         .def_property_readonly("coeff", [] (const Term& arg) { return arg.coeff(); })
         .def_property_readonly("monomial", [](const Term& arg) { return arg.monomial(); })
 
         .def("__str__", &streamToString<Term>)
 
-        .def("__getstate__", [](const Term& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Term& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Term& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> Term {
+                    throw NoPickling();
+                }
+            ))
         .def("__hash__", [](const Term& v) { std::hash<Term> h; return h(v);})
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_formula/constraint.cpp` & `pycarl-2.2.0/src/typed_formula/constraint.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -43,36 +43,54 @@
                 return Formula(carl::FormulaType::XOR, {Formula(lhs), rhs});
             })
 
         //.def("satisfied_by", [](const Constraint& constraint, const carl::EvaluationMap<Rational>& evaluation) { return Formula(constraint).satisfiedBy(evaluation); })
 
         .def_property_readonly("relation", &Constraint::relation)
         .def_property_readonly("lhs", &Constraint::lhs)
-        .def("__getstate__", [](const Constraint& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Constraint& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Constraint& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> Constraint {
+                    throw NoPickling();
+                }
+            ))
     ;
 }
 //
 void define_simple_constraint(py::module& m) {
     py::class_<SimpleConstraint>(m, "SimpleConstraint")
         .def(py::init<bool>())
         .def(py::init<Polynomial, carl::Relation>())
         .def("__str__", &streamToString<SimpleConstraint>)
 
         .def("lhs", &SimpleConstraint::lhs, "Get the left hand side of the constraint")
         .def("rel", &SimpleConstraint::rel, "Get the relation of the constraint")
-        .def("__getstate__", [](const SimpleConstraint& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](SimpleConstraint& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const SimpleConstraint& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> SimpleConstraint {
+                    throw NoPickling();
+                }
+            ))
     ;
     
     py::class_<SimpleConstraintRatFunc>(m, "SimpleConstraintRatFunc")
         .def(py::init<bool>())
         .def(py::init<FactorizedRationalFunction, carl::Relation>())
         .def("__str__", &streamToString<SimpleConstraintRatFunc>)
 
         .def("lhs", &SimpleConstraintRatFunc::lhs, "Get the left hand side of the constraint")
         .def("rel", &SimpleConstraintRatFunc::rel, "Get the relation of the constraint")
 
-        .def("__getstate__", [](const SimpleConstraintRatFunc& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](SimpleConstraintRatFunc& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const SimpleConstraintRatFunc& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> SimpleConstraintRatFunc {
+                    throw NoPickling();
+                }
+            ))
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_formula/formula.cpp` & `pycarl-2.2.0/src/typed_formula/formula.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 void define_formula(py::module& m) {
     py::class_<Formula>(m, "Formula")
         .def(py::init<carl::Variable>(), "Create Formula given Boolean variable")
         .def(py::init<Constraint>())
         .def(py::init<carl::FormulaType, Formula>())
         .def(py::init<carl::FormulaType, carl::Formulas<Polynomial>>())
-        .def("__init__", [](bool b) {
+        .def(py::init([](bool b) {
                 return b ? Formula(carl::FormulaType::TRUE) : Formula(carl::FormulaType::FALSE);
-            })
+            }))
         .def("__str__", &streamToString<carl::Formula<Polynomial>>)
         .def("to_smt2", [](Formula const& f) {
                 return f.toString(false, 2);
             })
 
         .def("__invert__", [](const Formula& lhs){
                 return lhs.negated();
@@ -60,11 +60,17 @@
         .def("get_implication_conclusion", &Formula::conclusion, "Get conclusion of implication formula")
         .def("get_ite_condition", &Formula::condition, "Get condition of ITE formula")
         .def("get_ite_first_case", &Formula::firstCase, "Get then case of ITE formula")
         .def("get_ite_second_case", &Formula::secondCase, "Get else case of ITE formula")
         .def("get_subformulas", &Formula::subformulas, "Get list of subformulas for n-ary formula")
         .def("get_constraint", &Formula::constraint, "Get constraint of constraint formula")
 
-        .def("__getstate__", [](const Formula& val) -> std::tuple<std::string> { throw NoPickling(); })
-        .def("__setstate__", [](Formula& val, const std::tuple<std::string>& data) { throw NoPickling(); })
+        .def(py::pickle(
+                [](const Formula& val) -> std::tuple<std::string> {
+                    throw NoPickling();
+                },
+                [](const std::tuple<std::string>& data) -> Formula {
+                    throw NoPickling();
+                }
+            ))
     ;
 }
```

### Comparing `pycarl-2.0.4/src/typed_parse/parser.h` & `pycarl-2.2.0/src/typed_parse/parser.h`

 * *Files identical despite different names*

### Comparing `pycarl-2.0.4/src/types.h` & `pycarl-2.2.0/src/types.h`

 * *Files identical despite different names*

