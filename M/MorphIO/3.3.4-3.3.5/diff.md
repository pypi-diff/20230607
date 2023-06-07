# Comparing `tmp/MorphIO-3.3.4.tar.gz` & `tmp/MorphIO-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MorphIO-3.3.4.tar", last modified: Tue Jan 17 08:25:28 2023, max compression
+gzip compressed data, was "dist/MorphIO-3.3.5.tar", last modified: Wed Jun  7 10:42:54 2023, max compression
```

## Comparing `MorphIO-3.3.4.tar` & `MorphIO-3.3.5.tar`

### file list

```diff
@@ -1,329 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.github/workflows/check-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.github/workflows/clang_format_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.github/workflows/coverage_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.github/workflows/docstring_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.github/workflows/publish-sdist-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-01-17 08:25:07.000000 MorphIO-3.3.4/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-17 08:25:07.000000 MorphIO-3.3.4/3rdparty/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/cmake/gsl-lite-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/gsl-lite.natvis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl-lite.h
--rw-r--r--   0 runner    (1001) docker     (123)   188581 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl-lite/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-17 08:25:14.000000 MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMake/config/TestHelpers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   114690 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/DoxygenLayout.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/doxygen-awesome-css/
--rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/mainpage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example1_hdf5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example1_highfive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example6.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_boost.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_props.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/examples.js
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/godbolt.org.ico
--rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/doc/poster/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Attribute.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5DataSet.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5DataSpace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5DataType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Easy.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5File.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5FileDriver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Group.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5PropertyList.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Reference.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Selection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Utility.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Version.hpp.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5ConverterEigen_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-01-17 08:25:16.000000 MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/char_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/dot.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/enums.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30752 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/generator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/internals.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/licence_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/lookup.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/match_results.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/memory_file.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/narrow.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/observer_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    37446 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/parser.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/
--rw-r--r--   0 runner    (1001) docker     (123)    32275 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    39423 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    29156 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28271 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23049 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc
--rw-r--r--   0 runner    (1001) docker     (123)    46160 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/partition/charset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34712 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/rules.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/runtime_error.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/serialise.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/sm_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/state_machine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/string_token.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-01-17 08:25:17.000000 MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-01-17 08:25:07.000000 MorphIO-3.3.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-01-17 08:25:07.000000 MorphIO-3.3.4/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/CMake/
--rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-01-17 08:25:07.000000 MorphIO-3.3.4/CMake/CodeCoverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-01-17 08:25:07.000000 MorphIO-3.3.4/CMake/CompilerFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-17 08:25:07.000000 MorphIO-3.3.4/CMake/MorphIOConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-17 08:25:07.000000 MorphIO-3.3.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-01-17 08:25:07.000000 MorphIO-3.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-17 08:25:07.000000 MorphIO-3.3.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-17 08:25:07.000000 MorphIO-3.3.4/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-17 08:25:07.000000 MorphIO-3.3.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/MorphIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-01-17 08:25:27.000000 MorphIO-3.3.4/MorphIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-01-17 08:25:27.000000 MorphIO-3.3.4/MorphIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:25:27.000000 MorphIO-3.3.4/MorphIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:25:27.000000 MorphIO-3.3.4/MorphIO.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-17 08:25:27.000000 MorphIO-3.3.4/MorphIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-17 08:25:27.000000 MorphIO-3.3.4/MorphIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-01-17 08:25:28.000000 MorphIO-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-17 08:25:07.000000 MorphIO-3.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_enums.h
--rw-r--r--   0 runner    (1001) docker     (123)    24887 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_immutable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_immutable.h
--rw-r--r--   0 runner    (1001) docker     (123)    15991 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_misc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_misc.h
--rw-r--r--   0 runner    (1001) docker     (123)    29814 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_mutable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_mutable.h
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_vasculature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bind_vasculature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bindings_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/bindings_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/generated/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/generated/docstrings.h
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-17 08:25:07.000000 MorphIO-3.3.4/binds/python/morphio.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65705 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    49082 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31971 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79251 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126295 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    90338 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/binds/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-01-17 08:25:18.000000 MorphIO-3.3.4/binds/python/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/include/morphio/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/dendritic_spine.h
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/endoplasmic_reticulum.h
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/enums.h
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/errorMessages.h
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/glial_cell.h
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mito_section.h
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mitochondria.h
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/morphology.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/include/morphio/mut/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/dendritic_spine.h
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/endoplasmic_reticulum.h
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/glial_cell.h
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/mito_section.h
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/mitochondria.h
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/modifiers.h
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/morphology.h
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/section.h
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/soma.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/mut/writers.h
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/properties.h
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/section.h
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/section_base.h
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/section_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/soma.h
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/tools.h
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/include/morphio/vasc/
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/vasc/iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/vasc/properties.h
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/vasc/section.h
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/vasc/vasculature.h
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/vector_types.h
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-17 08:25:07.000000 MorphIO-3.3.4/include/morphio/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/morphio/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-01-17 08:25:07.000000 MorphIO-3.3.4/morphio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/morphio/mut/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-17 08:25:07.000000 MorphIO-3.3.4/morphio/mut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/morphio/vasculature/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-17 08:25:07.000000 MorphIO-3.3.4/morphio/vasculature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-17 08:25:07.000000 MorphIO-3.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 08:25:28.000000 MorphIO-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-01-17 08:25:07.000000 MorphIO-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/dendritic_spine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/endoplasmic_reticulum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/enums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/errorMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/glial_cell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mito_section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mitochondria.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/morphology.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/src/mut/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/dendritic_spine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/endoplasmic_reticulum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/glial_cell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/mito_section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/mitochondria.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/modifiers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/morphology.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/soma.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/mut/writers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/point_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/point_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/properties.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/src/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/NeurolucidaLexer.inc
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/morphologyASC.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/morphologyASC.h
--rw-r--r--   0 runner    (1001) docker     (123)    15162 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/morphologyHDF5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/morphologyHDF5.h
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/morphologySWC.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/morphologySWC.h
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/vasculatureHDF5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/readers/vasculatureHDF5.h
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/shared_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/soma.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:25:28.000000 MorphIO-3.3.4/src/vasc/
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/vasc/properties.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/vasc/section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/vasc/vasculature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-01-17 08:25:07.000000 MorphIO-3.3.4/src/version.cpp.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/check-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/clang_format_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/coverage_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/docstring_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/publish-sdist-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 10:42:35.000000 MorphIO-3.3.5/3rdparty/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/gsl-lite-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/gsl-lite.natvis
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.h
+-rw-r--r--   0 runner    (1001) docker     (123)   188581 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl-lite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/TestHelpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   114982 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/DoxygenLayout.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/
+-rw-r--r--   0 runner    (1001) docker     (123)    63015 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example1_hdf5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example1_highfive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example6.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_easy_h5py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_props.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/examples.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/godbolt.org.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Attribute.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSpace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Easy.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5File.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5FileDriver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Group.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5PropertyList.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Selection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Utility.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Version.hpp.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30878 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Friends.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/
+-rw-r--r--   0 runner    (1001) docker     (123)   192164 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/char_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/dot.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/enums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30752 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/internals.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/licence_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/lookup.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/match_results.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/memory_file.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/narrow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/observer_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    37446 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/parser.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/
+-rw-r--r--   0 runner    (1001) docker     (123)    32275 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39423 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29156 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28271 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23049 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    46160 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/charset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34712 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/rules.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/runtime_error.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/serialise.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/state_machine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/string_token.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 10:42:35.000000 MorphIO-3.3.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/CMake/
+-rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMake/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMake/CompilerFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMake/MorphIOConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 10:42:35.000000 MorphIO-3.3.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-07 10:42:35.000000 MorphIO-3.3.5/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 10:42:35.000000 MorphIO-3.3.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/MorphIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-06-07 10:42:54.000000 MorphIO-3.3.5/MorphIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-07 10:42:54.000000 MorphIO-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-07 10:42:35.000000 MorphIO-3.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_immutable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_immutable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_misc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30892 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_mutable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_mutable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_vasculature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_vasculature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bindings_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bindings_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/generated/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)    73608 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/generated/docstrings.h
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/morphio.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65705 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49082 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31971 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79251 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126295 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    90338 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/morphio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/collection.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/dendritic_spine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/endoplasmic_reticulum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/errorMessages.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/glial_cell.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mito_section.h
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mitochondria.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/morphology.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/morphio/mut/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/dendritic_spine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/endoplasmic_reticulum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/glial_cell.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/mito_section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/mitochondria.h
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/modifiers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/morphology.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/soma.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/writers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/properties.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/section_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/section_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/soma.h
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/tools.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/morphio/vasc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/properties.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/vasculature.h
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vector_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/morphio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 10:42:35.000000 MorphIO-3.3.5/morphio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/morphio/mut/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 10:42:35.000000 MorphIO-3.3.5/morphio/mut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/morphio/vasculature/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 10:42:35.000000 MorphIO-3.3.5/morphio/vasculature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 10:42:35.000000 MorphIO-3.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:42:54.000000 MorphIO-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-07 10:42:35.000000 MorphIO-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/collection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/dendritic_spine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/endoplasmic_reticulum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/errorMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/glial_cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mito_section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mitochondria.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/morphology.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/mut/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/dendritic_spine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/endoplasmic_reticulum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/glial_cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/mito_section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/mitochondria.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/modifiers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/morphology.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/soma.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/writers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/point_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/point_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/properties.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/NeurolucidaLexer.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyASC.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyASC.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyHDF5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyHDF5.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologySWC.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologySWC.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/vasculatureHDF5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/vasculatureHDF5.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/shared_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/shared_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/soma.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/vasc/
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/vasc/properties.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/vasc/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/vasc/vasculature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/version.cpp.in
```

### Comparing `MorphIO-3.3.4/.clang-format` & `MorphIO-3.3.5/.clang-format`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/.github/workflows/check-sdist.yml` & `MorphIO-3.3.5/.github/workflows/check-sdist.yml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/.github/workflows/clang_format_check.yaml` & `MorphIO-3.3.5/.github/workflows/clang_format_check.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: clang-format-check
 on: [pull_request, push]
 
 jobs:
   build:
     name: clang-format-check
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
 
     # Run on external PRs, but not internal PRs as they'll be run by the push
     if: github.event_name == 'push' || github.event.pull_request.head.repo.full_name != github.repository
 
     steps:
         - name: Fetch repository
           uses: actions/checkout@v3
```

### Comparing `MorphIO-3.3.4/.github/workflows/coverage_test.yaml` & `MorphIO-3.3.5/.github/workflows/coverage_test.yaml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/.github/workflows/publish-sdist-wheels.yml` & `MorphIO-3.3.5/.github/workflows/publish-sdist-wheels.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Publish sdist and wheels for macos, manylinux, and windows, publish to pypi if a release
 on: [pull_request, push]
 
 env:
   CIBW_BUILD_VERBOSITY: 3
   CIBW_BUILD: 'cp*'
-  CIBW_SKIP: 'cp35-* cp36-* *-manylinux_i686 *-musllinux_* *-win32 cp311-win_amd64 cp311-macosx_x86_64'
+  CIBW_SKIP: 'cp35-* cp36-* *-manylinux_i686 *-musllinux_* *-win32 cp311-macosx_x86_64'
   CIBW_BEFORE_TEST: pip install -r {project}/tests/requirement_tests.txt
   CIBW_TEST_COMMAND: pytest -s -v {project}/tests
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
```

### Comparing `MorphIO-3.3.4/.github/workflows/run-tests.yml` & `MorphIO-3.3.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/.gitmodules` & `MorphIO-3.3.5/.gitmodules`

 * *Files 27% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 	url = https://github.com/martinmoene/gsl-lite.git
 [submodule "3rdparty/lexertl14"]
 	path = 3rdparty/lexertl14
 	url = https://github.com/BenHanson/lexertl14
 [submodule "3rdparty/Catch2"]
 	path = 3rdparty/Catch2
 	url = https://github.com/catchorg/Catch2.git
+[submodule "3rdparty/ghc_filesystem"]
+	path = 3rdparty/ghc_filesystem
+	url = https://github.com/gulrak/filesystem.git
```

### Comparing `MorphIO-3.3.4/.readthedocs.yaml` & `MorphIO-3.3.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/CMakeLists.txt` & `MorphIO-3.3.5/3rdparty/CMakeLists.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,7 +10,10 @@
 endif()
 
 add_subdirectory(GSL_LITE)
 target_include_directories(gsl-lite SYSTEM INTERFACE)
 
 add_library(lexertl INTERFACE)
 target_include_directories(lexertl SYSTEM INTERFACE lexertl14/include)
+
+add_subdirectory(ghc_filesystem)
+
```

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/CMakeLists.txt` & `MorphIO-3.3.5/3rdparty/GSL_LITE/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in` & `MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/gsl-lite.natvis` & `MorphIO-3.3.5/3rdparty/GSL_LITE/gsl-lite.natvis`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl-lite.h` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl.h` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/GSL_LITE/include/gsl.hpp` & `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in` & `MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
   endforeach()
 endfunction()
 
 if(TARGET HighFive)
     return()
 endif()
 
+@PACKAGE_INIT@
+
 # Get HighFive targets
 include("${CMAKE_CURRENT_LIST_DIR}/HighFiveTargets.cmake")
 
 # Recreate combined HighFive
 add_library(HighFive INTERFACE IMPORTED)
 set_property(TARGET HighFive APPEND PROPERTY INTERFACE_COMPILE_DEFINITIONS MPI_NO_CPPBIND)  # No c++ bindings
 
@@ -51,17 +53,22 @@
   set(HIGHFIVE_USE_BOOST ${HIGHFIVE_USE_BOOST} CACHE BOOL "Enable Boost Support")
 else()
   set(HIGHFIVE_USE_BOOST @HIGHFIVE_USE_BOOST@ CACHE BOOL "Enable Boost Support")
 endif()
 set(HIGHFIVE_USE_EIGEN "${HIGHFIVE_USE_EIGEN}" CACHE BOOL "Enable Eigen testing")
 set(HIGHFIVE_USE_XTENSOR "${HIGHFIVE_USE_XTENSOR}" CACHE BOOL "Enable xtensor testing")
 set(HIGHFIVE_PARALLEL_HDF5 @HIGHFIVE_PARALLEL_HDF5@ CACHE BOOL "Enable Parallel HDF5 support")
+option(HIGHFIVE_VERBOSE "Enable verbose logging" @HIGHFIVE_VERBOSE@)
 
 if(HIGHFIVE_USE_XTENSOR AND NOT CMAKE_VERSION VERSION_LESS 3.8)
   set_property(TARGET HighFive APPEND PROPERTY INTERFACE_COMPILE_FEATURES cxx_std_14)
 endif()
 
-message(STATUS "HIGHFIVE @PROJECT_VERSION@: (Re)Detecting Highfive dependencies (HIGHFIVE_USE_INSTALL_DEPS=NO)")
+if(NOT HighFive_FIND_QUIETLY)
+  message(STATUS "HIGHFIVE @PROJECT_VERSION@: (Re)Detecting Highfive dependencies (HIGHFIVE_USE_INSTALL_DEPS=NO)")
+endif()
 include("${CMAKE_CURRENT_LIST_DIR}/HighFiveTargetDeps.cmake")
 foreach(dependency HighFive_libheaders libdeps)
     copy_interface_properties(HighFive ${dependency})
 endforeach()
+
+check_required_components(HighFive)
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake` & `MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake`

 * *Files 20% similar despite different names*

```diff
@@ -2,38 +2,72 @@
 # -------------------------------
 
 if(NOT TARGET libdeps)
 
   # Independent target to make it possible to have new dependencies each build
   add_library(libdeps INTERFACE)
 
+  if(HIGHFIVE_VERBOSE)
+    target_compile_definitions(libdeps INTERFACE -DHIGHFIVE_LOG_LEVEL=0)
+  endif()
+
+  if(HIGHFIVE_GLIBCXX_ASSERTIONS)
+    target_compile_definitions(libdeps INTERFACE -D_GLIBCXX_ASSERTIONS)
+  endif()
+
+  if(HIGHFIVE_HAS_FRIEND_DECLARATIONS)
+    target_compile_definitions(libdeps INTERFACE -DHIGHFIVE_HAS_FRIEND_DECLARATIONS=1)
+  endif()
+
+  if(HIGHFIVE_SANITIZER)
+    target_compile_options(libdeps INTERFACE -fsanitize=${HIGHFIVE_SANITIZER})
+    target_link_options(libdeps INTERFACE -fsanitize=${HIGHFIVE_SANITIZER})
+  endif()
+
   # HDF5
   if(NOT DEFINED HDF5_C_LIBRARIES)
-    set(HDF5_NO_FIND_PACKAGE_CONFIG_FILE TRUE)  # Consistency
     set(HDF5_PREFER_PARALLEL ${HIGHFIVE_PARALLEL_HDF5})
     find_package(HDF5 REQUIRED)
   endif()
 
   if(HIGHFIVE_PARALLEL_HDF5 AND NOT HDF5_IS_PARALLEL)
     message(WARNING "Parallel HDF5 requested but libhdf5 doesnt support it")
   endif()
 
   target_include_directories(libdeps SYSTEM INTERFACE ${HDF5_INCLUDE_DIRS})
   target_link_libraries(libdeps INTERFACE ${HDF5_LIBRARIES})
   target_compile_definitions(libdeps INTERFACE ${HDF5_DEFINITIONS})
 
   # Boost
   if(HIGHFIVE_USE_BOOST)
-    set(Boost_NO_BOOST_CMAKE TRUE)  # Consistency
+    if(NOT DEFINED Boost_NO_BOOST_CMAKE)
+      # HighFive deactivated finding Boost via Boost's own CMake files
+      # in Oct 2016 (commit '25627b085'). Likely to appease one cluster.
+      # Boost's CMake support has since improved and likely this setting
+      # isn't needed anymore. It is kept for backwards compatibility.
+      # However, a rework of HighFive's CMake code should consider removing
+      # this default. Hard coding this to true has been reported to cause
+      # build failures.
+      set(Boost_NO_BOOST_CMAKE TRUE)
+    endif()
     find_package(Boost REQUIRED COMPONENTS system serialization)
     # Dont use imported targets yet, not avail before cmake 3.5
     target_include_directories(libdeps SYSTEM INTERFACE ${Boost_INCLUDE_DIR})
     target_compile_definitions(libdeps INTERFACE BOOST_ALL_NO_LIB H5_USE_BOOST)
   endif()
 
+  # Half
+  if(HIGHFIVE_USE_HALF_FLOAT)
+    find_file(FOUND_HALF half.hpp)
+    if (NOT FOUND_HALF)
+      message(FATAL_ERROR "Half-precision floating-point support requested but file half.hpp not found")
+    endif()
+    target_compile_definitions(libdeps INTERFACE H5_USE_HALF_FLOAT)
+  endif()
+
   # Eigen
   if(HIGHFIVE_USE_EIGEN)
     if (NOT EIGEN3_INCLUDE_DIRS)
       find_package(Eigen3 NO_MODULE)
       if(Eigen3_FOUND)
         message(STATUS "Found Eigen ${Eigen3_VERSION}: ${EIGEN3_INCLUDE_DIRS}")
       else()
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake` & `MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 # Define the HighFive INTERFACE library
 add_library(libheaders INTERFACE)
 
 target_include_directories(libheaders INTERFACE
   "$<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/include>"
+  "$<BUILD_INTERFACE:${PROJECT_BINARY_DIR}/include>"
   "$<INSTALL_INTERFACE:include>")
 
 # Combined HighFive
 add_library(HighFive INTERFACE)
 target_compile_definitions(HighFive INTERFACE MPI_NO_CPPBIND)  # No c++ bindings
 target_link_libraries(HighFive INTERFACE libheaders libdeps)
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake` & `MorphIO-3.3.5/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,15 @@
 		set(CMAKE_${COMPILER_LANGUAGE}_WARNING_ALL "-qformat=all -qinfo=lan:trx:ret:zea:cmp:ret")
 
 	## GCC, CLANG, rest of the world
 	elseif(CMAKE_${COMPILER_LANGUAGE}_COMPILER_ID MATCHES "Clang"
         OR CMAKE_${COMPILER_LANGUAGE}_COMPILER_ID MATCHES "GNU"
         OR CMAKE_${COMPILER_LANGUAGE}_COMPILER_ID MATCHES "Intel")
 		set(CMAKE_${COMPILER_LANGUAGE}_WARNING_ALL " -Wall -Wextra")
-		string(CONCAT CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG
-			" -Werror -Wshadow -Wnon-virtual-dtor -Wunused -Woverloaded-virtual"
-			" -Wformat=2 -Wconversion -Wsign-conversion -Wno-error=deprecated-declarations"
+		string(CONCAT CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG " -Werror -Wshadow -Wnon-virtual-dtor -Wunused -Woverloaded-virtual -Wformat=2 -Wconversion -Wsign-conversion -Wno-error=deprecated-declarations"
 		)
 		if(NOT CMAKE_${COMPILER_LANGUAGE}_COMPILER_IS_ICC)
 			string(CONCAT CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG
 				${CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG}
 				" -Wpedantic -Wcast-align -Wdouble-promotion"
 			)
 		endif()
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake` & `MorphIO-3.3.5/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/CMake/config/TestHelpers.cmake` & `MorphIO-3.3.5/3rdparty/HighFive/CMake/config/TestHelpers.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/Doxyfile` & `MorphIO-3.3.5/3rdparty/HighFive/doc/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -861,15 +861,17 @@
 # The INPUT tag is used to specify the files and/or directories that contain
 # documented source files. You may enter file names like myfile.cpp or
 # directories like /usr/src/myproject. Separate the files or directories with
 # spaces. See also FILE_PATTERNS and EXTENSION_MAPPING
 # Note: If this tag is empty the current directory is searched.
 
 INPUT                  = @CMAKE_CURRENT_SOURCE_DIR@/../include \
-                         @CMAKE_CURRENT_SOURCE_DIR@/mainpage.md
+                         @CMAKE_CURRENT_SOURCE_DIR@/installation.md \
+                         @CMAKE_CURRENT_SOURCE_DIR@/../CHANGELOG.md \
+                         @CMAKE_CURRENT_SOURCE_DIR@/../README.md
 
 # This tag can be used to specify the character encoding of the source files
 # that doxygen parses. Internally doxygen uses the UTF-8 encoding. Doxygen uses
 # libiconv (or the iconv built into libc) for the transcoding. See the libiconv
 # documentation (see:
 # https://www.gnu.org/software/libiconv/) for the list of possible encodings.
 # The default value is: UTF-8.
@@ -1057,15 +1059,15 @@
 FILTER_SOURCE_PATTERNS =
 
 # If the USE_MDFILE_AS_MAINPAGE tag refers to the name of a markdown file that
 # is part of the input, its contents will be placed on the main page
 # (index.html). This can be useful if you have a project on for instance GitHub
 # and want to reuse the introduction page also for the doxygen output.
 
-USE_MDFILE_AS_MAINPAGE =
+USE_MDFILE_AS_MAINPAGE = @CMAKE_CURRENT_SOURCE_DIR@/../README.md
 
 #---------------------------------------------------------------------------
 # Configuration options related to source browsing
 #---------------------------------------------------------------------------
 
 # If the SOURCE_BROWSER tag is set to YES then a list of source files will be
 # generated. Documented entities will be cross-referenced with these sources.
@@ -2172,23 +2174,23 @@
 # If the MACRO_EXPANSION tag is set to YES, doxygen will expand all macro names
 # in the source code. If set to NO, only conditional compilation will be
 # performed. Macro expansion can be done in a controlled way by setting
 # EXPAND_ONLY_PREDEF to YES.
 # The default value is: NO.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
 
-MACRO_EXPANSION        = NO
+MACRO_EXPANSION        = YES
 
 # If the EXPAND_ONLY_PREDEF and MACRO_EXPANSION tags are both set to YES then
 # the macro expansion is limited to the macros specified with the PREDEFINED and
 # EXPAND_AS_DEFINED tags.
 # The default value is: NO.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
 
-EXPAND_ONLY_PREDEF     = NO
+EXPAND_ONLY_PREDEF     = YES
 
 # If the SEARCH_INCLUDES tag is set to YES, the include files in the
 # INCLUDE_PATH will be searched if a #include is found.
 # The default value is: YES.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
 
 SEARCH_INCLUDES        = YES
@@ -2212,15 +2214,15 @@
 # defined before the preprocessor is started (similar to the -D option of e.g.
 # gcc). The argument of the tag is a list of macros of the form: name or
 # name=definition (no spaces). If the definition and the "=" are omitted, "=1"
 # is assumed. To prevent a macro definition from being undefined via #undef or
 # recursively expanded use the := operator instead of the = operator.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
 
-PREDEFINED             =
+PREDEFINED             = H5_HAVE_PARALLEL H5_USE_EIGEN H5_USE_BOOST H5_USE_OPENCV H5_USE_XTENSOR H5_USE_HALF_FLOAT H5_DEPRECATED(x):=
 
 # If the MACRO_EXPANSION and EXPAND_ONLY_PREDEF tags are set to YES then this
 # tag can be used to specify a list of macro names that should be expanded. The
 # macro definition that is found in the sources will be used. Use the PREDEFINED
 # tag if you want to use a different macro definition that overrules the
 # definition found in the source code.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/DoxygenLayout.xml` & `MorphIO-3.3.5/3rdparty/HighFive/doc/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css` & `MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
 
 Doxygen Awesome
 https://github.com/jothepro/doxygen-awesome-css
 
 MIT License
 
-Copyright (c) 2021 - 2022 jothepro
+Copyright (c) 2021 - 2023 jothepro
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -30,53 +30,58 @@
 html {
     /* primary theme color. This will affect the entire websites color scheme: links, arrows, labels, ... */
     --primary-color: #1779c4;
     --primary-dark-color: #335c80;
     --primary-light-color: #70b1e9;
 
     /* page base colors */
-    --page-background-color: white;
+    --page-background-color: #ffffff;
     --page-foreground-color: #2f4153;
-    --page-secondary-foreground-color: #637485;
+    --page-secondary-foreground-color: #6f7e8e;
 
     /* color for all separators on the website: hr, borders, ... */
     --separator-color: #dedede;
 
     /* border radius for all rounded components. Will affect many components, like dropdowns, memitems, codeblocks, ... */
     --border-radius-large: 8px;
     --border-radius-small: 4px;
     --border-radius-medium: 6px;
 
-    /* default spacings. Most compontest reference these values for spacing, to provide uniform spacing on the page. */
+    /* default spacings. Most components reference these values for spacing, to provide uniform spacing on the page. */
     --spacing-small: 5px;
     --spacing-medium: 10px;
     --spacing-large: 16px;
 
-    /* default box shadow used for raising an element above the normal content. Used in dropdowns, Searchresult, ... */
+    /* default box shadow used for raising an element above the normal content. Used in dropdowns, search result, ... */
     --box-shadow: 0 2px 8px 0 rgba(0,0,0,.075);
 
     --odd-color: rgba(0,0,0,.028);
 
     /* font-families. will affect all text on the website
      * font-family: the normal font for text, headlines, menus
      * font-family-monospace: used for preformatted text in memtitle, code, fragments
      */
     --font-family: -apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;
     --font-family-monospace: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
 
     /* font sizes */
     --page-font-size: 15.6px;
     --navigation-font-size: 14.4px;
+    --toc-font-size: 13.4px;
     --code-font-size: 14px; /* affects code, fragment */
     --title-font-size: 22px;
 
     /* content text properties. These only affect the page content, not the navigation or any other ui elements */
     --content-line-height: 27px;
     /* The content is centered and constraint in it's width. To make the content fill the whole page, set the variable to auto.*/
-    --content-maxwidth: 1000px;
+    --content-maxwidth: 1050px;
+    --table-line-height: 24px;
+    --toc-sticky-top: var(--spacing-medium);
+    --toc-width: 200px;
+    --toc-max-height: calc(100vh - 2 * var(--spacing-medium) - 85px);
 
     /* colors for various content boxes: @warning, @note, @deprecated @bug */
     --warning-color: #f8d1cc;
     --warning-color-dark: #b61825;
     --warning-color-darker: #75070f;
     --note-color: #faf3d8;
     --note-color-dark: #f3a600;
@@ -151,29 +156,30 @@
     --side-nav-foreground: var(--page-foreground-color);
     --side-nav-arrow-opacity: 0;
     --side-nav-arrow-hover-opacity: 0.9;
 
     --toc-background: var(--side-nav-background);
     --toc-foreground: var(--side-nav-foreground);
 
-    /* height of an item in any tree / collapsable table */
+    /* height of an item in any tree / collapsible table */
     --tree-item-height: 30px;
 
     --memname-font-size: var(--code-font-size);
     --memtitle-font-size: 18px;
 
     --webkit-scrollbar-size: 7px;
     --webkit-scrollbar-padding: 4px;
     --webkit-scrollbar-color: var(--separator-color);
 }
 
 @media screen and (max-width: 767px) {
     html {
         --page-font-size: 16px;
         --navigation-font-size: 16px;
+        --toc-font-size: 15px;
         --code-font-size: 15px; /* affects code, fragment */
         --title-font-size: 22px;
     }
 }
 
 @media (prefers-color-scheme: dark) {
     html:not(.light-mode) {
@@ -298,35 +304,43 @@
 
 body {
     color: var(--page-foreground-color);
     background-color: var(--page-background-color);
     font-size: var(--page-font-size);
 }
 
-body, table, div, p, dl, #nav-tree .label, .title, .sm-dox a, .sm-dox a:hover, .sm-dox a:focus, #projectname, .SelectItem, #MSearchField, .navpath li.navelem a, .navpath li.navelem a:hover {
+body, table, div, p, dl, #nav-tree .label, .title,
+.sm-dox a, .sm-dox a:hover, .sm-dox a:focus, #projectname,
+.SelectItem, #MSearchField, .navpath li.navelem a,
+.navpath li.navelem a:hover, p.reference, p.definition {
     font-family: var(--font-family);
 }
 
 h1, h2, h3, h4, h5 {
     margin-top: .9em;
     font-weight: 600;
     line-height: initial;
 }
 
-p, div, table, dl {
+p, div, table, dl, p.reference, p.definition {
     font-size: var(--page-font-size);
 }
 
+p.reference, p.definition {
+    color: var(--page-secondary-foreground-color);
+}
+
 a:link, a:visited, a:hover, a:focus, a:active {
     color: var(--primary-color) !important;
     font-weight: 500;
 }
 
 a.anchor {
     scroll-margin-top: var(--spacing-large);
+    display: block;
 }
 
 /*
  Title and top navigation
  */
 
 #top {
@@ -396,14 +410,18 @@
 }
 
 .tabs, .tabs2, .tabs3 {
     border-bottom: 1px solid var(--separator-color);
     margin-bottom: -1px;
 }
 
+.main-menu-btn-icon, .main-menu-btn-icon:before, .main-menu-btn-icon:after {
+    background: var(--page-secondary-foreground-color);
+}
+
 @media screen and (max-width: 767px) {
     .sm-dox a span.sub-arrow {
         background: var(--code-background);
     }
 
     #main-menu a.has-submenu span.sub-arrow {
         color: var(--page-secondary-foreground-color);
@@ -530,17 +548,31 @@
     width: var(--searchbar-width);
     position: relative;
     box-shadow: none;
     display: block;
     margin-top: 0;
 }
 
-.left #MSearchSelect {
+/* until Doxygen 1.9.4 */
+.left img#MSearchSelect {
+    left: 0;
+    user-select: none;
+    padding-left: 8px;
+}
+
+/* Doxygen 1.9.5 */
+.left span#MSearchSelect {
     left: 0;
     user-select: none;
+    margin-left: 8px;
+    padding: 0;
+}
+
+.left #MSearchSelect[src$=".png"] {
+    padding-left: 0
 }
 
 .SelectionMark {
     user-select: none;
 }
 
 .tabs .left #MSearchSelect {
