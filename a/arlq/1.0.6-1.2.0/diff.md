# Comparing `tmp/arlq-1.0.6.tar.gz` & `tmp/arlq-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.0.6.tar", last modified: Sat Apr 15 13:02:16 2023, max compression
+gzip compressed data, was "arlq-1.2.0.tar", last modified: Mon Apr 17 12:40:05 2023, max compression
```

## Comparing `arlq-1.0.6.tar` & `arlq-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 13:02:16.401621 arlq-1.0.6/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.6/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 13:02:16.401621 arlq-1.0.6/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-15 10:32:33.000000 arlq-1.0.6/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 13:02:16.397621 arlq-1.0.6/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.6/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-15 12:49:29.000000 arlq-1.0.6/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    19706 2023-04-15 12:56:17.000000 arlq-1.0.6/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 13:02:16.401621 arlq-1.0.6/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-15 13:02:16.401621 arlq-1.0.6/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.6/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-17 12:40:05.617907 arlq-1.2.0/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.2.0/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-17 12:40:05.617907 arlq-1.2.0/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-17 11:28:51.000000 arlq-1.2.0/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-17 12:40:05.617907 arlq-1.2.0/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.2.0/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-16 12:23:10.000000 arlq-1.2.0/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    21720 2023-04-17 11:56:08.000000 arlq-1.2.0/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-17 12:40:05.617907 arlq-1.2.0/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-17 12:40:05.617907 arlq-1.2.0/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.2.0/setup.py
```

### Comparing `arlq-1.0.6/LICENSE` & `arlq-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.0.6/PKG-INFO` & `arlq-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.6
+Version: 1.2.0
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.6/README.md` & `arlq-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,20 +37,20 @@
 |Monster Display, Name | Description |
 |---|---|
 |a Amoeba|Weak enough for the player to defeat from the start. Good for leveling up.|
 |b Bison|Second weakest. Gives lots of food. Hunt a Bison when you're hungry!|
 |c Chimera|Fairly strong. Carries a sword that you can obtain when defeated. With the sword, your attack power triples in the next battle.|
 |d Komodo Dragon|Strong. If defeated, provides a lot of food, but being poisoned, your attack power will be reduced to one-third in the next battle.|
 |f Fairy|Not a foe. Follows you when you come in contact. Gives you a small blessing.|
-|g Gorgon|A monster that petrifies you instantly just by making eye contact. Without a fairy companion, your body will be petrified for 48 hours! Be careful!|
 |A Rare Amoeba|A rare Amoeba that boosts your level significantly!|
 |B Rare Bison|So delicious that you'll probably eat much more than a regular Bison|
 |C Rare Chimera|In addition to the sword, it possesses clairvoyance.|
 |D Dragon|Strong. Defeating the Dragon reveals the treasure chest ("T") location. Even if you don't defeat it, you'll be able to recognize the chest.|
 |E Elemental|Not a foe. Teleports the player to a random location in the dungeon. Offers extra services for high-level players.|
+|G Gorgon|A monster that petrifies you instantly just by making eye contact. Without a fairy companion, your body will be petrified for 48 hours! Be careful!|
 
 ## License
 
 The license for this code is BSD-2.
 
 However, please note that the way the code generated by AI is treated depends on the laws in the country where you live, regardless of the license chosen by the developer (myself).
 Also, please note that I have not directly copied and pasted any source code other than what ChatGPT has generated.
```

### Comparing `arlq-1.0.6/arlq/arlq.py` & `arlq-1.2.0/arlq/arlq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from typing import Dict, List, Optional, Set, Tuple
 
 import argparse
 import curses
 import math
-import random
 import sys
+import time
 
 try:
     from ._version import __version__
 except:
     __version__ = "(unknown)"
 
 ROOM_WIDTH = 5
 ROOM_HEIGHT = 4
 ROOM_NUM_X = 12
 ROOM_NUM_Y = 4
 FIELD_WIDTH = (ROOM_WIDTH + 1) * ROOM_NUM_X + 1
 FIELD_HEIGHT = (ROOM_HEIGHT + 1) * ROOM_NUM_Y + 1
+CORRIDOR_V_WIDTH = 3
+CORRIDOR_H_WIDTH = 2
+WALL_CHARS = "###"  # cross, horizontal, vertical
 
 FOOD_MAX = 120
 FOOD_INIT = 90
+FOOD_STARVATION = 30
+
 FOOD_BISON = 40
 FOOD_SPECIAL_BISON = 80
 FOOD_AMOEBA = 8
 FOOD_CHIMERA = 8
 FOOD_COMODO_DRAGON = 30
 FOOD_DRAGON = 10
 FOOD_ELEMENTAL = 0
