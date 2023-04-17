# Comparing `tmp/pymodd-0.2.2.tar.gz` & `tmp/pymodd-0.3.0.tar.gz`

## Comparing `pymodd-0.2.2.tar` & `pymodd-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      285 1970-01-01 00:00:00.000000 pymodd-0.2.2/Cargo.toml
--rw-r--r--   0      501       20     1513 2023-02-26 06:10:27.000000 pymodd-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0      501       20     3103 2023-02-26 06:10:27.000000 pymodd-0.2.2/.gitignore
--rw-r--r--   0      501       20     1043 2022-11-03 01:15:30.000000 pymodd-0.2.2/LICENSE.txt
--rw-r--r--   0      501       20     2243 2023-04-04 02:20:56.000000 pymodd-0.2.2/README.rst
--rw-r--r--   0      501       20     1009 2023-04-03 02:53:13.000000 pymodd-0.2.2/examples/froge/entity_scripts.py
--rw-r--r--   0      501       20     1880 2023-03-29 23:39:09.000000 pymodd-0.2.2/examples/froge/game_variables.py
--rw-r--r--   0      501       20      602 2023-03-29 23:39:09.000000 pymodd-0.2.2/examples/froge/mapping.py
--rw-r--r--   0      501       20     6414 2023-04-03 02:53:13.000000 pymodd-0.2.2/examples/froge/scripts.py
--rw-r--r--   0      501       20    78188 2023-03-29 23:39:09.000000 pymodd-0.2.2/examples/froge/utils/game.json
--rw-r--r--   0      501       20        0 2023-03-16 03:19:40.000000 pymodd-0.2.2/pymodd/__init__.py
--rw-r--r--   0      501       20      205 2023-04-03 02:53:13.000000 pymodd-0.2.2/pymodd/_pymodd_generator.pyi
--rw-r--r--   0      501       20    43414 2023-04-04 02:08:06.000000 pymodd-0.2.2/pymodd/actions.py
--rw-r--r--   0      501       20      432 2023-04-04 02:04:39.000000 pymodd-0.2.2/pymodd/console_scripts/generate_project.py
--rw-r--r--   0      501       20    52956 2023-04-03 02:53:13.000000 pymodd-0.2.2/pymodd/functions.py
--rw-r--r--   0      501       20       26 2023-04-03 02:53:13.000000 pymodd-0.2.2/pymodd/py.typed
--rw-r--r--   0      501       20     9191 2023-03-23 22:29:44.000000 pymodd-0.2.2/pymodd/script.py
--rw-r--r--   0      501       20      808 2023-04-04 02:08:11.000000 pymodd-0.2.2/pyproject.toml
--rw-r--r--   0      501       20       41 2023-04-03 02:53:13.000000 pymodd-0.2.2/requirements.txt
--rw-r--r--   0      501       20     7765 2023-03-16 02:36:02.000000 pymodd-0.2.2/src/game_data/actions.rs
--rw-r--r--   0      501       20    20085 2023-04-03 02:53:13.000000 pymodd-0.2.2/src/game_data/argument.rs
--rw-r--r--   0      501       20     9297 2023-03-05 23:46:56.000000 pymodd-0.2.2/src/game_data/directory.rs
--rw-r--r--   0      501       20     2135 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/game_data/entity_types.rs
--rw-r--r--   0      501       20    10395 2023-03-05 23:46:56.000000 pymodd-0.2.2/src/game_data/variable_categories.rs
--rw-r--r--   0      501       20     1576 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/game_data.rs
--rw-r--r--   0      501       20     1389 2023-04-03 02:53:13.000000 pymodd-0.2.2/src/lib.rs
--rw-r--r--   0      501       20     4770 2023-04-04 02:04:39.000000 pymodd-0.2.2/src/project_generator/entity_scripts_file.rs
--rw-r--r--   0      501       20      183 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/project_generator/game_json_file.rs
--rw-r--r--   0      501       20     3459 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/project_generator/game_variables_file.rs
--rw-r--r--   0      501       20     6318 2023-04-04 02:04:39.000000 pymodd-0.2.2/src/project_generator/mapping_file.rs
--rw-r--r--   0      501       20    21011 2023-04-04 02:04:39.000000 pymodd-0.2.2/src/project_generator/scripts_file.rs
--rw-r--r--   0      501       20     9495 2023-03-18 23:37:16.000000 pymodd-0.2.2/src/project_generator/utils/iterators/argument_values_iterator.rs
--rw-r--r--   0      501       20     1820 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/project_generator/utils/iterators/directory_iterator.rs
--rw-r--r--   0      501       20       62 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/project_generator/utils/iterators.rs
--rw-r--r--   0      501       20     9420 2023-03-22 23:44:33.000000 pymodd-0.2.2/src/project_generator/utils/to_pymodd_maps.rs
--rw-r--r--   0      501       20     2267 2023-03-22 23:44:33.000000 pymodd-0.2.2/src/project_generator/utils.rs
--rw-r--r--   0      501       20     2373 2023-02-26 06:10:27.000000 pymodd-0.2.2/src/project_generator.rs
--rw-r--r--   0      501       20    11966 2023-04-03 01:26:12.000000 pymodd-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pymodd-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-0.3.0/Cargo.toml
+-rw-r--r--   0      501       20     1513 2023-04-16 22:43:12.000000 pymodd-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20     3103 2023-04-16 22:43:12.000000 pymodd-0.3.0/.gitignore
+-rw-r--r--   0      501       20     1043 2023-04-16 22:43:12.000000 pymodd-0.3.0/LICENSE.txt
+-rw-r--r--   0      501       20     2283 2023-04-16 22:43:12.000000 pymodd-0.3.0/README.rst
+-rw-r--r--   0      501       20      910 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/entity_scripts.py
+-rw-r--r--   0      501       20     1880 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/game_variables.py
+-rw-r--r--   0      501       20      466 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/mapping.py
+-rw-r--r--   0      501       20     6219 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/scripts.py
+-rw-r--r--   0      501       20    78188 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/utils/game.json
+-rw-r--r--   0      501       20        0 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/__init__.py
+-rw-r--r--   0      501       20     1040 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/_pymodd_helper.pyi
+-rw-r--r--   0      501       20    43418 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/actions.py
+-rw-r--r--   0      501       20     2772 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/console_scripts/pymodd_command.py
+-rw-r--r--   0      501       20    52968 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/functions.py
+-rw-r--r--   0      501       20       26 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/py.typed
+-rw-r--r--   0      501       20     8692 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/script.py
+-rw-r--r--   0      501       20      801 2023-04-17 01:03:34.000000 pymodd-0.3.0/pyproject.toml
+-rw-r--r--   0      501       20       41 2023-04-16 22:43:12.000000 pymodd-0.3.0/requirements.txt
+-rw-r--r--   0      501       20     7772 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/actions.rs
+-rw-r--r--   0      501       20    20091 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/argument.rs
+-rw-r--r--   0      501       20     9678 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/directory.rs
+-rw-r--r--   0      501       20     2135 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/entity_types.rs
+-rw-r--r--   0      501       20    10395 2023-04-17 01:01:26.000000 pymodd-0.3.0/src/game_data/variable_categories.rs
+-rw-r--r--   0      501       20     1800 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data.rs
+-rw-r--r--   0      501       20     2187 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/lib.rs
+-rw-r--r--   0      501       20     4820 2023-04-17 01:01:26.000000 pymodd-0.3.0/src/project_generator/entity_scripts_file.rs
+-rw-r--r--   0      501       20      183 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/game_json_file.rs
+-rw-r--r--   0      501       20     3459 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/game_variables_file.rs
+-rw-r--r--   0      501       20     6002 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/mapping_file.rs
+-rw-r--r--   0      501       20    24371 2023-04-16 22:43:22.000000 pymodd-0.3.0/src/project_generator/scripts_file.rs
+-rw-r--r--   0      501       20     9767 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/iterators/argument_values_iterator.rs
+-rw-r--r--   0      501       20     1820 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/iterators/directory_iterator.rs
+-rw-r--r--   0      501       20       62 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/iterators.rs
+-rw-r--r--   0      501       20     9420 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/to_pymodd_maps.rs
+-rw-r--r--   0      501       20     2267 2023-04-17 01:01:26.000000 pymodd-0.3.0/src/project_generator/utils.rs
+-rw-r--r--   0      501       20     2400 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator.rs
+-rw-r--r--   0      501       20    12887 2023-04-16 22:43:12.000000 pymodd-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 pymodd-0.3.0/PKG-INFO
```

### Comparing `pymodd-0.2.2/.github/workflows/CI.yml` & `pymodd-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/.gitignore` & `pymodd-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/LICENSE.txt` & `pymodd-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/README.rst` & `pymodd-0.3.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
    :alt: PyPI - License
 
 Features
 --------
 
 - edit global and entity scripts
 - organize folders and scripts with a mapping file