@@ -591,20 +623,17 @@
     color: var(--searchbar-foreground);
 }
 
 #MSearchSelect {
     top: calc(calc(var(--searchbar-height) / 2) - 11px);
 }
 
-.left #MSearchSelect {
-    padding-left: 8px;
-}
-
 #MSearchBox span.left, #MSearchBox span.right {
     background: none;
+    background-image: none;
 }
 
 #MSearchBox span.right {
     padding-top: calc(calc(var(--searchbar-height) / 2) - 12px);
     position: absolute;
     right: var(--spacing-small);
 }
@@ -650,14 +679,23 @@
     }
 }
 
 html.dark-mode iframe#MSearchResults {
     filter: invert() hue-rotate(180deg);
 }
 
+#MSearchResults .SRPage {
+    background-color: transparent;
+}
+
+#MSearchResults .SRPage .SREntry {
+    font-size: 10pt;
+    padding: var(--spacing-small) var(--spacing-medium);
+}
+
 #MSearchSelectWindow {
     border: 1px solid var(--separator-color);
     border-radius: var(--border-radius-medium);
     box-shadow: var(--box-shadow);
     background: var(--page-background-color);
     padding-top: var(--spacing-small);
     padding-bottom: var(--spacing-small);
@@ -706,14 +744,15 @@
 
     #MSearchResultsWindow {
         left: var(--spacing-medium) !important;
         right: var(--spacing-medium);
         overflow: auto;
         transform: translate(0, 20px);
         animation: ease-out 280ms slideInSearchResultsMobile;
+        width: auto !important;
     }
 
     /*
      * Overwrites for fixing the searchbox on mobile in doxygen 1.9.2
      */
     label.main-menu-btn ~ #searchBoxPos1 {
         top: 3px !important;
@@ -747,14 +786,15 @@
     #doc-content {
         margin-left: 0 !important;
     }
 }
 
 #nav-tree {
     background: transparent;
+    margin-right: 1px;
 }
 
 #nav-tree .label {
     font-size: var(--navigation-font-size);
 }
 
 #nav-tree .item {
@@ -833,14 +873,29 @@
 
 div.header {
     border-bottom: 1px solid var(--separator-color);
     background-color: var(--page-background-color);
     background-image: none;
 }
 