@@ -34,25 +39,42 @@
 ITEM_POISONED = "Poisoned"
 ITEM_RANDOM_TRANSPORT = "Random Trans."
 ITEM_SPECIAL_EXP = "Special Exp."
 ITEM_SPECIAL_BISON_MEAT = "Bison Meat++"
 ITEM_SWORD_AND_CLAIRVOYANCE = "Sword & Eye"
 ITEM_TREASURE_POINTER = "Treasure Ptr."
 ITEM_STONED = "Stoned"
+ITEM_TREASURE = "Treasure"
 
 COMPANION_FAIRY = "Fairy"
 
 CHAR_DRAGON = "D"
 CHAR_TREASURE = "T"
 
 
 Point = Tuple[int, int]
 Edge = Tuple[Point, Point]
 
 
+class MyRandom:
+    def __init__(self, seed):
+        self._value = self.seed = seed
+
+    def randrange(self, r):
+        self._value = (1103515245 * self._value + 12345) % (2 ** 32)
+        return self._value % r
+
+    def choice(self, items):
+        i = self.randrange(len(items))
+        return items[i]
+
+
+rand: MyRandom = None
+
+
 def gen_maze(width: int, height: int) -> List[Edge]:
     # Returns a list of neighboring points given a point p
     def neighbor_points(p):
         x, y = p
         return [(x, y - 1), (x, y + 1), (x - 1, y), (x + 1, y)]
 
     # Returns True if the given point p is within the bounds of the maze
@@ -62,36 +84,36 @@
     # Initialize the maze generation process
     unconnected_point_set = set((x, y) for y in range(height) for x in range(width))
     connecting_points = []
     done_points = []
     edges = []
 
     # Choose a random starting point
-    cur_p = random.choice(list(unconnected_point_set))
+    cur_p = rand.choice(list(unconnected_point_set))
     unconnected_point_set.remove(cur_p)
     connecting_points.append(cur_p)
 
     # Keep generating until all points have been connected
     while len(done_points) < width * height:
         # Choose a random connecting point
-        i = random.randrange(len(connecting_points))
+        i = rand.randrange(len(connecting_points))
         cur_p = connecting_points[i]
 
         # Find neighboring points that haven't been connected yet
         nps = neighbor_points(cur_p)
         unconnected_nps = [np for np in nps if is_within_bounds(np) and np in unconnected_point_set]
 
         # If there are no unconnected neighboring points, remove this point from the connecting points list
         if not unconnected_nps:
             done_points.append(cur_p)
             del connecting_points[i]
             continue
 
         # Choose a random unconnected neighboring point and connect it
-        selected_np = random.choice(unconnected_nps)
+        selected_np = rand.choice(unconnected_nps)
         unconnected_point_set.remove(selected_np)
         connecting_points.append(selected_np)
 
         # Add the edge between the current point and the selected neighboring point to the list of edges
         edges.append((cur_p, selected_np))
 
     # Return the list of edges that connect all points in the maze
@@ -158,40 +180,39 @@
     MonsterKind("a", 1, FOOD_AMOEBA),  # Amoeba
     MonsterKind("b", 3, FOOD_BISON, item=ITEM_BISON_MEAT),  # Bison
     MonsterKind("c", 6, FOOD_CHIMERA, item=ITEM_SWORD),  # Chimera
     MonsterKind("d", 15, FOOD_COMODO_DRAGON, item=ITEM_POISONED),  # Comodo Dragon
     MonsterKind(CHAR_DRAGON, 15, FOOD_DRAGON, item=ITEM_TREASURE_POINTER),  # Dragon
     MonsterKind("E", 20, FOOD_ELEMENTAL, item=ITEM_RANDOM_TRANSPORT),  # Elemental
     MonsterKind("f", 0, 0, companion=COMPANION_FAIRY),  # Fairy
-    MonsterKind("g", 0, FOOD_GORGON, item=ITEM_STONED),  # Gorgon
 ]
 
 RARE_MONSTER_KINDS: List[MonsterKind] = [
     MonsterKind("A", 1, FOOD_AMOEBA, item=ITEM_SPECIAL_EXP),  # Amoeba rare
     MonsterKind("B", 3, FOOD_SPECIAL_BISON, item=ITEM_SPECIAL_BISON_MEAT),  # Bison rare
     MonsterKind("C", 6, FOOD_CHIMERA, item=ITEM_SWORD_AND_CLAIRVOYANCE),  # Chimera rare
+    MonsterKind("G", 0, FOOD_GORGON, item=ITEM_STONED),  # Gorgon
 ]
 
 MONSTER_KIND_POPULATION: Dict[str, int] = {
     "a": 20,
     "b": 4,
     "c": 4,
     "d": 4,
     "D": 1,
     "E": 2,
     "f": 1,
-    "g": 1,
 }
 
 
 def find_random_place(objects: List[Entity], field: List[List[str]], distance: int) -> Point:
     places = [(o.x, o.y) for o in objects]
     while True:
