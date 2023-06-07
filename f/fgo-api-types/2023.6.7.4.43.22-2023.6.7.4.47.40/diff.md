# Comparing `tmp/fgo_api_types-2023.6.7.4.43.22.tar.gz` & `tmp/fgo_api_types-2023.6.7.4.47.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.6.7.4.43.22.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.6.7.4.47.40.tar", max compression
```

## Comparing `fgo_api_types-2023.6.7.4.43.22.tar` & `fgo_api_types-2023.6.7.4.47.40.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-06-07 04:43:01.173698 fgo_api_types-2023.6.7.4.43.22/LICENSE
--rw-r--r--   0        0        0      449 2023-06-07 04:43:01.173698 fgo_api_types-2023.6.7.4.43.22/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157892 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    76333 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50619 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-06-07 04:43:23.013691 fgo_api_types-2023.6.7.4.43.22/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.7.4.43.22/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-07 04:47:20.334114 fgo_api_types-2023.6.7.4.47.40/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-07 04:47:20.334114 fgo_api_types-2023.6.7.4.47.40/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   158848 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    76421 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50619 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-06-07 04:47:40.826154 fgo_api_types-2023.6.7.4.47.40/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.7.4.47.40/PKG-INFO
```

### Comparing `fgo_api_types-2023.6.7.4.43.22/LICENSE` & `fgo_api_types-2023.6.7.4.47.40/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/basic.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/common.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/enums.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/gameenums.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/gameenums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1571,17 +1571,19 @@
     IgnoreValueUp = 122
     ApplyValueUp = 123
     ActNoDamageBuff = 124
     ActSelectIndex = 125
     CopyTargetBuffType = 126
     NotSkillCopyTargetFuncIds = 127
     NotSkillCopyTargetIndividualities = 128
-    IntervalTurn = 129
-    IntervalCount = 130
-    TargetEnemyRange = 131
+    ClassIconAuraEffectId = 129
+    ActMasterGenderType = 130
+    IntervalTurn = 131
+    IntervalCount = 132
+    TargetEnemyRange = 133
 
 
 class ClassRelationOverwriteType(IntEnum):
     OVERWRITE_FORCE = 0
     OVERWRITE_MORE_THAN_TARGET = 1
     OVERWRITE_LESS_THAN_TARGET = 2
 
@@ -1631,14 +1633,15 @@
     CONTINUE_ITEM = 27
     EUQIP_SKILL_USE_ITEM = 28
     SVT_COIN = 29
     FRIENDSHIP_UP_ITEM = 30
     PP = 31
     TRADE_AP = 32
     RI = 33
+    STORMPOD = 34
 
 
 class NiceItemType(StrEnum):
     """Item Type Enum"""
 
     qp = "qp"
     stone = "stone"
@@ -1669,14 +1672,15 @@
     continueItem = "continueItem"
     euqipSkillUseItem = "euqipSkillUseItem"
     svtCoin = "svtCoin"
     friendshipUpItem = "friendshipUpItem"
     pp = "pp"
     tradeAp = "tradeAp"
     ri = "ri"
+    stormpod = "stormpod"
 
 
 ITEM_TYPE_NAME: dict[int, NiceItemType] = {
     1: NiceItemType.qp,
     2: NiceItemType.stone,
     3: NiceItemType.apRecover,
     4: NiceItemType.apAdd,
@@ -1705,14 +1709,15 @@
     27: NiceItemType.continueItem,
     28: NiceItemType.euqipSkillUseItem,
     29: NiceItemType.svtCoin,
     30: NiceItemType.friendshipUpItem,
     31: NiceItemType.pp,
     32: NiceItemType.tradeAp,
     33: NiceItemType.ri,
+    34: NiceItemType.stormpod,
 }
 
 
 class GiftType(IntEnum):
     SERVANT = 1
     ITEM = 2
     FRIENDSHIP = 3
@@ -2168,15 +2173,21 @@
     EVENT_TUTORIAL_FLAG_OFF = 171
     EVENT_SUPER_BOSS_VALUE_EQUAL = 172
     NOT_EVENT_SUPER_BOSS_VALUE_EQUAL = 173
     ALL_SVT_TARGET_SKILL_LV_NUM = 174
     SUPER_BOSS_DAMAGE_ABOVE = 175
     SUPER_BOSS_DAMAGE_BELOW = 176
     EVENT_MISSION_GROUP_ACHIEVE = 177
