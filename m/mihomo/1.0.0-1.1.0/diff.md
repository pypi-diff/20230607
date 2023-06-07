# Comparing `tmp/mihomo-1.0.0.tar.gz` & `tmp/mihomo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mihomo-1.0.0.tar", max compression
+gzip compressed data, was "mihomo-1.1.0.tar", max compression
```

## Comparing `mihomo-1.0.0.tar` & `mihomo-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.0.0/LICENSE
--rw-r--r--   0        0        0       75 2023-05-31 12:58:50.520388 mihomo-1.0.0/mihomo/__init__.py
--rw-r--r--   0        0        0     9671 2023-06-01 05:02:47.326835 mihomo-1.0.0/mihomo/api.py
--rw-r--r--   0        0        0     3125 2023-06-01 04:57:45.363361 mihomo-1.0.0/mihomo/model.py
--rw-r--r--   0        0        0      439 2023-06-01 05:18:02.694340 mihomo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1285 2023-06-01 05:17:31.781091 mihomo-1.0.0/README.md
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 mihomo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.1.0/LICENSE
+-rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.1.0/mihomo/__init__.py
+-rw-r--r--   0        0        0     9743 2023-06-07 08:48:35.687054 mihomo-1.1.0/mihomo/api.py
+-rw-r--r--   0        0        0     3075 2023-06-07 08:17:47.615390 mihomo-1.1.0/mihomo/model.py
+-rw-r--r--   0        0        0      479 2023-06-07 08:49:53.637921 mihomo-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.1.0/README.md
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.1.0/PKG-INFO
```

### Comparing `mihomo-1.0.0/LICENSE` & `mihomo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mihomo-1.0.0/mihomo/api.py` & `mihomo-1.1.0/mihomo/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "elements.json",
     "properties.json",
     "avatars.json",
 }
 
 
 class MihomoApi:
-    language: Language = Language.EN
+    language = Language.EN
     i18n: bool = False
     index_path = Path.cwd() / "data" / "index"
     res_url = "https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/"
     api_url = "https://api.mihomo.me/sr_info/"
     proxy: Optional[str] = None
     index: Dict[str, Index] = {}
 
@@ -73,19 +73,17 @@
 
     async def ensure_index(self):
         if not self.i18n:
             for file in file_set:
                 if not (self.index_path / self.language.value / file).exists():
                     if not (await self.download_index(file, self.language.value)):
                         raise Exception(
-                            f"Download index {file} of {self.language} failed."
+                            f"Download index {file} of {self.language.value} failed."
                         )