-- a command to generate a pymodd project
+- a command to generate and compile a pymodd project
 
 Installing
 ----------
 
 **Python 3.8 or higher is required**
 
 To install the library run the following command:
@@ -39,36 +39,36 @@
 Getting Started
 ---------------
 
 Export your modd game json file from the website and then generate a pymodd project by running the following command:
 
 .. code:: sh
 
-    generate-game [GAME_JSON_FILE_PATH]
+    pymodd generate-project [GAME_JSON_FILE_PATH]
 
 
 Quick Script Example
 --------------------
 
-view examples/sample_scripts.py in the github repo for the full example
+view the ``examples/froge directory`` for a generated pymodd project
 
 .. code:: py
 
-    class EverySecond(Script):
+    @script(triggers=[Trigger.EVERY_SECOND])
+    class EverySecond():
         def _build(self):
-            self.key = 'P8MwXcSxq7'
-            self.triggers = [Trigger.EVERY_SECOND]
             self.actions = [
                 if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG) < 5), [
                     create_unit_for_player_at_position_with_rotation(UnitTypes.FROG, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
                 ], [
                     if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG_BOSS) == 0), [
                         if_else((Variables.BOSS_TIMER <= 0), [
                             create_unit_for_player_at_position_with_rotation(UnitTypes.FROG_BOSS, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
                             update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000),
+                            set_variable(Variables.BOSS_TIMER, 200),
                         ], [
                         ]),
                         decrease_variable_by_number(Variables.BOSS_TIMER, 1),
                     ], [
                     ]),
                 ]),
             ]
```

### Comparing `pymodd-0.2.2/examples/froge/game_variables.py` & `pymodd-0.3.0/examples/froge/game_variables.py`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/examples/froge/scripts.py` & `pymodd-0.3.0/examples/froge/scripts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from pymodd.actions import *
 from pymodd.functions import *
-from pymodd.script import Script, Trigger, UiTarget, Flip
+from pymodd.script import Trigger, UiTarget, Flip, script
 
 from game_variables import *
 
 
-class Initialize(Script):
+@script(triggers=[Trigger.GAME_START])
+class Initialize():
 	def _build(self):
-		self.key = 'initialize'
-		self.triggers = [Trigger.GAME_START]
 		self.actions = [
 			assign_player_to_player_type(Variables.AI, PlayerTypes.AI),
 			
 		]
 
 
-class PlayerJoins(Script):
+@script(triggers=[Trigger.PLAYER_JOINS_GAME])
+class PlayerJoins():
 	def _build(self):
-		self.key = 'playerJoinsGame'
-		self.triggers = [Trigger.PLAYER_JOINS_GAME]
 		self.actions = [
 			create_unit_for_player_at_position_with_rotation(UnitTypes.POOPER, LastTriggeringPlayer(), RandomPositionInRegion(EntireMapRegion()), 0),
 			make_camera_of_player_track_unit(LastTriggeringPlayer(), LastCreatedUnit()),
 			assign_player_to_player_type(LastTriggeringPlayer(), PlayerTypes.PLAYER),
 			
 		]
 
 
-class PlayerLeaves(Script):
+@script(triggers=[Trigger.PLAYER_LEAVES_GAME])
+class PlayerLeaves():
 	def _build(self):
-		self.key = 'playerLeavesGame'
-		self.triggers = [Trigger.PLAYER_LEAVES_GAME]
 		self.actions = [
 			for_all_units_in(AllUnitsOwnedByPlayer(LastTriggeringPlayer()), [
 				destroy_entity(SelectedUnit()),
 				
 			], comment='when a player leaves, destroy all units owned by that player'),
 			
 		]
 
 
-class EverySecond(Script):
+@script(triggers=[Trigger.EVERY_SECOND])
+class EverySecond():
 	def _build(self):
-		self.key = 'P8MwXcSxq7'
-		self.triggers = [Trigger.EVERY_SECOND]
 		self.actions = [
 			if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG) < 5), [
 				create_unit_for_player_at_position_with_rotation(UnitTypes.FROG, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
 				
 			], [
 				if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG_BOSS) == 0), [
 					if_else((Variables.BOSS_TIMER <= 0), [
 						create_unit_for_player_at_position_with_rotation(UnitTypes.FROG_BOSS, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
 						update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000),
+						set_variable(Variables.BOSS_TIMER, 200),
 						
 					], [
 						
 					]),
 					decrease_variable_by_number(Variables.BOSS_TIMER, 1),
 					
 				], [
@@ -64,40 +61,38 @@
 				]),
 				
 			]),
 			
 		]
 
 
-class WhenAUnitsAttributeBecomes0OrLess(Script):
+@script(triggers=[Trigger.UNIT_ATTRIBUTE_BECOMES_ZERO])
+class WhenAUnitsAttributeBecomes0OrLess():
 	def _build(self):
-		self.key = 'CE0PBg1VWG'
-		self.triggers = [Trigger.UNIT_ATTRIBUTE_BECOMES_ZERO]
 		self.actions = [
-			if_else((AttributeTypeOfAttribute(TriggeringAttribute()) == AttributeTypes.HEALTH), [
+			if_else((AttributeTypeOfAttribute(LastTriggeringAttribute()) == AttributeTypes.HEALTH), [
 				if_else((PlayerTypeOfPlayer(OwnerOfEntity(LastTriggeringUnit())) == PlayerTypes.PLAYER), [
 					set_entity_attribute(AttributeTypes.HEALTH, LastTriggeringUnit(), AttributeMaxOfEntity(AttributeTypes.HEALTH, LastTriggeringUnit())),
 					set_entity_variable(EntityVariables.TARGET_UNIT, LastTriggeringUnit(), Undefined()),
 					move_entity_to_position(LastTriggeringUnit(), CenterOfRegion(EntireMapRegion())),
 					
 				], [
 					if_else((UnitTypeOfUnit(LastTriggeringUnit()) == UnitTypes.FROG_BOSS), [
-						set_variable(Variables.BOSS_TIMER, 200),
 						set_player_attribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit()), PlayerAttribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit())) + 7),
 						
 					], [
 						set_player_attribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit()), PlayerAttribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit())) + 1),
 						
 					]),
 					destroy_entity(LastTriggeringUnit()),
 					
 				]),
 				
 			], [
-				if_else((AttributeTypeOfAttribute(TriggeringAttribute()) == AttributeTypes.MOVE), [
+				if_else((AttributeTypeOfAttribute(LastTriggeringAttribute()) == AttributeTypes.MOVE), [
 					set_entity_variable(EntityVariables.TARGET_UNIT, LastTriggeringUnit(), Undefined()),
 					for_all_entities_in(AllEntitiesInRegion(DynamicRegion(XCoordinateOfPosition(PositionOfEntity(LastTriggeringUnit())) - (ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()) / 2), YCoordinateOfPosition(PositionOfEntity(LastTriggeringUnit())) - (ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()) / 2), ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()), ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()))), [
 						if_else((PlayerTypeOfPlayer(OwnerOfEntity(SelectedEntity())) == PlayerTypes.PLAYER), [
 							if_else(((ValueOfEntityVariable(EntityVariables.TARGET_UNIT, LastTriggeringUnit()) == Undefined()) | (DistanceBetweenPositions(PositionOfEntity(SelectedEntity()), PositionOfEntity(LastTriggeringUnit())) > DistanceBetweenPositions(PositionOfEntity(ValueOfEntityVariable(EntityVariables.TARGET_UNIT, LastTriggeringUnit())), PositionOfEntity(LastTriggeringUnit())))), [
 								create_floating_text_at_position_with_color('Froge sense', PositionOfEntity(LastTriggeringUnit()), '#327117', disabled=True),
 								set_entity_variable(EntityVariables.TARGET_UNIT, LastTriggeringUnit(), SelectedEntity()),
 								
@@ -140,15 +135,14 @@
 				]),
 				
 			]),
 			
 		]
 
 
-class OpenShop(Script):
+@script(triggers=[])
+class OpenShop():
 	def _build(self):
-		self.key = '5BUXtByxVf'
-		self.triggers = []
 		self.actions = [
 			open_shop_for_player(Shops.FROGE_SHOP, OwnerOfEntity(LastCastingUnit())),
 			
 		]
```

