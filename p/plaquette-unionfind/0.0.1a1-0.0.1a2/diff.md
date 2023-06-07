# Comparing `tmp/plaquette_unionfind-0.0.1a1-cp311-cp311-win_amd64.whl.zip` & `tmp/plaquette_unionfind-0.0.1a2-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1119614 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   647680 b- defN 23-Jun-06 06:42 Debug/plaquette_unionfind_bindings.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat  5263360 b- defN 23-Jun-06 06:42 Debug/plaquette_unionfind_bindings.pdb
--rw-rw-rw-  2.0 fat      232 b- defN 23-Jun-06 06:35 plaquette_unionfind/__init__.py
--rw-rw-rw-  2.0 fat     3652 b- defN 23-Jun-06 06:35 plaquette_unionfind/unionfind.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 06:42 plaquette_unionfind-0.0.1a1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8387 b- defN 23-Jun-06 06:42 plaquette_unionfind-0.0.1a1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-06 06:42 plaquette_unionfind-0.0.1a1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-06 06:41 plaquette_unionfind-0.0.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      845 b- defN 23-Jun-06 06:42 plaquette_unionfind-0.0.1a1.dist-info/RECORD
-9 files, 5935865 bytes uncompressed, 1118140 bytes compressed:  81.2%
+Zip file size: 1119704 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   647680 b- defN 23-Jun-06 07:46 Debug/plaquette_unionfind_bindings.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  5263360 b- defN 23-Jun-06 07:46 Debug/plaquette_unionfind_bindings.pdb
+-rw-rw-rw-  2.0 fat      232 b- defN 23-Jun-06 07:42 plaquette_unionfind/__init__.py
+-rw-rw-rw-  2.0 fat     3652 b- defN 23-Jun-06 07:42 plaquette_unionfind/unionfind.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 07:46 plaquette_unionfind-0.0.1a2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8647 b- defN 23-Jun-06 07:46 plaquette_unionfind-0.0.1a2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-06 07:46 plaquette_unionfind-0.0.1a2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-06 07:46 plaquette_unionfind-0.0.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      845 b- defN 23-Jun-06 07:46 plaquette_unionfind-0.0.1a2.dist-info/RECORD
+9 files, 5936125 bytes uncompressed, 1118230 bytes compressed:  81.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: plaquette_unionfind/__init__.py
 Comment: 
 
 Filename: plaquette_unionfind/unionfind.py
 Comment: 
 
-Filename: plaquette_unionfind-0.0.1a1.dist-info/LICENSE
+Filename: plaquette_unionfind-0.0.1a2.dist-info/LICENSE
 Comment: 
 
-Filename: plaquette_unionfind-0.0.1a1.dist-info/METADATA
+Filename: plaquette_unionfind-0.0.1a2.dist-info/METADATA
 Comment: 
 
-Filename: plaquette_unionfind-0.0.1a1.dist-info/WHEEL
+Filename: plaquette_unionfind-0.0.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: plaquette_unionfind-0.0.1a1.dist-info/top_level.txt
+Filename: plaquette_unionfind-0.0.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: plaquette_unionfind-0.0.1a1.dist-info/RECORD
+Filename: plaquette_unionfind-0.0.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plaquette_unionfind/__init__.py

```diff
@@ -1,6 +1,6 @@
 """Interface to UnionFind decoder from the plaquette C++ backend"""
 from .unionfind import UnionFindDecoderInterface
 from .unionfind import UnionFindDecoder
 from .unionfind import PeelingDecoder
 
-__version__ = "0.0.1-alpha.1"
+__version__ = "0.0.1-alpha.2"
```

## Comparing `plaquette_unionfind-0.0.1a1.dist-info/LICENSE` & `plaquette_unionfind-0.0.1a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plaquette_unionfind-0.0.1a1.dist-info/METADATA` & `plaquette_unionfind-0.0.1a2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plaquette-unionfind
-Version: 0.0.1a1
+Version: 0.0.1a2
 Project-URL: Homepage, https://docs.plaquette.design/projects/unionfind
 Project-URL: Bug Tracker, https://github.com/qc-design/plaquette-unionfind/issues
 Keywords: Quantum error correction,qec,quantum computing,fault tolerance,error decoding
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -157,37 +157,39 @@
             "pauli": {q.equbit_idx: {"x": error_rate} for q in code.lattice.dataqubits}
         }
         decoder = plaquette_unionfind.UnionFindDecoderInterface.from_code(code, qed, weighted=False)
     
 Benchmarks
 ==========
 
