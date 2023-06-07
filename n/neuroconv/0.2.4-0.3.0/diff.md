# Comparing `tmp/neuroconv-0.2.4.tar.gz` & `tmp/neuroconv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroconv-0.2.4.tar", last modified: Tue Feb  7 17:54:38 2023, max compression
+gzip compressed data, was "neuroconv-0.3.0.tar", last modified: Wed Jun  7 21:30:12 2023, max compression
```

## Comparing `neuroconv-0.2.4.tar` & `neuroconv-0.3.0.tar`

### file list

```diff
@@ -1,199 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-07 17:54:33.000000 neuroconv-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-07 17:54:33.000000 neuroconv-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-02-07 17:54:38.427961 neuroconv-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-02-07 17:54:33.000000 neuroconv-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-07 17:54:33.000000 neuroconv-0.2.4/base_gin_test_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-07 17:54:33.000000 neuroconv-0.2.4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-07 17:54:33.000000 neuroconv-0.2.4/make_environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-07 17:54:33.000000 neuroconv-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 17:54:38.427961 neuroconv-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-07 17:54:33.000000 neuroconv-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.407961 neuroconv-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.411961 neuroconv-0.2.4/src/neuroconv/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/basedatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/baseextractorinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.411961 neuroconv-0.2.4/src/neuroconv/datainterfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.411961 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.411961 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/audio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/sleap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/sleap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/video/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/video/video_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/video/videodatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/alphaomega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/alphaomega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/baserecordingextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/basesortingextractorinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/biocam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/biocam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/blackrock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/blackrock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/ced/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/ced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/ced/ceddatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/cellexplorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/cellexplorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/edf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/edf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/intan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/intan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/kilosort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.415961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mcsraw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mcsraw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mearec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mearec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuralynx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuralynx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuroscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuroscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/openephys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/openephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/phy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/phy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/plexon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/plexon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikegadgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikegadgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeglx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeglx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeinterface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeinterface/sipickledatainterfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/tdt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/tdt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/abf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/abf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/caiman/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/caiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.419961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/cnmfe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/cnmfe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/cnmfe/cnmfedatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sbx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/scanimage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/scanimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sima/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/suite2p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/tiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/tiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/csv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/csv/csvtimeintertervalsinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/excel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/datainterfaces/text/timeintervalsinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/nwbconverter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/schemas/metadata_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/schemas/source_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/schemas/yaml_conversion_specification_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.423961 neuroconv-0.2.4/src/neuroconv/tools/audio/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/audio/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/data_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/figshare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/hdmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/src/neuroconv/tools/neo/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/neo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/neo/neo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/nwb_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/src/neuroconv/tools/roiextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/roiextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43822 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/roiextractors/roiextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/signal_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/src/neuroconv/tools/spikeinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/spikeinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83162 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/spikeinterface/spikeinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/src/neuroconv/tools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/testing/mock_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/testing/mock_ttl_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/src/neuroconv/tools/yaml_conversion_specification/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/yaml_conversion_specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.427961 neuroconv-0.2.4/src/neuroconv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/utils/globbing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-07 17:54:33.000000 neuroconv-0.2.4/src/neuroconv/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:54:38.411961 neuroconv-0.2.4/src/neuroconv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-02-07 17:54:38.000000 neuroconv-0.2.4/src/neuroconv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-02-07 17:54:38.000000 neuroconv-0.2.4/src/neuroconv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 17:54:38.000000 neuroconv-0.2.4/src/neuroconv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-07 17:54:38.000000 neuroconv-0.2.4/src/neuroconv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-02-07 17:54:38.000000 neuroconv-0.2.4/src/neuroconv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-07 17:54:38.000000 neuroconv-0.2.4/src/neuroconv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.865862 neuroconv-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 21:30:07.000000 neuroconv-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-07 21:30:12.865862 neuroconv-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-07 21:30:07.000000 neuroconv-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 21:30:07.000000 neuroconv-0.3.0/base_gin_test_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-07 21:30:07.000000 neuroconv-0.3.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-07 21:30:07.000000 neuroconv-0.3.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 21:30:07.000000 neuroconv-0.3.0/make_environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-07 21:30:07.000000 neuroconv-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:30:12.865862 neuroconv-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-07 21:30:07.000000 neuroconv-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.845861 neuroconv-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/basedatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/baseextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/basetemporalalignmentinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/sleap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/sleap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/video/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/video/video_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/video/videodatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/alphaomega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/alphaomega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/baserecordingextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/basesortingextractorinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/biocam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/biocam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/blackrock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/blackrock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/edf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/edf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/intan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/intan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/maxwell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/maxwell/maxonedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mcsraw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mcsraw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mearec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mearec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuralynx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuralynx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuroscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/openephys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/openephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/openephys/openephysbinarydatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/openephys/openephyslegacydatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/openephys/openephyssortingdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/phy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/phy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/plexon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/plexon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spike2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spike2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spike2/spike2datainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/tdt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/tdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/abf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/abf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/brukertiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/brukertiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/brukertiff/brukertiffdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/caiman/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/caiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/cnmfe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/cnmfe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/cnmfe/cnmfedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.853861 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/micromanagertiffdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sbx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/scanimage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/scanimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sima/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/tiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/tiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/csv/csvtimeintertervalsinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/excel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/datainterfaces/text/timeintervalsinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/nwbconverter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.857862 neuroconv-0.3.0/src/neuroconv/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/schemas/base_metadata_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/schemas/metadata_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/schemas/source_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/schemas/time_series_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/schemas/yaml_conversion_specification_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.861862 neuroconv-0.3.0/src/neuroconv/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.861862 neuroconv-0.3.0/src/neuroconv/tools/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/audio/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/data_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/figshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/hdmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.861862 neuroconv-0.3.0/src/neuroconv/tools/neo/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/neo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/neo/neo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/nwb_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/path_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.861862 neuroconv-0.3.0/src/neuroconv/tools/roiextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/roiextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45824 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/roiextractors/roiextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/signal_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.861862 neuroconv-0.3.0/src/neuroconv/tools/spikeinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/spikeinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67405 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/spikeinterface/spikeinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.861862 neuroconv-0.3.0/src/neuroconv/tools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/testing/_path_expander_demo_ibl_filepaths.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32069 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/testing/data_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/testing/mock_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/testing/mock_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/testing/mock_ttl_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.865862 neuroconv-0.3.0/src/neuroconv/tools/yaml_conversion_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/yaml_conversion_specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.865862 neuroconv-0.3.0/src/neuroconv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 21:30:07.000000 neuroconv-0.3.0/src/neuroconv/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:30:12.849861 neuroconv-0.3.0/src/neuroconv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-07 21:30:12.000000 neuroconv-0.3.0/src/neuroconv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-07 21:30:12.000000 neuroconv-0.3.0/src/neuroconv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:30:12.000000 neuroconv-0.3.0/src/neuroconv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 21:30:12.000000 neuroconv-0.3.0/src/neuroconv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-07 21:30:12.000000 neuroconv-0.3.0/src/neuroconv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 21:30:12.000000 neuroconv-0.3.0/src/neuroconv.egg-info/top_level.txt
```

### Comparing `neuroconv-0.2.4/LICENSE` & `neuroconv-0.3.0/license.txt`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/setup.py` & `neuroconv-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from setuptools import setup, find_packages
+from collections import defaultdict
 from pathlib import Path
 from shutil import copy
-from collections import defaultdict
+
+from setuptools import find_packages, setup
 
 root = Path(__file__).parent
 
 with open(root / "README.md") as f:
     long_description = f.read()
 with open(root / "requirements-minimal.txt") as f:
     install_requires = f.readlines()
@@ -20,14 +21,16 @@
     modality_path = root / "src" / "neuroconv" / "datainterfaces" / modality
     modality_requirement_file = modality_path / "requirements.txt"
     if modality_requirement_file.exists():
         with open(modality_requirement_file) as f:
             modality_requirements = f.readlines()
             extras_require["full"].extend(modality_requirements)
             extras_require[modality].extend(modality_requirements)
+    else:
+        modality_requirements = list()
 
     format_subpaths = [path for path in modality_path.iterdir() if path.is_dir() and path.name != "__pycache__"]
     for format_subpath in format_subpaths:
         format_requirement_file = format_subpath / "requirements.txt"
         extras_require[format_subpath.name].extend(modality_requirements)
         if format_requirement_file.exists():
             with open(format_requirement_file) as f:
@@ -40,26 +43,27 @@
 gin_config_file_base = Path("./base_gin_test_config.json")
 gin_config_file_local = Path("./tests/test_on_data/gin_test_config.json")
 if not gin_config_file_local.exists():
     copy(src=gin_config_file_base, dst=gin_config_file_local)
 
 setup(
     name="neuroconv",
-    version="0.2.4",
+    version="0.3.0",
     description="Convert data from proprietary formats to NWB format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Cody Baker, Szonja Weigl, Heberto Mayorquin, Luiz Tauffer, and Ben Dichter.",
     author_email="ben.dichter@catalystneuro.com",
     url="https://github.com/catalystneuro/neuroconv",
     keywords="nwb",
+    license_files=("license.txt",),
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,  # Includes files described in MANIFEST.in in the installation.
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require=extras_require,
     entry_points={
         "console_scripts": [
             "neuroconv = neuroconv.tools.yaml_conversion_specification.yaml_conversion_specification:run_conversion_from_yaml_cli",
         ],
     },
```

### Comparing `neuroconv-0.2.4/src/neuroconv/basedatainterface.py` & `neuroconv-0.3.0/src/neuroconv/basedatainterface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,67 @@
-"""Authors: Cody Baker and Ben Dichter."""
-from abc import abstractmethod, ABC
 import uuid
-from typing import Optional
+from abc import ABC, abstractmethod
+from pathlib import Path
+from typing import List, Optional
 
 from pynwb import NWBFile
 
-from .utils import get_base_schema, get_schema_from_method_signature
+from .utils import get_schema_from_method_signature, load_dict_from_file
+from .utils.dict import DeepDict
 
 
 class BaseDataInterface(ABC):
     """Abstract class defining the structure of all DataInterfaces."""
 
+    keywords: List[str] = []
+
     @classmethod
     def get_source_schema(cls):
         """Infer the JSON schema for the source_data from the method signature (annotation typing)."""
-        return get_schema_from_method_signature(cls.__init__, exclude=["source_data"])
-
-    @classmethod
-    def get_conversion_options_schema(cls):
-        """Infer the JSON schema for the conversion options from the method signature (annotation typing)."""
-        return get_schema_from_method_signature(cls.run_conversion, exclude=["nwbfile", "metadata"])
+        return get_schema_from_method_signature(cls, exclude=["source_data"])
 
     def __init__(self, **source_data):
         self.source_data = source_data
 
+    def get_conversion_options_schema(self):
+        """Infer the JSON schema for the conversion options from the method signature (annotation typing)."""
+        return get_schema_from_method_signature(self.run_conversion, exclude=["nwbfile", "metadata"])
+
     def get_metadata_schema(self):
         """Retrieve JSON schema for metadata."""
-        metadata_schema = get_base_schema(
-            id_="metadata.schema.json",
-            root=True,
-            title="Metadata",
-            description="Schema for the metadata",
-            version="0.1.0",
-        )
+        metadata_schema = load_dict_from_file(Path(__file__).parent / "schemas" / "base_metadata_schema.json")
         return metadata_schema
 
     def get_metadata(self):
         """Child DataInterface classes should override this to match their metadata."""
-        metadata = dict(
-            NWBFile=dict(
-                session_description="Auto-generated by neuroconv",
-                identifier=str(uuid.uuid4()),
-            ),
-        )
+        metadata = DeepDict()
+        metadata["NWBFile"]["session_description"] = "Auto-generated by neuroconv"
+        metadata["NWBFile"]["identifier"] = str(uuid.uuid4())
 
         return metadata
 
-    def get_conversion_options(self):
-        """Child DataInterface classes should override this to match their conversion options."""
-        return dict()
-
     @abstractmethod
     def run_conversion(
         self,
         nwbfile_path: Optional[str] = None,
         nwbfile: Optional[NWBFile] = None,
         metadata: Optional[dict] = None,
         overwrite: bool = False,
         **conversion_options,
     ):
         """
         Run the NWB conversion for the instantiated data interface.
 
         Parameters
         ----------
-        nwbfile_path: FilePathType
+        nwbfile_path : FilePathType
             Path for where to write or load (if overwrite=False) the NWBFile.
             If specified, the context will always write to this location.
-        nwbfile: NWBFile, optional
+        nwbfile : NWBFile, optional
             An in-memory NWBFile object to write to the location.
-        metadata: dict, optional
+        metadata : dict, optional
             Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
-        overwrite: bool, optional
-            Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
+        overwrite : bool, default: False
+            Whether to overwrite the NWBFile if one exists at the nwbfile_path.
             The default is False (append mode).
-        verbose: bool, optional
-            If 'nwbfile_path' is specified, informs user after a successful write operation.
-            The default is True.
         """
-
         raise NotImplementedError("The run_conversion method for this DataInterface has not been defined!")
```

### Comparing `neuroconv-0.2.4/src/neuroconv/baseextractorinterface.py` & `neuroconv-0.3.0/src/neuroconv/baseextractorinterface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 """Abstract class defining the structure of all Extractor-based Interfaces."""
+from abc import ABC
 from typing import Optional
 
-from .basedatainterface import BaseDataInterface
+from .basetemporalalignmentinterface import BaseTemporalAlignmentInterface
 from .tools import get_package
 
 
-class _LazyExtractorImport(type(BaseDataInterface), type):
-    def __getattribute__(self, name):
-        if name == "Extractor" and super().__getattribute__("Extractor") is None:
-            extractor_module = get_package(package_name=super().__getattribute__("ExtractorModuleName"))
-            extractor = getattr(
-                extractor_module,
-                super().__getattribute__("ExtractorName") or self.__name__.replace("Interface", "Extractor"),
-            )
-            return extractor
-        return super().__getattribute__(name)
-
-
-class BaseExtractorInterface(BaseDataInterface, metaclass=_LazyExtractorImport):
+class BaseExtractorInterface(BaseTemporalAlignmentInterface, ABC):
     """
     Abstract class defining the structure of all Extractor-based Interfaces.
-
-    Harnesses an override of the class-level __getattribute__ to perform on-demand imports of the extractor class.
-    Since the type of every class is itself a 'type' (a builtin object), direct overrides are not possible.
-    Hence we use a metaclass whose parent is 'type' to act as an intermediary with the builtin.
-    This metaclass also requires a mix-in with the parent ABC class since the ABCMeta causes conflicts otherwise.
-
-    However, the __getattribute__ override is only a 'getter' with respect to the property; setting it in instances
-    of the class is performed by a slight injection into the __new__ of the base class.
     """
 
     # Manually override any of these attributes in a subclass if needed.
     # Note that values set at the level of class definition are called upon import.
     ExtractorModuleName: Optional[str] = None
     ExtractorName: Optional[str] = None  # Defaults to __name__.replace("Interface", "Extractor").
-    Extractor = None  # Loads dynamically on first access attempt
+    Extractor = None  # Class loads dynamically on first call to .get_extractor()
 
-    def __new__(cls, *args, **kwargs):
-        cls.Extractor = getattr(cls, "Extractor")
-        return object.__new__(cls)
+    @classmethod
+    def get_extractor(cls):
+        if cls.Extractor is not None:
+            return cls.Extractor
+        extractor_module = get_package(package_name=cls.ExtractorModuleName)
+        extractor = getattr(
+            extractor_module,
+            cls.ExtractorName or cls.__name__.replace("Interface", "Extractor"),
+        )
+        cls.Extractor = extractor
+        return extractor
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/__init__.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,175 @@
+# Behavior
+from .behavior.audio.audiointerface import AudioInterface
+from .behavior.deeplabcut.deeplabcutdatainterface import DeepLabCutInterface
+from .behavior.sleap.sleapdatainterface import SLEAPInterface
+from .behavior.video.videodatainterface import VideoInterface
+
 # Ecephys