### Comparing `pymodd-0.2.2/examples/froge/utils/game.json` & `pymodd-0.3.0/examples/froge/utils/game.json`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/pymodd/actions.py` & `pymodd-0.3.0/pymodd/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import functools
 
 from .functions import Condition, Number, String
-from .script import Base, to_dict
+from .script import Script, to_dict
 
 
 def action(func):
     @functools.wraps(func)
     def wrapper_action(*args, **kwargs):
         action_dictionary = (func(*args))
         action_dictionary.update(
@@ -374,18 +374,18 @@
 def return_loop(comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'return',
     }
 
 
 @action
-def run_script(script_name, comment=None, disabled=False, run_on_client=False):
+def run_script(script: Script, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'runScript',
-        'scriptName': to_dict(script_name),
+        'scriptName': to_dict(script.key),
     }
 
 
 @action
 def set_camera_zoom_of_player(zoom: Number, player, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'playerCameraSetZoom',
```

### Comparing `pymodd-0.2.2/pymodd/functions.py` & `pymodd-0.3.0/pymodd/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 
 class SelectedItem(Item):
     def __init__(self):
         self.function = 'selectedItem'
         self.options = {}
 
 
-class TriggeringItem(Item):
+class LastTriggeringItem(Item):
     def __init__(self):
         self.function = 'getTriggeringItem'
         self.options = {}
 
 
 class ItemCurrentlyHeldByUnit(Item):
     def __init__(self, entity):
@@ -549,15 +549,15 @@
 # ---------------------------------------------------------------------------- #
 
 
 class Attribute(Function):
     pass
 
 
-class TriggeringAttribute(Attribute):
+class LastTriggeringAttribute(Attribute):
     def __init__(self):
         self.function = 'getTriggeringAttribute'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                                    Sensor                                    #
@@ -572,15 +572,15 @@
     def __init__(self, unit):
         self.function = 'getSensorOfUnit'
         self.options = {
             'unit': to_dict(unit),
         }
 
 
-class TriggeringSensor(Sensor):
+class LastTriggeringSensor(Sensor):
     def __init__(self):
         self.function = 'getTriggeringSensor'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                                    States                                    #
```

### Comparing `pymodd-0.2.2/pymodd/script.py` & `pymodd-0.3.0/pymodd/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
-import os
+import random
+import string
 from enum import Enum
 
 from caseconverter import camelcase, snakecase
 
 
 class Base():
     def to_dict(self):
@@ -91,15 +92,15 @@
         self.parent = parent
 
 
 class Folder(File):
     def __init__(self, name, scripts: list):
         super().__init__()
         self.name = name
-        self.key = key_from_name(self.name)
+        self.key = generate_random_key()
         self.scripts = scripts
         # set position of scripts inside the folder
         for i, script in enumerate(scripts):
             script.set_position(i, self.key)
 
     def to_dict(self):
         return {
@@ -108,18 +109,25 @@
             'parent': self.parent,
             'order': self.order,
             'expanded': True
         }
 
 
 class Script(File):
+    _class_to_key = {}
+
+    def __new__(cls, *args, **kwargs):
+        if cls._class_to_key.get(cls, None) is None:
+            cls._class_to_key[cls] = generate_random_key()
+        return super(Script, cls).__new__(cls, *args, **kwargs)
+
     def __init__(self):
         super().__init__()
         self.name = snakecase(self.__class__.__name__).replace('_', ' ')
-        self.key = key_from_name(self.name)
+        self.key = Script._class_to_key[self.__class__]
         self.triggers = []
         self.actions = []
 
     def _build(self):
         pass
 
     def to_dict(self):
@@ -131,68 +139,39 @@
             'name': self.name,
             'parent': self.parent,
             'key': self.key,
             'order': self.order
         }
 
 
-def key_from_name(name):
-    return snakecase(name)
+def script(triggers=[], name=None):
+    """
+    Args:
+        triggers (list, optional): triggers for the script. Defaults to [].
+        name (str, optional): name to override the default name of the script. Defaults to the class name of the script.
+    """
+    def wrapper_script(cls):
+        class NewScript(Script):
+            def __init__(self):
+                super().__init__()
+                self.triggers = triggers
+                if name is not None:
+                    self.name = name
+                else:
+                    self.name = snakecase(cls.__name__).replace('_', ' ')
+
+            def _build(self):
+                cls._build(self)
 
+        return NewScript
+    return wrapper_script
 
-def write_game_to_output(game):
-    print(f'\nWriting json files for {game.name}...')
 
-    base_output_path = f'{snakecase(game.name)}/output/'
-    write_scripts_to_output(f'{base_output_path}/game_scripts', game.scripts)
-    write_entity_scripts_to_output(
-        f'{base_output_path}/entity_scripts', game.entity_scripts)
-    write_game_json(base_output_path, game)
-
-    print('\nFinished writing.\n')
-
-
-def write_game_json(path, game):
-    file_name = f'{game.name}.json'
-    with open(f'{path}/{file_name}', 'w') as output:
-        output.write(json.dumps(game.to_dict(), indent=4))
-    print(f'\n{file_name} successfuly created')
-
-
-def write_entity_scripts_to_output(path, entity_scripts):
-    print('\nWriting entity scripts...')
-    for entity in entity_scripts:
-        entity_name = snakecase(entity.__class__.__name__)
-        print(f'\n  entity type: {entity_name}')
-        write_scripts_to_output(f'{path}/{entity_name}', entity.scripts)
-
-
-def write_scripts_to_output(path, scripts):
-    for script in scripts:
-        write_to_output(path, script)
-
-
-def write_to_output(path, obj):
-    depth = path.count('/')
-    if not os.path.exists(f'{path}/'):
-        os.makedirs(f'{path}/')
-    # create scripts inside folders
-    if isinstance(obj, Folder):
-        folder_name = snakecase(obj.name)
-        print(f"{'  ' * depth} {folder_name}/")
-        write_scripts_to_output(f'{path}/{folder_name}', obj.scripts)
-        return
-
-    file_name = f'{obj.__class__.__name__}'
-    # use script name
-    if isinstance(obj, Script):
-        file_name = f'{snakecase(obj.name)}'
-    with open(f'{path}/{file_name}.json', 'w') as output:
-        output.write(json.dumps(obj.to_dict(), indent=4))
-        print(f"{'  ' * depth} - {file_name}")
+def generate_random_key():
+    return ''.join(random.choices(string.ascii_letters + string.digits, k=10))
 
 
 def to_dict(obj):
     if isinstance(obj, Base):
         return obj.to_dict()
     if isinstance(obj, Enum):
         return obj.value
@@ -263,14 +242,18 @@
     DEBRIS_ENTERS_REGION = 'debrisEntersRegion'
 
     AD_PLAY_COMPLETED = 'adPlayCompleted'
     AD_PLAY_SKIPPED = 'adPlaySkipped'
     AD_PLAY_FAILED = 'adPlayFailed'
     AD_PLAY_BLOCKED = 'adPlayBlocked'
 
+    SEND_COINS_SUCCESS = 'sendCoinsSuccess'
+    COIN_SEND_FAILURE_DUE_TO_DAILY_LIMIT = 'coinSendFailureDueToDailyLimit'
+    COIN_SEND_FAILURE_DUE_TO_INSUFFICIENT_COINS = 'coinSendFailureDueToInsufficientCoins'
+
 
 class UiTarget(Enum):
     TOP = 'top'
     CENTER = 'center-lg'
     SCOREBOARD = 'scoreboard'
```

### Comparing `pymodd-0.2.2/pyproject.toml` & `pymodd-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pymodd"
-version = "0.2.2"
+version = "0.3.0"
 description = "A package for creating modd.io games using python!"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
     {name = "Jeff"}
 ]
