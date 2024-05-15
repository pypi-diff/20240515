# Comparing `tmp/twitch_dota_extension-0.1.3.tar.gz` & `tmp/twitch_dota_extension-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dota_extension-0.1.3.tar", max compression
+gzip compressed data, was "twitch_dota_extension-0.1.4.tar", max compression
```

## Comparing `twitch_dota_extension-0.1.3.tar` & `twitch_dota_extension-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       58 2024-04-17 16:20:11.616674 twitch_dota_extension-0.1.3/README.md
--rw-r--r--   0        0        0      480 2024-05-09 17:44:37.606257 twitch_dota_extension-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6796 2024-05-09 17:00:39.841479 twitch_dota_extension-0.1.3/twitch_dota_extension/lib.py
--rw-r--r--   0        0        0     4546 2024-05-09 17:42:34.346097 twitch_dota_extension-0.1.3/twitch_dota_extension/tooltips.py
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 twitch_dota_extension-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-05-11 15:03:15.113903 twitch_dota_extension-0.1.4/README.md
+-rw-r--r--   0        0        0      526 2024-05-14 18:12:30.553090 twitch_dota_extension-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    10483 2024-05-14 16:54:45.519763 twitch_dota_extension-0.1.4/twitch_dota_extension/lib.py
+-rw-r--r--   0        0        0     2578 2024-05-14 15:17:07.083769 twitch_dota_extension-0.1.4/twitch_dota_extension/pgl.py
+-rw-r--r--   0        0        0     4808 2024-05-12 17:03:34.213397 twitch_dota_extension-0.1.4/twitch_dota_extension/tooltips.py
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 twitch_dota_extension-0.1.4/PKG-INFO
```

### Comparing `twitch_dota_extension-0.1.3/twitch_dota_extension/lib.py` & `twitch_dota_extension-0.1.4/twitch_dota_extension/lib.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import dataclasses
 import enum
 import json
 from dataclasses import dataclass
 from typing import Optional, Any
 
 import dacite
 import httpx
+from twitch_dota_extension.pgl import PGLGameState
 
 from twitch_dota_extension.tooltips import Hero, Ability, Item
 
 
 @dataclass
 class HDAbility:
     name: str
@@ -21,80 +23,96 @@
 
 @dataclass
 class Inventory:
     items: list[Item]
     neutral_slot: Optional[Item]
 
     @staticmethod
-    def from_parts(items: dict[str, HDItem], itemdef: dict[str, Item]) -> 'Inventory':
+    def from_parts(items: dict[str, HDItem], itemdef: dict[str, Item]) -> "Inventory":
         items_ = []
         for slot in ["slot0", "slot1", "slot2", "slot3", "slot4", "slot5"]:
-            if items[slot].name != 'empty':
+            if items[slot].name != "empty":
                 items_.append(itemdef[items[slot].name])
-        neutral = itemdef[items["neutral0"].name] if items["neutral0"].name != 'empty' else None
+        neutral = itemdef[items["neutral0"].name] if items["neutral0"].name != "empty" else None
         return Inventory(items_, neutral)
 
+
 @dataclass
 class HeroData:
     t: list[int]
     items: dict[str, HDItem]
-    # base_ability_count: int
+    # This is not provided by the API
+    lvl: int = 1
+    aghs: list[int] = dataclasses.field(default_factory=lambda: [0,0])
+
 
 @dataclass
 class TournamentHeroData(HeroData):
-    p: str
-    lvl: int
-    aghs: list[int]
+    p: str = "unknown"
+    #aghs: list[int]
+
 
 @dataclass
 class TalentEntry:
     name: str
     picked: bool
 
+
 @dataclass
 class TalentTree:
     entries: list[tuple[TalentEntry, TalentEntry]]
 
     @staticmethod
-    def from_parts(talents: list[str], picks: list[int]) -> 'TalentTree':
+    def from_parts(talents: list[str], picks: list[int]) -> "TalentTree":
         entries: list[TalentEntry] = []
         for talent, picked in zip(talents, picks):
             entries.append(TalentEntry(name=talent, picked=bool(picked)))
-        # TODO: these are backwards in the API!!
-        # it returns 0, 1, 2, 3, .. where 0, 2, 4, 6 are RIGHT and 1,3,5,7 are LEFT
         list_of_groups = list(zip(*(iter(entries),) * 2))