-            self.index[self.language.value] = Index(
-                self.index_path / self.language.value
-            )
+            self.index[self.language] = Index(self.index_path / self.language.value)
         else:
             for language in Language:
                 for file in file_set:
                     if not (self.index_path / language.value / file).exists():
                         if not (await self.download_index(file, language.value)):
                             raise Exception(
                                 f"Download index {file} of {language} failed."
@@ -98,14 +96,15 @@
         if not response:
             return False
         folder = Path(self.index_path / language)
         if not folder.exists():
             folder.mkdir(parents=True)
         with open(folder / file, "wb") as f:
             f.write(response.content)
+        print(f"Succeed to download: {language} index {file}.")
         return True
 
     async def request(self, url):
         params = {}
         headers = {"User-Agent": "Mar-7th/mihomo.py"}
         if self.proxy:
             params["proxies"] = {"https": self.proxy, "http": self.proxy}
@@ -119,54 +118,54 @@
             if response.status_code != 200:
                 return None
             return response
 
     def character_parse(
         self, data: CharacterData, language: Optional[Language] = None
     ) -> Optional[CharacterInfo]:
-        if data.EquipmentID:
+        if data.equipment:
             light_cone = LightConeBasicInfo(
-                id=str(data.EquipmentID.ID),
-                rank=data.EquipmentID.Rank,
-                level=data.EquipmentID.Level,
-                promotion=data.EquipmentID.Promotion,
+                id=str(data.equipment.tid),
+                rank=data.equipment.rank,
+                level=data.equipment.level,
+                promotion=data.equipment.promotion,
             )
         else:
             light_cone = None
         relics = []
-        for relic in data.RelicList:
+        for relic in data.relicList:
             sub_affix = []
-            for affix in relic.RelicSubAffix:
+            for affix in relic.subAffixList:
                 sub_affix.append(
                     SubAffixInfo(
-                        id=str(affix.SubAffixID),
-                        cnt=affix.Cnt,
-                        step=affix.Step,
+                        id=str(affix.affixId),
+                        cnt=affix.cnt,
+                        step=affix.step,
                     )
                 )
             relic_data = RelicBasicInfo(
-                id=str(relic.ID),
-                level=relic.Level,
-                main_affix_id=str(relic.MainAffixID),
+                id=str(relic.tid),
+                level=relic.level,
+                main_affix_id=str(relic.mainAffixId),
                 sub_affix_info=sub_affix,
             )
             relics.append(relic_data)
         skill_tree_levels = []
-        for behavior in data.BehaviorList:
+        for behavior in data.skillTreeList:
             skill_tree_levels.append(
                 LevelInfo(
-                    id=str(behavior.BehaviorID),
-                    level=behavior.Level,
+                    id=str(behavior.pointId),
+                    level=behavior.level,
                 )
             )
         character_basic = CharacterBasicInfo(
-            id=str(data.AvatarID),
-            rank=data.Rank,
-            level=data.Level,
-            promotion=data.Promotion,
+            id=str(data.avatarId),
+            rank=data.rank,
+            level=data.level,
+            promotion=data.promotion,
             skill_tree_levels=skill_tree_levels,
             light_cone=light_cone,
             relics=relics,
         )
         if not language:
             language = self.language
         character = self.index[language.value].get_character_info(character_basic)
@@ -186,73 +185,77 @@
         api_data = decode(data, type=MihomoApiData)
         return api_data
 
     async def get_parsed_api_data(
         self, uid: str, language: Optional[Language] = None
     ) -> Optional[FormattedApiInfo]:
         api_data = await self.get_api_data(uid)
+        return await self.parse_api_data(api_data, language)
+
+    async def parse_api_data(
+        self, api_data: Optional[MihomoApiData], language: Optional[Language] = None
+    ) -> Optional[FormattedApiInfo]:
         if not api_data:
             return None
-        if not api_data.PlayerDetailInfo:
+        if not api_data.detailInfo:
             return None
         if not language:
             language = self.language
-        if self.language.value not in self.index:
+        if self.language not in self.index:
             await self.ensure_index()
         avatar = self.index[language.value].avatars.get(
-            str(api_data.PlayerDetailInfo.HeadIconID)
+            str(api_data.detailInfo.headIcon)
         )
         player_info = PlayerInfo(
-            uid=str(api_data.PlayerDetailInfo.UID),
-            nickname=api_data.PlayerDetailInfo.NickName,
-            level=api_data.PlayerDetailInfo.Level,
-            world_level=api_data.PlayerDetailInfo.WorldLevel,
-            friend_count=api_data.PlayerDetailInfo.CurFriendCount,
+            uid=str(api_data.detailInfo.uid),
+            nickname=api_data.detailInfo.nickname,
+            level=api_data.detailInfo.level,
+            world_level=api_data.detailInfo.worldLevel,
+            friend_count=api_data.detailInfo.friendCount,
             avatar=AvatarInfo(
-                id=str(api_data.PlayerDetailInfo.HeadIconID),
+                id=str(api_data.detailInfo.headIcon),
                 name=avatar.name if avatar else "",
                 icon=avatar.icon if avatar else "",
             ),
-            signature=api_data.PlayerDetailInfo.Signature,
-            birthday=api_data.PlayerDetailInfo.Birthday,
-            is_display=api_data.PlayerDetailInfo.IsDisplayAvatarList,
+            signature=api_data.detailInfo.signature,
+            is_display=api_data.detailInfo.isDisplayAvatar,
         )
-        if api_data.PlayerDetailInfo.PlayerSpaceInfo:
-            space_info = api_data.PlayerDetailInfo.PlayerSpaceInfo
+        if api_data.detailInfo.recordInfo:
+            space_info = api_data.detailInfo.recordInfo
             if space_info:
-                if space_info.ChallengeData:
+                if space_info.challengeInfo:
                     challenge_info = SpaceChallengeInfo(
-                        maze_group_id=space_info.ChallengeData.MazeGroupID,
-                        maze_group_index=space_info.ChallengeData.MazeGroupIndex,
-                        pre_maze_group_index=space_info.ChallengeData.PreMazeGroupIndex,
+                        maze_group_id=space_info.challengeInfo.scheduleGroupId,
+                        maze_group_index=space_info.challengeInfo.scheduleMaxLevel,
+                        pre_maze_group_index=space_info.challengeInfo.noneScheduleMaxLevel,
                     )
                 else:
                     challenge_info = None
                 player_info.space_info = SpaceInfo(
                     challenge_data=challenge_info,
-                    pass_area_progress=space_info.PassAreaProgress,
-                    light_cone_count=space_info.LightConeCount,
-                    avatar_count=space_info.AvatarCount,
-                    achievement_count=space_info.AchievementCount,
+                    pass_area_progress=space_info.maxRogueChallengeScore,
+                    light_cone_count=space_info.equipmentCount,
+                    avatar_count=space_info.avatarCount,
+                    achievement_count=space_info.achievementCount,
                 )
         character_ids = set()
         characters: List[CharacterInfo] = []
-        if api_data.PlayerDetailInfo.AssistAvatar:
+        if api_data.detailInfo.assistAvatarDetail:
             character_info = self.character_parse(
-                api_data.PlayerDetailInfo.AssistAvatar, language
+                api_data.detailInfo.assistAvatarDetail, language
             )
             if character_info:
                 character_info.name = character_info.name.replace(
                     "{NICKNAME}", player_info.nickname
                 )
                 character_ids.add(character_info.id)
                 characters.append(character_info)
-        if api_data.PlayerDetailInfo.DisplayAvatarList:
-            for character in api_data.PlayerDetailInfo.DisplayAvatarList:
-                if str(character.AvatarID) in character_ids:
+        if api_data.detailInfo.avatarDetailList:
+            for character in api_data.detailInfo.avatarDetailList:
+                if str(character.avatarId) in character_ids:
                     continue
                 character_info = self.character_parse(character, language)
                 if character_info:
                     character_info.name = character_info.name.replace(
                         "{NICKNAME}", player_info.nickname
                     )
                     characters.append(character_info)
```

### Comparing `mihomo-1.0.0/mihomo/model.py` & `mihomo-1.1.0/mihomo/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,81 +32,80 @@
                 result[field] = [i.to_dict() for i in value]
             else:
                 result[field] = value
         return result
 
 
 class SpaceChallengeData(BaseData):
-    MazeGroupID: int = 0
-    MazeGroupIndex: int = 0
-    PreMazeGroupIndex: int = 0
+    scheduleMaxLevel: int = 0
+    scheduleGroupId: int = 0
+    noneScheduleMaxLevel: int = 0
 
 
 class SpaceData(BaseData):
-    ChallengeData: Optional[SpaceChallengeData] = None
-    PassAreaProgress: int = 0
-    LightConeCount: int = 0
-    AvatarCount: int = 0
-    AchievementCount: int = 0
+    challengeInfo: Optional[SpaceChallengeData] = None
+    maxRogueChallengeScore: int = 0
+    equipmentCount: int = 0
+    avatarCount: int = 0
+    achievementCount: int = 0
 
 
 class EquipmentData(BaseData):
-    ID: int
-    Rank: int = 1
-    Level: int = 1
-    Promotion: int = 0
+    tid: int
+    rank: int = 1
+    level: int = 1
+    promotion: int = 0
 
 
-class BehaviorData(BaseData):
-    BehaviorID: int
-    Level: int = 0
+class SkillTreeData(BaseData):
+    pointId: int
+    level: int = 0
 
 
 class SubAffixData(BaseData):
-    SubAffixID: int
-    Cnt: int = 0
-    Step: int = 0
+    affixId: int
+    cnt: int = 0
+    step: int = 0
 
 
 class RelicData(BaseData):
-    ID: int
-    MainAffixID: int
-    Type: int
-    Level: int = 0
-    EXP: int = 0
-    RelicSubAffix: List[SubAffixData] = []
+    tid: int
+    mainAffixId: int
+    type: int
+    level: int = 0
+    exp: int = 0
+    subAffixList: List[SubAffixData] = []
 
 
 class CharacterData(BaseData):
-    AvatarID: int
-    Rank: int = 0
-    Level: int = 1
-    Promotion: int = 0
-    EquipmentID: Optional[EquipmentData] = None
-    BehaviorList: List[BehaviorData] = []
-    RelicList: List[RelicData] = []
+    avatarId: int
+    rank: int = 0
+    level: int = 1
+    promotion: int = 0
+    equipment: Optional[EquipmentData] = None
+    skillTreeList: List[SkillTreeData] = []
+    relicList: List[RelicData] = []
 
 
 class PlayerData(BaseData):
-    UID: int
-    NickName: str
-    Level: int = 0
-    WorldLevel: int = 0
-    CurFriendCount: int = 0
-    HeadIconID: int = 200001
-    Signature: str = ""
-    Birthday: int = 0
-    IsDisplayAvatarList: bool = False
-    PlayerSpaceInfo: Optional[SpaceData] = None
-    AssistAvatar: Optional[CharacterData] = None
-    DisplayAvatarList: List[CharacterData] = []
+    uid: int
+    nickname: str
+    level: int = 0
+    worldLevel: int = 0
+    friendCount: int = 0
+    headIcon: int = 200001
+    signature: str = ""
+    isDisplayAvatar: bool = False
+    recordInfo: Optional[SpaceData] = None
+    assistAvatarDetail: Optional[CharacterData] = None
+    avatarDetailList: List[CharacterData] = []
 
 
 class MihomoApiData(BaseData):
-    PlayerDetailInfo: Optional[PlayerData] = None
+    detailInfo: Optional[PlayerData] = None
 
 
 class SpaceChallengeInfo(BaseData):
     maze_group_id: int = 0
     maze_group_index: int = 0
     pre_maze_group_index: int = 0
 
@@ -123,15 +122,14 @@
     uid: str
     nickname: str
     level: int = 0
     world_level: int = 0
     friend_count: int = 0
     avatar: Optional[AvatarInfo] = None
     signature: str = ""
-    birthday: int = 0
     is_display: bool = False
     space_info: Optional[SpaceInfo] = None
 
 
 class FormattedApiInfo(BaseData):
     player: PlayerInfo
     characters: List[CharacterInfo] = []
```

### Comparing `mihomo-1.0.0/README.md` & `mihomo-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 from mihomo import MihomoApi
 from mihomo.model import Language
 
 
 async def main():
     api = MihomoApi()
 
+    # # Set index file path, default is "data/index"
+    # # Index files will be downloaded to this path
+    # api.set_index_path("data/index")
+
     # # Set i18n if needed, default is False
     # api.set_i18n(True)
 
     # # Set proxy if needed
     # api.set_proxy("http://127.0.0.1:7890")
 
     # Set language, default is Language.EN
```

### Comparing `mihomo-1.0.0/PKG-INFO` & `mihomo-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mihomo
-Version: 1.0.0
-Summary: 
+Version: 1.1.0
+Summary: Library for API wrapper data from mihomo
 Home-page: https://github.com/Mar-7th/mihomo.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,18 @@
 from mihomo import MihomoApi
 from mihomo.model import Language
 
 
 async def main():
     api = MihomoApi()
 
+    # # Set index file path, default is "data/index"
+    # # Index files will be downloaded to this path
+    # api.set_index_path("data/index")
+
     # # Set i18n if needed, default is False
     # api.set_i18n(True)
 
     # # Set proxy if needed
     # api.set_proxy("http://127.0.0.1:7890")
 
     # Set language, default is Language.EN
```

