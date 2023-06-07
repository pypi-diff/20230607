# Comparing `tmp/omnisoot-0.1.1-cp39-cp39-win_amd64.whl.zip` & `tmp/omnisoot-0.1.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2457777 bytes, number of entries: 34
+Zip file size: 2486288 bytes, number of entries: 36
 -rw-rw-rw-  2.0 fat      556 b- defN 23-May-31 02:05 eptlsoot/__init__.py
 -rw-rw-rw-  2.0 fat  1465856 b- defN 23-Apr-05 21:26 eptlsoot/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     6093 b- defN 23-Apr-05 21:43 eptlsoot/cpfr.py
 -rw-rw-rw-  2.0 fat      679 b- defN 23-Apr-05 21:38 eptlsoot/eptlsoot.py
 -rw-rw-rw-  2.0 fat      644 b- defN 23-Apr-05 21:43 eptlsoot/psr.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-05 04:38 eptlsoot/apps/__init__.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-May-24 15:14 eptlsoot/apps/flame.py
@@ -17,20 +17,22 @@
 -rw-rw-rw-  2.0 fat  1468928 b- defN 23-Apr-05 21:11 eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      527 b- defN 23-Jun-01 02:54 omnisoot/__init__.py
 -rw-rw-rw-  2.0 fat     6093 b- defN 23-May-31 12:31 omnisoot/cpfr.py
 -rw-rw-rw-  2.0 fat      679 b- defN 23-May-31 12:31 omnisoot/omnisoot.py
 -rw-rw-rw-  2.0 fat      644 b- defN 23-May-31 12:31 omnisoot/psr.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-05 04:38 omnisoot/apps/__init__.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-May-31 12:31 omnisoot/apps/flame.py
--rw-rw-rw-  2.0 fat     1843 b- defN 23-May-31 12:31 omnisoot/apps/pahgrowth.py
+-rw-rw-rw-  2.0 fat     2043 b- defN 23-Jun-06 15:23 omnisoot/apps/pahgrowth.py
 -rw-rw-rw-  2.0 fat    10461 b- defN 23-Jun-01 02:53 omnisoot/apps/reactors.py
 -rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-05 04:46 omnisoot/apps/solutionarray.py
 -rw-rw-rw-  2.0 fat     4044 b- defN 23-May-31 12:31 omnisoot/apps/sootgas.py
--rw-rw-rw-  2.0 fat      950 b- defN 23-May-31 12:31 omnisoot/apps/sootmodels.py
+-rw-rw-rw-  2.0 fat     1900 b- defN 23-Jun-01 22:16 omnisoot/apps/sootmodels.py
 -rw-rw-rw-  2.0 fat     5993 b- defN 23-May-31 12:31 omnisoot/apps/sootwrappers.py
 -rw-rw-rw-  2.0 fat      239 b- defN 23-May-31 12:31 omnisoot/apps/surfacereactions.py
--rw-rw-rw-  2.0 fat  1866752 b- defN 23-Jun-01 13:28 omnisoot/lib/_omnisoot.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      772 b- defN 23-Jun-01 13:28 omnisoot-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-01 13:28 omnisoot-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-01 13:27 omnisoot-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2789 b- defN 23-Jun-01 13:28 omnisoot-0.1.1.dist-info/RECORD
-34 files, 6736723 bytes uncompressed, 2453343 bytes compressed:  63.6%
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 14:09 omnisoot/apps/reactors_/__init__.py
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-06 14:11 omnisoot/apps/reactors_/psr.py
+-rw-rw-rw-  2.0 fat  1954304 b- defN 23-Jun-07 05:08 omnisoot/lib/_omnisoot.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2057 b- defN 23-Jun-07 05:08 omnisoot-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-07 05:08 omnisoot-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-07 05:07 omnisoot-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2965 b- defN 23-Jun-07 05:08 omnisoot-0.1.2.dist-info/RECORD
+36 files, 6826917 bytes uncompressed, 2481572 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -81,23 +81,29 @@
 
 Filename: omnisoot/apps/sootwrappers.py
 Comment: 
 
 Filename: omnisoot/apps/surfacereactions.py
 Comment: 
 