+@media screen and (min-width: 1000px) {
+    #doc-content > div > div.contents,
+    .PageDoc > div.contents {
+        display: flex;
+        flex-direction: row-reverse;
+        flex-wrap: nowrap;
+        align-items: flex-start;
+    }
+    
+    div.contents .textblock {
+        min-width: 200px;
+        flex-grow: 1;
+    }
+}
+
 div.contents, div.header .title, div.header .summary {
     max-width: var(--content-maxwidth);
 }
 
 div.contents, div.header .title  {
     line-height: initial;
     margin: calc(var(--spacing-medium) + .2em) auto var(--spacing-medium) auto;
@@ -852,15 +907,15 @@
 
 div.headertitle {
     padding: 0;
 }
 
 div.header .title {
     font-weight: 600;
-    font-size: 210%;
+    font-size: 225%;
     padding: var(--spacing-medium) var(--spacing-large);
     word-break: break-word;
 }
 
 div.header .summary {
     width: auto;
     display: block;
@@ -895,51 +950,58 @@
 div.contents div.dyncontent {
     margin: var(--spacing-medium) 0;
 }
 
 @media (prefers-color-scheme: dark) {
     html:not(.light-mode) div.contents div.dyncontent img,
     html:not(.light-mode) div.contents center img,
-    html:not(.light-mode) div.contents table img,
+    html:not(.light-mode) div.contents > table img,
     html:not(.light-mode) div.contents div.dyncontent iframe,
     html:not(.light-mode) div.contents center iframe,
-    html:not(.light-mode) div.contents table iframe {
-        filter: hue-rotate(180deg) invert();
+    html:not(.light-mode) div.contents table iframe,
+    html:not(.light-mode) div.contents .dotgraph iframe {
+        filter: brightness(89%) hue-rotate(180deg) invert();
     }
 }
 
 html.dark-mode div.contents div.dyncontent img,
 html.dark-mode div.contents center img,
-html.dark-mode div.contents table img,
+html.dark-mode div.contents > table img,
 html.dark-mode div.contents div.dyncontent iframe,
 html.dark-mode div.contents center iframe,
-html.dark-mode div.contents table iframe {
-    filter: hue-rotate(180deg) invert();
+html.dark-mode div.contents table iframe,
+html.dark-mode div.contents .dotgraph iframe
+ {
+    filter: brightness(89%) hue-rotate(180deg) invert();
 }
 
 h2.groupheader {
     border-bottom: 0px;
     color: var(--page-foreground-color);
     box-shadow: 
         100px 0 var(--page-background-color), 
         -100px 0 var(--page-background-color),
         100px 0.75px var(--separator-color),
         -100px 0.75px var(--separator-color),
         500px 0 var(--page-background-color), 
         -500px 0 var(--page-background-color),
         500px 0.75px var(--separator-color),
         -500px 0.75px var(--separator-color),
-        1500px 0 var(--page-background-color),
-        -1500px 0 var(--page-background-color), 
-        1500px 0.75px var(--separator-color),
-        -1500px 0.75px var(--separator-color),
-        2000px 0 var(--page-background-color),
-        -2000px 0 var(--page-background-color),
-        2000px 0.75px var(--separator-color),
-        -2000px 0.75px var(--separator-color);
+        900px 0 var(--page-background-color), 
+        -900px 0 var(--page-background-color),
+        900px 0.75px var(--separator-color),
+        -900px 0.75px var(--separator-color),
+        1400px 0 var(--page-background-color),
+        -1400px 0 var(--page-background-color), 
+        1400px 0.75px var(--separator-color),
+        -1400px 0.75px var(--separator-color),
+        1900px 0 var(--page-background-color),
+        -1900px 0 var(--page-background-color),
+        1900px 0.75px var(--separator-color),
+        -1900px 0.75px var(--separator-color);
 }
 
 blockquote {
     margin: 0 var(--spacing-medium) 0 var(--spacing-medium);
     padding: var(--spacing-small) var(--spacing-large);
     background: var(--blockquote-background);
     color: var(--blockquote-foreground);
@@ -983,74 +1045,155 @@
 }
 
 table.params .paramname {
     font-weight: 600;
     font-family: var(--font-family-monospace);
     font-size: var(--code-font-size);
     padding-right: var(--spacing-small);
+    line-height: var(--table-line-height);
 }
 
-.glow {
-    text-shadow: 0 0 15px var(--primary-light-color) !important;
+h1.glow, h2.glow, h3.glow, h4.glow, h5.glow, h6.glow {
+    text-shadow: 0 0 15px var(--primary-light-color);
 }
 
 .alphachar a {
     color: var(--page-foreground-color);
 }
 
+.dotgraph {
+    max-width: 100%;
+    overflow-x: scroll;
+}
+
+.dotgraph .caption {
+    position: sticky;
+    left: 0;
+}
+
+/* Wrap Graphviz graphs with the `interactive_dotgraph` class if `INTERACTIVE_SVG = YES` */
+.interactive_dotgraph .dotgraph iframe {
+    max-width: 100%;
+}
+
 /*
  Table of Contents
  */
 
-div.toc {
-    z-index: 10;
-    position: relative;
-    background-color: var(--toc-background);
-    border: 1px solid var(--separator-color);
-    border-radius: var(--border-radius-medium);
-    box-shadow: var(--box-shadow);
+div.contents .toc {
+    max-height: var(--toc-max-height);
+    min-width: var(--toc-width);
+    border: 0;
+    border-left: 1px solid var(--separator-color);
+    border-radius: 0;
+    background-color: transparent;
+    box-shadow: none;
+    position: sticky;
+    top: var(--toc-sticky-top);
     padding: 0 var(--spacing-large);
-    margin: 0 0 var(--spacing-medium) var(--spacing-medium);
+    margin: var(--spacing-small) 0 var(--spacing-large) var(--spacing-large);
 }
 
 div.toc h3 {
     color: var(--toc-foreground);
     font-size: var(--navigation-font-size);
-    margin: var(--spacing-large) 0;
+    margin: var(--spacing-large) 0 var(--spacing-medium) 0;
 }
 
 div.toc li {
-    font-size: var(--navigation-font-size);
     padding: 0;
     background: none;
+    line-height: var(--toc-font-size);
+    margin: var(--toc-font-size) 0 0 0;
 }
 
-div.toc li:before {
-    content: '↓';
-    font-weight: 800;
-    font-family: var(--font-family);
-    margin-right: var(--spacing-small);
-    color: var(--toc-foreground);
-    opacity: .4;
+div.toc li::before {
+    display: none;
 }
 
-div.toc ul li.level1 {
-    margin: 0;
+div.toc ul {
+    margin-top: 0
 }
 
-div.toc ul li.level2, div.toc ul li.level3 {
-    margin-top: 0;
+div.toc li a {
+    font-size: var(--toc-font-size);
+    color: var(--page-foreground-color) !important;
+    text-decoration: none;
+}
+
+div.toc li a:hover, div.toc li a.active {
+    color: var(--primary-color) !important;
 }
 
+div.toc li a.aboveActive {
+    color: var(--page-secondary-foreground-color) !important;
+}
 
-@media screen and (max-width: 767px) {
-    div.toc {
+
+@media screen and (max-width: 999px) {
+    div.contents .toc {
+        max-height: 45vh;
         float: none;
         width: auto;
         margin: 0 0 var(--spacing-medium) 0;
+        position: relative;
+        top: 0;
+        position: relative;
+        border: 1px solid var(--separator-color);
+        border-radius: var(--border-radius-medium);
+        background-color: var(--toc-background);
+        box-shadow: var(--box-shadow);
+    }
+
+    div.contents .toc.interactive {
+        max-height: calc(var(--navigation-font-size) + 2 * var(--spacing-large));
+        overflow: hidden;
+    }
+
+    div.contents .toc > h3 {
+        -webkit-tap-highlight-color: transparent;
+        cursor: pointer;
+        position: sticky;
+        top: 0;
+        background-color: var(--toc-background);
+        margin: 0;
+        padding: var(--spacing-large) 0;
+        display: block;
+    }
+
+    div.contents .toc.interactive > h3::before {
+        content: "";
+        width: 0; 
+        height: 0; 
+        border-left: 4px solid transparent;
+        border-right: 4px solid transparent;
+        border-top: 5px solid var(--primary-color);
+        display: inline-block;
+        margin-right: var(--spacing-small);
+        margin-bottom: calc(var(--navigation-font-size) / 4);
+        transform: rotate(-90deg);
+        transition: transform 0.25s ease-out;
+    }
+
+    div.contents .toc.interactive.open > h3::before {
+        transform: rotate(0deg);
+    }
+
+    div.contents .toc.interactive.open {
+        max-height: 45vh;
+        overflow: auto;
+        transition: max-height 0.2s ease-in-out;
+    }
+
+    div.contents .toc a, div.contents .toc a.active {
+        color: var(--primary-color) !important;
+    }
+
+    div.contents .toc a:hover {
+        text-decoration: underline;
     }
 }
 
 /*
  Code & Fragments
  */
 
@@ -1061,15 +1204,14 @@
 }
 
 code {
     display: inline;
     background: var(--code-background);
     color: var(--code-foreground);
     padding: 2px 6px;
-    word-break: break-word;
 }
 
 div.fragment, pre.fragment {
     margin: var(--spacing-medium) 0;
     padding: calc(var(--spacing-large) - (var(--spacing-large) / 6)) var(--spacing-large);
     background: var(--fragment-background);
     color: var(--fragment-foreground);
@@ -1178,23 +1320,32 @@
     color: var(--fragment-link) !important;
 }
 
 div.fragment .line:first-child .lineno {
     box-shadow: -999999px 0px 0 999999px var(--fragment-linenumber-background), -999998px 0px 0 999999px var(--fragment-linenumber-border);
 }
 
+div.line {
+    border-radius: var(--border-radius-small);
+}
+
+div.line.glow {
+    background-color: var(--primary-light-color);
+    box-shadow: none;
+}
+
 /*
  dl warning, attention, note, deprecated, bug, ...
  */
 
 dl.bug dt a, dl.deprecated dt a, dl.todo dt a {
     font-weight: bold !important;
 }
 
-dl.warning, dl.attention, dl.note, dl.deprecated, dl.bug, dl.invariant, dl.pre, dl.todo, dl.remark {
+dl.warning, dl.attention, dl.note, dl.deprecated, dl.bug, dl.invariant, dl.pre, dl.post, dl.todo, dl.remark {
     padding: var(--spacing-medium);
     margin: var(--spacing-medium) 0;
     color: var(--page-background-color);
     overflow: hidden;
     margin-left: 0;
     border-radius: var(--border-radius-small);
 }
@@ -1257,21 +1408,21 @@
     color: var(--deprecated-color-dark) !important;
 }
 
 dl.section dd, dl.bug dd, dl.deprecated dd, dl.todo dd {
     margin-inline-start: 0px;
 }
 
-dl.invariant, dl.pre {
+dl.invariant, dl.pre, dl.post {
     background: var(--invariant-color);
     border-left: 8px solid var(--invariant-color-dark);
     color: var(--invariant-color-darker);
 }
 
-dl.invariant dt, dl.pre dt {
+dl.invariant dt, dl.pre dt, dl.post dt {
     color: var(--invariant-color-dark);
 }
 
 /*
  memitem
  */
 
@@ -1297,15 +1448,14 @@
 
 div.memitem {
     transition: none;
 }
 
 div.memproto, h2.memtitle {
     background: var(--fragment-background);
-    text-shadow: none;
 }
 
 h2.memtitle {
     font-weight: 500;
     font-size: var(--memtitle-font-size);
     font-family: var(--font-family-monospace);
     border-bottom: none;
@@ -1373,21 +1523,23 @@
     border-top-left-radius: var(--border-radius-medium);
 }
 
 div.memproto table.memname {
     font-family: var(--font-family-monospace);
     color: var(--page-foreground-color);
     font-size: var(--memname-font-size);
+    text-shadow: none;
 }
 
 div.memproto div.memtemplate {
     font-family: var(--font-family-monospace);
     color: var(--primary-dark-color);
     font-size: var(--memname-font-size);
     margin-left: 2px;
+    text-shadow: none;
 }
 
 table.mlabels, table.mlabels > tbody {
     display: block;
 }
 
 td.mlabels-left {
@@ -1445,105 +1597,179 @@
     background: none;
 }
 
 /*
  Table
  */
 
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) {
-     display: inline-block;
-     max-width: 100%;
- }
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname),
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody {
+    display: inline-block;
+    max-width: 100%;
+}
 
 .contents > table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname):not(.classindex) {
     margin-left: calc(0px - var(--spacing-large));
     margin-right: calc(0px - var(--spacing-large));
     max-width: calc(100% + 2 * var(--spacing-large));
 }
 
-table.markdownTable, table.fieldtable {
+table.fieldtable,
+table.markdownTable tbody,
+table.doxtable tbody {
     border: none;
     margin: var(--spacing-medium) 0;
     box-shadow: 0 0 0 1px var(--separator-color);
     border-radius: var(--border-radius-small);
 }
 
+table.markdownTable, table.doxtable, table.fieldtable {
+    padding: 1px;
+}
+
+table.doxtable caption {
+    display: block;
+}
+
 table.fieldtable {
+    border-collapse: collapse;
     width: 100%;
 }
 
-th.markdownTableHeadLeft, th.markdownTableHeadRight, th.markdownTableHeadCenter, th.markdownTableHeadNone {
+th.markdownTableHeadLeft,
+th.markdownTableHeadRight,
+th.markdownTableHeadCenter,
+th.markdownTableHeadNone,
+table.doxtable th {
     background: var(--tablehead-background);
     color: var(--tablehead-foreground);
     font-weight: 600;
     font-size: var(--page-font-size);
 }
 
-th.markdownTableHeadLeft:first-child, th.markdownTableHeadRight:first-child, th.markdownTableHeadCenter:first-child, th.markdownTableHeadNone:first-child {
+th.markdownTableHeadLeft:first-child,
+th.markdownTableHeadRight:first-child,
+th.markdownTableHeadCenter:first-child,
+th.markdownTableHeadNone:first-child,
+table.doxtable tr th:first-child {
     border-top-left-radius: var(--border-radius-small);
 }
 
-th.markdownTableHeadLeft:last-child, th.markdownTableHeadRight:last-child, th.markdownTableHeadCenter:last-child, th.markdownTableHeadNone:last-child {
+th.markdownTableHeadLeft:last-child,
+th.markdownTableHeadRight:last-child,
+th.markdownTableHeadCenter:last-child,
+th.markdownTableHeadNone:last-child,
+table.doxtable tr th:last-child {
     border-top-right-radius: var(--border-radius-small);
 }
 
-table.markdownTable td, table.markdownTable th, table.fieldtable dt {
-    border: none;
-    border-right: 1px solid var(--separator-color);
+table.markdownTable td,
+table.markdownTable th,
+table.fieldtable td,
+table.fieldtable th,
+table.doxtable td,
+table.doxtable th {
+    border: 1px solid var(--separator-color);
     padding: var(--spacing-small) var(--spacing-medium);
 }
 
-table.markdownTable td:last-child, table.markdownTable th:last-child, table.fieldtable dt:last-child {
-    border: none;
+table.markdownTable td:last-child,
+table.markdownTable th:last-child,
+table.fieldtable td:last-child,
+table.fieldtable th:last-child,
+table.doxtable td:last-child,
+table.doxtable th:last-child {
+    border-right: none;
 }
 
-table.markdownTable tr, table.markdownTable tr {
+table.markdownTable td:first-child,
+table.markdownTable th:first-child,
+table.fieldtable td:first-child,
+table.fieldtable th:first-child,
+table.doxtable td:first-child,
+table.doxtable th:first-child {
+    border-left: none;
+}
+
+table.markdownTable tr:first-child td,
+table.markdownTable tr:first-child th,
+table.fieldtable tr:first-child td,
+table.fieldtable tr:first-child th,
+table.doxtable tr:first-child td,
+table.doxtable tr:first-child th {
+    border-top: none;
+}
+
+table.markdownTable tr:last-child td,
+table.markdownTable tr:last-child th,
+table.fieldtable tr:last-child td,
+table.fieldtable tr:last-child th,
+table.doxtable tr:last-child td,
+table.doxtable tr:last-child th {
+    border-bottom: none;
+}
+
+table.markdownTable tr, table.doxtable tr {
     border-bottom: 1px solid var(--separator-color);
 }
 
-table.markdownTable tr:last-child, table.markdownTable tr:last-child {
+table.markdownTable tr:last-child, table.doxtable tr:last-child {
     border-bottom: none;
 }
 
+.full_width_table table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) {
+    display: block;
+}
+
+.full_width_table table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody {
+    display: table;
+    width: 100%;
+}
+
 table.fieldtable th {
     font-size: var(--page-font-size);
     font-weight: 600;
     background-image: none;
     background-color: var(--tablehead-background);
     color: var(--tablehead-foreground);
-    border-bottom: 1px solid var(--separator-color);
 }
 
-.fieldtable td.fieldtype, .fieldtable td.fieldname {
+table.fieldtable td.fieldtype, .fieldtable td.fieldname, .fieldtable td.fielddoc, .fieldtable th {
     border-bottom: 1px solid var(--separator-color);
     border-right: 1px solid var(--separator-color);
 }
 
-.fieldtable td.fielddoc {
-    border-bottom: 1px solid var(--separator-color);
+table.fieldtable tr:last-child td:first-child {
+    border-bottom-left-radius: var(--border-radius-small);
+}
+
+table.fieldtable tr:last-child td:last-child {
+    border-bottom-right-radius: var(--border-radius-small);
 }
 
 .memberdecls td.glow, .fieldtable tr.glow {
     background-color: var(--primary-light-color);
-    box-shadow: 0 0 15px var(--primary-light-color);
+    box-shadow: none;
 }
 
 table.memberdecls {
     display: block;
+    -webkit-tap-highlight-color: transparent;
 }
 
 table.memberdecls tr[class^='memitem'] {
     font-family: var(--font-family-monospace);
     font-size: var(--code-font-size);
 }
 
 table.memberdecls tr[class^='memitem'] .memTemplParams {
     font-family: var(--font-family-monospace);
     font-size: var(--code-font-size);
     color: var(--primary-dark-color);
+    white-space: normal;
 }
 
 table.memberdecls .memItemLeft,
 table.memberdecls .memItemRight,
 table.memberdecls .memTemplItemLeft,
 table.memberdecls .memTemplItemRight,
 table.memberdecls .memTemplParams {
@@ -1561,26 +1787,27 @@
 }
 
 table.memberdecls .memTemplParams {
     border-bottom: 0;
     border-left: 1px solid var(--separator-color);
     border-right: 1px solid var(--separator-color);
     border-radius: var(--border-radius-small) var(--border-radius-small) 0 0;
-    padding-bottom: 0;
+    padding-bottom: var(--spacing-small);
 }
 
 table.memberdecls .memTemplItemLeft {
     border-radius: 0 0 0 var(--border-radius-small);
     border-left: 1px solid var(--separator-color);
     border-top: 0;
 }
 
 table.memberdecls .memTemplItemRight {
     border-radius: 0 0 var(--border-radius-small) 0;
     border-right: 1px solid var(--separator-color);
+    padding-left: 0;
     border-top: 0;
 }
 
 table.memberdecls .memItemLeft {
     border-radius: var(--border-radius-small) 0 0 var(--border-radius-small);
     border-left: 1px solid var(--separator-color);
     padding-left: var(--spacing-medium);
@@ -1597,32 +1824,68 @@
 
 table.memberdecls .mdescLeft, table.memberdecls .mdescRight {
     background: none;
     color: var(--page-foreground-color);
     padding: var(--spacing-small) 0;
 }
 
+table.memberdecls .memItemLeft,
+table.memberdecls .memTemplItemLeft {
+    padding-right: var(--spacing-medium);
+}
+
 table.memberdecls .memSeparator {
     background: var(--page-background-color);
     height: var(--spacing-large);
     border: 0;
     transition: none;
 }
 
 table.memberdecls .groupheader {
     margin-bottom: var(--spacing-large);
 }
 
 table.memberdecls .inherit_header td {
     padding: 0 0 var(--spacing-medium) 0;
     text-indent: -12px;
-    line-height: 1.5em;
     color: var(--page-secondary-foreground-color);
 }
 
+table.memberdecls img[src="closed.png"],
+table.memberdecls img[src="open.png"],
+div.dynheader img[src="open.png"],
+div.dynheader img[src="closed.png"] {
+    width: 0; 
+    height: 0; 
+    border-left: 4px solid transparent;
+    border-right: 4px solid transparent;
+    border-top: 5px solid var(--primary-color);
+    margin-top: 8px;
+    display: block;
+    float: left;
+    margin-left: -10px;
+    transition: transform 0.25s ease-out;
+}
+
+table.memberdecls img {
+    margin-right: 10px;
+}
+
+table.memberdecls img[src="closed.png"],
+div.dynheader img[src="closed.png"] {
+    transform: rotate(-90deg);
+    
+}
+
+.compoundTemplParams {
+    font-family: var(--font-family-monospace);
+    color: var(--primary-dark-color);
+    font-size: var(--code-font-size);
+}
+
 @media screen and (max-width: 767px) {
 
     table.memberdecls .memItemLeft,
     table.memberdecls .memItemRight,
     table.memberdecls .mdescLeft,
     table.memberdecls .mdescRight,
     table.memberdecls .memTemplItemLeft,
@@ -1631,29 +1894,30 @@
         display: block;
         text-align: left;
         padding-left: var(--spacing-large);
         margin: 0 calc(0px - var(--spacing-large)) 0 calc(0px - var(--spacing-large));
         border-right: none;
         border-left: none;
         border-radius: 0;
+        white-space: normal;
     }
 
     table.memberdecls .memItemLeft,
     table.memberdecls .mdescLeft,
     table.memberdecls .memTemplItemLeft {
         border-bottom: 0;
         padding-bottom: 0;
     }
 
     table.memberdecls .memTemplItemLeft {
         padding-top: 0;
     }
 
     table.memberdecls .mdescLeft {
-        margin-top: calc(0px - var(--page-font-size));
+        margin-bottom: calc(0px - var(--page-font-size));
     }
 
     table.memberdecls .memItemRight, 
     table.memberdecls .mdescRight,
     table.memberdecls .memTemplItemRight {
         border-top: 0;
         padding-top: 0;
@@ -1743,42 +2007,69 @@
 table.directory {
     font-family: var(--font-family);
     font-size: var(--page-font-size);
     font-weight: normal;
     width: 100%;
 }
 
-table.directory td.entry {
-    padding: var(--spacing-small);
+table.directory td.entry, table.directory td.desc {
+    padding: calc(var(--spacing-small) / 2) var(--spacing-small);
+    line-height: var(--table-line-height);
+}
+
+table.directory tr.even td:last-child {
+    border-radius: 0 var(--border-radius-small) var(--border-radius-small) 0;
+}
+
+table.directory tr.even td:first-child {
+    border-radius: var(--border-radius-small) 0 0 var(--border-radius-small);
+}
+
+table.directory tr.even:last-child td:last-child {
+    border-radius: 0 var(--border-radius-small) 0 0;
+}
+
+table.directory tr.even:last-child td:first-child {
+    border-radius: var(--border-radius-small) 0 0 0;
 }
 
 table.directory td.desc {
     min-width: 250px;
 }
 
 table.directory tr.even {
     background-color: var(--odd-color);
 }
 
+table.directory tr.odd {
+    background-color: transparent;
+}
+
 .icona {
     width: auto;
     height: auto;
     margin: 0 var(--spacing-small);
 }
 
 .icon {
     background: var(--primary-color);
-    width: 18px;
-    height: 18px;
-    line-height: 18px;
+    border-radius: var(--border-radius-small);
+    font-size: var(--page-font-size);
+    padding: calc(var(--page-font-size) / 5);
+    line-height: var(--page-font-size);
+    transform: scale(0.8);
+    height: auto;
+    width: var(--page-font-size);
+    user-select: none;
 }
 
 .iconfopen, .icondoc, .iconfclosed {
     background-position: center;
     margin-bottom: 0;
+    height: var(--table-line-height);
 }
 
 .icondoc {
     filter: saturate(0.2);
 }
 
 @media screen and (max-width: 767px) {
@@ -1803,14 +2094,18 @@
  */
 
 .classindex dl.odd {
     background: var(--odd-color);
     border-radius: var(--border-radius-small);
 }
 
+.classindex dl.even {
+    background-color: transparent;
+}
+
 /* 
  Class Index Doxygen 1.8 
 */
 
 table.classindex {
     margin-left: 0;
     margin-right: 0;
@@ -1927,63 +2222,77 @@
 
 #nav-tree::-webkit-scrollbar,
 div.fragment::-webkit-scrollbar,
 pre.fragment::-webkit-scrollbar,
 div.memproto::-webkit-scrollbar,
 .contents center::-webkit-scrollbar,
 .contents .center::-webkit-scrollbar,
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname)::-webkit-scrollbar {
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody::-webkit-scrollbar,
+div.contents .toc::-webkit-scrollbar,
+.contents .dotgraph::-webkit-scrollbar,
+.contents .tabs-overview-container::-webkit-scrollbar {
+    background: transparent;
     width: calc(var(--webkit-scrollbar-size) + var(--webkit-scrollbar-padding) + var(--webkit-scrollbar-padding));
     height: calc(var(--webkit-scrollbar-size) + var(--webkit-scrollbar-padding) + var(--webkit-scrollbar-padding));
 }
 
 #nav-tree::-webkit-scrollbar-thumb,
 div.fragment::-webkit-scrollbar-thumb,
 pre.fragment::-webkit-scrollbar-thumb,
 div.memproto::-webkit-scrollbar-thumb,
 .contents center::-webkit-scrollbar-thumb,
 .contents .center::-webkit-scrollbar-thumb,
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname)::-webkit-scrollbar-thumb {
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody::-webkit-scrollbar-thumb,
+div.contents .toc::-webkit-scrollbar-thumb,
+.contents .dotgraph::-webkit-scrollbar-thumb,
+.contents .tabs-overview-container::-webkit-scrollbar-thumb {
     background-color: transparent;
     border: var(--webkit-scrollbar-padding) solid transparent;
     border-radius: calc(var(--webkit-scrollbar-padding) + var(--webkit-scrollbar-padding));
     background-clip: padding-box;  
 }
 
 #nav-tree:hover::-webkit-scrollbar-thumb,
 div.fragment:hover::-webkit-scrollbar-thumb,
 pre.fragment:hover::-webkit-scrollbar-thumb,
 div.memproto:hover::-webkit-scrollbar-thumb,
 .contents center:hover::-webkit-scrollbar-thumb,
 .contents .center:hover::-webkit-scrollbar-thumb,
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname):hover::-webkit-scrollbar-thumb {
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody:hover::-webkit-scrollbar-thumb,
+div.contents .toc:hover::-webkit-scrollbar-thumb,
+.contents .dotgraph:hover::-webkit-scrollbar-thumb,
+.contents .tabs-overview-container:hover::-webkit-scrollbar-thumb {
     background-color: var(--webkit-scrollbar-color);
 }
 
 #nav-tree::-webkit-scrollbar-track,
 div.fragment::-webkit-scrollbar-track,
 pre.fragment::-webkit-scrollbar-track,
 div.memproto::-webkit-scrollbar-track,
 .contents center::-webkit-scrollbar-track,
 .contents .center::-webkit-scrollbar-track,
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname)::-webkit-scrollbar-track {
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody::-webkit-scrollbar-track,
+div.contents .toc::-webkit-scrollbar-track,
+.contents .dotgraph::-webkit-scrollbar-track,
+.contents .tabs-overview-container::-webkit-scrollbar-track {
     background: transparent;
 }
 
 #nav-tree::-webkit-scrollbar-corner {
     background-color: var(--side-nav-background);
 }
 
 #nav-tree,
 div.fragment,
 pre.fragment,
 div.memproto,
 .contents center,
 .contents .center,
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) {
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody,
+div.contents .toc {
     overflow-x: auto;
     overflow-x: overlay;
 }
 
 #nav-tree {
     overflow-x: auto;
     overflow-y: auto;
@@ -1996,15 +2305,18 @@
 
 #nav-tree,
 div.fragment,
 pre.fragment,
 div.memproto,
 .contents center,
 .contents .center,
-.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) {
+.contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody,
+div.contents .toc,
+.contents .dotgraph,
+.contents .tabs-overview-container {
     scrollbar-width: thin;
 }
 
 /*
   Optional Dark mode toggle button
 */
 
@@ -2129,7 +2441,82 @@
 a.anchorlink:hover {
     opacity: .45;
 }
 
 h2:hover a.anchorlink, h1:hover a.anchorlink, h3:hover a.anchorlink, h4:hover a.anchorlink  {
     display: inline-block;
 }
+
+/*
+ Optional tab feature
+*/
+
+.tabbed ul {
+    padding-inline-start: 0px;
+    margin: 0;
+    padding: var(--spacing-small) 0;
+    border-bottom: 1px solid var(--separator-color);
+}
+
+.tabbed li {
+    display: none;
+}
+
+.tabbed li.selected {
+    display: block;
+}
+
+.tabs-overview-container {
+    overflow-x: auto;
+    display: block;
+    overflow-y: visible;
+}
+
+.tabs-overview {
+    border-bottom: 1px solid var(--separator-color);
+    display: flex;
+    flex-direction: row;
+}
+
+.tabs-overview button.tab-button {
+    color: var(--page-foreground-color);
+    margin: 0;
+    border: none;
+    background: transparent;
+    padding: var(--spacing-small) 0;
+    display: inline-block;
+    font-size: var(--page-font-size);
+    cursor: pointer;
+    box-shadow: 0 1px 0 0 var(--separator-color);
+}
+
+.tabs-overview button.tab-button .tab-title {
+    float: left;
+    white-space: nowrap;
+    padding: var(--spacing-small) var(--spacing-large);
+    border-radius: var(--border-radius-medium);
+}
+
+.tabs-overview button.tab-button:not(:last-child) .tab-title {
+    box-shadow: 8px 0 0 -7px var(--separator-color);
+}
+
+.tabs-overview button.tab-button:hover .tab-title {
+    background: var(--primary-color);
+    color: var(--page-background-color);
+    box-shadow: none;
+}
+
+.tabs-overview button.tab-button.active {
+    color: var(--primary-color);
+    box-shadow: 0 1px 0 0 var(--primary-color), inset 0 -1px 0 0 var(--primary-color);
+}
+
+@media (prefers-color-scheme: dark) {
+    html:not(.light-mode) .tabs-overview button.tab-button:hover .tab-title {
+        color: var(--page-foreground-color);
+    }
+}
+
+html.dark-mode .tabs-overview button.tab-button:hover .tab-title {
+    color: var(--page-foreground-color);
+}
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh` & `MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example1_hdf5.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example1_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example3.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example3.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example6.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example6.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_boost.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_eigen.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_eigen.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/example_props.cpp` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_props.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/examples.js` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/examples.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -6,21 +6,21 @@
     window.open(url);
 
 }
 
 function setup_examples() {
     $(".example").each(function() {
         let cblock = this;
-        let file = this.id + ".cpp";
+        let file = this.id + '.' + this.dataset.lang;
         $.ajax({
             url: file,
             dataType: 'text',
             success: function(code) {
                 res = hljs.highlight(code, {
-                    language: "cpp",
+                    language: cblock.dataset.lang,
                     ignoreIllegals: true
                 });
                 cblock.innerHTML += res.value;
                 let encoded = encodeURIComponent(code);
                 cblock.setAttribute("rawsrc", encoded);
             }
         });
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/godbolt.org.ico` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/godbolt.org.ico`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/doc/poster/index.html` & `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -89,22 +89,22 @@
             </tr>
           </thead>
           <tbody>
             <tr>
               <td>
                 <div class="card w-100">
                   <div class="code card-body"><img src="godbolt.org.ico" id="gb_example1_highfive" width=32 height=32  class="godbolt float-end img-thumbnail">
-                    <pre class="font-monospace"><div class="example" id="example1_highfive"></div></pre>
+                    <pre class="font-monospace"><div class="example" data-lang="cpp" id="example1_highfive"></div></pre>
                   </div>
                 </div>
               </td>
               <td>
                 <div class="card w-100">
                   <div class="code card-body"><img src="godbolt.org.ico" id="gb_example1_hdf5" width=32 height=32  class="godbolt float-end img-thumbnail">
-                    <pre class="font-monospace"><div class="example" id="example1_hdf5"></div></pre>
+                    <pre class="font-monospace"><div class="example" data-lang="cpp" id="example1_hdf5"></div></pre>
                   </div>
                 </div>
               </td>
             </tr>
           </tbody>
         </table>
       </div>
@@ -114,15 +114,15 @@
         <p>Its simplified data-management does not come at a loss of HDF5's flexibility and
         advanced features and tunable parameters are exposed through a simple interface. File
         version bounds can be read and written to define object compatibility, the metadata
         block size can be set. Group properties for compression, chunking and link info
         estimates can be set and read:</p>
         <div class="card w-75">
           <div class="code card-body"><img src="godbolt.org.ico" id="gb_example_props" width=32 height=32  class="godbolt float-end img-thumbnail">
-              <pre class="font-monospace"><div class="example" id="example_props"></div></pre>
+              <pre class="font-monospace"><div class="example" data-lang="cpp" id="example_props"></div></pre>
           </div>
         </div>
       </div>
       <div class="container mb-5">
         <h2>Complex data types</h2>
         <p>HighFive is built with scientific applications in mind. Besides scalar and simple STL
         vectors it is possible to map C++ structs to HDF5 compound types and to read and write
@@ -156,46 +156,80 @@
                                                                              type="button" role="tab" aria-controls="eigen" aria-selected="false">Eigen</button>
               </li>
             </ul>
           </div>
           <div class="tab-content code card-body" id="highfive-type-support-content">
             <div class="tab-pane fade show active" id="compound" role="tabpanel" aria-labelledby="compound-tab">
               <img src="godbolt.org.ico" id="gb_example3" width=32 height=32  class="godbolt float-end img-thumbnail">
-              <pre class="font-monospace"><div class="example" id="example3"></div></pre>
+              <pre class="font-monospace"><div class="example" data-lang="cpp" id="example3"></div></pre>
             </div>
             <div class="tab-pane fade" id="boost" role="tabpanel" aria-labelledby="boost-tab">
               <img src="godbolt.org.ico" id="gb_example_boost" width=32 height=32  class="godbolt float-end img-thumbnail">
-              <pre class="font-monospace"><div class="example" id="example_boost"></div></pre>
+              <pre class="font-monospace"><div class="example" data-lang="cpp" id="example_boost"></div></pre>
             </div>
             <div class="tab-pane fade" id="boost-ublas" role="tabpanel" aria-labelledby="boost-ublas-tab">
               <img src="godbolt.org.ico" id="gb_example_boost_ublas" width=32 height=32  class="godbolt float-end img-thumbnail">
-              <pre class="font-monospace"><div class="example" id="example_boost_ublas"></div></pre>
+              <pre class="font-monospace"><div class="example" data-lang="cpp" id="example_boost_ublas"></div></pre>
             </div>
             <div class="tab-pane fade" id="eigen" role="tabpanel" aria-labelledby="eigen-tab">
               <img src="godbolt.org.ico" id="gb_example_eigen" width=32 height=32  class="godbolt float-end img-thumbnail">
-              <pre class="font-monospace"><div class="example" id="example_eigen"></div></pre>
+              <pre class="font-monospace"><div class="example" data-lang="cpp" id="example_eigen"></div></pre>
             </div>
           </div>
         </div>
       </div>
       <div class="container mb-5">
         <h2>HighFive for parallel applications</h2>
         <p>With the aim to support large-scale scientific application, we have made an effort to
         also natively support the HDF5 MPI backend in HighFive. A special
         <code>MPIOFileDriver</code> is used in the application code to ensure that HDF5 is correctly
         initialized. No other special API calls are required since all necessary provisions are
         handled transparently.</p>
         <div class="card w-75">
           <div class="code card-body"><img src="godbolt.org.ico" id="gb_example6" width=32 height=32  class="godbolt float-end img-thumbnail">
-            <pre class="font-monospace"><div class="example" id="example6"></div></pre>
+            <pre class="font-monospace"><div class="example" data-lang="cpp" data-lang="cpp" id="example6"></div></pre>
           </div>
         </div>
       </div>
 
       <div class="container mb-5">
+        <h2>H5Easy: one-liners</h2>
+        <p>HighFive also offers the H5Easy API (on its own namespace).
+        This has an API in which things can be done in one-liners, with a syntax comparable
+        to for example h5py for Python.
+        It offers overloads for STL containers, Boost, Eigen, xtensor, and OpenCV.</p>
+        <table class="table">
+          <thead>
+            <tr>
+              <td>H5Easy</td>
+              <td>h5py</td>
+            </tr>
+          </thead>
+          <tbody>
+            <tr>
+              <td>
+                <div class="card w-100">
+                  <div class="code card-body"><img src="godbolt.org.ico" id="gb_example_easy_highfive" width=32 height=32  class="godbolt float-end img-thumbnail">
+                    <pre class="font-monospace"><div class="example" data-lang="cpp" id="example_easy_highfive"></div></pre>
+                  </div>
+                </div>
+              </td>
+              <td>
+                <div class="card w-100">
+                  <div class="code card-body">
+                    <pre class="font-monospace"><div class="example" data-lang="py" id="example_easy_h5py"></div></pre>
+                  </div>
+                </div>
+              </td>
+            </tr>
+          </tbody>
+        </table>
+      </div>
+
+      <div class="container mb-5">
         <h2>Obtaining and building HighFive</h2>
         <p>HighFive is developed open-source and can be cloned and forked from
         <a href="https://github.com/BlueBrain/HighFive">GitHub</a>.
         It can also be installed from the clone,
         via <a href="https://spack.readthedocs.io/en/latest/package_list.html#highfive">spack</a>,
         or via <a href="https://anaconda.org/conda-forge/highfive">conda</a>.
         It can then be used for example with <code>find_package(HighFive)</code> in CMake.
@@ -218,12 +252,13 @@
             </span>
           </div>
           <div class="col-md-4 justify-content-end list-unstyled d-flex">
             <span class="text-muted">Boost Software License 1.0</span>
           </div>
         </footer>
       </div>
+
       <!-- Example code loading -->
       <script src="examples.js"></script>
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -52,14 +52,21 @@
 ***** HighFive for parallel applications *****
 With the aim to support large-scale scientific application, we have made an
 effort to also natively support the HDF5 MPI backend in HighFive. A special
 MPIOFileDriver is used in the application code to ensure that HDF5 is correctly
 initialized. No other special API calls are required since all necessary
 provisions are handled transparently.
 [godbolt.org.ico]
+***** H5Easy: one-liners *****
+HighFive also offers the H5Easy API (on its own namespace). This has an API in
+which things can be done in one-liners, with a syntax comparable to for example
+h5py for Python. It offers overloads for STL containers, Boost, Eigen, xtensor,
+and OpenCV.
+H5Easy            h5py
+[godbolt.org.ico]
 ***** Obtaining and building HighFive *****
 HighFive is developed open-source and can be cloned and forked from GitHub. It
 can also be installed from the clone, via spack, or via conda. It can then be
 used for example with find_package(HighFive) in CMake. Being a header-only
 library, HighFive can be used directly as a subfolder in a C++ project, for
 example by adding it as a submodule. More details can be found in the
 github.com/BlueBrain/HighFive/blob/master/README.md>README.md
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Attribute.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSet.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 /*
- *  Copyright (c), 2017, Ali Can Demiralp <ali.demiralp@rwth-aachen.de>
+ *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5ATTRIBUTE_HPP
-#define H5ATTRIBUTE_HPP
+#pragma once
 
 #include <vector>
 
 #include "H5DataSpace.hpp"
 #include "H5DataType.hpp"
 #include "H5Object.hpp"
+#include "bits/H5_definitions.hpp"
+#include "bits/H5Annotate_traits.hpp"
+#include "bits/H5Slice_traits.hpp"
 #include "bits/H5Path_traits.hpp"
+#include "bits/H5_definitions.hpp"
 
 namespace HighFive {
 
 ///
-/// \brief Class representing an attribute of a dataset or group
+/// \brief Class representing a dataset.
 ///
-class Attribute: public Object, public PathTraits<Attribute> {
+class DataSet: public Object,
+               public SliceTraits<DataSet>,
+               public AnnotateTraits<DataSet>,
+               public PathTraits<DataSet> {
   public:
-    const static ObjectType type = ObjectType::Attribute;
+    const static ObjectType type = ObjectType::Dataset;
 
     ///
-    /// \brief return the name of the current attribute
-    /// \return the name of the attribute
-    std::string getName() const;
+    /// \brief getStorageSize
+    /// \return returns the amount of storage allocated for a dataset.
+    ///
+    uint64_t getStorageSize() const;
 
-    size_t getStorageSize() const;
+    ///
+    /// \brief getOffset
+    /// \return returns DataSet address in file
+    ///
+    uint64_t getOffset() const;
 
     ///
     /// \brief getDataType
     /// \return return the datatype associated with this dataset
     ///
     DataType getDataType() const;
 
@@ -47,53 +58,59 @@
     ///
     /// \brief getMemSpace
     /// \return same than getSpace for DataSet, compatibility with Selection
     /// class
     ///
     DataSpace getMemSpace() const;
 
-    ///
-    /// Read the attribute into a buffer
-    /// An exception is raised if the numbers of dimension of the buffer and of
-    /// the attribute are different
-    ///
-    /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
-    /// dimensional array )
-    template <typename T>
-    void read(T& array) const;
 
+    /// \brief Change the size of the dataset
     ///
-    /// Read the attribute into a buffer
-    ///
-    template <typename T>
-    void read(T* array, const DataType& dtype = DataType()) const;
+    /// This requires that the dataset was created with chunking, and you would
+    /// generally want to have set a larger maxdims setting
+    /// \param dims New size of the dataset
+    void resize(const std::vector<size_t>& dims);
 
-    ///
-    /// Write the integrality N-dimension buffer to this attribute
-    /// An exception is raised if the numbers of dimension of the buffer and of
-    /// the attribute are different
-    ///
-    /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
-    /// dimensional array )
-    template <typename T>
-    void write(const T& buffer);
 
+    /// \brief Get the dimensions of the whole DataSet.
+    ///       This is a shorthand for getSpace().getDimensions()
+    /// \return The shape of the current HighFive::DataSet
     ///
-    /// Write a buffer to this attribute
+    inline std::vector<size_t> getDimensions() const {
+        return getSpace().getDimensions();
+    }
+
+    /// \brief Get the total number of elements in the current dataset.
+    ///       E.g. 2x2x2 matrix has size 8.
+    ///       This is a shorthand for getSpace().getTotalCount()
+    /// \return The shape of the current HighFive::DataSet
     ///
-    template <typename T>
-    void write_raw(const T* buffer, const DataType& dtype = DataType());
+    inline size_t getElementCount() const {
+        return getSpace().getElementCount();
+    }
+
+    /// \brief Get the list of properties for creation of this dataset
+    DataSetCreateProps getCreatePropertyList() const {
+        return details::get_plist<DataSetCreateProps>(*this, H5Dget_create_plist);
+    }
+
+    /// \brief Get the list of properties for accession of this dataset
+    DataSetAccessProps getAccessPropertyList() const {
+        return details::get_plist<DataSetAccessProps>(*this, H5Dget_access_plist);
+    }
 
-    // No empty attributes
-    Attribute() = delete;
+    /// \deprecated Default constructor creates unsafe uninitialized objects
+    H5_DEPRECATED("Default constructor creates unsafe uninitialized objects")
+    DataSet() = default;
 
-  private:
-    using Object::Object;
+  protected:
+    using Object::Object;  // bring DataSet(hid_t)
 
+    DataSet(Object&& o) noexcept
+        : Object(std::move(o)) {}
+
+    friend class Reference;
     template <typename Derivate>
-    friend class ::HighFive::AnnotateTraits;
+    friend class NodeTraits;
 };
 
 }  // namespace HighFive
-
-
-#endif  // H5ATTRIBUTE_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5DataSet.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSpace.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -2,107 +2,117 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5DATASET_HPP
-#define H5DATASET_HPP
+#pragma once
 
 #include <vector>
+#include <array>
+#include <cstdint>
+#include <type_traits>
+#include <initializer_list>
 
-#include "H5DataSpace.hpp"
-#include "H5DataType.hpp"
 #include "H5Object.hpp"
 #include "bits/H5_definitions.hpp"
-#include "bits/H5Annotate_traits.hpp"
-#include "bits/H5Slice_traits.hpp"
-#include "bits/H5Path_traits.hpp"
-#include "bits/H5_definitions.hpp"
 
 namespace HighFive {
 
 ///
-/// \brief Class representing a dataset.
+/// \brief Class representing the space (dimensions) of a dataset
 ///
-class DataSet: public Object,
-               public SliceTraits<DataSet>,
-               public AnnotateTraits<DataSet>,
-               public PathTraits<DataSet> {
+class DataSpace: public Object {
   public:
-    const static ObjectType type = ObjectType::Dataset;
+    const static ObjectType type = ObjectType::DataSpace;
 
-    ///
-    /// \brief getStorageSize
-    /// \return returns the amount of storage allocated for a dataset.
-    ///
-    uint64_t getStorageSize() const;
+    static const size_t UNLIMITED = SIZE_MAX;
 
-    ///
-    /// \brief getOffset
-    /// \return returns DataSet address in file
-    ///
-    uint64_t getOffset() const;
+    /// dataspace type
+    enum DataspaceType {
+        dataspace_scalar,
+        dataspace_null
+        // simple dataspace are handle directly from their dimensions
+    };
 
+    /// create a dataspace of N-dimensions
+    /// Each dimension is configured this way
+    ///  size(dim1) = vec[0]
+    ///  size(dim2) = vec[1]
+    ///  etc...
+    explicit DataSpace(const std::vector<size_t>& dims);
+
+    // create a dataspace of N-dimensions
+    template <size_t N>
+    explicit DataSpace(const std::array<size_t, N>& dims);
+
+    /// Make sure that DataSpace({1,2,3}) works on GCC. This is
+    /// the shortcut form of the vector initializer, but one some compilers (gcc)
+    /// this does not resolve correctly without this constructor.
+    DataSpace(const std::initializer_list<size_t>& items);
+
+    /// Allow directly listing 1 or more dimensions to initialize,
+    /// that is, DataSpace(1,2) means DataSpace(std::vector<size_t>{1,2}).
+    template <typename... Args>
+    explicit DataSpace(size_t dim1, Args... dims);
+
+    /// Create a dataspace from an iterator pair
     ///
-    /// \brief getDataType
-    /// \return return the datatype associated with this dataset
-    ///
-    DataType getDataType() const;
+    /// Explicitly disable DataSpace(int_like, int_like) from trying to use this constructor
+    template <typename IT,
+              typename = typename std::enable_if<!std::is_integral<IT>::value, IT>::type>
+    DataSpace(const IT begin, const IT end);
+
+    /// \brief Create a resizable N-dimensional dataspace
+    /// \param dims Initial size of dataspace
+    /// \param maxdims Maximum size of the dataspace
+    explicit DataSpace(const std::vector<size_t>& dims, const std::vector<size_t>& maxdims);
 
     ///
-    /// \brief getSpace
-    /// \return return the dataspace associated with this dataset
+    /// \brief DataSpace create a scalar dataspace or a null dataset
     ///
-    DataSpace getSpace() const;
+    explicit DataSpace(DataspaceType dtype);
+
+    /// Create a new DataSpace
+    ///  with a different id available for modifications
+    DataSpace clone() const;
 
     ///
-    /// \brief getMemSpace
-    /// \return same than getSpace for DataSet, compatibility with Selection
-    /// class
+    /// \brief getNumberDimensions
+    /// \return the number of dimensions in the current dataspace
     ///
-    DataSpace getMemSpace() const;
+    size_t getNumberDimensions() const;
 
+    /// \brief getDimensions
+    /// \return return a vector of N-element, each element is the size of the
+    /// associated dataset dimension
+    std::vector<size_t> getDimensions() const;
 
-    /// \brief Change the size of the dataset
-    ///
-    /// This requires that the dataset was created with chunking, and you would
-    /// generally want to have set a larger maxdims setting
-    /// \param dims New size of the dataset
-    void resize(const std::vector<size_t>& dims);
+    /// \brief getElementCount
+    /// \return the total number of elements in the dataspace
+    size_t getElementCount() const;
 
+    /// \brief getMaxDimensions
+    /// \return return a vector of N-element, each element is the size of the
+    /// associated dataset maximum dimension
+    std::vector<size_t> getMaxDimensions() const;
 
-    /// \brief Get the dimensions of the whole DataSet.
-    ///       This is a shorthand for getSpace().getDimensions()
-    /// \return The shape of the current HighFive::DataSet
-    ///
-    inline std::vector<size_t> getDimensions() const {
-        return getSpace().getDimensions();
-    }
-
-    /// \brief Get the total number of elements in the current dataset.
-    ///       E.g. 2x2x2 matrix has size 8.
-    ///       This is a shorthand for getSpace().getTotalCount()
-    /// \return The shape of the current HighFive::DataSet
-    ///
-    inline size_t getElementCount() const {
-        return getSpace().getElementCount();
-    }
+    /// Create a dataspace matching a type accepted by details::inspector
+    template <typename T>
+    static DataSpace From(const T& value);
 
-    H5_DEPRECATED("Default constructor creates unsafe uninitialized objects")
-    DataSet() = default;
+    template <std::size_t N, std::size_t Width>
+    static DataSpace FromCharArrayStrings(const char (&)[N][Width]);
 
   protected:
-    using Object::Object;  // bring DataSet(hid_t)
-
-    DataSet(Object&& o) noexcept
-        : Object(std::move(o)) {}
+    DataSpace() = default;
 
-    friend class Reference;
-    template <typename Derivate>
-    friend class NodeTraits;
+    friend class Attribute;
+    friend class File;
+    friend class DataSet;
 };
 
 }  // namespace HighFive
 
-#endif  // H5DATASET_HPP
+// We include bits right away since DataSpace is user-constructible
+#include "bits/H5Dataspace_misc.hpp"
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5DataSpace.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Attribute.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,152 @@
 /*
- *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
+ *  Copyright (c), 2017, Ali Can Demiralp <ali.demiralp@rwth-aachen.de>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5DATASPACE_HPP
-#define H5DATASPACE_HPP
+#pragma once
 
 #include <vector>
-#include <array>
-#include <cstdint>
-#include <type_traits>
-#include <initializer_list>
 
+#include <H5Apublic.h>
+
+#include "H5DataType.hpp"
 #include "H5Object.hpp"
-#include "bits/H5_definitions.hpp"
+#include "bits/H5Friends.hpp"
+#include "bits/H5Path_traits.hpp"
 
 namespace HighFive {
+class DataSpace;
+
+namespace detail {
 
+/// \brief Internal hack to create an `Attribute` from an ID.
 ///
-/// \brief Class representing the space (dimensions) of a dataset
+/// WARNING: Creating an Attribute from an ID has implications w.r.t. the lifetime of the object
+///          that got passed via its ID. Using this method careless opens up the suite of issues
+///          related to C-style resource management, including the analog of double free, dangling
+///          pointers, etc.
 ///
-class DataSpace: public Object {
-  public:
-    const static ObjectType type = ObjectType::DataSpace;
-
-    static const size_t UNLIMITED = SIZE_MAX;
-
-    /// dataspace type
-    enum DataspaceType {
-        dataspace_scalar,
-        dataspace_null
-        // simple dataspace are handle directly from their dimensions
-    };
-
-    /// create a dataspace of N-dimensions
-    /// Each dimension is configured this way
-    ///  size(dim1) = vec[0]
-    ///  size(dim2) = vec[1]
-    ///  etc...
-    explicit DataSpace(const std::vector<size_t>& dims);
+/// NOTE: This is not part of the API and only serves to work around a compiler issue in GCC which
+///       prevents us from using `friend`s instead. This function should only be used for internal
+///       purposes. The problematic construct is:
+///
+///           template<class Derived>
+///           friend class SomeCRTP<Derived>;
+///
+/// \private
+Attribute make_attribute(hid_t hid);
+}  // namespace detail
 
-    // create a dataspace of N-dimensions
-    template <size_t N>
-    explicit DataSpace(const std::array<size_t, N>& dims);
+///
+/// \brief Class representing an attribute of a dataset or group
+///
+class Attribute: public Object, public PathTraits<Attribute> {
+  public:
+    const static ObjectType type = ObjectType::Attribute;
 
-    /// Make sure that DataSpace({1,2,3}) works on GCC. This is
-    /// the shortcut form of the vector initializer, but one some compilers (gcc)
-    /// this does not resolve correctly without this constructor.
-    DataSpace(const std::initializer_list<size_t>& items);
+    ///
+    /// \brief return the name of the current attribute
+    /// \return the name of the attribute
+    std::string getName() const;
 
-    /// Allow directly listing 1 or more dimensions to initialize,
-    /// that is, DataSpace(1,2) means DataSpace(std::vector<size_t>{1,2}).
-    template <typename... Args>
-    explicit DataSpace(size_t dim1, Args... dims);
+    size_t getStorageSize() const;
 
-    /// Create a dataspace from an iterator pair
     ///
-    /// Explicitly disable DataSpace(int_like, int_like) from trying to use this constructor
-    template <typename IT,
-              typename = typename std::enable_if<!std::is_integral<IT>::value, IT>::type>
-    DataSpace(const IT begin, const IT end);
+    /// \brief getDataType
+    /// \return return the datatype associated with this dataset
+    ///
+    DataType getDataType() const;
 
-    /// \brief Create a resizable N-dimensional dataspace
-    /// \param dims Initial size of dataspace
-    /// \param maxdims Maximum size of the dataspace
-    explicit DataSpace(const std::vector<size_t>& dims, const std::vector<size_t>& maxdims);
+    ///
+    /// \brief getSpace
+    /// \return return the dataspace associated with this dataset
+    ///
+    DataSpace getSpace() const;
 
     ///
-    /// \brief DataSpace create a scalar dataspace or a null dataset
+    /// \brief getMemSpace
+    /// \return same than getSpace for DataSet, compatibility with Selection
+    /// class
     ///
-    explicit DataSpace(DataspaceType dtype);
+    DataSpace getMemSpace() const;
 
-    /// Create a new DataSpace
-    ///  with a different id available for modifications
-    DataSpace clone() const;
+    /// \brief Return the attribute
+    template <typename T>
+    T read() const;
 
     ///
-    /// \brief getNumberDimensions
-    /// \return the number of dimensions in the current dataspace
+    /// Read the attribute into a buffer
+    /// An exception is raised if the numbers of dimension of the buffer and of
+    /// the attribute are different
     ///
-    size_t getNumberDimensions() const;
+    /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
+    /// dimensional array )
+    template <typename T>
+    void read(T& array) const;
 
-    /// \brief getDimensions
-    /// \return return a vector of N-element, each element is the size of the
-    /// associated dataset dimension
-    std::vector<size_t> getDimensions() const;
+    /// \brief Read the attribute into a buffer.
+    ///
+    /// Note, this is the shallowest wrapper around `H5Aread`.
+    template <typename T>
+    void read(T* array, const DataType& mem_datatype) const;
+
+    /// \brief Read the attribute into a buffer
+    ///
+    /// This overload deduces the memory datatype from `T`.
+    template <typename T>
+    void read(T* array) const;
 
-    /// \brief getElementCount
-    /// \return the total number of elements in the dataspace
-    size_t getElementCount() const;
+    ///
+    /// Write the integrality N-dimension buffer to this attribute
+    /// An exception is raised if the numbers of dimension of the buffer and of
+    /// the attribute are different
+    ///
+    /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
+    /// dimensional array )
+    template <typename T>
+    void write(const T& buffer);
 
-    /// \brief getMaxDimensions
-    /// \return return a vector of N-element, each element is the size of the
-    /// associated dataset maximum dimension
-    std::vector<size_t> getMaxDimensions() const;
+    /// \brief Write to this attribute from `buffer`.
+    ///
+    /// Note that this is the shallowest wrapper around `H5Awrite`. It's useful
+    /// if you need full control. If possible prefer `Attribute::write`.
+    template <typename T>
+    void write_raw(const T* buffer, const DataType& mem_dtype);
 
-    /// Create a dataspace matching a type accepted by details::inspector
+    /// \brief Write to this attribute from `buffer`.
+    ///
+    /// This version attempts to automatically deduce the datatype
+    /// of the buffer. Note, that the file datatype is already set.
     template <typename T>
-    static DataSpace From(const T& value);
+    void write_raw(const T* buffer);
+
+    /// \brief Get the list of properties for creation of this attribute
+    AttributeCreateProps getCreatePropertyList() const {
+        return details::get_plist<AttributeCreateProps>(*this, H5Aget_create_plist);
+    }
 
-    template <std::size_t N, std::size_t Width>
-    static DataSpace FromCharArrayStrings(const char (&)[N][Width]);
+    // No empty attributes
+    Attribute() = delete;
 
   protected:
-    DataSpace() = default;
+    using Object::Object;
 
-    friend class Attribute;
-    friend class File;
-    friend class DataSet;
-};
+  private:
+#if HIGHFIVE_HAS_FRIEND_DECLARATIONS
+    template <typename Derivate>
+    friend class ::HighFive::AnnotateTraits;
+#endif
 
-}  // namespace HighFive
+    friend Attribute detail::make_attribute(hid_t);
+};
 
-// We include bits right away since DataSpace is user-constructible
-#include "bits/H5Dataspace_misc.hpp"
+namespace detail {
+inline Attribute make_attribute(hid_t hid) {
+    return Attribute(hid);
+}
+}  // namespace detail
 
-#endif  // H5DATASPACE_HPP
+}  // namespace HighFive
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5DataType.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataType.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,55 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5DATATYPE_HPP
-#define H5DATATYPE_HPP
+#pragma once
 
+#include <type_traits>
 #include <vector>
 
 #include "H5Object.hpp"
 #include "bits/H5Utils.hpp"
 
+#include "H5PropertyList.hpp"
+
 namespace HighFive {
 
 
 ///
 /// \brief Enum of Fundamental data classes
 ///
 enum class DataTypeClass {
-    Time,
-    Integer,
-    Float,
-    String,
-    BitField,
-    Opaque,
-    Compound,
-    Reference,
-    Enum,
-    VarLen,
-    Array,
-    Invalid
+    Time = 1 << 1,
+    Integer = 1 << 2,
+    Float = 1 << 3,
+    String = 1 << 4,
+    BitField = 1 << 5,
+    Opaque = 1 << 6,
+    Compound = 1 << 7,
+    Reference = 1 << 8,
+    Enum = 1 << 9,
+    VarLen = 1 << 10,
+    Array = 1 << 11,
+    Invalid = 0
 };
 
+inline DataTypeClass operator|(DataTypeClass lhs, DataTypeClass rhs) {
+    using T = std::underlying_type<DataTypeClass>::type;
+    return static_cast<DataTypeClass>(static_cast<T>(lhs) | static_cast<T>(rhs));
+}
+
+inline DataTypeClass operator&(DataTypeClass lhs, DataTypeClass rhs) {
+    using T = std::underlying_type<DataTypeClass>::type;
+    return static_cast<DataTypeClass>(static_cast<T>(lhs) & static_cast<T>(rhs));
+}
+
 
 ///
 /// \brief HDF5 Data Type
 ///
 class DataType: public Object {
   public:
     bool operator==(const DataType& other) const;
@@ -78,14 +90,19 @@
     /// Such value might represent auto-detection of the datatype from a buffer
     ///
     bool empty() const noexcept;
 
     /// \brief Returns whether the type is a Reference
     bool isReference() const;
 
+    /// \brief Get the list of properties for creation of this DataType
+    DataTypeCreateProps getCreatePropertyList() const {
+        return details::get_plist<DataTypeCreateProps>(*this, H5Tget_create_plist);
+    }
+
   protected:
     using Object::Object;
 
     friend class Attribute;
     friend class File;
     friend class DataSet;
     friend class CompoundType;
@@ -382,16 +399,14 @@
 /// enum FooBar { FOO = 1, BAR = 2 };
 /// EnumType create_enum_foobar() {
 ///    return EnumType<FooBar>({{"FOO", FooBar::FOO},
 ///                             {"BAR", FooBar::BAR}});
 /// }
 /// HIGHFIVE_REGISTER_TYPE(FooBar, create_enum_foobar)
 /// \endcode
-#define HIGHFIVE_REGISTER_TYPE(type, function)             \
-    template <>                                            \
-    HighFive::DataType HighFive::create_datatype<type>() { \
-        return function();                                 \
+#define HIGHFIVE_REGISTER_TYPE(type, function)                    \
+    template <>                                                   \
+    inline HighFive::DataType HighFive::create_datatype<type>() { \
+        return function();                                        \
     }
 
 #include "bits/H5DataType_misc.hpp"
-
-#endif  // H5DATATYPE_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Easy.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Easy.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 /// Read/dump DataSets or Attribute using a minimalistic syntax.
 /// To this end, the functions are templated, and accept:
 /// - Any type accepted by HighFive
 /// - Eigen objects
 /// - xtensor objects
 /// - OpenCV objects
 
-#ifndef H5EASY_HPP
-#define H5EASY_HPP
+#pragma once
 
 #include <string>
 #include <vector>
 
 // optionally enable xtensor plug-in and load the library
 #ifdef XTENSOR_VERSION_MAJOR
 #ifndef H5_USE_XTENSOR
@@ -395,9 +394,7 @@
 #include "h5easy_bits/H5Easy_Eigen.hpp"
 #include "h5easy_bits/H5Easy_misc.hpp"
 #include "h5easy_bits/H5Easy_opencv.hpp"
 #include "h5easy_bits/H5Easy_public.hpp"
 #include "h5easy_bits/H5Easy_scalar.hpp"
 #include "h5easy_bits/H5Easy_vector.hpp"
 #include "h5easy_bits/H5Easy_xtensor.hpp"
-
-#endif  // H5EASY_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Exception.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Exception.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EXCEPTION_HPP
-#define H5EXCEPTION_HPP
+#pragma once
 
 #include <memory>
 #include <stdexcept>
 #include <string>
 
 #include <H5Ipublic.h>
 
@@ -159,9 +158,7 @@
   public:
     ReferenceException(const std::string& err_msg)
         : Exception(err_msg) {}
 };
 }  // namespace HighFive
 
 #include "bits/H5Exception_misc.hpp"
-
-#endif  // H5EXCEPTION_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5File.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5File.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,21 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5FILE_HPP
-#define H5FILE_HPP
+#pragma once
 
 #include <string>
 
 #include "H5FileDriver.hpp"
 #include "H5Object.hpp"
+#include "H5PropertyList.hpp"
 #include "bits/H5Annotate_traits.hpp"
 #include "bits/H5Node_traits.hpp"
 
 namespace HighFive {
 
 ///
 /// \brief File class
@@ -52,14 +52,27 @@
     ///
     /// Open or create a new HDF5 file
     explicit File(const std::string& filename,
                   unsigned openFlags = ReadOnly,
                   const FileAccessProps& fileAccessProps = FileAccessProps::Default());
 
     ///
+    /// \brief File
+    /// \param filename: filepath of the HDF5 file
+    /// \param openFlags: Open mode / flags ( ReadOnly, ReadWrite)
+    /// \param fileCreateProps: the file create properties
+    /// \param fileAccessProps: the file access properties
+    ///
+    /// Open or create a new HDF5 file
+    File(const std::string& filename,
+         unsigned openFlags,
+         const FileCreateProps& fileCreateProps,
+         const FileAccessProps& fileAccessProps = FileAccessProps::Default());
+
+    ///
     /// \brief Return the name of the file
     ///
     const std::string& getName() const noexcept;
 
 
     /// \brief Object path of a File is always "/"
     std::string getPath() const noexcept {
@@ -68,32 +81,50 @@
 
     /// \brief Returns the block size for metadata in bytes
     hsize_t getMetadataBlockSize() const;
 
     /// \brief Returns the HDF5 version compatibility bounds
     std::pair<H5F_libver_t, H5F_libver_t> getVersionBounds() const;
 
+#if H5_VERSION_GE(1, 10, 1)
+    /// \brief Returns the HDF5 file space strategy.
+    H5F_fspace_strategy_t getFileSpaceStrategy() const;
+
+    /// \brief Returns the page size, if paged allocation is used.
+    hsize_t getFileSpacePageSize() const;
+#endif
+
     ///
     /// \brief flush
     ///
     /// Flushes all buffers associated with a file to disk
     ///
     void flush();
 
-  private:
+    /// \brief Get the list of properties for creation of this file
+    FileCreateProps getCreatePropertyList() const {
+        return details::get_plist<FileCreateProps>(*this, H5Fget_create_plist);
+    }
+
+    /// \brief Get the list of properties for accession of this file
+    FileAccessProps getAccessPropertyList() const {
+        return details::get_plist<FileAccessProps>(*this, H5Fget_access_plist);
+    }
+
+  protected:
+    File() = default;
     using Object::Object;
 
+  private:
     mutable std::string _filename{};
 
     template <typename>
     friend class PathTraits;
 };
 
 }  // namespace HighFive
 
 // H5File is the main user constructible -> bring in implementation headers
 #include "bits/H5Annotate_traits_misc.hpp"
 #include "bits/H5File_misc.hpp"
 #include "bits/H5Node_traits_misc.hpp"
 #include "bits/H5Path_traits_misc.hpp"
-
-#endif  // H5FILE_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5FileDriver.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5FileDriver.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,31 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5FILEDRIVER_HPP
-#define H5FILEDRIVER_HPP
+#pragma once
 
 #include "H5PropertyList.hpp"
+#include "bits/H5_definitions.hpp"
 
 namespace HighFive {
 
-///
 /// \brief file driver base concept
-///
-class FileDriver: public FileAccessProps {};
+/// \deprecated Use FileAccessProps directly
+class H5_DEPRECATED("Use FileAccessProps directly") FileDriver: public FileAccessProps {};
 
 #ifdef H5_HAVE_PARALLEL
-///
 /// \brief MPIIO Driver for Parallel HDF5
-///
-class MPIOFileDriver: public FileAccessProps {
+/// \deprecated Add MPIOFileAccess directly to FileAccessProps
+class H5_DEPRECATED("Add MPIOFileAccess directly to FileAccessProps") MPIOFileDriver
+    : public FileAccessProps {
   public:
     inline MPIOFileDriver(MPI_Comm mpi_comm, MPI_Info mpi_info);
-
-  private:
 };
 #endif
 
 }  // namespace HighFive
 
 #include "bits/H5FileDriver_misc.hpp"
-
-#endif  // H5FILEDRIVER_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Reference.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Reference.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,30 @@
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
 
-#ifndef H5REFERENCE_HPP
-#define H5REFERENCE_HPP
+#pragma once
 
 #include <string>
 #include <vector>
 
 #include <H5Ipublic.h>
 #include <H5Rpublic.h>
 
-#include "H5Object.hpp"
 #include "bits/H5_definitions.hpp"
 
 namespace HighFive {
 
+namespace details {
+template <typename T>
+struct inspector;
+}
 ///
 /// \brief An HDF5 (object) reference type
 ///
 /// HDF5 object references allow pointing to groups, datasets (and compound types). They
 /// differ from links in their ability to be stored and retrieved as data from the HDF5
 /// file in datasets themselves.
 ///
@@ -67,15 +69,13 @@
   private:
     Object get_ref(const Object& location) const;
 
     hobj_ref_t href{};
     std::string obj_name{};
     hid_t parent_id{};
 
-    friend details::data_converter<std::vector<Reference>>;
+    friend struct details::inspector<Reference>;
 };
 
 }  // namespace HighFive
 
 #include "bits/H5Reference_misc.hpp"
-
-#endif  // H5REFERENCE_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/H5Selection.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Selection.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,27 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5SELECTION_HPP
-#define H5SELECTION_HPP
+#pragma once
 
 #include "H5DataSet.hpp"
 #include "H5DataSpace.hpp"
 #include "bits/H5Slice_traits.hpp"
+#include "bits/H5Friends.hpp"
 
 namespace HighFive {
 
+namespace detail {
+Selection make_selection(const DataSpace&, const DataSpace&, const DataSet&);
+}
+
 ///
 /// \brief Selection: represent a view on a slice/part of a dataset
 ///
 /// A Selection is valid only if its parent dataset is valid
 ///
 class Selection: public SliceTraits<Selection> {
   public:
@@ -43,21 +47,22 @@
     const DataSet& getDataset() const noexcept;
 
     ///
     /// \brief return the datatype of the selection
     /// \return return the datatype of the selection
     const DataType getDataType() const;
 
-  private:
+  protected:
     Selection(const DataSpace& memspace, const DataSpace& file_space, const DataSet& set);
 
+  private:
     DataSpace _mem_space, _file_space;
     DataSet _set;
 
+#if HIGHFIVE_HAS_FRIEND_DECLARATIONS
     template <typename Derivate>
     friend class ::HighFive::SliceTraits;
-    // absolute namespace naming due to GCC bug 52625
+#endif
+    friend Selection detail::make_selection(const DataSpace&, const DataSpace&, const DataSet&);
 };
 
 }  // namespace HighFive
-
-#endif  // H5SELECTION_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5ANNOTATE_TRAITS_HPP
-#define H5ANNOTATE_TRAITS_HPP
+#pragma once
 
 #include <string>
 
 #include "../H5Attribute.hpp"
 
 namespace HighFive {
 
@@ -76,10 +75,7 @@
     /// \return number of attributes
     bool hasAttribute(const std::string& attr_name) const;
 
   private:
     using derivate_type = Derivate;
 };
 }  // namespace HighFive
-
-
-#endif  // H5ANNOTATE_TRAITS_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5ANNOTATE_TRAITS_MISC_HPP
-#define H5ANNOTATE_TRAITS_MISC_HPP
+#pragma once
 
 #include <string>
 #include <vector>
 
 #include <H5Apublic.h>
 #include <H5Ppublic.h>
 
@@ -22,23 +21,23 @@
 
 template <typename Derivate>
 inline Attribute AnnotateTraits<Derivate>::createAttribute(const std::string& attribute_name,
                                                            const DataSpace& space,
                                                            const DataType& dtype) {
     auto attr_id = H5Acreate2(static_cast<Derivate*>(this)->getId(),
                               attribute_name.c_str(),
-                              dtype._hid,
-                              space._hid,
+                              dtype.getId(),
+                              space.getId(),
                               H5P_DEFAULT,
                               H5P_DEFAULT);
     if (attr_id < 0) {
         HDF5ErrMapper::ToException<AttributeException>(
             std::string("Unable to create the attribute \"") + attribute_name + "\":");
     }
-    return Attribute(attr_id);
+    return detail::make_attribute(attr_id);
 }
 
 template <typename Derivate>
 template <typename Type>
 inline Attribute AnnotateTraits<Derivate>::createAttribute(const std::string& attribute_name,
                                                            const DataSpace& space) {
     return createAttribute(attribute_name, space, create_and_check_datatype<Type>());
@@ -68,15 +67,15 @@
 inline Attribute AnnotateTraits<Derivate>::getAttribute(const std::string& attribute_name) const {
     const auto attr_id =
         H5Aopen(static_cast<const Derivate*>(this)->getId(), attribute_name.c_str(), H5P_DEFAULT);
     if (attr_id < 0) {
         HDF5ErrMapper::ToException<AttributeException>(
             std::string("Unable to open the attribute \"") + attribute_name + "\":");
     }
-    return Attribute(attr_id);
+    return detail::make_attribute(attr_id);
 }
 
 template <typename Derivate>
 inline size_t AnnotateTraits<Derivate>::getNumberAttributes() const {
     int res = H5Aget_num_attrs(static_cast<const Derivate*>(this)->getId());
     if (res < 0) {
         HDF5ErrMapper::ToException<AttributeException>(
@@ -113,9 +112,7 @@
         HDF5ErrMapper::ToException<AttributeException>(
             std::string("Unable to check for attribute in group"));
     }
     return res;
 }
 
 }  // namespace HighFive
-
-#endif  // H5ANNOTATE_TRAITS_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5DATASET_MISC_HPP
-#define H5DATASET_MISC_HPP
+#pragma once
 
 #include <algorithm>
 #include <functional>
 #include <numeric>
 #include <sstream>
 #include <string>
 
@@ -62,9 +61,7 @@
 
     if (H5Dset_extent(getId(), real_dims.data()) < 0) {
         HDF5ErrMapper::ToException<DataSetException>("Could not resize dataset.");
     }
 }
 
 }  // namespace HighFive
-
-#endif  // H5DATASET_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,92 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5DATATYPE_MISC_HPP
-#define H5DATATYPE_MISC_HPP
+#pragma once
 
 #include <string>
 #include <complex>
 #include <cstring>
+#if HIGHFIVE_CXX_STD >= 17
+#include <cstddef>
+#endif
 
 #include <H5Ppublic.h>
 #include <H5Tpublic.h>
 
+#ifdef H5_USE_HALF_FLOAT
+#include <half.hpp>
+#endif
+
+#include "H5Converter_misc.hpp"
 
 namespace HighFive {
 
+namespace detail {
+
+inline hid_t h5t_copy(hid_t original) {
+    auto copy = H5Tcopy(original);
+    if (copy == H5I_INVALID_HID) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error copying datatype.");
+    }
+
+    return copy;
+}
+
+inline hsize_t h5t_get_size(hid_t hid) {
+    hsize_t size = H5Tget_size(hid);
+    if (size == 0) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error getting size of datatype.");
+    }
+
+    return size;
+}
+
+inline H5T_cset_t h5t_get_cset(hid_t hid) {
+    auto cset = H5Tget_cset(hid);
+    if (cset == H5T_CSET_ERROR) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error getting cset of datatype.");
+    }
+
+    return cset;
+}
+
+inline H5T_str_t h5t_get_strpad(hid_t hid) {
+    auto strpad = H5Tget_strpad(hid);
+    if (strpad == H5T_STR_ERROR) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error getting strpad of datatype.");
+    }
+
+    return strpad;
+}
+
+inline void h5t_set_size(hid_t hid, hsize_t size) {
+    if (H5Tset_size(hid, size) < 0) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error setting size of datatype.");
+    }
+}
+
+inline void h5t_set_cset(hid_t hid, H5T_cset_t cset) {
+    if (H5Tset_cset(hid, cset) < 0) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error setting cset of datatype.");
+    }
+}
+
+inline void h5t_set_strpad(hid_t hid, H5T_str_t strpad) {
+    if (H5Tset_strpad(hid, strpad) < 0) {
+        HDF5ErrMapper::ToException<DataTypeException>("Error setting strpad of datatype.");
+    }
+}
+}  // namespace detail
+
+
 namespace {  // unnamed
 inline DataTypeClass convert_type_class(const H5T_class_t& tclass);
 inline std::string type_class_string(DataTypeClass);
 inline hid_t create_string(std::size_t length);
 }  // namespace
 
 inline bool DataType::empty() const noexcept {
@@ -30,15 +95,15 @@
 }
 
 inline DataTypeClass DataType::getClass() const {
     return convert_type_class(H5Tget_class(_hid));
 }
 
 inline size_t DataType::getSize() const {
-    return H5Tget_size(_hid);
+    return detail::h5t_get_size(_hid);
 }
 
 inline bool DataType::operator==(const DataType& other) const {
     return (H5Tequal(_hid, other._hid) > 0);
 }
 
 inline bool DataType::operator!=(const DataType& other) const {
@@ -64,99 +129,116 @@
 inline std::string DataType::string() const {
     return type_class_string(getClass()) + std::to_string(getSize() * 8);
 }
 
 // char mapping
 template <>
 inline AtomicType<char>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_CHAR);
+    _hid = detail::h5t_copy(H5T_NATIVE_CHAR);
 }
 
 template <>
 inline AtomicType<signed char>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_SCHAR);
+    _hid = detail::h5t_copy(H5T_NATIVE_SCHAR);
 }
 
 template <>
 inline AtomicType<unsigned char>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_UCHAR);
+    _hid = detail::h5t_copy(H5T_NATIVE_UCHAR);
 }
 
 // short mapping
 template <>
 inline AtomicType<short>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_SHORT);
+    _hid = detail::h5t_copy(H5T_NATIVE_SHORT);
 }
 
 template <>
 inline AtomicType<unsigned short>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_USHORT);
+    _hid = detail::h5t_copy(H5T_NATIVE_USHORT);
 }
 
 // integer mapping
 template <>
 inline AtomicType<int>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_INT);
+    _hid = detail::h5t_copy(H5T_NATIVE_INT);
 }
 
 template <>
 inline AtomicType<unsigned>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_UINT);
+    _hid = detail::h5t_copy(H5T_NATIVE_UINT);
 }
 
 // long mapping
 template <>
 inline AtomicType<long>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_LONG);
+    _hid = detail::h5t_copy(H5T_NATIVE_LONG);
 }
 
 template <>
 inline AtomicType<unsigned long>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_ULONG);
+    _hid = detail::h5t_copy(H5T_NATIVE_ULONG);
 }
 
 // long long mapping
 template <>
 inline AtomicType<long long>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_LLONG);
+    _hid = detail::h5t_copy(H5T_NATIVE_LLONG);
 }
 
 template <>
 inline AtomicType<unsigned long long>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_ULLONG);
+    _hid = detail::h5t_copy(H5T_NATIVE_ULLONG);
 }
 
-// float, double and long double mapping
+// half-float, float, double and long double mapping
+#ifdef H5_USE_HALF_FLOAT
+using float16_t = half_float::half;
+
 template <>
-inline AtomicType<float>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_FLOAT);
+inline AtomicType<float16_t>::AtomicType() {
+    _hid = detail::h5t_copy(H5T_NATIVE_FLOAT);
+    // Sign position, exponent position, exponent size, mantissa position, mantissa size
+    H5Tset_fields(_hid, 15, 10, 5, 0, 10);
+    // Total datatype size (in bytes)
+    detail::h5t_set_size(_hid, 2);
+    // Floating point exponent bias
+    H5Tset_ebias(_hid, 15);
 }
+#endif
 
 template <>
-inline AtomicType<double>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_DOUBLE);
+inline AtomicType<float>::AtomicType() {
+    _hid = detail::h5t_copy(H5T_NATIVE_FLOAT);
 }
 
 template <>
-inline AtomicType<long double>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_LDOUBLE);
+inline AtomicType<double>::AtomicType() {
+    _hid = detail::h5t_copy(H5T_NATIVE_DOUBLE);
 }
 
-// boolean mapping
 template <>
-inline AtomicType<bool>::AtomicType() {
-    _hid = H5Tcopy(H5T_NATIVE_HBOOL);
+inline AtomicType<long double>::AtomicType() {
+    _hid = detail::h5t_copy(H5T_NATIVE_LDOUBLE);
 }
 
 // std string
 template <>
 inline AtomicType<std::string>::AtomicType() {
     _hid = create_string(H5T_VARIABLE);
 }
 
+#if HIGHFIVE_CXX_STD >= 17
+// std byte
+template <>
+inline AtomicType<std::byte>::AtomicType() {
+    _hid = detail::h5t_copy(H5T_NATIVE_B8);
+}
+#endif
+
 // Fixed-Length strings
 // require class specialization templated for the char length
 template <size_t StrLen>
 class AtomicType<char[StrLen]>: public DataType {
   public:
     inline AtomicType()
         : DataType(create_string(StrLen)) {}
@@ -177,14 +259,19 @@
               CompoundType({{"r", create_datatype<T>(), 0}, {"i", create_datatype<T>(), sizeof(T)}},
                            sizeof(std::complex<T>))) {
         static_assert(std::is_floating_point<T>::value,
                       "std::complex accepts only floating point numbers.");
     }
 };
 
+// For boolean we act as h5py
+inline EnumType<details::Boolean> create_enum_boolean() {
+    return {{"FALSE", details::Boolean::HighFiveFalse}, {"TRUE", details::Boolean::HighFiveTrue}};
+}
+
 // Other cases not supported. Fail early with a user message
 template <typename T>
 AtomicType<T>::AtomicType() {
     static_assert(details::inspector<T>::recursive_ndim == 0,
                   "Atomic types cant be arrays, except for char[] (fixed-length strings)");
     static_assert(details::inspector<T>::recursive_ndim > 0, "Type not supported");
 }
@@ -238,50 +325,69 @@
     return std::string(datavec[i].data());
 }
 
 // Internal
 // Reference mapping
 template <>
 inline AtomicType<Reference>::AtomicType() {
-    _hid = H5Tcopy(H5T_STD_REF_OBJ);
+    _hid = detail::h5t_copy(H5T_STD_REF_OBJ);
 }
 
 inline size_t find_first_atomic_member_size(hid_t hid) {
     // Recursive exit condition
-    if (H5Tget_class(hid) != H5T_COMPOUND) {
-        return H5Tget_size(hid);
-    }
+    if (H5Tget_class(hid) == H5T_COMPOUND) {
+        auto number_of_members = H5Tget_nmembers(hid);
+        if (number_of_members == -1) {
+            throw DataTypeException("Cannot get members of CompoundType with hid: " +
+                                    std::to_string(hid));
+        }
+        if (number_of_members == 0) {
+            throw DataTypeException("No members defined for CompoundType with hid: " +
+                                    std::to_string(hid));
+        }
 
-    auto number_of_members = H5Tget_nmembers(hid);
-    if (number_of_members == -1) {
-        throw DataTypeException("Cannot get members of CompoundType with hid: " +
-                                std::to_string(hid));
-    }
-    if (number_of_members == 0) {
-        throw DataTypeException("No members defined for CompoundType with hid: " +
-                                std::to_string(hid));
+        auto member_type = H5Tget_member_type(hid, 0);
+        auto size = find_first_atomic_member_size(member_type);
+        H5Tclose(member_type);
+        return size;
+    } else if (H5Tget_class(hid) == H5T_STRING) {
+        return 1;
     }
-
-    auto member_type = H5Tget_member_type(hid, 0);
-    auto size = find_first_atomic_member_size(member_type);
-    H5Tclose(member_type);
-    return size;
+    return detail::h5t_get_size(hid);
 }
 
 // Calculate the padding required to align an element of a struct
-#define _H5_STRUCT_PADDING(current_size, member_size) \
-    ((std::max(member_size, current_size) - std::min(member_size, current_size)) % (member_size))
+// For padding see explanation here: https://en.cppreference.com/w/cpp/language/object#Alignment
+// It is to compute padding following last element inserted inside a struct
+// 1) We want to push back an element padded to the structure
+// 'current_size' is the size of the structure before adding the new element.
+// 'member_size' the size of the element we want to add.
+// 2) We want to compute the final padding for the global structure
+// 'current_size' is the size of the whole structure without final padding
+// 'member_size' is the maximum size of all element of the struct
+//
+// The basic formula is only to know how much we need to add to 'current_size' to fit
+// 'member_size'.
+// And at the end, we do another computation because the end padding, should fit the biggest
+// element of the struct.
+//
+// As we are with `size_t` element, we need to compute everything inside R+
+#define _H5_STRUCT_PADDING(current_size, member_size)                                \
+    (((member_size) >= (current_size))                                               \
+         ? (((member_size) - (current_size)) % (member_size))                        \
+         : ((((member_size) - (((current_size) - (member_size)) % (member_size)))) % \
+            (member_size)))
 
 inline void CompoundType::create(size_t size) {
     if (size == 0) {
         size_t current_size = 0, max_atomic_size = 0;
 
         // Do a first pass to find the total size of the compound datatype
         for (auto& member: members) {
-            size_t member_size = H5Tget_size(member.base_type.getId());
+            size_t member_size = detail::h5t_get_size(member.base_type.getId());
 
             if (member_size == 0) {
                 throw DataTypeException("Cannot get size of DataType with hid: " +
                                         std::to_string(member.base_type.getId()));
             }
 
             size_t first_atomic_size = find_first_atomic_member_size(member.base_type.getId());
@@ -341,20 +447,17 @@
 inline void EnumType<T>::commit(const Object& object, const std::string& name) const {
     H5Tcommit2(object.getId(), name.c_str(), getId(), H5P_DEFAULT, H5P_DEFAULT, H5P_DEFAULT);
 }
 
 namespace {
 
 inline hid_t create_string(size_t length) {
-    hid_t _hid = H5Tcopy(H5T_C_S1);
-    if (H5Tset_size(_hid, length) < 0) {
-        HDF5ErrMapper::ToException<DataTypeException>("Unable to define datatype size to variable");
-    }
-    // define encoding to UTF-8 by default
-    H5Tset_cset(_hid, H5T_CSET_UTF8);
+    hid_t _hid = detail::h5t_copy(H5T_C_S1);
+    detail::h5t_set_size(_hid, length);
+    detail::h5t_set_cset(_hid, H5T_CSET_UTF8);
     return _hid;
 }
 
 
 inline DataTypeClass convert_type_class(const H5T_class_t& tclass) {
     switch (tclass) {
     case H5T_TIME:
@@ -451,10 +554,8 @@
         throw DataTypeException(ss.str());
     }
 
     return t;
 }
 
 }  // namespace HighFive
-
-
-#endif  // H5DATATYPE_MISC_HPP
+HIGHFIVE_REGISTER_TYPE(HighFive::details::Boolean, HighFive::create_enum_boolean)
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5DATASPACE_MISC_HPP
-#define H5DATASPACE_MISC_HPP
+#pragma once
 
 #include <array>
 #include <initializer_list>
 #include <vector>
 #include <numeric>
 
 #include <H5Spublic.h>
 
 #include "H5Utils.hpp"
+#include "H5Converter_misc.hpp"
 
 namespace HighFive {
 
 inline DataSpace::DataSpace(const std::vector<size_t>& dims)
     : DataSpace(dims.begin(), dims.end()) {}
 
 template <size_t N>
@@ -137,34 +137,13 @@
 inline DataSpace DataSpace::FromCharArrayStrings(const char (&)[N][Width]) {
     return DataSpace(N);
 }
 
 namespace details {
 
 /// dimension checks @internal
-inline bool checkDimensions(const DataSpace& mem_space, size_t input_dims) {
-    size_t dataset_dims = mem_space.getNumberDimensions();
-    if (input_dims == dataset_dims)
-        return true;
-
-    const std::vector<size_t>& dims = mem_space.getDimensions();
-    for (auto i = dims.crbegin(); i != --dims.crend() && *i == 1; ++i)
-        --dataset_dims;
-
-    if (input_dims == dataset_dims)
-        return true;
-
-    dataset_dims = dims.size();
-    for (auto i = dims.cbegin(); i != --dims.cend() && *i == 1; ++i)
-        --dataset_dims;
-
-    if (input_dims == dataset_dims)
-        return true;
-
-    // The final tests is for scalars
-    return input_dims == 0 && dataset_dims == 1 && dims[dims.size() - 1] == 1;
+inline bool checkDimensions(const DataSpace& mem_space, size_t n_dim_requested) {
+    return checkDimensions(mem_space.getDimensions(), n_dim_requested);
 }
 
 }  // namespace details
 }  // namespace HighFive
-
-#endif  // H5DATASPACE_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EXCEPTION_MISC_HPP
-#define H5EXCEPTION_MISC_HPP
+#pragma once
 
 #include <cstdlib>
 #include <sstream>
 
 #include <H5Epublic.h>
 
 namespace HighFive {
@@ -24,14 +23,17 @@
 
         const char* major_err = H5Eget_major(err_desc->maj_num);
         const char* minor_err = H5Eget_minor(err_desc->min_num);
 
         std::ostringstream oss;
         oss << '(' << major_err << ") " << minor_err;
 
+        H5free_memory((void*) major_err);
+        H5free_memory((void*) minor_err);
+
         auto* e = new ExceptionType(oss.str());
         e->_err_major = err_desc->maj_num;
         e->_err_minor = err_desc->min_num;
         (*e_iter)->_next.reset(e);
         *e_iter = e;
         return 0;
     }
@@ -54,9 +56,7 @@
         }
         // throw generic error, unrecognized error
         throw ExceptionType(prefix_msg + ": Unknown HDF5 error");
     }
 };
 
 }  // namespace HighFive
-
-#endif  // H5OBJECT_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,18 @@
  *                            Juan Hernando <juan.hernando@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5FILEDRIVER_MISC_HPP
-#define H5FILEDRIVER_MISC_HPP
+#pragma once
 
 namespace HighFive {
 
 #ifdef H5_HAVE_PARALLEL
 inline MPIOFileDriver::MPIOFileDriver(MPI_Comm comm, MPI_Info info) {
     add(MPIOFileAccess(comm, info));
 }
 #endif
 
 }  // namespace HighFive
-
-#endif  // H5FILEDRIVER_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5FILE_MISC_HPP
-#define H5FILE_MISC_HPP
+#pragma once
 
 #include <string>
 
 #include <H5Fpublic.h>
 
 #include "../H5Utility.hpp"
 #include "H5Utils.hpp"
@@ -34,17 +33,23 @@
         res_open |= H5F_ACC_TRUNC;
     if (openFlags & File::Excl)
         res_open |= H5F_ACC_EXCL;
     return res_open;
 }
 }  // namespace
 
+inline File::File(const std::string& filename,
+                  unsigned openFlags,
+                  const FileAccessProps& fileAccessProps)
+    : File(filename, openFlags, FileCreateProps::Default(), fileAccessProps) {}
+
 
 inline File::File(const std::string& filename,
                   unsigned openFlags,
+                  const FileCreateProps& fileCreateProps,
                   const FileAccessProps& fileAccessProps) {
     openFlags = convert_open_flag(openFlags);
 
     unsigned createMode = openFlags & (H5F_ACC_TRUNC | H5F_ACC_EXCL);
     unsigned openMode = openFlags & (H5F_ACC_RDWR | H5F_ACC_RDONLY);
     bool mustCreate = createMode > 0;
     bool openOrCreate = (openFlags & H5F_ACC_CREAT) > 0;
@@ -67,51 +72,59 @@
             createMode = H5F_ACC_EXCL;
         } else {
             HDF5ErrMapper::ToException<FileException>(
                 std::string("Unable to open file " + filename));
         }
     }
 
-    if ((_hid = H5Fcreate(filename.c_str(), createMode, H5P_DEFAULT, fileAccessProps.getId())) <
-        0) {
+    auto fcpl = fileCreateProps.getId();
+    auto fapl = fileAccessProps.getId();
+    if ((_hid = H5Fcreate(filename.c_str(), createMode, fcpl, fapl)) < 0) {
         HDF5ErrMapper::ToException<FileException>(std::string("Unable to create file " + filename));
     }
 }
 
 inline const std::string& File::getName() const noexcept {
     if (_filename.empty()) {
         _filename = details::get_name(
             [this](char* buffer, size_t length) { return H5Fget_name(getId(), buffer, length); });
     }
     return _filename;
 }
 
 inline hsize_t File::getMetadataBlockSize() const {
-    hsize_t size;
-    auto fid_fapl = H5Fget_access_plist(getId());
-    if (H5Pget_meta_block_size(fid_fapl, &size) < 0) {
-        HDF5ErrMapper::ToException<FileException>(
-            std::string("Unable to access file metadata block size"));
-    }
-    return size;
+    auto fapl = getAccessPropertyList();
+    return MetadataBlockSize(fapl).getSize();
 }
 
 inline std::pair<H5F_libver_t, H5F_libver_t> File::getVersionBounds() const {
-    H5F_libver_t low;
-    H5F_libver_t high;
-    auto fid_fapl = H5Fget_access_plist(getId());
-    if (H5Pget_libver_bounds(fid_fapl, &low, &high) < 0) {
+    auto fapl = getAccessPropertyList();
+    auto fileVer = FileVersionBounds(fapl);
+    return fileVer.getVersion();
+}
+
+#if H5_VERSION_GE(1, 10, 1)
+inline H5F_fspace_strategy_t File::getFileSpaceStrategy() const {
+    auto fcpl = getCreatePropertyList();
+    FileSpaceStrategy spaceStrategy(fcpl);
+    return spaceStrategy.getStrategy();
+}
+
+inline hsize_t File::getFileSpacePageSize() const {
+    auto fcpl = getCreatePropertyList();
+
+    if (getFileSpaceStrategy() != H5F_FSPACE_STRATEGY_PAGE) {
         HDF5ErrMapper::ToException<FileException>(
-            std::string("Unable to access file version bounds"));
+            std::string("Cannot obtain page size as paged allocation is not used."));
     }
-    return std::make_pair(low, high);
+
+    return FileSpacePageSize(fcpl).getPageSize();
 }
+#endif
 
 inline void File::flush() {
     if (H5Fflush(_hid, H5F_SCOPE_GLOBAL) < 0) {
         HDF5ErrMapper::ToException<FileException>(std::string("Unable to flush file " + getName()));
     }
 }
 
 }  // namespace HighFive
-
-#endif  // H5FILE_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5ITERABLE_MISC_HPP
-#define H5ITERABLE_MISC_HPP
+#pragma once
 
 #include <exception>
 #include <string>
 #include <vector>
 
 #include <H5Ipublic.h>
 
@@ -49,9 +48,7 @@
         data->err = new ObjectException("Exception during H5Iterate, abort listing");
     }
     return -1;
 }
 
 }  // namespace details
 }  // namespace HighFive
-
-#endif  // H5ITERABLE_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,29 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5NODE_TRAITS_HPP
-#define H5NODE_TRAITS_HPP
+#pragma once
 
 #include <string>
 
 #include "../H5PropertyList.hpp"
 #include "H5_definitions.hpp"
+#include "H5Converter_misc.hpp"
 
 namespace HighFive {
 
+enum class IndexType : std::underlying_type<H5_index_t>::type {
+    NAME = H5_INDEX_NAME,
+    CRT_ORDER = H5_INDEX_CRT_ORDER,
+};
+
 ///
 /// \brief NodeTraits: Base class for Group and File
 ///
 template <typename Derivate>
 class NodeTraits {
   public:
     ///
@@ -44,15 +49,28 @@
     /// size specified by space
     /// \param dataset_name identifier of the dataset
     /// \param space Associated DataSpace, see \ref DataSpace for more information
     /// \param createProps A property list with data set creation properties
     /// \param accessProps A property list with data set access properties
     /// \param parents Create intermediate groups if needed. Default: true.
     /// \return DataSet Object
-    template <typename Type>
+    template <typename T,
+              typename std::enable_if<
+                  std::is_same<typename details::inspector<T>::base_type, details::Boolean>::value,
+                  int>::type* = nullptr>
+    DataSet createDataSet(const std::string& dataset_name,
+                          const DataSpace& space,
+                          const DataSetCreateProps& createProps = DataSetCreateProps::Default(),
+                          const DataSetAccessProps& accessProps = DataSetAccessProps::Default(),
+                          bool parents = true);
+
+    template <typename T,
+              typename std::enable_if<
+                  !std::is_same<typename details::inspector<T>::base_type, details::Boolean>::value,
+                  int>::type* = nullptr>
     DataSet createDataSet(const std::string& dataset_name,
                           const DataSpace& space,
                           const DataSetCreateProps& createProps = DataSetCreateProps::Default(),
                           const DataSetAccessProps& accessProps = DataSetAccessProps::Default(),
                           bool parents = true);
 
     ///
@@ -129,16 +147,19 @@
     /// \return boolean that is true if the move was successful
     bool rename(const std::string& src_path,
                 const std::string& dest_path,
                 bool parents = true) const;
 
     ///
     /// \brief list all leaf objects name of the node / group
+    /// \param idx_type tell if the list should be ordered by Name or CreationOrderTime.
+    /// CreationOrderTime can be use only if the file/group has been created with
+    /// the HighFive::LinkCreationTime property.
     /// \return number of leaf objects
-    std::vector<std::string> listObjectNames() const;
+    std::vector<std::string> listObjectNames(IndexType idx_type = IndexType::NAME) const;
 
     ///
     /// \brief check a dataset or group exists in the current node / group
     /// \param node_name dataset/group name to check
     /// \return true if a dataset/group with the associated name exists, or false
     bool exist(const std::string& node_name) const;
 
@@ -209,10 +230,7 @@
     Soft,
     External,
     Other  // Reserved or User-defined
 };
 
 
 }  // namespace HighFive
-
-
-#endif  // H5NODE_TRAITS_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5NODE_TRAITS_MISC_HPP
-#define H5NODE_TRAITS_MISC_HPP
+#pragma once
 
 #include <string>
 #include <vector>
 
 #include <H5Apublic.h>
 #include <H5Dpublic.h>
 #include <H5Fpublic.h>
@@ -38,35 +37,56 @@
                                                    const DataSetCreateProps& createProps,
                                                    const DataSetAccessProps& accessProps,
                                                    bool parents) {
     LinkCreateProps lcpl;
     lcpl.add(CreateIntermediateGroup(parents));
     const auto hid = H5Dcreate2(static_cast<Derivate*>(this)->getId(),
                                 dataset_name.c_str(),
-                                dtype._hid,
-                                space._hid,
+                                dtype.getId(),
+                                space.getId(),
                                 lcpl.getId(),
                                 createProps.getId(),
                                 accessProps.getId());
     if (hid < 0) {
         HDF5ErrMapper::ToException<DataSetException>(
             std::string("Unable to create the dataset \"") + dataset_name + "\":");
     }
     return DataSet(hid);
 }
 
 template <typename Derivate>
-template <typename Type>
+template <typename T,
+          typename std::enable_if<
+              std::is_same<typename details::inspector<T>::base_type, details::Boolean>::value,
+              int>::type*>
+inline DataSet NodeTraits<Derivate>::createDataSet(const std::string& dataset_name,
+                                                   const DataSpace& space,
+                                                   const DataSetCreateProps& createProps,
+                                                   const DataSetAccessProps& accessProps,
+                                                   bool parents) {
+    return createDataSet(dataset_name,
+                         space,
+                         create_and_check_datatype<typename details::inspector<T>::base_type>(),
+                         createProps,
+                         accessProps,
+                         parents);
+}
+
+template <typename Derivate>
+template <typename T,
+          typename std::enable_if<
+              !std::is_same<typename details::inspector<T>::base_type, details::Boolean>::value,
+              int>::type*>
 inline DataSet NodeTraits<Derivate>::createDataSet(const std::string& dataset_name,
                                                    const DataSpace& space,
                                                    const DataSetCreateProps& createProps,
                                                    const DataSetAccessProps& accessProps,
                                                    bool parents) {
     return createDataSet(
-        dataset_name, space, create_and_check_datatype<Type>(), createProps, accessProps, parents);
+        dataset_name, space, create_and_check_datatype<T>(), createProps, accessProps, parents);
 }
 
 template <typename Derivate>
 template <typename T>
 inline DataSet NodeTraits<Derivate>::createDataSet(const std::string& dataset_name,
                                                    const T& data,
                                                    const DataSetCreateProps& createProps,
@@ -118,15 +138,15 @@
                                 lcpl.getId(),
                                 H5P_DEFAULT,
                                 H5P_DEFAULT);
     if (hid < 0) {
         HDF5ErrMapper::ToException<GroupException>(std::string("Unable to create the group \"") +
                                                    group_name + "\":");
     }
-    return Group(hid);
+    return detail::make_group(hid);
 }
 
 template <typename Derivate>
 inline Group NodeTraits<Derivate>::createGroup(const std::string& group_name,
                                                const GroupCreateProps& createProps,
                                                bool parents) {
     LinkCreateProps lcpl;
@@ -136,26 +156,26 @@
                                 lcpl.getId(),
                                 createProps.getId(),
                                 H5P_DEFAULT);
     if (hid < 0) {
         HDF5ErrMapper::ToException<GroupException>(std::string("Unable to create the group \"") +
                                                    group_name + "\":");
     }
-    return Group(hid);
+    return detail::make_group(hid);
 }
 
 template <typename Derivate>
 inline Group NodeTraits<Derivate>::getGroup(const std::string& group_name) const {
     const auto hid =
         H5Gopen2(static_cast<const Derivate*>(this)->getId(), group_name.c_str(), H5P_DEFAULT);
     if (hid < 0) {
         HDF5ErrMapper::ToException<GroupException>(std::string("Unable to open the group \"") +
                                                    group_name + "\":");
     }
-    return Group(hid);
+    return detail::make_group(hid);
 }
 
 template <typename Derivate>
 inline size_t NodeTraits<Derivate>::getNumberObjects() const {
     hsize_t res;
     if (H5Gget_num_objs(static_cast<const Derivate*>(this)->getId(), &res) < 0) {
         HDF5ErrMapper::ToException<GroupException>(
@@ -195,23 +215,23 @@
                                                    dst_path + "\":");
         return false;
     }
     return true;
 }
 
 template <typename Derivate>
-inline std::vector<std::string> NodeTraits<Derivate>::listObjectNames() const {
+inline std::vector<std::string> NodeTraits<Derivate>::listObjectNames(IndexType idx_type) const {
     std::vector<std::string> names;
     details::HighFiveIterateData iterateData(names);
 
     size_t num_objs = getNumberObjects();
     names.reserve(num_objs);
 
     if (H5Literate(static_cast<const Derivate*>(this)->getId(),
-                   H5_INDEX_NAME,
+                   static_cast<H5_index_t>(idx_type),
                    H5_ITER_INC,
                    NULL,
                    &details::internal_high_five_iterate<H5L_info_t>,
                    static_cast<void*>(&iterateData)) < 0) {
         HDF5ErrMapper::ToException<GroupException>(std::string("Unable to list objects in group"));
     }
 
@@ -345,14 +365,12 @@
     const auto id = H5Oopen(static_cast<const Derivate*>(this)->getId(),
                             node_name.c_str(),
                             accessProps.getId());
     if (id < 0) {
         HDF5ErrMapper::ToException<GroupException>(std::string("Unable to open \"") + node_name +
                                                    "\":");
     }
-    return Object(id);
+    return detail::make_object(id);
 }
 
 
 }  // namespace HighFive
-
-#endif  // H5NODE_TRAITS_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,28 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5OBJECT_MISC_HPP
-#define H5OBJECT_MISC_HPP
+#pragma once
 
 #include <iostream>
 
+#include "../H5Exception.hpp"
+#include "../H5Utility.hpp"
+
 namespace HighFive {
+namespace detail {
+inline Object make_object(hid_t hid) {
+    return Object(hid);
+}
+}  // namespace detail
+
 
 inline Object::Object()
     : _hid(H5I_INVALID_HID) {}
 
 inline Object::Object(hid_t hid)
     : _hid(hid) {}
 
@@ -42,15 +50,15 @@
         }
     }
     return *this;
 }
 
 inline Object::~Object() {
     if (isValid() && H5Idec_ref(_hid) < 0) {
-        std::cerr << "HighFive::~Object: reference counter decrease failure" << std::endl;
+        HIGHFIVE_LOG_ERROR("HighFive::~Object: reference counter decrease failure");
     }
 }
 
 inline bool Object::isValid() const noexcept {
     return (_hid != H5I_INVALID_HID) && (H5Iis_valid(_hid) != false);
 }
 
@@ -109,9 +117,7 @@
 }
 inline time_t ObjectInfo::getModificationTime() const noexcept {
     return raw_info.mtime;
 }
 
 
 }  // namespace HighFive
-
-#endif  // H5OBJECT_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     }
     _file_obj.reset(new File(file_id));
 }
 
 template <typename Derivate>
 inline std::string PathTraits<Derivate>::getPath() const {
     return details::get_name([this](char* buffer, size_t length) {
-        return H5Iget_name(static_cast<const Derivate*>(this)->getId(), buffer, length);
+        return H5Iget_name(static_cast<const Derivate&>(*this).getId(), buffer, length);
     });
 }
 
 template <typename Derivate>
 inline File& PathTraits<Derivate>::getFile() const noexcept {
     return *_file_obj;
 }
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -4,30 +4,56 @@
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
 #pragma once
 
-#include "H5Tpublic.h"
+#include <H5Tpublic.h>
 #include "H5Utils.hpp"
 
 namespace HighFive {
 
 namespace details {
 
 template <typename T>
+using unqualified_t = typename std::remove_const<typename std::remove_reference<T>::type>::type;
+
+// Find the type of an eventual char array, otherwise void
+template <typename>
+struct type_char_array {
+    using type = void;
+};
+
+template <typename T>
+struct type_char_array<T*> {
+    using type = typename std::conditional<std::is_same<unqualified_t<T>, char>::value,
+                                           char*,
+                                           typename type_char_array<T>::type>::type;
+};
+
+template <typename T, std::size_t N>
+struct type_char_array<T[N]> {
+    using type = typename std::conditional<std::is_same<unqualified_t<T>, char>::value,
+                                           char[N],
+                                           typename type_char_array<T>::type>::type;
+};
+
+template <typename T>
 struct BufferInfo {
     using type_no_const = typename std::remove_const<T>::type;
     using elem_type = typename details::inspector<type_no_const>::base_type;
     using char_array_t = typename details::type_char_array<type_no_const>::type;
     static constexpr bool is_char_array = !std::is_same<char_array_t, void>::value;
 
+    enum Operation { read, write };
+    const Operation op;
+
     template <class F>
-    BufferInfo(const DataType& dtype, F getName);
+    BufferInfo(const DataType& dtype, F getName, Operation _op);
 
     // member data for info depending on the destination dataset type
     const bool is_fixed_len_string;
     const size_t n_dimensions;
     const DataType data_type;
 };
 
@@ -76,30 +102,41 @@
         }
         return return_type;
     }
 };
 
 template <typename T>
 template <class F>
-BufferInfo<T>::BufferInfo(const DataType& dtype, F getName)
-    : is_fixed_len_string(dtype.isFixedLenStr())
+BufferInfo<T>::BufferInfo(const DataType& dtype, F getName, Operation _op)
+    : op(_op)
+    , is_fixed_len_string(dtype.isFixedLenStr())
     // In case we are using Fixed-len strings we need to subtract one dimension
     , n_dimensions(details::inspector<type_no_const>::recursive_ndim -
                    ((is_fixed_len_string && is_char_array) ? 1 : 0))
     , data_type(
           string_type_checker<char_array_t>::getDataType(create_datatype<elem_type>(), dtype)) {
     if (is_fixed_len_string && std::is_same<elem_type, std::string>::value) {
         throw DataSetException(
             "Can't output std::string as fixed-length. "
             "Use raw arrays or FixedLenStringArray");
     }
     // We warn. In case they are really not convertible an exception will rise on read/write
     if (dtype.getClass() != data_type.getClass()) {
-        std::cerr << "HighFive WARNING \"" << getName()
-                  << "\": data and hdf5 dataset have different types: " << data_type.string()
-                  << " -> " << dtype.string() << std::endl;
+        HIGHFIVE_LOG_WARN(getName() + "\": data and hdf5 dataset have different types: " +
+                          data_type.string() + " -> " + dtype.string());
+    } else if ((dtype.getClass() & data_type.getClass()) == DataTypeClass::Float) {
+        HIGHFIVE_LOG_WARN_IF(
+            (op == read) && (dtype.getSize() > data_type.getSize()),
+            getName() + "\": hdf5 dataset has higher floating point precision than data on read: " +
+                dtype.string() + " -> " + data_type.string());
+
+        HIGHFIVE_LOG_WARN_IF(
+            (op == write) && (dtype.getSize() < data_type.getSize()),
+            getName() +
+                "\": data has higher floating point precision than hdf5 dataset on write: " +
+                data_type.string() + " -> " + dtype.string());
     }
 }
 
 }  // namespace details
 
 }  // namespace HighFive
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,23 @@
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
 
-#ifndef H5REFERENCE_MISC_HPP
-#define H5REFERENCE_MISC_HPP
+#pragma once
 
 #include <string>
 #include <H5Ppublic.h>
 
 #include "H5Utils.hpp"
 
+#include "../H5Object.hpp"
+
 namespace HighFive {
 
 inline Reference::Reference(const Object& location, const Object& object)
     : parent_id(location.getId()) {
     obj_name = details::get_name(
         [&](char* buffer, size_t length) { return H5Iget_name(object.getId(), buffer, length); });
 }
@@ -60,9 +61,7 @@
         HDF5ErrMapper::ToException<ReferenceException>("Unable to dereference.");
     }
 #endif
     return Object(res);
 }
 
 }  // namespace HighFive
-
-#endif  // H5REFERENCE_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,24 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5SLICE_TRAITS_HPP
-#define H5SLICE_TRAITS_HPP
+#pragma once
 
 #include <cstdlib>
 #include <vector>
 
 #include "H5_definitions.hpp"
 #include "H5Utils.hpp"
 
+#include "../H5PropertyList.hpp"
+
 namespace HighFive {
 
 class ElementSet {
   public:
     ///
     /// \brief Create a list of points of N-dimension for selection.
     ///
@@ -254,81 +255,121 @@
     /// by taking the union of regular hyperslabs. An irregular hyperslab, in general, does not fit
     /// nicely into a multi-dimensional array, but only a subset of such an array.
     ///
     /// Therefore, the only memspaces supported for general hyperslabs are one-dimensional arrays.
     Selection select(const HyperSlab& hyperslab) const;
 
     ///
+    /// \brief Select an \p hyperslab in the current Slice/Dataset.
+    ///
+    /// If the selection can be read into a simple, multi-dimensional dataspace,
+    /// then this overload enable specifying the shape of the memory dataspace
+    /// with `memspace`. Note, that simple implies no offsets, strides or
+    /// number of blocks, just the size of the block in each dimension.
+    Selection select(const HyperSlab& hyperslab, const DataSpace& memspace) const;
+
+    ///
     /// \brief Select a region in the current Slice/Dataset of \p count points at
     /// \p offset separated by \p stride. If strides are not provided they will
     /// default to 1 in all dimensions.
     ///
     /// vector offset and count have to be from the same dimension
     ///
     Selection select(const std::vector<size_t>& offset,
                      const std::vector<size_t>& count,
-                     const std::vector<size_t>& stride = std::vector<size_t>()) const;
+                     const std::vector<size_t>& stride = {},
+                     const std::vector<size_t>& block = {}) const;
 
     ///
     /// \brief Select a set of columns in the last dimension of this dataset.
     ///
     /// The column indices must be smaller than the dimension size.
     ///
     Selection select(const std::vector<size_t>& columns) const;
 
     ///
     /// \brief Select a region in the current Slice/Dataset out of a list of elements.
     ///
     Selection select(const ElementSet& elements) const;
 
+    template <typename T>
+    T read(const DataTransferProps& xfer_props = DataTransferProps()) const;
+
     ///
     /// Read the entire dataset into a buffer
     /// An exception is raised is if the numbers of dimension of the buffer and
     /// of the dataset are different.
     ///
     /// The array type can be a N-pointer or a N-vector. For plain pointers
     /// not dimensionality checking will be performed, it is the user's
     /// responsibility to ensure that the right amount of space has been
     /// allocated.
     template <typename T>
-    void read(T& array) const;
+    void read(T& array, const DataTransferProps& xfer_props = DataTransferProps()) const;
 
     ///
     /// Read the entire dataset into a raw buffer
     ///
     /// No dimensionality checks will be performed, it is the user's
     /// responsibility to ensure that the right amount of space has been
     /// allocated.
     /// \param array: A buffer containing enough space for the data
     /// \param dtype: The type of the data, in case it cannot be automatically guessed
+    /// \param xfer_props: Data Transfer properties
+    template <typename T>
+    void read(T* array,
+              const DataType& dtype,
+              const DataTransferProps& xfer_props = DataTransferProps()) const;
+
+    ///
+    /// Read the entire dataset into a raw buffer
+    ///
+    /// Same as `read(T*, const DataType&, const DataTransferProps&)`. However,
+    /// this overload deduces the HDF5 datatype of the element of `array` from
+    /// `T`. Note, that the file datatype is already fixed.
+    ///
+    /// \param array: A buffer containing enough space for the data
+    /// \param xfer_props: Data Transfer properties
     template <typename T>
-    void read(T* array, const DataType& dtype = DataType()) const;
+    void read(T* array, const DataTransferProps& xfer_props = DataTransferProps()) const;
 
     ///
     /// Write the integrality N-dimension buffer to this dataset
     /// An exception is raised is if the numbers of dimension of the buffer and
     /// of the dataset are different
     ///
     /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
     /// dimensional array )
     template <typename T>
-    void write(const T& buffer);
+    void write(const T& buffer, const DataTransferProps& xfer_props = DataTransferProps());
 
     ///
-    /// Write from a raw buffer into this dataset
+    /// Write from a raw pointer into this dataset.
     ///
     /// No dimensionality checks will be performed, it is the user's
     /// responsibility to ensure that the buffer holds the right amount of
     /// elements. For n-dimensional matrices the buffer layout follows H5
     /// default conventions.
+    ///
+    /// Note, this is the shallowest wrapper around `H5Dwrite` and should
+    /// be used if full control is needed. Generally prefer `write`.
+    ///
     /// \param buffer: A buffer containing the data to be written
-    /// \param dtype: The type of the data, in case it cannot be automatically guessed
+    /// \param dtype: The datatype of `buffer`, i.e. the memory data type.
+    /// \param xfer_props: The HDF5 data transfer properties, e.g. collective MPI-IO.
     template <typename T>
-    void write_raw(const T* buffer, const DataType& dtype = DataType());
+    void write_raw(const T* buffer,
+                   const DataType& mem_datatype,
+                   const DataTransferProps& xfer_props = DataTransferProps());
 
-  protected:
-    inline Selection select_impl(const HyperSlab& hyperslab, const DataSpace& memspace) const;
+    ///
+    /// Write from a raw pointer into this dataset.
+    ///
+    /// Same as `write_raw(const T*, const DataTransferProps&)`. However, this
+    /// overload attempts to guess the data type of `buffer`, i.e. the memory
+    /// datatype. Note that the file datatype is already fixed.
+    ///
+    template <typename T>
+    void write_raw(const T* buffer, const DataTransferProps& xfer_props = DataTransferProps());
 };
 
 }  // namespace HighFive
-
-#endif  // H5SLICE_TRAITS_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,23 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5SLICE_TRAITS_MISC_HPP
-#define H5SLICE_TRAITS_MISC_HPP
+#pragma once
 
 #include <algorithm>
 #include <cassert>
 #include <functional>
 #include <numeric>
 #include <sstream>
 #include <string>
 
-#ifdef H5_USE_BOOST
-// starting Boost 1.64, serialization header must come before ublas
-#include <boost/multi_array.hpp>
-#include <boost/numeric/ublas/matrix.hpp>
-#include <boost/serialization/vector.hpp>
-#endif
-
 #include <H5Dpublic.h>
 #include <H5Ppublic.h>
 
 #include "H5ReadWrite_misc.hpp"
 #include "H5Converter_misc.hpp"
 
 namespace HighFive {
@@ -68,48 +60,49 @@
 inline ElementSet::ElementSet(const std::vector<std::vector<std::size_t>>& element_ids) {
     for (const auto& vec: element_ids) {
         std::copy(vec.begin(), vec.end(), std::back_inserter(_ids));
     }
 }
 
 template <typename Derivate>
-inline Selection SliceTraits<Derivate>::select_impl(const HyperSlab& hyperslab,
-                                                    const DataSpace& memspace) const {
+inline Selection SliceTraits<Derivate>::select(const HyperSlab& hyperslab,
+                                               const DataSpace& memspace) const {
     // Note: The current limitation are that memspace must describe a
     //       packed memspace.
     //
     //       The reason for this is that we're unable to unpack general
     //       hyperslabs when the memory is not contiguous, e.g.
     //       `std::vector<std::vector<double>>`.
     const auto& slice = static_cast<const Derivate&>(*this);
     auto filespace = hyperslab.apply(slice.getSpace());
 
-    return Selection(memspace, filespace, details::get_dataset(slice));
+    return detail::make_selection(memspace, filespace, details::get_dataset(slice));
 }
 
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const HyperSlab& hyper_slab) const {
     const auto& slice = static_cast<const Derivate&>(*this);
     auto filespace = slice.getSpace();
     filespace = hyper_slab.apply(filespace);
 
     auto n_elements = H5Sget_select_npoints(filespace.getId());
     auto memspace = DataSpace(std::array<size_t, 1>{size_t(n_elements)});
 
-    return Selection(memspace, filespace, details::get_dataset(slice));
+    return detail::make_selection(memspace, filespace, details::get_dataset(slice));
 }
 
 
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const std::vector<size_t>& offset,
                                                const std::vector<size_t>& count,
-                                               const std::vector<size_t>& stride) const {
-    auto slab = HyperSlab(RegularHyperSlab(offset, count, stride));
+                                               const std::vector<size_t>& stride,
+                                               const std::vector<size_t>& block) const {
+    auto slab = HyperSlab(RegularHyperSlab(offset, count, stride, block));
     auto memspace = DataSpace(count);
-    return select_impl(slab, memspace);
+    return select(slab, memspace);
 }
 
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const std::vector<size_t>& columns) const {
     const auto& slice = static_cast<const Derivate&>(*this);
     const DataSpace& space = slice.getSpace();
     std::vector<size_t> dims = space.getDimensions();
@@ -124,15 +117,15 @@
         offsets.back() = column;
         slab |= RegularHyperSlab(offsets, counts);
     }
 
     std::vector<size_t> memdims = dims;
     memdims.back() = columns.size();
 
-    return select_impl(slab, DataSpace(memdims));
+    return select(slab, DataSpace(memdims));
 }
 
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const ElementSet& elements) const {
     const auto& slice = static_cast<const Derivate&>(*this);
     const hsize_t* data = nullptr;
     const DataSpace space = slice.getSpace().clone();
@@ -156,96 +149,150 @@
         data = raw_elements.data();
     }
 
     if (H5Sselect_elements(space.getId(), H5S_SELECT_SET, num_elements, data) < 0) {
         HDF5ErrMapper::ToException<DataSpaceException>("Unable to select elements");
     }
 
-    return Selection(DataSpace(num_elements), space, details::get_dataset(slice));
+    return detail::make_selection(DataSpace(num_elements), space, details::get_dataset(slice));
 }
 
 
 template <typename Derivate>
 template <typename T>
-inline void SliceTraits<Derivate>::read(T& array) const {
+inline T SliceTraits<Derivate>::read(const DataTransferProps& xfer_props) const {
+    T array;
+    read(array, xfer_props);
+    return array;
+}
+
+
+template <typename Derivate>
+template <typename T>
+inline void SliceTraits<Derivate>::read(T& array, const DataTransferProps& xfer_props) const {
     const auto& slice = static_cast<const Derivate&>(*this);
     const DataSpace& mem_space = slice.getMemSpace();
-    const details::BufferInfo<T> buffer_info(slice.getDataType(), [slice]() -> std::string {
-        return details::get_dataset(slice).getPath();
-    });
+
+    const details::BufferInfo<T> buffer_info(
+        slice.getDataType(),
+        [&slice]() -> std::string { return details::get_dataset(slice).getPath(); },
+        details::BufferInfo<T>::Operation::read);
 
     if (!details::checkDimensions(mem_space, buffer_info.n_dimensions)) {
         std::ostringstream ss;
         ss << "Impossible to read DataSet of dimensions " << mem_space.getNumberDimensions()
            << " into arrays of dimensions " << buffer_info.n_dimensions;
         throw DataSpaceException(ss.str());
     }
-    details::data_converter<T> converter(mem_space);
-    read(converter.transform_read(array), buffer_info.data_type);
+    auto dims = mem_space.getDimensions();
+
+    if (mem_space.getElementCount() == 0) {
+        auto effective_dims = details::squeezeDimensions(dims,
+                                                         details::inspector<T>::recursive_ndim);
+
+        details::inspector<T>::prepare(array, effective_dims);
+        return;
+    }
+
+    auto r = details::data_converter::get_reader<T>(dims, array);
+    read(r.get_pointer(), buffer_info.data_type, xfer_props);
     // re-arrange results
-    converter.process_result(array);
+    r.unserialize();
+    auto t = create_datatype<typename details::inspector<T>::base_type>();
+    auto c = t.getClass();
+    if (c == DataTypeClass::VarLen || t.isVariableStr()) {
+#if H5_VERSION_GE(1, 12, 0)
+        // This one have been created in 1.12.0
+        (void) H5Treclaim(t.getId(), mem_space.getId(), xfer_props.getId(), r.get_pointer());
+#else
+        // This one is deprecated since 1.12.0
+        (void) H5Dvlen_reclaim(t.getId(), mem_space.getId(), xfer_props.getId(), r.get_pointer());
+#endif
+    }
 }
 
+
 template <typename Derivate>
 template <typename T>
-inline void SliceTraits<Derivate>::read(T* array, const DataType& dtype) const {
+inline void SliceTraits<Derivate>::read(T* array,
+                                        const DataType& mem_datatype,
+                                        const DataTransferProps& xfer_props) const {
     static_assert(!std::is_const<T>::value,
                   "read() requires a non-const structure to read data into");
-    const auto& slice = static_cast<const Derivate&>(*this);
-    using element_type = typename details::inspector<T>::base_type;
 
-    // Auto-detect mem datatype if not provided
-    const DataType& mem_datatype = dtype.empty() ? create_and_check_datatype<element_type>()
-                                                 : dtype;
+    const auto& slice = static_cast<const Derivate&>(*this);
 
     if (H5Dread(details::get_dataset(slice).getId(),
                 mem_datatype.getId(),
                 details::get_memspace_id(slice),
                 slice.getSpace().getId(),
-                H5P_DEFAULT,
+                xfer_props.getId(),
                 static_cast<void*>(array)) < 0) {
-        HDF5ErrMapper::ToException<DataSetException>("Error during HDF5 Read: ");
+        HDF5ErrMapper::ToException<DataSetException>("Error during HDF5 Read.");
     }
 }
 
+template <typename Derivate>
+template <typename T>
+inline void SliceTraits<Derivate>::read(T* array, const DataTransferProps& xfer_props) const {
+    using element_type = typename details::inspector<T>::base_type;
+    const DataType& mem_datatype = create_and_check_datatype<element_type>();
+
+    read(array, mem_datatype, xfer_props);
+}
+
 
 template <typename Derivate>
 template <typename T>
-inline void SliceTraits<Derivate>::write(const T& buffer) {
+inline void SliceTraits<Derivate>::write(const T& buffer, const DataTransferProps& xfer_props) {
     const auto& slice = static_cast<const Derivate&>(*this);
     const DataSpace& mem_space = slice.getMemSpace();
-    const details::BufferInfo<T> buffer_info(slice.getDataType(), [slice]() -> std::string {
-        return details::get_dataset(slice).getPath();
-    });
+
+    if (mem_space.getElementCount() == 0) {
+        return;
+    }
+
+    const details::BufferInfo<T> buffer_info(
+        slice.getDataType(),
+        [&slice]() -> std::string { return details::get_dataset(slice).getPath(); },
+        details::BufferInfo<T>::Operation::write);
 
     if (!details::checkDimensions(mem_space, buffer_info.n_dimensions)) {
         std::ostringstream ss;
-        ss << "Impossible to write buffer of dimensions " << buffer_info.n_dimensions
-           << " into dataset of dimensions " << mem_space.getNumberDimensions();
+        ss << "Impossible to write buffer of dimensions "
+           << details::format_vector(mem_space.getDimensions())
+           << " into dataset with n = " << buffer_info.n_dimensions << " dimensions.";
         throw DataSpaceException(ss.str());
     }
-    details::data_converter<T> converter(mem_space);
-    write_raw(converter.transform_write(buffer), buffer_info.data_type);
+    auto w = details::data_converter::serialize<T>(buffer);
+    write_raw(w.get_pointer(), buffer_info.data_type, xfer_props);
 }
 
 
 template <typename Derivate>
 template <typename T>
-inline void SliceTraits<Derivate>::write_raw(const T* buffer, const DataType& dtype) {
-    using element_type = typename details::inspector<T>::base_type;
+inline void SliceTraits<Derivate>::write_raw(const T* buffer,
+                                             const DataType& mem_datatype,
+                                             const DataTransferProps& xfer_props) {
     const auto& slice = static_cast<const Derivate&>(*this);
-    const auto& mem_datatype = dtype.empty() ? create_and_check_datatype<element_type>() : dtype;
 
     if (H5Dwrite(details::get_dataset(slice).getId(),
                  mem_datatype.getId(),
                  details::get_memspace_id(slice),
                  slice.getSpace().getId(),
-                 H5P_DEFAULT,
+                 xfer_props.getId(),
                  static_cast<const void*>(buffer)) < 0) {
         HDF5ErrMapper::ToException<DataSetException>("Error during HDF5 Write: ");
     }
 }
 
+template <typename Derivate>
+template <typename T>
+inline void SliceTraits<Derivate>::write_raw(const T* buffer, const DataTransferProps& xfer_props) {
+    using element_type = typename details::inspector<T>::base_type;
+    const auto& mem_datatype = create_and_check_datatype<element_type>();
+
+    write_raw(buffer, mem_datatype, xfer_props);
+}
+
 
 }  // namespace HighFive
-
-#endif  // H5SLICE_TRAITS_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #if defined(__GNUC__) || defined(__clang__)
 #define H5_DEPRECATED(msg) __attribute__((deprecated(#msg)))
 #elif defined(_MSC_VER)
 #define H5_DEPRECATED(msg) __declspec(deprecated(#msg))
 #else
 #pragma message("WARNING: Compiler doesnt support deprecation")
-#define H5_DEPRECATED
+#define H5_DEPRECATED(msg)
 #endif
 
 
 // Forward declarations
 
 namespace HighFive {
 
@@ -43,19 +43,8 @@
 
 template <typename Derivate>
 class NodeTraits;
 
 template <PropertyType T>
 class PropertyList;
 
-
-// Internal
-
-namespace details {
-
-// Forward declaration of data_converter with default value of Enable
-template <typename T, typename Enable = void>
-struct data_converter;
-
-}  // namespace details
-
 }  // namespace HighFive
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_EIGEN_HPP
-#define H5EASY_BITS_EIGEN_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 #include "H5Easy_misc.hpp"
 #include "H5Easy_scalar.hpp"
 
 #ifdef H5_USE_EIGEN
 
@@ -140,8 +139,7 @@
     }
 };
 
 }  // namespace detail
 }  // namespace H5Easy
 
 #endif  // H5_USE_EIGEN
-#endif  // H5EASY_BITS_EIGEN_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_MISC_HPP
-#define H5EASY_BITS_MISC_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 
 namespace H5Easy {
 
 namespace detail {
 
@@ -148,9 +147,7 @@
     throw error(file,
                 path,
                 "H5Easy: Attribute exists, overwrite with H5Easy::DumpMode::Overwrite.");
 }
 
 }  // namespace detail
 }  // namespace H5Easy
-
-#endif  // H5EASY_BITS_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_OPENCV_HPP
-#define H5EASY_BITS_OPENCV_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 #include "H5Easy_misc.hpp"
 #include "H5Easy_scalar.hpp"
 
 #ifdef H5_USE_OPENCV
 
@@ -95,8 +94,7 @@
     }
 };
 
 }  // namespace detail
 }  // namespace H5Easy
 
 #endif  // H5_USE_OPENCV
-#endif  // H5EASY_BITS_OPENCV_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_PUBLIC_HPP
-#define H5EASY_BITS_PUBLIC_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 
 namespace H5Easy {
 
 inline Compression::Compression(bool enable) {
     if (enable) {
@@ -165,9 +164,7 @@
 
 template <class T>
 inline T loadAttribute(const File& file, const std::string& path, const std::string& key) {
     return detail::io_impl<T>::loadAttribute(file, path, key);
 }
 
 }  // namespace H5Easy
-
-#endif  // H5EASY_BITS_MISC_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_SCALAR_HPP
-#define H5EASY_BITS_SCALAR_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 #include "H5Easy_misc.hpp"
 
 namespace H5Easy {
 
 namespace detail {
@@ -127,9 +126,7 @@
         dataset.select(idx, ones).read(data);
         return data;
     }
 };
 
 }  // namespace detail
 }  // namespace H5Easy
-
-#endif  // H5EASY_BITS_SCALAR_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_VECTOR_HPP
-#define H5EASY_BITS_VECTOR_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 #include "H5Easy_misc.hpp"
 #include "H5Easy_scalar.hpp"
 
 namespace H5Easy {
 
@@ -75,9 +74,7 @@
         attribute.read(data);
         return data;
     }
 };
 
 }  // namespace detail
 }  // namespace H5Easy
-
-#endif  // H5EASY_BITS_VECTOR_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp` & `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_XTENSOR_HPP
-#define H5EASY_BITS_XTENSOR_HPP
+#pragma once
 
 #include "../H5Easy.hpp"
 #include "H5Easy_misc.hpp"
 #include "H5Easy_scalar.hpp"
 
 #ifdef H5_USE_XTENSOR
 
@@ -79,8 +78,7 @@
     }
 };
 
 }  // namespace detail
 }  // namespace H5Easy
 
 #endif  // H5_USE_XTENSOR
-#endif  // H5EASY_BITS_XTENSOR_HPP
```

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/CMakeLists.txt` & `MorphIO-3.3.5/3rdparty/lexertl14/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/char_traits.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/char_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/debug.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/debug.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/dot.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/dot.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/enums.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/enums.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/generator.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generator.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/internals.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/internals.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/iterator.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/iterator.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/licence_1_0.txt` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/licence_1_0.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/lookup.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/lookup.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/match_results.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/match_results.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/memory_file.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/memory_file.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/narrow.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/narrow.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/parser.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/parser.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/partition/charset.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/charset.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/rules.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/rules.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/runtime_error.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/runtime_error.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/serialise.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/serialise.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/sm_traits.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/state_machine.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/state_machine.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/string_token.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/string_token.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp` & `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/CHANGELOG.md` & `MorphIO-3.3.5/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+v3.3.5
+======
+New Features:
+* Abstraction for morphology collection. (#444)
+
+Improvements:
+* Don't ignore choice of `MORPHIO_ENABLE_COVERAGE`. (#452)
+* enable windows py311, since new h5py release has wheels (#441)
+* Update clang-format CI to 22.04. (#445)
+* Make neurolucida state machine thread-safe (#440)
+* Improve doc (#439)
 
 v3.3.4
 ======
 
 New Features:
 * Add operator-> for iterators, for better ergonomics (#408)
 * Allow SWC and ASC morphologies to be built from strings (#407)
```

### Comparing `MorphIO-3.3.4/CMake/CodeCoverage.cmake` & `MorphIO-3.3.5/CMake/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/CMake/CompilerFlags.cmake` & `MorphIO-3.3.5/CMake/CompilerFlags.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
   # get access to M_PI constant
   set(FLAGS "${FLAGS} /D_USE_MATH_DEFINES")
 
 elseif(CMAKE_CXX_COMPILER_ID MATCHES "Clang")
   # Taken from https://github.com/BlueBrain/hpc-coding-conventions/blob/master/cpp/cmake/bob.cmake#L192-L255
   if(${PROJECT_NAME}_CXX_WARNINGS)
-    set(FLAGS "${FLAGS} -Werror -Weverything")
+    if(${PROJECT_NAME}_WERROR)
+      set(FLAGS "${FLAGS} -Werror")
+    endif()
+    set(FLAGS "${FLAGS} -Weverything")
     # Using std=c++11, no need for 98 compat
     set(FLAGS "${FLAGS} -Wno-c++98-compat")
     set(FLAGS "${FLAGS} -Wno-c++98-compat-pedantic")
 
     # allow static objects
     set(FLAGS "${FLAGS} -Wno-global-constructors")
     set(FLAGS "${FLAGS} -Wno-exit-time-destructors")
@@ -41,19 +44,21 @@
     if(CMAKE_CXX_COMPILER_VERSION VERSION_GREATER "5.0.0")
       set(FLAGS "${FLAGS} -fcomment-block-commands=file")
     endif()
   endif()
 
 elseif(${CMAKE_CXX_COMPILER_ID} STREQUAL "GNU")
   if(${PROJECT_NAME}_CXX_WARNINGS)
+    if(${PROJECT_NAME}_WERROR)
+      set(FLAGS "${FLAGS} -Werror")
+    endif()
     set(FLAGS "${FLAGS} -Wall")
     set(FLAGS "${FLAGS} -Wcast-align")
     set(FLAGS "${FLAGS} -Wconversion")
     set(FLAGS "${FLAGS} -Wdouble-promotion")
-    set(FLAGS "${FLAGS} -Werror")
     set(FLAGS "${FLAGS} -Wextra")
     set(FLAGS "${FLAGS} -Wformat=2")
     set(FLAGS "${FLAGS} -Wnon-virtual-dtor")
     set(FLAGS "${FLAGS} -Wold-style-cast")
     set(FLAGS "${FLAGS} -Woverloaded-virtual")
     set(FLAGS "${FLAGS} -Wshadow")
     set(FLAGS "${FLAGS} -Wsign-conversion")
```

### Comparing `MorphIO-3.3.4/CMakeLists.txt` & `MorphIO-3.3.5/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 set(CMAKE_VERBOSE_MAKEFILE ON)
 
 option(BUILD_BINDINGS "Build the python bindings" ON)
 option(MorphIO_CXX_WARNINGS "Compile C++ with warnings" ON)
+option(MorphIO_WERROR "If compiled with warnings, additionally activate '-Werror'" ON)
 option(EXTERNAL_CATCH2 "Use Catch2 from external source" OFF)
 option(EXTERNAL_HIGHFIVE "Use HighFive from external source" OFF)
 option(EXTERNAL_PYBIND11 "Use pybind11 from external source" OFF)
 option(MORPHIO_TESTS "Build tests" ON)
 option(MORPHIO_USE_DOUBLE "Use doubles instead of floats" OFF)
 
-set(MORPHIO_ENABLE_COVERAGE OFF)
-if (CMAKE_BUILD_TYPE STREQUAL "Debug")
-  set(MORPHIO_ENABLE_COVERAGE ON)
+if (NOT DEFINED MORPHIO_ENABLE_COVERAGE)
+  if (CMAKE_BUILD_TYPE STREQUAL "Debug")
+    set(MORPHIO_ENABLE_COVERAGE ON)
+  else()
+    set(MORPHIO_ENABLE_COVERAGE OFF)
+  endif()
 endif()
 
 if(MORPHIO_USE_DOUBLE)
   add_definitions(-DMORPHIO_USE_DOUBLE)
   message("Floating Point Type: double")
 else()
   message("Floating Point Type: float")
```

### Comparing `MorphIO-3.3.4/CONTRIBUTING.md` & `MorphIO-3.3.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/COPYING` & `MorphIO-3.3.5/COPYING`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/COPYING.LESSER` & `MorphIO-3.3.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/MANIFEST.in` & `MorphIO-3.3.5/MANIFEST.in`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,28 @@
 recursive-include 3rdparty/HighFive/include *
 recursive-include 3rdparty/HighFive/CMake *
 recursive-include 3rdparty/HighFive/doc *
 
 include 3rdparty/lexertl14/CMakeLists.txt
 recursive-include 3rdparty/lexertl14/include/lexertl *
 
+# ghc::filesystem
+recursive-include 3rdparty/ghc_filesystem/include *
+recursive-include 3rdparty/ghc_filesystem/cmake *
+include 3rdparty/ghc_filesystem/CMakeLists.txt
+include 3rdparty/ghc_filesystem/LICENSE
+
 # pybind11 for python bindings
 recursive-include binds/python/pybind11/include *
 recursive-include binds/python/pybind11/tools *.cmake
 include binds/python/pybind11/CMakeLists.txt
 include binds/python/pybind11/LICENSE
 
 # setuptools_scm forces all SCM files to be packaged into sdist
 # we need to manually exclude them to prevent their inclusion
 # see https://github.com/pypa/setuptools_scm/issues/190
 prune ci
 prune doc
 prune tests
 prune scripts
 prune examples
+
```

### Comparing `MorphIO-3.3.4/MorphIO.egg-info/PKG-INFO` & `MorphIO-3.3.5/MorphIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MorphIO
-Version: 3.3.4
+Version: 3.3.5
 Summary: A neuron morphology IO library
 Home-page: https://github.com/BlueBrain/MorphIO/
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Description: .. image:: doc/source/logo/BBP-MorphIO.jpg
```

### Comparing `MorphIO-3.3.4/MorphIO.egg-info/SOURCES.txt` & `MorphIO-3.3.5/MorphIO.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -37,23 +37,25 @@
 3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
 3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
 3rdparty/HighFive/CMake/config/TestHelpers.cmake
 3rdparty/HighFive/doc/CMakeLists.txt
 3rdparty/HighFive/doc/Doxyfile
 3rdparty/HighFive/doc/DoxygenLayout.xml
 3rdparty/HighFive/doc/environment.yaml
-3rdparty/HighFive/doc/mainpage.md
+3rdparty/HighFive/doc/installation.md
 3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
 3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
 3rdparty/HighFive/doc/poster/example1_hdf5.cpp
 3rdparty/HighFive/doc/poster/example1_highfive.cpp
 3rdparty/HighFive/doc/poster/example3.cpp
 3rdparty/HighFive/doc/poster/example6.cpp
 3rdparty/HighFive/doc/poster/example_boost.cpp
 3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
+3rdparty/HighFive/doc/poster/example_easy_h5py.py
+3rdparty/HighFive/doc/poster/example_easy_highfive.cpp
 3rdparty/HighFive/doc/poster/example_eigen.cpp
 3rdparty/HighFive/doc/poster/example_props.cpp
 3rdparty/HighFive/doc/poster/examples.js
 3rdparty/HighFive/doc/poster/godbolt.org.ico
 3rdparty/HighFive/doc/poster/index.html
 3rdparty/HighFive/include/highfive/H5Attribute.hpp
 3rdparty/HighFive/include/highfive/H5DataSet.hpp
@@ -69,22 +71,22 @@
 3rdparty/HighFive/include/highfive/H5Reference.hpp
 3rdparty/HighFive/include/highfive/H5Selection.hpp
 3rdparty/HighFive/include/highfive/H5Utility.hpp
 3rdparty/HighFive/include/highfive/H5Version.hpp.in
 3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
 3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
-3rdparty/HighFive/include/highfive/bits/H5ConverterEigen_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
+3rdparty/HighFive/include/highfive/bits/H5Friends.hpp
 3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
 3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
 3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
 3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
@@ -98,14 +100,24 @@
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
 3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
+3rdparty/ghc_filesystem/CMakeLists.txt
+3rdparty/ghc_filesystem/LICENSE
+3rdparty/ghc_filesystem/cmake/GhcHelper.cmake
+3rdparty/ghc_filesystem/cmake/config.cmake.in
+3rdparty/ghc_filesystem/include/ghc/filesystem.hpp
+3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp
+3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp
+3rdparty/ghc_filesystem/include/ghc/fs_std.hpp
+3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp
+3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp
 3rdparty/lexertl14/CMakeLists.txt
 3rdparty/lexertl14/include/lexertl/char_traits.hpp
 3rdparty/lexertl14/include/lexertl/debug.hpp
 3rdparty/lexertl14/include/lexertl/dot.hpp
 3rdparty/lexertl14/include/lexertl/enums.hpp
 3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
 3rdparty/lexertl14/include/lexertl/generator.hpp
@@ -200,14 +212,15 @@
 binds/python/pybind11/include/pybind11/stl/filesystem.h
 binds/python/pybind11/tools/FindCatch.cmake
 binds/python/pybind11/tools/FindEigen3.cmake
 binds/python/pybind11/tools/FindPythonLibsNew.cmake
 binds/python/pybind11/tools/pybind11Common.cmake
 binds/python/pybind11/tools/pybind11NewTools.cmake
 binds/python/pybind11/tools/pybind11Tools.cmake
+include/morphio/collection.h
 include/morphio/dendritic_spine.h
 include/morphio/endoplasmic_reticulum.h
 include/morphio/enums.h
 include/morphio/errorMessages.h
 include/morphio/exceptions.h
 include/morphio/glial_cell.h
 include/morphio/mito_section.h
@@ -236,26 +249,28 @@
 include/morphio/vasc/properties.h
 include/morphio/vasc/section.h
 include/morphio/vasc/vasculature.h
 morphio/__init__.py
 morphio/mut/__init__.py
 morphio/vasculature/__init__.py
 src/CMakeLists.txt
+src/collection.cpp
 src/dendritic_spine.cpp
 src/endoplasmic_reticulum.cpp
 src/enums.cpp
 src/errorMessages.cpp
 src/glial_cell.cpp
 src/mito_section.cpp
 src/mitochondria.cpp
 src/morphology.cpp
 src/point_utils.cpp
 src/point_utils.h
 src/properties.cpp
 src/section.cpp
+src/shared_utils.cpp
 src/shared_utils.hpp
 src/soma.cpp
 src/version.cpp.in
 src/mut/dendritic_spine.cpp
 src/mut/endoplasmic_reticulum.cpp
 src/mut/glial_cell.cpp
 src/mut/mito_section.cpp
```

### Comparing `MorphIO-3.3.4/PKG-INFO` & `MorphIO-3.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MorphIO
-Version: 3.3.4
+Version: 3.3.5
 Summary: A neuron morphology IO library
 Home-page: https://github.com/BlueBrain/MorphIO/
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Description: .. image:: doc/source/logo/BBP-MorphIO.jpg
```

### Comparing `MorphIO-3.3.4/README.rst` & `MorphIO-3.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/bind_immutable.cpp` & `MorphIO-3.3.5/binds/python/bind_immutable.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,67 @@
 #include <morphio/endoplasmic_reticulum.h>
 #include <morphio/enums.h>
 #include <morphio/glial_cell.h>
 #include <morphio/mut/dendritic_spine.h>
 #include <morphio/mut/endoplasmic_reticulum.h>
 #include <morphio/mut/glial_cell.h>
 #include <morphio/mut/mitochondria.h>
-//#include <morphio/mut/dendritic_spine.h>
 #include <morphio/mut/morphology.h>
 #include <morphio/soma.h>
 #include <morphio/types.h>
 
 #include <memory>  // std::make_unique
 
 #include "bind_enums.h"
 #include "bindings_utils.h"
 
 namespace py = pybind11;
 
-void bind_immutable_module(py::module& m) {
+immutable_binding_classes bind_immutable_classes(py::module& m) {
     using namespace py::literals;
 
     // http://pybind11.readthedocs.io/en/stable/advanced/pycpp/utilities.html?highlight=iostream#capturing-standard-output-from-ostream
     py::add_ostream_redirect(m, "ostream_redirect");
 
-    py::class_<morphio::Morphology>(m, "Morphology")
+    return immutable_binding_classes{
+        py::class_<morphio::Morphology>(m,
+                                        "Morphology",
+                                        "Class representing a complete morphology"),
+        py::class_<morphio::GlialCell, morphio::Morphology>(m,
+                                                            "GlialCell",
+                                                            "Class representing a Glial Cell"),
+        py::class_<morphio::Mitochondria>(
+            m,
+            "Mitochondria",
+            "The entry-point class to access mitochondrial data\n"
+            "By design, it is the equivalent of the Morphology class but at the mitochondrial "
+            "level\n"
+            "As the Morphology class, it implements a section accessor and a root section "
+            "accessor\n"
+            "returning views on the Properties object for the queried mitochondrial section"),
+        py::class_<morphio::EndoplasmicReticulum>(
+            m,
+            "EndoplasmicReticulum",
+            "The entry-point class to access endoplasmic reticulum data\n"
+            "Spec "
+            "https://bbpteam.epfl.ch/documentation/projects/Morphology%20Documentation/latest/"
+            "h5v1.html"),
+        py::class_<morphio::Soma>(m, "Soma", "Class representing a Soma"),
+        py::class_<morphio::Section>(m, "Section", "Class representing a Section"),
+        py::class_<morphio::MitoSection>(m,
+                                         "MitoSection",
+                                         "Class representing a Mitochondrial Section"),
+        py::class_<morphio::DendriticSpine, morphio::Morphology>(
+            m, "DendriticSpine", "Class representing a Dendritic Spine")};
+}
+
+void bind_immutable_methods(immutable_binding_classes& immutable_classes) {
+    using namespace py::literals;
+
+    immutable_classes.Morphology_class
         .def(py::init<const std::string&, unsigned int>(),
              "filename"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
         .def(py::init<const std::string&, const std::string&, unsigned int>(),
              "filename"_a,
              "extension"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
@@ -156,70 +190,57 @@
                 default:
                     throw morphio::MorphioError(
                         "Only iteration types depth_first and breadth_first are supported");
                 }
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
             "Section iterator that runs successively on every neurite\n"
+            "\n"
             "iter_type controls the order of iteration on sections of a given neurite. 2 values "
             "can be passed:\n"
-            "- morphio.IterType.depth_first (default)\n"
-            "- morphio.IterType.breadth_first (default)\n"
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n",
             "iter_type"_a = IterType::DEPTH_FIRST);
 
-    py::class_<morphio::GlialCell, morphio::Morphology>(m, "GlialCell")
-        .def(py::init<const std::string&>())
+    immutable_classes.GlialCell_class.def(py::init<const std::string&>())
         .def(py::init(
                  [](py::object arg) { return std::make_unique<morphio::GlialCell>(py::str(arg)); }),
              "filename"_a,
              "Additional Ctor that accepts as filename any python object that implements __repr__ "
              "or __str__");
 
-    py::class_<morphio::Mitochondria>(
-        m,
-        "Mitochondria",
-        "The entry-point class to access mitochondrial data\n"
-        "By design, it is the equivalent of the Morphology class but at the mitochondrial level\n"
-        "As the Morphology class, it implements a section accessor and a root section accessor\n"
-        "returning views on the Properties object for the queried mitochondrial section")
+    immutable_classes.Mitochondria_class
         .def("section",
              &morphio::Mitochondria::section,
              "Returns the mithochondrial section with the given ID",
              "section_id"_a)
         .def_property_readonly("sections",
                                &morphio::Mitochondria::sections,
                                "Returns a list of all mitochondrial sections")
         .def_property_readonly(
             "root_sections",
             &morphio::Mitochondria::rootSections,
             "Returns a list of all root sections (section whose parent ID is -1)");
 
-    py::class_<morphio::EndoplasmicReticulum>(
-        m,
-        "EndoplasmicReticulum",
-        "The entry-point class to access endoplasmic reticulum data\n"
-        "Spec "
-        "https://bbpteam.epfl.ch/documentation/projects/Morphology%20Documentation/latest/"
-        "h5v1.html")
+    immutable_classes.EndoplasmicReticulum_class
         .def_property_readonly("section_indices",
                                &morphio::EndoplasmicReticulum::sectionIndices,
                                "Returns the list of neuronal section indices")
         .def_property_readonly("volumes",
                                &morphio::EndoplasmicReticulum::volumes,
                                "Returns the list of neuronal section indices")
         .def_property_readonly("surface_areas",
                                &morphio::EndoplasmicReticulum::surfaceAreas,
                                "Returns the surface areas for each neuronal section")
         .def_property_readonly("filament_counts",
                                &morphio::EndoplasmicReticulum::filamentCounts,
                                "Returns the number of filaments for each neuronal section");
 
-
-    py::class_<morphio::Soma>(m, "Soma")
-        .def(py::init<const morphio::Soma&>())
+    immutable_classes.Soma_class.def(py::init<const morphio::Soma&>())
         .def_property_readonly(
             "points",
             [](morphio::Soma* soma) { return span_array_to_ndarray(soma->points()); },
             "Returns the coordinates (x,y,z) of all soma point")
         .def_property_readonly(
             "diameters",
             [](morphio::Soma* soma) { return span_to_ndarray(soma->diameters()); },
@@ -236,15 +257,15 @@
         .def_property_readonly("type", &morphio::Soma::type, "Returns the soma type")
 
         .def_property_readonly("surface",
                                &morphio::Soma::surface,
                                "Returns the soma surface\n\n"
                                "Note: the soma surface computation depends on the soma type");
 
-    py::class_<morphio::Section>(m, "Section")
+    immutable_classes.Section_class
         .def("__str__",
              [](const morphio::Section& section) {
                  std::stringstream ss;
                  ss << section;
                  return ss.str();
              })
 
@@ -315,22 +336,23 @@
                         "upstream are supported");
                 }
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
             "Section iterator\n"
             "\n"
             "iter_type controls the iteration order. 3 values can be passed:\n"
-            "- morphio.IterType.depth_first (default)\n"
-            "- morphio.IterType.breadth_first\n"
-            "- morphio.IterType.upstream\n",
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n"
+            "- ``morphio.IterType.upstream``\n",
             "iter_type"_a = IterType::DEPTH_FIRST);
 
 
-    py::class_<morphio::MitoSection>(m, "MitoSection")
-        // Topology-related member functions
+    // Topology-related member functions
+    immutable_classes.MitoSection_class
         .def_property_readonly("parent",
                                &morphio::MitoSection::parent,
                                "Returns the parent mitochondrial section of this section\n"
                                "throw MissingParentError is the section doesn't have a parent")
         .def_property_readonly("is_root",
                                &morphio::MitoSection::isRoot,
                                "Returns true if this section is a root section (parent ID == -1)")
@@ -389,15 +411,15 @@
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
             "Depth first iterator starting at a given section id\n"
             "\n"
             "If id == -1, the iteration will be successively performed starting\n"
             "at each root section",
             "iter_type"_a = IterType::DEPTH_FIRST);
 
-    py::class_<morphio::DendriticSpine, morphio::Morphology>(m, "DendriticSpine")
+    immutable_classes.DendriticSpine_class
         .def(py::init([](py::object arg) {
                  return std::make_unique<morphio::DendriticSpine>(py::str(arg));
              }),
              "filename"_a)
         .def_property_readonly("root_sections",
                                &morphio::DendriticSpine::rootSections,
                                "Returns a list of all root sections "
@@ -480,17 +502,19 @@
                 default:
                     throw morphio::MorphioError(
                         "Only iteration types depth_first and breadth_first are supported");
                 }
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
             "Section iterator that runs successively on every neurite\n"
+            "\n"
             "iter_type controls the order of iteration on sections of a given neurite. 2 values "
             "can be passed:\n"
-            "- morphio.IterType.depth_first (default)\n"
-            "- morphio.IterType.breadth_first (default)\n",
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n",
             "iter_type"_a = IterType::DEPTH_FIRST)
         .def(
             "write",
             [](morphio::mut::DendriticSpine* morph, py::object arg) { morph->write(py::str(arg)); },
             "filename"_a);
 }
```

### Comparing `MorphIO-3.3.4/binds/python/bind_misc.cpp` & `MorphIO-3.3.5/binds/python/bind_misc.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "bind_misc.h"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
+#include <morphio/collection.h>
 #include <morphio/enums.h>
 #include <morphio/errorMessages.h>
 #include <morphio/types.h>
 #include <morphio/version.h>
 
 #include "../../include/morphio/enums.h"
 #include "bind_enums.h"
@@ -289,8 +290,120 @@
                       "Returns `sectionId` of post-synaptic density")
         .def_readonly("segment_id",
                       &morphio::Property::DendriticSpine::PostSynapticDensity::segmentId,
                       "Returns `segmentId` of post-synaptic density")
         .def_readonly("offset",
                       &morphio::Property::DendriticSpine::PostSynapticDensity::offset,
                       "Returns `offset` of post-synaptic density");
+
+    py::class_<morphio::Collection>(m, "Collection", "A collection of morphologies")
+        .def(py::init<std::string>(), "collection_path"_a)
+        .def(py::init([](py::object arg) { return morphio::Collection(py::str(arg)); }),
+             "collection_path"_a,
+             "Create a collection from a Path-like object.")
+        .def(py::init([](py::object arg, std::vector<std::string> extensions) {
+                 return morphio::Collection(py::str(arg), std::move(extensions));
+             }),
+             "collection_path"_a,
+             "extensions"_a,
+             "Create a collection from a Path-like object.")
+        .def(
+            "load",
+            [](morphio::Collection* collection,
+               const std::string& morph_name,
+               unsigned int options,
+               bool is_mutable) -> py::object {
+                if (is_mutable) {
+                    return py::cast(
+                        collection->load<morphio::mut::Morphology>(morph_name, options));
+                } else {
+                    return py::cast(collection->load<morphio::Morphology>(morph_name, options));
+                }
+            },
+            "morph_name"_a,
+            "options"_a = morphio::enums::Option::NO_MODIFIER,
+            "mutable"_a = false,
+            "Load the morphology named 'morph_name' form the collection.")
+        .def(
+            "load_unordered",
+            [](morphio::Collection* collection,
+               std::vector<std::string> morphology_names,
+               unsigned int options,
+               bool is_mutable) -> py::object {
+                if (is_mutable) {
+                    return py::cast(
+                        collection->load_unordered<morphio::mut::Morphology>(morphology_names,
+                                                                             options));
+                } else {
+                    return py::cast(
+                        collection->load_unordered<morphio::Morphology>(morphology_names, options));
+                }
+            },
+            "morphology_names"_a,
+            "options"_a = morphio::enums::Option::NO_MODIFIER,
+            "mutable"_a = false,
+            R"(Create an iterable of loop index and morphology.
+
+When reading from containers, the order in which morphologies are read can
+have a large impact on the overall time to load those morphologies.
+
+This iterator provides means of reordering loops to optimize the access
+pattern. Loops such as the following
+
+    for k, morph_name in enumerate(morphology_names):
+        morph = collection.load(morphology_names[k])
+        f(k, morph)
+
+can be replaced with
+
+    for k, morph in collection.load_unordered(morphology_names):
+      assert collection.load(morphology_names[k]) == morph
+      f(k, morph)
+
+The order in which the morphologies are returned in unspecified, but the
+loop index `k` can be used to retrieve the correct state corresponding to
+iteration `k` of the original loop.
+
+The iterable returned by `Collection.load_unordered` should only be used while
+`collection` is valid, e.g. within its context or before calling
+`Collection.close`.
+
+Note: This API is 'experimental', meaning it might change in the future.
+)")
+
+        .def("argsort",
+             &morphio::Collection::argsort,
+             "morphology_names"_a,
+             R"(Argsort `morphology_names` by optimal access order.
+
+Note: This API is 'experimental', meaning it might change in the future.
+)")
+        .def("__enter__", [](morphio::Collection* collection) { return collection; })
+        .def("__exit__",
+             [](morphio::Collection* collection,
+                const py::object&,
+                const py::object&,
+                const py::object&) { collection->close(); })
+        .def("close", &morphio::Collection::close);
+
+    py::class_<morphio::LoadUnordered<morphio::Morphology>>(
+        m, "LoadImmutableUnordered", "An iterable of immutable morphologies.")
+        .def(
+            "__iter__",
+            [](const morphio::LoadUnordered<morphio::Morphology>& iterable) {
+                return py::make_iterator(iterable.begin(), iterable.end());
+            },
+            // Bind the lifetime of the `morphio::LoadUnordered` (1) to the
+            // lifetime of the returned iterator (0).
+            py::keep_alive<0, 1>());
+
+    py::class_<morphio::LoadUnordered<morphio::mut::Morphology>>(
+        m, "LoadMutableUnordered", "An iterable of mutable morphologies.")
+        .def(
+            "__iter__",
+            [](const morphio::LoadUnordered<morphio::mut::Morphology>& iterable) {
+                return py::make_iterator(iterable.begin(), iterable.end());
+            },
+            // Bind the lifetime of the `morphio::LoadUnordered` (1) to the
+            // lifetime of the returned iterator (0).
+            py::keep_alive<0, 1>());
 }
```

### Comparing `MorphIO-3.3.4/binds/python/bind_mutable.cpp` & `MorphIO-3.3.5/binds/python/bind_mutable.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include "bind_mutable.h"
 
-#include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
 
 #include <morphio/endoplasmic_reticulum.h>
 #include <morphio/mut/dendritic_spine.h>
 #include <morphio/mut/endoplasmic_reticulum.h>
 #include <morphio/mut/glial_cell.h>
 #include <morphio/mut/mitochondria.h>
 #include <morphio/mut/morphology.h>
@@ -15,31 +15,53 @@
 #include <memory>  // std::make_unique
 
 #include "bind_enums.h"
 #include "bindings_utils.h"
 
 namespace py = pybind11;
 
-void bind_mutable_module(py::module& m) {
+mutable_binding_classes bind_mutable_classes(py::module& m) {
+    using namespace py::literals;
+
+    return mutable_binding_classes{
+        py::class_<morphio::mut::Morphology>(m,
+                                             "Morphology",
+                                             "Class representing a mutable Morphology"),
+        py::class_<morphio::mut::GlialCell, morphio::mut::Morphology>(
+            m, "GlialCell", "Class representing a mutable Glial Cell"),
+        py::class_<morphio::mut::Mitochondria>(m,
+                                               "Mitochondria",
+                                               "Class representing a mutable Mitochondria"),
+        py::class_<morphio::mut::MitoSection, std::shared_ptr<morphio::mut::MitoSection>>(
+            m, "MitoSection", "Class representing a mutable Mitochondrial Section"),
+        py::class_<morphio::mut::Section, std::shared_ptr<morphio::mut::Section>>(
+            m, "Section", "Class representing a mutable Section"),
+        py::class_<morphio::mut::Soma, std::shared_ptr<morphio::mut::Soma>>(
+            m, "Soma", "Class representing a mutable Soma"),
+        py::class_<morphio::mut::EndoplasmicReticulum>(
+            m, "EndoplasmicReticulum", "Class representing a mutable Endoplasmic Reticulum"),
+        py::class_<morphio::mut::DendriticSpine, morphio::mut::Morphology>(
+            m, "DendriticSpine", "Class representing a mutable Dendritic Spine")};
+}
+
+void bind_mutable_methods(mutable_binding_classes& mutable_classes) {
     using namespace py::literals;
 
-    py::class_<morphio::mut::Morphology>(m, "Morphology")
-        .def(py::init<>())
+    mutable_classes.Morphology_mut_class.def(py::init<>())
         .def(py::init<const std::string&, unsigned int>(),
              "filename"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
         .def(py::init<const morphio::Morphology&, unsigned int>(),
              "morphology"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
         .def(py::init<const morphio::mut::Morphology&, unsigned int>(),
              "morphology"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
         .def(py::init([](py::object arg, unsigned int options) {
-                 return std::make_unique<morphio::mut::Morphology>(
-                     py::str(arg), options);
+                 return std::make_unique<morphio::mut::Morphology>(py::str(arg), options);
              }),
              "filename"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER,
              "Additional Ctor that accepts as filename any python "
              "object that implements __repr__ or __str__")
 
         // Cell sub-part accessors
@@ -128,15 +150,15 @@
         .def_property_readonly("soma_type",
                                &morphio::mut::Morphology::somaType,
                                "Returns the soma type")
 
         .def_property_readonly("version", &morphio::mut::Morphology::version, "Returns the version")
 
         .def("remove_unifurcations",
-             static_cast<void (morphio::mut::Morphology::*) ()>(
+             static_cast<void (morphio::mut::Morphology::*)()>(
                  &morphio::mut::Morphology::removeUnifurcations),
              "Fixes the morphology single child sections and issues warnings"
              "if the section starts and ends are inconsistent")
 
         .def(
             "write",
             [](morphio::mut::Morphology* morph, py::object arg) { morph->write(py::str(arg)); },
@@ -151,49 +173,50 @@
                 switch (type) {
                 case IterType::DEPTH_FIRST:
                     return py::make_iterator(morph->depth_begin(), morph->depth_end());
                 case IterType::BREADTH_FIRST:
                     return py::make_iterator(morph->breadth_begin(), morph->breadth_end());
                 case IterType::UPSTREAM:
                 default:
-                    throw morphio::MorphioError("Only iteration types depth_first and "
-                                                "breadth_first are supported");
+                    throw morphio::MorphioError(
+                        "Only iteration types depth_first and "
+                        "breadth_first are supported");
                 }
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive
                                       while iterator exists */
             ,
             "Section iterator that runs successively on every "
             "neurite\n"
+            "\n"
             "iter_type controls the order of iteration on sections of "
             "a given neurite. 2 values can be passed:\n"
-            "- morphio.IterType.depth_first (default)\n"
-            "- morphio.IterType.breadth_first",
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n",
             "iter_type"_a = IterType::DEPTH_FIRST)
         .def("append_root_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (
                  morphio::mut::Morphology::*)(const std::shared_ptr<morphio::mut::Section>&, bool)>(
                  &morphio::mut::Morphology::appendRootSection),
              "Append the existing mutable Section as a root section\n"
              "If recursive == true, all descendent will be appended as well",
              "mutable_section"_a,
              "recursive"_a = false);
 
-    py::class_<morphio::mut::GlialCell, morphio::mut::Morphology>(m, "GlialCell")
-        .def(py::init<>())
+    mutable_classes.GlialCell_mut_class.def(py::init<>())
         .def(py::init([](py::object arg) {
                  return std::make_unique<morphio::mut::GlialCell>(py::str(arg));
              }),
              "filename"_a,
              "Additional Ctor that accepts as filename any python "
              "object that implements __repr__ or __str__");
 
 
-    py::class_<morphio::mut::Mitochondria>(m, "Mitochondria")
-        .def(py::init<>())
+    mutable_classes.Mitochondria_mut_class.def(py::init<>())
         .def_property_readonly("root_sections",
                                &morphio::mut::Mitochondria::rootSections,
                                "Returns a list of all root sections IDs "
                                "(sections whose parent ID are -1)",
                                py::return_value_policy::reference)
         .def_property_readonly("sections",
                                &morphio::mut::Mitochondria::sections,
@@ -275,16 +298,15 @@
             "If id == -1, the iteration will be successively performed starting\n"
             "at each root section",
             "section_id"_a = -1);
 
     using mitosection_floats_f = std::vector<morphio::floatType>& (morphio::mut::MitoSection::*) ();
     using mitosection_ints_f = std::vector<uint32_t>& (morphio::mut::MitoSection::*) ();
 
-    py::class_<morphio::mut::MitoSection, std::shared_ptr<morphio::mut::MitoSection>>(m,
-                                                                                      "MitoSection")
+    mutable_classes.MitoSection_mut_class
         .def_property_readonly("id", &morphio::mut::MitoSection::id, "Return the section ID")
         .def_property(
             "diameters",
             static_cast<mitosection_floats_f>(&morphio::mut::MitoSection::diameters),
             [](morphio::mut::MitoSection* section,
                const std::vector<morphio::floatType>& _diameters) {
                 section->diameters() = _diameters;
@@ -332,15 +354,15 @@
                  const morphio::MitoSection&, bool)>(&morphio::mut::MitoSection::appendSection),
              "Append the existing immutable MitoSection to this section\n"
              "If recursive == true, all descendent will be appended as well",
              "immutable_section"_a,
              "recursive"_a = false);
 
 
-    py::class_<morphio::mut::Section, std::shared_ptr<morphio::mut::Section>>(m, "Section")
+    mutable_classes.Section_mut_class
         .def("__str__",
              [](const morphio::mut::Section& section) {
                  std::stringstream ss;
                  ss << section;
                  return ss.str();
              })
 
@@ -410,25 +432,27 @@
                 case IterType::DEPTH_FIRST:
                     return py::make_iterator(section->depth_begin(), section->depth_end());
                 case IterType::BREADTH_FIRST:
                     return py::make_iterator(section->breadth_begin(), section->breadth_end());
                 case IterType::UPSTREAM:
                     return py::make_iterator(section->upstream_begin(), section->upstream_end());
                 default:
-                    throw morphio::MorphioError("Only iteration types depth_first, breadth_first and "
-                                                "upstream are supported");
+                    throw morphio::MorphioError(
+                        "Only iteration types depth_first, breadth_first and "
+                        "upstream are supported");
                 }
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
             "Section iterator\n"
             "\n"
             "iter_type controls the iteration order. 3 values can be passed:\n"
-            "- morphio.IterType.depth_first (default)\n"
-            "- morphio.IterType.breadth_first\n"
-            "- morphio.IterType.upstream\n",
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n"
+            "- ``morphio.IterType.upstream``\n",
             "iter_type"_a = IterType::DEPTH_FIRST)
 
         // Editing
         .def("append_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::Section::*)(
                  const morphio::Section&, bool)>(&morphio::mut::Section::appendSection),
              "Append the existing immutable Section to this section"
@@ -451,16 +475,15 @@
                  &morphio::mut::Section::appendSection),
              "Append a new Section to this section\n"
              " If section_type is omitted or set to 'undefined'"
              " the type of the parent section will be used",
              "point_level_properties"_a,
              "section_type"_a = morphio::SectionType::SECTION_UNDEFINED);
 
-    py::class_<morphio::mut::Soma, std::shared_ptr<morphio::mut::Soma>>(m, "Soma")
-        .def(py::init<const morphio::Property::PointLevel&>())
+    mutable_classes.Soma_mut_class.def(py::init<const morphio::Property::PointLevel&>())
         .def_property(
             "points",
             [](morphio::mut::Soma* soma) {
                 return py::array(static_cast<py::ssize_t>(soma->points().size()),
                                  soma->points().data());
             },
             [](morphio::mut::Soma* soma, py::array_t<morphio::floatType> _points) {
@@ -487,16 +510,15 @@
                                "Return the maximum distance between the center of gravity "
                                "and any of the soma points")
         .def_property_readonly(
             "center",
             [](morphio::mut::Soma* soma) { return py::array(3, soma->center().data()); },
             "Returns the center of gravity of the soma points");
 
-    py::class_<morphio::mut::EndoplasmicReticulum>(m, "EndoplasmicReticulum")
-        .def(py::init<>())
+    mutable_classes.EndoplasmicReticulum_mut_class.def(py::init<>())
         .def(py::init<const std::vector<uint32_t>&,
                       const std::vector<morphio::floatType>&,
                       const std::vector<morphio::floatType>&,
                       const std::vector<uint32_t>&>())
         .def(py::init<const morphio::EndoplasmicReticulum&>())
         .def(py::init<const morphio::mut::EndoplasmicReticulum&>())
 
@@ -541,16 +563,15 @@
                                  reticulum->filamentCounts().data());
             },
             [](morphio::mut::EndoplasmicReticulum* reticulum, py::array_t<uint32_t> counts) {
                 reticulum->filamentCounts() = counts.cast<std::vector<uint32_t>>();
             },
             "Returns the number of filaments for each neuronal section");
 
-    py::class_<morphio::mut::DendriticSpine, morphio::mut::Morphology>(m, "DendriticSpine")
-        .def(py::init<>())
+    mutable_classes.DendriticSpine_mut_class.def(py::init<>())
         .def(py::init([](py::object arg) {
                  return std::make_unique<morphio::mut::DendriticSpine>(py::str(arg));
              }),
              "filename"_a,
              "Additional Ctor that accepts as filename any python "
              "object that implements __repr__ or __str__")
         .def_property_readonly("sections",
```

### Comparing `MorphIO-3.3.4/binds/python/bind_vasculature.cpp` & `MorphIO-3.3.5/binds/python/bind_vasculature.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 #include "bindings_utils.h"
 
 namespace py = pybind11;
 
 void bind_vasculature(py::module& m) {
     using namespace py::literals;
 
-    py::class_<morphio::vasculature::Vasculature>(m, "Vasculature")
+    py::class_<morphio::vasculature::Vasculature>(m,
+                                                  "Vasculature",
+                                                  "Class representing a Vasculature")
         .def(py::init<const std::string&>(), "filename"_a)
         .def(py::init([](py::object arg) {
                  return std::make_unique<morphio::vasculature::Vasculature>(py::str(arg));
              }),
              "filename"_a,
              "Additional Ctor that accepts as filename any python object that implements __repr__ "
              "or __str__")
@@ -32,15 +34,14 @@
 
         .def("section",
              &morphio::vasculature::Vasculature::section,
              "Returns the Section with the given id\n"
              "throw RawDataError if the id is out of range",
              "section_id"_a)
 
-
         .def_property_readonly(
             "section_offsets",
             [](morphio::vasculature::Vasculature& vasculature) {
                 return as_pyarray(vasculature.sectionOffsets());
             },
             "Returns a list with offsets to access data of a specific section in the points\n"
             "and diameters arrays.\n"
@@ -94,15 +95,17 @@
             [](morphio::vasculature::Vasculature* morpho) {
                 return py::make_iterator(morpho->begin(), morpho->end());
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
             "Iterate on all sections of the graph");
 
 
-    py::class_<morphio::vasculature::Section>(m, "Section")
+    py::class_<morphio::vasculature::Section>(m,
+                                              "Section",
+                                              "Class representing a mutable Vasculature Section")
         .def("__str__",
              [](const morphio::vasculature::Section& section) {
                  std::stringstream ss;
                  ss << section;
                  return ss.str();
              })
```

### Comparing `MorphIO-3.3.4/binds/python/bindings_utils.cpp` & `MorphIO-3.3.5/binds/python/bindings_utils.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/CMakeLists.txt` & `MorphIO-3.3.5/binds/python/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/LICENSE` & `MorphIO-3.3.5/binds/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/attr.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/buffer_info.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/cast.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/chrono.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/complex.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/class.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/common.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/descr.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/init.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/internals.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/type_caster_base.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/detail/typeid.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/eigen.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/embed.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/eval.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/functional.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/gil.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/iostream.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/numpy.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/operators.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/options.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/pybind11.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/pytypes.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl/filesystem.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/include/pybind11/stl_bind.h` & `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/tools/FindCatch.cmake` & `MorphIO-3.3.5/binds/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/tools/FindEigen3.cmake` & `MorphIO-3.3.5/binds/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/tools/FindPythonLibsNew.cmake` & `MorphIO-3.3.5/binds/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/tools/pybind11Common.cmake` & `MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/tools/pybind11NewTools.cmake` & `MorphIO-3.3.5/binds/python/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/binds/python/pybind11/tools/pybind11Tools.cmake` & `MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/dendritic_spine.h` & `MorphIO-3.3.5/include/morphio/dendritic_spine.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/endoplasmic_reticulum.h` & `MorphIO-3.3.5/include/morphio/endoplasmic_reticulum.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/enums.h` & `MorphIO-3.3.5/include/morphio/enums.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/errorMessages.h` & `MorphIO-3.3.5/include/morphio/errorMessages.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/exceptions.h` & `MorphIO-3.3.5/include/morphio/exceptions.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mito_section.h` & `MorphIO-3.3.5/include/morphio/mito_section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mitochondria.h` & `MorphIO-3.3.5/include/morphio/mitochondria.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/morphology.h` & `MorphIO-3.3.5/include/morphio/morphology.h`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  * release of resources upon destruction.
  */
 class Morphology
 {
   public:
     virtual ~Morphology() = default;
 
-    Morphology(Morphology&) noexcept = default;
+    Morphology(const Morphology&) noexcept = default;
     Morphology& operator=(const Morphology&) noexcept = default;
     Morphology(Morphology&&) noexcept = default;
     Morphology& operator=(Morphology&&) noexcept = default;
 
     /** @name Read API */
 
     /** Open the given source to a morphology file and parse it.
```

### Comparing `MorphIO-3.3.4/include/morphio/mut/dendritic_spine.h` & `MorphIO-3.3.5/include/morphio/mut/dendritic_spine.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mut/endoplasmic_reticulum.h` & `MorphIO-3.3.5/include/morphio/mut/endoplasmic_reticulum.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mut/mito_section.h` & `MorphIO-3.3.5/include/morphio/mut/mito_section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mut/mitochondria.h` & `MorphIO-3.3.5/include/morphio/mut/mitochondria.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mut/modifiers.h` & `MorphIO-3.3.5/include/morphio/mut/modifiers.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mut/morphology.h` & `MorphIO-3.3.5/include/morphio/mut/morphology.h`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,18 @@
     their enum: morphio::enum::Option and can be composed.
 
        Example:
            Morphology("neuron.asc", TWO_POINTS_SECTIONS | SOMA_SPHERE);
     **/
     explicit Morphology(const std::string& uri, unsigned int options = NO_MODIFIER);
 
-    /// Build a mutable Morphology from a mutable morphology aaaaaa
+    /// Build a mutable Morphology from an HighFive::Group
+    explicit Morphology(const HighFive::Group& group, unsigned int options = NO_MODIFIER);
+
+    /// Build a mutable Morphology from a mutable morphology
     Morphology(const morphio::mut::Morphology& morphology, unsigned int options = NO_MODIFIER);
 
     /// Build a mutable Morphology from a read-only morphology
     explicit Morphology(const morphio::Morphology& morphology, unsigned int options = NO_MODIFIER);
 
     virtual ~Morphology();
```

### Comparing `MorphIO-3.3.4/include/morphio/mut/section.h` & `MorphIO-3.3.5/include/morphio/mut/section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/mut/soma.h` & `MorphIO-3.3.5/include/morphio/mut/soma.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/properties.h` & `MorphIO-3.3.5/include/morphio/properties.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/section.h` & `MorphIO-3.3.5/include/morphio/section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/section_base.h` & `MorphIO-3.3.5/include/morphio/section_base.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/section_iterators.hpp` & `MorphIO-3.3.5/include/morphio/section_iterators.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/soma.h` & `MorphIO-3.3.5/include/morphio/soma.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/tools.h` & `MorphIO-3.3.5/include/morphio/tools.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/types.h` & `MorphIO-3.3.5/include/morphio/types.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/vasc/iterators.hpp` & `MorphIO-3.3.5/include/morphio/vasc/iterators.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/vasc/properties.h` & `MorphIO-3.3.5/include/morphio/vasc/properties.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/vasc/section.h` & `MorphIO-3.3.5/include/morphio/vasc/section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/vasc/vasculature.h` & `MorphIO-3.3.5/include/morphio/vasc/vasculature.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/include/morphio/vector_types.h` & `MorphIO-3.3.5/include/morphio/vector_types.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/morphio/__init__.py` & `MorphIO-3.3.5/morphio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 from ._morphio import (
     Annotation,
     AnnotationType,
     CellFamily,
     CellLevel,
+    Collection,
     DendriticSpine,
     EndoplasmicReticulum,
     GlialCell,
     IDSequenceError,
     IterType,
     LogLevel,
     MissingParentError,
```

### Comparing `MorphIO-3.3.4/setup.py` & `MorphIO-3.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/CMakeLists.txt` & `MorphIO-3.3.5/src/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 set(MORPHIO_SOURCES
+    collection.cpp
     dendritic_spine.cpp
     endoplasmic_reticulum.cpp
     enums.cpp
     errorMessages.cpp
     glial_cell.cpp
     mito_section.cpp
     mitochondria.cpp
@@ -21,14 +22,15 @@
     point_utils.cpp
     properties.cpp
     readers/morphologyASC.cpp
     readers/morphologyHDF5.cpp
     readers/morphologySWC.cpp
     readers/vasculatureHDF5.cpp
     section.cpp
+    shared_utils.cpp
     soma.cpp
     vasc/properties.cpp
     vasc/section.cpp
     vasc/vasculature.cpp
     version.cpp
     )
 
@@ -61,14 +63,16 @@
 
 target_include_directories(morphio_obj
   SYSTEM
   PUBLIC
    $<TARGET_PROPERTY:gsl-lite,INTERFACE_INCLUDE_DIRECTORIES>
    $<TARGET_PROPERTY:HighFive,INTERFACE_INCLUDE_DIRECTORIES>
    $<TARGET_PROPERTY:lexertl,INTERFACE_INCLUDE_DIRECTORIES>
+  PRIVATE
+   $<TARGET_PROPERTY:ghc_filesystem,INTERFACE_INCLUDE_DIRECTORIES>
   )
 
 set_target_properties(morphio_obj
   PROPERTIES
   CXX_STANDARD 14
   CXX_STANDARD_REQUIRED YES
   CXX_EXTENSIONS NO
```

### Comparing `MorphIO-3.3.4/src/dendritic_spine.cpp` & `MorphIO-3.3.5/src/dendritic_spine.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/endoplasmic_reticulum.cpp` & `MorphIO-3.3.5/src/endoplasmic_reticulum.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/enums.cpp` & `MorphIO-3.3.5/src/enums.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/errorMessages.cpp` & `MorphIO-3.3.5/src/errorMessages.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mito_section.cpp` & `MorphIO-3.3.5/src/mito_section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mitochondria.cpp` & `MorphIO-3.3.5/src/mitochondria.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/morphology.cpp` & `MorphIO-3.3.5/src/morphology.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/dendritic_spine.cpp` & `MorphIO-3.3.5/src/mut/dendritic_spine.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/endoplasmic_reticulum.cpp` & `MorphIO-3.3.5/src/mut/endoplasmic_reticulum.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/mito_section.cpp` & `MorphIO-3.3.5/src/mut/mito_section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/mitochondria.cpp` & `MorphIO-3.3.5/src/mut/mitochondria.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/modifiers.cpp` & `MorphIO-3.3.5/src/mut/modifiers.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/morphology.cpp` & `MorphIO-3.3.5/src/mut/morphology.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 namespace morphio {
 namespace mut {
 
 using morphio::readers::ErrorMessages;
 Morphology::Morphology(const std::string& uri, unsigned int options)
     : Morphology(morphio::Morphology(uri, options)) {}
 
+Morphology::Morphology(const HighFive::Group& group, unsigned int options)
+    : Morphology(morphio::Morphology(group, options)) {}
+
 Morphology::Morphology(const morphio::mut::Morphology& morphology, unsigned int options)
     : _soma(std::make_shared<Soma>(*morphology.soma()))
     , _cellProperties(std::make_shared<morphio::Property::CellLevel>(*morphology._cellProperties))
     , _endoplasmicReticulum(morphology.endoplasmicReticulum())
     , _dendriticSpineLevel(morphology._dendriticSpineLevel) {
     for (const std::shared_ptr<Section>& root : morphology.rootSections()) {
         appendRootSection(root, true);
```

### Comparing `MorphIO-3.3.4/src/mut/section.cpp` & `MorphIO-3.3.5/src/mut/section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/soma.cpp` & `MorphIO-3.3.5/src/mut/soma.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/mut/writers.cpp` & `MorphIO-3.3.5/src/mut/writers.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/point_utils.cpp` & `MorphIO-3.3.5/src/point_utils.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/point_utils.h` & `MorphIO-3.3.5/src/point_utils.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/properties.cpp` & `MorphIO-3.3.5/src/properties.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/readers/NeurolucidaLexer.inc` & `MorphIO-3.3.5/src/readers/NeurolucidaLexer.inc`

 * *Files 2% similar despite different names*

```diff
@@ -104,96 +104,102 @@
 }
 
 constexpr std::size_t operator+(Token type) {
     return static_cast<std::size_t>(type);
 }
 
 namespace {
-const lexertl::state_machine& build_lexer() {
-    static lexertl::state_machine sm;
-    if (!sm.empty()) {
-        return sm;
-    }
+class StateMachineBuilder 
+{
+public:
+    static lexertl::state_machine build() {
+        lexertl::rules rules_;
+        rules_.push("\n", +Token::NEWLINE);
+        rules_.push("[ \t\r]+", +Token::WS);
+        rules_.push(";[^\n]*", +Token::COMMENT);
+
+        rules_.push("\\(", +Token::LPAREN);
+        rules_.push("\\)", +Token::RPAREN);
+
+        rules_.push("<[ \t\r]*\\(", +Token::LSPINE);
+        rules_.push("\\)>", +Token::RSPINE);
+
+        rules_.push(",", +Token::COMMA);
+        rules_.push("\\|", +Token::PIPE);
+
+        rules_.push("Color", +Token::COLOR);
+        rules_.push("Font", +Token::FONT);
+
+        rules_.push("[Aa]xon", +Token::AXON);
+        rules_.push("[Aa]pical", +Token::APICAL);
+        rules_.push("[Dd]endrite", +Token::DENDRITE);
+        rules_.push("[Cc]ell ?[Bb]ody", +Token::CELLBODY);
+
+        // The code snippet used to infer the marker list is available at:
+        // https://github.com/BlueBrain/MorphIO/pull/229
+        rules_.push("Dot[0-9]*", +Token::MARKER);
+        rules_.push("Plus[0-9]*", +Token::MARKER);
+        rules_.push("Cross[0-9]*", +Token::MARKER);
+        rules_.push("Splat[0-9]*", +Token::MARKER);
+        rules_.push("Flower[0-9]*", +Token::MARKER);
+        rules_.push("Circle[0-9]*", +Token::MARKER);
+        rules_.push("Flower[0-9]*", +Token::MARKER);
+        rules_.push("TriStar[0-9]*", +Token::MARKER);
+        rules_.push("OpenStar[0-9]*", +Token::MARKER);
+        rules_.push("Asterisk[0-9]*", +Token::MARKER);
+        rules_.push("SnowFlake[0-9]*", +Token::MARKER);
+        rules_.push("OpenCircle[0-9]*", +Token::MARKER);
+        rules_.push("ShadedStar[0-9]*", +Token::MARKER);
+        rules_.push("FilledStar[0-9]*", +Token::MARKER);
+        rules_.push("TexacoStar[0-9]*", +Token::MARKER);
+        rules_.push("MoneyGreen[0-9]*", +Token::MARKER);
+        rules_.push("DarkYellow[0-9]*", +Token::MARKER);
+        rules_.push("OpenSquare[0-9]*", +Token::MARKER);
+        rules_.push("OpenDiamond[0-9]*", +Token::MARKER);
+        rules_.push("CircleArrow[0-9]*", +Token::MARKER);
+        rules_.push("CircleCross[0-9]*", +Token::MARKER);
+        rules_.push("OpenQuadStar[0-9]*", +Token::MARKER);
+        rules_.push("DoubleCircle[0-9]*", +Token::MARKER);
+        rules_.push("FilledSquare[0-9]*", +Token::MARKER);
+        rules_.push("MalteseCross[0-9]*", +Token::MARKER);
+        rules_.push("FilledCircle[0-9]*", +Token::MARKER);
+        rules_.push("FilledDiamond[0-9]*", +Token::MARKER);
+        rules_.push("FilledQuadStar[0-9]*", +Token::MARKER);
+        rules_.push("OpenUpTriangle[0-9]*", +Token::MARKER);
+        rules_.push("FilledUpTriangle[0-9]*", +Token::MARKER);
+        rules_.push("OpenDownTriangle[0-9]*", +Token::MARKER);
+        rules_.push("FilledDownTriangle[0-9]*", +Token::MARKER);
+
+        rules_.push("Generated", +Token::GENERATED);
+        rules_.push("High", +Token::HIGH);
+        rules_.push("Incomplete", +Token::INCOMPLETE);
+        rules_.push("Low", +Token::LOW);
+        rules_.push("Normal", +Token::NORMAL);
+        rules_.push("Midpoint", +Token::MIDPOINT);
+        rules_.push("Origin", +Token::ORIGIN);
+
+        rules_.push(R"(\"[^"]*\")", +Token::STRING);
+
+        rules_.push(R"([+-]?[0-9]+(\.[0-9]+)?([eE][+-]?[0-9]+)?)", +Token::NUMBER);
+        rules_.push("[a-zA-Z][0-9a-zA-Z]+", +Token::WORD);
 
-    lexertl::rules rules_;
-    rules_.push("\n", +Token::NEWLINE);
-    rules_.push("[ \t\r]+", +Token::WS);
-    rules_.push(";[^\n]*", +Token::COMMENT);
-
-    rules_.push("\\(", +Token::LPAREN);
-    rules_.push("\\)", +Token::RPAREN);
-
-    rules_.push("<[ \t\r]*\\(", +Token::LSPINE);
-    rules_.push("\\)>", +Token::RSPINE);
-
-    rules_.push(",", +Token::COMMA);
-    rules_.push("\\|", +Token::PIPE);
-
-    rules_.push("Color", +Token::COLOR);
-    rules_.push("Font", +Token::FONT);
-
-    rules_.push("[Aa]xon", +Token::AXON);
-    rules_.push("[Aa]pical", +Token::APICAL);
-    rules_.push("[Dd]endrite", +Token::DENDRITE);
-    rules_.push("[Cc]ell ?[Bb]ody", +Token::CELLBODY);
-
-    // The code snippet used to infer the marker list is available at:
-    // https://github.com/BlueBrain/MorphIO/pull/229
-    rules_.push("Dot[0-9]*", +Token::MARKER);
-    rules_.push("Plus[0-9]*", +Token::MARKER);
-    rules_.push("Cross[0-9]*", +Token::MARKER);
-    rules_.push("Splat[0-9]*", +Token::MARKER);
-    rules_.push("Flower[0-9]*", +Token::MARKER);
-    rules_.push("Circle[0-9]*", +Token::MARKER);
-    rules_.push("Flower[0-9]*", +Token::MARKER);
-    rules_.push("TriStar[0-9]*", +Token::MARKER);
-    rules_.push("OpenStar[0-9]*", +Token::MARKER);
-    rules_.push("Asterisk[0-9]*", +Token::MARKER);
-    rules_.push("SnowFlake[0-9]*", +Token::MARKER);
-    rules_.push("OpenCircle[0-9]*", +Token::MARKER);
-    rules_.push("ShadedStar[0-9]*", +Token::MARKER);
-    rules_.push("FilledStar[0-9]*", +Token::MARKER);
-    rules_.push("TexacoStar[0-9]*", +Token::MARKER);
-    rules_.push("MoneyGreen[0-9]*", +Token::MARKER);
-    rules_.push("DarkYellow[0-9]*", +Token::MARKER);
-    rules_.push("OpenSquare[0-9]*", +Token::MARKER);
-    rules_.push("OpenDiamond[0-9]*", +Token::MARKER);
-    rules_.push("CircleArrow[0-9]*", +Token::MARKER);
-    rules_.push("CircleCross[0-9]*", +Token::MARKER);
-    rules_.push("OpenQuadStar[0-9]*", +Token::MARKER);
-    rules_.push("DoubleCircle[0-9]*", +Token::MARKER);
-    rules_.push("FilledSquare[0-9]*", +Token::MARKER);
-    rules_.push("MalteseCross[0-9]*", +Token::MARKER);
-    rules_.push("FilledCircle[0-9]*", +Token::MARKER);
-    rules_.push("FilledDiamond[0-9]*", +Token::MARKER);
-    rules_.push("FilledQuadStar[0-9]*", +Token::MARKER);
-    rules_.push("OpenUpTriangle[0-9]*", +Token::MARKER);
-    rules_.push("FilledUpTriangle[0-9]*", +Token::MARKER);
-    rules_.push("OpenDownTriangle[0-9]*", +Token::MARKER);
-    rules_.push("FilledDownTriangle[0-9]*", +Token::MARKER);
-
-    rules_.push("Generated", +Token::GENERATED);
-    rules_.push("High", +Token::HIGH);
-    rules_.push("Incomplete", +Token::INCOMPLETE);
-    rules_.push("Low", +Token::LOW);
-    rules_.push("Normal", +Token::NORMAL);
-    rules_.push("Midpoint", +Token::MIDPOINT);
-    rules_.push("Origin", +Token::ORIGIN);
-
-    rules_.push(R"(\"[^"]*\")", +Token::STRING);
+        lexertl::state_machine sm;
 
-    rules_.push(R"([+-]?[0-9]+(\.[0-9]+)?([eE][+-]?[0-9]+)?)", +Token::NUMBER);
-    rules_.push("[a-zA-Z][0-9a-zA-Z]+", +Token::WORD);
+        lexertl::generator::build(rules_, sm);
+        sm.minimise();
 
-    lexertl::generator::build(rules_, sm);
-    sm.minimise();
+        // useful to debug
+        // lexertl::debug::dump(sm, std::cout);
 
-    // useful to debug
-    // lexertl::debug::dump(sm, std::cout);
+        return sm;
+    }
+};
 
+const lexertl::state_machine& lexer_singleton() {
+    static lexertl::state_machine sm = StateMachineBuilder::build();
     return sm;
 }
 
 }  // namespace
 
 
 class NeurolucidaLexer
@@ -210,15 +216,15 @@
 
   public:
     explicit NeurolucidaLexer(const std::string& path, bool debug = false)
         : debug_(debug)
         , err_(path) {}
 
     void start_parse(const std::string& input) {
-        const auto& sm = build_lexer();
+        const auto& sm = lexer_singleton();
         current_ = next_ = lexertl::siterator(input.begin(), input.end(), sm);
 
         // will set the above, current_ to next_, AND consume whitespace
         size_t n_skipped = skip_whitespace(current_);
         current_line_num_ += n_skipped;
         next_line_num_ += n_skipped;
```

### Comparing `MorphIO-3.3.4/src/readers/morphologyASC.cpp` & `MorphIO-3.3.5/src/readers/morphologyASC.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/readers/morphologyHDF5.cpp` & `MorphIO-3.3.5/src/readers/morphologyHDF5.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -80,24 +80,26 @@
 
 MorphologyHDF5::MorphologyHDF5(const HighFive::Group& group)
     : _group(group)
     , _uri("HDF5 Group") {}
 
 Property::Properties load(const std::string& uri) {
     try {
+        std::lock_guard<std::recursive_mutex> lock(morphio::readers::h5::global_hdf5_mutex());
         HighFive::SilenceHDF5 silence;
         auto file = HighFive::File(uri, HighFive::File::ReadOnly);
         return MorphologyHDF5(file.getGroup("/")).load();
 
     } catch (const HighFive::FileException& exc) {
         throw RawDataError("Could not open morphology file " + uri + ": " + exc.what());
     }
 }
 
 Property::Properties load(const HighFive::Group& group) {
+    std::lock_guard<std::recursive_mutex> lock(morphio::readers::h5::global_hdf5_mutex());
     return MorphologyHDF5(group).load();
 }
 
 Property::Properties MorphologyHDF5::load() {
     _readMetadata(_uri);
 
     int firstSectionOffset = _readSections();
@@ -287,48 +289,49 @@
         types.emplace_back(type);
     }
 
     return firstSectionOffset;
 }
 
 void MorphologyHDF5::_readPerimeters(int firstSectionOffset) {
-    assert(_properties._cellLevel.majorVersion() == 1 &&
-           _properties._cellLevel.minorVersion() > 0 &&
-           "Perimeter information is available starting at v1.1");
+    if (!(_properties._cellLevel.majorVersion() == 1 &&
+          _properties._cellLevel.minorVersion() > 0)) {
+        throw RawDataError("Perimeter information is available starting at v1.1");
+    }
 
     // soma only, won't have perimeters
     if (firstSectionOffset == SOMA_ONLY) {
         return;
     }
 
     if (!_group.exist(_d_perimeters)) {
         if (_properties._cellLevel._cellFamily == GLIA) {
             throw RawDataError("No empty perimeters allowed for glia morphology");
         }
         return;
     }
 
     auto& perimeters = _properties.get_mut<Property::Perimeter>();
-    _read("/", _d_perimeters, 1, perimeters);
+    _read("", _d_perimeters, 1, perimeters);
     perimeters.erase(perimeters.begin(), perimeters.begin() + firstSectionOffset);
 }
 
 
 template <typename T>
 void MorphologyHDF5::_read(const std::string& groupName,
                            const std::string& datasetName,
                            unsigned int expectedDimension,
                            T& data) {
-    if (!_group.exist(groupName)) {
+    if (groupName != "" && !_group.exist(groupName)) {
         throw(
             RawDataError("Reading morphology '" + _uri + "': Missing required group " + groupName));
     }
-    const auto group = _group.getGroup(groupName);
+    const auto group = groupName == "" ? _group : _group.getGroup(groupName);
 
-    if (!_group.exist(groupName)) {
+    if (!group.exist(datasetName)) {
         throw(RawDataError("Reading morphology '" + _uri + "': Missing required dataset " +
                            datasetName));
     }
     const HighFive::DataSet dataset = group.getDataSet(datasetName);
 
     const auto dims = dataset.getSpace().getDimensions();
     if (dims.size() != expectedDimension) {
```

### Comparing `MorphIO-3.3.4/src/readers/morphologyHDF5.h` & `MorphIO-3.3.5/src/readers/morphologyHDF5.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #pragma once
+#include <mutex>
 #include <string>  // std::string
 
 #include <morphio/properties.h>
 
 #include <highfive/H5File.hpp>
 
 namespace morphio {
@@ -34,10 +35,16 @@
                unsigned int expectedDimension,
                T& data);
 
     HighFive::Group _group;
     Property::Properties _properties;
     std::string _uri;
 };
+
+inline std::recursive_mutex& global_hdf5_mutex() {
+    static std::recursive_mutex _mutex;
+    return _mutex;
+}
+
 }  // namespace h5
 }  // namespace readers
 }  // namespace morphio
```

### Comparing `MorphIO-3.3.4/src/readers/morphologySWC.cpp` & `MorphIO-3.3.5/src/readers/morphologySWC.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/readers/vasculatureHDF5.cpp` & `MorphIO-3.3.5/src/readers/vasculatureHDF5.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/readers/vasculatureHDF5.h` & `MorphIO-3.3.5/src/readers/vasculatureHDF5.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/section.cpp` & `MorphIO-3.3.5/src/section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/shared_utils.hpp` & `MorphIO-3.3.5/src/shared_utils.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -64,8 +64,31 @@
     if (data.empty())
         return {};
 
     return {data.begin() + static_cast<long int>(range.first),
             data.begin() + static_cast<long int>(range.second)};
 }
 
+/**
+ * Is `path` a directory?
+ *
+ * Symlinks to directories are considered directories.
+ */
+bool is_directory(const std::string& path);
+
+/**
+ * Is `path` a regular file?
+ *
+ * Symlinks to regular files are considered files.
+ */
+bool is_regular_file(const std::string& path);
+
+/**
+ * Join `dirname` and `filename` into one path.
+ *
+ * This follows the Python `os.path.join` semantics, i.e.,
+ *   - join_path("", "foo") == "foo" (not "/foo")
+ *   - join_path("/usr", "/home/foo") == "/home/foo" (not "/usr/home/foo")
+ */
+std::string join_path(const std::string& dirname, const std::string& filename);
+
 }  // namespace morphio
```

### Comparing `MorphIO-3.3.4/src/soma.cpp` & `MorphIO-3.3.5/src/soma.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/vasc/properties.cpp` & `MorphIO-3.3.5/src/vasc/properties.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/vasc/section.cpp` & `MorphIO-3.3.5/src/vasc/section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.4/src/vasc/vasculature.cpp` & `MorphIO-3.3.5/src/vasc/vasculature.cpp`

 * *Files identical despite different names*