-from .ecephys.neuroscope.neuroscopedatainterface import (
-    NeuroScopeRecordingInterface,
-    NeuroScopeLFPInterface,
-    NeuroScopeMultiRecordingTimeInterface,
-    NeuroScopeSortingInterface,
-)
-from .ecephys.spikeglx.spikeglxdatainterface import SpikeGLXRecordingInterface, SpikeGLXLFPInterface
-from .ecephys.spikeglx.spikeglxnidqinterface import SpikeGLXNIDQInterface
-from .ecephys.spikegadgets.spikegadgetsdatainterface import SpikeGadgetsRecordingInterface
-from .ecephys.spikeinterface.sipickledatainterfaces import (
-    SIPickleRecordingInterface,
-    SIPickleSortingInterface,
+from .ecephys.alphaomega.alphaomegadatainterface import AlphaOmegaRecordingInterface
+from .ecephys.axona.axonadatainterface import (
+    AxonaLFPDataInterface,
+    AxonaPositionDataInterface,
+    AxonaRecordingInterface,
+    AxonaUnitRecordingInterface,
 )
-from .ecephys.intan.intandatainterface import IntanRecordingInterface
-from .ecephys.ced.ceddatainterface import CEDRecordingInterface
-from .ecephys.cellexplorer.cellexplorerdatainterface import CellExplorerSortingInterface
+from .ecephys.biocam.biocamdatainterface import BiocamRecordingInterface
 from .ecephys.blackrock.blackrockdatainterface import (
     BlackrockRecordingInterface,
     BlackrockSortingInterface,
 )
-from .ecephys.openephys.openephysdatainterface import (
-    OpenEphysRecordingInterface,
-    OpenEphysSortingInterface,
+from .ecephys.cellexplorer.cellexplorerdatainterface import CellExplorerSortingInterface
+from .ecephys.edf.edfdatainterface import EDFRecordingInterface
+from .ecephys.intan.intandatainterface import IntanRecordingInterface
+from .ecephys.kilosort.kilosortdatainterface import KiloSortSortingInterface
+from .ecephys.maxwell.maxonedatainterface import MaxOneRecordingInterface
+from .ecephys.mcsraw.mcsrawdatainterface import MCSRawRecordingInterface
+from .ecephys.mearec.mearecdatainterface import MEArecRecordingInterface
+from .ecephys.neuralynx.neuralynxdatainterface import (
+    NeuralynxRecordingInterface,
+    NeuralynxSortingInterface,
 )
-from .ecephys.axona.axonadatainterface import (
-    AxonaRecordingInterface,
-    AxonaPositionDataInterface,
-    AxonaLFPDataInterface,
-    AxonaUnitRecordingInterface,
+from .ecephys.neuroscope.neuroscopedatainterface import (
+    NeuroScopeLFPInterface,
+    NeuroScopeRecordingInterface,
+    NeuroScopeSortingInterface,
+)
+from .ecephys.openephys.openephysbinarydatainterface import (
+    OpenEphysBinaryRecordingInterface,
+)
+from .ecephys.openephys.openephysdatainterface import OpenEphysRecordingInterface
+from .ecephys.openephys.openephyslegacydatainterface import (
+    OpenEphysLegacyRecordingInterface,
 )
-from .ecephys.neuralynx.neuralynxdatainterface import NeuralynxRecordingInterface, NeuralynxSortingInterface
+from .ecephys.openephys.openephyssortingdatainterface import OpenEphysSortingInterface
 from .ecephys.phy.phydatainterface import PhySortingInterface
-from .ecephys.kilosort.kilosortdatainterface import KiloSortSortingInterface
-from .ecephys.edf.edfdatainterface import EDFRecordingInterface
+from .ecephys.plexon.plexondatainterface import (
+    PlexonRecordingInterface,
+    PlexonSortingInterface,
+)
+from .ecephys.spike2.spike2datainterface import (
+    CEDRecordingInterface,
+    Spike2RecordingInterface,
+)
+from .ecephys.spikegadgets.spikegadgetsdatainterface import (
+    SpikeGadgetsRecordingInterface,
+)
+from .ecephys.spikeglx.spikeglxdatainterface import (
+    SpikeGLXLFPInterface,
+    SpikeGLXRecordingInterface,
+)
+from .ecephys.spikeglx.spikeglxnidqinterface import SpikeGLXNIDQInterface
 from .ecephys.tdt.tdtdatainterface import TdtRecordingInterface
-from .ecephys.plexon.plexondatainterface import PlexonRecordingInterface
-from .ecephys.biocam.biocamdatainterface import BiocamRecordingInterface
-from .ecephys.alphaomega.alphaomegadatainterface import AlphaOmegaRecordingInterface
-from .ecephys.mearec.mearecdatainterface import MEArecRecordingInterface
-from .ecephys.mcsraw.mcsrawdatainterface import MCSRawRecordingInterface
 
 # Icephys
 from .icephys.abf.abfdatainterface import AbfInterface
 
-
 # Ophys
+from .ophys.brukertiff.brukertiffdatainterface import BrukerTiffImagingInterface
 from .ophys.caiman.caimandatainterface import CaimanSegmentationInterface
 from .ophys.cnmfe.cnmfedatainterface import CnmfeSegmentationInterface
-from .ophys.suite2p.suite2pdatainterface import Suite2pSegmentationInterface
 from .ophys.extract.extractdatainterface import ExtractSegmentationInterface
-from .ophys.sima.simadatainterface import SimaSegmentationInterface
-
-from .ophys.sbx.sbxdatainterface import SbxImagingInterface
-from .ophys.tiff.tiffdatainterface import TiffImagingInterface
 from .ophys.hdf5.hdf5datainterface import Hdf5ImagingInterface
+from .ophys.micromanagertiff.micromanagertiffdatainterface import (
+    MicroManagerTiffImagingInterface,
+)
+from .ophys.sbx.sbxdatainterface import SbxImagingInterface
 from .ophys.scanimage.scanimageimaginginterface import ScanImageImagingInterface
-
-
-# Behavior
-from .behavior.video.videodatainterface import VideoInterface, MovieInterface
-from .behavior.deeplabcut.deeplabcutdatainterface import DeepLabCutInterface
-from .behavior.sleap.sleapdatainterface import SLEAPInterface
+from .ophys.sima.simadatainterface import SimaSegmentationInterface
+from .ophys.suite2p.suite2pdatainterface import Suite2pSegmentationInterface
+from .ophys.tiff.tiffdatainterface import TiffImagingInterface
 
 # Text
 from .text.csv.csvtimeintertervalsinterface import CsvTimeIntervalsInterface
 from .text.excel.exceltimeintervalsinterface import ExcelTimeIntervalsInterface
 
 interface_list = [
     # Ecephys
     NeuralynxRecordingInterface,
     NeuralynxSortingInterface,
     NeuroScopeRecordingInterface,
-    NeuroScopeMultiRecordingTimeInterface,
     NeuroScopeSortingInterface,
     NeuroScopeLFPInterface,
+    Spike2RecordingInterface,
     SpikeGLXRecordingInterface,
     SpikeGLXLFPInterface,
     SpikeGLXNIDQInterface,
     SpikeGadgetsRecordingInterface,
-    SIPickleRecordingInterface,
-    SIPickleSortingInterface,
     IntanRecordingInterface,
     CEDRecordingInterface,
     CellExplorerSortingInterface,
     BlackrockRecordingInterface,
     BlackrockSortingInterface,
     OpenEphysRecordingInterface,
+    OpenEphysBinaryRecordingInterface,
+    OpenEphysLegacyRecordingInterface,
     OpenEphysSortingInterface,
     PhySortingInterface,
     KiloSortSortingInterface,
     AxonaRecordingInterface,
     AxonaPositionDataInterface,
     AxonaLFPDataInterface,
     AxonaUnitRecordingInterface,
     EDFRecordingInterface,
     TdtRecordingInterface,
     PlexonRecordingInterface,
+    PlexonSortingInterface,
     BiocamRecordingInterface,
     AlphaOmegaRecordingInterface,
     MEArecRecordingInterface,
     MCSRawRecordingInterface,
+    MaxOneRecordingInterface,
     # Icephys
     AbfInterface,
     # Ophys
     CaimanSegmentationInterface,
     CnmfeSegmentationInterface,
     Suite2pSegmentationInterface,
     ExtractSegmentationInterface,
     SimaSegmentationInterface,
     SbxImagingInterface,
     TiffImagingInterface,
     Hdf5ImagingInterface,
     ScanImageImagingInterface,
+    BrukerTiffImagingInterface,
+    MicroManagerTiffImagingInterface,
     # Behavior
-    MovieInterface,  # TO-DO: deprecate on April 2023
     VideoInterface,
+    AudioInterface,
     DeepLabCutInterface,
     SLEAPInterface,
     # Text
     CsvTimeIntervalsInterface,
     ExcelTimeIntervalsInterface,
 ]
+
+interfaces_by_category = dict(
+    ecephys={
+        interface.__name__.replace("RecordingInterface", ""): interface  # TODO: use removesuffix when 3.8 is dropped
+        for interface in interface_list
+        if "Recording" in interface.__name__
+    },
+    sorting={
+        interface.__name__.replace("SortingInterface", ""): interface
+        for interface in interface_list
+        if "Sorting" in interface.__name__
+    },
+    imaging={
+        interface.__name__.replace("ImagingInterface", ""): interface
+        for interface in interface_list
+        if "Imaging" in interface.__name__
+    },
+    segmentation={
+        interface.__name__.replace("SegmentationInterface", ""): interface
+        for interface in interface_list
+        if "Segmentation" in interface.__name__
+    },
+    icephys=dict(Abf=AbfInterface),
+    behavior=dict(
+        Video=VideoInterface,
+        DeepLabCut=DeepLabCutInterface,
+        SLEAP=SLEAPInterface,
+        # Text
+        CsvTimeIntervals=CsvTimeIntervalsInterface,
+        ExcelTimeIntervals=ExcelTimeIntervalsInterface,
+    ),
+)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py` & `neuroconv-0.3.0/src/neuroconv/tools/nwb_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,188 +1,186 @@
+import uuid
+from contextlib import contextmanager
+from datetime import datetime
 from pathlib import Path
 from typing import Optional
 from warnings import warn
 
-from scipy.io.wavfile import read
+from pynwb import NWBHDF5IO, NWBFile
+from pynwb.file import Subject
 
-from neuroconv.basedatainterface import BaseDataInterface
-from neuroconv.datainterfaces.behavior.video.videodatainterface import _check_duplicates
-from neuroconv.tools.audio import add_acoustic_waveform_series
-from neuroconv.tools.nwb_helpers import (
-    make_or_load_nwbfile,
-)
-from neuroconv.utils import (
-    get_schema_from_hdmf_class,
-    get_base_schema,
-    FilePathType,
-)
-from pynwb import NWBFile, TimeSeries
-
-
-def _check_file_paths(file_paths, metadata: dict):
-    number_of_file_paths = len(file_paths)
-    assert len(metadata) == number_of_file_paths, (
-        f"Incomplete metadata, the number of metadata for Audio is ({len(metadata)}) "
-        f"is not equal to the number of expected metadata ({number_of_file_paths})."
-    )
+from ..utils import FilePathType, dict_deep_update
+from ..utils.dict import DeepDict
 
 
-def _check_audio_names_are_unique(metadata: dict):
-    neurodata_names = [neurodata["name"] for neurodata in metadata]
-    neurodata_names_are_unique = len(set(neurodata_names)) == len(neurodata_names)
-    assert neurodata_names_are_unique, f"Some of the names for Audio metadata are not unique."
-
-
-def _check_starting_times(starting_times: list, metadata: dict) -> list:
-    if starting_times is not None:
-        assert isinstance(starting_times, list) and all(
-            [isinstance(x, float) for x in starting_times]
-        ), "Argument 'starting_times' must be a list of floats."
-
-    if len(metadata) == 1 and starting_times is None:
-        warn("starting_times not provided, setting to 0.0")
-        starting_times = [0.0]
-
-    assert len(starting_times) == len(metadata), (
-        f"The number of entries in 'starting_times' ({len(starting_times)}) must be equal to number of unique "
-        f"AcousticWaveformSeries ({len(metadata)}). \n"
-        f"'starting_times' provided as input {starting_times}."
+def get_module(nwbfile: NWBFile, name: str, description: str = None):
+    """Check if processing module exists. If not, create it. Then return module."""
+    if name in nwbfile.processing:
+        if description is not None and nwbfile.processing[name].description != description:
+            warn(
+                "Custom description given to get_module does not match existing module description! "
+                "Ignoring custom description."
+            )
+        return nwbfile.processing[name]
+    else:
+        if description is None:
+            description = "No description."
+        return nwbfile.create_processing_module(name=name, description=description)
+
+
+def get_default_nwbfile_metadata() -> DeepDict:
+    """
+    Return structure with defaulted metadata values required for a NWBFile.
+
+    These standard defaults are
+        metadata["NWBFile"]["session_description"] = "no description"
+        metadata["NWBFile"]["identifier"] = str(uuid.uuid4())
+    Proper conversions should override these fields prior to calling NWBConverter.run_conversion()
+    """
+    metadata = DeepDict()
+    metadata["NWBFile"].deep_update(
+        session_description="no description",
+        identifier=str(uuid.uuid4()),
     )
-    return starting_times
 
+    return metadata
 
-class AudioInterface(BaseDataInterface):
-    """Data interface for writing acoustic recordings to an NWB file."""
 
-    def __init__(self, file_paths: list, verbose: bool = False):
-        """
-        Create the interface for writing acoustic recordings as AcousticWaveformSeries.
-
-        Parameters
-        ----------
-        file_paths : list of FilePathTypes
-            The file paths to the audio recordings in sorted, consecutive order.
-            We recommend using `natsort` to ensure the files are in consecutive order.
-            from natsort import natsorted
-            natsorted(file_paths)
-        verbose : bool, default: False
-        """
-        suffixes = [suffix for file_path in file_paths for suffix in Path(file_path).suffixes]
-        format_is_not_supported = [
-            suffix for suffix in suffixes if suffix not in [".wav"]
-        ]  # TODO: add support for more formats
-        if format_is_not_supported:
-            raise ValueError(
-                "The currently supported file format for audio is WAV file. "
-                f"Some of the provided files does not match this format: {format_is_not_supported}."
-            )
-        self.verbose = verbose
-        super().__init__(file_paths=file_paths)
+def make_nwbfile_from_metadata(metadata: dict):
+    """Make NWBFile from available metadata."""
+    metadata = dict_deep_update(get_default_nwbfile_metadata(), metadata)
+    nwbfile_kwargs = metadata["NWBFile"]
+    if "Subject" in metadata:
+        # convert ISO 8601 string to datetime
+        if "date_of_birth" in metadata["Subject"] and isinstance(metadata["Subject"]["date_of_birth"], str):
+            metadata["Subject"]["date_of_birth"] = datetime.fromisoformat(metadata["Subject"]["date_of_birth"])
+        nwbfile_kwargs.update(subject=Subject(**metadata["Subject"]))
+    # convert ISO 8601 string to datetime
+    assert "session_start_time" in nwbfile_kwargs, (
+        "'session_start_time' was not found in metadata['NWBFile']! Please add the correct start time of the "
+        "session in ISO8601 format (%Y-%m-%dT%H:%M:%S) to this key of the metadata."
+    )
+    if isinstance(nwbfile_kwargs.get("session_start_time", None), str):
+        nwbfile_kwargs["session_start_time"] = datetime.fromisoformat(metadata["NWBFile"]["session_start_time"])
+    return NWBFile(**nwbfile_kwargs)
+
+
+def add_device_from_metadata(nwbfile: NWBFile, modality: str = "Ecephys", metadata: dict = None):
+    """
+    Add device information from metadata to NWBFile object.
+
+    Will always ensure nwbfile has at least one device, but multiple
+    devices within the metadata list will also be created.
+
+    Parameters
+    ----------
+    nwbfile: NWBFile
+        nwb file to which the new device information is to be added
+    modality: str
+        Type of data recorded by device. Options:
+        - Ecephys (default)
+        - Icephys
+        - Ophys
+        - Behavior
+    metadata: dict
+        Metadata info for constructing the NWBFile (optional).
+        Should be of the format
+            metadata[modality]['Device'] = [
+                {
+                    'name': my_name,
+                    'description': my_description
+                },
+                ...
+            ]
+        Missing keys in an element of metadata['Ecephys']['Device'] will be auto-populated with defaults.
+    """
+    assert isinstance(nwbfile, NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
+    assert modality in [
+        "Ecephys",
+        "Icephys",
+        "Ophys",
+        "Behavior",
+    ], f"Invalid modality {modality} when creating device."
+
+    defaults = dict(name=f"Device{modality}", description=f"{modality} device. Automatically generated.")
+
+    if metadata is None:
+        metadata = dict()
+    if modality not in metadata:
+        metadata[modality] = dict()
+    if "Device" not in metadata[modality]:
+        metadata[modality]["Device"] = [defaults]
+
+    for dev in metadata[modality]["Device"]:
+        if dev.get("name", defaults["name"]) not in nwbfile.devices:
+            nwbfile.create_device(**dict(defaults, **dev))
+
+
+@contextmanager
+def make_or_load_nwbfile(
+    nwbfile_path: Optional[FilePathType] = None,
+    nwbfile: Optional[NWBFile] = None,
+    metadata: Optional[dict] = None,
+    overwrite: bool = False,
+    verbose: bool = True,
+):
+    """
+    Context for automatically handling decision of write vs. append for writing an NWBFile.
+
+    Parameters
+    ----------
+    nwbfile_path: FilePathType
+        Path for where to write or load (if overwrite=False) the NWBFile.
+        If specified, the context will always write to this location.
+    nwbfile: NWBFile, optional
+        An in-memory NWBFile object to write to the location.
+    metadata: dict, optional
+        Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
+    overwrite: bool, optional
+        Whether to overwrite the NWBFile if one exists at the nwbfile_path.
+        The default is False (append mode).
+    verbose: bool, optional
+        If 'nwbfile_path' is specified, informs user after a successful write operation.
+        The default is True.
+    """
+    nwbfile_path_in = Path(nwbfile_path) if nwbfile_path else None
+    assert not (nwbfile_path is None and nwbfile is None and metadata is None), (
+        "You must specify either an 'nwbfile_path', or an in-memory 'nwbfile' object, "
+        "or provide the metadata for creating one."
+    )
+    assert not (overwrite is False and nwbfile_path_in and nwbfile_path_in.exists() and nwbfile is not None), (
+        "'nwbfile_path' exists at location, 'overwrite' is False (append mode), but an in-memory 'nwbfile' object was "
+        "passed! Cannot reconcile which nwbfile object to write."
+    )
 
-    def get_metadata_schema(self):
-        metadata_schema = super().get_metadata_schema()
-        time_series_metadata_schema = get_schema_from_hdmf_class(TimeSeries)
-        metadata_schema["properties"]["Behavior"] = get_base_schema(tag="Behavior")
-        time_series_metadata_schema.update(required=["name"])
-        metadata_schema["properties"]["Behavior"].update(
-            required=["Audio"],
-            properties=dict(
-                Audio=dict(
-                    type="array",
-                    minItems=1,
-                    items=time_series_metadata_schema,
-                )
-            ),
-        )
-        return metadata_schema
-
-    def get_metadata(self) -> dict:
-        default_name = "AcousticWaveformSeries"
-        is_multiple_file_path = len(self.source_data["file_paths"]) > 1
-        audio_metadata = [
-            dict(
-                name=default_name + str(file_ind) if is_multiple_file_path and file_ind > 0 else default_name,
-                description="Acoustic waveform series.",
-            )
-            for file_ind, file_path in enumerate(self.source_data["file_paths"])
-        ]
-        behavior_metadata = dict(Audio=audio_metadata)
-
-        metadata = super().get_metadata()
-        metadata.update(Behavior=behavior_metadata)
-        return metadata
-
-    def run_conversion(
-        self,
-        nwbfile_path: Optional[FilePathType] = None,
-        nwbfile: Optional[NWBFile] = None,
-        metadata: Optional[dict] = None,
-        stub_test: bool = False,
-        stub_frames: int = 1000,
-        write_as: str = "stimulus",
-        starting_times: Optional[list] = None,
-        iterator_options: Optional[dict] = None,
-        compression_options: Optional[dict] = None,
-        overwrite: bool = False,
-        verbose: bool = True,
-    ):
-        """
-
-        Parameters
-        ----------
-        nwbfile_path : FilePathType, optional
-            If a file exists at this path, append to it. If not, write the file here.
-        nwbfile : NWBFile, optional
-            Append to this NWBFile object
-        metadata : dict, optional
-        stub_test : bool, default: False
-        stub_frames : int, default: 1000
-        write_as : {'stimulus', 'acquisition'}
-            The acoustic waveform series can be added to the NWB file either as
-            "stimulus" or as "acquisition".
-        starting_times : list, optional
-            Starting time for each AcousticWaveformSeries
-        iterator_options : dict, optional
-            Dictionary of options for the SliceableDataChunkIterator.
-        compression_options : dict, optional
-            Dictionary of options for compressing the data for H5DataIO.
-        overwrite : bool, default: False
-        verbose : bool, default: True
-
-        Returns
-        -------
-        NWBFile
-
-        """
-        file_paths = self.source_data["file_paths"]
-        audio_metadata = metadata["Behavior"]["Audio"]
-        # Checks for metadata
-        _check_file_paths(file_paths=file_paths, metadata=audio_metadata)
-        _check_audio_names_are_unique(metadata=audio_metadata)
-
-        audio_metadata_unique, file_paths_unique = _check_duplicates(audio_metadata, file_paths)
-        unpacked_file_paths_unique = [file_path[0] for file_path in file_paths_unique]
-
-        starting_times = _check_starting_times(starting_times=starting_times, metadata=audio_metadata_unique)
-
-        with make_or_load_nwbfile(
-            nwbfile_path=nwbfile_path, nwbfile=nwbfile, metadata=metadata, overwrite=overwrite, verbose=self.verbose
-        ) as nwbfile_out:
-            for file_ind, (acoustic_waveform_series_metadata, file_path) in enumerate(
-                zip(audio_metadata_unique, unpacked_file_paths_unique)
-            ):
-                sampling_rate, acoustic_series = read(filename=file_path, mmap=True)
-                if stub_test:
-                    acoustic_series = acoustic_series[:stub_frames]
-
-                add_acoustic_waveform_series(
-                    acoustic_series=acoustic_series,
-                    nwbfile=nwbfile_out,
-                    rate=sampling_rate,
-                    metadata=acoustic_waveform_series_metadata,
-                    write_as=write_as,
-                    starting_time=starting_times[file_ind],
-                    iterator_options=iterator_options,
-                    compression_options=compression_options,
-                )
+    load_kwargs = dict()
+    success = True
+    file_initially_exists = nwbfile_path_in.is_file() if nwbfile_path_in is not None else None
+    if nwbfile_path_in:
+        load_kwargs.update(path=nwbfile_path_in)
+        if file_initially_exists and not overwrite:
+            load_kwargs.update(mode="r+", load_namespaces=True)
+        else:
+            load_kwargs.update(mode="w")
+        io = NWBHDF5IO(**load_kwargs)
+    try:
+        if load_kwargs.get("mode", "") == "r+":
+            nwbfile = io.read()
+        elif nwbfile is None:
+            nwbfile = make_nwbfile_from_metadata(metadata=metadata)
+        yield nwbfile
+    except Exception as e:
+        success = False
+        raise e
+    finally:
+        if nwbfile_path_in:
+            try:
+                if success:
+                    io.write(nwbfile)
+
+                    if verbose:
+                        print(f"NWB file saved at {nwbfile_path_in}!")
+            finally:
+                io.close()
 
-        return nwbfile_out
+                if not success and not file_initially_exists:
+                    nwbfile_path_in.unlink()
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,70 @@
-"""Author: Heberto Mayorquin."""
-from typing import Optional
 from pathlib import Path
+from typing import Optional
 
+import numpy as np
 from pynwb.file import NWBFile
 
-from ....basedatainterface import BaseDataInterface
-from ....tools.nwb_helpers import make_or_load_nwbfile
-from ....tools import get_package
-from ....utils import dict_deep_update, FilePathType, OptionalFilePathType
-
 from .sleap_utils import extract_timestamps
+from ....basetemporalalignmentinterface import BaseTemporalAlignmentInterface
+from ....tools import get_package
+from ....tools.nwb_helpers import make_or_load_nwbfile
+from ....utils import FilePathType, dict_deep_update
 
 
-class SLEAPInterface(BaseDataInterface):
+class SLEAPInterface(BaseTemporalAlignmentInterface):
     """Data interface for SLEAP datasets."""
 
     def __init__(
         self,
         file_path: FilePathType,
-        video_file_path: OptionalFilePathType = None,
+        video_file_path: Optional[FilePathType] = None,
         verbose: bool = True,
         frames_per_second: Optional[float] = None,
     ):
         """
         Interface for writing sleap .slp files to nwb using the sleap-io library.
 
         Parameters
         ----------
-        file_path: FilePathType
+        file_path : FilePathType
             Path to the .slp file (the output of sleap)
-        verbose: Bool
+        verbose : bool, default: True
             controls verbosity. ``True`` by default.
-        video_file_path: OptionalFilePathType
-            The file path of the video for extracting timestamps
-        frames_per_second: float
-            The frames per second (fps) or sampling rate of the video
+        video_file_path : FilePath, optional
+            The file path of the video for extracting timestamps.
+        frames_per_second : float, optional
+            The frames per second (fps) or sampling rate of the video.
         """
-
         self.file_path = Path(file_path)
         self.sleap_io = get_package(package_name="sleap_io")
         self.video_file_path = video_file_path
         self.video_sample_rate = frames_per_second
         self.verbose = verbose
+        self._timestamps = None
         super().__init__(file_path=file_path)
 
+    def get_original_timestamps(self) -> np.ndarray:
+        if self.video_file_path is None:
+            raise ValueError(
+                "Unable to fetch the original timestamps from the video! "
+                "Please specify 'video_file_path' when initializing the interface."
+            )
+        return np.array(extract_timestamps(self.video_file_path))
+
+    def get_timestamps(self) -> np.ndarray:
+        timestamps = self._timestamps if self._timestamps is not None else self.get_original_timestamps()
+        return timestamps
+
+    def set_aligned_timestamps(self, aligned_timestamps: np.ndarray):
+        self._timestamps = aligned_timestamps
+
     def run_conversion(
         self,
-        nwbfile_path: OptionalFilePathType = None,
+        nwbfile_path: Optional[FilePathType] = None,
         nwbfile: Optional[NWBFile] = None,
         metadata: Optional[dict] = None,
         overwrite: bool = False,
     ):
         """
         Conversion from DLC output files to nwb. Derived from sleap-io library.
 
@@ -60,23 +74,22 @@
             Path for where to write or load (if overwrite=False) the NWBFile.
             If specified, this context will always write to this location.
         nwbfile: NWBFile
             nwb file to which the recording information is to be added
         metadata: dict
             metadata info for constructing the nwb file (optional).
         overwrite: bool, optional
-            Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
+            Whether to overwrite the NWBFile if one exists at the nwbfile_path.
         """
-
         base_metadata = self.get_metadata()
         metadata = dict_deep_update(base_metadata, metadata)
 
         pose_estimation_metadata = dict()
-        if self.video_file_path:
-            video_timestamps = extract_timestamps(self.video_file_path)
+        if self.video_file_path or self._timestamps:
+            video_timestamps = self.get_timestamps()
             pose_estimation_metadata.update(video_timestamps=video_timestamps)
 
         if self.video_sample_rate:
             pose_estimation_metadata.update(video_sample_rate=self.video_sample_rate)
 
         with make_or_load_nwbfile(
             nwbfile_path=nwbfile_path, nwbfile=nwbfile, metadata=metadata, overwrite=overwrite, verbose=self.verbose
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/behavior/video/video_utils.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/behavior/video/video_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""Authors: Saksham Sharda, Cody Baker."""
-from typing import Tuple, Iterable, Optional
+from typing import Iterable, Optional, Tuple
 
 import numpy as np
-from tqdm import tqdm
 from hdmf.data_utils import GenericDataChunkIterator
+from tqdm import tqdm
 
 from ....tools import get_package
 from ....utils import FilePathType
 
 
 def get_video_timestamps(file_path: FilePathType, max_frames: Optional[int] = None) -> list:
     """Extract the timestamps of the video located in file_path
@@ -31,25 +30,25 @@
     return timestamps
 
 
 class VideoCaptureContext:
     """Retrieving video metadata and frames using a context manager."""
 
     def __init__(self, file_path: FilePathType):
-        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python")
+        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python-headless")
 
         self.vc = cv2.VideoCapture(filename=file_path)
         self.file_path = file_path
         self._current_frame = 0
         self._frame_count = None
         self._video_open_msg = "The video file is not open!"
 
     def get_video_timestamps(self, max_frames=None):
         """Return numpy array of the timestamps(s) for a video file."""
-        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python")
+        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python-headless")
 
         timestamps = []
         total_frames = self.get_video_frame_count()
         frames_to_extract = min(total_frames, max_frames) if max_frames else total_frames
         for _ in tqdm(range(frames_to_extract), desc="retrieving timestamps"):
             success, _ = self.vc.read()
             if not success:
@@ -90,15 +89,15 @@
         """Return the total number of frames for a video file."""
         assert self.isOpened(), self._video_open_msg
         prop = self.get_cv_attribute("CAP_PROP_FRAME_COUNT")
         return int(self.vc.get(prop))
 
     @staticmethod
     def get_cv_attribute(attribute_name: str):
-        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python")
+        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python-headless")
 
         if int(cv2.__version__.split(".")[0]) < 3:  # pragma: no cover
             return getattr(cv2.cv, "CV_" + attribute_name)
         return getattr(cv2, attribute_name)
 
     @property
     def current_frame(self):
@@ -149,15 +148,15 @@
             else:
                 raise StopIteration
         else:
             self.vc.release()
             raise StopIteration
 
     def __enter__(self):
-        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python")
+        cv2 = get_package(package_name="cv2", installation_instructions="pip install opencv-python-headless")
 
         self.vc = cv2.VideoCapture(self.file_path)
         return self
 
     def __exit__(self, *args):
         self.vc.release()
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-"""Authors: Cody Baker."""
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-
 from ....utils.types import FolderPathType
 
 
 class AlphaOmegaRecordingInterface(BaseRecordingExtractorInterface):
     """
     Primary data interface class for converting AlphaOmega data.
 
     Uses the :py:class:`~spikeinterface.extractors.AlphaOmegaRecordingExtractor`.
     """
 
-    def __init__(self, folder_path: FolderPathType, verbose: bool = True):
+    def __init__(self, folder_path: FolderPathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
         Load and prepare data for AlphaOmega.
 
         Parameters
         ----------
         folder_path: string or Path
             Path to the folder of .mrx files.
         verbose: boolean
             Allows verbose.
             Default is True.
+        es_key: str, default: "ElectricalSeries"
         """
-        super().__init__(folder_path=folder_path, stream_id="RAW", verbose=verbose)
+        super().__init__(folder_path=folder_path, stream_id="RAW", verbose=verbose, es_key=es_key)
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
         annotation = self.recording_extractor.neo_reader.raw_annotations
         metadata["NWBFile"].update(session_start_time=annotation["blocks"][0]["rec_datetime"])
         return metadata
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     return path_list
 
 
 def read_all_eeg_file_lfp_data(file_path: FilePathType) -> np.ndarray:
     """
     Read LFP data from all Axona `.eeg` or `.egf` files in file_path's directory.
     E.g. if file_path='/my/directory/my_file.eeg', all .eeg channels will be conactenated
-    to a single np.array (chans x nobs). For .egf files substitude the file suffix.
+    to a single np.array (chans x nobs). For .egf files substitute the file suffix.
 
     Parameters
     ---------
     file_path FilePathType
         Full file_path of Axona `.eeg` or `.egf` file.
 
     Returns
@@ -118,15 +118,15 @@
 
     eeg_data = np.concatenate(eeg_memmaps, axis=0)
 
     return eeg_data
 
 
 # Helper functions for AxonaPositionDataInterface
-def parse_generic_header(file_path: FilePathType, params: Union[list, set]):
+def parse_generic_header(file_path: FilePathType, params: Union[list, set]) -> dict:
     """
     Given a binary file with phrases and line breaks, enters the
     first word of a phrase as dictionary key and the following
     string (without linebreaks) as value. Returns the dictionary.
 
     Parameters
     ----------
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,63 @@
-"""Authors: Heberto Mayorquin, Steffen Buergers."""
 from pynwb import NWBFile
 
-from .axona_utils import read_all_eeg_file_lfp_data, get_eeg_sampling_frequency, get_position_object
-from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
+from .axona_utils import (
+    get_eeg_sampling_frequency,
+    get_position_object,
+    read_all_eeg_file_lfp_data,
+)
 from ..baselfpextractorinterface import BaseLFPExtractorInterface
+from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
 from ....basedatainterface import BaseDataInterface
 from ....tools.nwb_helpers import get_module
-from ....utils import get_schema_from_method_signature, FilePathType
+from ....utils import FilePathType, get_schema_from_method_signature
 
 
 class AxonaRecordingInterface(BaseRecordingExtractorInterface):
-    """Primary data interface class for converting a Axona data using a
-    :py:class:`~spikeinterface.extractors.AxonaRecordingExtractor`."""
+    """
+    DataInterface for converting raw Axona data using a :py:class:`~spikeinterface.extractors.AxonaRecordingExtractor`.
+    """
 
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(self, file_path: FilePathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
 
         Parameters
         ----------
         file_path: FilePathType
             Path to .bin file.
         verbose: bool, optional, default: True
+        es_key: str, default: "ElectricalSeries"
         """
 
-        super().__init__(file_path=file_path, all_annotations=True, verbose=verbose)
+        super().__init__(file_path=file_path, all_annotations=True, verbose=verbose, es_key=es_key)
         self.source_data = dict(file_path=file_path, verbose=verbose)
         self.metadata_in_set_file = self.recording_extractor.neo_reader.file_parameters["set"]["file_header"]
 
         # Set the channel groups
         tetrode_id = self.recording_extractor.get_property("tetrode_id")
         self.recording_extractor.set_channel_groups(tetrode_id)
 
-    def extract_nwb_file_metadata(self):
+    def extract_nwb_file_metadata(self) -> dict:
         raw_annotations = self.recording_extractor.neo_reader.raw_annotations
         session_start_time = raw_annotations["blocks"][0]["segments"][0]["rec_datetime"]
         session_description = self.metadata_in_set_file["comments"]
         experimenter = self.metadata_in_set_file["experimenter"]
 
         nwbfile_metadata = dict(
             session_start_time=session_start_time,
             session_description=session_description,
-            experimenter=[experimenter],  # The schema expects an array of strings
+            experimenter=[experimenter] if experimenter else None,  # The schema expects an array of strings
         )
 
         # Filter empty values
         nwbfile_metadata = {property: value for property, value in nwbfile_metadata.items() if value}
 
         return nwbfile_metadata
 
-    def extract_ecephys_metadata(self):
+    def extract_ecephys_metadata(self) -> dict:
         unique_elec_group_names = set(self.recording_extractor.get_channel_groups())
         sw_version = self.metadata_in_set_file["sw_version"]
         description = f"Axona DacqUSB, sw_version={sw_version}"
 
         ecephys_metadata = dict(
             Device=[
                 dict(
@@ -77,24 +82,24 @@
     def get_metadata(self):
         metadata = super().get_metadata()
 
         nwbfile_metadata = self.extract_nwb_file_metadata()
         metadata["NWBFile"].update(nwbfile_metadata)
 
         ecephys_metadata = self.extract_ecephys_metadata()
-        metadata["Ecephys"] = ecephys_metadata
+        metadata["Ecephys"].update(ecephys_metadata)
 
         return metadata
 
 
 class AxonaUnitRecordingInterface(AxonaRecordingInterface):
     """Primary data interface class for converting a AxonaRecordingExtractor"""
 
     @classmethod
-    def get_source_schema(cls):
+    def get_source_schema(cls) -> dict:
         return dict(
             required=["file_path"],
             properties=dict(
                 file_path=dict(
                     type="string",
                     format="file",
                     description="Path to Axona file.",
@@ -109,15 +114,15 @@
         self.source_data = dict(file_path=file_path, noise_std=noise_std)
 
 
 class AxonaLFPDataInterface(BaseLFPExtractorInterface):
     ExtractorName = "NumpyRecording"
 
     @classmethod
-    def get_source_schema(cls):
+    def get_source_schema(cls) -> dict:
         return dict(
             required=["file_path"],
             properties=dict(file_path=dict(type="string")),
             type="object",
             additionalProperties=False,
         )
 
@@ -129,15 +134,15 @@
         self.source_data = dict(file_path=file_path)
 
 
 class AxonaPositionDataInterface(BaseDataInterface):
     """Primary data interface class for converting Axona position data"""
 
     @classmethod
-    def get_source_schema(cls):
+    def get_source_schema(cls) -> dict:
         return get_schema_from_method_signature(cls.__init__)
 
     def __init__(self, file_path: str):
         super().__init__(filename=file_path)
         self.source_data(file_path=file_path)
 
     def run_conversion(self, nwbfile: NWBFile, metadata: dict):
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,50 @@
-"""Authors: Cody Baker and Ben Dichter."""
-from typing import Optional, Union
-from pathlib import Path
+from typing import Literal, Optional
+
 from pynwb import NWBFile
-from pynwb.ecephys import ElectricalSeries
 
 from .baserecordingextractorinterface import BaseRecordingExtractorInterface
-from ...utils import get_schema_from_hdmf_class, OptionalFilePathType
-
-OptionalPathType = Optional[Union[str, Path]]
+from ...utils import FilePathType
 
 
 class BaseLFPExtractorInterface(BaseRecordingExtractorInterface):
     """Primary class for all LFP data interfaces."""
 
-    def get_metadata_schema(self):
-        metadata_schema = super().get_metadata_schema()
-        metadata_schema["properties"]["Ecephys"]["properties"].update(
-            ElectricalSeriesLFP=get_schema_from_hdmf_class(ElectricalSeries)
-        )
-        return metadata_schema
+    keywords = BaseRecordingExtractorInterface.keywords + [
+        "extracellular electrophysiology",
+        "LFP",
+        "local field potential",
+        "LF",
+    ]
 
-    def get_metadata(self):
-        metadata = super().get_metadata()
-        metadata["Ecephys"].update(
-            ElectricalSeriesLFP=dict(name="ElectricalSeriesLFP", description="Local field potential signal.")
-        )
-        return metadata
+    def __init__(self, verbose: bool = True, es_key: str = "ElectricalSeriesLFP", **source_data):
+        super().__init__(verbose=verbose, es_key=es_key, **source_data)
 
     def run_conversion(
         self,
-        nwbfile_path: OptionalFilePathType = None,
+        nwbfile_path: Optional[FilePathType] = None,
         nwbfile: Optional[NWBFile] = None,
         metadata: Optional[dict] = None,
         overwrite: bool = False,
         stub_test: bool = False,
         starting_time: Optional[float] = None,
-        write_as: str = "lfp",  # Literal["raw", "lfp", "processed"]
+        write_as: Literal["raw", "lfp", "processed"] = "lfp",
         write_electrical_series: bool = True,
-        es_key: str = "ElectricalSeriesLFP",
         compression: Optional[str] = None,
         compression_opts: Optional[int] = None,
         iterator_type: str = "v2",
         iterator_opts: Optional[dict] = None,
     ):
-        from ...tools.spikeinterface import write_recording
-
-        if stub_test or self.subset_channels is not None:
-            recording = self.subset_recording(stub_test=stub_test)
-        else:
-            recording = self.recording_extractor
-        write_recording(
-            recording=recording,
+        return super().run_conversion(
             nwbfile_path=nwbfile_path,
             nwbfile=nwbfile,
             metadata=metadata,
             overwrite=overwrite,
-            verbose=self.verbose,
+            stub_test=stub_test,
             starting_time=starting_time,
             write_as=write_as,
-            es_key=es_key,
+            write_electrical_series=write_electrical_series,
             compression=compression,
             compression_opts=compression_opts,
             iterator_type=iterator_type,
             iterator_opts=iterator_opts,
         )
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-"""Authors: Cody Baker."""
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-
 from ....utils.types import FilePathType
 
 
 class BiocamRecordingInterface(BaseRecordingExtractorInterface):
     """
     Primary data interface class for converting Biocam data.
 
     Using the :py:class:`~spikeinterface.extractors.BiocamRecordingExtractor`.
     """
 
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(self, file_path: FilePathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
         Load and prepare data for Biocam.
 
         Parameters
         ----------
-        folder_path : string or Path
+        file_path : string or Path
             Path to the .bwr file.
         verbose : bool, default: True
             Allows verbose.
+        es_key: str, default: "ElectricalSeries"
         """
-        super().__init__(file_path=file_path, verbose=verbose)
+        super().__init__(file_path=file_path, verbose=verbose, es_key=es_key)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,160 +1,153 @@
-"""Authors: Luiz Tauffer."""
+"""Authors: Heberto Mayorquin, Cody Baker and Ben Dichter."""
 from typing import Optional
-from pathlib import Path
-from warnings import warn
 
-from pynwb.ecephys import ElectricalSeries
+import numpy as np
+from pynwb import NWBFile
+from pynwb.device import Device
+from pynwb.ophys import Fluorescence, ImageSegmentation, ImagingPlane, TwoPhotonSeries
 
-from .header_tools import parse_nsx_basic_header, parse_nev_basic_header
-from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-from ..basesortingextractorinterface import BaseSortingExtractorInterface
-from ....tools import get_package
-from ....utils import (
-    get_schema_from_hdmf_class,
-    get_schema_from_method_signature,
+from ...baseextractorinterface import BaseExtractorInterface
+from ...utils import (
     FilePathType,
-    OptionalFilePathType,
+    fill_defaults,
+    get_base_schema,
+    get_schema_from_hdmf_class,
 )
 
 
-class BlackrockRecordingInterface(BaseRecordingExtractorInterface):
-    """Primary data interface class for converting Blackrock data using a
-    :py:class:`~spikeinterface.extractors.BlackrockRecordingExtractor`."""
-
-    @classmethod
-    def get_source_schema(cls):
-        source_schema = get_schema_from_method_signature(
-            class_method=cls.__init__, exclude=["block_index", "seg_index"]
-        )
-        source_schema["properties"]["file_path"]["description"] = "Path to Blackrock file."
-        return source_schema
+class BaseSegmentationExtractorInterface(BaseExtractorInterface):
+    """Parent class for all SegmentationExtractorInterfaces."""
 
-    def __init__(
-        self,
-        file_path: FilePathType,
-        nsx_override: OptionalFilePathType = None,
-        verbose: bool = True,
-        spikeextractors_backend: bool = False,
-    ):
-        """
-        Load and prepare data corresponding to Blackrock interface.
+    ExtractorModuleName = "roiextractors"
 
-        Parameters
-        ----------
-        file_path : FilePathType
-            The path to the Blackrock with suffix being .ns1, .ns2, .ns3, .ns4m .ns4, or .ns6
-        verbose: bool, default: True
-        spikeextractors_backend : bool
-            False by default. When True the interface uses the old extractor from the spikextractors library instead
-            of a new spikeinterface object.
-        """
-        file_path = Path(file_path)
-        if file_path.suffix == "":
-            assert nsx_override is not None, (
-                "if file_path is empty " 'provide a nsx file to load with "nsx_override" arg'
-            )
-            nsx_to_load = None
-            self.file_path = Path(nsx_override)
-        else:
-            assert "ns" in file_path.suffix, "file_path should be an nsx file"
-            nsx_to_load = int(file_path.suffix[-1])
-            self.file_path = file_path
-
-        if spikeextractors_backend:
-            # TODO: Remove spikeextractors backend
-            warn(
-                message=(
-                    "Interfaces using a spikeextractors backend will soon be deprecated! "
-                    "Please use the SpikeInterface backend instead."
-                ),
-                category=DeprecationWarning,
-                stacklevel=2,
-            )
-            spikeextractors = get_package(package_name="spikeextractors")
-            spikeinterface = get_package(package_name="spikeinterface")
-
-            self.Extractor = spikeextractors.BlackrockRecordingExtractor
-            super().__init__(filename=file_path, nsx_override=nsx_override, nsx_to_load=nsx_to_load, verbose=verbose)
-            self.source_data = dict(
-                file_path=file_path, nsx_override=nsx_override, nsx_to_load=nsx_to_load, verbose=verbose
-            )
-            self.recording_extractor = spikeinterface.core.old_api_utils.OldToNewRecording(
-                oldapi_recording_extractor=self.recording_extractor
-            )
-
-        else:
-            spikeinterface = get_package(package_name="spikeinterface")
-
-            self.RX = spikeinterface.extractors.BlackrockRecordingExtractor
-            super().__init__(file_path=file_path, stream_id=str(nsx_to_load), verbose=verbose)
+    def __init__(self, **source_data):
+        super().__init__(**source_data)
+        self.segmentation_extractor = self.get_extractor()(**source_data)
 
-    def get_metadata_schema(self):
+    def get_metadata_schema(self) -> dict:
         metadata_schema = super().get_metadata_schema()
-        metadata_schema["properties"]["Ecephys"]["properties"].update(
-            ElectricalSeriesRaw=get_schema_from_hdmf_class(ElectricalSeries),
-            ElectricalSeriesProcessed=get_schema_from_hdmf_class(ElectricalSeries),
+        metadata_schema["required"] = ["Ophys"]
+        metadata_schema["properties"]["Ophys"] = get_base_schema()
+        metadata_schema["properties"]["Ophys"]["properties"] = dict(
+            Device=dict(type="array", minItems=1, items=get_schema_from_hdmf_class(Device)),
         )
+        metadata_schema["properties"]["Ophys"]["properties"].update(
+            Fluorescence=get_schema_from_hdmf_class(Fluorescence),
+            ImageSegmentation=get_schema_from_hdmf_class(ImageSegmentation),
+            ImagingPlane=get_schema_from_hdmf_class(ImagingPlane),
+            TwoPhotonSeries=get_schema_from_hdmf_class(TwoPhotonSeries),
+        )
+        metadata_schema["properties"]["Ophys"]["required"] = ["Device", "ImageSegmentation"]
+
+        # Temporary fixes until centralized definition of metadata schemas
+        metadata_schema["properties"]["Ophys"]["properties"]["ImagingPlane"].update(type="array")
+        metadata_schema["properties"]["Ophys"]["properties"]["TwoPhotonSeries"].update(type="array")
+
+        metadata_schema["properties"]["Ophys"]["properties"]["Fluorescence"]["properties"]["roi_response_series"][
+            "items"
+        ]["required"] = list()
+        metadata_schema["properties"]["Ophys"]["properties"]["ImageSegmentation"]["additionalProperties"] = True
+        metadata_schema["properties"]["Ophys"]["properties"]["Fluorescence"]["properties"]["roi_response_series"].pop(
+            "maxItems"
+        )
+        metadata_schema["properties"]["Ophys"]["properties"]["DfOverF"] = metadata_schema["properties"]["Ophys"][
+            "properties"
+        ]["Fluorescence"]
+
+        fill_defaults(metadata_schema, self.get_metadata())
         return metadata_schema
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
+        from ...tools.roiextractors import get_nwb_segmentation_metadata
+
         metadata = super().get_metadata()
-        # Open file and extract headers
-        basic_header = parse_nsx_basic_header(self.source_data["file_path"])
-        if "TimeOrigin" in basic_header:
-            session_start_time = basic_header["TimeOrigin"]
-            metadata["NWBFile"].update(session_start_time=session_start_time.strftime("%Y-%m-%dT%H:%M:%S"))
-        if "Comment" in basic_header:
-            metadata["NWBFile"].update(session_description=basic_header["Comment"])
-        # Checks if data is raw or processed
-        if int(self.file_path.suffix[-1]) >= 5:
-            metadata["Ecephys"]["ElectricalSeriesRaw"] = dict(name="ElectricalSeriesRaw")
-        else:
-            metadata["Ecephys"]["ElectricalSeriesProcessed"] = dict(name="ElectricalSeriesProcessed")
+        metadata.update(get_nwb_segmentation_metadata(self.segmentation_extractor))
         return metadata
 
-    def get_conversion_options(self):
-        if int(self.file_path.suffix[-1]) >= 5:
-            write_as = "raw"
-            es_key = "ElectricalSeriesRaw"
-        else:
-            write_as = "processed"
-            es_key = "ElectricalSeriesProcessed"
-        conversion_options = dict(write_as=write_as, es_key=es_key, stub_test=False)
-        return conversion_options
-
+    def get_original_timestamps(self) -> np.ndarray:
+        reinitialized_extractor = self.get_extractor()(**self.source_data)
+        return reinitialized_extractor.frame_to_time(frames=np.arange(stop=reinitialized_extractor.get_num_frames()))
+
+    def get_timestamps(self) -> np.ndarray:
+        return self.segmentation_extractor.frame_to_time(
+            frames=np.arange(stop=self.segmentation_extractor.get_num_frames())
+        )
 
-class BlackrockSortingInterface(BaseSortingExtractorInterface):
-    """Primary data interface class for converting Blackrock spiking data."""
-
-    @classmethod
-    def get_source_schema(cls):
-        metadata_schema = get_schema_from_method_signature(class_method=cls.__init__)
-        metadata_schema["additionalProperties"] = True
-        metadata_schema["properties"]["file_path"].update(description="Path to Blackrock file.")
-        return metadata_schema
+    def set_aligned_timestamps(self, aligned_timestamps: np.ndarray):
+        self.segmentation_extractor.set_times(times=aligned_timestamps)
 
-    def __init__(self, file_path: FilePathType, sampling_frequency: float = None, verbose: bool = True):
+    def run_conversion(
+        self,
+        nwbfile_path: Optional[FilePathType] = None,
+        nwbfile: Optional[NWBFile] = None,
+        metadata: Optional[dict] = None,
+        overwrite: bool = False,
+        stub_test: bool = False,
+        stub_frames: int = 100,
+        include_roi_centroids: bool = True,
+        include_roi_acceptance: bool = True,
+        mask_type: Optional[str] = "image",  # Optional[Literal["image", "pixel", "voxel"]]
+        iterator_options: Optional[dict] = None,
+        compression_options: Optional[dict] = None,
+    ):
         """
+
         Parameters
         ----------
-        file_path : str, Path
-            The file path to the ``.nev`` data
-        sampling_frequency: float,
-            The sampling frequency for the sorting extractor. When the signal data is available (.ncs) those files will be
-        used to extract the frequency automatically. Otherwise, the sampling frequency needs to be specified for
-        this extractor to be initialized.
-        verbose : bool, optional
-            Enables verbosity
+        nwbfile_path : FilePathType, optional
+        nwbfile : NWBFile, optional
+            The NWBFile to add the plane segmentation to.
+        metadata : dict, optional
+            The metadata for the interface
+        overwrite : bool, default: False
+        stub_test : bool, default: False
+        stub_frames : int, default: 100
+        include_roi_centroids : bool, default: True
+            Whether to include the ROI centroids on the PlaneSegmentation table.
+            If there are a very large number of ROIs (such as in whole-brain recordings),
+            you may wish to disable this for faster write speeds.
+        include_roi_acceptance : bool, default: True
+            Whether to include if the detected ROI was 'accepted' or 'rejected'.
+            If there are a very large number of ROIs (such as in whole-brain recordings), you may wish to ddisable this for
+            faster write speeds.
+        mask_type : {'image', 'pixel', 'voxel'}, optional
+            There are two types of ROI masks in NWB: ImageMasks and PixelMasks.
+            Image masks have the same shape as the reference images the segmentation was applied to, and weight each pixel
+                by its contribution to the ROI (typically boolean, with 0 meaning 'not in the ROI').
+            Pixel masks are instead indexed by ROI, with the data at each index being the shape of the image by the number
+                of pixels in each ROI.
+            Voxel masks are instead indexed by ROI, with the data at each index being the shape of the volume by the number
+                of voxels in each ROI.
+            Specify your choice between these three as mask_type='image', 'pixel', 'voxel', or None.
+            If None, the mask information is not written to the NWB file.
+            Defaults to 'image'.
+        iterator_options : dict, optional
+            The options to use when iterating over the image masks of the segmentation extractor.
+        compression_options : dict, optional
+            The options to use when compressing the image masks of the segmentation extractor.
+
+        Returns
+        -------
+
         """
-        super().__init__(file_path=file_path, sampling_frequency=sampling_frequency, verbose=verbose)
+        from ...tools.roiextractors import write_segmentation
 
-    def get_metadata(self):
-        metadata = super().get_metadata()
-        # Open file and extract headers
-        basic_header = parse_nev_basic_header(self.source_data["file_path"])
-        if "TimeOrigin" in basic_header:
-            session_start_time = basic_header["TimeOrigin"]
-            metadata["NWBFile"].update(session_start_time=session_start_time.strftime("%Y-%m-%dT%H:%M:%S"))
-        if "Comment" in basic_header:
-            metadata["NWBFile"].update(session_description=basic_header["Comment"])
-        return metadata
+        if stub_test:
+            stub_frames = min([stub_frames, self.segmentation_extractor.get_num_frames()])
+            segmentation_extractor = self.segmentation_extractor.frame_slice(start_frame=0, end_frame=stub_frames)
+        else:
+            segmentation_extractor = self.segmentation_extractor
+
+        write_segmentation(
+            segmentation_extractor=segmentation_extractor,
+            nwbfile_path=nwbfile_path,
+            nwbfile=nwbfile,
+            metadata=metadata,
+            overwrite=overwrite,
+            verbose=self.verbose,
+            include_roi_centroids=include_roi_centroids,
+            include_roi_acceptance=include_roi_acceptance,
+            mask_type=mask_type,
+            iterator_options=iterator_options,
+            compression_options=compression_options,
+        )
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         FieldDef("TimeStampResolution", "I", format_none),  # 4 bytes   - uint32
         FieldDef("TimeOrigin", "8H", format_timeorigin),  # 16 bytes  - 8 uint16
         FieldDef("ChannelCount", "I", format_none),
     ]  # 4 bytes   - uint32
     datafile = open(nsx_file, "rb")
     filetype_id = bytes.decode(datafile.read(8), "latin-1")
     if filetype_id == "NEURALSG":
-        # this wont contain fields that can be added to NWBFile metadata
+        # this won't contain fields that can be added to NWBFile metadata
         return dict()
     return processheaders(datafile, nsx_basic_dict)
 
 
 def parse_nev_basic_header(nev_file):
     nev_basic_dict = [
         FieldDef("FileTypeID", "8s", format_stripstring),  # 8 bytes   - 8 char array
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/ced/ceddatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,44 @@
-"""Authors: Heberto Mayorquin, Luiz Tauffer."""
-from pathlib import Path
+from typing import Optional
+from warnings import warn
 
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-from ....tools import get_package
-from ....utils import get_schema_from_method_signature, FilePathType
+from ....utils import ArrayType, FilePathType
 
 
-def _test_sonpy_installation() -> None:
-    get_package(
-        package_name="sonpy",
-        excluded_python_versions=["3.10"],
-        excluded_platforms_and_python_versions=dict(darwin=["3.7"]),
-    )
-
-
-class CEDRecordingInterface(BaseRecordingExtractorInterface):
-    """Primary data interface class for converting data from CED (Cambridge Electronic
-    Design) using the :py:class:`~spikeinterface.extractors.CedRecordingExtractor`."""
-
-    ExtractorName = "CedRecordingExtractor"
+class SpikeGadgetsRecordingInterface(BaseRecordingExtractorInterface):
+    """Data interface class for converting data in the SpikeGadgets format.
+    Uses :py:class:`~spikeinterface.extractors.SpikeGadgetsRecordingExtractor`."""
 
     @classmethod
-    def get_source_schema(cls):
-        source_schema = get_schema_from_method_signature(class_method=cls.__init__, exclude=["smrx_channel_ids"])
-        source_schema.update(additionalProperties=True)
-        source_schema["properties"]["file_path"].update(description="Path to CED data file.")
+    def get_source_schema(cls) -> dict:
+        source_schema = super().get_source_schema()
+        source_schema["properties"]["file_path"].update(description="Path to SpikeGadgets (.rec) file.")
         return source_schema
 
-    @classmethod
-    def get_all_channels_info(cls, file_path: FilePathType):
-        """Retrieve and inspect necessary channel information prior to initialization."""
-        _test_sonpy_installation()
-        getattr(cls, "RX")  # Required to trigger dynamic access in case this method is called first
-        return cls.RX.get_all_channels_info(file_path=file_path)
-
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(
+        self,
+        file_path: FilePathType,
+        stream_id: str = "trodes",
+        gains: Optional[ArrayType] = None,
+        verbose: bool = True,
+        es_key: str = "ElectricalSeries",
+    ):
         """
-        Initialize reading of CED file.
+        Recording Interface for the SpikeGadgets Format.
 
         Parameters
         ----------
-        file_path: FilePathType
-            Path to .smr or .smrx file.
-        verbose: bool, default: True
+        file_path : FilePathType
+            Path to the .rec file.
+        gains : array_like, optional
+            The early versions of SpikeGadgets do not automatically record the conversion factor ('gain') of the
+            acquisition system. Thus it must be specified either as a single value (if all channels have the same gain)
+            or an array of values for each channel.
+        es_key : str, default: "ElectricalSeries"
         """
-        _test_sonpy_installation()
-
-        stream_id = "1" if Path(file_path).suffix == ".smr" else None
-        super().__init__(file_path=file_path, stream_id=stream_id, verbose=verbose)
+        super().__init__(file_path=file_path, stream_id=stream_id, verbose=verbose, es_key=es_key)
 
-        # Subset raw channel properties
-        signal_channels = self.recording_extractor.neo_reader.header["signal_channels"]
-        channel_ids_of_raw_data = [channel_info[1] for channel_info in signal_channels if channel_info[4] == "mV"]
-        self.recording_extractor = self.recording_extractor.channel_slice(channel_ids=channel_ids_of_raw_data)
+        if gains is not None:
+            if len(gains) == 1:
+                gains = [gains[0]] * self.recording_extractor.get_num_channels()
+            self.recording_extractor.set_channel_gains(gains=gains)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-"""Authors: Cody Baker and Ben Dichter."""
 from pathlib import Path
 from warnings import warn
 
-import scipy
 import numpy as np
+import scipy
 
 from ..basesortingextractorinterface import BaseSortingExtractorInterface
 from ....tools import get_package
 from ....utils import FilePathType
 
 
 class CellExplorerSortingInterface(BaseSortingExtractorInterface):
     """Primary data interface class for converting Cell Explorer spiking data."""
 
-    ExtractorModuleName = "spikeextractors"
-
     def __init__(self, file_path: FilePathType, verbose: bool = True):
         """
         Initialize read of Cell Explorer file.
 
         Parameters
         ----------
         file_path: FilePathType
@@ -53,51 +50,58 @@
             self.read_spikes_info_with_scipy = True
         except NotImplementedError:
             spikes_mat = hdf5storage.loadmat(file_name=str(spikes_matfile_path))
             self.read_spikes_info_with_scipy = False
         cell_info = spikes_mat.get("spikes", np.empty(0))
         self.cell_info_fields = cell_info.dtype.names
 
+        unit_ids = self.sorting_extractor.get_unit_ids()
         if self.read_spikes_info_with_scipy:
-            unit_ids = self.sorting_extractor.get_unit_ids()
             if "cluID" in self.cell_info_fields:
-                for unit_id, value in zip(unit_ids, [int(x) for x in cell_info["cluID"][0][0][0]]):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="clu_id", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids, key="clu_id", values=[int(x) for x in cell_info["cluID"][0][0][0]]
+                )
             if "shankID" in self.cell_info_fields:
-                for unit_id, value in zip(unit_ids, [f"Group{x}" for x in cell_info["shankID"][0][0][0]]):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="group_id", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids, key="group_id", values=[f"Group{x}" for x in cell_info["shankID"][0][0][0]]
+                )
             if "region" in self.cell_info_fields:
-                for unit_id, value in zip(unit_ids, [str(x[0]) for x in cell_info["region"][0][0][0]]):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="location", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids, key="location", values=[str(x[0]) for x in cell_info["region"][0][0][0]]
+                )
         else:  # Logic for hdf5storage
-            unit_ids = self.sorting_extractor.get_unit_ids()
             if "cluID" in self.cell_info_fields:
-                for unit_id, value in zip(unit_ids, [int(x) for x in cell_info["cluID"][0][0]]):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="clu_id", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids, key="clu_id", values=[int(x) for x in cell_info["cluID"][0][0]]
+                )
             if "shankID" in self.cell_info_fields:
-                for unit_id, value in zip(unit_ids, [f"Group{x}" for x in cell_info["shankID"][0][0]]):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="group_id", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids, key="group_id", values=[f"Group{x}" for x in cell_info["shankID"][0][0]]
+                )
             if "region" in self.cell_info_fields:
-                for unit_id, value in zip(unit_ids, [str(x[0]) for x in cell_info["region"][0]][0]):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="location", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids, key="location", values=[str(x[0]) for x in cell_info["region"][0][0]]
+                )
         celltype_mapping = {"pE": "excitatory", "pI": "inhibitory", "[]": "unclassified"}
         celltype_file_path = session_path / f"{session_id}.CellClass.cellinfo.mat"
         if celltype_file_path.is_file():
             celltype_info = scipy.io.loadmat(celltype_file_path).get("CellClass", np.empty(0))
             if "label" in celltype_info.dtype.names:
-                for unit_id, value in zip(
-                    unit_ids, [str(celltype_mapping[str(x[0])]) for x in celltype_info["label"][0][0][0]]
-                ):
-                    self.sorting_extractor.set_unit_property(unit_id=unit_id, property_name="cell_type", value=value)
+                self.sorting_extractor.set_property(
+                    ids=unit_ids,
+                    key="cell_type",
+                    values=[str(celltype_mapping[str(x[0])]) for x in celltype_info["label"][0][0][0]],
+                )
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
+        metadata = super().get_metadata()
         session_path = Path(self.source_data["file_path"]).parent
         session_id = session_path.stem
         # TODO: add condition for retrieving ecephys metadata if no recording or lfp are included in conversion
-        metadata = dict(NWBFile=dict(session_id=session_id))
+        metadata["NWBFile"].update(session_id=session_id)
 
         unit_properties = []
         cellinfo_file_path = session_path / f"{session_id}.spikes.cellinfo.mat"
         if cellinfo_file_path.is_file():
             cell_info_fields = self.cell_info_fields
             if "cluID" in cell_info_fields:
                 unit_properties.append(
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,69 @@
-"""Authors: Heberto Mayorquin"""
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-
 from ....tools import get_package
 from ....utils.types import FilePathType
 
 
 class EDFRecordingInterface(BaseRecordingExtractorInterface):
-    """Primary data interface class for converting European Data Format (EDF) data
-    using the :py:class:`~spikeinterface.extractors.EDFRecordingExtractor`."""
+    """
+    Data interface class for converting European Data Format (EDF) data using the
+    :py:class:`~spikeinterface.extractors.EDFRecordingExtractor`.
+
+    Not supported for Python 3.8 and 3.9 on M1 macs.
+    """
+
+    keywords = BaseRecordingExtractorInterface.keywords + [
+        "European Data Format",
+    ]
 
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(self, file_path: FilePathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
-        Load and prepare data for EDF
-        Currently only continuous EDF+ files (EDF+C) and original EDF files (EDF) are supported
+        Load and prepare data for EDF.
+        Currently, only continuous EDF+ files (EDF+C) and original EDF files (EDF) are supported
 
 
         Parameters
         ----------
-        folder_path : str or Path
+        file_path : str or Path
             Path to the edf file
         verbose : bool, default: True
             Allows verbose.
+        es_key : str, default: "ElectricalSeries"
         """
-        _ = get_package(package_name="pyedflib")
+        get_package(
+            package_name="pyedflib",
+            excluded_platforms_and_python_versions=dict(darwin=dict(arm=["3.8", "3.9"])),
+        )
 
-        super().__init__(file_path=file_path, verbose=verbose)
+        super().__init__(file_path=file_path, verbose=verbose, es_key=es_key)
         self.edf_header = self.recording_extractor.neo_reader.edf_header
 
-    def extract_nwb_file_metadata(self):
+    def extract_nwb_file_metadata(self) -> dict:
         nwbfile_metadata = dict(
             session_start_time=self.edf_header["startdate"],
             experimenter=self.edf_header["technician"],
         )
 
         # Filter empty values
         nwbfile_metadata = {property: value for property, value in nwbfile_metadata.items() if value}
 
         return nwbfile_metadata
 
-    def extract_subject_metadata(self):
+    def extract_subject_metadata(self) -> dict:
         subject_metadata = dict(
             subject_id=self.edf_header["patientcode"],
             date_of_birth=self.edf_header["birthdate"],
         )
 
-        # Filfter empty values
+        # Filter empty values
         subject_metadata = {property: value for property, value in subject_metadata.items() if value}
 
         return subject_metadata
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
         nwbfile_metadata = self.extract_nwb_file_metadata()
         metadata["NWBFile"].update(nwbfile_metadata)
 
         subject_metadata = self.extract_subject_metadata()
         metadata.get("Subject", dict()).update(subject_metadata)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""Authors: Heberto Mayorquin, Cody Baker and Ben Dichter."""
 from pathlib import Path
 from warnings import warn
 
 from pynwb.ecephys import ElectricalSeries
 
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
 from ....tools import get_package
-from ....utils import get_schema_from_hdmf_class, FilePathType
+from ....utils import FilePathType, get_schema_from_hdmf_class
 
 
-def extract_electrode_metadata_with_pyintan(file_path):
+def extract_electrode_metadata_with_pyintan(file_path) -> dict:
     pyintan = get_package(package_name="pyintan")
 
     if ".rhd" in Path(file_path).suffixes:
         intan_file_metadata = pyintan.intan.read_rhd(file_path)[1]
     else:
         intan_file_metadata = pyintan.intan.read_rhs(file_path)[1]
 
@@ -34,15 +33,15 @@
         group_electrode_numbers=group_electrode_numbers,
         custom_names=custom_names,
     )
 
     return electrodes_metadata
 
 
-def extract_electrode_metadata(recording_extractor):
+def extract_electrode_metadata(recording_extractor) -> dict:
     channel_name_array = recording_extractor.get_property("channel_name")
 
     group_names = [channel.split("-")[0] for channel in channel_name_array]
     unique_group_names = set(group_names)
     group_electrode_numbers = [int(channel.split("-")[1]) for channel in channel_name_array]
     custom_names = list()
 
@@ -60,56 +59,34 @@
     """Primary data interface class for converting Intan data using the
     :py:class:`~spikeinterface.extractors.IntanRecordingExtractor`."""
 
     def __init__(
         self,
         file_path: FilePathType,
         stream_id: str = "0",
-        spikeextractors_backend: bool = False,
         verbose: bool = True,
+        es_key: str = "ElectricalSeries",
     ):
         """
         Load and prepare raw data and corresponding metadata from the Intan format (.rhd or .rhs files).
 
         Parameters
         ----------
         file_path : FilePathType
             Path to either a rhd or a rhs file
         stream_id : str, optional
             The stream of the data for spikeinterface, "0" by default.
-        spikeextractors_backend : bool
-            False by default. When True the interface uses the old extractor from the spikextractors library instead
-            of a new spikeinterface object.
-        verbose : bool
+        verbose : bool, default: True
             Verbose
+        es_key : str, default: "ElectricalSeries"
         """
 
-        if spikeextractors_backend:
-            # TODO: Remove spikeextractors backend and pyintan dependency
-            warn(
-                message=(
-                    "Interfaces using a spikeextractors backend will soon be deprecated! "
-                    "Please use the SpikeInterface backend instead."
-                ),
-                category=DeprecationWarning,
-                stacklevel=2,
-            )
-
-            _ = get_package(package_name="pyintan")
-            from spikeextractors import IntanRecordingExtractor
-            from spikeinterface.core.old_api_utils import OldToNewRecording
-
-            self.Extractor = IntanRecordingExtractor
-            super().__init__(file_path=file_path, verbose=verbose)
-            self.recording_extractor = OldToNewRecording(oldapi_recording_extractor=self.recording_extractor)
-            electrodes_metadata = extract_electrode_metadata_with_pyintan(file_path)
-        else:
-            self.stream_id = stream_id
-            super().__init__(file_path=file_path, stream_id=self.stream_id, verbose=verbose)
-            electrodes_metadata = extract_electrode_metadata(recording_extractor=self.recording_extractor)
+        self.stream_id = stream_id
+        super().__init__(file_path=file_path, stream_id=self.stream_id, verbose=verbose, es_key=es_key)
+        electrodes_metadata = extract_electrode_metadata(recording_extractor=self.recording_extractor)
 
         group_names = electrodes_metadata["group_names"]
         group_electrode_numbers = electrodes_metadata["group_electrode_numbers"]
         unique_group_names = electrodes_metadata["unique_group_names"]
         custom_names = electrodes_metadata["custom_names"]
 
         channel_ids = self.recording_extractor.get_channel_ids()
@@ -118,22 +95,22 @@
             self.recording_extractor.set_property(
                 key="group_electrode_number", ids=channel_ids, values=group_electrode_numbers
             )
 
         if any(custom_names):
             self.recording_extractor.set_property(key="custom_channel_name", ids=channel_ids, values=custom_names)
 
-    def get_metadata_schema(self):
+    def get_metadata_schema(self) -> dict:
         metadata_schema = super().get_metadata_schema()
         metadata_schema["properties"]["Ecephys"]["properties"].update(
             ElectricalSeriesRaw=get_schema_from_hdmf_class(ElectricalSeries)
         )
         return metadata_schema
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
         ecephys_metadata = metadata["Ecephys"]
 
         # Add device
         device = dict(
             name="Intan",
             description="Intan recording",
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-"""Authors: Heberto Mayorquin, Cody Baker."""
 from ..basesortingextractorinterface import BaseSortingExtractorInterface
 from ....utils import FolderPathType
 
 
 class KiloSortSortingInterface(BaseSortingExtractorInterface):
     """Primary data interface class for converting a KiloSortingExtractor from spikeinterface."""
 
-    def __init__(self, folder_path: FolderPathType, keep_good_only: bool = False, verbose: bool = True):
+    def __init__(
+        self,
+        folder_path: FolderPathType,
+        keep_good_only: bool = False,
+        verbose: bool = True,
+    ):
         """
         Load and prepare sorting data for kilosort
 
         Parameters
         ----------
         folder_path: str or Path
             Path to the output Phy folder (containing the params.py)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""Authors: Cody Baker."""
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-
 from ....utils.types import FilePathType
 
 
 class MCSRawRecordingInterface(BaseRecordingExtractorInterface):
     """
     Primary data interface class for converting MCSRaw data.
 
     Using the :py:class:`~spikeinterface.extractors.MCSRawRecordingExtractor`.
     """
 
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(self, file_path: FilePathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
         Load and prepare data for MCSRaw.
 
         Parameters
         ----------
         folder_path: string or Path
             Path to the .raw file.
         verbose: bool, default: True
             Allows verbose.
-            Default is True.
+        es_key: str, default: "ElectricalSeries"
         """
-        super().__init__(file_path=file_path, verbose=verbose)
+        super().__init__(file_path=file_path, verbose=verbose, es_key=es_key)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,38 @@
-"""Authors: Cody Baker."""
 import json
 
 from pynwb.ecephys import ElectricalSeries
 
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-from ....utils.types import FilePathType
 from ....utils.json_schema import NWBMetaDataEncoder, get_schema_from_hdmf_class
+from ....utils.types import FilePathType
 
 
 class MEArecRecordingInterface(BaseRecordingExtractorInterface):
     """
     Primary data interface class for converting MEArec recording data.
 
     Uses the :py:class:`~spikeinterface.extractors.MEArecRecordingExtractor`.
     """
 
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(self, file_path: FilePathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
         Load and prepare data for MEArec.
 
         Parameters
         ----------
-        folder_path: string or Path
+        folder_path : str or Path
             Path to the MEArec .h5 file.
-        verbose: bool, default: True
+        verbose : bool, default: True
             Allows verbose.
+        es_key : str, default: "ElectricalSeries"
         """
-        super().__init__(file_path=file_path, verbose=verbose)
-        self.es_key = "ElectricalSeries"
-
-    def get_metadata_schema(self):
-        metadata_schema = super().get_metadata_schema()
-
-        metadata_schema["properties"]["Ecephys"]["properties"].update(
-            ElectricalSeries=get_schema_from_hdmf_class(ElectricalSeries)
-        )
-
-        return metadata_schema
+        super().__init__(file_path=file_path, verbose=verbose, es_key=es_key)
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
 
         # TODO: improve ProbeInterface integration in our writing procedures
         # probe = self.recording_extractor.get_probe()  # TODO: Need to check if this is always available
 
         # There is a lot of device/electrode/waveform/sorting configuration information...
         # But no session start time...
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Authors: Heberto Mayorquin, Cody Baker, Ben Dichter and Julia Sprenger."""
 import json
-from typing import List, Dict
+from typing import List
+
 import numpy as np
 
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
 from ..basesortingextractorinterface import BaseSortingExtractorInterface
 from ....utils import FolderPathType
 from ....utils.json_schema import dict_deep_update
 
 
 class NeuralynxRecordingInterface(BaseRecordingExtractorInterface):
     """Primary data interface for converting Neuralynx data. Uses
     :py:class:`~spikeinterface.extractors.NeuralynxRecordingExtractor`."""
 
-    def __init__(self, folder_path: FolderPathType, verbose: bool = True):
-        super().__init__(folder_path=folder_path, verbose=verbose, all_annotations=True)
+    def __init__(self, folder_path: FolderPathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
+        super().__init__(folder_path=folder_path, verbose=verbose, all_annotations=True, es_key=es_key)
 
         # convert properties of object dtype (e.g. datetime) and bool as these are not supported by nwb
         for key in self.recording_extractor.get_property_keys():
             value = self.recording_extractor.get_property(key)
             if value.dtype == object or value.dtype == np.bool_:
                 self.recording_extractor.set_property(key, np.asarray(value, dtype=str))
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         neo_metadata = extract_neo_header_metadata(self.recording_extractor.neo_reader)
 
         # remove filter related entries already covered by `add_recording_extractor_properties`
         neo_metadata = {k: v for k, v in neo_metadata.items() if not k.lower().startswith("dsp")}
 
         # map Neuralynx metadata to NWB
         nwb_metadata = {"NWBFile": {}, "Ecephys": {"Device": []}}
@@ -110,15 +110,15 @@
         common_header["recording_opened"] = min([h["recording_opened"] for h in headers])
     if "recording_closed" not in common_header and all(["recording_closed" in h for h in headers]):
         common_header["recording_closed"] = max([h["recording_closed"] for h in headers])
 
     return common_header
 
 
-def _dict_intersection(dict_list: List) -> Dict:
+def _dict_intersection(dict_list: List) -> dict:
     """
     Intersect dict_list and return only common keys and values
     Parameters
     ----------
     dict_list: list of dicitionaries each representing a header
     Returns
     -------
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Authors: Cody Baker and Ben Dichter."""
-from pathlib import Path
 from datetime import datetime
+from pathlib import Path
+
 from dateutil import parser
 
 from ....tools import get_package
 
 
-def get_xml_file_path(data_file_path: str):
+def get_xml_file_path(data_file_path: str) -> str:
     """
     Infer the xml_file_path from the data_file_path (.dat or .eeg).
 
     Assumes the two are in the same folder and follow the session_id naming convention.
     """
     session_path = Path(data_file_path).parent
     return str(session_path / f"{session_path.stem}.xml")
@@ -74,15 +75,15 @@
         for group in root.find("anatomicalDescription").find("channelGroups").findall("group")
     ]
     return channel_groups
 
 
 def get_session_start_time(xml_file_path: str) -> datetime:
     """
-    Auxiliary function for retrieving the session start tiem from the xml file.
+    Auxiliary function for retrieving the session start time from the xml file.
 
     Returns
     -------
         datetime object describing the start time
     """
     root = get_xml(xml_file_path)
     date_elem = safe_nested_find(root, ["generalInfo", "date"])
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,98 @@
-"""Authors: Heberto Mayorquin, Luiz Tauffer."""
+from pathlib import Path
 from typing import Optional
-from warnings import warn
 
+from .header_tools import parse_nev_basic_header, parse_nsx_basic_header
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
 from ..basesortingextractorinterface import BaseSortingExtractorInterface
-from ....utils import get_schema_from_method_signature, FolderPathType
+from ....utils import FilePathType, get_schema_from_method_signature
 
 
-class OpenEphysRecordingInterface(BaseRecordingExtractorInterface):
-    """Primary data interface for converting OpenEphys data. Uses
-    :py:class:`~spikeinterface.extractors.OpenEphysBinaryRecordingExtractor`."""
-
-    ExtractorName = "OpenEphysBinaryRecordingExtractor"
+class BlackrockRecordingInterface(BaseRecordingExtractorInterface):
+    """Primary data interface class for converting Blackrock data using a
+    :py:class:`~spikeinterface.extractors.BlackrockRecordingExtractor`."""
 
     @classmethod
     def get_source_schema(cls):
-        """Compile input schema for the RecordingExtractor."""
-        source_schema = get_schema_from_method_signature(
-            class_method=cls.__init__, exclude=["recording_id", "experiment_id", "stub_test"]
-        )
-        source_schema["properties"]["folder_path"]["description"] = "Path to directory containing OpenEphys files."
+        source_schema = get_schema_from_method_signature(method=cls.__init__, exclude=["block_index", "seg_index"])
+        source_schema["properties"]["file_path"]["description"] = "Path to Blackrock file."
         return source_schema
 
     def __init__(
         self,
-        folder_path: FolderPathType,
-        experiment_id: int = 0,
-        recording_id: int = 0,
-        stub_test: bool = False,
+        file_path: FilePathType,
+        nsx_override: Optional[FilePathType] = None,
         verbose: bool = True,
-        spikeextractors_backend: bool = False,
+        es_key: str = "ElectricalSeries",
     ):
         """
-        Initialize reading of OpenEphys binary recording.
+        Load and prepare data corresponding to Blackrock interface.
 
         Parameters
         ----------
-        folder_path: FolderPathType
-            Path to OpenEphys directory.
-        experiment_id : int, default: 0
-        recording_id : int, default: 0
-        stub_test : bool, default: False
-        verbose : bool, default: True
-        spikeextractors_backend : bool, default: False
+        file_path : FilePathType
+            The path to the Blackrock with suffix being .ns1, .ns2, .ns3, .ns4m .ns4, or .ns6
+        verbose: bool, default: True
+        es_key : str, default: "ElectricalSeries"
         """
-        self.spikeextractors_backend = spikeextractors_backend
-        if spikeextractors_backend:
-            # TODO: Remove spikeextractors backend
-            warn(
-                message=(
-                    "Interfaces using a spikeextractors backend will soon be deprecated! "
-                    "Please use the SpikeInterface backend instead."
-                ),
-                category=DeprecationWarning,
-                stacklevel=2,
-            )
-            from spikeextractors import OpenEphysRecordingExtractor
-            from spikeinterface.core.old_api_utils import OldToNewRecording
 
-            self.Extractor = OpenEphysRecordingExtractor
-            super().__init__(
-                folder_path=folder_path, experiment_id=experiment_id, recording_id=recording_id, verbose=verbose
+        file_path = Path(file_path)
+        if file_path.suffix == "":
+            assert nsx_override is not None, (
+                "if file_path is empty " 'provide a nsx file to load with "nsx_override" arg'
             )
-            self.recording_extractor = OldToNewRecording(oldapi_recording_extractor=self.recording_extractor)
-            # Remove when spikeinterface 0.95 is released, this has an int sampling rate that causes problems
-            self.recording_extractor._sampling_frequency = float(self.recording_extractor.get_sampling_frequency())
+            nsx_to_load = None
+            self.file_path = Path(nsx_override)
         else:
-            from spikeinterface.extractors import OpenEphysBinaryRecordingExtractor
-
-            self.RX = OpenEphysBinaryRecordingExtractor
-            super().__init__(folder_path=folder_path, verbose=verbose)
+            assert "ns" in file_path.suffix, "file_path should be an nsx file"
+            nsx_to_load = int(file_path.suffix[-1])
+            self.file_path = file_path
 
-        if stub_test:
-            self.subset_channels = [0, 1]
-
-    def get_metadata(self):
-        """Auto-fill as much of the metadata as possible. Must comply with metadata schema."""
-        import pyopenephys
+        super().__init__(file_path=file_path, stream_id=str(nsx_to_load), verbose=verbose, es_key=es_key)
 
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
+        # Open file and extract headers
+        basic_header = parse_nsx_basic_header(self.source_data["file_path"])
+        if "TimeOrigin" in basic_header:
+            metadata["NWBFile"].update(session_start_time=basic_header["TimeOrigin"])
+        if "Comment" in basic_header:
+            metadata["NWBFile"].update(session_description=basic_header["Comment"])
 
-        folder_path = self.source_data["folder_path"]
-        fileobj = pyopenephys.File(foldername=folder_path)
-        session_start_time = fileobj.experiments[0].datetime
-
-        metadata["NWBFile"].update(session_start_time=session_start_time)
         return metadata
 
 
-class OpenEphysSortingInterface(BaseSortingExtractorInterface):
-    """Primary data interface class for converting OpenEphys spiking data."""
+class BlackrockSortingInterface(BaseSortingExtractorInterface):
+    """Primary data interface class for converting Blackrock spiking data."""
 
     @classmethod
-    def get_source_schema(cls):
-        """Compile input schema for the SortingExtractor."""
-        metadata_schema = get_schema_from_method_signature(
-            class_method=cls.__init__, exclude=["recording_id", "experiment_id"]
-        )
-        metadata_schema["properties"]["folder_path"].update(description="Path to directory containing OpenEphys files.")
-        metadata_schema["additionalProperties"] = False
+    def get_source_schema(cls) -> dict:
+        metadata_schema = get_schema_from_method_signature(method=cls.__init__)
+        metadata_schema["additionalProperties"] = True
+        metadata_schema["properties"]["file_path"].update(description="Path to Blackrock file.")
         return metadata_schema
 
-    def __init__(self, folder_path: FolderPathType, experiment_id: int = 0, recording_id: int = 0):
-        from spikeextractors import OpenEphysSortingExtractor
+    def __init__(self, file_path: FilePathType, sampling_frequency: float = None, verbose: bool = True):
+        """
+        Parameters
+        ----------
+        file_path : str, Path
+            The file path to the ``.nev`` data
+        sampling_frequency: float, optional
+            The sampling frequency for the sorting extractor. When the signal data is available (.ncs) those files will be
+        used to extract the frequency automatically. Otherwise, the sampling frequency needs to be specified for
+        this extractor to be initialized.
+        verbose : bool, default: True
+            Enables verbosity
+        """
+        super().__init__(file_path=file_path, sampling_frequency=sampling_frequency, verbose=verbose)
 
-        self.Extractor = OpenEphysSortingExtractor
-        super().__init__(folder_path=str(folder_path), experiment_id=experiment_id, recording_id=recording_id)
+    def get_metadata(self) -> dict:
+        metadata = super().get_metadata()
+        # Open file and extract headers
+        basic_header = parse_nev_basic_header(self.source_data["file_path"])
+        if "TimeOrigin" in basic_header:
+            session_start_time = basic_header["TimeOrigin"]
+            metadata["NWBFile"].update(session_start_time=session_start_time.strftime("%Y-%m-%dT%H:%M:%S"))
+        if "Comment" in basic_header:
+            metadata["NWBFile"].update(session_description=basic_header["Comment"])
+        return metadata
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,90 @@
-"""Authors: Cody Baker."""
 from pathlib import Path
-from typing import List, Optional
+from typing import List
 
 import numpy as np
-from pynwb import NWBFile
-from pynwb.ecephys import ElectricalSeries
 
-from .spikeglxdatainterface import SpikeGLXRecordingInterface
+from .spikeglx_utils import get_device_metadata, get_session_start_time
+from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
 from ....tools.signal_processing import get_rising_frames_from_ttl
-from ....utils import get_schema_from_method_signature, get_schema_from_hdmf_class, FilePathType
+from ....utils import FilePathType, get_schema_from_method_signature
 
 
-class SpikeGLXNIDQInterface(SpikeGLXRecordingInterface):
+class SpikeGLXNIDQInterface(BaseRecordingExtractorInterface):
     """Primary data interface class for converting the high-pass (ap) SpikeGLX format."""
 
     ExtractorName = "SpikeGLXRecordingExtractor"
 
     @classmethod
-    def get_source_schema(cls):
-        source_schema = get_schema_from_method_signature(class_method=cls.__init__, exclude=["x_pitch", "y_pitch"])
+    def get_source_schema(cls) -> dict:
+        source_schema = get_schema_from_method_signature(method=cls.__init__, exclude=["x_pitch", "y_pitch"])
         source_schema["properties"]["file_path"]["description"] = "Path to SpikeGLX .nidq file."
         return source_schema
 
     def __init__(
-        self, file_path: FilePathType, stub_test: bool = False, verbose: bool = True, load_sync_channel: bool = False
+        self,
+        file_path: FilePathType,
+        verbose: bool = True,
+        load_sync_channel: bool = False,
+        es_key: str = "ElectricalSeriesNIDQ",
     ):
         """
         Read channel data from the NIDQ board for the SpikeGLX recording.
 
         Useful for synchronizing multiple data streams into the common time basis of the SpikeGLX system.
 
         Parameters
         ----------
         file_path : FilePathType
             Path to .nidq.bin file.
-        stub_test : bool, default: False
-            Whether to shorten file for testing purposes.
         verbose : bool, default: True
             Whether to output verbose text.
         load_sync_channel : bool, default: False
-            Whether or not to load the last channel in the stream, which is typically used for synchronization.
+            Whether to load the last channel in the stream, which is typically used for synchronization.
             If True, then the probe is not loaded.
+        es_key : str, default: "ElectricalSeriesNIDQ"
         """
-        self.stream_id = "nidq"
 
         folder_path = Path(file_path).parent
-        super(SpikeGLXRecordingInterface, self).__init__(
+        super().__init__(
             folder_path=folder_path,
-            stream_id=self.stream_id,
+            stream_id="nidq",
             verbose=verbose,
             load_sync_channel=load_sync_channel,
+            es_key=es_key,
         )
         self.source_data.update(file_path=str(file_path))
 
         self.recording_extractor.set_property(
             key="group_name", values=["NIDQChannelGroup"] * self.recording_extractor.get_num_channels()
         )
-        self.meta = self.recording_extractor.neo_reader.signals_info_dict[(0, self.stream_id)]["meta"]
-
-    def get_metadata_schema(self):
-        metadata_schema = super().get_metadata_schema()
-        metadata_schema["properties"]["Ecephys"]["properties"].update(
-            ElectricalSeriesNIDQ=get_schema_from_hdmf_class(ElectricalSeries)
-        )
-        return metadata_schema
+        self.meta = self.recording_extractor.neo_reader.signals_info_dict[(0, "nidq")]["meta"]
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
 
-        metadata["Ecephys"]["ElectrodeGroup"][0]["description"] = "A group representing the NIDQ channels."
+        session_start_time = get_session_start_time(self.meta)
+        if session_start_time:
+            metadata["NWBFile"]["session_start_time"] = session_start_time
+
+        # Device metadata
+        device = get_device_metadata(self.meta)
+
+        # Add groups metadata
+        metadata["Ecephys"]["Device"] = [device]
+
+        metadata["Ecephys"]["ElectrodeGroup"][0].update(
+            name="NIDQChannelGroup", description="A group representing the NIDQ channels.", device=device["name"]
+        )
         metadata["Ecephys"]["Electrodes"] = [
             dict(name="group_name", description="Name of the ElectrodeGroup this electrode is a part of."),
         ]
-        metadata["Ecephys"].pop("ElectricalSeriesRaw")
-        metadata["Ecephys"]["ElectricalSeriesNIDQ"] = dict(
-            name="ElectricalSeriesNIDQ", description="Raw acquisition traces from the NIDQ (.nidq.bin) channels."
-        )
+        metadata["Ecephys"]["ElectricalSeriesNIDQ"][
+            "description"
+        ] = "Raw acquisition traces from the NIDQ (.nidq.bin) channels."
         return metadata
 
     def get_channel_names(self) -> List[str]:
         """Return a list of channel names as set in the recording extractor."""
         return list(self.recording_extractor.get_channel_ids())
 
     def get_event_times_from_ttl(self, channel_name: str) -> np.ndarray:
@@ -101,43 +106,7 @@
             trace=self.recording_extractor.get_traces(channel_ids=[channel_name])
         )
 
         nidq_timestamps = self.recording_extractor.get_times()
         rising_times = nidq_timestamps[rising_frames]
 
         return rising_times
-
-    def get_conversion_options(self) -> dict:
-        # Currently this method is only used by NWBConverter classes
-        # We still need a similar override for run_conversion default es_key for stand-alone interface conversion
-        conversion_options = dict(write_as="raw", es_key="ElectricalSeriesNIDQ")
-        return conversion_options
-
-    def run_conversion(
-        self,
-        nwbfile_path: Optional[FilePathType] = None,
-        nwbfile: Optional[NWBFile] = None,
-        metadata: Optional[dict] = None,
-        overwrite: bool = False,
-        stub_test: bool = False,
-        write_as: Optional[str] = None,
-        write_electrical_series: bool = True,
-        es_key: str = None,
-        compression: Optional[str] = None,
-        compression_opts: Optional[int] = None,
-        iterator_type: str = "v2",
-        iterator_opts: Optional[dict] = None,
-    ):
-        super().run_conversion(
-            nwbfile_path=nwbfile_path,
-            nwbfile=nwbfile,
-            metadata=metadata,
-            overwrite=overwrite,
-            stub_test=stub_test,
-            write_as=write_as,
-            write_electrical_series=write_electrical_series,
-            es_key=es_key or "ElectricalSeriesNIDQ",
-            compression=compression,
-            compression_opts=compression_opts,
-            iterator_type=iterator_type,
-            iterator_opts=iterator_opts,
-        )
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/spikeinterface/sipickledatainterfaces.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-"""Authors: Alessio Buccino."""
-from warnings import warn
-
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
 from ..basesortingextractorinterface import BaseSortingExtractorInterface
-from ....utils import FilePathType
+from ....utils.types import FilePathType
 
 
-class SIPickleRecordingInterface(BaseRecordingExtractorInterface):
-    """Primary interface for reading and converting SpikeInterface Recording objects through .pkl files."""
+class PlexonRecordingInterface(BaseRecordingExtractorInterface):
+    """
+    Primary data interface class for converting Plexon data.
 
-    ExtractorModuleName = "spikeextractors"
-    ExtractorName = "load_extractor_from_pickle"
+    Uses the :py:class:`~spikeinterface.extractors.PlexonRecordingExtractor`.
+    """
 
-    def __init__(self, file_path: FilePathType, verbose: bool = True):
+    def __init__(self, file_path: FilePathType, verbose: bool = True, es_key: str = "ElectricalSeries"):
         """
-        Initialize reading of SpikeInterface Pickle files.
+        Load and prepare data for Plexon.
 
         Parameters
         ----------
-        file_path : FilePathType
-            Path to .pkl file.
-        verbose : bool, optional, default=True
+        file_path : str or Path
+            Path to the .plx file.
+        verbose : bool, default: True
+            Allows verbosity.
+        es_key : str, default: "ElectricalSeries"
         """
-        # TODO: Remove entire interfaces
-        warn(
-            message=(
-                "Interfaces using a spikeextractors backend will soon be deprecated! "
-                "Please use the SpikeInterface backend instead."
-            ),
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-
-        from spikeextractors import load_extractor_from_pickle
-
-        self.recording_extractor = load_extractor_from_pickle(pkl_file=file_path)
-        self.subset_channels = None
-        self.source_data = dict(file_path=file_path)
-        self.verbose = verbose
-        self.es_key = None
+        super().__init__(file_path=file_path, verbose=verbose, es_key=es_key)
 
 
-class SIPickleSortingInterface(BaseSortingExtractorInterface):
-    """Primary interface for reading and converting SpikeInterface Sorting objects through .pkl files."""
+class PlexonSortingInterface(BaseSortingExtractorInterface):
+    """
+    Primary data interface class for converting Plexon spiking data.
 
-    ExtractorModuleName = "spikeextractors"
-    ExtractorName = "load_extractor_from_pickle"
+    Uses :py:class:`~spikeinterface.extractors.PlexonSortingExtractor`.
+    """
 
     def __init__(self, file_path: FilePathType, verbose: bool = True):
-        from spikeextractors import load_extractor_from_pickle
+        """
+        Load and prepare data for Plexon.
+
+        Parameters
+        ----------
+        file_path: FilePathType
+            Path to the plexon spiking data (.plx file).
+        verbose: bool, default: True
+            Allows verbosity.
+        """
+        super().__init__(file_path=file_path, verbose=verbose)
+
+    def get_metadata(self) -> dict:
+        metadata = super().get_metadata()
+        neo_reader = self.sorting_extractor.neo_reader
+
+        if hasattr(neo_reader, "raw_annotations"):
+            block_ind = self.sorting_extractor.block_index
+            neo_metadata = neo_reader.raw_annotations["blocks"][block_ind]
+
+            if "rec_datetime" in neo_metadata:
+                metadata["NWBFile"].update(session_start_time=neo_metadata["rec_datetime"])
 
-        self.sorting_extractor = load_extractor_from_pickle(pkl_file=file_path)
-        self.source_data = dict(file_path=file_path)
-        self.verbose = verbose
+        return metadata
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-"""Author: Heberto Mayorquin"""
 from ..baserecordingextractorinterface import BaseRecordingExtractorInterface
-
 from ....utils.types import FolderPathType
 
 
 class TdtRecordingInterface(BaseRecordingExtractorInterface):
     """Primary data interface class for converting Tucker-Davis Technologies (TDT) data."""
 
-    def __init__(self, folder_path: FolderPathType, stream_id: str = "0", verbose: bool = True):
+    def __init__(
+        self, folder_path: FolderPathType, stream_id: str = "0", verbose: bool = True, es_key: str = "ElectricalSeries"
+    ):
         """
         Initialize reading of a TDT recording.
 
         Parameters
         ----------
         folder_path : str or Path
             Path to the directory with the corresponding files (TSQ, TBK, TEV, SEV)
         stream_id : str, "0" by default
             Select from multiple streams.
         verbose : bool, default: True
             Allows verbose.
+        es_key : str, optional
+
 
         Notes
         -----
         Stream "0" corresponds to LFP for gin data. Other streams seem non-electrical.
         """
-
         super().__init__(
             folder_path=folder_path,
             stream_id=stream_id,
             verbose=verbose,
+            es_key=es_key,
         )
 
         # Fix channel name format
         channel_names = self.recording_extractor.get_property("channel_name")
         channel_names = [name.replace("'", "")[1:] for name in channel_names]
         self.recording_extractor.set_property(key="channel_name", values=channel_names)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Author: Luiz Tauffer."""
 from typing import Optional, Tuple
 from warnings import warn
 
-from pynwb import NWBFile, NWBHDF5IO
+import numpy as np
+from pynwb import NWBHDF5IO, NWBFile
 
 from ...baseextractorinterface import BaseExtractorInterface
 from ...tools.nwb_helpers import make_nwbfile_from_metadata
 from ...utils import (
     FilePathType,
+    get_metadata_schema_for_icephys,
     get_schema_from_hdmf_class,
     get_schema_from_method_signature,
-    get_metadata_schema_for_icephys,
 )
 
-
 try:
     from ndx_dandi_icephys import DandiIcephysMetadata
 
     HAVE_NDX_DANDI_ICEPHYS = True
 except ImportError:
     DandiIcephysMetadata = None
     HAVE_NDX_DANDI_ICEPHYS = False
@@ -25,31 +24,33 @@
 
 class BaseIcephysInterface(BaseExtractorInterface):
     """Primary class for all intracellular NeoInterfaces."""
 
     ExtractorModuleName = "neo"
 
     @classmethod
-    def get_source_schema(cls):
-        source_schema = get_schema_from_method_signature(class_method=cls.__init__, exclude=[])
+    def get_source_schema(cls) -> dict:
+        source_schema = get_schema_from_method_signature(method=cls.__init__, exclude=[])
         return source_schema
 
     def __init__(self, file_paths: list):
         from ...tools.neo import get_number_of_electrodes, get_number_of_segments
 
         super().__init__(file_paths=file_paths)
 
         self.readers_list = list()
         for f in file_paths:
-            self.readers_list.append(self.Extractor(filename=f))
+            self.readers_list.append(self.get_extractor()(filename=f))
 
         self.subset_channels = None
         self.n_segments = get_number_of_segments(neo_reader=self.readers_list[0], block=0)
         self.n_channels = get_number_of_electrodes(neo_reader=self.readers_list[0])
 
+        self._timestamps = None
+
     def get_metadata_schema(self) -> dict:
         metadata_schema = super().get_metadata_schema()
         if DandiIcephysMetadata:
             metadata_schema["properties"]["ndx-dandi-icephys"] = get_schema_from_hdmf_class(DandiIcephysMetadata)
         metadata_schema["properties"]["Icephys"] = get_metadata_schema_for_icephys()
         return metadata_schema
 
@@ -62,14 +63,29 @@
             Electrode=[
                 dict(name=f"electrode-{i}", description="no description", device="DeviceIcephys")
                 for i in range(get_number_of_electrodes(self.readers_list[0]))
             ],
         )
         return metadata
 
+    def get_original_timestamps(self) -> np.ndarray:
+        raise NotImplementedError("Icephys interfaces do not yet support timestamps.")
+
+    def get_timestamps(self) -> np.ndarray:
+        raise NotImplementedError("Icephys interfaces do not yet support timestamps.")
+
+    def set_aligned_timestamps(self, aligned_timestamps: np.ndarray):
+        raise NotImplementedError("Icephys interfaces do not yet support timestamps.")
+
+    def set_aligned_starting_time(self, aligned_starting_time: float):
+        raise NotImplementedError("This icephys interface has not specified the method for aligning starting time.")
+
+    def align_by_interpolation(self, unaligned_timestamps: np.ndarray, aligned_timestamps: np.ndarray):
+        raise NotImplementedError("Icephys interfaces do not yet support timestamps.")
+
     def run_conversion(
         self,
         nwbfile: NWBFile = None,
         nwbfile_path: Optional[FilePathType] = None,
         metadata: dict = None,
         overwrite: bool = False,
         icephys_experiment_type: str = "voltage_clamp",
@@ -91,14 +107,15 @@
             metadata info for constructing the nwb file (optional).
         overwrite : bool, default: False
             Whether to overwrite the NWB file if one exists at the nwbfile_path.
         icephys_experiment_type : {'voltage_clamp', 'current_clamp', 'izero'}
             Type of icephys recording.
         skip_electrodes : tuple, optional
             Electrode IDs to skip. Defaults to ().
+        save_path: string, optional
         """
         from ...tools.neo import write_neo_to_nwb
 
         if nwbfile is None:
             nwbfile = make_nwbfile_from_metadata(metadata)
 
         # TODO on or after August 1st, 2022, remove argument and deprecation warnings
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Author: Ben Dichter."""
 from typing import Optional
 
+import numpy as np
 from pynwb import NWBFile
 from pynwb.device import Device
 from pynwb.ophys import ImagingPlane, TwoPhotonSeries
 
 from ...baseextractorinterface import BaseExtractorInterface
 from ...utils import (
-    get_schema_from_hdmf_class,
-    fill_defaults,
-    get_base_schema,
     OptionalFilePathType,
     dict_deep_update,
+    fill_defaults,
+    get_base_schema,
+    get_schema_from_hdmf_class,
 )
 
 
 class BaseImagingExtractorInterface(BaseExtractorInterface):
     """Parent class for all ImagingExtractorInterfaces."""
 
-    ExtractorModuleName: Optional[str] = "roiextractors"
+    ExtractorModuleName = "roiextractors"
 
     def __init__(self, verbose: bool = True, **source_data):
         super().__init__(**source_data)
-        self.imaging_extractor = self.Extractor(**source_data)
+        self.imaging_extractor = self.get_extractor()(**source_data)
         self.verbose = verbose
 
-    def get_metadata_schema(self):
+    def get_metadata_schema(self) -> dict:
         metadata_schema = super().get_metadata_schema()
 
         metadata_schema["required"] = ["Ophys"]
 
         # Initiate Ophys metadata
         metadata_schema["properties"]["Ophys"] = get_base_schema(tag="Ophys")
         metadata_schema["properties"]["Ophys"]["required"] = ["Device", "ImagingPlane", "TwoPhotonSeries"]
@@ -52,15 +53,15 @@
             ImagingPlane=imaging_plane_schema,
             TwoPhotonSeries=get_schema_from_hdmf_class(TwoPhotonSeries),
         )
 
         fill_defaults(metadata_schema, self.get_metadata())
         return metadata_schema
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         from ...tools.roiextractors import get_nwb_imaging_metadata
 
         metadata = super().get_metadata()
         default_metadata = get_nwb_imaging_metadata(self.imaging_extractor)
         metadata = dict_deep_update(default_metadata, metadata)
 
         # fix troublesome data types
@@ -68,14 +69,24 @@
             for two_photon_series in metadata["Ophys"]["TwoPhotonSeries"]:
                 if "dimension" in two_photon_series:
                     two_photon_series["dimension"] = list(two_photon_series["dimension"])
                 if "rate" in two_photon_series:
                     two_photon_series["rate"] = float(two_photon_series["rate"])
         return metadata
 
+    def get_original_timestamps(self) -> np.ndarray:
+        reinitialized_extractor = self.get_extractor()(**self.source_data)
+        return reinitialized_extractor.frame_to_time(frames=np.arange(stop=reinitialized_extractor.get_num_frames()))
+
+    def get_timestamps(self) -> np.ndarray:
+        return self.imaging_extractor.frame_to_time(frames=np.arange(stop=self.imaging_extractor.get_num_frames()))
+
+    def set_aligned_timestamps(self, aligned_timestamps: np.ndarray):
+        self.imaging_extractor.set_times(times=aligned_timestamps)
+
     def run_conversion(
         self,
         nwbfile_path: OptionalFilePathType = None,
         nwbfile: Optional[NWBFile] = None,
         metadata: Optional[dict] = None,
         overwrite: bool = False,
         stub_test: bool = False,
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..baseimagingextractorinterface import BaseImagingExtractorInterface
-from ....utils import FilePathType, ArrayType
+from ....utils import ArrayType, FilePathType
 
 
 class Hdf5ImagingInterface(BaseImagingExtractorInterface):
     """Data Interface for Hdf5ImagingExtractor."""
 
     def __init__(
         self,
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,11 +13,11 @@
             Path to .sbx file.
         sampling_frequency : float, optional
         verbose : bool, default: True
         """
 
         super().__init__(file_path=file_path, sampling_frequency=sampling_frequency, verbose=verbose)
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         metadata = super().get_metadata()
         metadata["Ophys"]["Device"][0]["description"] = "Scanbox imaging"
         return metadata
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+import datetime
 import json
-from dateutil.parser import parse as dateparse
 from typing import Optional
 
+from dateutil.parser import parse as dateparse
+
 from ..baseimagingextractorinterface import BaseImagingExtractorInterface
 from ....tools import get_package
 from ....utils import FilePathType
 
 
-def extract_extra_metadata(file_path):
+def extract_extra_metadata(file_path) -> dict:
     ScanImageTiffReader = get_package(
         package_name="ScanImageTiffReader", installation_instructions="pip install scanimage-tiff-reader"
     )
-
-    description = ScanImageTiffReader.ScanImageTiffReader(str(file_path)).description(iframe=0)
-    extra_metadata = {x.split("=")[0]: x.split("=")[1] for x in description.split("\r") if "=" in x}
-
+    src_file = ScanImageTiffReader.ScanImageTiffReader(str(file_path))
+    extra_metadata = {}
+    for metadata_string in (src_file.description(iframe=0), src_file.metadata()):
+        metadata_dict = {
+            x.split("=")[0].strip(): x.split("=")[1].strip()
+            for x in metadata_string.replace("\n", "\r").split("\r")
+            if "=" in x
+        }
+        extra_metadata = dict(**extra_metadata, **metadata_dict)
     return extra_metadata
 
 
 class ScanImageImagingInterface(BaseImagingExtractorInterface):
     ExtractorName = "ScanImageTiffImagingExtractor"
 
     @classmethod
-    def get_source_schema(cls):
+    def get_source_schema(cls) -> dict:
         source_schema = super().get_source_schema()
         source_schema["properties"]["file_path"]["description"] = "Path to Tiff file."
         return source_schema
 
     def __init__(
         self,
         file_path: FilePathType,
@@ -45,32 +52,42 @@
             The sampling frequency can usually be extracted from the scanimage metadata in
             exif:ImageDescription:state.acq.frameRate. If not, use this.
         """
         self.image_metadata = extract_extra_metadata(file_path=file_path)
 
         if "state.acq.frameRate" in self.image_metadata:
             sampling_frequency = float(self.image_metadata["state.acq.frameRate"])
+        elif "SI.hRoiManager.scanFrameRate" in self.image_metadata:
+            sampling_frequency = float(self.image_metadata["SI.hRoiManager.scanFrameRate"])
         else:
             assert_msg = (
                 "sampling frequency not found in image metadata, "
                 "input the frequency using the argument `fallback_sampling_frequency`"
             )
             assert fallback_sampling_frequency is not None, assert_msg
             sampling_frequency = fallback_sampling_frequency
 
         super().__init__(file_path=file_path, sampling_frequency=sampling_frequency, verbose=verbose)
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         device_number = 0  # Imaging plane metadata is a list with metadata for each plane
 
         metadata = super().get_metadata()
 
         if "state.internal.triggerTimeString" in self.image_metadata:
             extracted_session_start_time = dateparse(self.image_metadata["state.internal.triggerTimeString"])
             metadata["NWBFile"].update(session_start_time=extracted_session_start_time)
+        elif "epoch" in self.image_metadata:
+            # Versions of ScanImage at least as recent as 2020, and possibly earlier, store the start time under keyword
+            # `epoch`, as a string encoding of a Matlab array, example `'[2022  8  8 16 56 7.329]'`
+            # dateparse can't cope with this representation, so using strptime directly
+            extracted_session_start_time = datetime.datetime.strptime(
+                self.image_metadata["epoch"], "[%Y %m %d %H %M %S.%f]"
+            )
+            metadata["NWBFile"].update(session_start_time=extracted_session_start_time)
 
         # Extract many scan image properties and attach them as dic in the description
         ophys_metadata = metadata["Ophys"]
         two_photon_series_metadata = ophys_metadata["TwoPhotonSeries"][device_number]
         if self.image_metadata is not None:
             extracted_description = json.dumps(self.image_metadata)
             two_photon_series_metadata.update(description=extracted_description)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py` & `neuroconv-0.3.0/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ....utils import FilePathType
 
 
 class TiffImagingInterface(BaseImagingExtractorInterface):
     """Data Interface for TiffImagingExtractor."""
 
     @classmethod
-    def get_source_schema(cls):
+    def get_source_schema(cls) -> dict:
         source_schema = super().get_source_schema()
         source_schema["properties"]["file_path"]["description"] = "Path to Tiff file."
         return source_schema
 
     def __init__(self, file_path: FilePathType, sampling_frequency: float, verbose: bool = True):
         """
         Initialize reading of TIFF file.
```

### Comparing `neuroconv-0.2.4/src/neuroconv/nwbconverter.py` & `neuroconv-0.3.0/src/neuroconv/nwbconverter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-"""Authors: Cody Baker and Ben Dichter."""
 import json
-from jsonschema import validate
-from typing import Optional, Dict, List, Union
 from collections import Counter
 from pathlib import Path
+from typing import Dict, List, Optional, Union
 
+from jsonschema import validate
 from pynwb import NWBFile
-from pynwb.file import Subject
 
-from .tools.nwb_helpers import get_default_nwbfile_metadata, make_nwbfile_from_metadata, make_or_load_nwbfile
+from .basedatainterface import BaseDataInterface
+from .tools.nwb_helpers import get_default_nwbfile_metadata, make_or_load_nwbfile
 from .utils import (
-    get_schema_from_hdmf_class,
-    get_schema_for_NWBFile,
     dict_deep_update,
+    fill_defaults,
     get_base_schema,
+    load_dict_from_file,
     unroot_schema,
-    fill_defaults,
 )
-from .basedatainterface import BaseDataInterface
+from .utils.dict import DeepDict
 from .utils.json_schema import NWBMetaDataEncoder
 
 
 class NWBConverter:
     """Primary class for all NWB conversion classes."""
 
     data_interface_classes = None
@@ -36,25 +34,24 @@
             description="Schema for the source data, files and directories",
             version="0.1.0",
         )
         for interface_name, data_interface in cls.data_interface_classes.items():
             source_schema["properties"].update({interface_name: unroot_schema(data_interface.get_source_schema())})
         return source_schema
 
-    @classmethod
-    def get_conversion_options_schema(cls):
+    def get_conversion_options_schema(self):
         """Compile conversion option schemas from each of the data interface classes."""
         conversion_options_schema = get_base_schema(
             root=True,
             id_="conversion_options.schema.json",
             title="Conversion options schema",
             description="Schema for the conversion options",
             version="0.1.0",
         )
-        for interface_name, data_interface in cls.data_interface_classes.items():
+        for interface_name, data_interface in self.data_interface_objects.items():
             conversion_options_schema["properties"].update(
                 {interface_name: unroot_schema(data_interface.get_conversion_options_schema())}
             )
         return conversion_options_schema
 
     @classmethod
     def validate_source(cls, source_data: Dict[str, dict], verbose: bool = True):
@@ -69,46 +66,31 @@
             name: data_interface(**source_data[name])
             for name, data_interface in self.data_interface_classes.items()
             if name in source_data
         }
 
     def get_metadata_schema(self):
         """Compile metadata schemas from each of the data interface objects."""
-        metadata_schema = get_base_schema(
-            id_="metadata.schema.json",
-            root=True,
-            title="Metadata",
-            description="Schema for the metadata",
-            version="0.1.0",
-            required=["NWBFile"],
-            properties=dict(NWBFile=get_schema_for_NWBFile(), Subject=get_schema_from_hdmf_class(Subject)),
-        )
+        metadata_schema = load_dict_from_file(Path(__file__).parent / "schemas" / "base_metadata_schema.json")
         for data_interface in self.data_interface_objects.values():
             interface_schema = unroot_schema(data_interface.get_metadata_schema())
             metadata_schema = dict_deep_update(metadata_schema, interface_schema)
 
         default_values = self.get_metadata()
         fill_defaults(metadata_schema, default_values)
         return metadata_schema
 
-    def get_metadata(self):
+    def get_metadata(self) -> DeepDict:
         """Auto-fill as much of the metadata as possible. Must comply with metadata schema."""
         metadata = get_default_nwbfile_metadata()
         for interface in self.data_interface_objects.values():
             interface_metadata = interface.get_metadata()
             metadata = dict_deep_update(metadata, interface_metadata)
         return metadata
 
-    def get_conversion_options(self):
-        """Auto-fill as much of the conversion options as possible. Must comply with conversion_options_schema."""
-        conversion_options = dict()
-        for interface_name, interface in self.data_interface_objects.items():
-            conversion_options[interface_name] = interface.get_conversion_options()
-        return conversion_options
-
     def validate_metadata(self, metadata: Dict[str, dict]):
         """Validate metadata against Converter metadata_schema."""
         encoder = NWBMetaDataEncoder()
         # The encoder produces a serialiazed object so we de serialized it for comparison
         serialized_metadata = encoder.encode(metadata)
         decoded_metadata = json.loads(serialized_metadata)
         validate(instance=decoded_metadata, schema=self.get_metadata_schema())
@@ -134,55 +116,51 @@
         overwrite: bool = False,
         conversion_options: Optional[dict] = None,
     ) -> NWBFile:
         """
         Run the NWB conversion over all the instantiated data interfaces.
         Parameters
         ----------
-        nwbfile_path: FilePathType
+        nwbfile_path : FilePathType
             Path for where to write or load (if overwrite=False) the NWBFile.
             If specified, the context will always write to this location.
-        nwbfile: NWBFile, optional
+        nwbfile : NWBFile, optional
             An in-memory NWBFile object to write to the location.
-        metadata: dict, optional
+        metadata : dict, optional
             Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
-        overwrite: bool, optional
-            Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
+        overwrite : bool, default: False
+            Whether to overwrite the NWBFile if one exists at the nwbfile_path.
             The default is False (append mode).
-        verbose: bool, optional
-            If 'nwbfile_path' is specified, informs user after a successful write operation.
-            The default is True.
-        conversion_options: dict, optional
+        conversion_options : dict, optional
             Similar to source_data, a dictionary containing keywords for each interface for which non-default
             conversion specification is requested.
         Returns
         -------
         nwbfile: NWBFile
             The in-memory NWBFile object after all conversion operations are complete.
         """
         if metadata is None:
             metadata = self.get_metadata()
         self.validate_metadata(metadata=metadata)
 
         if conversion_options is None:
             conversion_options = dict()
-        default_conversion_options = self.get_conversion_options()
-        conversion_options_to_run = dict_deep_update(default_conversion_options, conversion_options)
-        self.validate_conversion_options(conversion_options=conversion_options_to_run)
+
+        self.validate_conversion_options(conversion_options=conversion_options)
 
         with make_or_load_nwbfile(
             nwbfile_path=nwbfile_path,
             nwbfile=nwbfile,
             metadata=metadata,
             overwrite=overwrite,
             verbose=self.verbose,
         ) as nwbfile_out:
             for interface_name, data_interface in self.data_interface_objects.items():
                 data_interface.run_conversion(
-                    nwbfile=nwbfile_out, metadata=metadata, **conversion_options_to_run.get(interface_name, dict())
+                    nwbfile=nwbfile_out, metadata=metadata, **conversion_options.get(interface_name, dict())
                 )
 
         return nwbfile_out
 
 
 class ConverterPipe(NWBConverter):
     """Takes a list or dict of pre-initialized interfaces as arguments to build an NWBConverter class"""
@@ -192,25 +170,25 @@
         conversion_options_schema = get_base_schema(
             root=True,
             id_="conversion_options.schema.json",
             title="Conversion options schema",
             description="Schema for the conversion options",
             version="0.1.0",
         )
-        for interface_name, data_interface in self.data_interface_classes.items():
+        for interface_name, data_interface in self.data_interface_objects.items():
             conversion_options_schema["properties"].update(
                 {interface_name: unroot_schema(data_interface.get_conversion_options_schema())}
             )
         return conversion_options_schema
 
     def get_source_schema(self):
-        raise NotImplementedError("Source data not available with previously intialized classes")
+        raise NotImplementedError("Source data not available with previously initialized classes")
 
     def validate_source(self):
-        raise NotImplementedError("Source data not available with previously intialized classes")
+        raise NotImplementedError("Source data not available with previously initialized classes")
 
     def __init__(self, data_interfaces: Union[List[BaseDataInterface], Dict[str, BaseDataInterface]], verbose=True):
         self.verbose = verbose
         if isinstance(data_interfaces, list):
             # Create unique names for each interface
             counter = {interface.__class__.__name__: 0 for interface in data_interfaces}
             total_counts = Counter([interface.__class__.__name__ for interface in data_interfaces])
```

### Comparing `neuroconv-0.2.4/src/neuroconv/schemas/metadata_schema.json` & `neuroconv-0.3.0/src/neuroconv/schemas/metadata_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998809523809523%*

 * *Differences: {"'properties'": "{'Ophys': {'properties': {'OnePhotonSeries': OrderedDict([('type', 'array'), "*

 * *                 "('items', OrderedDict([('title', 'OnePhotonSeries'), ('type', 'object'), "*

 * *                 "('required', ['name', 'description']), ('properties', OrderedDict([('name', "*

 * *                 "OrderedDict([('type', 'string'), ('default', 'OnePhotonSeries')])), "*

 * *                 "('description', OrderedDict([('type', 'string')])), ('imaging_plane', "*

 * *                 "OrderedDict([('type', 'string' […]*

```diff
@@ -416,14 +416,37 @@
                             "description"
                         ],
                         "title": "ImagingPlane",
                         "type": "object"
                     },
                     "type": "array"
                 },
+                "OnePhotonSeries": {
+                    "items": {
+                        "properties": {
+                            "description": {
+                                "type": "string"
+                            },
+                            "imaging_plane": {
+                                "type": "string"
+                            },
+                            "name": {
+                                "default": "OnePhotonSeries",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "name",
+                            "description"
+                        ],
+                        "title": "OnePhotonSeries",
+                        "type": "object"
+                    },
+                    "type": "array"
+                },
                 "TwoPhotonSeries": {
                     "items": {
                         "properties": {
                             "description": {
                                 "type": "string"
                             },
                             "imaging_plane": {
```

### Comparing `neuroconv-0.2.4/src/neuroconv/schemas/source_schema.json` & `neuroconv-0.3.0/src/neuroconv/schemas/source_schema.json`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/schemas/yaml_conversion_specification_schema.json` & `neuroconv-0.3.0/src/neuroconv/schemas/yaml_conversion_specification_schema.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6927351518110796%*

 * *Differences: {"'additionalProperties'": 'False',*

 * * "'properties'": "{'experiments': {'additionalProperties': {'properties': {'sessions': {'items': "*

 * *                 "{'properties': {'metadata': OrderedDict([('$ref', './metadata_schema.json#')]), "*

 * *                 "'conversion_options': OrderedDict([('type', 'object')])}, delete: ['allOf']}}, "*

 * *                 "'metadata': OrderedDict([('$ref', './metadata_schema.json#')])}, delete: "*

 * *                 "['allOf']}}, 'metadata': OrderedDict([('$ref', './metadata_schema.j […]*

```diff
@@ -1,53 +1,37 @@
 {
-    "$defs": {
-        "level": {
-            "properties": {
-                "conversion_options": {
-                    "type": "object"
-                },
-                "data_interfaces": {
-                    "items": {
-                        "title": "DataInterface",
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
-                "metadata": {
-                    "$ref": "./metadata_schema.json#"
-                }
-            },
-            "type": "object"
-        }
-    },
     "$id": "yaml_conversion_specification_schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "allOf": [
-        {
-            "$ref": "#/$defs/level"
-        }
-    ],
+    "additionalProperties": false,
     "description": "Schema for a NWB conversion specified by a YAML file.",
     "properties": {
+        "conversion_options": {
+            "type": "object"
+        },
+        "data_interfaces": {
+            "additionalProperties": {
+                "type": "string"
+            },
+            "type": "object"
+        },
         "experiments": {
             "additionalProperties": {
-                "allOf": [
-                    {
-                        "$ref": "#/$defs/level"
-                    }
-                ],
                 "properties": {
+                    "metadata": {
+                        "$ref": "./metadata_schema.json#"
+                    },
                     "sessions": {
                         "items": {
-                            "allOf": [
-                                {
-                                    "$ref": "#/$defs/level"
-                                }
-                            ],
                             "properties": {
+                                "conversion_options": {
+                                    "type": "object"
+                                },
+                                "metadata": {
+                                    "$ref": "./metadata_schema.json#"
+                                },
                                 "nwbfile_name": {
                                     "type": "string"
                                 },
                                 "source_data": {
                                     "type": "object"
                                 }
                             },
@@ -62,14 +46,17 @@
                 },
                 "required": [
                     "sessions"
                 ],
                 "type": "object"
             },
             "type": "object"
+        },
+        "metadata": {
+            "$ref": "./metadata_schema.json#"
         }
     },
     "required": [
         "experiments"
     ],
     "title": "YAML conversion specification schema",
     "type": "object",
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/audio/audio.py` & `neuroconv-0.3.0/src/neuroconv/tools/audio/audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import Optional
+from typing import Literal, Optional
 from warnings import warn
 
 from hdmf.backends.hdf5 import H5DataIO
-from ndx_sound import AcousticWaveformSeries
 from pynwb import NWBFile
 
 from neuroconv.tools.hdmf import SliceableDataChunkIterator
 from neuroconv.utils import ArrayType
 
 
 def add_acoustic_waveform_series(
     acoustic_series: ArrayType,
     nwbfile: NWBFile,
     rate: float,
     metadata: dict,
     starting_time: float = 0.0,
-    write_as: str = "stimulus",
+    write_as: Literal["stimulus", "acquisition"] = "stimulus",
     iterator_options: Optional[dict] = None,
     compression_options: Optional[dict] = None,
 ) -> NWBFile:
     """
 
     Adds the audio and its metadata to the NWB file either as stimulus or acquisition.
     The neurodata type that is used is an AcousticWaveformSeries object which holds a
@@ -46,14 +45,16 @@
     compression_options : dict, optional
         Dictionary of options for compressing the data for H5DataIO.
 
     Returns
     -------
         The nwbfile passed as an input with the AcousticWaveformSeries added.
     """
+    from ndx_sound import AcousticWaveformSeries
+
     assert write_as in [
         "stimulus",
         "acquisition",
     ], "Acoustic series can be written either as 'stimulus' or 'acquisition'."
 
     compression_options = compression_options or dict(compression="gzip")
     iterator_options = iterator_options or dict()
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/data_transfers.py` & `neuroconv-0.3.0/src/neuroconv/tools/data_transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,35 @@
 """Collection of helper functions for assessing and performing automated data transfers."""
-import os
-import subprocess
 import json
+import os
 import re
-from typing import Dict, Optional, List, Union, Tuple
 from pathlib import Path
-from warnings import warn
 from shutil import rmtree
-from time import sleep, time
 from tempfile import mkdtemp
+from time import sleep, time
+from typing import Dict, List, Tuple, Union
+from warnings import warn
 
-import psutil
-from tqdm import tqdm
-from pynwb import NWBHDF5IO
 from dandi.download import download as dandi_download
 from dandi.organize import organize as dandi_organize
 from dandi.upload import upload as dandi_upload
+from pynwb import NWBHDF5IO
+from tqdm import tqdm
 
+from .processes import deploy_process
 from ..utils import FolderPathType, OptionalFolderPathType
 
 try:  # pragma: no cover
     import globus_cli
 
     HAVE_GLOBUS = True
 except ModuleNotFoundError:
     HAVE_GLOBUS = False
 
 
-def _kill_process(proc):
-    """Private helper for ensuring a process and any subprocesses are properly terminated after a timeout period."""
-    try:
-        process = psutil.Process(proc.pid)
-        for proc in process.children(recursive=True):
-            proc.kill()
-        process.kill()
-    except psutil.NoSuchProcess:  # good process cleaned itself up
-        pass
-
-
-def deploy_process(command, catch_output: bool = False, timeout: Optional[float] = None):
-    """Private helper for efficient submission and cleanup of shell processes."""
-    proc = subprocess.Popen(command, stdout=subprocess.PIPE, shell=True, text=True)
-    output = proc.communicate()[0].strip() if catch_output else None
-    proc.wait(timeout=timeout)
-    _kill_process(proc=proc)
-    return output
-
-
 def get_globus_dataset_content_sizes(
     globus_endpoint_id: str, path: str, recursive: bool = True, timeout: float = 120.0
 ) -> Dict[str, int]:  # pragma: no cover
     """
     May require external login via 'globus login' from CLI.
 
     Returns dictionary whose keys are file names and values are sizes in bytes.
@@ -92,15 +71,15 @@
         and to batch a large number of very small files together.
 
         It is also generally recommended to submit up to 3 simultaneous transfer,
         *i.e.*, `source_files` is recommended to have at most 3 items all of similar total byte size.
     destination_endpoint_id : str
         Destination Globus ID.
     destination_folder : FolderPathType
-        Absolute path to a local folder where all content will be transfered to.
+        Absolute path to a local folder where all content will be transferred to.
     display_progress : bool, default: True
         Whether to display the transfer as progress bars using `tqdm`.
     progress_update_rate : float, default: 60.0
         How frequently (in seconds) to update the progress bar display tracking the data transfer.
     progress_update_timeout : float, default: 600.0
         Maximum amount of time to monitor the transfer progress.
         You may wish to set this to be longer when transferring very large files.
@@ -340,15 +319,15 @@
     dandi_download(urls=dandiset_url, output_dir=str(dandiset_folder_path), get_metadata=True, get_assets=False)
     assert dandiset_path.exists(), "DANDI download failed!"
 
     dandi_organize(paths=str(nwb_folder_path), dandiset_path=str(dandiset_path))
     organized_nwbfiles = dandiset_path.rglob("*.nwb")
 
     # DANDI has yet to implement forcing of session_id inclusion in organize step
-    # This manually enforces it when only a single sesssion per subject is organized
+    # This manually enforces it when only a single session per subject is organized
     for organized_nwbfile in organized_nwbfiles:
         if "ses" not in organized_nwbfile.stem:
             with NWBHDF5IO(path=organized_nwbfile, mode="r") as io:
                 nwbfile = io.read()
                 session_id = nwbfile.session_id
             dandi_stem = organized_nwbfile.stem
             dandi_stem_split = dandi_stem.split("_")
@@ -356,15 +335,15 @@
             corrected_name = "_".join(dandi_stem_split) + ".nwb"
             organized_nwbfile.rename(organized_nwbfile.parent / corrected_name)
     organized_nwbfiles = dandiset_path.rglob("*.nwb")
     # The above block can be removed once they add the feature
 
     assert len(list(dandiset_path.iterdir())) > 1, "DANDI organize failed!"
 
-    dandi_instance = "dandi-staging" if staging else "dandi"
+    dandi_instance = "dandi-staging" if staging else "dandi"  # Test
     dandi_upload(paths=[str(x) for x in organized_nwbfiles], dandi_instance=dandi_instance)
 
     # Cleanup should be confirmed manually; Windows especially can complain
     if cleanup:
         try:
             rmtree(path=dandiset_folder_path)
             rmtree(path=nwb_folder_path)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/figshare.py` & `neuroconv-0.3.0/src/neuroconv/tools/figshare.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/hdmf.py` & `neuroconv-0.3.0/src/neuroconv/tools/hdmf.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/importing.py` & `neuroconv-0.3.0/src/neuroconv/tools/importing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tool functions for performaing imports."""
-import sys
+"""Tool functions for performing imports."""
 import importlib.util
-from platform import python_version
+import sys
+from platform import processor, python_version
 from types import ModuleType
-from typing import Optional, Dict, List
+from typing import Dict, List, Optional, Union
 
 from packaging import version
 
 
 def get_package(
     package_name: str,
     installation_instructions: Optional[str] = None,
     excluded_python_versions: Optional[List[str]] = None,
-    excluded_platforms_and_python_versions: Optional[Dict[str, List[str]]] = None,
+    excluded_platforms_and_python_versions: Optional[Dict[str, Union[List[str], Dict[str, List[str]]]]] = None,
 ) -> ModuleType:
     """
     Check if package is installed and return module if so.
 
     Otherwise, raise informative error describing how to perform the installation.
     Inspired by https://docs.python.org/3/library/importlib.html#checking-if-a-module-can-be-imported.
 
@@ -25,25 +25,25 @@
     package_name : str
         Name of the package to be imported.
     installation_instructions : str, optional
         String describing the source, options, and alias of package name (if needed) for installation.
         For example,
             >>> installation_source = "conda install -c conda-forge my-package-name"
         Defaults to f"pip install {package_name}".
-    excluded_python_versions : list of string versions, optional
+    excluded_python_versions : list of strs, optional
         If a given package has no distribution available for a certain Python version, it can be excluded by this
         import across all platforms. If you wish to be more specific about combinations of platforms and versions,
         use the 'excluded_platforms_and_python_versions' keyword argument instead.
         Allows all Python versions by default.
-    excluded_platforms_and_python_versions : dict mapping string platform names to a list of string versions, optional
-        In case some combinations of platforms or Python versions are not allowed for the given package, specify
-        this dictionary to raise a more specific error to that issue.
-        For example, `excluded_platforms_and_python_versions = dict(darwin=["3.7"])` will raise an informative error
-        when running on MacOS with Python version 3.7.
-        Allows all platforms and Python versions by default.
+    excluded_platforms_and_python_versions : dict, optional
+        mapping string platform names to a list of string versions. In case some combinations of platforms or Python
+        versions are not allowed for the given package, specify this dictionary to raise a more specific error to
+        that issue. For example, `excluded_platforms_and_python_versions = dict(darwin=["3.7"])` will raise an
+        informative error when running on MacOS with Python version 3.7. Allows all platforms and Python versions by
+        default.
 
     Raises
     ------
     ModuleNotFoundError
     """
     installation_instructions = installation_instructions or f"pip install {package_name}"
     excluded_python_versions = excluded_python_versions or list()
@@ -54,20 +54,32 @@
         version.parse(excluded_version).minor for excluded_version in excluded_python_versions
     ]
     if python_minor_version in excluded_python_minor_versions:
         raise ModuleNotFoundError(
             f"\nThe package '{package_name}' is not available for Python version 3.{python_minor_version}!"
         )
 
-    for excluded_version in excluded_platforms_and_python_versions.get(sys.platform, list()):
-        if python_minor_version == version.parse(excluded_version).minor:
-            raise ModuleNotFoundError(
-                f"\nThe package '{package_name}' is not available on the {sys.platform} platform for "
-                f"Python version {excluded_version}!"
-            )
+    # Specific architecture of specific platform is specified
+    if isinstance(excluded_platforms_and_python_versions.get(sys.platform), dict):
+        architecture = processor()
+        for excluded_version in excluded_platforms_and_python_versions[sys.platform].get(architecture, list()):
+            platform_string = f"{sys.platform}:{architecture}"
+
+            if python_minor_version == version.parse(excluded_version).minor:
+                raise ModuleNotFoundError(
+                    f"\nThe package '{package_name}' is not available on the {platform_string} platform for "
+                    f"Python version {excluded_version}!"
+                )
+    else:
+        for excluded_version in excluded_platforms_and_python_versions.get(sys.platform, list()):
+            if python_minor_version == version.parse(excluded_version).minor:
+                raise ModuleNotFoundError(
+                    f"\nThe package '{package_name}' is not available on the {sys.platform} platform for "
+                    f"Python version {excluded_version}!"
+                )
 
     if package_name in sys.modules:
         return sys.modules[package_name]
 
     if importlib.util.find_spec(package_name) is not None:
         return importlib.import_module(name=package_name)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/neo/neo.py` & `neuroconv-0.3.0/src/neuroconv/tools/neo/neo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""Author: Luiz Tauffer."""
-from typing import Optional, Tuple
 import distutils.version
 import uuid
+import warnings
 from datetime import datetime
 from pathlib import Path
-import warnings
-import numpy as np
+from typing import Optional, Tuple
 
 import neo.io.baseio
+import numpy as np
 import pynwb
 from hdmf.backends.hdf5 import H5DataIO
 
 from ..nwb_helpers import add_device_from_metadata
 from ...utils import OptionalFilePathType
 
-
 response_classes = dict(
     voltage_clamp=pynwb.icephys.VoltageClampSeries,
     current_clamp=pynwb.icephys.CurrentClampSeries,
     izero=pynwb.icephys.IZeroClampSeries,
 )
 
 stim_classes = dict(
@@ -113,15 +111,15 @@
         conversion = 1.0
     else:
         conversion = 1.0
         warnings.warn("No valid units found for traces in the current file. Gain is set to 1, but this might be wrong.")
     return float(conversion)
 
 
-def get_nwb_metadata(neo_reader, metadata: dict = None):
+def get_nwb_metadata(neo_reader, metadata: dict = None) -> dict:
     """
     Return default metadata for all recording fields.
 
     Parameters
     ----------
     neo_reader: Neo reader object
     metadata: dict, optional
@@ -484,14 +482,15 @@
         properties in the RecordingExtractor object.
     compression: str (optional, defaults to "gzip")
         Type of compression to use. Valid types are "gzip" and "lzf".
         Set to None to disable all compression.
     icephys_experiment_type: str (optional)
         Type of Icephys experiment. Allowed types are: 'voltage_clamp', 'current_clamp' and 'izero'.
         If no value is passed, 'voltage_clamp' is used as default.
+    stimulus_type: str, optional
     skip_electrodes: tuple, optional
         Electrode IDs to skip. Defaults to ().
     """
     if nwbfile is not None:
         assert isinstance(nwbfile, pynwb.NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
 
     assert (
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py` & `neuroconv-0.3.0/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """General purpose iterator for all ImagingExtractor data."""
-from typing import Tuple, Optional
+from typing import Optional, Tuple
 
 import numpy as np
 from hdmf.data_utils import GenericDataChunkIterator
 from roiextractors import ImagingExtractor
 
 
 class ImagingExtractorDataChunkIterator(GenericDataChunkIterator):
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/roiextractors/roiextractors.py` & `neuroconv-0.3.0/src/neuroconv/tools/roiextractors/roiextractors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,52 @@
-"""Authors: Heberto Mayorquin, Saksham Sharda, Alessio Buccino and Szonja Weigl."""
 from collections import defaultdict
 from copy import deepcopy
-from typing import Optional
+from typing import Literal, Optional
 from warnings import warn
 
 import numpy as np
 import psutil
 from hdmf.backends.hdf5.h5_utils import H5DataIO
 
-# from hdmf.commmon import VectorData
+# from hdmf.common import VectorData
 from hdmf.data_utils import DataChunkIterator
 from pynwb import NWBFile
 from pynwb.base import Images
 from pynwb.device import Device
 from pynwb.image import GrayscaleImage
 from pynwb.ophys import (
+    DfOverF,
+    Fluorescence,
     ImageSegmentation,
     ImagingPlane,
-    PlaneSegmentation,
-    Fluorescence,
+    OnePhotonSeries,
     OpticalChannel,
-    TwoPhotonSeries,
+    PlaneSegmentation,
     RoiResponseSeries,
-    DfOverF,
+    TwoPhotonSeries,
+)
+from roiextractors import (
+    ImagingExtractor,
+    MultiSegmentationExtractor,
+    SegmentationExtractor,
 )
-from roiextractors import ImagingExtractor, SegmentationExtractor, MultiSegmentationExtractor
 
 from .imagingextractordatachunkiterator import ImagingExtractorDataChunkIterator
 from ..hdmf import SliceableDataChunkIterator
-from ..nwb_helpers import get_default_nwbfile_metadata, make_or_load_nwbfile, get_module
-from ...utils import OptionalFilePathType, dict_deep_update, calculate_regular_series_rate
+from ..nwb_helpers import get_default_nwbfile_metadata, get_module, make_or_load_nwbfile
+from ...utils import (
+    DeepDict,
+    OptionalFilePathType,
+    calculate_regular_series_rate,
+    dict_deep_update,
+)
 
 
-def get_default_ophys_metadata() -> dict:
-    """Fill default metadata for optical physiology."""
+def get_default_ophys_metadata() -> DeepDict:
+    """Fill default metadata for Device and ImagingPlane."""
     metadata = get_default_nwbfile_metadata()
 
     default_device = dict(name="Microscope")
 
     default_optical_channel = dict(
         name="OpticalChannel",
         emission_lambda=np.nan,
@@ -50,97 +59,113 @@
         excitation_lambda=np.nan,
         indicator="unknown",
         location="unknown",
         device=default_device["name"],
         optical_channel=[default_optical_channel],
     )
 
+    metadata.update(
+        Ophys=dict(
+            Device=[default_device],
+            ImagingPlane=[default_imaging_plane],
+        ),
+    )
+
+    return metadata
+
+
+def get_default_segmentation_metadata() -> DeepDict:
+    """Fill default metadata for segmentation."""
+    metadata = get_default_ophys_metadata()
+
     default_fluorescence_roi_response_series = dict(
         name="RoiResponseSeries", description="Array of raw fluorescence traces.", unit="n.a."
     )
 
     default_fluorescence = dict(
         name="Fluorescence",
         roi_response_series=[default_fluorescence_roi_response_series],
     )
 
-    default_dff_roi_response_series = dict(name="RoiResponseSeries", description="Array of df/F traces.", unit="n.a.")
+    default_dff_roi_response_series = dict(
+        name="RoiResponseSeries",
+        description="Array of df/F traces.",
+        unit="n.a.",
+    )
 
     default_df_over_f = dict(
         name="DfOverF",
         roi_response_series=[default_dff_roi_response_series],
     )
 
-    default_two_photon_series = dict(
-        name="TwoPhotonSeries",
-        description="Imaging data from two-photon excitation microscopy.",
-        unit="n.a.",
-    )
-
     default_image_segmentation = dict(
         name="ImageSegmentation",
         plane_segmentations=[
             dict(
                 name="PlaneSegmentation",
                 description="Segmented ROIs",
             )
         ],
     )
 
-    metadata.update(
-        Ophys=dict(
-            Device=[default_device],
+    metadata["Ophys"].update(
+        dict(
             Fluorescence=default_fluorescence,
             DfOverF=default_df_over_f,
             ImageSegmentation=default_image_segmentation,
-            ImagingPlane=[default_imaging_plane],
-            TwoPhotonSeries=[default_two_photon_series],
         ),
     )
 
     return metadata
 
 
-def get_nwb_imaging_metadata(imgextractor: ImagingExtractor) -> dict:
+def get_nwb_imaging_metadata(
+    imgextractor: ImagingExtractor,
+    photon_series_type: Literal["OnePhotonSeries", "TwoPhotonSeries"] = "TwoPhotonSeries",
+) -> dict:
     """
     Convert metadata from the ImagingExtractor into nwb specific metadata.
 
     Parameters
     ----------
-    imgextractor: ImagingExtractor
+    imgextractor : ImagingExtractor
+    photon_series_type : {'OnePhotonSeries', 'TwoPhotonSeries'}, optional
     """
     metadata = get_default_ophys_metadata()
 
     channel_name_list = imgextractor.get_channel_names() or (
         ["OpticalChannel"]
         if imgextractor.get_num_channels() == 1
         else [f"OpticalChannel{idx}" for idx in range(imgextractor.get_num_channels())]
     )
+
+    imaging_plane = metadata["Ophys"]["ImagingPlane"][0]
     for index, channel_name in enumerate(channel_name_list):
         if index == 0:
-            metadata["Ophys"]["ImagingPlane"][0]["optical_channel"][index]["name"] = channel_name
+            imaging_plane["optical_channel"][index]["name"] = channel_name
         else:
-            metadata["Ophys"]["ImagingPlane"][0]["optical_channel"].append(
+            imaging_plane["optical_channel"].append(
                 dict(
                     name=channel_name,
                     emission_lambda=np.nan,
                     description="An optical channel of the microscope.",
                 )
             )
 
-    # TwoPhotonSeries update:
-    metadata["Ophys"]["TwoPhotonSeries"][0].update(dimension=list(imgextractor.get_image_size()))
-
-    plane_name = metadata["Ophys"]["ImagingPlane"][0]["name"]
-    metadata["Ophys"]["TwoPhotonSeries"][0]["imaging_plane"] = plane_name
+    one_photon_description = "Imaging data from one-photon excitation microscopy."
+    two_photon_description = "Imaging data from two-photon excitation microscopy."
+    photon_series_metadata = dict(
+        name=photon_series_type,
+        description=two_photon_description if photon_series_type == "TwoPhotonSeries" else one_photon_description,
+        unit="n.a.",
+        imaging_plane=imaging_plane["name"],
+        dimension=list(imgextractor.get_image_size()),
+    )
+    metadata["Ophys"].update({photon_series_type: [photon_series_metadata]})
 
-    # remove what Segmentation extractor will input:
-    _ = metadata["Ophys"].pop("ImageSegmentation")
-    _ = metadata["Ophys"].pop("Fluorescence")
-    _ = metadata["Ophys"].pop("DfOverF")
     return metadata
 
 
 def add_devices(nwbfile: NWBFile, metadata: dict) -> NWBFile:
     """
     Add optical physiology devices from metadata.
     The metadata concerning the optical physiology should be stored in metadata["Ophys]["Device"]
@@ -189,15 +214,15 @@
     imaging_plane = ImagingPlane(**imaging_plane_metadata)
 
     return imaging_plane
 
 
 def add_imaging_plane(nwbfile: NWBFile, metadata: dict, imaging_plane_index: int = 0) -> NWBFile:
     """
-    Adds the imaging plane specificied by the metadata to the nwb file.
+    Adds the imaging plane specified by the metadata to the nwb file.
     The imaging plane that is added is the one located in metadata["Ophys"]["ImagingPlane"][imaging_plane_index]
 
     Parameters
     ----------
     nwbfile : NWBFile
         An previously defined -in memory- NWBFile.
     metadata : dict
@@ -243,99 +268,139 @@
     Returns
     -------
     NWBFile
         The NWBFile passed as an input with the image segmentation added.
     """
     # Set the defaults and required infrastructure
     metadata_copy = deepcopy(metadata)
-    default_metadata = get_default_ophys_metadata()
+    default_metadata = get_default_segmentation_metadata()
     metadata_copy = dict_deep_update(default_metadata, metadata_copy, append_list=False)
 
     image_segmentation_metadata = metadata_copy["Ophys"]["ImageSegmentation"]
     image_segmentation_name = image_segmentation_metadata["name"]
 
     ophys = get_module(nwbfile, "ophys")
 
     # Check if the image segmentation already exists in the NWB file
     if image_segmentation_name not in ophys.data_interfaces:
         ophys.add(ImageSegmentation(name=image_segmentation_name))
 
     return nwbfile
 
 
-def add_two_photon_series(
+def add_photon_series(
     imaging: ImagingExtractor,
     nwbfile: NWBFile,
     metadata: dict,
-    two_photon_series_index: int = 0,
+    photon_series_type: Literal["TwoPhotonSeries", "OnePhotonSeries"] = "TwoPhotonSeries",
+    photon_series_index: int = 0,
+    two_photon_series_index: Optional[int] = None,  # TODO: to be removed
     iterator_type: Optional[str] = "v2",
     iterator_options: Optional[dict] = None,
     use_times=False,  # TODO: to be removed
     buffer_size: Optional[int] = None,  # TODO: to be removed
 ) -> NWBFile:
     """
     Auxiliary static method for nwbextractor.
 
-    Adds two photon series from imaging object as TwoPhotonSeries to nwbfile object.
+    Adds photon series from ImagingExtractor to NWB file object.
+    The photon series can be added to the NWB file either as a TwoPhotonSeries
+    or OnePhotonSeries object.
+
+    Parameters
+    ----------
+    imaging : ImagingExtractor
+        The imaging extractor to get the data from.
+    nwbfile : NWBFile
+        The nwbfile to add the photon series to.
+    metadata: dict
+        The metadata for the photon series.
+    photon_series_type: {'OnePhotonSeries', 'TwoPhotonSeries'}, optional
+        The type of photon series to add, default is TwoPhotonSeries.
+    photon_series_index: int, default: 0
+        The metadata for the photon series is a list of the different photon series to add.
+        Specify which element of the list with this parameter.
+
+    Returns
+    -------
+    NWBFile
+        The NWBFile passed as an input with the photon series added.
     """
     if use_times:
         warn("Keyword argument 'use_times' is deprecated and will be removed on or after August 1st, 2022.")
     if buffer_size:
         warn(
             "Keyword argument 'buffer_size' is deprecated and will be removed on or after September 1st, 2022."
             "Specify as a key in the new 'iterator_options' dictionary instead."
         )
+    if two_photon_series_index:
+        warn("Keyword argument 'two_photon_series_index' is deprecated. Use 'photon_series_index' instead.")
+        photon_series_index = two_photon_series_index
 
     iterator_options = iterator_options or dict()
 
     metadata_copy = deepcopy(metadata)
-    metadata_copy = dict_deep_update(get_nwb_imaging_metadata(imaging), metadata_copy, append_list=False)
-
-    # Tests if TwoPhotonSeries already exists in acquisition
-    two_photon_series_metadata = metadata_copy["Ophys"]["TwoPhotonSeries"][two_photon_series_index]
-    two_photon_series_name = two_photon_series_metadata["name"]
+    assert photon_series_type in [
+        "OnePhotonSeries",
+        "TwoPhotonSeries",
+    ], "'photon_series_type' must be either 'OnePhotonSeries' or 'TwoPhotonSeries'."
+    metadata_copy = dict_deep_update(
+        get_nwb_imaging_metadata(imaging, photon_series_type=photon_series_type), metadata_copy, append_list=False
+    )
+    if photon_series_type == "TwoPhotonSeries":
+        assert (
+            "OnePhotonSeries" not in metadata_copy["Ophys"]
+        ), "Received metadata for 'OnePhotonSeries' but `photon_series_type` was not explicitly specified."
+
+    # Tests if TwoPhotonSeries//OnePhotonSeries already exists in acquisition
+    photon_series_kwargs = metadata_copy["Ophys"][photon_series_type][photon_series_index]
+    photon_series_name = photon_series_kwargs["name"]
 
-    if two_photon_series_name in nwbfile.acquisition:
-        warn(f"{two_photon_series_name} already on nwbfile")
+    if photon_series_name in nwbfile.acquisition:
+        warn(f"{photon_series_name} already on nwbfile")
         return nwbfile
 
     # Add the image plane to nwb
     nwbfile = add_imaging_plane(nwbfile=nwbfile, metadata=metadata_copy)
-    imaging_plane_name = two_photon_series_metadata["imaging_plane"]
+    imaging_plane_name = photon_series_kwargs["imaging_plane"]
     imaging_plane = nwbfile.get_imaging_plane(name=imaging_plane_name)
-    two_photon_series_metadata.update(imaging_plane=imaging_plane)
+    photon_series_kwargs.update(imaging_plane=imaging_plane)
 
     # Add the data
-    two_p_series_kwargs = two_photon_series_metadata
     frames_to_iterator = _imaging_frames_to_hdmf_iterator(
         imaging=imaging,
         iterator_type=iterator_type,
         iterator_options=iterator_options,
     )
     data = H5DataIO(data=frames_to_iterator, compression=True)
-    two_p_series_kwargs.update(data=data)
+    photon_series_kwargs.update(data=data)
 
     # Add dimension
-    two_p_series_kwargs.update(dimension=imaging.get_image_size())
+    photon_series_kwargs.update(dimension=imaging.get_image_size())
 
     # Add timestamps or rate
     if imaging.has_time_vector():
         timestamps = imaging.frame_to_time(np.arange(imaging.get_num_frames()))
         estimated_rate = calculate_regular_series_rate(series=timestamps)
         if estimated_rate:
-            two_p_series_kwargs.update(starting_time=timestamps[0], rate=estimated_rate)
+            photon_series_kwargs.update(starting_time=timestamps[0], rate=estimated_rate)
         else:
-            two_p_series_kwargs.update(timestamps=H5DataIO(data=timestamps, compression="gzip"), rate=None)
+            photon_series_kwargs.update(timestamps=H5DataIO(data=timestamps, compression="gzip"), rate=None)
     else:
         rate = float(imaging.get_sampling_frequency())
-        two_p_series_kwargs.update(starting_time=0.0, rate=rate)
+        photon_series_kwargs.update(starting_time=0.0, rate=rate)
 
-    # Add the TwoPhotonSeries to the nwbfile
-    two_photon_series = TwoPhotonSeries(**two_p_series_kwargs)
-    nwbfile.add_acquisition(two_photon_series)
+    # Add the photon series to the nwbfile (either as OnePhotonSeries or TwoPhotonSeries)
+    photon_series = dict(
+        OnePhotonSeries=OnePhotonSeries,
+        TwoPhotonSeries=TwoPhotonSeries,
+    )[
+        photon_series_type
+    ](**photon_series_kwargs)
+    nwbfile.add_acquisition(photon_series)
 
     return nwbfile
 
 
 def check_if_imaging_fits_into_memory(imaging: ImagingExtractor) -> None:
     """
     Raise an error if the full traces of an imaging extractor are larger than available memory.
@@ -418,14 +483,15 @@
     nwbfile_path: OptionalFilePathType = None,
     nwbfile: Optional[NWBFile] = None,
     metadata: Optional[dict] = None,
     overwrite: bool = False,
     verbose: bool = True,
     iterator_type: Optional[str] = "v2",
     iterator_options: Optional[dict] = None,
+    photon_series_type: Literal["TwoPhotonSeries", "OnePhotonSeries"] = "TwoPhotonSeries",
     buffer_size: Optional[int] = None,  # TODO: to be removed
 ):
     """
     Primary method for writing an ImagingExtractor object to an NWBFile.
 
     Parameters
     ----------
@@ -440,15 +506,15 @@
             write_recording(recording=my_recording_extractor, nwbfile=my_nwbfile)
         will result in the appropriate changes to the my_nwbfile object.
         If neither 'nwbfile_path' nor 'nwbfile' are specified, an NWBFile object will be automatically generated
         and returned by the function.
     metadata: dict, optional
         Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
     overwrite: bool, optional
-        Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
+        Whether to overwrite the NWBFile if one exists at the nwbfile_path.
         The default is False (append mode).
     verbose: bool, optional
         If 'nwbfile_path' is specified, informs user after a successful write operation.
         The default is True.
     num_chunks: int
         Number of chunks for writing data to file
     iterator_type: {"v2", "v1",  None}, default: 'v2'
@@ -481,33 +547,34 @@
     if hasattr(imaging, "nwb_metadata"):
         metadata = dict_deep_update(imaging.nwb_metadata, metadata, append_list=False)
 
     with make_or_load_nwbfile(
         nwbfile_path=nwbfile_path, nwbfile=nwbfile, metadata=metadata, overwrite=overwrite, verbose=verbose
     ) as nwbfile_out:
         add_devices(nwbfile=nwbfile_out, metadata=metadata)
-        add_two_photon_series(
+        add_photon_series(
             imaging=imaging,
             nwbfile=nwbfile_out,
             metadata=metadata,
+            photon_series_type=photon_series_type,
             iterator_type=iterator_type,
             iterator_options=iterator_options,
         )
     return nwbfile_out
 
 
-def get_nwb_segmentation_metadata(sgmextractor: SegmentationExtractor):
+def get_nwb_segmentation_metadata(sgmextractor: SegmentationExtractor) -> dict:
     """
     Convert metadata from the segmentation into nwb specific metadata.
 
     Parameters
     ----------
     sgmextractor: SegmentationExtractor
     """
-    metadata = get_default_ophys_metadata()
+    metadata = get_default_segmentation_metadata()
     # Optical Channel name:
     for i in range(sgmextractor.get_num_channels()):
         ch_name = sgmextractor.get_channel_names()[i]
         if i == 0:
             metadata["Ophys"]["ImagingPlane"][0]["optical_channel"][i]["name"] = ch_name
         else:
             metadata["Ophys"]["ImagingPlane"][0]["optical_channel"].append(
@@ -521,16 +588,15 @@
         if trace_data is not None and len(trace_data.shape) != 0:
             metadata["Ophys"]["Fluorescence"]["roi_response_series"].append(
                 dict(
                     name=trace_name.capitalize(),
                     description=f"description of {trace_name} traces",
                 )
             )
-    # remove what imaging extractor will input:
-    _ = metadata["Ophys"].pop("TwoPhotonSeries")
+
     return metadata
 
 
 def add_plane_segmentation(
     segmentation_extractor: SegmentationExtractor,
     nwbfile: NWBFile,
     metadata: Optional[dict],
@@ -591,15 +657,15 @@
     )
 
     iterator_options = iterator_options or dict()
     compression_options = compression_options or dict(compression="gzip")
 
     # Set the defaults and required infrastructure
     metadata_copy = deepcopy(metadata)
-    default_metadata = get_default_ophys_metadata()
+    default_metadata = get_default_segmentation_metadata()
     metadata_copy = dict_deep_update(default_metadata, metadata_copy, append_list=False)
 
     image_segmentation_metadata = metadata_copy["Ophys"]["ImageSegmentation"]
     plane_segmentation_metadata = image_segmentation_metadata["plane_segmentations"][plane_segmentation_index]
     plane_segmentation_name = plane_segmentation_metadata["name"]
 
     add_imaging_plane(nwbfile=nwbfile, metadata=metadata_copy, imaging_plane_index=plane_segmentation_index)
@@ -716,15 +782,15 @@
         The nwbfile passed as an input with the fluorescence traces added.
     """
     iterator_options = iterator_options or dict()
     compression_options = compression_options or dict(compression="gzip")
 
     # Set the defaults and required infrastructure
     metadata_copy = deepcopy(metadata)
-    default_metadata = get_default_ophys_metadata()
+    default_metadata = get_default_segmentation_metadata()
     metadata_copy = dict_deep_update(default_metadata, metadata_copy, append_list=False)
 
     # df/F metadata
     df_over_f_metadata = metadata_copy["Ophys"]["DfOverF"]
     df_over_f_name = df_over_f_metadata["name"]
 
     # Fluorescence traces metadata
@@ -894,15 +960,15 @@
 
     image_collection_does_not_exist = images_set_name not in ophys.data_interfaces
     if image_collection_does_not_exist:
         ophys.add(Images(images_set_name))
     image_collection = ophys.data_interfaces[images_set_name]
 
     for img_name, img in images_to_add.items():
-        # Note that nwb uses the conversion width x heigth (columns, rows) and roiextractors uses the transpose
+        # Note that nwb uses the conversion width x height (columns, rows) and roiextractors uses the transpose
         image_collection.add_image(GrayscaleImage(name=img_name, data=img.T))
 
     return nwbfile
 
 
 def write_segmentation(
     segmentation_extractor: SegmentationExtractor,
@@ -914,15 +980,15 @@
     buffer_size: int = 10,
     plane_num: int = 0,
     include_roi_centroids: bool = True,
     include_roi_acceptance: bool = True,
     mask_type: Optional[str] = "image",  # Optional[Literal["image", "pixel"]]
     iterator_options: Optional[dict] = None,
     compression_options: Optional[dict] = None,
-):
+) -> NWBFile:
     """
     Primary method for writing an SegmentationExtractor object to an NWBFile.
 
     Parameters
     ----------
     segmentation_extractor: SegmentationExtractor
         The segentation extractor object to be written to nwb
@@ -934,30 +1000,28 @@
         E.g., calling
             write_recording(recording=my_recording_extractor, nwbfile=my_nwbfile)
         will result in the appropriate changes to the my_nwbfile object.
         If neither 'nwbfile_path' nor 'nwbfile' are specified, an NWBFile object will be automatically generated
         and returned by the function.
     metadata: dict, optional
         Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
-    overwrite: bool, optional
-        Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
-        The default is False (append mode).
-    verbose: bool, optional
+    overwrite: bool, default: False
+        Whether to overwrite the NWBFile if one exists at the nwbfile_path.
+    verbose: bool, default: True
         If 'nwbfile_path' is specified, informs user after a successful write operation.
-        The default is True.
-    buffer_size : int, optional
-        The buffer size in GB, by default 10
+    buffer_size : int, default: 10
+        The buffer size in GB.
     plane_num : int, default: 0
         The plane number to be extracted.
-    include_roi_centroids : bool, optional
+    include_roi_centroids : bool, default: True
         Whether to include the ROI centroids on the PlaneSegmentation table.
         If there are a very large number of ROIs (such as in whole-brain recordings), you may wish to disable this for
             faster write speeds.
         Defaults to True.
-    include_roi_acceptance : bool, optional
+    include_roi_acceptance : bool, default: True
         Whether to include if the detected ROI was 'accepted' or 'rejected'.
         If there are a very large number of ROIs (such as in whole-brain recordings), you may wish to ddisable this for
             faster write speeds.
         Defaults to True.
     mask_type : str, optional
         There are two types of ROI masks in NWB: ImageMasks and PixelMasks.
         Image masks have the same shape as the reference images the segmentation was applied to, and weight each pixel
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/signal_processing.py` & `neuroconv-0.3.0/src/neuroconv/tools/signal_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-"""Author: Cody Baker."""
 from typing import Optional
 
 import numpy as np
 
+from ..utils import ArrayType
+
 
 def get_rising_frames_from_ttl(trace: np.ndarray, threshold: Optional[float] = None) -> np.ndarray:
     """
     Return the frame indices for rising events in a TTL pulse.
 
     Parameters
     ----------
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/spikeinterface/spikeinterface.py` & `neuroconv-0.3.0/src/neuroconv/tools/spikeinterface/spikeinterface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,51 @@
-"""Author: Heberto Mayorquin, Cody Baker."""
 import uuid
 import warnings
-import numpy as np
-from packaging.version import Version
-from typing import Union, Optional, List
-from warnings import warn
 from collections import defaultdict
+from numbers import Real
+from typing import List, Literal, Optional, Union
 
-from nwbinspector.utils import get_package_version
+import numpy as np
+import psutil
 import pynwb
-from spikeinterface import BaseRecording, BaseSorting, WaveformExtractor
-from spikeinterface.core.old_api_utils import OldToNewRecording, OldToNewSorting
-from spikeextractors import RecordingExtractor, SortingExtractor
-from numbers import Real
-from hdmf.data_utils import DataChunkIterator, AbstractDataChunkIterator
 from hdmf.backends.hdf5.h5_utils import H5DataIO
-import psutil
-
+from hdmf.common.table import DynamicTable
+from hdmf.data_utils import AbstractDataChunkIterator, DataChunkIterator
+from nwbinspector.utils import get_package_version
+from packaging.version import Version
+from pynwb import NWBFile
+from spikeinterface import BaseRecording, BaseSorting, WaveformExtractor
 
-from .spikeinterfacerecordingdatachunkiterator import SpikeInterfaceRecordingDataChunkIterator
+from .spikeinterfacerecordingdatachunkiterator import (
+    SpikeInterfaceRecordingDataChunkIterator,
+)
 from ..nwb_helpers import get_module, make_or_load_nwbfile
-from ...utils import dict_deep_update, OptionalFilePathType, calculate_regular_series_rate
-
-
-SpikeInterfaceRecording = Union[BaseRecording, RecordingExtractor]
-SpikeInterfaceSorting = Union[BaseSorting, SortingExtractor]
+from ...utils import FilePathType, calculate_regular_series_rate, dict_deep_update
 
 
-def set_dynamic_table_property(
-    dynamic_table,
-    row_ids,
-    property_name,
-    values,
-    index=False,
-    default_value=np.nan,
-    table=False,
-    description="no description",
-):
-    if not isinstance(row_ids, list) or not all(isinstance(x, int) for x in row_ids):
-        raise TypeError("'ids' must be a list of integers")
-    ids = list(dynamic_table.id[:])
-    if any([i not in ids for i in row_ids]):
-        raise ValueError("'ids' contains values outside the range of existing ids")
-    if not isinstance(property_name, str):
-        raise TypeError("'property_name' must be a string")
-    if len(row_ids) != len(values) and index is False:
-        raise ValueError("'ids' and 'values' should be lists of same size")
-    if index is False:
-        if property_name in dynamic_table:
-            for row_id, value in zip(row_ids, values):
-                dynamic_table[property_name].data[ids.index(row_id)] = value
-        else:
-            col_data = [default_value] * len(ids)  # init with default val
-            for row_id, value in zip(row_ids, values):
-                col_data[ids.index(row_id)] = value
-            dynamic_table.add_column(
-                name=property_name, description=description, data=col_data, index=index, table=table
-            )
-    else:
-        if property_name in dynamic_table:
-            # TODO
-            raise NotImplementedError
-        else:
-            dynamic_table.add_column(name=property_name, description=description, data=values, index=index, table=table)
-
-
-def get_nwb_metadata(recording: SpikeInterfaceRecording, metadata: dict = None):
+def get_nwb_metadata(recording: BaseRecording, metadata: dict = None):
     """
     Return default metadata for all recording fields.
 
     Parameters
     ----------
-    recording: SpikeInterfaceRecording
+    recording: spikeinterface.BaseRecording
     metadata: dict
         metadata info for constructing the nwb file (optional).
     """
-    if isinstance(recording, RecordingExtractor):
-        checked_recording = OldToNewRecording(oldapi_recording_extractor=recording)
-    else:
-        checked_recording = recording
     metadata = dict(
         NWBFile=dict(
             session_description="Auto-generated by NwbRecordingExtractor without description.",
             identifier=str(uuid.uuid4()),
         ),
         Ecephys=dict(
             Device=[dict(name="Device", description="Ecephys probe. Automatically generated.")],
             ElectrodeGroup=[
-                dict(name=str(gn), description="no description", location="unknown", device="Device")
-                for gn in np.unique(checked_recording.get_channel_groups())
+                dict(name=str(group_name), description="no description", location="unknown", device="Device")
+                for group_name in np.unique(recording.get_channel_groups())
             ],
         ),
     )
     return metadata
 
 
 def add_devices(nwbfile: pynwb.NWBFile, metadata: dict = None):
@@ -130,25 +83,25 @@
     if "Device" not in metadata["Ecephys"]:
         metadata["Ecephys"]["Device"] = [defaults]
     for dev in metadata["Ecephys"]["Device"]:
         if dev.get("name", defaults["name"]) not in nwbfile.devices:
             nwbfile.create_device(**dict(defaults, **dev))
 
 
-def add_electrode_groups(recording: SpikeInterfaceRecording, nwbfile: pynwb.NWBFile, metadata: dict = None):
+def add_electrode_groups(recording: BaseRecording, nwbfile: pynwb.NWBFile, metadata: dict = None):
     """
     Add electrode group information to nwbfile object.
 
     Will always ensure nwbfile has at least one electrode group.
     Will auto-generate a linked device if the specified name does not exist in the nwbfile.
 
     Parameters
     ----------
-    recording: SpikeInterfaceRecording
-    nwbfile: NWBFile
+    recording: spikeinterface.BaseRecording
+    nwbfile: pynwb.NWBFile
         nwb file to which the recording information is to be added
     metadata: dict
         metadata info for constructing the nwb file (optional).
         Should be of the format
             metadata['Ecephys']['ElectrodeGroup'] = [
                 {
                     'name': my_name,
@@ -159,30 +112,26 @@
                 ...
             ]
         Missing keys in an element of metadata['Ecephys']['ElectrodeGroup'] will be auto-populated with defaults.
         Group names set by RecordingExtractor channel properties will also be included with passed metadata,
         but will only use default description and location.
     """
     assert isinstance(nwbfile, pynwb.NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
-    if isinstance(recording, RecordingExtractor):
-        checked_recording = OldToNewRecording(oldapi_recording_extractor=recording)
-    else:
-        checked_recording = recording
     if len(nwbfile.devices) == 0:
         warnings.warn("When adding ElectrodeGroup, no Devices were found on nwbfile. Creating a Device now...")
         add_devices(nwbfile=nwbfile, metadata=metadata)
     if metadata is None:
         metadata = dict()
     if "Ecephys" not in metadata:
         metadata["Ecephys"] = dict()
 
-    if "group_name" in checked_recording.get_property_keys():
-        group_names = np.unique(checked_recording.get_property("group_name"))
+    if "group_name" in recording.get_property_keys():
+        group_names = np.unique(recording.get_property("group_name"))
     else:
-        group_names = np.unique(checked_recording.get_channel_groups()).astype("str", copy=False)
+        group_names = np.unique(recording.get_channel_groups()).astype("str", copy=False)
 
     defaults = [
         dict(
             name=group_name,
             description="no description",
             location="unknown",
             device=[i.name for i in nwbfile.devices.values()][0],
@@ -216,28 +165,26 @@
             warnings.warn(
                 "More than one device found when adding electrode group "
                 f"via channel properties: using device '{device_name}'. To use a "
                 "different device, indicate it the metadata argument."
             )
         electrode_group_kwargs = dict(defaults[0])
         electrode_group_kwargs.update(device=device)
-        for grp_name in np.unique(checked_recording.get_channel_groups()).tolist():
-            electrode_group_kwargs.update(name=str(grp_name))
+        for group_name in np.unique(recording.get_channel_groups()).tolist():
+            electrode_group_kwargs.update(name=str(group_name))
             nwbfile.create_electrode_group(**electrode_group_kwargs)
 
 
-def add_electrodes(
-    recording: SpikeInterfaceRecording, nwbfile: pynwb.NWBFile, metadata: dict = None, exclude: tuple = ()
-):
+def add_electrodes(recording: BaseRecording, nwbfile: pynwb.NWBFile, metadata: dict = None, exclude: tuple = ()):
     """
     Add channels from recording object as electrodes to nwbfile object.
 
     Parameters
     ----------
-    recording: SpikeInterfaceRecording
+    recording: spikeinterface.BaseRecording
     nwbfile: NWBFile
         nwb file to which the recording information is to be added
     metadata: dict
         metadata info for constructing the nwb file (optional).
         Should be of the format
             metadata['Ecephys']['Electrodes'] = [
                 {
@@ -258,42 +205,14 @@
         If no group information is passed via metadata, automatic linking to existing electrode groups,
         possibly including the default, will occur.
     exclude: tuple
         An iterable containing the string names of channel properties in the RecordingExtractor
         object to ignore when writing to the NWBFile.
     """
     assert isinstance(nwbfile, pynwb.NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
-    if isinstance(recording, RecordingExtractor):
-        msg = (
-            "Support for spikeextractors.RecordingExtractor objects is deprecated. "
-            "Use spikeinterface.BaseRecording objects"
-        )
-        warnings.warn(msg, DeprecationWarning, stacklevel=2)
-        checked_recording = OldToNewRecording(oldapi_recording_extractor=recording)
-        # TODO: Remove spikeextractors backend
-        warn(
-            message=(
-                "Interfaces using a spikeextractors backend will soon be deprecated! "
-                "Please use the SpikeInterface backend instead."
-            ),
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-    else:
-        checked_recording = recording
-
-    # this flag is used to keep old behavior of assigning "id" from int channel_ids
-    old_api = isinstance(checked_recording, OldToNewRecording)
-
-    # For older versions of pynwb, we need to manually add these columns
-    if get_package_version("pynwb") < Version("1.3.0"):
-        if nwbfile.electrodes is None or "rel_x" not in nwbfile.electrodes.colnames:
-            nwbfile.add_electrode_column("rel_x", "x position of electrode in electrode group")
-        if nwbfile.electrodes is None or "rel_y" not in nwbfile.electrodes.colnames:
-            nwbfile.add_electrode_column("rel_y", "y position of electrode in electrode group")
 
     # Test that metadata has the expected structure
     electrodes_metadata = list()
     if metadata is not None:
         electrodes_metadata = metadata.get("Ecephys", dict()).get("Electrodes", list())
 
     required_keys = {"name", "description"}
@@ -312,44 +231,40 @@
     property_descriptions = dict()
     for property in electrodes_metadata:
         property_descriptions[property["name"]] = property["description"]
 
     # 1. Build columns details from extractor properties: dict(name: dict(description='',data=data, index=False))
     data_to_add = defaultdict(dict)
 
-    recorder_properties = checked_recording.get_property_keys()
+    recorder_properties = recording.get_property_keys()
     excluded_properties = list(exclude) + ["contact_vector"]
     properties_to_extract = [property for property in recorder_properties if property not in excluded_properties]
 
     for property in properties_to_extract:
-        data = checked_recording.get_property(property)
+        data = recording.get_property(property)
         index = isinstance(data[0], (list, np.ndarray, tuple))
         # booleans are parsed as strings
         if isinstance(data[0], (bool, np.bool_)):
             data = data.astype(str)
         # Fill with provided custom descriptions
         description = property_descriptions.get(property, "no description")
         data_to_add[property].update(description=description, data=data, index=index)
 
     extra_descriptions = [property for property in property_descriptions.keys() if property not in data_to_add]
     if extra_descriptions:
         raise ValueError(f"{extra_descriptions} are not available in the recording extractor, set them first")
 
     # Channel name logic
-    channel_ids = checked_recording.get_channel_ids()
+    channel_ids = recording.get_channel_ids()
     if "channel_name" in data_to_add:
         # if 'channel_name' is set as a property, it is used to override default channel_ids (and "id")
         channel_name_array = data_to_add["channel_name"]["data"]
     else:
         channel_name_array = channel_ids.astype("str", copy=False)
         data_to_add["channel_name"].update(description="unique channel reference", data=channel_name_array, index=False)
-        if old_api:
-            # If the channel ids are integer keep the old behavior of asigning nwbfile.electrodes.id equal to channel_ids
-            if np.issubdtype(channel_ids.dtype, np.integer):
-                data_to_add["id"].update(data=channel_ids, index=False)
 
     # Location in spikeinterface is equivalent to rel_x, rel_y, rel_z in the nwb standard
     if "location" in data_to_add:
         data = data_to_add["location"]["data"]
         column_number_to_property = {0: "rel_x", 1: "rel_y", 2: "rel_z"}
         for column_number in range(data.shape[1]):
             property = column_number_to_property[column_number]
@@ -376,15 +291,15 @@
     data_to_add["group_name"].update(description="group_name", data=group_name_array, index=False)
 
     # Add missing groups to the nwb file
     groupless_names = [group_name for group_name in group_name_array if group_name not in nwbfile.electrode_groups]
     if len(groupless_names) > 0:
         electrode_group_list = [dict(name=group_name) for group_name in groupless_names]
         missing_group_metadata = dict(Ecephys=dict(ElectrodeGroup=electrode_group_list))
-        add_electrode_groups(recording=checked_recording, nwbfile=nwbfile, metadata=missing_group_metadata)
+        add_electrode_groups(recording=recording, nwbfile=nwbfile, metadata=missing_group_metadata)
 
     group_list = [nwbfile.electrode_groups[group_name] for group_name in group_name_array]
     data_to_add["group"].update(description="the ElectrodeGroup object", data=group_list, index=False)
 
     # 2 Divide properties to those that will be added as rows (default plus previous) and columns (new properties)
     # This mapping contains all the defaults that might be required by by pre-defined columns on the NWB schema
     # https://nwb-schema.readthedocs.io/en/latest/format.html#groups-general-extracellular-ephys-electrodes
@@ -394,15 +309,15 @@
         group_name="default",
         location="unknown",
     )
     optional_schema_property_to_default_value = dict(
         x=np.nan,
         y=np.nan,
         z=np.nan,
-        # There doesn't seem to be a canonical default for impedence, if missing.
+        # There doesn't seem to be a canonical default for impedance, if missing.
         # The NwbRecordingExtractor follows the -1.0 convention, other scripts sometimes use np.nan
         imp=-1.0,
         filtering="none",
     )
     required_schema_properties = set(required_schema_property_to_default_value)
     optional_schema_properties = set(optional_schema_property_to_default_value)
     schema_properties = required_schema_properties | optional_schema_properties
@@ -434,15 +349,15 @@
     if "channel_name" in electrode_table_previous_properties and "group_name" in electrode_table_previous_properties:
         channel_group_names_used_previously = [
             (ch_name, gr_name)
             for ch_name, gr_name in zip(nwbfile.electrodes["channel_name"].data, nwbfile.electrodes["group_name"].data)
         ]
 
     properties_with_data = [property for property in properties_to_add_by_rows if "data" in data_to_add[property]]
-    rows_in_data = [index for index in range(checked_recording.get_num_channels())]
+    rows_in_data = [index for index in range(recording.get_num_channels())]
     rows_to_add = [
         index
         for index in rows_in_data
         if (channel_name_array[index], group_name_array[index]) not in channel_group_names_used_previously
     ]
     for row in rows_to_add:
         electrode_kwargs = dict(all_properties_to_default_value)
@@ -493,20 +408,21 @@
         extended_data[indexes_for_new_data] = data
 
         extended_data[indexes_for_default_values] = default_value
         cols_args["data"] = extended_data
         nwbfile.add_electrode_column(property, **cols_args)
 
 
-def check_if_recording_traces_fit_into_memory(recording: SpikeInterfaceRecording, segment_index: int = 0) -> None:
-    """Raises an error if the full traces of a recording extractor are larger than psutil.virtual_memory().available
+def check_if_recording_traces_fit_into_memory(recording: BaseRecording, segment_index: int = 0) -> None:
+    """
+    Raises an error if the full traces of a recording extractor are larger than psutil.virtual_memory().available.
 
     Parameters
     ----------
-    recording : SpikeInterfaceRecording
+    recording : spikeinterface.BaseRecording
         A recording extractor object from spikeinterface.
     segment_index : int, optional
         The segment index of the recording extractor object, by default 0
 
     Raises
     ------
     MemoryError
@@ -533,41 +449,40 @@
     iterator_type: str = "v2",
     iterator_opts: dict = None,
 ) -> AbstractDataChunkIterator:
     """Function to wrap traces of spikeinterface recording into an AbstractDataChunkIterator.
 
     Parameters
     ----------
-    recording : BaseRecording
+    recording : spikeinterface.BaseRecording
         A recording extractor from spikeinterface
     segment_index : int, optional
         The recording segment to add to the NWBFile.
     return_scaled : bool, defaults to False
         When True recording extractor objects from spikeinterface return their traces in microvolts.
     iterator_type: {"v2", "v1",  None}, default: 'v2'
         The type of DataChunkIterator to use.
         'v1' is the original DataChunkIterator of the hdmf data_utils.
         'v2' is the locally developed SpikeInterfaceRecordingDataChunkIterator, which offers full control over chunking.
         None: write the TimeSeries with no memory chunking.
-    iterator_opts: dict (optional)
+    iterator_opts: dict, optional
         Dictionary of options for the iterator.
         See https://hdmf.readthedocs.io/en/stable/hdmf.data_utils.html#hdmf.data_utils.GenericDataChunkIterator
         for the full list of options.
 
     Returns
     -------
     traces_as_iterator: AbstractDataChunkIterator
         The traces of the recording extractor wrapped in an iterator object.
 
     Raises
     ------
     ValueError
         If the iterator_type is not 'v1', 'v2' or None.
     """
-
     supported_iterator_types = ["v1", "v2", None]
     if iterator_type not in supported_iterator_types:
         message = f"iterator_type {iterator_type} should be either 'v1', 'v2' (recommended) or None"
         raise ValueError(message)
 
     iterator_opts = dict() if iterator_opts is None else iterator_opts
 
@@ -581,25 +496,27 @@
             return_scaled=return_scaled,
             **iterator_opts,
         )
     elif iterator_type == "v1":
         traces_as_iterator = DataChunkIterator(
             data=recording.get_traces(return_scaled=return_scaled, segment_index=segment_index), **iterator_opts
         )
+    else:
+        raise ValueError("iterator_type must be None, 'v1', or 'v2'.")
 
     return traces_as_iterator
 
 
 def add_electrical_series(
-    recording: SpikeInterfaceRecording,
+    recording: BaseRecording,
     nwbfile: pynwb.NWBFile,
     metadata: dict = None,
     segment_index: int = 0,
     starting_time: Optional[float] = None,
-    write_as: str = "raw",
+    write_as: Literal["raw", "processed", "lfp"] = "raw",
     es_key: str = None,
     write_scaled: bool = False,
     compression: Optional[str] = "gzip",
     compression_opts: Optional[int] = None,
     iterator_type: str = "v2",
     iterator_opts: Optional[dict] = None,
 ):
@@ -608,22 +525,22 @@
 
     Parameters
     ----------
     recording : SpikeInterfaceRecording
         A recording extractor from spikeinterface
     nwbfile : NWBFile
         nwb file to which the recording information is to be added
-    metadata : dict
-        metadata info for constructing the nwb file (optional).
+    metadata : dict, optional
+        metadata info for constructing the nwb file.
         Should be of the format
             metadata['Ecephys']['ElectricalSeries'] = dict(
                 name=my_name,
                 description=my_description
             )
-    segment_index : int
+    segment_index : int, default: 0
         The recording segment to add to the NWBFile.
     starting_time : float, optional
         Sets the starting time of the ElectricalSeries to a manually set value.
     write_as : {'raw', 'processed', 'lfp'}
         How to save the traces data in the nwb file. Options:
         - 'raw': save it in acquisition
         - 'processed': save it as FilteredEphys, in a processing module
@@ -638,45 +555,30 @@
     compression_opts: int, default: 4
         Only applies to compression="gzip". Controls the level of the GZIP.
     iterator_type: {"v2", "v1",  None}, default: 'v2'
         The type of DataChunkIterator to use.
         'v1' is the original DataChunkIterator of the hdmf data_utils.
         'v2' is the locally developed SpikeInterfaceRecordingDataChunkIterator, which offers full control over chunking.
         None: write the TimeSeries with no memory chunking.
-    iterator_opts: dict (optional)
+    iterator_opts: dict, optional
         Dictionary of options for the iterator.
         See https://hdmf.readthedocs.io/en/stable/hdmf.data_utils.html#hdmf.data_utils.GenericDataChunkIterator
         for the full list of options.
 
     Missing keys in an element of metadata['Ecephys']['ElectrodeGroup'] will be auto-populated with defaults
     whenever possible.
     """
-    if isinstance(recording, RecordingExtractor):
-        checked_recording = OldToNewRecording(oldapi_recording_extractor=recording)
-        # TODO: Remove spikeextractors backend
-        warn(
-            message=(
-                "Interfaces using a spikeextractors backend will soon be deprecated! "
-                "Please use the SpikeInterface backend instead."
-            ),
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-    else:
-        checked_recording = recording
-
     assert write_as in [
         "raw",
         "processed",
         "lfp",
     ], f"'write_as' should be 'raw', 'processed' or 'lfp', but instead received value {write_as}"
 
-    segment_signature = "" if checked_recording.get_num_segments() == 1 else segment_index
     modality_signature = write_as.upper() if write_as == "lfp" else write_as.capitalize()
-    default_name = f"ElectricalSeries{modality_signature}{segment_signature}"
+    default_name = f"ElectricalSeries{modality_signature}"
     default_description = dict(raw="Raw acquired data", lfp="Processed data - LFP", processed="Processed data")
 
     eseries_kwargs = dict(name=default_name, description=default_description[write_as])
 
     # Select and/or create module if lfp or processed data is to be stored.
     if write_as in ["lfp", "processed"]:
         ecephys_mod = get_module(
@@ -689,34 +591,41 @@
         if write_as == "processed" and "Processed" not in ecephys_mod.data_interfaces:
             ecephys_mod.add(pynwb.ecephys.FilteredEphys(name="Processed"))
 
     if metadata is not None and "Ecephys" in metadata and es_key is not None:
         assert es_key in metadata["Ecephys"], f"metadata['Ecephys'] dictionary does not contain key '{es_key}'"
         eseries_kwargs.update(metadata["Ecephys"][es_key])
 
+    # If the recording extractor has more than 1 segment, append numbers to the names so that the names are unique.
+    # 0-pad these names based on the number of segments.
+    # If there are 10 segments use 2 digits, if there are 100 segments use 3 digits, etc.
+    if recording.get_num_segments() > 1:
+        width = int(np.ceil(np.log10((recording.get_num_segments()))))
+        eseries_kwargs["name"] += f"{segment_index:0{width}}"
+
     # Indexes by channel ids if they are integer or by indices otherwise.
-    channel_name_array = checked_recording.get_channel_ids()
+    channel_name_array = recording.get_channel_ids()
     if np.issubdtype(channel_name_array.dtype, np.integer):
         channel_indices = channel_name_array
     else:
-        channel_indices = checked_recording.ids_to_indices(channel_name_array)
+        channel_indices = recording.ids_to_indices(channel_name_array)
 
     add_electrodes(recording=recording, nwbfile=nwbfile, metadata=metadata)
 
     table_ids = [list(nwbfile.electrodes.id[:]).index(id) for id in channel_indices]
 
     electrode_table_region = nwbfile.create_electrode_table_region(
         region=table_ids, description="electrode_table_region"
     )
     eseries_kwargs.update(electrodes=electrode_table_region)
 
     # Spikeinterface guarantees data in micro volts when return_scaled=True. This multiplies by gain and adds offsets
     # In nwb to get traces in Volts we take data*channel_conversion*conversion + offset
-    channel_conversion = checked_recording.get_channel_gains()
-    channel_offset = checked_recording.get_channel_offsets()
+    channel_conversion = recording.get_channel_gains()
+    channel_offset = recording.get_channel_offsets()
 
     unique_channel_conversion = np.unique(channel_conversion)
     unique_channel_conversion = unique_channel_conversion[0] if len(unique_channel_conversion) == 1 else None
 
     unique_offset = np.unique(channel_offset)
     if unique_offset.size > 1:
         raise ValueError("Recording extractors with heterogeneous offsets are not supported")
@@ -730,31 +639,31 @@
         eseries_kwargs.update(conversion=unique_channel_conversion * micro_to_volts_conversion_factor)
 
     if not write_scaled:
         eseries_kwargs.update(offset=unique_offset * micro_to_volts_conversion_factor)
 
     # Iterator
     ephys_data_iterator = _recording_traces_to_hdmf_iterator(
-        recording=checked_recording,
+        recording=recording,
         segment_index=segment_index,
         iterator_type=iterator_type,
         iterator_opts=iterator_opts,
     )
     eseries_kwargs.update(
         data=H5DataIO(data=ephys_data_iterator, compression=compression, compression_opts=compression_opts)
     )
 
     # Timestamps vs rate
-    timestamps = checked_recording.get_times(segment_index=segment_index)
+    timestamps = recording.get_times(segment_index=segment_index)
     rate = calculate_regular_series_rate(series=timestamps)  # Returns None if it is not regular
     starting_time = starting_time if starting_time is not None else 0
 
     if rate:
         starting_time = starting_time + timestamps[0]
-        eseries_kwargs.update(starting_time=starting_time, rate=checked_recording.get_sampling_frequency())
+        eseries_kwargs.update(starting_time=starting_time, rate=recording.get_sampling_frequency())
     else:
         shifted_time_stamps = starting_time + timestamps
         wrapped_timestamps = H5DataIO(
             data=shifted_time_stamps, compression=compression, compression_opts=compression_opts
         )
         eseries_kwargs.update(timestamps=wrapped_timestamps)
 
@@ -764,65 +673,15 @@
         nwbfile.add_acquisition(es)
     elif write_as == "processed":
         ecephys_mod.data_interfaces["Processed"].add_electrical_series(es)
     elif write_as == "lfp":
         ecephys_mod.data_interfaces["LFP"].add_electrical_series(es)
 
 
-def add_epochs(recording: RecordingExtractor, nwbfile: pynwb.NWBFile):
-    """
-    Auxiliary static method for nwbextractor.
-
-    Adds epochs from recording object to nwbfile object.
-
-    Parameters
-    ----------
-    recording: RecordingExtractor
-        Epochs are supported only by spikeinterface/spikeextractors RecordingExtractor objects; does not support
-        spikeinterface/spikeinterface BaseRecording objects.
-    nwbfile: NWBFile
-        nwb file to which the recording information is to be added
-    """
-    assert isinstance(
-        recording, RecordingExtractor
-    ), "'recording' should be a spikeinterface/spikeextractors RecordingExtractor object!"
-    assert isinstance(nwbfile, pynwb.NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
-
-    # TODO: Remove spikeextractors backend
-    warn(
-        message=(
-            "Interfaces using a spikeextractors backend will soon be deprecated! "
-            "Please use the SpikeInterface backend instead."
-        ),
-        category=DeprecationWarning,
-        stacklevel=2,
-    )
-
-    for epoch_name in recording.get_epoch_names():
-        epoch = recording.get_epoch_info(epoch_name)
-        if nwbfile.epochs is None:
-            nwbfile.add_epoch(
-                start_time=recording.frame_to_time(epoch["start_frame"]),
-                stop_time=recording.frame_to_time(epoch["end_frame"] - 1),
-                tags=epoch_name,
-            )
-        else:
-            if [epoch_name] in nwbfile.epochs["tags"][:]:
-                ind = nwbfile.epochs["tags"][:].index([epoch_name])
-                nwbfile.epochs["start_time"].data[ind] = recording.frame_to_time(epoch["start_frame"])
-                nwbfile.epochs["stop_time"].data[ind] = recording.frame_to_time(epoch["end_frame"])
-            else:
-                nwbfile.add_epoch(
-                    start_time=recording.frame_to_time(epoch["start_frame"]),
-                    stop_time=recording.frame_to_time(epoch["end_frame"]),
-                    tags=epoch_name,
-                )
-
-
-def add_electrodes_info(recording: RecordingExtractor, nwbfile: pynwb.NWBFile, metadata: dict = None):
+def add_electrodes_info(recording: BaseRecording, nwbfile: pynwb.NWBFile, metadata: dict = None):
     """
     Add device, electrode_groups, and electrodes info to the nwbfile.
 
     Parameters
     ----------
     recording : SpikeInterfaceRecording
     nwbfile : NWBFile
@@ -850,201 +709,128 @@
         possibly including the default, will occur.
     """
     add_devices(nwbfile=nwbfile, metadata=metadata)
     add_electrode_groups(recording=recording, nwbfile=nwbfile, metadata=metadata)
     add_electrodes(recording=recording, nwbfile=nwbfile, metadata=metadata)
 
 
-def add_all_to_nwbfile(
-    recording: SpikeInterfaceRecording,
-    nwbfile=None,
-    starting_time: Optional[float] = None,
-    metadata: dict = None,
-    write_as: str = "raw",
-    es_key: str = None,
-    write_electrical_series: bool = True,
-    write_scaled: bool = False,
-    compression: Optional[str] = "gzip",
-    compression_opts: Optional[int] = None,
-    iterator_type: Optional[str] = None,
-    iterator_opts: Optional[dict] = None,
-):
-    """
-    Auxiliary static method for nwbextractor.
-    Adds all recording related information from recording object and metadata to the NWBFile object.
-
-    Parameters
-    ----------
-    recording : SpikeInterfaceRecording
-    nwbfile : NWBFile, optional
-        nwb file to which the recording information is to be added
-    starting_time : float, optional
-        Sets the starting time of the ElectricalSeries to a manually set value.
-    metadata : dict, optional
-        metadata info for constructing the NWB file.
-        Check the auxiliary function docstrings for more information
-        about metadata format.
-    write_as : {'raw', 'processed', 'lfp'}
-        How to save the traces data in the NWB file.
-        - 'raw': save it in acquisition
-        - 'processed': save it as FilteredEphys, in a processing module
-        - 'lfp': save it as LFP, in a processing module
-    es_key : str, optional
-        Key in metadata dictionary containing metadata info for the specific electrical series
-    write_electrical_series : bool, default: True
-        If True (default), electrical series are written in acquisition. If False, only device, electrode_groups,
-        and electrodes are written to NWB.
-    write_scaled : bool, default: True
-        If True, writes the scaled traces (return_scaled=True)
-    compression : {'gzip', 'lzf'}, optional
-        Type of compression to use.
-        Set to None to disable all compression.
-    compression_opts : int (optional, defaults to 4)
-        Only applies to compression="gzip". Controls the level of the GZIP.
-    iterator_type : {'v2', 'v1'}
-        The type of DataChunkIterator to use.
-        'v1' is the original DataChunkIterator of the hdmf data_utils.
-        'v2' is the locally developed RecordingExtractorDataChunkIterator, which offers full control over chunking.
-    iterator_opts : dict, optional
-        Dictionary of options for the RecordingExtractorDataChunkIterator (iterator_type='v2')
-        or DataChunkIterator (iterator_type='v1').
-        Valid options are
-            buffer_gb : float (optional, defaults to 1 GB, available for both 'v2' and 'v1')
-                Recommended to be as much free RAM as available). Automatically calculates suitable buffer shape.
-            chunk_mb : float (optional, defaults to 1 MB, only available for 'v2')
-                Should be below 1 MB. Automatically calculates suitable chunk shape.
-        If manual specification of buffer_shape and chunk_shape are desired, these may be specified as well.
-    """
-    if nwbfile is not None:
-        assert isinstance(nwbfile, pynwb.NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
-    add_electrodes_info(recording=recording, nwbfile=nwbfile, metadata=metadata)
-
-    if write_electrical_series:
-        add_electrical_series(
-            recording=recording,
-            nwbfile=nwbfile,
-            starting_time=starting_time,
-            metadata=metadata,
-            write_as=write_as,
-            es_key=es_key,
-            write_scaled=write_scaled,
-            compression=compression,
-            compression_opts=compression_opts,
-            iterator_type=iterator_type,
-            iterator_opts=iterator_opts,
-        )
-    if isinstance(recording, RecordingExtractor):
-        add_epochs(recording=recording, nwbfile=nwbfile)
-
-
 def write_recording(
-    recording: SpikeInterfaceRecording,
-    nwbfile_path: OptionalFilePathType = None,
+    recording: BaseRecording,
+    nwbfile_path: Optional[FilePathType] = None,
     nwbfile: Optional[pynwb.NWBFile] = None,
     metadata: Optional[dict] = None,
     overwrite: bool = False,
     verbose: bool = True,
     starting_time: Optional[float] = None,
     write_as: Optional[str] = None,
     es_key: Optional[str] = None,
     write_electrical_series: bool = True,
     write_scaled: bool = False,
     compression: Optional[str] = None,
     compression_opts: Optional[int] = None,
     iterator_type: str = "v2",
     iterator_opts: Optional[dict] = None,
-):
+) -> pynwb.NWBFile:
     """
     Primary method for writing a RecordingExtractor object to an NWBFile.
 
     Parameters
     ----------
-    recording : SpikeInterfaceRecording
-    nwbfile_path : FilePathType
+    recording : spikeinterface.BaseRecording
+    nwbfile_path : FilePathType, optional
         Path for where to write or load (if overwrite=False) the NWBFile.
         If specified, the context will always write to this location.
     nwbfile : NWBFile, optional
         If passed, this function will fill the relevant fields within the NWBFile object.
         E.g., calling
             write_recording(recording=my_recording_extractor, nwbfile=my_nwbfile)
         will result in the appropriate changes to the my_nwbfile object.
         If neither 'nwbfile_path' nor 'nwbfile' are specified, an NWBFile object will be automatically generated
         and returned by the function.
     metadata : dict, optional
         metadata info for constructing the nwb file (optional). Should be
         of the format
-            metadata['Ecephys'] = {}
-        with keys of the forms
-            metadata['Ecephys']['Device'] = [
-                {
-                    'name': my_name,
-                    'description': my_description
-                },
-                ...
-            ]
-            metadata['Ecephys']['ElectrodeGroup'] = [
-                {
-                    'name': my_name,
-                    'description': my_description,
-                    'location': electrode_location,
-                    'device': my_device_name
-                },
-                ...
-            ]
-            metadata['Ecephys']['Electrodes'] = [
-                {
+            metadata['Ecephys'] = {
+                'Device': [
+                    {
+                        'name': my_name,
+                        'description': my_description
+                    },
+                    ...
+                ]
+                'ElectrodeGroup': [
+                    {
+                        'name': my_name,
+                        'description': my_description,
+                        'location': electrode_location,
+                        'device': my_device_name
+                    },
+                    ...
+                ]
+                'Electrodes': [
+                    {
+                        'name': my_name,
+                        'description': my_description
+                    },
+                    ...
+                ]
+                'ElectricalSeries' = {
                     'name': my_name,
                     'description': my_description
-                },
-                ...
-            ]
-            metadata['Ecephys']['ElectricalSeries'] = {
-                'name': my_name,
-                'description': my_description
-            }
+                }
         Note that data intended to be added to the electrodes table of the NWBFile should be set as channel
         properties in the RecordingExtractor object.
-    overwrite : bool, optional
-        Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
-        The default is False (append mode).
-    verbose : bool, optional
+    overwrite : bool, default: False
+        Whether to overwrite the NWBFile if one exists at the nwbfile_path.
+    verbose : bool, default: True
         If 'nwbfile_path' is specified, informs user after a successful write operation.
-        The default is True.
     starting_time : float, optional
         Sets the starting time of the ElectricalSeries to a manually set value.
     write_as: {'raw', 'processed', 'lfp'}, optional
         How to save the traces data in the nwb file.
         - 'raw' will save it in acquisition
         - 'processed' will save it as FilteredEphys, in a processing module
         - 'lfp' will save it as LFP, in a processing module
     es_key: str, optional
         Key in metadata dictionary containing metadata info for the specific electrical series
     write_electrical_series: bool, default: True
         If True, electrical series are written in acquisition. If False, only device, electrode_groups,
         and electrodes are written to NWB.
-    write_scaled: bool, optional, default: True
+    write_scaled: bool, default: True
         If True, writes the scaled traces (return_scaled=True)
     compression: {None, 'gzip', 'lzp'}
         Type of compression to use.
         Set to None to disable all compression.
     compression_opts: int, optional, default: 4
         Only applies to compression="gzip". Controls the level of the GZIP.
-    iterator_type: {"v2", "v1",  None}, default: 'v2'
+    iterator_type: {"v2", "v1",  None}
         The type of DataChunkIterator to use.
         'v1' is the original DataChunkIterator of the hdmf data_utils.
         'v2' is the locally developed SpikeInterfaceRecordingDataChunkIterator, which offers full control over chunking.
         None: write the TimeSeries with no memory chunking.
     iterator_opts: dict, optional
         Dictionary of options for the RecordingExtractorDataChunkIterator (iterator_type='v2').
-        Valid options are
-            buffer_gb : float (optional, defaults to 1 GB)
-                Recommended to be as much free RAM as available). Automatically calculates suitable buffer shape.
-            chunk_mb : float (optional, defaults to 1 MB)
+        Valid options are:
+            buffer_gb : float, default: 1.0
+                In units of GB. Recommended to be as much free RAM as available. Automatically calculates suitable
+                buffer shape.
+            buffer_shape : tuple, optional
+                Manual specification of buffer shape to return on each iteration.
+                Must be a multiple of chunk_shape along each axis.
+                Cannot be set if `buffer_gb` is specified.
+            chunk_mb : float. default: 1.0
                 Should be below 1 MB. Automatically calculates suitable chunk shape.
-        If manual specification of buffer_shape and chunk_shape are desired, these may be specified as well.
+            chunk_shape : tuple, optional
+                Manual specification of the internal chunk shape for the HDF5 dataset.
+                Cannot be set if `chunk_mb` is also specified.
+            display_progress : bool, default: False
+                Display a progress bar with iteration rate and estimated completion time.
+            progress_bar_options : dict, optional
+                Dictionary of keyword arguments to be passed directly to tqdm.
+                See https://github.com/tqdm/tqdm#parameters for options.
     """
     if nwbfile is not None:
         assert isinstance(nwbfile, pynwb.NWBFile), "'nwbfile' should be of type pynwb.NWBFile"
     assert get_package_version("pynwb") >= Version(
         "1.3.3"
     ), "'write_recording' not supported for version < 1.3.3. Run pip install --upgrade pynwb"
     write_as = "raw" if write_as is None else write_as
@@ -1058,15 +844,15 @@
     with make_or_load_nwbfile(
         nwbfile_path=nwbfile_path, nwbfile=nwbfile, metadata=metadata, overwrite=overwrite, verbose=verbose
     ) as nwbfile_out:
         # Convenience function to add device, electrode groups and electrodes info
         add_electrodes_info(recording=recording, nwbfile=nwbfile_out, metadata=metadata)
 
         if write_electrical_series:
-            number_of_segments = recording.get_num_segments() if isinstance(recording, BaseRecording) else 1
+            number_of_segments = recording.get_num_segments()
             for segment_index in range(number_of_segments):
                 add_electrical_series(
                     recording=recording,
                     nwbfile=nwbfile_out,
                     segment_index=segment_index,
                     starting_time=starting_time,
                     metadata=metadata,
@@ -1074,36 +860,32 @@
                     es_key=es_key,
                     write_scaled=write_scaled,
                     compression=compression,
                     compression_opts=compression_opts,
                     iterator_type=iterator_type,
                     iterator_opts=iterator_opts,
                 )
-
-        # For objects of the legacy spikeextractors we support adding epochs
-        if isinstance(recording, RecordingExtractor):
-            add_epochs(recording=recording, nwbfile=nwbfile_out)
     return nwbfile_out
 
 
-def get_nspikes(units_table: pynwb.misc.Units, unit_id: int):
+def get_nspikes(units_table: pynwb.misc.Units, unit_id: int) -> int:
     """Return the number of spikes for chosen unit."""
     ids = np.array(units_table.id[:])
     indexes = np.where(ids == unit_id)[0]
     if not len(indexes):
         raise ValueError(f"{unit_id} is an invalid unit_id. Valid ids: {ids}.")
     index = indexes[0]
     if index == 0:
         return units_table["spike_times_index"].data[index]
     else:
         return units_table["spike_times_index"].data[index] - units_table["spike_times_index"].data[index - 1]
 
 
 def add_units_table(
-    sorting: SpikeInterfaceSorting,
+    sorting: BaseSorting,
     nwbfile: pynwb.NWBFile,
     unit_ids: Optional[List[Union[str, int]]] = None,
     property_descriptions: Optional[dict] = None,
     skip_properties: Optional[List[str]] = None,
     skip_features: Optional[List[str]] = None,
     units_table_name: str = "units",
     unit_table_description: str = "Autogenerated by neuroconv.",
@@ -1114,72 +896,50 @@
     unit_electrode_indices=None,
 ):
     """
     Primary method for writing a SortingExtractor object to an NWBFile.
 
     Parameters
     ----------
-    sorting : SpikeInterfaceSorting
+    sorting : spikeinterface.BaseSorting
     nwbfile : NWBFile
     unit_ids : list of int or list of str, optional
         Controls the unit_ids that will be written to the nwb file. If None, all
         units are written.
     property_descriptions : dict, optional
         For each key in this dictionary which matches the name of a unit
         property in sorting, adds the value as a description to that
         custom unit column.
     skip_properties : list of str, optional
         Each string in this list that matches a unit property will not be written to the NWBFile.
     skip_features : list of str, optional
         Each string in this list that matches a spike feature will not be written to the NWBFile.
-    write_in_processing_module : bool default: False
+    write_in_processing_module : bool, default: False
         How to save the units table in the nwb file.
         - True will save it to the processing module to serve as a historical provenance for the official table.
         - False will save it to the official NWBFile.Units position; recommended only for the final form of the data.
     units_table_name : str, default: 'units'
         The name of the units table. If write_as=='units', then units_table_name must also be 'units'.
     unit_table_description : str, optional
         Text description of the units table; it is recommended to include information such as the sorting method,
         curation steps, etc.
     write_waveforms : bool, default: False
         if True and either sorting is a spikeextractors SortingExtractor object with "template" property or
         waveform_means (and optionally waveform_sd) are given, then waveforms are added to the units table
         after writing.
     waveform_means : np.ndarray, optional
         Waveform mean (template) for each unit (num_units, num_samples, num_channels)
-    waveform_sds : np.array (optional, default to None)
+    waveform_sds : np.ndarray, optional
         Waveform standard deviation for each unit (num_units, num_samples, num_channels)
-    unit_electrode_indices : list of lists or arrays (optional, default to None)
+    unit_electrode_indices : list of lists or arrays, optional
         For each unit, the indices of electrodes that each waveform_mean/sd correspond to.
     """
     if not isinstance(nwbfile, pynwb.NWBFile):
         raise TypeError(f"nwbfile type should be an instance of pynwb.NWBFile but got {type(nwbfile)}")
 
-    if isinstance(sorting, SortingExtractor):
-        msg = (
-            "Support for spikeextractors.SortingExtractor objects is deprecated. "
-            "Use spikeinterface.BaseSorting objects"
-        )
-        warnings.warn(msg, DeprecationWarning, stacklevel=2)
-        checked_sorting = OldToNewSorting(oldapi_sorting_extractor=sorting)
-        # TODO: Remove spikeextractors backend
-        warn(
-            message=(
-                "Interfaces using a spikeextractors backend will soon be deprecated! "
-                "Please use the SpikeInterface backend instead."
-            ),
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-    else:
-        checked_sorting = sorting
-
-    # this flag is used to keep old behavior of assigning "id" from int unit_ids
-    old_api = isinstance(checked_sorting, OldToNewSorting)
-
     if write_in_processing_module:
         ecephys_mod = get_module(
             nwbfile=nwbfile,
             name="ecephys",
             description="Intermediate data from extracellular electrophysiology recordings, e.g., LFP.",
         )
         write_table_first_time = units_table_name not in ecephys_mod.data_interfaces
@@ -1211,27 +971,27 @@
         property_descriptions = dict()
     if skip_properties is None:
         skip_properties = list()
 
     property_descriptions = dict(default_descriptions, **property_descriptions)
 
     data_to_add = defaultdict(dict)
-    sorting_properties = checked_sorting.get_property_keys()
+    sorting_properties = sorting.get_property_keys()
     excluded_properties = list(skip_properties) + ["contact_vector"]
     properties_to_extract = [property for property in sorting_properties if property not in excluded_properties]
 
     if unit_ids is not None:
-        checked_sorting = checked_sorting.select_units(unit_ids=unit_ids)
+        sorting = sorting.select_units(unit_ids=unit_ids)
         if unit_electrode_indices is not None:
-            unit_electrode_indices = np.array(unit_electrode_indices)[checked_sorting.ids_to_indices(unit_ids)]
-    unit_ids = checked_sorting.unit_ids
+            unit_electrode_indices = np.array(unit_electrode_indices)[sorting.ids_to_indices(unit_ids)]
+    unit_ids = sorting.unit_ids
 
     # Extract properties
     for property in properties_to_extract:
-        data = checked_sorting.get_property(property)
+        data = sorting.get_property(property)
         if isinstance(data[0], (bool, np.bool_)):
             data = data.astype(str)
         index = isinstance(data[0], (list, np.ndarray, tuple))
         description = property_descriptions.get(property, "No description.")
         data_to_add[property].update(description=description, data=data, index=index)
         if property in ["max_channel", "max_electrode"] and nwbfile.electrodes is not None:
             data_to_add[property].update(table=nwbfile.electrodes)
@@ -1239,22 +999,18 @@
     # Unit name logic
     if "unit_name" in data_to_add:
         # if 'unit_name' is set as a property, it is used to override default unit_ids (and "id")
         unit_name_array = data_to_add["unit_name"]["data"]
     else:
         unit_name_array = unit_ids.astype("str", copy=False)
         data_to_add["unit_name"].update(description="Unique reference for each unit.", data=unit_name_array)
-        if old_api:
-            # If the channel ids are integer keep the old behavior of asigning table's id equal to unit_ids
-            if np.issubdtype(unit_ids.dtype, np.integer):
-                data_to_add["id"].update(data=unit_ids.astype("int"))
 
-    units_table_previous_properties = set(units_table.colnames) - set({"spike_times"})
+    units_table_previous_properties = set(units_table.colnames) - {"spike_times"}
     extracted_properties = set(data_to_add)
-    properties_to_add_by_rows = units_table_previous_properties | set({"id"})
+    properties_to_add_by_rows = units_table_previous_properties | {"id"}
     properties_to_add_by_columns = extracted_properties - properties_to_add_by_rows
 
     # Find default values for properties / columns already in the table
     type_to_default_value = {list: [], np.ndarray: np.array(np.nan), str: "", Real: np.nan}
     property_to_default_values = {"id": None}
     for property in units_table_previous_properties:
         # Find a matching data type and get the default value
@@ -1266,15 +1022,15 @@
     # Add data by rows excluding the rows with previously added unit names
     unit_names_used_previously = []
     if "unit_name" in units_table_previous_properties:
         unit_names_used_previously = units_table["unit_name"].data
     has_electrodes_column = "electrodes" in units_table.colnames
 
     properties_with_data = {property for property in properties_to_add_by_rows if "data" in data_to_add[property]}
-    rows_in_data = [index for index in range(checked_sorting.get_num_units())]
+    rows_in_data = [index for index in range(sorting.get_num_units())]
     if not has_electrodes_column:
         rows_to_add = [index for index in rows_in_data if unit_name_array[index] not in unit_names_used_previously]
     else:
         rows_to_add = []
         for index in rows_in_data:
             if unit_name_array[index] not in unit_names_used_previously:
                 rows_to_add.append(index)
@@ -1287,28 +1043,28 @@
     for row in rows_to_add:
         unit_kwargs = dict(property_to_default_values)
         for property in properties_with_data:
             unit_kwargs[property] = data_to_add[property]["data"][row]
         spike_times = []
 
         # Extract and concatenate the spike times from multiple segments
-        for segment_index in range(checked_sorting.get_num_segments()):
-            segment_spike_times = checked_sorting.get_unit_spike_train(
+        for segment_index in range(sorting.get_num_segments()):
+            segment_spike_times = sorting.get_unit_spike_train(
                 unit_id=unit_ids[row], segment_index=segment_index, return_times=True
             )
             spike_times.append(segment_spike_times)
         spike_times = np.concatenate(spike_times)
         if waveform_means is not None:
             unit_kwargs["waveform_mean"] = waveform_means[row]
             if waveform_sds is not None:
                 unit_kwargs["waveform_sd"] = waveform_sds[row]
             if unit_electrode_indices is not None:
                 unit_kwargs["electrodes"] = unit_electrode_indices[row]
         units_table.add_unit(spike_times=spike_times, **unit_kwargs, enforce_unique_id=True)
-    added_unit_table_ids = units_table.id[-len(rows_to_add) :]
+    # added_unit_table_ids = units_table.id[-len(rows_to_add) :]  # TODO - this line is unused?
 
     # Add unit_name as a column and fill previously existing rows with unit_name equal to str(ids)
     previous_table_size = len(units_table.id[:]) - len(unit_name_array)
     if "unit_name" in properties_to_add_by_columns:
         cols_args = data_to_add["unit_name"]
         data = cols_args["data"]
 
@@ -1325,15 +1081,15 @@
         unit_name: table_df.query(f"unit_name=='{unit_name}'").index[0] for unit_name in unit_name_array
     }
 
     indexes_for_new_data = [unit_name_to_electrode_index[unit_name] for unit_name in unit_name_array]
     indexes_for_default_values = table_df.index.difference(indexes_for_new_data).values
 
     # Add properties as columns
-    for property in properties_to_add_by_columns - set({"unit_name"}):
+    for property in properties_to_add_by_columns - {"unit_name"}:
         cols_args = data_to_add[property]
         data = cols_args["data"]
         if np.issubdtype(data.dtype, np.integer):
             data = data.astype("float")
 
         # Find first matching data-type
         sample_data = data[0]
@@ -1346,140 +1102,36 @@
         extended_data[indexes_for_default_values] = default_value
         # Always store numpy objects as strings
         if np.issubdtype(extended_data.dtype, np.object_):
             extended_data = extended_data.astype("str", copy=False)
         cols_args["data"] = extended_data
         units_table.add_column(property, **cols_args)
 
-    if write_waveforms:
-        assert write_table_first_time, "write_waveforms is not supported with re-write"
-        units_table = _add_waveforms_to_units_table(
-            sorting=sorting,
-            units_table=units_table,
-            row_ids=added_unit_table_ids,
-            skip_features=skip_features,
-        )
-
-
-def _add_waveforms_to_units_table(
-    sorting: SortingExtractor,
-    units_table,
-    row_ids,
-    skip_features: Optional[List[str]] = None,
-):
-    """
-    Auxiliary method for adding waveforms to an existing units_table.
-
-    Parameters
-    ----------
-    sorting :  A spikeextractors SortingExtractor.
-    units_table : a previously created units table
-    skip_features : list of str
-        Each string in this list that matches a spike feature will not be written to the NWBFile.
-    """
-    unit_ids = sorting.get_unit_ids()
-
-    if isinstance(sorting, SortingExtractor):
-        # TODO: Remove spikeextractors backend
-        warn(
-            message=(
-                "Interfaces using a spikeextractors backend will soon be deprecated! "
-                "Please use the SpikeInterface backend instead."
-            ),
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-
-        all_features = set()
-        for unit_id in unit_ids:
-            all_features.update(sorting.get_unit_spike_feature_names(unit_id))
-        if skip_features is None:
-            skip_features = []
-        # Check that multidimensional features have the same shape across units
-        feature_shapes = dict()
-        for feature_name in all_features:
-            shapes = []
-            for unit_id in unit_ids:
-                if feature_name in sorting.get_unit_spike_feature_names(unit_id=unit_id):
-                    feat_value = sorting.get_unit_spike_features(unit_id=unit_id, feature_name=feature_name)
-                    if isinstance(feat_value[0], (int, np.integer, float, str, bool)):
-                        break
-                    elif isinstance(feat_value[0], (list, np.ndarray)):  # multidimensional features
-                        if np.array(feat_value).ndim > 1:
-                            shapes.append(np.array(feat_value).shape)
-                            feature_shapes[feature_name] = shapes
-                    elif isinstance(feat_value[0], dict):
-                        print(f"Skipping feature '{feature_name}' because dictionaries are not supported.")
-                        skip_features.append(feature_name)
-                        break
-                else:
-                    print(f"Skipping feature '{feature_name}' because not share across all units.")
-                    skip_features.append(feature_name)
-                    break
-        nspikes = {k: get_nspikes(units_table, k) for k in row_ids}
-        for feature_name in feature_shapes.keys():
-            # skip first dimension (num_spikes) when comparing feature shape
-            if not np.all([elem[1:] == feature_shapes[feature_name][0][1:] for elem in feature_shapes[feature_name]]):
-                print(f"Skipping feature '{feature_name}' because it has variable size across units.")
-                skip_features.append(feature_name)
-        for feature_name in set(all_features) - set(skip_features):
-            values = []
-            if not feature_name.endswith("_idxs"):
-                for unit_id in sorting.get_unit_ids():
-                    feat_vals = sorting.get_unit_spike_features(unit_id=unit_id, feature_name=feature_name)
-                    if len(feat_vals) < nspikes[unit_id]:
-                        skip_features.append(feature_name)
-                        print(f"Skipping feature '{feature_name}' because it is not defined for all spikes.")
-                        break
-                    else:
-                        all_feat_vals = feat_vals
-                    values.append(all_feat_vals)
-                flatten_vals = [item for sublist in values for item in sublist]
-                nspks_list = [sp for sp in nspikes.values()]
-                spikes_index = np.cumsum(nspks_list).astype("int64")
-                if feature_name in units_table:  # If property already exists, skip it
-                    warnings.warn(f"Feature {feature_name} already present in units table, skipping it")
-                    continue
-                set_dynamic_table_property(
-                    dynamic_table=units_table,
-                    row_ids=[int(k) for k in row_ids],
-                    property_name=feature_name,
-                    values=flatten_vals,
-                    index=spikes_index,
-                )
-    else:
-        """
-        Currently (2022-04-22), spikeinterface does not support waveform features.
-        """
-        pass
-
-    return units_table
-
 
 def write_sorting(
-    sorting: SpikeInterfaceSorting,
-    nwbfile_path: OptionalFilePathType = None,
+    sorting: BaseSorting,
+    nwbfile_path: Optional[FilePathType] = None,
     nwbfile: Optional[pynwb.NWBFile] = None,
     metadata: Optional[dict] = None,
     overwrite: bool = False,
     verbose: bool = True,
     unit_ids: Optional[List[Union[str, int]]] = None,
     property_descriptions: Optional[dict] = None,
     skip_properties: Optional[List[str]] = None,
     skip_features: Optional[List[str]] = None,
-    write_as: str = "units",
+    write_as: Literal["units", "processing"] = "units",
     units_name: str = "units",
     units_description: str = "Autogenerated by neuroconv.",
-):
+) -> NWBFile:
     """
     Primary method for writing a SortingExtractor object to an NWBFile.
 
     Parameters
     ----------
-    sorting : SpikeInterfaceSorting
+    sorting : spikeinterface.BaseSorting
     nwbfile_path : FilePathType, optional
         Path for where to write or load (if overwrite=False) the NWBFile.
         If specified, the context will always write to this location.
     nwbfile : NWBFile, optional
         If passed, this function will fill the relevant fields within the NWBFile object.
         E.g., calling
             write_recording(recording=my_recording_extractor, nwbfile=my_nwbfile)
@@ -1487,29 +1139,28 @@
         If neither 'nwbfile_path' nor 'nwbfile' are specified, an NWBFile object will be automatically generated
         and returned by the function.
     metadata : dict, optional
         Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
     overwrite : bool, default: False
         Whether to overwrite the NWBFile if one exists at the nwbfile_path.
         The default is False (append mode).
-    verbose : bool, optional
+    verbose : bool, default: True
         If 'nwbfile_path' is specified, informs user after a successful write operation.
-        The default is True.
     unit_ids : list, optional
         Controls the unit_ids that will be written to the nwb file. If None (default), all
         units are written.
-    property_descriptions : dict, opptional
+    property_descriptions : dict, optional
         For each key in this dictionary which matches the name of a unit
         property in sorting, adds the value as a description to that
         custom unit column.
     skip_properties : list of str, optional
         Each string in this list that matches a unit property will not be written to the NWBFile.
     skip_features : list of str
         Each string in this list that matches a spike feature will not be written to the NWBFile.
-    write_as : str, default: 'units'
+    write_as : {'units', 'processing'}
         How to save the units table in the nwb file. Options:
         - 'units' will save it to the official NWBFile.Units position; recommended only for the final form of the data.
         - 'processing' will save it to the processing module to serve as a historical provenance for the official table.
     units_name : str, default: 'units'
         The name of the units table. If write_as=='units', then units_name must also be 'units'.
     units_description : str, default: 'Autogenerated by neuroconv.'
     """
@@ -1549,15 +1200,15 @@
     waveform_extractor: WaveformExtractor,
     nwbfile: Optional[pynwb.NWBFile] = None,
     metadata: Optional[dict] = None,
     recording: Optional[BaseRecording] = None,
     unit_ids: Optional[List[Union[str, int]]] = None,
     skip_properties: Optional[List[str]] = None,
     property_descriptions: Optional[dict] = None,
-    write_as: str = "units",
+    write_as: Literal["units", "processing"] = "units",
     units_name: str = "units",
     units_description: str = "Autogenerated by neuroconv.",
 ):
     """
     Primary method for writing a WaveformExtractor object to an NWBFile.
 
     Parameters
@@ -1569,32 +1220,27 @@
             write_recording(recording=my_recording_extractor, nwbfile=my_nwbfile)
         will result in the appropriate changes to the my_nwbfile object.
         If neither 'nwbfile_path' nor 'nwbfile' are specified, an NWBFile object will be automatically generated
         and returned by the function.
     metadata : dict, optional
         Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
         The "Ecephys" section of metadata is also used to create electrodes and electrical series fields.
-    overwrite : bool, default: False
-        Whether to overwrite the NWBFile if one exists at the nwbfile_path.
-        The default is False (append mode).
     recording : BaseRecording, optional
         If the waveform_extractor is 'recordingless', this argument needs to be passed to save electrode info.
         Otherwise, electrodes info is not added to the nwb file.
     unit_ids : list, optional
         Controls the unit_ids that will be written to the nwb file. If None (default), all
         units are written.
-    property_descriptions : dict
+    property_descriptions : dict, optional
         For each key in this dictionary which matches the name of a unit
         property in sorting, adds the value as a description to that
         custom unit column.
-    skip_properties : list of str
+    skip_properties : list of str, optional
         Each string in this list that matches a unit property will not be written to the NWBFile.
-    skip_features : list of str
-        Each string in this list that matches a spike feature will not be written to the NWBFile.
-    write_as : str default: 'units'
+    write_as : {'units', 'processing'}
         How to save the units table in the nwb file. Options:
         - 'units' will save it to the official NWBFile.Units position; recommended only for the final form of the data.
         - 'processing' will save it to the processing module to serve as a historical provenance for the official table.
     units_name : str, optional, default: 'units'
         The name of the units table. If write_as=='units', then units_name must also be 'units'.
     units_description : str, default: 'Autogenerated by neuroconv.'
     """
@@ -1647,72 +1293,68 @@
         waveform_sds=template_stds,
         unit_electrode_indices=unit_electrode_indices,
     )
 
 
 def write_waveforms(
     waveform_extractor: WaveformExtractor,
-    nwbfile_path: OptionalFilePathType = None,
+    nwbfile_path: Optional[FilePathType] = None,
     nwbfile: Optional[pynwb.NWBFile] = None,
     metadata: Optional[dict] = None,
     overwrite: bool = False,
     recording: Optional[BaseRecording] = None,
     verbose: bool = True,
     unit_ids: Optional[List[Union[str, int]]] = None,
     write_electrical_series: bool = False,
     add_electrical_series_kwargs: Optional[dict] = None,
     skip_properties: Optional[List[str]] = None,
     property_descriptions: Optional[dict] = None,
-    write_as: str = "units",
+    write_as: Literal["units", "processing"] = "units",
     units_name: str = "units",
     units_description: str = "Autogenerated by neuroconv.",
 ):
     """
     Primary method for writing a WaveformExtractor object to an NWBFile.
 
     Parameters
     ----------
-    sorting : SortingExtractor
+    waveform_extractor : WaveformExtractor
     nwbfile_path : FilePathType
         Path for where to write or load (if overwrite=False) the NWBFile.
         If specified, the context will always write to this location.
     nwbfile : NWBFile, optional
         If passed, this function will fill the relevant fields within the NWBFile object.
         E.g., calling
             write_recording(recording=my_recording_extractor, nwbfile=my_nwbfile)
         will result in the appropriate changes to the my_nwbfile object.
         If neither 'nwbfile_path' nor 'nwbfile' are specified, an NWBFile object will be automatically generated
         and returned by the function.
     metadata : dict, optional
         Metadata dictionary with information used to create the NWBFile when one does not exist or overwrite=True.
         The "Ecephys" section of metadata is also used to create electrodes and electrical series fields.
-    overwrite : bool, optional
-        Whether or not to overwrite the NWBFile if one exists at the nwbfile_path.
-        The default is False (append mode).
+    overwrite : bool, default: False
+        Whether to overwrite the NWBFile if one exists at the nwbfile_path.
     recording : BaseRecording, optional
         If the waveform_extractor is 'recordingless', this argument needs to be passed to save electrode info.
         Otherwise, electrodes info is not added to the nwb file.
-    verbose : bool, optional
+    verbose : bool, default: True
         If 'nwbfile_path' is specified, informs user after a successful write operation.
-        The default is True.
     unit_ids : list, optional
         Controls the unit_ids that will be written to the nwb file. If None (default), all
         units are written.
     write_electrical_series : bool, default: False
         If True, the recording object associated to the WaveformExtractor is written as an electrical series.
     add_electrical_series_kwargs: dict, optional
         Keyword arguments to control the `add_electrical_series()` function in case write_electrical_series=True
     property_descriptions: dict, optional
         For each key in this dictionary which matches the name of a unit
         property in sorting, adds the value as a description to that
         custom unit column.
     skip_properties: list of str, optional
         Each string in this list that matches a unit property will not be written to the NWBFile.
-    skip_features: list of str, optional
-        Each string in this list that matches a spike feature will not be written to the NWBFile.
     write_as: {'units', 'processing'}
         How to save the units table in the nwb file. Options:
         - 'units' will save it to the official NWBFile.Units position; recommended only for the final form of the data.
         - 'processing' will save it to the processing module to serve as a historical provenance for the official table.
     units_name : str, default: 'units'
         The name of the units table. If write_as=='units', then units_name must also be 'units'.
     units_description : str, default: 'Autogenerated by neuroconv.'
@@ -1760,17 +1402,17 @@
     if group_names is None:
         electrode_group_indices = None
     else:
         electrode_group_indices = nwbfile.electrodes.to_dataframe().query(f"group_name in {group_names}").index.values
     return electrode_group_indices
 
 
-def waveform_extractor_has_recording(waveform_extractor) -> bool:
+def waveform_extractor_has_recording(waveform_extractor) -> bool:  # TODO - this can probably be replaced now
     """
-    Temporary helper function to substitute unreleased built-in waveform_extractor.has_recording()
+    Temporary helper function to substitute unreleased built-in waveform_extractor.has_recording().
 
     Parameters
     ----------
     waveform_extractor : si.WaveformExtractor
         The waveform extractor
 
     Returns
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py` & `neuroconv-0.3.0/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-"""Authors: Cody Baker and Saksham Sharda."""
-from typing import Tuple, Iterable, Optional, Union
+from typing import Iterable, Optional, Tuple, Union
 from warnings import warn
 
-from spikeinterface.core.old_api_utils import OldToNewRecording
-from spikeextractors import RecordingExtractor
 from hdmf.data_utils import GenericDataChunkIterator
 from spikeinterface import BaseRecording
 
-SpikeInterfaceRecording = Union[BaseRecording, RecordingExtractor]
-
 
 class SpikeInterfaceRecordingDataChunkIterator(GenericDataChunkIterator):
     """DataChunkIterator specifically for use on RecordingExtractor objects."""
 
     def __init__(
         self,
-        recording: SpikeInterfaceRecording,
+        recording: BaseRecording,
         segment_index: int = 0,
         return_scaled: bool = False,
         buffer_gb: Optional[float] = None,
         buffer_shape: Optional[tuple] = None,
         chunk_mb: Optional[float] = None,
         chunk_shape: Optional[tuple] = None,
         display_progress: bool = False,
@@ -60,27 +55,15 @@
             The default is None.
         display_progress : bool, optional
             Display a progress bar with iteration rate and estimated completion time.
         progress_bar_options : dict, optional
             Dictionary of keyword arguments to be passed directly to tqdm.
             See https://github.com/tqdm/tqdm#parameters for options.
         """
-        if isinstance(recording, RecordingExtractor):
-            self.recording = OldToNewRecording(oldapi_recording_extractor=recording)
-            # TODO: Remove spikeextractors backend
-            warn(
-                message=(
-                    "Interfaces using a spikeextractors backend will soon be deprecated! "
-                    "Please use the SpikeInterface backend instead."
-                ),
-                category=DeprecationWarning,
-                stacklevel=2,
-            )
-        else:
-            self.recording = recording
+        self.recording = recording
         self.segment_index = segment_index
         self.return_scaled = return_scaled
         self.channel_ids = recording.get_channel_ids()
         super().__init__(
             buffer_gb=buffer_gb,
             buffer_shape=buffer_shape,
             chunk_mb=chunk_mb,
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/testing/mock_ttl_signals.py` & `neuroconv-0.3.0/src/neuroconv/tools/testing/mock_ttl_signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""Author: Cody Baker."""
-from typing import Optional, Union
 from pathlib import Path
+from typing import Optional, Union
 
 import numpy as np
 from numpy.typing import DTypeLike
 from nwbinspector.tools import make_minimal_nwbfile
 from nwbinspector.utils import is_module_installed
-from pynwb import NWBHDF5IO, TimeSeries, H5DataIO
+from pynwb import NWBHDF5IO, H5DataIO, TimeSeries
 
 from ...utils import ArrayType, FolderPathType
 
 
 def _check_parameter_dtype_consistency(
     parameter_name: str,
     parameter_value: Union[int, float],
@@ -109,15 +108,16 @@
     num_frames = np.ceil(signal_duration * sampling_frequency_hz).astype(int)
     trace = (np.random.randn(num_frames) * channel_noise + baseline_mean).astype(dtype)
 
     if ttl_times is not None:
         ttl_times = np.array(ttl_times)
     else:
         ttl_times = np.arange(start=1.0, stop=signal_duration, step=2.0)
-    assert not any(
+
+    assert len(ttl_times) == 1 or not any(  # np.diff errors out when len(ttl_times) < 2
         np.diff(ttl_times) <= ttl_duration
     ), "There are overlapping TTL 'on' intervals! Please specify disjoint on/off periods."
 
     ttl_start_frames = np.round(ttl_times * sampling_frequency_hz).astype(int)
     num_frames_ttl_duration = np.round(ttl_duration * sampling_frequency_hz).astype(int)
     ttl_intervals = (slice(start, start + num_frames_ttl_duration) for start in ttl_start_frames)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/text.py` & `neuroconv-0.3.0/src/neuroconv/tools/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Dict
 
 import numpy as np
 import pandas as pd
 from pynwb.epoch import TimeIntervals
 
 
 def convert_df_to_time_intervals(
```

### Comparing `neuroconv-0.2.4/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py` & `neuroconv-0.3.0/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-"""Authors: Cody Baker, Alessio Buccino."""
 import sys
-from pathlib import Path
 from importlib import import_module
-from itertools import chain
-from jsonschema import validate, RefResolver
+from pathlib import Path
 from typing import Optional
-from warnings import warn
 
 import click
-from dandi.organize import create_unique_filenames_from_metadata
 from dandi.metadata import _get_pynwb_metadata
+from dandi.organize import create_unique_filenames_from_metadata
+from jsonschema import RefResolver, validate
 
 from ...nwbconverter import NWBConverter
-from ...utils import dict_deep_update, load_dict_from_file, FilePathType, OptionalFolderPathType
+from ...utils import FilePathType, FolderPathType, dict_deep_update, load_dict_from_file
 
 
 @click.command()
 @click.argument("specification-file-path")
 @click.option(
     "--data-folder-path",
     help="Path to folder where the source data may be found.",
@@ -47,19 +44,17 @@
         output_folder_path=output_folder_path,
         overwrite=overwrite,
     )
 
 
 def run_conversion_from_yaml(
     specification_file_path: FilePathType,
-    data_folder_path: OptionalFolderPathType = None,
-    output_folder_path: OptionalFolderPathType = None,
+    data_folder_path: Optional[FolderPathType] = None,
+    output_folder_path: Optional[FolderPathType] = None,
     overwrite: bool = False,
-    data_folder: OptionalFolderPathType = None,
-    output_folder: OptionalFolderPathType = None,
 ):
     """
     Run conversion to NWB given a yaml specification file.
 
     Parameters
     ----------
     specification_file_path : FilePathType
@@ -70,90 +65,67 @@
     output_folder_path : FolderPathType, optional
         Folder path leading to the desired output location of the .nwb files.
         The default is the parent directory of the specification_file_path.
     overwrite : bool, default: False
         If True, replaces any existing NWBFile at the nwbfile_path location, if save_to_file is True.
         If False, appends the existing NWBFile at the nwbfile_path location, if save_to_file is True.
     """
-    deprecation_warning_string = (
-        "'data_folder' and 'output_folder' keyword arguments are deprecated and will be removed on or before "
-        "August 2022! Please use 'data_folder_path' and 'output_folder_path' instead."
-    )
-    if data_folder is not None:
-        assert data_folder_path is None, "Cannot specify both 'data_folder' and 'data_folder_path'. "
-        "Please use 'data_folder_path'."
-        data_folder_path = data_folder
-        warn(deprecation_warning_string)
-    if output_folder is not None:
-        assert output_folder_path is None, "Cannot specify both 'output_folder' and 'output_folder_path'. "
-        "Please use 'output_folder_path'."
-        output_folder_path = output_folder
-        warn(deprecation_warning_string)
 
     if data_folder_path is None:
         data_folder_path = Path(specification_file_path).parent
     if output_folder_path is None:
         output_folder_path = Path(specification_file_path).parent
     else:
         output_folder_path = Path(output_folder_path)
     specification = load_dict_from_file(file_path=specification_file_path)
     schema_folder = Path(__file__).parent.parent.parent / "schemas"
     specification_schema = load_dict_from_file(file_path=schema_folder / "yaml_conversion_specification_schema.json")
-    sys_uri_base = "file://"
-    if sys.platform.startswith("win32"):
-        sys_uri_base = "file:/"
+    sys_uri_base = "file:/" if sys.platform.startswith("win32") else "file://"
     validate(
         instance=specification,
         schema=specification_schema,
         resolver=RefResolver(base_uri=sys_uri_base + str(schema_folder) + "/", referrer=specification_schema),
     )
 
     global_metadata = specification.get("metadata", dict())
-    global_data_interfaces = specification.get("data_interfaces")
-    neuroconv_datainterfaces = import_module(name=".datainterfaces", package="neuroconv")
+    global_conversion_options = specification.get("conversion_options", dict())
+    data_interfaces_spec = specification.get("data_interfaces")
+    data_interfaces_module = import_module(name=".datainterfaces", package="neuroconv")
+    data_interface_classes = {key: getattr(data_interfaces_module, name) for key, name in data_interfaces_spec.items()}
+
+    CustomNWBConverter = type(
+        "CustomNWBConverter", (NWBConverter,), dict(data_interface_classes=data_interface_classes)
+    )
+
     file_counter = 0
     for experiment in specification["experiments"].values():
         experiment_metadata = experiment.get("metadata", dict())
-        experiment_data_interfaces = experiment.get("data_interfaces")
         for session in experiment["sessions"]:
             file_counter += 1
-            session_data_interfaces = session.get("data_interfaces")
-            data_interface_classes = dict()
-            data_interfaces_names_chain = chain(
-                *[
-                    data_interfaces
-                    for data_interfaces in [global_data_interfaces, experiment_data_interfaces, session_data_interfaces]
-                    if data_interfaces is not None
-                ]
-            )
-            for data_interface_name in data_interfaces_names_chain:
-                data_interface_classes.update(
-                    {data_interface_name: getattr(neuroconv_datainterfaces, data_interface_name)}
-                )
-            CustomNWBConverter = type(
-                "CustomNWBConverter", (NWBConverter,), dict(data_interface_classes=data_interface_classes)
-            )
-
             source_data = session["source_data"]
             for interface_name, interface_source_data in session["source_data"].items():
                 for key, value in interface_source_data.items():
                     if key == "file_paths":
                         source_data[interface_name].update({key: [str(Path(data_folder_path) / x) for x in value]})
-                    else:
+                    elif key in ("file_path", "folder_path"):
                         source_data[interface_name].update({key: str(Path(data_folder_path) / value)})
             converter = CustomNWBConverter(source_data=source_data)
             metadata = converter.get_metadata()
             for metadata_source in [global_metadata, experiment_metadata, session.get("metadata", dict())]:
                 metadata = dict_deep_update(metadata, metadata_source)
             nwbfile_name = session.get("nwbfile_name", f"temp_nwbfile_name_{file_counter}").strip(".nwb")
+            session_conversion_options = session.get("conversion_options", dict())
+            conversion_options = dict()
+            for key in converter.data_interface_objects:
+                conversion_options[key] = dict(session_conversion_options.get(key, dict()), **global_conversion_options)
             converter.run_conversion(
                 nwbfile_path=output_folder_path / f"{nwbfile_name}.nwb",
                 metadata=metadata,
                 overwrite=overwrite,
-                conversion_options=session.get("conversion_options", dict()),
+                conversion_options=conversion_options,
             )
     # To properly mimic a true dandi organization, the full directory must be populated with NWBFiles.
     all_nwbfile_paths = [nwbfile_path for nwbfile_path in output_folder_path.iterdir() if nwbfile_path.suffix == ".nwb"]
     if any(["temp_nwbfile_name_" in nwbfile_path.stem for nwbfile_path in all_nwbfile_paths]):
         dandi_metadata_list = []
         for nwbfile_path in all_nwbfile_paths:
             dandi_metadata = _get_pynwb_metadata(path=nwbfile_path)
```

### Comparing `neuroconv-0.2.4/src/neuroconv/utils/checks.py` & `neuroconv-0.3.0/src/neuroconv/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.2.4/src/neuroconv/utils/dict.py` & `neuroconv-0.3.0/src/neuroconv/utils/dict.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-"""Authors: Luiz Tauffer, Cody Baker, Saksham Sharda and Ben Dichter."""
 import collections.abc
-import warnings
 import json
+import warnings
+from collections import defaultdict
 from copy import deepcopy
+from ctypes import Union
 from pathlib import Path
+from typing import Any, Optional, Union
 
-import yaml
 import numpy as np
+import yaml
 
 from .types import FilePathType
 
 
 class NoDatesSafeLoader(yaml.SafeLoader):
     """Custom override of yaml Loader class for datetime considerations."""
 
@@ -108,15 +110,15 @@
     d: collections.abc.Mapping,
     u: collections.abc.Mapping,
     append_list: bool = True,
     remove_repeats: bool = True,
     copy: bool = True,
     compare_key: str = "name",
     list_dict_deep_update: bool = True,
-) -> dict:
+) -> collections.abc.Mapping:
     """
     Perform an update to all nested keys of dictionary d(input) from dictionary u(updating dict).
 
     Parameters
     ----------
     d: dict
         dictionary to update
@@ -136,15 +138,15 @@
             >>> d = {
                 [
                     {"name": "timeseries1", "desc": "desc1 of d", "starting_time": 0.0},
                     {"name": "timeseries2", "desc": "desc2"},
                 ]
             }
             >>> u = [{"name": "timeseries1", "desc": "desc2 of u", "unit": "n.a."}]
-            >>> # if compre_key='name' output is below
+            >>> # if compare_key='name' output is below
             >>> output = [
                 {"name": "timeseries1", "desc": "desc2 of u", "starting_time": 0.0, "unit": "n.a."},
                 {"name": "timeseries2", "desc": "desc2"},
             ]
             >>> # else the output is:
             >>> # dict with the same key will be updated instead of being appended to the list
             >>> output = [
@@ -195,7 +197,50 @@
                     dict_or_list_of_dicts, value, compare_key, list_dict_deep_update, remove_repeats
                 )
         # Update with something else
         else:
             dict_to_update[key_to_update] = update_values
 
     return dict_to_update
+
+
+class DeepDict(defaultdict):
+    """A defaultdict of defaultdicts"""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(lambda: DeepDict(), *args, **kwargs)
+        for key, value in self.items():
+            if isinstance(value, dict):
+                self[key] = DeepDict(value)
+
+    def deep_update(self, other: Optional[Union[dict, "DeepDict"]] = None, **kwargs) -> None:
+        for key, value in (other or kwargs).items():
+            if key in self and isinstance(self[key], dict) and isinstance(value, dict):
+                self[key].deep_update(value)
+            else:
+                self[key] = value
+
+    def to_dict(self) -> dict:
+        """Turn a DeepDict into a normal dictionary"""
+
+        def _to_dict(d: Union[dict, "DeepDict"]) -> dict:
+            return {key: _to_dict(value) for key, value in d.items()} if isinstance(d, dict) else d
+
+        return _to_dict(self)
+
+    def __deepcopy__(self, memodict={}):
+        """
+
+        Parameters
+        ----------
+        memodict: dict
+            unused
+
+        Returns
+        -------
+        DeepDict
+
+        """
+        return DeepDict(deepcopy(self.to_dict()))
+
+    def __repr__(self) -> str:
+        return "DeepDict: " + dict.__repr__(self.to_dict())
```

### Comparing `neuroconv-0.2.4/src/neuroconv/utils/json_schema.py` & `neuroconv-0.3.0/src/neuroconv/utils/json_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Authors: Luiz Tauffer, Cody Baker, Saksham Sharda and Ben Dichter."""
 import collections.abc
-import json
 import inspect
+import json
 from datetime import datetime
-import numpy as np
+from typing import Callable, Literal
 
+import hdmf.data_utils
+import numpy as np
 import pynwb
 from pynwb.device import Device
 from pynwb.icephys import IntracellularElectrode
 
 from .dict import dict_deep_update
 from .types import FilePathType, FolderPathType
 
@@ -44,25 +45,27 @@
         base_schema.update({"$schema": "http://json-schema.org/draft-07/schema#"})
     if id_:
         base_schema.update({"$id": id_})
     base_schema.update(**kwargs)
     return base_schema
 
 
-def get_schema_from_method_signature(class_method: classmethod, exclude: list = None) -> dict:
+def get_schema_from_method_signature(method: Callable, exclude: list = None) -> dict:
     """
     Take a class method and return a json-schema of the input args.
 
     Parameters
     ----------
-    class_method: function
+    method: function
     exclude: list, optional
+
     Returns
     -------
     dict
+
     """
     if exclude is None:
         exclude = ["self", "kwargs"]
     else:
         exclude = exclude + ["self", "kwargs"]
     input_schema = get_base_schema()
     annotation_json_type_map = dict(
@@ -72,75 +75,91 @@
         float="number",
         dict="object",
         list="array",
         tuple="array",
         FilePathType="string",
         FolderPathType="string",
     )
-    for param_name, param in inspect.signature(class_method).parameters.items():
-        if param_name not in exclude:
-            if param.annotation:
-                if hasattr(param.annotation, "__args__"):  # Annotation has __args__ if it was made by typing.Union
-                    args = param.annotation.__args__
-                    valid_args = [x.__name__ in annotation_json_type_map for x in args]
-                    if any(valid_args):
-                        param_types = [annotation_json_type_map[x.__name__] for x in np.array(args)[valid_args]]
-                    else:
-                        raise ValueError("No valid arguments were found in the json type mapping!")
-                    num_params = len(set(param_types))
-                    conflict_message = (
-                        "Conflicting json parameter types were detected from the annotation! "
-                        f"{param.annotation.__args__} found."
-                    )
-                    # Normally cannot support Union[...] of multiple annotation types
-                    if num_params > 2:
-                        raise ValueError(conflict_message)
-                    # Special condition for Optional[...]
-                    if num_params == 2 and not args[1] is type(None):  # noqa: E721
-                        raise ValueError(conflict_message)
-                    param_type = param_types[0]
+    args_spec = dict()
+    for param_name, param in inspect.signature(method).parameters.items():
+        if param_name in exclude:
+            continue
+        args_spec[param_name] = dict()
+        if param.annotation:
+            if getattr(param.annotation, "__origin__", None) == Literal:
+                args_spec[param_name]["enum"] = list(param.annotation.__args__)
+            elif getattr(param.annotation, "__origin__", None) == dict:
+                args_spec[param_name] = dict(type="object")
+                if param.annotation.__args__ == (str, str):
+                    args_spec[param_name].update(additionalProperties={"^.*$": dict(type="string")})
                 else:
-                    arg = param.annotation
-                    if arg.__name__ in annotation_json_type_map:
-                        param_type = annotation_json_type_map[arg.__name__]
-                    else:
-                        raise ValueError(
-                            f"No valid arguments were found in the json type mapping {arg} for parameter {param}"
-                        )
-                    if arg == FilePathType:
-                        input_schema["properties"].update({param_name: dict(format="file")})
-                    if arg == FolderPathType:
-                        input_schema["properties"].update({param_name: dict(format="directory")})
-            else:
-                raise NotImplementedError(
-                    f"The annotation type of '{param}' in function '{class_method}' is not implemented! "
-                    "Please request it to be added at github.com/catalystneuro/nwb-conversion-tools/issues "
-                    "or create the json-schema for this method manually."
+                    args_spec[param_name].update(additionalProperties=True)
+            elif hasattr(param.annotation, "__args__"):  # Annotation has __args__ if it was made by typing.Union
+                args = param.annotation.__args__
+                valid_args = [x.__name__ in annotation_json_type_map for x in args]
+                if any(valid_args):
+                    param_types = [annotation_json_type_map[x.__name__] for x in np.array(args)[valid_args]]
+                else:
+                    raise ValueError(f"No valid arguments were found in the json type mapping for parameter {param}")
+                num_params = len(set(param_types))
+                conflict_message = (
+                    "Conflicting json parameter types were detected from the annotation! "
+                    f"{param.annotation.__args__} found."
                 )
-            arg_spec = {param_name: dict(type=param_type)}
-            if param.default is param.empty:
-                input_schema["required"].append(param_name)
-            elif param.default is not None:
-                arg_spec[param_name].update(default=param.default)
-            input_schema["properties"] = dict_deep_update(input_schema["properties"], arg_spec)
+                # Normally cannot support Union[...] of multiple annotation types
+                if num_params > 2:
+                    raise ValueError(conflict_message)
+                # Special condition for Optional[...]
+                if num_params == 2 and not args[1] is type(None):  # noqa: E721
+                    raise ValueError(conflict_message)
+                args_spec[param_name]["type"] = param_types[0]
+            else:
+                arg = param.annotation
+                if arg.__name__ in annotation_json_type_map:
+                    args_spec[param_name]["type"] = annotation_json_type_map[arg.__name__]
+                else:
+                    raise ValueError(
+                        f"No valid arguments were found in the json type mapping '{arg}' for parameter {param}"
+                    )
+                if arg == FilePathType:
+                    input_schema["properties"].update({param_name: dict(format="file")})
+                if arg == FolderPathType:
+                    input_schema["properties"].update({param_name: dict(format="directory")})
+        else:
+            raise NotImplementedError(
+                f"The annotation type of '{param}' in function '{method}' is not implemented! "
+                "Please request it to be added at github.com/catalystneuro/nwb-conversion-tools/issues "
+                "or create the json-schema for this method manually."
+            )
+        if param.default is param.empty:
+            input_schema["required"].append(param_name)
+        elif param.default is not None:
+            args_spec[param_name].update(default=param.default)
+        input_schema["properties"] = dict_deep_update(input_schema["properties"], args_spec)
         input_schema["additionalProperties"] = param.kind == inspect.Parameter.VAR_KEYWORD
     return input_schema
 
 
 def fill_defaults(schema: dict, defaults: dict, overwrite: bool = True):
     """
     Insert the values of the defaults dict as default values in the schema in place.
 
     Parameters
     ----------
     schema: dict
     defaults: dict
     overwrite: bool
     """
-    for key, val in schema["properties"].items():
+    # patternProperties introduced with the CsvTimeIntervalsInterface
+    # caused issue with NWBConverter.get_metadata_schema() call leading here
+    properties_reference = "properties"
+    if properties_reference not in schema and "patternProperties" in schema:
+        properties_reference = "patternProperties"
+
+    for key, val in schema[properties_reference].items():
         if key in defaults:
             if val["type"] == "object":
                 fill_defaults(val, defaults[key], overwrite=overwrite)
             else:
                 if overwrite or ("default" not in val):
                     val["default"] = defaults[key]
 
@@ -184,14 +203,19 @@
         elif docval_arg["type"] is str or (isinstance(docval_arg["type"], tuple) and str in docval_arg["type"]):
             schema_arg[docval_arg["name"]].update(type="string")
         # type array
         elif docval_arg["type"] is collections.abc.Iterable or (
             isinstance(docval_arg["type"], tuple) and collections.abc.Iterable in docval_arg["type"]
         ):
             schema_arg[docval_arg["name"]].update(type="array")
+        elif isinstance(docval_arg["type"], tuple) and (
+            np.ndarray in docval_arg["type"] and hdmf.data_utils.DataIO not in docval_arg["type"]
+        ):
+            # extend type array without including type where DataIO in tuple
+            schema_arg[docval_arg["name"]].update(type="array")
         # type datetime
         elif docval_arg["type"] is datetime or (
             isinstance(docval_arg["type"], tuple) and datetime in docval_arg["type"]
         ):
             schema_arg[docval_arg["name"]].update(type="string", format="date-time")
         # if TimeSeries, skip it
         elif docval_arg["type"] is pynwb.base.TimeSeries or (
@@ -230,84 +254,14 @@
             schema["required"].append(docval_arg["name"])
         schema["properties"].update(schema_arg)
     if "allow_extra" in docval:
         schema["additionalProperties"] = docval["allow_extra"]
     return schema
 
 
-# TODO - centralize into schema folder
-def get_schema_for_NWBFile():
-    schema = get_base_schema()
-    schema["tag"] = "pynwb.file.NWBFile"
-    schema["required"] = ["session_description", "identifier", "session_start_time"]
-    schema["properties"] = {
-        "session_description": {
-            "type": "string",
-            "format": "long",
-            "description": "a description of the session where this data was generated",
-        },
-        "identifier": {"type": "string", "description": "a unique text identifier for the file"},
-        "session_start_time": {
-            "type": "string",
-            "description": "the start date and time of the recording session",
-            "format": "date-time",
-        },
-        "experimenter": {
-            "type": "array",
-            "items": {"type": "string", "title": "experimenter"},
-            "description": "name of person who performed experiment",
-        },
-        "experiment_description": {"type": "string", "description": "general description of the experiment"},
-        "session_id": {"type": "string", "description": "lab-specific ID for the session"},
-        "institution": {"type": "string", "description": "institution(s) where experiment is performed"},
-        "notes": {"type": "string", "description": "Notes about the experiment."},
-        "pharmacology": {
-            "type": "string",
-            "description": "Description of drugs used, including how and when they were administered. Anesthesia(s), "
-            "painkiller(s), etc., plus dosage, concentration, etc.",
-        },
-        "protocol": {
-            "type": "string",
-            "description": "Experimental protocol, if applicable. E.g., include IACUC protocol",
-        },
-        "related_publications": {
-            "type": "string",
-            "description": "Publication information.PMID, DOI, URL, etc. If multiple, concatenate together and describe"
-            " which is which. such as PMID, DOI, URL, etc",
-        },
-        "slices": {
-            "type": "string",
-            "description": "Description of slices, including information about preparation thickness, orientation, "
-            "temperature and bath solution",
-        },
-        "source_script": {"type": "string", "description": "Script file used to create this NWB file."},
-        "source_script_file_name": {"type": "string", "description": "Name of the source_script file"},
-        "data_collection": {"type": "string", "description": "Notes about data collection and analysis."},
-        "surgery": {
-            "type": "string",
-            "description": (
-                "Narrative description about surgery/surgeries, including date(s) and who performed surgery."
-            ),
-        },
-        "virus": {
-            "type": "string",
-            "description": "Information about virus(es) used in experiments, including virus ID, source, date made, "
-            "injection location, volume, etc.",
-        },
-        "stimulus_notes": {"type": "string", "description": "Notes about stimuli, such as how and where presented."},
-        "lab": {"type": "string", "description": "lab where experiment was performed"},
-        "keywords": {
-            "description": "Terms to search over",
-            "type": "array",
-            "items": {"title": "keyword", "type": "string"},
-        },
-    }
-    return schema
-
-
 def get_metadata_schema_for_icephys():
     schema = get_base_schema(tag="Icephys")
     schema["required"] = ["Device", "Electrode"]
     schema["properties"] = dict(
         Device=dict(type="array", minItems=1, items={"$ref": "#/properties/Icephys/properties/definitions/Device"}),
         Electrode=dict(
             type="array",
```

### Comparing `neuroconv-0.2.4/src/neuroconv.egg-info/SOURCES.txt` & `neuroconv-0.3.0/src/neuroconv.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-LICENSE
 MANIFEST.in
 README.md
 base_gin_test_config.json
 codecov.yml
+license.txt
 make_environment.yml
 pyproject.toml
 setup.py
 src/neuroconv/__init__.py
 src/neuroconv/basedatainterface.py
 src/neuroconv/baseextractorinterface.py
+src/neuroconv/basetemporalalignmentinterface.py
 src/neuroconv/nwbconverter.py
 src/neuroconv.egg-info/PKG-INFO
 src/neuroconv.egg-info/SOURCES.txt
 src/neuroconv.egg-info/dependency_links.txt
 src/neuroconv.egg-info/entry_points.txt
 src/neuroconv.egg-info/requires.txt
 src/neuroconv.egg-info/top_level.txt
+src/neuroconv/converters/__init__.py
 src/neuroconv/datainterfaces/__init__.py
 src/neuroconv/datainterfaces/behavior/__init__.py
 src/neuroconv/datainterfaces/behavior/audio/__init__.py
 src/neuroconv/datainterfaces/behavior/audio/audiointerface.py
 src/neuroconv/datainterfaces/behavior/deeplabcut/__init__.py
 src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py
 src/neuroconv/datainterfaces/behavior/sleap/__init__.py
@@ -38,64 +40,72 @@
 src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py
 src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py
 src/neuroconv/datainterfaces/ecephys/biocam/__init__.py
 src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py
 src/neuroconv/datainterfaces/ecephys/blackrock/__init__.py
 src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py
 src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py
-src/neuroconv/datainterfaces/ecephys/ced/__init__.py
-src/neuroconv/datainterfaces/ecephys/ced/ceddatainterface.py
 src/neuroconv/datainterfaces/ecephys/cellexplorer/__init__.py
 src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py
 src/neuroconv/datainterfaces/ecephys/edf/__init__.py
 src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py
 src/neuroconv/datainterfaces/ecephys/intan/__init__.py
 src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py
 src/neuroconv/datainterfaces/ecephys/kilosort/__init__.py
 src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py
+src/neuroconv/datainterfaces/ecephys/maxwell/__init__.py
+src/neuroconv/datainterfaces/ecephys/maxwell/maxonedatainterface.py
 src/neuroconv/datainterfaces/ecephys/mcsraw/__init__.py
 src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py
 src/neuroconv/datainterfaces/ecephys/mearec/__init__.py
 src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py
 src/neuroconv/datainterfaces/ecephys/neuralynx/__init__.py
 src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py
 src/neuroconv/datainterfaces/ecephys/neuroscope/__init__.py
 src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py
 src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py
 src/neuroconv/datainterfaces/ecephys/openephys/__init__.py
+src/neuroconv/datainterfaces/ecephys/openephys/openephysbinarydatainterface.py
 src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py
+src/neuroconv/datainterfaces/ecephys/openephys/openephyslegacydatainterface.py
+src/neuroconv/datainterfaces/ecephys/openephys/openephyssortingdatainterface.py
 src/neuroconv/datainterfaces/ecephys/phy/__init__.py
 src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py
 src/neuroconv/datainterfaces/ecephys/plexon/__init__.py
 src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py
+src/neuroconv/datainterfaces/ecephys/spike2/__init__.py
+src/neuroconv/datainterfaces/ecephys/spike2/spike2datainterface.py
 src/neuroconv/datainterfaces/ecephys/spikegadgets/__init__.py
 src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py
 src/neuroconv/datainterfaces/ecephys/spikeglx/__init__.py
 src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py
+src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxconverter.py
 src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py
 src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py
-src/neuroconv/datainterfaces/ecephys/spikeinterface/__init__.py
-src/neuroconv/datainterfaces/ecephys/spikeinterface/sipickledatainterfaces.py
 src/neuroconv/datainterfaces/ecephys/tdt/__init__.py
 src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py
 src/neuroconv/datainterfaces/icephys/__init__.py
 src/neuroconv/datainterfaces/icephys/baseicephysinterface.py
 src/neuroconv/datainterfaces/icephys/abf/__init__.py
 src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py
 src/neuroconv/datainterfaces/ophys/__init__.py
 src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py
 src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py
+src/neuroconv/datainterfaces/ophys/brukertiff/__init__.py
+src/neuroconv/datainterfaces/ophys/brukertiff/brukertiffdatainterface.py
 src/neuroconv/datainterfaces/ophys/caiman/__init__.py
 src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py
 src/neuroconv/datainterfaces/ophys/cnmfe/__init__.py
 src/neuroconv/datainterfaces/ophys/cnmfe/cnmfedatainterface.py
 src/neuroconv/datainterfaces/ophys/extract/__init__.py
 src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py
 src/neuroconv/datainterfaces/ophys/hdf5/__init__.py
 src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py
+src/neuroconv/datainterfaces/ophys/micromanagertiff/__init__.py
+src/neuroconv/datainterfaces/ophys/micromanagertiff/micromanagertiffdatainterface.py
 src/neuroconv/datainterfaces/ophys/sbx/__init__.py
 src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py
 src/neuroconv/datainterfaces/ophys/scanimage/__init__.py
 src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py
 src/neuroconv/datainterfaces/ophys/sima/__init__.py
 src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py
 src/neuroconv/datainterfaces/ophys/suite2p/__init__.py
@@ -104,39 +114,45 @@
 src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py
 src/neuroconv/datainterfaces/text/__init__.py
 src/neuroconv/datainterfaces/text/timeintervalsinterface.py
 src/neuroconv/datainterfaces/text/csv/__init__.py
 src/neuroconv/datainterfaces/text/csv/csvtimeintertervalsinterface.py
 src/neuroconv/datainterfaces/text/excel/__init__.py
 src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py
+src/neuroconv/schemas/base_metadata_schema.json
 src/neuroconv/schemas/metadata_schema.json
 src/neuroconv/schemas/source_schema.json
+src/neuroconv/schemas/time_series_schema.json
 src/neuroconv/schemas/yaml_conversion_specification_schema.json
 src/neuroconv/tools/__init__.py
 src/neuroconv/tools/data_transfers.py
 src/neuroconv/tools/figshare.py
 src/neuroconv/tools/hdmf.py
 src/neuroconv/tools/importing.py
 src/neuroconv/tools/nwb_helpers.py
+src/neuroconv/tools/path_expansion.py
+src/neuroconv/tools/processes.py
 src/neuroconv/tools/signal_processing.py
 src/neuroconv/tools/text.py
 src/neuroconv/tools/audio/__init__.py
 src/neuroconv/tools/audio/audio.py
 src/neuroconv/tools/neo/__init__.py
 src/neuroconv/tools/neo/neo.py
 src/neuroconv/tools/roiextractors/__init__.py
 src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py
 src/neuroconv/tools/roiextractors/roiextractors.py
 src/neuroconv/tools/spikeinterface/__init__.py
 src/neuroconv/tools/spikeinterface/spikeinterface.py
 src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py
 src/neuroconv/tools/testing/__init__.py
+src/neuroconv/tools/testing/_path_expander_demo_ibl_filepaths.txt
+src/neuroconv/tools/testing/data_interface_mixins.py
+src/neuroconv/tools/testing/mock_files.py
 src/neuroconv/tools/testing/mock_interfaces.py
 src/neuroconv/tools/testing/mock_ttl_signals.py
 src/neuroconv/tools/yaml_conversion_specification/__init__.py
 src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py
 src/neuroconv/utils/__init__.py
 src/neuroconv/utils/checks.py
 src/neuroconv/utils/dict.py
-src/neuroconv/utils/globbing.py
 src/neuroconv/utils/json_schema.py
 src/neuroconv/utils/types.py
```