+Filename: omnisoot/apps/reactors_/__init__.py
+Comment: 
+
+Filename: omnisoot/apps/reactors_/psr.py
+Comment: 
+
 Filename: omnisoot/lib/_omnisoot.cp39-win_amd64.pyd
 Comment: 
 
-Filename: omnisoot-0.1.1.dist-info/METADATA
+Filename: omnisoot-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: omnisoot-0.1.1.dist-info/WHEEL
+Filename: omnisoot-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: omnisoot-0.1.1.dist-info/top_level.txt
+Filename: omnisoot-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: omnisoot-0.1.1.dist-info/RECORD
+Filename: omnisoot-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnisoot/apps/pahgrowth.py

```diff
@@ -1,8 +1,8 @@
-from ..lib._omnisoot import CReactDim, CDimerCoal, CCrossLink, CCrossLinkMod, CCrossLinkMerge
+from ..lib._omnisoot import CReactDim, CDimerCoal, CCrossLink, CCrossLinkMod, CCrossLinkMerge, CIrrevDim
 
 class PAHGrowthAbstract:
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
 
     def set_precursor_names(self, precursor_list):
@@ -44,8 +44,13 @@
 
 
 class CrossLinkMerge(PAHGrowthAbstract, CCrossLinkMerge):
     serialized_name = "CrossLinkMerge"
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
-PAH_GROWTH_MODELS = [ReactDim, DimerCoal, CrossLink, CrossLinkMod, CrossLinkMerge]
+class IrrevDim(PAHGrowthAbstract, CIrrevDim):
+    serialized_name = "IrreversibleDimerization"
+    def __init__(self, soot_wrapper):
+        super().__init__(soot_wrapper);
+
+PAH_GROWTH_MODELS = [ReactDim, DimerCoal, CrossLink, CrossLinkMod, CrossLinkMerge, IrrevDim]
```

## omnisoot/apps/sootmodels.py

```diff
@@ -1,8 +1,9 @@
-from ..lib._omnisoot import CMonodisperseSootModel
+from ..lib._omnisoot import CMonodisperseSootModel, CMonodisperseCoalesceSootModel
+
 class MonodisperseSootModel(CMonodisperseSootModel):
     serialized_name = "Monodisperse"
     soot_att = ["N_agg", "N_pri", "H_tot", "C_tot", "A_tot",
               "d_p", "d_m", "d_g", "d_v", "n_p",
               "SSA", "total_mass", "volume_fraction",
               "carbon_mass", "hydrogen_mass",
               "inception_mass", "inception_vol",
@@ -17,8 +18,30 @@
         super().__init__(soot_wrapper);
 
     def det_soot_att(self, name):
         if name in self.soot_att:
             att_func = getattr(self, name);
             return att_func();
 
-SOOT_MODELS = [MonodisperseSootModel]
+class MonodisperseSootCoalesceModel(CMonodisperseCoalesceSootModel):
+    serialized_name = "MonodisperseCoalesce"
+    soot_att = ["N_agg", "N_pri", "H_tot", "C_tot", "A_tot",
+              "d_p", "d_m", "d_g", "d_v", "n_p",
+              "SSA", "total_mass", "volume_fraction",
+              "carbon_mass", "hydrogen_mass",
+              "inception_mass", "inception_vol",
+              "PAH_adsorption_mass", "PAH_adsorption_vol",
+              "surface_growth_mass", "surface_growth_vol",
+              "oxidation_mass", "oxidation_vol",
+              "coagulation_mass", "coagulation_vol",
+              "min_array"
+              ]
+    
+    def __init__(self, soot_wrapper):
+        super().__init__(soot_wrapper);
+
+    def det_soot_att(self, name):
+        if name in self.soot_att:
+            att_func = getattr(self, name);
+            return att_func();
+
+SOOT_MODELS = [MonodisperseSootModel, MonodisperseSootCoalesceModel]
```

