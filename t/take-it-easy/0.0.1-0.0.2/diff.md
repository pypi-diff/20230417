# Comparing `tmp/take_it_easy-0.0.1.tar.gz` & `tmp/take_it_easy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "take_it_easy-0.0.1.tar", last modified: Sun Apr 16 06:40:54 2023, max compression
+gzip compressed data, was "take_it_easy-0.0.2.tar", last modified: Mon Apr 17 13:51:15 2023, max compression
```

## Comparing `take_it_easy-0.0.1.tar` & `take_it_easy-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-04-16 06:40:54.238827 take_it_easy-0.0.1/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-04-16 03:41:50.000000 take_it_easy-0.0.1/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-01-20 02:50:04.000000 take_it_easy-0.0.1/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     2534 2023-04-16 06:40:54.238665 take_it_easy-0.0.1/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1679 2023-04-16 06:33:05.000000 take_it_easy-0.0.1/README.md
--rw-r--r--   0 magnus     (501) staff       (20)     1035 2023-04-16 05:39:54.000000 take_it_easy-0.0.1/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-04-16 06:40:54.238875 take_it_easy-0.0.1/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2560 2023-01-20 02:50:04.000000 take_it_easy-0.0.1/setup.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-04-16 06:40:54.236584 take_it_easy-0.0.1/take_it_easy/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-04-16 06:33:04.000000 take_it_easy-0.0.1/take_it_easy/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     3227 2023-04-16 06:33:09.000000 take_it_easy-0.0.1/take_it_easy/_modidx.py
--rw-r--r--   0 magnus     (501) staff       (20)     3478 2023-04-16 06:33:04.000000 take_it_easy-0.0.1/take_it_easy/board.py
--rw-r--r--   0 magnus     (501) staff       (20)     1660 2023-04-16 06:33:04.000000 take_it_easy-0.0.1/take_it_easy/play.py
--rw-r--r--   0 magnus     (501) staff       (20)     1966 2023-04-16 06:33:04.000000 take_it_easy-0.0.1/take_it_easy/tiles.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-04-16 06:40:54.238405 take_it_easy-0.0.1/take_it_easy.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     2534 2023-04-16 06:40:54.000000 take_it_easy-0.0.1/take_it_easy.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      418 2023-04-16 06:40:54.000000 take_it_easy-0.0.1/take_it_easy.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-04-16 06:40:54.000000 take_it_easy-0.0.1/take_it_easy.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       46 2023-04-16 06:40:54.000000 take_it_easy-0.0.1/take_it_easy.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-04-16 04:44:14.000000 take_it_easy-0.0.1/take_it_easy.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-04-16 06:40:54.000000 take_it_easy-0.0.1/take_it_easy.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)       13 2023-04-16 06:40:54.000000 take_it_easy-0.0.1/take_it_easy.egg-info/top_level.txt
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-04-17 13:51:15.907550 take_it_easy-0.0.2/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-04-16 03:41:50.000000 take_it_easy-0.0.2/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-01-20 02:50:04.000000 take_it_easy-0.0.2/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     2534 2023-04-17 13:51:15.907402 take_it_easy-0.0.2/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1679 2023-04-16 06:33:05.000000 take_it_easy-0.0.2/README.md
+-rw-r--r--   0 magnus     (501) staff       (20)     1063 2023-04-17 13:51:08.000000 take_it_easy-0.0.2/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-04-17 13:51:15.907603 take_it_easy-0.0.2/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2560 2023-01-20 02:50:04.000000 take_it_easy-0.0.2/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-04-17 13:51:15.905579 take_it_easy-0.0.2/take_it_easy/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-04-17 13:44:05.000000 take_it_easy-0.0.2/take_it_easy/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3344 2023-04-17 13:44:05.000000 take_it_easy-0.0.2/take_it_easy/_modidx.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3478 2023-04-17 13:44:05.000000 take_it_easy-0.0.2/take_it_easy/board.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1761 2023-04-17 13:44:05.000000 take_it_easy-0.0.2/take_it_easy/play.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1966 2023-04-17 13:44:05.000000 take_it_easy-0.0.2/take_it_easy/tiles.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-04-17 13:51:15.907143 take_it_easy-0.0.2/take_it_easy.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     2534 2023-04-17 13:51:15.000000 take_it_easy-0.0.2/take_it_easy.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      418 2023-04-17 13:51:15.000000 take_it_easy-0.0.2/take_it_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-04-17 13:51:15.000000 take_it_easy-0.0.2/take_it_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       46 2023-04-17 13:51:15.000000 take_it_easy-0.0.2/take_it_easy.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-04-16 04:44:14.000000 take_it_easy-0.0.2/take_it_easy.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       13 2023-04-17 13:51:15.000000 take_it_easy-0.0.2/take_it_easy.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       13 2023-04-17 13:51:15.000000 take_it_easy-0.0.2/take_it_easy.egg-info/top_level.txt
```

### Comparing `take_it_easy-0.0.1/LICENSE` & `take_it_easy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `take_it_easy-0.0.1/PKG-INFO` & `take_it_easy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: take_it_easy
-Version: 0.0.1
+Version: 0.0.2
 Summary: An implementation of the popular board game Take It Easy! to be used for Reinforcement Learning
 Home-page: https://github.com/majoma7/take_it_easy
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `take_it_easy-0.0.1/README.md` & `take_it_easy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `take_it_easy-0.0.1/settings.ini` & `take_it_easy-0.0.2/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = take_it_easy
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = take_it_easy
@@ -33,12 +33,16 @@
 copyright = 2023 onwards, %(author)s
 description = An implementation of the popular board game Take It Easy! to be used for Reinforcement Learning
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = majoma7
 
+### Conda ###
+conda_user = majoma7
+
+
 ### Optional ###
-requirements = fastcore numpy
+requirements = numpy
 # dev_requirements = 
 # console_scripts =
```