@@ -23,12 +23,12 @@
 ]
 
 [project.urls]
 repository = "https://github.com/jeff5343/pymodd"
 changelog = "https://github.com/jeff5343/pymodd/releases"
 
 [project.scripts]
-generate-game = "pymodd.console_scripts.generate_project:main"
+pymodd = "pymodd.console_scripts.pymodd_command:main_cli"
 
 [tool.maturin]
-module-name = "pymodd._pymodd_generator"
-bindings = 'pyo3'
+module-name = "pymodd._pymodd_helper"
+bindings = 'pyo3'
```

### Comparing `pymodd-0.2.2/src/game_data/actions.rs` & `pymodd-0.3.0/src/game_data/actions.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use serde_json::{Map, Value};
 
-use crate::project_generator::utils::to_pymodd_maps::{PymoddStructure, ACTIONS_TO_PYMODD_STRUCTURE};
+use crate::project_generator::utils::to_pymodd_maps::{
+    PymoddStructure, ACTIONS_TO_PYMODD_STRUCTURE,
+};
 
 use super::argument::{
     align_arguments_with_pymodd_structure_parameters, parse_arguments_of_object_data, Argument,
 };
 
 pub fn parse_actions(actions_data: &Vec<Value>) -> Vec<Action> {
     actions_data
```

### Comparing `pymodd-0.2.2/src/game_data/argument.rs` & `pymodd-0.3.0/src/game_data/argument.rs`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                         "getVariable" => ArgumentValue::Value(
                             variable_id_from_get_variable_function_data(function_data),
                         ),
                         _ => ArgumentValue::Function(Function::parse(function_data)),
                     }
                 }
                 Value::Array(list_data) => {
-                    if list_data_contains_operator(&list_data) {
+                    if list_data_contains_an_operator(&list_data) {
                         // Convert conditions represented as a list by modd.io into a function
                         ArgumentValue::Function(Function::parse_condition_function(&list_data))
                     } else {
                         ArgumentValue::Actions(parse_actions(&list_data))
                     }
                 }
                 _ => ArgumentValue::Value(argument_data.clone()),
@@ -234,15 +234,15 @@
         .get("variable")
         .unwrap_or(&Value::Object(Map::new()))
         .get("key")
         .unwrap_or(&Value::Null)
         .to_owned()
 }
 
-fn list_data_contains_operator(list_data: &Vec<Value>) -> bool {
+fn list_data_contains_an_operator(list_data: &Vec<Value>) -> bool {
     list_data.len() == 3
         && list_data.iter().any(|value| {
             value
                 .as_object()
                 .unwrap_or(&Map::new())
                 .contains_key("operator")
         })
```

### Comparing `pymodd-0.2.2/src/game_data/directory.rs` & `pymodd-0.3.0/src/game_data/directory.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 use heck::ToPascalCase;
 use serde_json::{map::Values, Map, Value};
 
-use crate::project_generator::utils::{is_valid_class_name, to_pymodd_maps::TRIGGERS_TO_PYMODD_ENUM};
+use crate::project_generator::utils::{
+    is_valid_class_name, iterators::directory_iterator::DirectoryIterItem,
+    to_pymodd_maps::TRIGGERS_TO_PYMODD_ENUM,
+};
 
 use super::actions::{self, Action};
 
 const UNDEFINED_STRING: &str = "UNDEFINED";
 
 #[derive(Debug, PartialEq, Eq)]
 pub enum DirectoryItem {
@@ -62,14 +65,22 @@
             key: String::from("root"),
         }
     }
 
     pub fn is_empty(&self) -> bool {
         self.children.is_empty()
     }