## Comparing `omnisoot-0.1.1.dist-info/RECORD` & `omnisoot-0.1.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd,sha256=_ZuT4TUsgcE1q80t6Dpxopn37BhJUZsMZcqBhaRKFiM,1468928
 omnisoot/__init__.py,sha256=icQ0nQ2y1B6Dso3e1ygztRIFBvWP06MmC7nX_fFH8yo,527
 omnisoot/cpfr.py,sha256=xFQv12SM3syCwom0HMoNxobCV-bcnETupPmOUTgDcpU,6093
 omnisoot/omnisoot.py,sha256=ZIMyVmZ9ct1fIzW-yAG9fkEjdRXY8oLaRLi5WkEoEmY,679
 omnisoot/psr.py,sha256=BsWn_vupqnpCQzaJPoOIRHBfukoc9Y0vje42dEMFeFA,644
 omnisoot/apps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 omnisoot/apps/flame.py,sha256=Zg9CxaQIMwrK0RkirXHLnXnXlIi4OLzzEdUVvMe1UeA,1047
-omnisoot/apps/pahgrowth.py,sha256=OEWaKhdMDmqyUwgmlrDx08abKorR_7qPhJQ4zBTuBLk,1843
+omnisoot/apps/pahgrowth.py,sha256=8xLR-MAh4DNgXcmIuGQ9SYfDfeZFC7YSz6uJRDgKqj4,2043
 omnisoot/apps/reactors.py,sha256=ed-ssqGGI-1HUFrpFFwotgMX25wWJkCqr-MTCL55sig,10461
 omnisoot/apps/solutionarray.py,sha256=gGyAu8LnGNU3CuDvae8rXD3TrEnAanYeWOa1QErsV8U,265
 omnisoot/apps/sootgas.py,sha256=zN88OOxFAYxSTIkhES2EIKZRcSkPWEtImX-DujF8E20,4044
-omnisoot/apps/sootmodels.py,sha256=vQzzM37OsI0awcETawB9xae66E1b1CcNLKNr3sk_a0s,950
+omnisoot/apps/sootmodels.py,sha256=Ts77fMwWQ5t9wRlFZrcSb3AAQtpLHOQkKAODCBMMBBk,1900
 omnisoot/apps/sootwrappers.py,sha256=YFhbFT2JUGmlMKkT9eSfZa0_IMU1sjpB331_G5xv1eM,5993
 omnisoot/apps/surfacereactions.py,sha256=5zgz_HKCeGgBW6L1nYUp_mFEFIgjDQchT3ZejRGV2BY,239
-omnisoot/lib/_omnisoot.cp39-win_amd64.pyd,sha256=CZ-YzZePWcuD54qSKv130XFs0PaI2HsEVD11u6XfZFY,1866752
-omnisoot-0.1.1.dist-info/METADATA,sha256=4Wiam8eED_yoFByappDoNUj9RSsWNSgd_2SI0gwXy8I,772
-omnisoot-0.1.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-omnisoot-0.1.1.dist-info/top_level.txt,sha256=k7bKrgnA_SQG4D5xcsVXUOdVMLes9lFzeDbvtIw7oAo,9
-omnisoot-0.1.1.dist-info/RECORD,,
+omnisoot/apps/reactors_/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+omnisoot/apps/reactors_/psr.py,sha256=HvWLBLXQzl_OyzMW46HH7Xft-YrSV6dOs4RwapHCRzw,31
+omnisoot/lib/_omnisoot.cp39-win_amd64.pyd,sha256=HeXx5HBngw3Axg_JaGTOcqL4zeiwLdg3WWgPPwlmqL0,1954304
+omnisoot-0.1.2.dist-info/METADATA,sha256=q1dwYYuMT0Sd4WNcgXp33ZN40GYGKnByGxWhCw_Oy9Y,2057
+omnisoot-0.1.2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+omnisoot-0.1.2.dist-info/top_level.txt,sha256=k7bKrgnA_SQG4D5xcsVXUOdVMLes9lFzeDbvtIw7oAo,9
+omnisoot-0.1.2.dist-info/RECORD,,
```

