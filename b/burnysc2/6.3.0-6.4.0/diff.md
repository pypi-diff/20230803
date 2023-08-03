# Comparing `tmp/burnysc2-6.3.0.tar.gz` & `tmp/burnysc2-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burnysc2-6.3.0.tar", max compression
+gzip compressed data, was "burnysc2-6.4.0.tar", max compression
```

## Comparing `burnysc2-6.3.0.tar` & `burnysc2-6.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1072 2023-07-14 21:38:46.401621 burnysc2-6.3.0/LICENSE
--rw-r--r--   0        0        0     3487 2023-07-14 21:38:46.405621 burnysc2-6.3.0/pyproject.toml
--rw-r--r--   0        0        0      305 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/__init__.py
--rw-r--r--   0        0        0     4139 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/action.py
--rw-r--r--   0        0        0    61153 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/bot_ai.py
--rw-r--r--   0        0        0    43060 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/bot_ai_internal.py
--rw-r--r--   0        0        0     1807 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/cache.py
--rw-r--r--   0        0        0    36292 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/client.py
--rw-r--r--   0        0        0    25400 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/constants.py
--rw-r--r--   0        0        0     3088 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/controller.py
--rw-r--r--   0        0        0     3392 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/data.py
--rw-r--r--   0        0        0      306 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/__init__.py
--rw-r--r--   0        0        0    16982 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/generic_redirect_abilities.py
--rw-r--r--   0        0        0    39206 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_abilities.py
--rw-r--r--   0        0        0    18259 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_research_abilities.py
--rw-r--r--   0        0        0     2088 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_tech_alias.py
--rw-r--r--   0        0        0    21568 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_train_build_abilities.py
--rw-r--r--   0        0        0     5830 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_trained_from.py
--rw-r--r--   0        0        0     2521 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_unit_alias.py
--rw-r--r--   0        0        0     5668 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/upgrade_researched_from.py
--rw-r--r--   0        0        0     5640 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/expiring_dict.py
--rw-r--r--   0        0        0    12982 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/game_data.py
--rw-r--r--   0        0        0    14000 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/game_info.py
--rw-r--r--   0        0        0    12317 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/game_state.py
--rw-r--r--   0        0        0     8590 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/generate_ids.py
--rw-r--r--   0        0        0      191 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/__init__.py
--rw-r--r--   0        0        0    52948 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/ability_id.py
--rw-r--r--   0        0        0     9427 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/buff_id.py
--rw-r--r--   0        0        0      685 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/effect_id.py
--rw-r--r--   0        0        0       35 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/id_version.py
--rw-r--r--   0        0        0    63891 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/ids/unit_typeid.py
--rw-r--r--   0        0        0     9494 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/ids/upgrade_id.py
--rw-r--r--   0        0        0    29769 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/main.py
--rw-r--r--   0        0        0     1558 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/maps.py
--rw-r--r--   0        0        0     5773 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/observer_ai.py
--rw-r--r--   0        0        0     4699 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/paths.py
--rw-r--r--   0        0        0     4181 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/pixel_map.py
--rw-r--r--   0        0        0     7021 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/player.py
--rw-r--r--   0        0        0     2854 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/portconfig.py
--rw-r--r--   0        0        0    13130 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/position.py
--rw-r--r--   0        0        0      883 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/power_source.py
--rw-r--r--   0        0        0     3014 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/protocol.py
--rw-r--r--   0        0        0    10401 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/proxy.py
--rw-r--r--   0        0        0     5817 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/renderer.py
--rw-r--r--   0        0        0     9635 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/sc2process.py
--rw-r--r--   0        0        0    11941 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/score.py
--rw-r--r--   0        0        0    59173 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/unit.py
--rw-r--r--   0        0        0     1404 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/unit_command.py
--rw-r--r--   0        0        0    29208 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/units.py
--rw-r--r--   0        0        0    17314 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/versions.py
--rw-r--r--   0        0        0     4155 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/wsl.py
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 burnysc2-6.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-03 11:25:13.695377 burnysc2-6.4.0/LICENSE
+-rw-r--r--   0        0        0     3487 2023-08-03 11:25:13.703378 burnysc2-6.4.0/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/__init__.py
+-rw-r--r--   0        0        0     4139 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/action.py
+-rw-r--r--   0        0        0    61428 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/bot_ai.py
+-rw-r--r--   0        0        0    43410 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/bot_ai_internal.py
+-rw-r--r--   0        0        0     1807 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/cache.py
+-rw-r--r--   0        0        0    36292 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/client.py
+-rw-r--r--   0        0        0    26125 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/constants.py
+-rw-r--r--   0        0        0     3088 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/controller.py
+-rw-r--r--   0        0        0     3392 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/data.py
+-rw-r--r--   0        0        0      306 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/__init__.py
+-rw-r--r--   0        0        0    16982 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/generic_redirect_abilities.py
+-rw-r--r--   0        0        0    39206 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/unit_abilities.py
+-rw-r--r--   0        0        0    18259 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/unit_research_abilities.py
+-rw-r--r--   0        0        0     2088 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/unit_tech_alias.py
+-rw-r--r--   0        0        0    21568 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/unit_train_build_abilities.py
+-rw-r--r--   0        0        0     5830 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/unit_trained_from.py
+-rw-r--r--   0        0        0     2521 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/unit_unit_alias.py
+-rw-r--r--   0        0        0     5668 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/dicts/upgrade_researched_from.py
+-rw-r--r--   0        0        0     5640 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/expiring_dict.py
+-rw-r--r--   0        0        0    12982 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/game_data.py
+-rw-r--r--   0        0        0    14000 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/game_info.py
+-rw-r--r--   0        0        0    12317 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/game_state.py
+-rw-r--r--   0        0        0     8590 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/generate_ids.py
+-rw-r--r--   0        0        0      191 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/__init__.py
+-rw-r--r--   0        0        0    52948 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/ability_id.py
+-rw-r--r--   0        0        0     9427 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/buff_id.py
+-rw-r--r--   0        0        0      685 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/effect_id.py
+-rw-r--r--   0        0        0       35 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/id_version.py
+-rw-r--r--   0        0        0    63891 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/unit_typeid.py
+-rw-r--r--   0        0        0     9494 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/ids/upgrade_id.py
+-rw-r--r--   0        0        0    29769 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/main.py
+-rw-r--r--   0        0        0     1558 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/maps.py
+-rw-r--r--   0        0        0     5773 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/observer_ai.py
+-rw-r--r--   0        0        0     4699 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/paths.py
+-rw-r--r--   0        0        0     4181 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/pixel_map.py
+-rw-r--r--   0        0        0     7021 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/player.py
+-rw-r--r--   0        0        0     2854 2023-08-03 11:25:13.703378 burnysc2-6.4.0/sc2/portconfig.py
+-rw-r--r--   0        0        0    13130 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/position.py
+-rw-r--r--   0        0        0      883 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/power_source.py
+-rw-r--r--   0        0        0     3014 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/protocol.py
+-rw-r--r--   0        0        0    10401 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/proxy.py
+-rw-r--r--   0        0        0     5817 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/renderer.py
+-rw-r--r--   0        0        0     9635 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/sc2process.py
+-rw-r--r--   0        0        0    11941 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/score.py
+-rw-r--r--   0        0        0    59173 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/unit.py
+-rw-r--r--   0        0        0     1404 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/unit_command.py
+-rw-r--r--   0        0        0    29208 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/units.py
+-rw-r--r--   0        0        0    17314 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/versions.py
+-rw-r--r--   0        0        0     4155 2023-08-03 11:25:13.707378 burnysc2-6.4.0/sc2/wsl.py
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 burnysc2-6.4.0/PKG-INFO
```

### Comparing `burnysc2-6.3.0/LICENSE` & `burnysc2-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/pyproject.toml` & `burnysc2-6.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burnysc2"
-version = "6.3.0"
+version = "6.4.0"
 description = "A StarCraft II API Client for Python 3"
 authors = ["BurnySc2 <gamingburny@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Burnysc2/python-sc2"
 documentation = "https://burnysc2.github.io/python-sc2/docs/index.html"
 keywords = ["StarCraft", "StarCraft 2", "StarCraft II", "AI", "Bot"]
 classifiers=[
```

### Comparing `burnysc2-6.3.0/sc2/action.py` & `burnysc2-6.4.0/sc2/action.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/bot_ai.py` & `burnysc2-6.4.0/sc2/bot_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import TYPE_CHECKING, Dict, List, Optional, Set, Tuple, Union
 
 from loguru import logger
 
 from sc2.bot_ai_internal import BotAIInternal
 from sc2.cache import property_cache_once_per_frame
 from sc2.constants import (
+    CREATION_ABILITY_FIX,
     EQUIVALENTS_FOR_TECH_PROGRESS,
     PROTOSS_TECH_REQUIREMENT,
     TERRAN_STRUCTURES_REQUIRE_SCV,
     TERRAN_TECH_REQUIREMENT,
     ZERG_TECH_REQUIREMENT,
 )
 from sc2.data import Alert, Race, Result, Target
@@ -787,15 +788,15 @@
             return max((s.build_progress for s in self.structures if s._proto.unit_type in equiv_values), default=0)
         creation_ability_data: AbilityData = self.game_data.units[structure_type_value].creation_ability
         if creation_ability_data is None:
             return 0
         creation_ability: AbilityId = creation_ability_data.exact_id
         max_value = max(
             [s.build_progress for s in self.structures if s._proto.unit_type in equiv_values] +
-            [self._abilities_all_units[1].get(creation_ability, 0)],
+            [self._abilities_count_and_build_progress[1].get(creation_ability, 0)],
             default=0,
         )
         return max_value
 
     def tech_requirement_progress(self, structure_type: UnitTypeId) -> float:
         """Returns the tech requirement progress for a specific building
 
@@ -849,20 +850,23 @@
         :param unit_type:
         """
         if isinstance(unit_type, UpgradeId):
             return self.already_pending_upgrade(unit_type)
         try:
             ability = self.game_data.units[unit_type.value].creation_ability.exact_id
         except AttributeError:
-            # Hotfix for checking pending archons
-            if unit_type == UnitTypeId.ARCHON:
-                return self._abilities_all_units[0][AbilityId.ARCHON_WARP_TARGET] / 2
+            if unit_type in CREATION_ABILITY_FIX:
+                # Hotfix for checking pending archons
+                if unit_type == UnitTypeId.ARCHON:
+                    return self._abilities_count_and_build_progress[0][AbilityId.ARCHON_WARP_TARGET] / 2
+                # Hotfix for rich geysirs
+                return self._abilities_count_and_build_progress[0][CREATION_ABILITY_FIX[unit_type]]
             logger.error(f"Uncaught UnitTypeId: {unit_type}")
             return 0
-        return self._abilities_all_units[0][ability]
+        return self._abilities_count_and_build_progress[0][ability]
 
     def worker_en_route_to_build(self, unit_type: UnitTypeId) -> float:
         """This function counts how many workers are on the way to start the construction a building.
 
         :param unit_type:"""
         ability = self.game_data.units[unit_type.value].creation_ability.exact_id
         return self._worker_orders[ability]
```

### Comparing `burnysc2-6.3.0/sc2/bot_ai_internal.py` & `burnysc2-6.4.0/sc2/bot_ai_internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import numpy as np
 from loguru import logger
 from s2clientprotocol import sc2api_pb2 as sc_pb
 
 from sc2.cache import property_cache_once_per_frame
 from sc2.constants import (
     ALL_GAS,
+    CREATION_ABILITY_FIX,
     IS_PLACEHOLDER,
     TERRAN_STRUCTURES_REQUIRE_SCV,
     FakeEffectID,
     abilityid_to_unittypeid,
     geyser_ids,
     mineral_ids,
 )
@@ -262,31 +263,36 @@
         correction = self.units(half_supply_units).amount % 2
         self.supply_used += correction
         self.supply_army += correction
         self.supply_left -= correction
 
     @final
     @property_cache_once_per_frame
-    def _abilities_all_units(self) -> Tuple[CounterType[AbilityId], Dict[AbilityId, float]]:
+    def _abilities_count_and_build_progress(self) -> Tuple[CounterType[AbilityId], Dict[AbilityId, float]]:
         """Cache for the already_pending function, includes protoss units warping in,
         all units in production and all structures, and all morphs"""
         abilities_amount: CounterType[AbilityId] = Counter()
         max_build_progress: Dict[AbilityId, float] = {}
         unit: Unit
         for unit in self.units + self.structures:
             for order in unit.orders:
                 abilities_amount[order.ability.exact_id] += 1
             if not unit.is_ready:
                 if self.race != Race.Terran or not unit.is_structure:
                     # If an SCV is constructing a building, already_pending would count this structure twice
                     # (once from the SCV order, and once from "not structure.is_ready")
-                    if unit.type_id == UnitTypeId.ARCHON:
-                        # Hotfix for archons in morph state
-                        creation_ability = AbilityId.ARCHON_WARP_TARGET
-                        abilities_amount[creation_ability] += 2
+                    if unit.type_id in CREATION_ABILITY_FIX:
+                        if unit.type_id == UnitTypeId.ARCHON:
+                            # Hotfix for archons in morph state
+                            creation_ability = AbilityId.ARCHON_WARP_TARGET
+                            abilities_amount[creation_ability] += 2
+                        else:
+                            # Hotfix for rich geysirs
+                            creation_ability = CREATION_ABILITY_FIX[unit.type_id]
+                            abilities_amount[creation_ability] += 1
                     else:
                         creation_ability: AbilityId = self.game_data.units[unit.type_id.value].creation_ability.exact_id
                         abilities_amount[creation_ability] += 1
                     max_build_progress[creation_ability] = max(
                         max_build_progress.get(creation_ability, 0), unit.build_progress
                     )
 
@@ -739,15 +745,15 @@
             if enemy_structure.tag not in self._enemy_structures_previous_map:
                 await self.on_enemy_unit_entered_vision(enemy_structure)
 
         # Call events for enemy unit left vision
         enemy_units_left_vision: Set[int] = set(self._enemy_units_previous_map) - self.enemy_units.tags
         for enemy_unit_tag in enemy_units_left_vision:
             await self.on_enemy_unit_left_vision(enemy_unit_tag)
-        enemy_structures_left_vision: Set[int] = (set(self._enemy_structures_previous_map) - self.enemy_structures.tags)
+        enemy_structures_left_vision: Set[int] = set(self._enemy_structures_previous_map) - self.enemy_structures.tags
         for enemy_structure_tag in enemy_structures_left_vision:
             await self.on_enemy_unit_left_vision(enemy_structure_tag)
 
     @final
     async def _issue_unit_dead_events(self):
         for unit_tag in self.state.dead_units & set(self._all_units_previous_map):
             await self.on_unit_destroyed(unit_tag)
```

### Comparing `burnysc2-6.3.0/sc2/cache.py` & `burnysc2-6.4.0/sc2/cache.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/client.py` & `burnysc2-6.4.0/sc2/client.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/constants.py` & `burnysc2-6.4.0/sc2/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,7 +677,20 @@
 TARGET_HELPER = {
     1: "no target",
     2: "Point2",
     3: "Unit",
     4: "Point2 or Unit",
     5: "Point2 or no target",
 }
+CREATION_ABILITY_FIX: Dict[UnitTypeId, AbilityId] = {
+    UnitTypeId.ARCHON: AbilityId.ARCHON_WARP_TARGET,
+    UnitTypeId.ASSIMILATORRICH: AbilityId.PROTOSSBUILD_ASSIMILATOR,
+    UnitTypeId.BANELINGCOCOON: AbilityId.MORPHZERGLINGTOBANELING_BANELING,
+    UnitTypeId.CHANGELING: AbilityId.SPAWNCHANGELING_SPAWNCHANGELING,
+    UnitTypeId.EXTRACTORRICH: AbilityId.ZERGBUILD_EXTRACTOR,
+    UnitTypeId.INTERCEPTOR: AbilityId.BUILD_INTERCEPTORS,
+    UnitTypeId.LURKERMPEGG: AbilityId.MORPH_LURKER,
+    UnitTypeId.MULE: AbilityId.CALLDOWNMULE_CALLDOWNMULE,
+    UnitTypeId.RAVAGERCOCOON: AbilityId.MORPHTORAVAGER_RAVAGER,
+    UnitTypeId.REFINERYRICH: AbilityId.TERRANBUILD_REFINERY,
+    UnitTypeId.TECHLAB: AbilityId.BUILD_TECHLAB,
+}
```

### Comparing `burnysc2-6.3.0/sc2/controller.py` & `burnysc2-6.4.0/sc2/controller.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/data.py` & `burnysc2-6.4.0/sc2/data.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/generic_redirect_abilities.py` & `burnysc2-6.4.0/sc2/dicts/generic_redirect_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/unit_abilities.py` & `burnysc2-6.4.0/sc2/dicts/unit_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/unit_research_abilities.py` & `burnysc2-6.4.0/sc2/dicts/unit_research_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/unit_tech_alias.py` & `burnysc2-6.4.0/sc2/dicts/unit_tech_alias.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/unit_train_build_abilities.py` & `burnysc2-6.4.0/sc2/dicts/unit_train_build_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/unit_trained_from.py` & `burnysc2-6.4.0/sc2/dicts/unit_trained_from.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/unit_unit_alias.py` & `burnysc2-6.4.0/sc2/dicts/unit_unit_alias.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/dicts/upgrade_researched_from.py` & `burnysc2-6.4.0/sc2/dicts/upgrade_researched_from.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/expiring_dict.py` & `burnysc2-6.4.0/sc2/expiring_dict.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/game_data.py` & `burnysc2-6.4.0/sc2/game_data.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/game_info.py` & `burnysc2-6.4.0/sc2/game_info.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/game_state.py` & `burnysc2-6.4.0/sc2/game_state.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/generate_ids.py` & `burnysc2-6.4.0/sc2/generate_ids.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/ids/ability_id.py` & `burnysc2-6.4.0/sc2/ids/ability_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/ids/buff_id.py` & `burnysc2-6.4.0/sc2/ids/buff_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/ids/effect_id.py` & `burnysc2-6.4.0/sc2/ids/effect_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/ids/unit_typeid.py` & `burnysc2-6.4.0/sc2/ids/unit_typeid.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/ids/upgrade_id.py` & `burnysc2-6.4.0/sc2/ids/upgrade_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/main.py` & `burnysc2-6.4.0/sc2/main.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/maps.py` & `burnysc2-6.4.0/sc2/maps.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/observer_ai.py` & `burnysc2-6.4.0/sc2/observer_ai.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/paths.py` & `burnysc2-6.4.0/sc2/paths.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/pixel_map.py` & `burnysc2-6.4.0/sc2/pixel_map.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/player.py` & `burnysc2-6.4.0/sc2/player.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/portconfig.py` & `burnysc2-6.4.0/sc2/portconfig.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/position.py` & `burnysc2-6.4.0/sc2/position.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/power_source.py` & `burnysc2-6.4.0/sc2/power_source.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/protocol.py` & `burnysc2-6.4.0/sc2/protocol.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/proxy.py` & `burnysc2-6.4.0/sc2/proxy.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/renderer.py` & `burnysc2-6.4.0/sc2/renderer.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/sc2process.py` & `burnysc2-6.4.0/sc2/sc2process.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/score.py` & `burnysc2-6.4.0/sc2/score.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/unit.py` & `burnysc2-6.4.0/sc2/unit.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/unit_command.py` & `burnysc2-6.4.0/sc2/unit_command.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/units.py` & `burnysc2-6.4.0/sc2/units.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/versions.py` & `burnysc2-6.4.0/sc2/versions.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/sc2/wsl.py` & `burnysc2-6.4.0/sc2/wsl.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.3.0/PKG-INFO` & `burnysc2-6.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burnysc2
-Version: 6.3.0
+Version: 6.4.0
 Summary: A StarCraft II API Client for Python 3
 Home-page: https://github.com/Burnysc2/python-sc2
 License: MIT
 Keywords: StarCraft,StarCraft 2,StarCraft II,AI,Bot
 Author: BurnySc2
 Author-email: gamingburny@gmail.com
 Requires-Python: >=3.8,<3.12
```