+        # these are backwards in the API!!
+        # it returns 0, 1, 2, 3, .. where 0, 2, 4, 6 are RIGHT and 1,3,5,7 are LEFT
+        list_of_groups = [(second, first) for first, second in list_of_groups]
         return TalentTree(entries=list_of_groups)
 
+
 @dataclass
 class ProcessedHeroData:
     n: str
     name: str
     talent_tree: TalentTree
     abilities: list[Ability]
     inventory: Inventory
+    # not provided by the API
+    has_scepter: bool
+    has_shard: bool
+    level: int
+    player: str
+
 
 @dataclass
 class TourProcessedHeroData(ProcessedHeroData):
-    player: Optional[str] = None
-    level: Optional[int] = None
-    has_aghs: Optional[bool] = False
-    has_shard: Optional[bool] = False
+    pass
 
 
 @dataclass
 class Playing:
     selected_hero: str
     selected_hero_data: HeroData
 
-    def process_data(self, heroes: dict[str, Hero], items) -> ProcessedHeroData:
+    def process_data(self, streamer: str, heroes: dict[str, Hero], items) -> ProcessedHeroData:
         hero = heroes[self.selected_hero]
         talents = TalentTree.from_parts(hero.talents, self.selected_hero_data.t)
         inv = Inventory.from_parts(self.selected_hero_data.items, items)
 
-        phd = ProcessedHeroData(hero.n, hero.name, talents, hero.abilities, inv)
+        phd = ProcessedHeroData(hero.n, hero.name, talents, hero.abilities, inv,
+                # not provided by the API
+                player=streamer,
+                level=1,
+                has_scepter=False,
+                has_shard=False,
+                )
         return phd
 
 
 @dataclass
 class CDNConfig:
     domain: str
 
@@ -103,43 +121,114 @@
         return CDNConfig("dotatooltips.b-cdn.net")
 
 
 @dataclass
 class APIConfig:
     domain: str
     tour_domain: str
+    pgl_domain: str
 
     @staticmethod
     def default() -> "APIConfig":
-        return APIConfig("tooltips.layerth.dev", "tour-tooltips.layerth.dev")
+        return APIConfig("tooltips.layerth.dev", "tour-tooltips.layerth.dev", "dota2-twitch.pglesports.com")
 
 
 @dataclass
 class Spectating:
     heroes: list[str]
     hero_data: dict[str, HeroData]
 
+    def process_data(self, heroes: dict[str, Hero], items) -> list[TourProcessedHeroData]:
+        ret = []
+        for hero_name, hero_state in self.hero_data.items():
+            hero = heroes[hero_name]
+            talents = TalentTree.from_parts(hero.talents, hero_state.t)
+            inv = Inventory.from_parts(hero_state.items, items)
+
+            phd = TourProcessedHeroData(
+                hero.n,
+                hero.name,
+                talents,
+                hero.abilities,
+                inv,
+                player="unknown",
+                level=hero_state.lvl,
+                has_scepter=bool(hero_state.aghs[0]),
+                has_shard=bool(hero_state.aghs[1]),
+            )
+            ret.append(phd)
+        return ret
+
 
 @dataclass
 class SpectatingTournament:
     hero_data: dict[str, TournamentHeroData]
 
     def process_data(self, heroes: dict[str, Hero], items) -> list[TourProcessedHeroData]:
         ret = []
         for hero_name, hero_state in self.hero_data.items():
             hero = heroes[hero_name]
             talents = TalentTree.from_parts(hero.talents, hero_state.t)
             inv = Inventory.from_parts(hero_state.items, items)
 
-            phd = TourProcessedHeroData(hero.n, hero.name, talents, hero.abilities, inv,
-                                    player=hero_state.p, level=hero_state.lvl,
-                                    has_aghs=bool(hero_state.aghs[0]), has_shard=bool(hero_state.aghs[1]))
+            phd = TourProcessedHeroData(
+                hero.n,
+                hero.name,
+                talents,
+                hero.abilities,
+                inv,
+                player=hero_state.p,
+                level=hero_state.lvl,
+                has_scepter=bool(hero_state.aghs[0]),
+                has_shard=bool(hero_state.aghs[1]),
+            )
             ret.append(phd)
         return ret
 