+
+    pub fn find_item_with_key(&self, key: &str) -> Option<DirectoryIterItem> {
+        self.iter_flattened().find(|item| match item {
+            DirectoryIterItem::StartOfDirectory(dir) => dir.key == key,
+            DirectoryIterItem::Script(script) => script.key == key,
+            _ => false,
+        })
+    }
 }
 
 fn root_children_from_scripts_data(scripts: &Value) -> Vec<DirectoryItem> {
     let empty_map = Map::new();
     let mut items: Vec<&Value> =
         sort_based_on_order(scripts.as_object().unwrap_or(&empty_map).values());
 
@@ -171,15 +182,15 @@
             root_children_from_scripts_data, Directory, DirectoryItem, Script, UNDEFINED_STRING,
         },
     };
 
     use super::filter_out_children_of_parent;
 
     impl Directory {
-        fn new(name: &str, key: &str, children: Vec<DirectoryItem>) -> Directory {
+        pub fn new(name: &str, key: &str, children: Vec<DirectoryItem>) -> Directory {
             Directory {
                 name: name.to_string(),
                 key: key.to_string(),
                 children,
             }
         }
     }
```

### Comparing `pymodd-0.2.2/src/game_data/entity_types.rs` & `pymodd-0.3.0/src/game_data/entity_types.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/src/game_data/variable_categories.rs` & `pymodd-0.3.0/src/game_data/variable_categories.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/src/game_data.rs` & `pymodd-0.3.0/src/game_data.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 pub mod actions;
 pub mod argument;
 pub mod directory;
 pub mod entity_types;
 pub mod variable_categories;
 
 use heck::ToSnakeCase;
+use serde::Deserialize;
 use serde_json::Value;
 
 use self::{
     directory::Directory, entity_types::CategoriesToEntityTypes,
     variable_categories::CategoriesToVariables,
 };
 
@@ -18,15 +19,18 @@
     pub categories_to_variables: CategoriesToVariables,
     pub root_directory: Directory,
     pub categories_to_entity_types: CategoriesToEntityTypes,
 }
 
 impl GameData {
     pub fn parse(game_json_file_content: String) -> Result<GameData, &'static str> {
-        let game_json: Value = serde_json::from_str(&game_json_file_content)
+        let mut deserializer = serde_json::Deserializer::from_str(&game_json_file_content);
+        deserializer.disable_recursion_limit();
+        let deserializer = serde_stacker::Deserializer::new(&mut deserializer);
+        let game_json = Value::deserialize(deserializer)
             .map_err(|_| "error parsing modd.io json file!")?;
         let game_data = &game_json["data"];
         Ok(GameData {
             name: game_json
                 .get("title")
                 .ok_or("invalid modd.io json file! missing key: title")?
                 .to_string(),
```

### Comparing `pymodd-0.2.2/src/project_generator/entity_scripts_file.rs` & `pymodd-0.3.0/src/project_generator/entity_scripts_file.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 pub struct EntityScriptsFile {}
 
 impl EntityScriptsFile {
     pub fn build_content(game_data: &GameData) -> String {
         let mut content = format!(
             "from pymodd.actions import *\n\
             from pymodd.functions import *\n\
-            from pymodd.script import EntityScripts, Folder, Script, Trigger, UiTarget, Flip\n\n\
+            from pymodd.script import EntityScripts, Folder, Trigger, UiTarget, Flip, script\n\n\
             from game_variables import *\n\n\n"
         );
-        let scripts_class_content_builder =
-            ScriptsContentBuilder::new(&game_data.categories_to_variables);
+        let scripts_class_content_builder = ScriptsContentBuilder::new(
+            &game_data.categories_to_variables,
+            &game_data.root_directory,
+        );
 
         game_data
             .categories_to_entity_types
             .iter()
             .for_each(|(category, entity_types)| {
                 entity_types
                     .iter()
```

### Comparing `pymodd-0.2.2/src/project_generator/game_variables_file.rs` & `pymodd-0.3.0/src/project_generator/game_variables_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/src/project_generator/mapping_file.rs` & `pymodd-0.3.0/src/project_generator/mapping_file.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 use std::ops::Add;
 
 use heck::ToPascalCase;
 
 use crate::game_data::{directory::Directory, entity_types::CategoriesToEntityTypes, GameData};
 
-use super::{
-    utils::{iterators::directory_iterator::DirectoryIterItem, surround_string_with_quotes},
-    STORED_GAME_JSON_FILE_PATH,
-};
+use super::utils::{iterators::directory_iterator::DirectoryIterItem, surround_string_with_quotes};
 
 pub struct MappingFile {}
 
 impl MappingFile {
     pub fn build_content(game_data: &GameData) -> String {
         let game_class_name = game_data.name.to_pascal_case().to_string();
         let mut content = format!(
-            "from pymodd.script import Game, Folder, write_game_to_output, write_to_output\n\n\
+            "from pymodd.script import Game, Folder\n\n\
             from scripts import *\n\
             from entity_scripts import * \n\n\n\
             class {game_class_name}(Game):\n\
                 \tdef _build(self):\n\
                     \t\tself.entity_scripts = [{}]\n\
                     \t\tself.scripts = [\n",
             retrieve_clases_of_entity_scripts(&game_data.categories_to_entity_types).join(", ")
@@ -27,23 +24,25 @@
         content.push_str(
             &build_directory_items_contents(&game_data.root_directory)
                 .into_iter()
                 .map(|element| format!("{}{element}\n", "\t".repeat(3)))
                 .collect::<String>()
                 .as_str(),
         );
-        let project_directory = game_data.pymodd_project_name();
         content.add(
             &format!(
                 "\t\t\t\n\
-                \t\t]\n\n\
-                # run `python {project_directory}/mapping.py` to generate this game's files\n\
-                write_game_to_output({game_class_name}('{project_directory}/{STORED_GAME_JSON_FILE_PATH}'))\n\
-                # uncomment the following to quickly generate the json file for a script\n\
-                # write_to_output('output/', SCRIPT_OBJECT())"
+                \t\t]\n\n\n\
+                # run `pymodd compile` within this project directory to generate this game's json files\n\
+                # example:\n\
+                \"\"\"\n\
+                $ cd {}\n\
+                $ pymodd compile\n\
+                \"\"\"\n",
+                game_data.pymodd_project_name()
             )
             .as_str(),
         )
     }
 }
 
 fn retrieve_clases_of_entity_scripts(
@@ -133,26 +132,28 @@
                     "RW31QW2": { "name": "bob", "scripts": {
                         "DF31W32": { "name": "initialize", "key": "DF31W32", "actions": [], "parent": null, "order": 1 }
                     }},
                     "IO53IWD": { "name": "empty" }
                 }
             }
         }"#.to_string()).unwrap()), 
-        "from pymodd.script import Game, Folder, write_game_to_output, write_to_output\n\n\
+        "from pymodd.script import Game, Folder\n\n\
         from scripts import *\n\
         from entity_scripts import * \n\n\n\
         class TestGame(Game):\n\
             \tdef _build(self):\n\
                 \t\tself.entity_scripts = [Bob()]\n\
                 \t\tself.scripts = [\n\
                     \t\t\tInitialize(),\n\
                     \t\t\tFolder('utils', [\n\
                         \t\t\t\tChangeState(),\n\
                     \t\t\t]),\n\
                     \t\t\t\n\
-                \t\t]\n\n\
-        # run `python test_game/mapping.py` to generate this game's files\n\
-        write_game_to_output(TestGame('test_game/utils/game.json'))\n\
-        # uncomment the following to quickly generate the json file for a script\n\
-        # write_to_output('output/', SCRIPT_OBJECT())");
+                \t\t]\n\n\n\
+        # run `pymodd compile` within this project directory to generate this game's json files\n\
+        # example:\n\
+        \"\"\"\n\
+        $ cd test_game\n\
+        $ pymodd compile\n\
+        \"\"\"\n");
     }
 }
```

### Comparing `pymodd-0.2.2/src/project_generator/scripts_file.rs` & `pymodd-0.3.0/src/project_generator/scripts_file.rs`

 * *Files 11% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 pub struct ScriptsFile {}
 
 impl ScriptsFile {
     pub fn build_content(game_data: &GameData) -> String {
         let content = format!(
             "from pymodd.actions import *\n\
             from pymodd.functions import *\n\
-            from pymodd.script import Script, Trigger, UiTarget, Flip\n\n\
+            from pymodd.script import Trigger, UiTarget, Flip, script\n\n\
             from game_variables import *\n\n\n"
         );
         content.add(&build_directory_content(
             &game_data.root_directory,
-            &ScriptsContentBuilder::new(&game_data.categories_to_variables),
+            &ScriptsContentBuilder::new(
+                &game_data.categories_to_variables,
+                &game_data.root_directory,
+            ),
         ))
     }
 }
 
 pub fn build_directory_content(
     directory: &Directory,
     scripts_class_content_builder: &ScriptsContentBuilder,
@@ -58,89 +61,96 @@
         .collect::<String>()
         .trim_end()
         .to_string()
 }
 
 pub struct ScriptsContentBuilder<'a> {
     categories_to_variables: &'a CategoriesToVariables,
+    root_directory: &'a Directory,
 }
 
 impl<'a> ScriptsContentBuilder<'a> {
-    pub fn new(categories_to_variables: &'a CategoriesToVariables) -> ScriptsContentBuilder<'a> {
+    pub fn new(
+        categories_to_variables: &'a CategoriesToVariables,
+        root_directory: &'a Directory,
+    ) -> ScriptsContentBuilder<'a> {
         ScriptsContentBuilder {
             categories_to_variables,
+            root_directory,
         }
     }
 
     pub fn build_script_content(&self, script: &Script) -> String {
-        let (class_name, script_key): (String, &str) = (script.pymodd_class_name(), &script.key);
+        let class_name = script.pymodd_class_name();
         format!(
-            "class {class_name}(Script):\n\
+            "@script(triggers=[{}]{})\n\
+            class {class_name}():\n\
             \tdef _build(self):\n\
-                \t\tself.key = '{script_key}'\n\
-                \t\tself.triggers = [{}]\n\
                 \t\tself.actions = [\n\
                 {}\
                 \t\t\t\n\
                 \t\t]\n",
             script.triggers_into_pymodd_enums().join(", "),
+            if !script.name.is_ascii() {
+                format!(", name={}", surround_string_with_quotes(&script.name))
+            } else {
+                String::new()
+            },
             self.build_actions_content(&script.actions)
                 .lines()
                 .map(|action| format!("{}{action}\n", "\t".repeat(3)))
                 .collect::<String>(),
         )
     }
 
     fn build_actions_content(&self, actions: &Vec<Action>) -> String {
         actions
             .iter()
-            .map(|action| {
-                match action.name.as_str() {
-                    "comment" => {
-                        // pull out comment field for Comment action
-                        format!(
-                            "{}({}{}),\n",
-                            action.pymodd_class_name(),
-                            surround_string_with_quotes(
-                                action.comment.as_ref().unwrap_or(&String::from("None"))
-                            ),
-                            self.build_optional_arguments_contents(&action)
-                                .into_iter()
-                                .skip(1)
-                                .map(|arg| String::from(", ") + &arg)
-                                .collect::<String>(),
-                        )
-                    }
-                    _ => self.build_action_content(&action),
-                }
-            })
+            .map(|action| self.build_action_content(&action))
             .collect::<String>()
     }
 
     fn build_action_content(&self, action: &Action) -> String {
-        format!(
-            "{}({}",
-            action.pymodd_class_name(),
-            self.build_arguments_content(action.iter_flattened_argument_values())
-        )
-        .add(
-            &self
-                .build_optional_arguments_contents(&action)
-                .into_iter()
-                .enumerate()
-                .map(|(i, arg)| {
-                    if action.args.is_empty() && i == 0 {
-                        arg
-                    } else {
-                        String::from(", ") + &arg
-                    }
-                })
-                .collect::<String>(),
-        )
-        .add("),\n")
+        match action.name.as_str() {
+            "comment" => {
+                format!(
+                    "{}({}{}),\n",
+                    action.pymodd_class_name(),
+                    // set argument manually for comments
+                    surround_string_with_quotes(
+                        action.comment.as_ref().unwrap_or(&String::from("None"))
+                    ),
+                    self.build_optional_arguments_contents(&action)
+                        .into_iter()
+                        .skip(1) // skip over optional comment argument
+                        .map(|arg| String::from(", ") + &arg)
+                        .collect::<String>(),
+                )
+            }
+            _ => format!(
+                "{}({}",
+                action.pymodd_class_name(),
+                self.build_arguments_content(action.iter_flattened_argument_values())
+            )
+            .add(
+                &self
+                    .build_optional_arguments_contents(&action)
+                    .into_iter()
+                    .enumerate()
+                    .map(|(i, arg)| {
+                        if action.args.is_empty() && i == 0 {
+                            arg
+                        } else {
+                            String::from(", ") + &arg
+                        }
+                    })
+                    .collect::<String>(),
+            )
+            .add("),\n"),
+        }
     }
 
     fn build_arguments_content(&self, args_iter: ArgumentValuesIterator) -> String {
         args_iter
             .fold(String::from("("), |pymodd_args, arg| {
                 let include_seperator =
                     !pymodd_args.ends_with("(") && arg != ArgumentValueIterItem::FunctionEnd;
@@ -198,14 +208,24 @@
             },
             ArgumentValueIterItem::Constant(constant) => constant.to_owned(),
             ArgumentValueIterItem::Condition(operation)
             | ArgumentValueIterItem::Concatenation(operation)
             | ArgumentValueIterItem::Calculation(operation) => {
                 self.build_operation_content(&operation)
             }
+            ArgumentValueIterItem::ScriptKey(key) => {
+                let item_with_key = self.root_directory.find_item_with_key(&key);
+                if item_with_key.is_some() {
+                    if let DirectoryIterItem::Script(script) = item_with_key.unwrap() {
+                        // run_script action accepts Script objects, not keys
+                        return format!("{}()", script.pymodd_class_name());
+                    }
+                }
+                String::from("None")
+            }
             ArgumentValueIterItem::FunctionEnd => String::from(")"),
         }
     }
 
     fn build_operation_content(&self, operator: &Operation) -> String {
         let (item_a, operator, item_b) = (
             ArgumentValueIterItem::from_argument(&operator.item_a),
@@ -271,49 +291,78 @@
 mod tests {
     use std::collections::HashMap;
 
     use serde_json::json;
 
     use crate::game_data::{
         actions::parse_actions,
-        directory::Script,
+        directory::{Directory, DirectoryItem, Script},
         variable_categories::{CategoriesToVariables, Variable},
     };
 
     use super::ScriptsContentBuilder;
 
     #[test]
     fn script_content() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
-                .build_script_content(&Script::new(
-                    "initialize",
-                    "WI31HDK",
-                    vec!["gameStart"],
-                    Vec::new()
-                )),
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_script_content(&Script::new(
+                "initialize",
+                "WI31HDK",
+                vec!["gameStart"],
+                Vec::new()
+            )),
+            String::from(format!(
+                "@script(triggers=[Trigger.GAME_START])\n\
+                class Initialize():\n\
+                    \tdef _build(self):\n\
+                        \t\tself.actions = [\n\
+                        \t\t\t\n\
+                        \t\t]\n",
+            ))
+        );
+    }
+
+    #[test]
+    fn script_with_weird_name_content() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_script_content(&Script::new(
+                "【 𝚒𝚗𝚒𝚝𝚒𝚊𝚕𝚒𝚣𝚎 イ】",
+                "WI31HDK",
+                vec!["gameStart"],
+                Vec::new()
+            )),
             String::from(format!(
-                "class Initialize(Script):\n\
+                "@script(triggers=[Trigger.GAME_START], name='【 𝚒𝚗𝚒𝚝𝚒𝚊𝚕𝚒𝚣𝚎 イ】')\n\
+                class q():\n\
                     \tdef _build(self):\n\
-                        \t\tself.key = 'WI31HDK'\n\
-                        \t\tself.triggers = [Trigger.GAME_START]\n\
                         \t\tself.actions = [\n\
                         \t\t\t\n\
                         \t\t]\n",
             ))
         );
     }
 
     #[test]
     fn parse_action_with_variable_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::from([(
-                "shops",
-                vec![Variable::new("OJbEQyc7is", "WEAPONS", None)]
-            )])))
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::from([(
+                    "shops",
+                    vec![Variable::new("OJbEQyc7is", "WEAPONS", None)]
+                )])),
+                &Directory::new("root", "null", Vec::new())
+            )
             .build_actions_content(&parse_actions(
                 &json!([
                     {
                         "type": "openShopForPlayer",
                             "player": {
                                 "function": "getOwner",
                                 "entity": {
@@ -332,93 +381,110 @@
             "open_shop_for_player(Shops.WEAPONS, OwnerOfEntity(LastCastingUnit())),\n"
         )
     }
 
     #[test]
     fn parse_action_with_optional_arguments_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
-                .build_actions_content(&parse_actions(
-                    &json!([
-                        {
-                            "type": "runScript",
-                            "scriptName": "fjw24WdJ",
-                            "comment": "hi!",
-                            "runOnClient": true,
-                            "disabled": true,
-                        }
-                    ])
-                    .as_array()
-                    .unwrap()
-                )),
-            "run_script('fjw24WdJ', comment='hi!', disabled=True, run_on_client=True),\n"
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([
+                    {
+                        "type": "startUsingItem",
+                        "entity": {
+                            "function": "getTriggeringItem"
+                        },
+                        "comment": "hi!",
+                        "runOnClient": true,
+                        "disabled": true,
+                    }
+                ])
+                .as_array()
+                .unwrap()
+            )),
+            "use_item_continuously_until_stopped(LastTriggeringItem(), comment='hi!', disabled=True, run_on_client=True),\n"
         )
     }
 
     #[test]
     fn parse_action_with_only_optional_arguments_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
-                .build_actions_content(&parse_actions(
-                    &json!([
-                        {
-                            "type": "return",
-                            "comment": "hi!",
-                            "runOnClient": true,
-                            "disabled": false,
-                        }
-                    ])
-                    .as_array()
-                    .unwrap()
-                )),
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([
+                    {
+                        "type": "return",
+                        "comment": "hi!",
+                        "runOnClient": true,
+                        "disabled": false,
+                    }
+                ])
+                .as_array()
+                .unwrap()
+            )),
             "return_loop(comment='hi!', run_on_client=True),\n"
         )
     }
 
     #[test]
     fn parse_action_with_constant_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
-                .build_actions_content(&parse_actions(
-                    &json!([
-                        {
-                            "type": "updateUiTextForEveryone",
-                            "target": "top",
-                            "value": "Hello!"
-                        }
-                    ])
-                    .as_array()
-                    .unwrap()
-                )),
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([
+                    {
+                        "type": "updateUiTextForEveryone",
+                        "target": "top",
+                        "value": "Hello!"
+                    }
+                ])
+                .as_array()
+                .unwrap()
+            )),
             "update_ui_text_for_everyone(UiTarget.TOP, 'Hello!'),\n"
         )
     }
 
     #[test]
     fn parse_comment_action_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
-                .build_actions_content(&parse_actions(
-                    &json!([
-                        {
-                            "type": "comment",
-                            "comment": "hey there",
-                        }
-                    ])
-                    .as_array()
-                    .unwrap()
-                )),
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([
+                    {
+                        "type": "comment",
+                        "comment": "hey there",
+                    }
+                ])
+                .as_array()
+                .unwrap()
+            )),
             "comment('hey there'),\n"
         );
     }
 
     #[test]
     fn parse_nested_calculations_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
                 .build_actions_content(&parse_actions(
                     &json!([
                         {
                             "type": "increaseVariableByNumber",
                             "variable": null,
                             "number": {
                                 "function": "calculate",
@@ -441,15 +507,18 @@
             "increase_variable_by_number(None, RandomNumberBetween(0, 5) * ((CurrentUnixTimeStamp() ** 2) + 3)),\n"
         );
     }
 
     #[test]
     fn parse_nested_concatenations_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
                 .build_actions_content(&parse_actions(
                     &json!([
                         {
                             "type": "sendChatMessage",
                             "message": {
                                 "function": "concat",
                                 "textA": "hi ",
@@ -472,54 +541,57 @@
             "send_chat_message_to_everyone('hi ' + IdOfPlayer(LastTriggeringPlayer()) + ' player!'),\n"
         );
     }
 
     #[test]
     fn parse_nested_if_statements_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
-                .build_actions_content(&parse_actions(
-                    json!([
-                         {
-                            "type": "condition",
-                            "conditions": [
-                                { "operandType": "boolean", "operator": "==" },
-                                true,
-                                true
-                            ],
-                            "then": [
-                                {
-                                    "type": "condition",
-                                    "conditions": [
-                                        { "operandType": "boolean", "operator": "==" },
-                                        true,
-                                        true
-                                    ],
-                                    "then": [
-                                        {
-                                            "type": "condition",
-                                            "conditions": [
-                                                { "operandType": "boolean", "operator": "==" },
-                                                true,
-                                                true
-                                            ],
-                                            "then": [],
-                                            "else": []
-                                        }
-                                    ],
-                                    "else": []
-                                   }
-                              ],
-                              "else": []
-                         }
-                    ])
-                    .as_array()
-                    .unwrap(),
-                ))
-                .as_str(),
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                     {
+                        "type": "condition",
+                        "conditions": [
+                            { "operandType": "boolean", "operator": "==" },
+                            true,
+                            true
+                        ],
+                        "then": [
+                            {
+                                "type": "condition",
+                                "conditions": [
+                                    { "operandType": "boolean", "operator": "==" },
+                                    true,
+                                    true
+                                ],
+                                "then": [
+                                    {
+                                        "type": "condition",
+                                        "conditions": [
+                                            { "operandType": "boolean", "operator": "==" },
+                                            true,
+                                            true
+                                        ],
+                                        "then": [],
+                                        "else": []
+                                    }
+                                ],
+                                "else": []
+                               }
+                          ],
+                          "else": []
+                     }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
             "if_else((True == True), [\n\
                 \tif_else((True == True), [\n\
     		        \t\tif_else((True == True), [\n\
 		                \t\t\t\n\
 		            \t\t], [\n\
 		                \t\t\t\n\
 		            \t\t]),\n\
@@ -533,15 +605,18 @@
             ]),\n"
         )
     }
 
     #[test]
     fn parse_nested_conditions_into_pymodd() {
         assert_eq!(
-            ScriptsContentBuilder::new(&CategoriesToVariables::new(HashMap::new()))
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
                 .build_actions_content(&parse_actions(
                     json!([
                          {
                             "type": "condition",
                             "conditions": [
                                 { "operandType": "and", "operator": "AND" },
                                 [
@@ -566,8 +641,43 @@
             "if_else(((NumberOfUnitsOfUnitType('oTDQ3jlcMa') == 5) & (True == True)), [\n\
                 \t\n\
             ], [\n\
                 \t\n\
             ]),\n"
         );
     }
+
+    #[test]
+    fn parse_run_script_action_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new(
+                    "root",
+                    "null",
+                    vec![DirectoryItem::Directory(Directory::new(
+                        "utils",
+                        "n3DhW3",
+                        vec![DirectoryItem::Script(Script {
+                            name: String::from("spawn boss"),
+                            key: String::from("If2aW3B"),
+                            triggers: Vec::new(),
+                            actions: Vec::new()
+                        })]
+                    ))]
+                )
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                     {
+                        "type": "runScript",
+                        "scriptName": "If2aW3B"
+                     }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "run_script(SpawnBoss()),\n"
+        )
+    }
 }
```

### Comparing `pymodd-0.2.2/src/project_generator/utils/iterators/argument_values_iterator.rs` & `pymodd-0.3.0/src/project_generator/utils/iterators/argument_values_iterator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     StartOfFunction(&'a Function),
     Actions(&'a Vec<Action>),
     Value(&'a Value),
     Constant(&'a String),
     Condition(Operation),
     Concatenation(Operation),
     Calculation(Operation),
+    ScriptKey(String),
     FunctionEnd,
 }
 
 impl<'a> ArgumentValueIterItem<'a> {
     pub fn from_argument(argument: &Argument) -> ArgumentValueIterItem {
         match &argument.value {
             ArgumentValue::Function(function) => {
@@ -78,15 +79,21 @@
                     ("condition", Some(operation)) => ArgumentValueIterItem::Condition(operation),
                     ("concat", Some(operation)) => ArgumentValueIterItem::Concatenation(operation),
                     (_, Some(operation)) => ArgumentValueIterItem::Calculation(operation),
                     _ => ArgumentValueIterItem::StartOfFunction(&function),
                 }
             }
             ArgumentValue::Constant(constant) => ArgumentValueIterItem::Constant(&constant),
-            ArgumentValue::Value(value) => ArgumentValueIterItem::Value(&value),
+            ArgumentValue::Value(value) => {
+                if value.is_string() && argument.name.as_str() == "scriptName" {
+                    ArgumentValueIterItem::ScriptKey(value.as_str().unwrap().to_string())
+                } else {
+                    ArgumentValueIterItem::Value(&value)
+                }
+            }
             ArgumentValue::Actions(actions) => ArgumentValueIterItem::Actions(&actions),
         }
     }
 }
 
 #[derive(Debug, Eq, PartialEq)]
 pub struct Operation {
```

### Comparing `pymodd-0.2.2/src/project_generator/utils/iterators/directory_iterator.rs` & `pymodd-0.3.0/src/project_generator/utils/iterators/directory_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/src/project_generator/utils/to_pymodd_maps.rs` & `pymodd-0.3.0/src/project_generator/utils/to_pymodd_maps.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/src/project_generator/utils.rs` & `pymodd-0.3.0/src/project_generator/utils.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.2.2/src/project_generator.rs` & `pymodd-0.3.0/src/project_generator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,22 @@
             // insert project directory as parent to all file paths
             path: PathBuf::from(game_data.pymodd_project_name()).join(file.path),
             content: file.content,
         }) {
             // unwrap is fine as all files have the project directory as parent
             let parent = file.path.parent().unwrap();
             if !parent.exists() {
-                fs::create_dir_all(parent).map_err(|_| "error creating project directories!")?;
+                fs::create_dir_all(parent).map_err(|_| "error creating a pymodd project directories!")?;
             }
             write!(
-                fs::File::create(&file.path).map_err(|_| "error creating project file!")?,
+                fs::File::create(&file.path).map_err(|_| "error creating a pymodd project file!")?,
                 "{}",
                 file.content
             )
-            .map_err(|_| "error writing to project file!")?;
+            .map_err(|_| "error writing to a pymodd project file!")?;
             generation_logger(file);
         }
         Ok(())
     }
 }
 
 pub struct File {
```

### Comparing `pymodd-0.2.2/Cargo.lock` & `pymodd-0.3.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "crossterm"
@@ -150,22 +156,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
-name = "pymodd_generator"
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "pymodd_helper"
 version = "0.1.0"
 dependencies = [
  "crossterm",
  "heck",
  "lazy_static",
  "pyo3",
+ "serde",
  "serde_json",
+ "serde_stacker",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
@@ -252,30 +269,40 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
 
 [[package]]
 name = "serde_json"
 version = "1.0.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "877c235533714907a8c2464236f5c4b2a17262ef1bd71f38f35ea592c8da6883"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_stacker"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f5557f4c1103cecd0e639a17ab22d670b89912d8a506589ee627bf738a15a5d"
+dependencies = [
+ "serde",
+ "stacker",
+]
+
+[[package]]
 name = "signal-hook"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
 dependencies = [
  "libc",
  "signal-hook-registry",
@@ -304,14 +331,27 @@
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "syn"
 version = "1.0.107"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
 dependencies = [
  "proc-macro2",
  "quote",
```

### Comparing `pymodd-0.2.2/PKG-INFO` & `pymodd-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodd
-Version: 0.2.2
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: case-converter==1.1.0
 License-File: LICENSE.txt
 Summary: A package for creating modd.io games using python!
 Author: Jeff
@@ -30,15 +30,15 @@
    :alt: PyPI - License
 
 Features
 --------
 
 - edit global and entity scripts
 - organize folders and scripts with a mapping file
-- a command to generate a pymodd project
+- a command to generate and compile a pymodd project
 
 Installing
 ----------
 
 **Python 3.8 or higher is required**
 
 To install the library run the following command:
@@ -55,36 +55,36 @@
 Getting Started
 ---------------
 
 Export your modd game json file from the website and then generate a pymodd project by running the following command:
 
 .. code:: sh
 
-    generate-game [GAME_JSON_FILE_PATH]
+    pymodd generate-project [GAME_JSON_FILE_PATH]
 
 
 Quick Script Example
 --------------------
 
-view examples/sample_scripts.py in the github repo for the full example
+view the ``examples/froge directory`` for a generated pymodd project
 
 .. code:: py
 
-    class EverySecond(Script):
+    @script(triggers=[Trigger.EVERY_SECOND])
+    class EverySecond():
         def _build(self):
-            self.key = 'P8MwXcSxq7'
-            self.triggers = [Trigger.EVERY_SECOND]
             self.actions = [
                 if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG) < 5), [
                     create_unit_for_player_at_position_with_rotation(UnitTypes.FROG, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
                 ], [
                     if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG_BOSS) == 0), [
                         if_else((Variables.BOSS_TIMER <= 0), [
                             create_unit_for_player_at_position_with_rotation(UnitTypes.FROG_BOSS, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
                             update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000),
+                            set_variable(Variables.BOSS_TIMER, 200),
                         ], [
                         ]),
                         decrease_variable_by_number(Variables.BOSS_TIMER, 1),
                     ], [
                     ]),
                 ]),
             ]
```