-For our benchmarks, we have been careful to only time the intrinsic Pymatching-v2 and FusionBlossom decoding
-functions. We do not use the decode_batch function for Pymatching-v2 because this does not test the intrinsic speed of the
-decoder. We also set FusionBlossom to single-threaded mode since we are running both our code and Pymatching-v2 in that mode.
-All benchmarks are performed on a m6id.4xlarge AWS node. All benchmarks are reproducible (see below) using our scripts on
-a m6id.4xlarge.
+We benchmark plaquette-unionfind along with two of the leading open source decorders `PyMatching-v2 <https://arxiv.org/abs/2303.15933>`_ 
+and `FusionBlosson <https://arxiv.org/abs/2305.08307>`_. 
+
+For our benchmarks, we have been careful to only time the intrinsic PyMatching and FusionBlossom decoding
+functions. Only the intrinsic speed of the decoder was timed, so e.g., we do not yet benchmark along with 
+the decode_batch function for Pymatching-v2. We also set FusionBlossom to single-threaded mode for a fair 
+comparison with PyMatching and plaquette-unionfind. All benchmarks are performed on a m6id.4xlarge AWS node. 
+All benchmarks are reproducible (see below) using our scripts on a m6id.4xlarge.
 
 For our first benchmark, we use the 2-D (perfect measurement) Planar Code with p = 0.05 depolarization
-error. We see around 8-10x speedup over competitors
+error. We observe up to 8-10x speedup over PyMatching and FusionBlossom.
 
 .. image:: https://github.com/qc-design/plaquette-unionfind/blob/40fb8fab11ad60e281089e3b0b26865c899749cb/benchmarks/perfect_planar_0.05.png?raw=true
    :align: center
    :width: 500px 
 
-For our second benchmark we use the 3-D (imperfect measurement) Rotated Planar Code with p = 0.01 depolarization
-error and p = 0.01 measurement error. We see that Pymatching-v2 is much more sensitive to the lattice size.
+For our second benchmark we use the 3-D Rotated Planar Code to account for measurement errors, with p = 0.01 depolarization
+error and p = 0.01 measurement error. We observe that Pymatching is more sensitive to the lattice size than the other decoders.
 
 .. image:: https://github.com/qc-design/plaquette-unionfind/blob/40fb8fab11ad60e281089e3b0b26865c899749cb/benchmarks/imperfect_rotated_planar_0.01.png?raw=true
    :align: center
    :width: 500px 
 
-
-Finally we benchmark a 30x30 Rotated Planar Code (29 rounds of measurement) with varying probability. We see that
-fusion-blossom is heavily sensitive to the error probability.
+Finally we benchmark a 30x30 Rotated Planar Code (29 rounds of measurement) with varying probability. We observe that
+FusionBlossom is sensitive to the error probability.
 
 .. image:: https://github.com/qc-design/plaquette-unionfind/blob/40fb8fab11ad60e281089e3b0b26865c899749cb/benchmarks/imperfect_rotated_planar_fixed_size.png?raw=true
    :align: center
    :width: 500px 
 
 To run all three benchmarks, use the following bash commands:
```

## Comparing `plaquette_unionfind-0.0.1a1.dist-info/RECORD` & `plaquette_unionfind-0.0.1a2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Debug/plaquette_unionfind_bindings.cp311-win_amd64.pyd,sha256=BqQBFo8Tc3Id-LshDppTbxRygT9KkK6lbD6VYrVmRuU,647680
+Debug/plaquette_unionfind_bindings.cp311-win_amd64.pyd,sha256=elikTdscR_rwVL2HTUZYT7Dr6AWue6rSLF5V5CSPsgY,647680
 Debug/plaquette_unionfind_bindings.pdb,sha256=2tkjK7rBZ6pI5Bmv_kNQMA3hTj3d7u59748J97KUoX0,5263360
-plaquette_unionfind/__init__.py,sha256=qchPQj3CQ7j6-YT8RFR_xvNN7UL0KNLV6k2zLJXePp4,232
+plaquette_unionfind/__init__.py,sha256=vBj4eUBjSeT72eL5i8OUSt90qoPa6c547X1pn_3fhws,232
 plaquette_unionfind/unionfind.py,sha256=bqyr5JHQJLSlx6DullLiMVPBlDo0p_Lg2Q7VbPUuvDg,3652
-plaquette_unionfind-0.0.1a1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-plaquette_unionfind-0.0.1a1.dist-info/METADATA,sha256=0r-ImZK0_0H3ldkYVgxxqSGvOwjytU-1MswH4-toTmk,8387
-plaquette_unionfind-0.0.1a1.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-plaquette_unionfind-0.0.1a1.dist-info/top_level.txt,sha256=BR7yqN2eJOhw-YlCSgb3bmvPyjWvSmLXgVAfsylRKbU,49
-plaquette_unionfind-0.0.1a1.dist-info/RECORD,,
+plaquette_unionfind-0.0.1a2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+plaquette_unionfind-0.0.1a2.dist-info/METADATA,sha256=sSXrK4SuR3usRy-Tf9jk6t42TIMdlkoxA77HDHFA-Qo,8647
+plaquette_unionfind-0.0.1a2.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+plaquette_unionfind-0.0.1a2.dist-info/top_level.txt,sha256=BR7yqN2eJOhw-YlCSgb3bmvPyjWvSmLXgVAfsylRKbU,49
+plaquette_unionfind-0.0.1a2.dist-info/RECORD,,
```