-        x = random.randint(1, FIELD_WIDTH - 2)
-        y = random.randint(1, FIELD_HEIGHT - 2)
+        x = rand.randrange(FIELD_WIDTH - 2) + 1
+        y = rand.randrange(FIELD_HEIGHT - 2) + 1
         if (
             field[y][x] == " "
             and field[y][x + 1] == " "
             and not any(abs(p[0] - x) <= distance and abs(p[1] - y) <= distance for p in places)
         ):
             return x, y
 
@@ -205,50 +226,56 @@
     - field: the game field
 
     This function modifies the objects list by adding newly spawned monsters.
     """
 
     for kind in MONSTER_KINDS:
         for _ in range(MONSTER_KIND_POPULATION[kind.char]):
-            x, y = find_random_place(objects, field, 2)
+            x, y = find_random_place(objects, field, 3)
             m = Monster(x, y, kind)
             objects.append(m)
-    kind = random.choice(RARE_MONSTER_KINDS)
-    x, y = find_random_place(objects, field, 2)
+    kind = rand.choice(RARE_MONSTER_KINDS)
+    x, y = find_random_place(objects, field, 3)
     m = Monster(x, y, kind)
     objects.append(m)
 
 
-def create_field() -> List[List[str]]:
+def create_field(corridor_h_width: int, corridor_v_width: int, wall_chars: str) -> List[List[str]]:
     # Create field filled with spaces
     field = [[" " for _ in range(FIELD_WIDTH)] for _ in range(FIELD_HEIGHT)]
 
     # Create walls
     for ry in range(ROOM_NUM_Y + 1):
         y = ry * (ROOM_HEIGHT + 1)
         for x in range(0, FIELD_WIDTH):
-            field[y][x] = "#"
+            field[y][x] = wall_chars[1]
     for rx in range(ROOM_NUM_X + 1):
         x = rx * (ROOM_WIDTH + 1)
         for y in range(0, FIELD_HEIGHT):
-            field[y][x] = "#"
+            field[y][x] = wall_chars[2]
+    for ry in range(ROOM_NUM_Y + 1):
+        y = ry * (ROOM_HEIGHT + 1)
+        for rx in range(ROOM_NUM_X + 1):
+            x = rx * (ROOM_WIDTH + 1)
+            field[y][x] = wall_chars[0]
 
     # Create corridors
     edges = gen_maze(ROOM_NUM_X, ROOM_NUM_Y)
     for edge in edges:
         (x1, y1), (x2, y2) = sorted(edge)
         assert x1 <= x2
         assert y1 <= y2
-        d = random.randrange(3) + 1  # 1, 2, 3
         if y1 == y2:
-            for y in range(ROOM_HEIGHT - 2):
+            d = rand.randrange(ROOM_HEIGHT + 1 - corridor_h_width) + 1
+            for y in range(corridor_h_width):
                 field[y1 * (ROOM_HEIGHT + 1) + d + y][x2 * (ROOM_WIDTH + 1)] = " "
         else:
             assert x1 == x2
-            for x in range(ROOM_WIDTH - 2):
+            d = rand.randrange(ROOM_WIDTH + 1 - corridor_v_width) + 1
+            for x in range(corridor_v_width):
                 field[y2 * (ROOM_HEIGHT + 1)][x1 * (ROOM_WIDTH + 1) + d + x] = " "
 
     return field
 
 
 def draw_stage(
     stdscr: curses.window,
@@ -268,16 +295,16 @@
     if player.companion:
         stdscr.addstr(py, px + 1, "'", curses.color_pair(2) | curses.A_BOLD)
 
     for y, row in enumerate(field):
         for x, cell in enumerate(row):
             if (not show_entities or cell == " ") and torched[y][x] == 0:
                 stdscr.addstr(y, x, ".", curses.A_DIM)
-            elif cell == "#":
-                stdscr.addstr(y, x, "#", curses.color_pair(1))
+            elif cell != " ":
+                stdscr.addstr(y, x, cell, curses.color_pair(1))
 
     stdscr.addstr(py, px, "@", curses.color_pair(2) | curses.A_BOLD)
 
     for o in objects:
         if isinstance(o, Monster):
             m = o
             if torched[m.y][m.x] == 0:
@@ -349,14 +376,19 @@
     if beatable is not None:
         buf.append("> %s" % beatable.char)
     buf.append("FOOD: %d" % player.food)
     buf.append(item_str)
     buf.append("/ [Q] to exit")
     stdscr.addstr(FIELD_HEIGHT, 0, "  ".join(buf))
 
+    if player.item == ITEM_TREASURE or player.food <= 0:
+        if not message:
+            message = ''
+        message += "  SEED: %d" % rand.seed
+
     if message:
         stdscr.addstr(FIELD_HEIGHT + 1, 0, message)
 
 
 def key_to_dir(key: int) -> Optional[Point]:
     dx, dy = 0, 0
     if key in [ord("w"), curses.KEY_UP]:
@@ -398,15 +430,16 @@
     if sh < FIELD_HEIGHT + 2 or sw < FIELD_WIDTH:
         raise TerminalSizeSmall()
 
     assert args_box
     args = args_box[0]
 
     # Set up the game
-    field: List[List[str]] = create_field()
+    corridor_h_width, corridor_v_width = (1, 2) if args.narrower_corridors else (CORRIDOR_H_WIDTH, CORRIDOR_V_WIDTH)
+    field: List[List[str]] = create_field(corridor_h_width, corridor_v_width, WALL_CHARS)
     torched: List[List[int]] = [[0 for _ in range(FIELD_WIDTH)] for _ in range(FIELD_HEIGHT)]
     x, y = find_random_place([], field, 2)
     player: Player = Player(x, y, 1, FOOD_INIT)
     objects: List[Entity] = [player]
     treasure: Treasure = Treasure(*find_random_place(objects, field, 2))
     objects.append(treasure)
     spawn_monsters(objects, field)
@@ -444,14 +477,18 @@
     hours: int = -1
     game_ends = False
     while not game_ends:
         hours += 1
 
         # Starvation check
         player.food -= 1
+        if args.eating_frugal and player.food < FOOD_STARVATION and hours % 2 == 0:
+            player.food += 1
+        elif args.eating_excessive and player.food > FOOD_INIT and hours % 4 == 0:
+            player.food -= 1
         if player.food <= 0:
             message = ">> Starved to Death. <<"
             game_ends = True
             break
 
         # Show the field
         update_torched(torched, player, torch_radius)
@@ -489,14 +526,16 @@
         # Actions & events (combats, state changes, etc)
         for enc_obj_i, enc_obj in enc_obj_infos:
             if isinstance(enc_obj, Treasure):
                 if CHAR_DRAGON in encountered_types:
                     encountered_types.add(CHAR_TREASURE)
                     message = ">> Won the Treasure! <<"
                     game_ends = True
+                    player.item = ITEM_TREASURE
+                    player.item_taken_from = ''
                     break
             elif isinstance(enc_obj, Monster):
                 m = enc_obj
                 encountered_types.add(m.kind.char)
                 player_attack = player_attack_by_level(player)
 
                 if player_attack < m.kind.level:
@@ -565,28 +604,40 @@
             stdscr.clear()
             draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=True)
             draw_status_bar(stdscr, player, hours, message=message or temp_message)
             stdscr.refresh()
 
 
 def main():
+    global rand
+
     parser = argparse.ArgumentParser(
         description="A Rogue-Like game.",
     )
 
     parser.add_argument("--version", action="version", version="%(prog)s " + __version__)
 
     g = parser.add_mutually_exclusive_group()
-    g.add_argument("-l", "--large-torch", action="store_true", help="Large torch.")
-    g.add_argument("-s", "--small-torch", action="store_true", help="Small torch.")
-    g.add_argument("--debug-show-entities", action="store_true", help="Debug option.")
+    g.add_argument("-T", "--large-torch", action="store_true", help="Large torch.")
+    g.add_argument("-t", "--small-torch", action="store_true", help="Small torch.")
+
+    parser.add_argument("--debug-show-entities", action="store_true", help="Debug option.")
+    parser.add_argument("-n", "--narrower-corridors", action="store_true", help="Narrower corridors.")
+    parser.add_argument("-E", '--eating-frugal', action='store_true', help='Decrease rate of consuming food')
+    parser.add_argument("-e", '--eating-excessive', action='store_true', help='Increase rate of consuming food')
+    parser.add_argument("--seed", action='store', type=int, help='Seed value')
 
     args = parser.parse_args()
     args_box.append(args)
 
+    if args.seed is not None:
+        rand = MyRandom(args.seed)
+    else:
+        rand = MyRandom(int(time.time()) % 100000)
+
     curses.initscr()
     curses.noecho()
     curses.cbreak()
     curses.curs_set(0)
 
     curses.start_color()
     curses.use_default_colors()
```

### Comparing `arlq-1.0.6/arlq.egg-info/PKG-INFO` & `arlq-1.2.0/arlq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.6
+Version: 1.2.0
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.6/setup.cfg` & `arlq-1.2.0/setup.cfg`

 * *Files identical despite different names*