+
+@dataclass
+class SpectatingPglTournament:
+    data: PGLGameState
+
+    def process_data(
+        self, heroes: dict[str, Hero], hero_map: dict[str, str], items: dict[str, Any]
+    ) -> list[TourProcessedHeroData]:
+        ret = []
+        for hero_meta in self.data.HeroList:
+            hero_name = hero_map[hero_meta["name"]]
+            idx = hero_meta["index"]
+
+            _herod = self.data.Heroes[idx]
+            _pstatsd = self.data.PlayerStats[idx]
+            _invd = self.data.Inventory[idx]
+
+            t = [int(_herod[f"talent_{i}"]) for i in range(1, 9)]
+
+            hero = heroes[hero_name]
+            talents = TalentTree.from_parts(hero.talents, t)
+            inv = Inventory(
+                [items[name] for name in _invd["main"] if name != "empty"],
+                items[_invd["neutral"]] if _invd["neutral"] != "empty" else None,
+            )
+
+            phd = TourProcessedHeroData(
+                hero.n,
+                hero.name,
+                talents,
+                hero.abilities,
+                inv,
+                player=_pstatsd["name"],
+                level=_herod["level"],
+                has_scepter=_herod["aghanims_scepter"],
+                has_shard=_herod["aghanims_shard"],
+            )
+            ret.append(phd)
+        return ret
+
+
 @dataclass
 class InvalidResponse:
     r: dict[str, Any]
 
 
 @dataclass
 class APIError:
@@ -152,32 +241,46 @@
 
 
 class API:
     def __init__(self, cdn_config: Optional[CDNConfig] = None, api_config: Optional[APIConfig] = None):
         self.cdn_config = cdn_config or CDNConfig.default()
         self.api_config = api_config or APIConfig.default()
 
+    def _map_pgl_hero_names(self, raw_heroes: dict) -> dict[str, str]:
+        return {k: v["data_name"] for k, v in raw_heroes.items()}
+
+    async def fetch_pgl_hero_mappings(self) -> dict[str, str]:
+        url = "https://dota2-data.pglesports.com/static/heroes.json"
+        data = await self._fetch_json(url)
+        return self._map_pgl_hero_names(data)
+
     async def _fetch_json(self, url) -> dict:
         async with httpx.AsyncClient() as client:
             r = await client.get(url)
             r.raise_for_status()
         return json.loads(r.text)
 
     async def fetch_items(self, language: str = "english") -> dict[str, Item]:
         items = await self._fetch_data_file(DataType.Items, language)
+        return self._process_items(items)
+
+    def _process_items(self, items: dict[str, Any]) -> dict[str, Item]:
         ret = {}
         for k, v in items.items():
-            if 'name' not in v:
+            if "name" not in v:
                 continue
             i = Item.from_dict(v)
             ret[k] = i
         return ret
 
     async def fetch_heroes(self, language: str = "english") -> dict[str, Hero]:
         heroes = await self._fetch_data_file(DataType.Heroes, language)
+        return self._process_heroes(heroes)
+
+    def _process_heroes(self, heroes: dict[str, Any]) -> dict[str, Hero]:
         ret = {}
         for k, v in heroes.items():
             if k == "npc_dota_hero_target_dummy":
                 continue
             h = Hero.from_dict(v)
             ret[k] = h
         return ret
@@ -189,36 +292,49 @@
             case DataType.Heroes:
                 type_ = "full-heroes"
             case default:
                 raise ValueError(f"Unsupported value {default}")
         url = f"https://{self.cdn_config.domain}/data/{language}/{type_}.json"
         return await self._fetch_json(url)
 
-    async def get_stream_status(self, channel_id: int) -> Playing | APIError | Spectating | SpectatingTournament | InvalidResponse:
-        MAYBE_IN_TOURNAMENT = "Channel not found. It might take a few minutes for the channel to appear."
+    async def get_stream_status(
+        self, channel_id: int
+    ) -> Playing | APIError | Spectating | SpectatingTournament | SpectatingPglTournament | InvalidResponse:
+        # TODO: parallel? though unlikely to be the 2nd/3rd
+        # maybe return meta so client can cache type?
+        NOT_AVAIL = "Channel not found. It might take a few minutes for the channel to appear."
         url = f"https://{self.api_config.domain}/data/pubsub/{channel_id}"
         data = await self._fetch_json(url)
 