+    SVT_FRIENDSHIP_CLASS_NUM_ABOVE = 178
     NOT_WAR_CLEAR = 179
+    SVT_SKILL_LV_CLASS_NUM_ABOVE = 180
+    SVT_CLASS_LV_UP_COUNT = 181
+    SVT_CLASS_SKILL_LV_UP_COUNT = 182
+    SVT_CLASS_LIMIT_UP_COUNT = 183
+    SVT_CLASS_FRIENDSHIP_COUNT = 184
 
 
 class NiceCondType(StrEnum):
     """Condition Type Enum"""
 
     none = "none"
     questClear = "questClear"
@@ -2349,15 +2360,21 @@
     eventTutorialFlagOff = "eventTutorialFlagOff"
     eventSuperBossValueEqual = "eventSuperBossValueEqual"
     notEventSuperBossValueEqual = "notEventSuperBossValueEqual"
     allSvtTargetSkillLvNum = "allSvtTargetSkillLvNum"
     superBossDamageAbove = "superBossDamageAbove"
     superBossDamageBelow = "superBossDamageBelow"
     eventMissionGroupAchieve = "eventMissionGroupAchieve"
+    svtFriendshipClassNumAbove = "svtFriendshipClassNumAbove"
     notWarClear = "notWarClear"
+    svtSkillLvClassNumAbove = "svtSkillLvClassNumAbove"
+    svtClassLvUpCount = "svtClassLvUpCount"
+    svtClassSkillLvUpCount = "svtClassSkillLvUpCount"
+    svtClassLimitUpCount = "svtClassLimitUpCount"
+    svtClassFriendshipCount = "svtClassFriendshipCount"
 
 
 COND_TYPE_NAME: dict[int, NiceCondType] = {
     0: NiceCondType.none,
     1: NiceCondType.questClear,
     2: NiceCondType.itemGet,
     3: NiceCondType.useItemEternity,
@@ -2528,15 +2545,21 @@
     171: NiceCondType.eventTutorialFlagOff,
     172: NiceCondType.eventSuperBossValueEqual,
     173: NiceCondType.notEventSuperBossValueEqual,
     174: NiceCondType.allSvtTargetSkillLvNum,
     175: NiceCondType.superBossDamageAbove,
     176: NiceCondType.superBossDamageBelow,
     177: NiceCondType.eventMissionGroupAchieve,
+    178: NiceCondType.svtFriendshipClassNumAbove,
     179: NiceCondType.notWarClear,
+    180: NiceCondType.svtSkillLvClassNumAbove,
+    181: NiceCondType.svtClassLvUpCount,
+    182: NiceCondType.svtClassSkillLvUpCount,
+    183: NiceCondType.svtClassLimitUpCount,
+    184: NiceCondType.svtClassFriendshipCount,
 }
 
 
 class VoiceCondType(IntEnum):
     BIRTH_DAY = 1
     EVENT = 2
     FRIENDSHIP = 3
```

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/nice.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,16 @@
     IgnoreValueUp: int | None = None
     ApplyValueUp: list[str] | None = None
     ActNoDamageBuff: int | None = None
     ActSelectIndex: int | None = None
     CopyTargetBuffType: list[int] | None = None
     NotSkillCopyTargetFuncIds: list[int] | None = None
     NotSkillCopyTargetIndividualities: list[int] | None = None
+    ClassIconAuraEffectId: int | None = None
+    ActMasterGenderType: int | None = None
     IntervalTurn: int | None = None
     IntervalCount: int | None = None
     TargetEnemyRange: list[int] | None = None
     # Extra dataval from SkillLvEntty.DIC_KEY_APPLY_SUPPORT_SVT
     ApplySupportSvt: Optional[int] = None
     # These are not DataVals but guesses from SkillLvEntity and EventDropUpValInfo
     Individuality: Optional[int] = None
```

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/raw.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/rayshift.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/search.py` & `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.43.22/pyproject.toml` & `fgo_api_types-2023.6.7.4.47.40/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.06.07.04.43.22"
+version = "2023.06.07.04.47.40"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.6.7.4.43.22/PKG-INFO` & `fgo_api_types-2023.6.7.4.47.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.6.7.4.43.22
+Version: 2023.6.7.4.47.40
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