### Comparing `take_it_easy-0.0.1/setup.py` & `take_it_easy-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `take_it_easy-0.0.1/take_it_easy/_modidx.py` & `take_it_easy-0.0.2/take_it_easy/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
                                     'take_it_easy.board.Board.get_score_potential': ( 'board.html#board.get_score_potential',
                                                                                       'take_it_easy/board.py'),
                                     'take_it_easy.board.Board.is_full': ('board.html#board.is_full', 'take_it_easy/board.py'),
                                     'take_it_easy.board.Board.put_tile': ('board.html#board.put_tile', 'take_it_easy/board.py'),
                                     'take_it_easy.board.Board.reset': ('board.html#board.reset', 'take_it_easy/board.py')},
             'take_it_easy.play': { 'take_it_easy.play.Game': ('play.html#game', 'take_it_easy/play.py'),
                                    'take_it_easy.play.Game.__init__': ('play.html#game.__init__', 'take_it_easy/play.py'),
+                                   'take_it_easy.play.Game.reset': ('play.html#game.reset', 'take_it_easy/play.py'),
                                    'take_it_easy.play.Game.step': ('play.html#game.step', 'take_it_easy/play.py'),
                                    'take_it_easy.play.play_random_game': ('play.html#play_random_game', 'take_it_easy/play.py')},
             'take_it_easy.tiles': { 'take_it_easy.tiles.Tiles': ('tiles.html#tiles', 'take_it_easy/tiles.py'),
                                     'take_it_easy.tiles.Tiles.__init__': ('tiles.html#tiles.__init__', 'take_it_easy/tiles.py'),
                                     'take_it_easy.tiles.Tiles.__str__': ('tiles.html#tiles.__str__', 'take_it_easy/tiles.py'),
                                     'take_it_easy.tiles.Tiles.draw_tile': ('tiles.html#tiles.draw_tile', 'take_it_easy/tiles.py'),
                                     'take_it_easy.tiles.Tiles.input_tile': ('tiles.html#tiles.input_tile', 'take_it_easy/tiles.py'),
```

### Comparing `take_it_easy-0.0.1/take_it_easy/board.py` & `take_it_easy-0.0.2/take_it_easy/board.py`

 * *Files identical despite different names*

### Comparing `take_it_easy-0.0.1/take_it_easy/play.py` & `take_it_easy-0.0.2/take_it_easy/play.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,15 +33,19 @@
         score_change = self.board.get_score() - score_beginning
         score_potential_change = self.board.get_score_potential() - score_potential_beginning
 
         if self.board.is_full():
             self.finished = True
 
         return indices, coordinates, score_change, score_potential_change, next_tile
-    
+
+    def reset(self):
+        self.board.reset()
+        self.tiles.reset()
+        self.finished = False
 
 def play_random_game(board, tiles):
     """
     Play the game board.
     """
     game = Game(board, tiles)
     indices, coordinates = game.board.get_potential_moves()
```

### Comparing `take_it_easy-0.0.1/take_it_easy/tiles.py` & `take_it_easy-0.0.2/take_it_easy/tiles.py`

 * *Files identical despite different names*

### Comparing `take_it_easy-0.0.1/take_it_easy.egg-info/PKG-INFO` & `take_it_easy-0.0.2/take_it_easy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: take-it-easy
-Version: 0.0.1
+Version: 0.0.2
 Summary: An implementation of the popular board game Take It Easy! to be used for Reinforcement Learning
 Home-page: https://github.com/majoma7/take_it_easy
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