-        if data.get('error') == MAYBE_IN_TOURNAMENT:
+        if data.get("error") == NOT_AVAIL:
             print("Attempting to fetch from tournament domain")
             url_tour = f"https://{self.api_config.tour_domain}/data/pubsub/{channel_id}"
             data = await self._fetch_json(url_tour)
 
+        if data.get("error") == NOT_AVAIL:
+            print("Attempting to fetch from PGL domain")
+
+            pgs = await PGLGameState.from_stream(self.api_config.pgl_domain, channel_id)
+            if pgs is not None:
+                return SpectatingPglTournament(pgs)
+
         r = API._from_json(data)
         return r
 
     @staticmethod
     def _from_json(data: dict) -> Playing | APIError | Spectating | SpectatingTournament | InvalidResponse:
         error = data.get("error")
         if error:
             return APIError(error)
         game = data.get("active_game", {})
         state = game.get("gsi_state", "unpopulated in API")
 
         if state == "playing":
-            return dacite.from_dict(data_class=Playing, data=game)
-        elif state == "spectating" and game.get('matchid'):  # Tournament
+            ret = dacite.from_dict(data_class=Playing, data=game)
+            ret.selected_hero_data.aghs = [False, False]
+            return ret
+        elif state == "spectating" and game.get("matchid"):  # Tournament
             return dacite.from_dict(data_class=SpectatingTournament, data=game)
         elif state == "spectating":
             return dacite.from_dict(data_class=Spectating, data=game)
 
         return InvalidResponse(r=data)
```

### Comparing `twitch_dota_extension-0.1.3/twitch_dota_extension/tooltips.py` & `twitch_dota_extension-0.1.4/twitch_dota_extension/tooltips.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,14 @@
             continue
         cur_val += char
         cur += 1
 
     if cur_val:
         ret.append(Node(cur_tag or 'text', cur_val.strip()))
 
-    for i in ret:
-        print(i.tag)
     return ret
 
 @dataclass
 class Property:
     name: str
     value: list[str] | str
 
@@ -100,24 +98,28 @@
 @dataclass
 class Ability:
     name: str
     n: str
     tooltip: Tooltip
     has_scepter_upgrade: bool
     has_shard_upgrade: bool
+    granted_by_scepter: bool
+    granted_by_shard: bool
     properties: list[Property]
 
     @staticmethod
     def from_dict(d: dict) -> "Ability":
         return Ability(
             name=d["name"],
             n=d["n"],
             tooltip=Tooltip.from_dict(d["tooltips"]),
             has_scepter_upgrade=d.get("HasScepterUpgrade") == "1",
             has_shard_upgrade=d.get("HasShardUpgrade") == "1",
+            granted_by_scepter=d.get("IsGrantedByScepter") == "1",
+            granted_by_shard=d.get("IsGrantedByShard") == "1",
             properties=[Property.from_dict(p) for p in d["properties"]],
         )
 
 
 @dataclass
 class Hero:
     n: str
@@ -145,25 +147,27 @@
 @dataclass
 class Item:
     n: str
     name: str
     cooldown: Optional[str]
     manacost: Optional[str]
     cost: Optional[str]
+    description: list[Node]
     active: list[Node]
     use: list[Node]
     passive: list[Node]
     properties: dict[str, str]
 
     @staticmethod
     def from_dict(d: dict) -> "Item":
         return Item(
             n=d["n"],
             name=d["name"],
             active=markup_to_nodes(d.get("active", "")),
             use=markup_to_nodes(d.get("use", "")),
             passive=markup_to_nodes(d.get("passive", "")),
+            description=markup_to_nodes(d.get("tooltips", {}).get("Description", "")),
             cooldown=d.get("AbilityCooldown"),
             manacost=d.get("AbilityManaCost"),
             cost=d.get("ItemCost"),
             properties={prop['name']: prop['value'] for prop in d.get('properties', [])},
         )
```

### Comparing `twitch_dota_extension-0.1.3/PKG-INFO` & `twitch_dota_extension-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: twitch-dota-extension
-Version: 0.1.3
+Version: 0.1.4
 Summary: Interact with the Dota2 Extension API for a given Twitch channel ID
 License: MIT
 Author: David Ventura
 Author-email: davidventura27@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-Simple client to interact with the Dota2 twitch extension
+Simple client to interact with the Dota2 twitch extension and the PGL dota2 extension
```

