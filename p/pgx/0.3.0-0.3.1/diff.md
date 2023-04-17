# Comparing `tmp/pgx-0.3.0.tar.gz` & `tmp/pgx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.3.0.tar", last modified: Sat Apr 15 18:29:16 2023, max compression
+gzip compressed data, was "pgx-0.3.1.tar", last modified: Mon Apr 17 08:49:23 2023, max compression
```

## Comparing `pgx-0.3.0.tar` & `pgx-0.3.1.tar`

### file list

```diff
@@ -1,133 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.267836 pgx-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 18:29:07.000000 pgx-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-15 18:29:16.267836 pgx-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-15 18:29:07.000000 pgx-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.255836 pgx-0.3.0/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.259836 pgx-0.3.0/pgx/_dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.259836 pgx-0.3.0/pgx/_dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.259836 pgx-0.3.0/pgx/_dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/tictactoe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/_flax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_flax/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    43936 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28856 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/tic_tac_toe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.255836 pgx-0.3.0/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-15 18:29:07.000000 pgx-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:29:16.267836 pgx-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-15 18:29:07.000000 pgx-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.267836 pgx-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61039 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.199586 pgx-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:49:10.000000 pgx-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 08:49:23.199586 pgx-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-17 08:49:10.000000 pgx-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.187586 pgx-0.3.1/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.191586 pgx-0.3.1/pgx/_dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.191586 pgx-0.3.1/pgx/_dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.191586 pgx-0.3.1/pgx/_dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/tictactoe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/_flax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_flax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_flax/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_flax/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44105 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28934 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.199586 pgx-0.3.1/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25917 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.187586 pgx-0.3.1/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 08:49:10.000000 pgx-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:49:23.199586 pgx-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-17 08:49:10.000000 pgx-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.199586 pgx-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61258 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.3.0/LICENSE` & `pgx-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/README.md` & `pgx-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -215,11 +215,21 @@
 - [Anakin framework](https://arxiv.org/abs/2104.06272): Highly efficient RL framework that works with JAX-native environments on TPUs
 - [deepmind/mctx](https://github.com/deepmind/mctx): JAX-native MCTS implementations, including AlphaZero and MuZero
 - [deepmind/rlax](https://github.com/deepmind/rlax): JAX-native RL components
 - [google/evojax](https://github.com/google/evojax): Hardware-Accelerated neuroevolution
 - [RobertTLange/evosax](https://github.com/RobertTLange/evosax): JAX-native evolution strategy (ES) implementations
 - [adaptive-intelligent-robotics/QDax](https://github.com/adaptive-intelligent-robotics/QDax): JAX-native Quality-Diversity (QD) algorithms
 
+## Citation
+
+```
+@article{koyamada2023pgx,
+  title={Pgx: Hardware-accelerated parallel game simulation for reinforcement learning},
+  author={Koyamada, Sotetsu and Okano, Shinri and Nishimori, Soichiro and Murata, Yu and Habara, Keigo and Kita, Haruka and Ishii, Shin},
+  journal={arXiv preprint arXiv:2303.17503},
+  year={2023}
+}
+```
 
 ## LICENSE
 
 Apache-2.0
```

#### html2text {}

```diff
@@ -69,8 +69,12 @@
 [deepmind/mctx](https://github.com/deepmind/mctx): JAX-native MCTS
 implementations, including AlphaZero and MuZero - [deepmind/rlax](https://
 github.com/deepmind/rlax): JAX-native RL components - [google/evojax](https://
 github.com/google/evojax): Hardware-Accelerated neuroevolution - [RobertTLange/
 evosax](https://github.com/RobertTLange/evosax): JAX-native evolution strategy
 (ES) implementations - [adaptive-intelligent-robotics/QDax](https://github.com/
 adaptive-intelligent-robotics/QDax): JAX-native Quality-Diversity (QD)
-algorithms ## LICENSE Apache-2.0
+algorithms ## Citation ``` @article{koyamada2023pgx, title={Pgx: Hardware-
+accelerated parallel game simulation for reinforcement learning}, author=
+{Koyamada, Sotetsu and Okano, Shinri and Nishimori, Soichiro and Murata, Yu and
+Habara, Keigo and Kita, Haruka and Ishii, Shin}, journal={arXiv preprint arXiv:
+2303.17503}, year={2023} } ``` ## LICENSE Apache-2.0
```

### Comparing `pgx-0.3.0/pgx/_cache.py` & `pgx-0.3.1/pgx/_cache.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_chess_utils.py` & `pgx-0.3.1/pgx/_chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/animalshogi.py` & `pgx-0.3.1/pgx/_dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/backgammon.py` & `pgx-0.3.1/pgx/_dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/bridge_bidding.py` & `pgx-0.3.1/pgx/_dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/chess.py` & `pgx-0.3.1/pgx/_dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/connect_four.py` & `pgx-0.3.1/pgx/_dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/go.py` & `pgx-0.3.1/pgx/_dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/hex.py` & `pgx-0.3.1/pgx/_dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/LICENSE` & `pgx-0.3.1/pgx/_dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/bBishop.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/bKing.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/bKnight.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/bPawn.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/bQueen.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/bRook.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/wBishop.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/wKing.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/wKnight.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/wPawn.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/wQueen.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/chess/wRook.svg` & `pgx-0.3.1/pgx/_dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/b.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/kuhn_poker.py` & `pgx-0.3.1/pgx/_dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/leduc_holdem.py` & `pgx-0.3.1/pgx/_dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/othello.py` & `pgx-0.3.1/pgx/_dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/play2048.py` & `pgx-0.3.1/pgx/_dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/shogi.py` & `pgx-0.3.1/pgx/_dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/sparrow_mahjong.py` & `pgx-0.3.1/pgx/_dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_dwg/tictactoe.py` & `pgx-0.3.1/pgx/_dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_flax/serialization.py` & `pgx-0.3.1/pgx/_flax/serialization.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_flax/struct.py` & `pgx-0.3.1/pgx/_flax/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_shogi_utils.py` & `pgx-0.3.1/pgx/_shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/_test.py` & `pgx-0.3.1/pgx/_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 from dataclasses import fields
 
 import jax
 import jax.numpy as jnp
 
-from pgx.core import Env, State
+from pgx.core import Env, State, available_games
 from pgx.experimental.utils import act_randomly
 
 act_randomly = jax.jit(act_randomly)
 
 
 def api_test(env: Env, num: int = 100):
     api_test_single(env, num)
@@ -137,14 +137,15 @@
 
     - current_player is int8
     - terminated is bool_
     - reward is float
     - legal_action_mask is bool_
     - TODO: observation is bool_ or int8 (can promote to any other types)
     """
+    assert state.env_id in available_games()
     assert state.current_player.dtype == jnp.int8, state.current_player.dtype
     assert state.terminated.dtype == jnp.bool_, state.terminated.dtype
     assert state.reward.dtype == jnp.float32, state.reward.dtype
     assert (
         state.legal_action_mask.dtype == jnp.bool_
     ), state.legal_action_mask.dtype
```

### Comparing `pgx-0.3.0/pgx/_visualizer.py` & `pgx-0.3.1/pgx/_visualizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,50 +10,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from dataclasses import dataclass
-from typing import Literal, Optional
+from pathlib import Path
+from typing import Literal, Optional, Sequence, Union
 
 import svgwrite  # type: ignore
 
-from ._dwg.animalshogi import AnimalShogiState, _make_animalshogi_dwg
-from ._dwg.backgammon import BackgammonState, _make_backgammon_dwg
-from ._dwg.bridge_bidding import BridgeBiddingState, _make_bridge_dwg
-from ._dwg.chess import ChessState, _make_chess_dwg
-from ._dwg.connect_four import ConnectFourState, _make_connect_four_dwg
-from ._dwg.go import GoState, _make_go_dwg
-from ._dwg.hex import HexState, _make_hex_dwg
-from ._dwg.kuhn_poker import KuhnPokerState, _make_kuhnpoker_dwg
-from ._dwg.leduc_holdem import LeducHoldemState, _make_leducHoldem_dwg
-from ._dwg.othello import OthelloState, _make_othello_dwg
-from ._dwg.play2048 import Play2048State, _make_2048_dwg
-from ._dwg.shogi import ShogiState, _make_shogi_dwg
-from ._dwg.sparrow_mahjong import SparrowMahjongState, _make_sparrowmahjong_dwg
-from ._dwg.tictactoe import TictactoeState, _make_tictactoe_dwg
+from .core import State
 
 ColorTheme = Literal["light", "dark"]
 
 
 @dataclass
 class Config:
     color_theme: ColorTheme = "light"
     scale: float = 1.0
+    frame_duration_seconds: float = 0.2
 
 
 global_config = Config()
 
 
 def set_visualization_config(
-    *, color_theme: ColorTheme = "light", scale: float = 1.0
+    *,
+    color_theme: ColorTheme = "light",
+    scale: float = 1.0,
+    frame_duration_seconds: float = 0.2,
 ):
     global_config.color_theme = color_theme
     global_config.scale = scale
+    global_config.frame_duration_seconds = frame_duration_seconds
 
 
 @dataclass
 class ColorSet:
     p1_color: str = "black"
     p2_color: str = "white"
     p1_outline: str = "black"
@@ -96,22 +89,14 @@
     """
     notebook で可視化する際に、変数名のみで表示させる場合
     def _repr_html_(self) -> str:
         assert self.state is not None
         return self._to_dwg_from_states(states=self.state).tostring()
     """
 
-    def save_svg(
-        self,
-        state,
-        filename="temp.svg",
-    ) -> None:
-        assert filename.endswith(".svg")
-        self.get_dwg(states=state).saveas(filename=filename)
-
     def get_dwg(
         self,
         states,
     ):
         try:
             SIZE = len(states.current_player)
             WIDTH = math.ceil(math.sqrt(SIZE - 0.1))
@@ -195,20 +180,22 @@
                     stroke="gray",
                 )
             )
         group.scale(SCALE)
         dwg.add(group)
         return dwg
 
-    def _set_config_by_state(self, _state):  # noqa: C901
-        if isinstance(_state, AnimalShogiState):
+    def _set_config_by_state(self, _state: State):  # noqa: C901
+        if _state.env_id == "animal_shogi":
+            from ._dwg.animalshogi import _make_animalshogi_dwg
+
             self.config["GRID_SIZE"] = 60
             self.config["BOARD_WIDTH"] = 4
             self.config["BOARD_HEIGHT"] = 4
-            self._make_dwg_group = _make_animalshogi_dwg
+            self._make_dwg_group = _make_animalshogi_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "dimgray",
                     "black",
@@ -224,19 +211,21 @@
                     "lightgray",
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, BackgammonState):
+        elif _state.env_id == "backgammon":
+            from ._dwg.backgammon import _make_backgammon_dwg
+
             self.config["GRID_SIZE"] = 25
             self.config["BOARD_WIDTH"] = 17
             self.config["BOARD_HEIGHT"] = 14
-            self._make_dwg_group = _make_backgammon_dwg
+            self._make_dwg_group = _make_backgammon_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "darkgray",
@@ -252,19 +241,21 @@
                     "black",
                     "lightgray",
                     "white",
                     "white",
                     "black",
                     "gray",
                 )
-        elif isinstance(_state, BridgeBiddingState):
+        elif _state.env_id == "bridge_bidding":
+            from ._dwg.bridge_bidding import _make_bridge_dwg
+
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 14
             self.config["BOARD_HEIGHT"] = 10
-            self._make_dwg_group = _make_bridge_dwg
+            self._make_dwg_group = _make_bridge_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "gray",
                     "black",
@@ -280,19 +271,21 @@
                     "black",
                     "lightgray",
                     "white",
                     "white",
                     "black",
                     "black",
                 )
-        elif isinstance(_state, ChessState):
+        elif _state.env_id == "chess":
+            from ._dwg.chess import _make_chess_dwg
+
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
-            self._make_dwg_group = _make_chess_dwg
+            self._make_dwg_group = _make_chess_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "none",
                     "none",
@@ -308,19 +301,21 @@
                     "none",
                     "gray",
                     "white",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, ConnectFourState):
+        elif _state.env_id == "connect_four":
+            from ._dwg.connect_four import _make_connect_four_dwg
+
             self.config["GRID_SIZE"] = 35
             self.config["BOARD_WIDTH"] = 7
             self.config["BOARD_HEIGHT"] = 7
-            self._make_dwg_group = _make_connect_four_dwg
+            self._make_dwg_group = _make_connect_four_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "darkgray",
@@ -336,23 +331,27 @@
                     "white",
                     "black",
                     "black",
                     "white",
                     "black",
                     "gray",
                 )
-        elif isinstance(_state, GoState):
+        elif _state.env_id in ("go-9x9", "go-19x19"):
+            from ._dwg.go import _make_go_dwg
+
             self.config["GRID_SIZE"] = 25
             try:
-                self.config["BOARD_WIDTH"] = int(_state.size[0])
-                self.config["BOARD_HEIGHT"] = int(_state.size[0])
+                self.config["BOARD_WIDTH"] = int(_state.size[0])  # type:ignore
+                self.config["BOARD_HEIGHT"] = int(
+                    _state.size[0]  # type:ignore
+                )
             except IndexError:
-                self.config["BOARD_WIDTH"] = int(_state.size)
-                self.config["BOARD_HEIGHT"] = int(_state.size)
-            self._make_dwg_group = _make_go_dwg
+                self.config["BOARD_WIDTH"] = int(_state.size)  # type:ignore
+                self.config["BOARD_HEIGHT"] = int(_state.size)  # type:ignore
+            self._make_dwg_group = _make_go_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "darkgray",
@@ -368,31 +367,35 @@
                     "white",
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, HexState):
+        elif _state.env_id == "hex":
             import jax.numpy as jnp
 
-            from pgx._dwg.hex import four_dig
+            from ._dwg.hex import _make_hex_dwg, four_dig
 
             self.config["GRID_SIZE"] = 30
             try:
-                self.config["BOARD_WIDTH"] = four_dig(_state.size[0] * 1.5)
+                self.config["BOARD_WIDTH"] = four_dig(
+                    _state.size[0] * 1.5  # type:ignore
+                )
                 self.config["BOARD_HEIGHT"] = four_dig(
-                    _state.size[0] * jnp.sqrt(3) / 2
+                    _state.size[0] * jnp.sqrt(3) / 2  # type:ignore
                 )
             except IndexError:
-                self.config["BOARD_WIDTH"] = four_dig(_state.size * 1.5)
+                self.config["BOARD_WIDTH"] = four_dig(
+                    _state.size * 1.5  # type:ignore
+                )
                 self.config["BOARD_HEIGHT"] = four_dig(
-                    _state.size * jnp.sqrt(3) / 2
+                    _state.size * jnp.sqrt(3) / 2  # type:ignore
                 )
-            self._make_dwg_group = _make_hex_dwg
+            self._make_dwg_group = _make_hex_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "darkgray",
@@ -408,19 +411,21 @@
                     "white",
                     "black",
                     "black",
                     "white",
                     "black",
                     "lightgray",
                 )
-        elif isinstance(_state, KuhnPokerState):
+        elif _state.env_id == "kuhn_poker":
+            from ._dwg.kuhn_poker import _make_kuhnpoker_dwg
+
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
-            self._make_dwg_group = _make_kuhnpoker_dwg
+            self._make_dwg_group = _make_kuhnpoker_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "lightgray",
@@ -436,19 +441,21 @@
                     "white",
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, LeducHoldemState):
+        elif _state.env_id == "leduc_holdem":
+            from ._dwg.leduc_holdem import _make_leducHoldem_dwg
+
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
-            self._make_dwg_group = _make_leducHoldem_dwg
+            self._make_dwg_group = _make_leducHoldem_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "gray",
                     "lightgray",
@@ -464,19 +471,21 @@
                     "black",
                     "",
                     "",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, OthelloState):
+        elif _state.env_id == "othello":
+            from ._dwg.othello import _make_othello_dwg
+
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
-            self._make_dwg_group = _make_othello_dwg
+            self._make_dwg_group = _make_othello_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "darkgray",
@@ -492,19 +501,21 @@
                     "white",
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, Play2048State):
+        elif _state.env_id == "2048":
+            from ._dwg.play2048 import _make_2048_dwg
+
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 4
             self.config["BOARD_HEIGHT"] = 4
-            self._make_dwg_group = _make_2048_dwg
+            self._make_dwg_group = _make_2048_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "lightgray",
                     "",
@@ -520,19 +531,21 @@
                     "#f0f0f0",
                     "",
                     "",
                     "white",
                     "black",
                     "black",
                 )
-        elif isinstance(_state, ShogiState):
+        elif _state.env_id == "shogi":
+            from ._dwg.shogi import _make_shogi_dwg
+
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 10
             self.config["BOARD_HEIGHT"] = 9
-            self._make_dwg_group = _make_shogi_dwg
+            self._make_dwg_group = _make_shogi_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "gray", "black", "gray", "gray", "#1e1e1e", "gray", ""
                 )
@@ -542,19 +555,21 @@
                     "lightgray",
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
-        elif isinstance(_state, SparrowMahjongState):
+        elif _state.env_id == "sparrow_mahjong":
+            from ._dwg.sparrow_mahjong import _make_sparrowmahjong_dwg
+
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 15
             self.config["BOARD_HEIGHT"] = 10
-            self._make_dwg_group = _make_sparrowmahjong_dwg
+            self._make_dwg_group = _make_sparrowmahjong_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "lightgray",
                     "dimgray",
@@ -570,19 +585,21 @@
                     "white",
                     "gray",
                     "white",
                     "white",
                     "silver",
                     "black",
                 )
-        elif isinstance(_state, TictactoeState):
+        elif _state.env_id == "tic_tac_toe":
+            from ._dwg.tictactoe import _make_tictactoe_dwg
+
             self.config["GRID_SIZE"] = 60
             self.config["BOARD_WIDTH"] = 3
             self.config["BOARD_HEIGHT"] = 3
-            self._make_dwg_group = _make_tictactoe_dwg
+            self._make_dwg_group = _make_tictactoe_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "gray",
                     "black",
@@ -594,97 +611,189 @@
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "white", "black", "lightgray", "white", "white", "black"
                 )
         else:
             assert False
 
-    def _get_nth_state(self, _states, _i):
-        if isinstance(_states, AnimalShogiState):
+    # TODO: simplify me
+    def _get_nth_state(self, _states: State, _i):
+        if _states.env_id == "animal_shogi":
+            from ._dwg.animalshogi import AnimalShogiState
+
             return AnimalShogiState(
                 turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],
-                hand=_states.hand[_i],
+                board=_states.board[_i],  # type:ignore
+                hand=_states.hand[_i],  # type:ignore
             )
-        elif isinstance(_states, BackgammonState):
+        elif _states.env_id == "backgammon":
+            from ._dwg.backgammon import BackgammonState
+
             return BackgammonState(
                 turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],
+                board=_states.board[_i],  # type:ignore
             )
-        elif isinstance(_states, ConnectFourState):
+        elif _states.env_id == "connect_four":
+            from ._dwg.connect_four import ConnectFourState
+
             return ConnectFourState(  # type:ignore
-                turn=_states.turn[_i],
-                board=_states.board[_i],
+                turn=_states.turn[_i],  # type:ignore
+                board=_states.board[_i],  # type:ignore
             )
-        elif isinstance(_states, ChessState):
+        elif _states.env_id == "chess":
+            from ._dwg.chess import ChessState
+
             return ChessState(
                 turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],
+                board=_states.board[_i],  # type:ignore
             )
-        elif isinstance(_states, BridgeBiddingState):
+        elif _states.env_id == "bridge_bidding":
+            from ._dwg.bridge_bidding import BridgeBiddingState
+
             return BridgeBiddingState(  # type:ignore
-                turn=_states.turn[_i],
-                dealer=_states.dealer[_i],
-                current_player=_states.current_player[_i],
-                hand=_states.hand[_i],
-                bidding_history=_states.bidding_history[_i],
-                vul_NS=_states.vul_NS[_i],
-                vul_EW=_states.vul_EW[_i],
+                turn=_states.turn[_i],  # type:ignore
+                dealer=_states.dealer[_i],  # type:ignore
+                current_player=_states.current_player[_i],  # type:ignore
+                hand=_states.hand[_i],  # type:ignore
+                bidding_history=_states.bidding_history[_i],  # type:ignore
+                vul_NS=_states.vul_NS[_i],  # type:ignore
+                vul_EW=_states.vul_EW[_i],  # type:ignore
             )
-        elif isinstance(_states, GoState):
+        elif _states.env_id in ("go-9x9", "go-19x19"):
+            from ._dwg.go import GoState
+
             return GoState(  # type:ignore
-                size=_states.size[_i],
-                chain_id_board=_states.chain_id_board[_i],
-                turn=_states.turn[_i],
+                size=_states.size[_i],  # type:ignore
+                chain_id_board=_states.chain_id_board[_i],  # type:ignore
+                turn=_states.turn[_i],  # type:ignore
             )
-        elif isinstance(_states, HexState):
+        elif _states.env_id == "hex":
+            from ._dwg.hex import HexState
+
             return HexState(
-                size=_states.size[_i],
-                turn=_states.turn[_i],
-                board=_states.board[_i],
-            )
-        elif isinstance(_states, KuhnPokerState):
-            return KuhnPokerState(cards=_states.cards[_i], pot=_states.pot[_i])
-        elif isinstance(_states, LeducHoldemState):
+                size=_states.size[_i],  # type:ignore
+                turn=_states.turn[_i],  # type:ignore
+                board=_states.board[_i],  # type:ignore
+            )
+        elif _states.env_id == "kuhn_poker":
+            from ._dwg.kuhn_poker import KuhnPokerState
+
+            return KuhnPokerState(
+                cards=_states.cards[_i], pot=_states.pot[_i]  # type:ignore
+            )
+        elif _states.env_id == "leduc_holdem":
+            from ._dwg.leduc_holdem import LeducHoldemState
+
             return LeducHoldemState(
-                cards=_states.cards[_i],
-                chips=_states.chips[_i],
-                round=_states.round[_i],
+                cards=_states.cards[_i],  # type:ignore
+                chips=_states.chips[_i],  # type:ignore
+                round=_states.round[_i],  # type:ignore
             )
-        elif isinstance(_states, OthelloState):
+        elif _states.env_id == "othello":
+            from ._dwg.othello import OthelloState
+
             return OthelloState(
-                turn=_states.turn[_i],
-                board=_states.board[_i],
+                turn=_states.turn[_i],  # type:ignore
+                board=_states.board[_i],  # type:ignore
             )
-        elif isinstance(_states, Play2048State):
+        elif _states.env_id == "2048":
+            from ._dwg.play2048 import Play2048State
+
             return Play2048State(
-                board=_states.board[_i],
+                board=_states.board[_i],  # type:ignore
             )
-        elif isinstance(_states, ShogiState):
+        elif _states.env_id == "shogi":
+            from ._dwg.shogi import ShogiState
+
             return ShogiState(  # type:ignore
-                turn=_states.turn[_i],
-                piece_board=_states.piece_board[_i],
-                hand=_states.hand[_i],
+                turn=_states.turn[_i],  # type:ignore
+                piece_board=_states.piece_board[_i],  # type:ignore
+                hand=_states.hand[_i],  # type:ignore
             )
-        elif isinstance(_states, SparrowMahjongState):
+        elif _states.env_id == "sparrow_mahjong":
+            from ._dwg.sparrow_mahjong import SparrowMahjongState
+
             return SparrowMahjongState(
-                current_player=_states.current_player[_i],
-                turn=_states.turn[_i],
-                rivers=_states.rivers[_i],
-                hands=_states.hands[_i],
-                n_red_in_hands=_states.n_red_in_hands[_i],
-                is_red_in_river=_states.is_red_in_river[_i],
-                wall=_states.wall[_i],
-                draw_ix=_states.draw_ix[_i],
-                shuffled_players=_states.shuffled_players[_i],
-                dora=_states.dora[_i],
+                current_player=_states.current_player[_i],  # type:ignore
+                turn=_states.turn[_i],  # type:ignore
+                rivers=_states.rivers[_i],  # type:ignore
+                hands=_states.hands[_i],  # type:ignore
+                n_red_in_hands=_states.n_red_in_hands[_i],  # type:ignore
+                is_red_in_river=_states.is_red_in_river[_i],  # type:ignore
+                wall=_states.wall[_i],  # type:ignore
+                draw_ix=_states.draw_ix[_i],  # type:ignore
+                shuffled_players=_states.shuffled_players[_i],  # type:ignore
+                dora=_states.dora[_i],  # type:ignore
             )
-        elif isinstance(_states, TictactoeState):
+        elif _states.env_id == "tic_tac_toe":
+            from ._dwg.tictactoe import TictactoeState
+
             return TictactoeState(
-                current_player=_states.current_player[_i],
-                legal_action_mask=_states.legal_action_mask[_i],
-                terminated=_states.terminated[_i],
-                turn=_states.turn[_i],
-                board=_states.board[_i],
+                current_player=_states.current_player[_i],  # type:ignore
+                legal_action_mask=_states.legal_action_mask[_i],  # type:ignore
+                terminated=_states.terminated[_i],  # type:ignore
+                turn=_states.turn[_i],  # type:ignore
+                board=_states.board[_i],  # type:ignore
             )
         else:
             assert False
+
+
+def save_svg(
+    states: State,
+    filename: Union[str, Path],
+    *,
+    color_theme: Optional[Literal["light", "dark"]] = None,
+    scale: Optional[float] = None,
+) -> None:
+    assert str(filename).endswith(".svg")
+    v = Visualizer(color_theme=color_theme, scale=scale)
+    v.get_dwg(states=states).saveas(filename)
+
+
+def save_svg_animation(
+    states: Sequence[State],
+    filename: Union[str, Path],
+    *,
+    color_theme: Optional[Literal["light", "dark"]] = None,
+    scale: Optional[float] = None,
+    frame_duration_seconds: Optional[float] = None,
+) -> None:
+    assert str(filename).endswith(".svg")
+    v = Visualizer(color_theme=color_theme, scale=scale)
+
+    if frame_duration_seconds is None:
+        frame_duration_seconds = global_config.frame_duration_seconds
+
+    frame_groups = []
+    dwg = None
+    for i, state in enumerate(states):
+        dwg = v.get_dwg(states=state)
+        assert (
+            len(
+                [
+                    e
+                    for e in dwg.elements
+                    if type(e) == svgwrite.container.Group
+                ]
+            )
+            == 1
+        ), "Drawing must contain only one group"
+        group: svgwrite.container.Group = dwg.elements[-1]
+        group["id"] = f"_fr{i:x}"  # hex frame number
+        group["class"] = "frame"
+        frame_groups.append(group)
+
+    assert dwg is not None
+    del dwg.elements[-1]
+    total_seconds = frame_duration_seconds * len(frame_groups)
+
+    style = f".frame{{visibility:hidden; animation:{total_seconds}s linear _k infinite;}}"
+    style += f"@keyframes _k{{0%,{100/len(frame_groups)}%{{visibility:visible}}{100/len(frame_groups) * 1.000001}%,100%{{visibility:hidden}}}}"
+
+    for i, group in enumerate(frame_groups):
+        dwg.add(group)
+        style += (
+            f"#{group['id']}{{animation-delay:{i * frame_duration_seconds}s}}"
+        )
+    dwg.defs.add(svgwrite.container.Style(content=style))
+    dwg.saveas(filename)
```

### Comparing `pgx-0.3.0/pgx/animal_shogi.py` & `pgx-0.3.1/pgx/animal_shogi.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,18 @@
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Animal Shogi specific ---
     turn: jnp.ndarray = jnp.int8(0)
     board: jnp.ndarray = INIT_BOARD  # (12,)
     hand: jnp.ndarray = jnp.zeros((2, 3), dtype=jnp.int8)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "animal_shogi"
+
 
 @dataclass
 class Action:
     is_drop: jnp.ndarray = FALSE
     from_: jnp.ndarray = jnp.int8(-1)
     to: jnp.ndarray = jnp.int8(-1)
     drop_piece: jnp.ndarray = jnp.int8(-1)
```

### Comparing `pgx-0.3.0/pgx/backgammon.py` & `pgx-0.3.1/pgx/backgammon.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     # プレイできるサイコロの目
     playable_dice: jnp.ndarray = jnp.zeros(4, dtype=jnp.int16)
     # プレイしたサイコロの目の数
     played_dice_num: jnp.ndarray = jnp.int16(0)
     # 黒0, 白1
     turn: jnp.ndarray = jnp.int8(1)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "backgammon"
+
 
 class Backgammon(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/bridge_bidding.py` & `pgx-0.3.1/pgx/bridge_bidding.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     first_denomination_NS: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
     # first_denominaton_EW EWチームにおいて、各denominationをどのプレイヤー
     # が最初にbidしたかを表す
     first_denomination_EW: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
     # passの回数
     pass_num: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "bridge_bidding"
+
 
 class BridgeBidding(core.Env):
     def __init__(self):
         super().__init__()
         # fmt: off
         self.hash_keys, self.hash_values = jnp.array([[19556549, 61212362, 52381660, 50424958], [53254536, 21854346, 37287883, 14009558], [44178585, 6709002, 23279217, 16304124], [36635659, 48114215, 13583653, 26208086], [44309474, 39388022, 28376136, 59735189], [61391908, 52173479, 29276467, 31670621], [34786519, 13802254, 57433417, 43152306], [48319039, 55845612, 44614774, 58169152], [47062227, 32289487, 12941848, 21338650], [36579116, 15643926, 64729756, 18678099], [62136384, 37064817, 59701038, 39188202], [13417016, 56577539, 25995845, 27248037], [61125047, 43238281, 23465183, 20030494], [7139188, 31324229, 58855042, 14296487], [2653767, 47502150, 35507905, 43823846], [31453323, 11605145, 6716808, 41061859], [21294711, 49709, 26110952, 50058629], [48130172, 3340423, 60445890, 7686579], [16041939, 27817393, 37167847, 9605779], [61154057, 17937858, 12254613, 12568801], [13796245, 46546127, 49123920, 51772041], [7195005, 45581051, 41076865, 17429796], [20635965, 14642724, 7001617, 45370595], [35616421, 19938131, 45131030, 16524847], [14559399, 15413729, 39188470, 535365], [48743216, 39672069, 60203571, 60210880], [63862780, 2462075, 23267370, 36595020], [11229980, 11616119, 20292263, 3695004], [24135854, 37532826, 54421444, 14130249], [42798085, 33026223, 2460251, 18566823], [49558558, 65537599, 14768519, 31103243], [44321156, 20075251, 42663767, 11615602], [20186726, 42678073, 11763300, 56739471], [57534601, 16703645, 6039937, 17088125], [50795278, 17350238, 11955835, 21538127], [45919621, 5520088, 27736513, 52674927], [13928720, 57324148, 28222453, 15480785], [910719, 47238830, 26345802, 56166394], [58841430, 1098476, 61890558, 26907706], [10379825, 8624220, 39701822, 29045990], [54444873, 50000486, 48563308, 55867521], [47291672, 22084522, 45484828, 32878832], [55350706, 23903891, 46142039, 11499952], [4708326, 27588734, 31010458, 11730972], [27078872, 59038086, 62842566, 51147874], [28922172, 32377861, 9109075, 10154350], [26104086, 62786977, 224865, 14335943], [20448626, 33187645, 34338784, 26382893], [29194006, 19635744, 24917755, 8532577], [64047742, 34885257, 5027048, 58399668], [27603972, 26820121, 44837703, 63748595], [60038456, 19611050, 7928914, 38555047], [13583610, 19626473, 22239272, 19888268], [28521006, 1743692, 31319264, 15168920], [64585849, 63931241, 57019799, 14189800], [2632453, 7269809, 60404342, 57986125], [1996183, 49918209, 49490468, 47760867], [6233580, 15318425, 51356120, 55074857], [15769884, 61654638, 8374039, 43685186], [44162419, 47272176, 62693156, 35359329], [36345796, 15667465, 53341561, 2978505], [1664472, 12761950, 34145519, 55197543], [37567005, 3228834, 6198166, 15646487], [63233399, 42640049, 12969011, 41620641], [22090925, 3386355, 56655568, 31631004], [16442787, 9420273, 48595545, 29770176], [49404288, 37823218, 58551818, 6772527], [36575583, 53847347, 32379432, 1630009], [9004247, 12999580, 48379959, 14252211], [25850203, 26136823, 64934025, 29362603], [10214276, 43557352, 33387586, 55512773], [45810841, 49561478, 41130845, 27034816], [34460081, 16560450, 57722793, 41007718], [53414778, 6845803, 15340368, 16647575], [30535873, 5193469, 43608154, 11391114], [20622004, 34424126, 31475211, 29619615], [10428836, 49656416, 7912677, 33427787], [57600861, 18251799, 46147432, 58946294], [6760779, 14675737, 42952146, 5480498], [46037552, 39969058, 30103468, 55330772], [64466305, 29376674, 49914839, 55269895], [36494113, 27010567, 65752150, 12395385], [49385632, 19550767, 39809394, 58806235], [20987521, 37444597, 49290126, 42326125], [37150229, 37487849, 28254397, 32949826], [9724895, 53813417, 19431235, 27438556], [42132748, 47073733, 19396568, 10026137], [3961481, 27204521, 62087205, 37602005], [22178323, 17505521, 42006207, 44143605], [12753258, 63063515, 61993175, 8920985], [10998000, 64833190, 6446892, 63676805], [66983817, 63684932, 18378359, 39946382], [63476803, 60000436, 19442420, 66417845], [38004446, 64752157, 42570179, 52844512], [1270809, 23735482, 17543294, 18795903], [4862706, 16352249, 57100612, 6219870], [63203206, 25630930, 35608240, 51357885], [59819625, 64662579, 50925335, 55670434], [29216830, 26446697, 52243336, 58475666], [43138915, 30592834, 43931516, 50628002]], dtype=jnp.int32), jnp.array([[71233, 771721, 71505, 706185], [289177, 484147, 358809, 484147], [359355, 549137, 359096, 549137], [350631, 558133, 350630, 554037], [370087, 538677, 370087, 538677], [4432, 899725, 4432, 904077], [678487, 229987, 678487, 229987], [423799, 480614, 423799, 480870], [549958, 284804, 549958, 280708], [423848, 480565, 423848, 480549], [489129, 283940, 554921, 283940], [86641, 822120, 86641, 822120], [206370, 702394, 206370, 567209], [500533, 407959, 500533, 407959], [759723, 79137, 759723, 79137], [563305, 345460, 559209, 345460], [231733, 611478, 231733, 611478], [502682, 406082, 498585, 406082], [554567, 288662, 554567, 288662], [476823, 427846, 476823, 427846], [488823, 415846, 488823, 415846], [431687, 477078, 431687, 477078], [419159, 424070, 415062, 424070], [493399, 345734, 493143, 345718], [678295, 230451, 678295, 230451], [496520, 342596, 496520, 346709], [567109, 276116, 567109, 276116], [624005, 284758, 624005, 284758], [420249, 484420, 420248, 484420], [217715, 621418, 217715, 621418], [344884, 493977, 344884, 493977], [550841, 292132, 550841, 292132], [284262, 558967, 284006, 558967], [152146, 756616, 152146, 756616], [144466, 698763, 144466, 694667], [284261, 624504, 284261, 624504], [288406, 620102, 288405, 620358], [301366, 607383, 301366, 607382], [468771, 435882, 468771, 435882], [555688, 283444, 555688, 283444], [485497, 414820, 485497, 414820], [633754, 275010, 633754, 275010], [419141, 489608, 419157, 489608], [694121, 214387, 694121, 214387], [480869, 427639, 481125, 427639], [489317, 419447, 489301, 419447], [152900, 747672, 152900, 747672], [348516, 494457, 348516, 494457], [534562, 370088, 534562, 370088], [371272, 537475, 371274, 537475], [144194, 760473, 144194, 760473], [567962, 275011, 567962, 275011], [493161, 350052, 493161, 350052], [490138, 348979, 490138, 348979], [328450, 506552, 328450, 506552], [148882, 759593, 148626, 755497], [642171, 266593, 642171, 266593], [685894, 218774, 685894, 218774], [674182, 234548, 674214, 234548], [756347, 152146, 690811, 86353], [612758, 291894, 612758, 291894], [296550, 612214, 296550, 612214], [363130, 475730, 363130, 475730], [691559, 16496, 691559, 16496], [340755, 502202, 336659, 502218], [632473, 210499, 628377, 210483], [564410, 266513, 564410, 266513], [427366, 481399, 427366, 481399], [493159, 349797, 493159, 415605], [331793, 576972, 331793, 576972], [416681, 492084, 416681, 492084], [813496, 95265, 813496, 91153], [695194, 213571, 695194, 213571], [436105, 407124, 436105, 407124], [836970, 6243, 902506, 6243], [160882, 747882, 160882, 747882], [493977, 414788, 489624, 414788], [29184, 551096, 29184, 616888], [903629, 4880, 899517, 4880], [351419, 553250, 351419, 553250], [75554, 767671, 75554, 767671], [279909, 563304, 279909, 563304], [215174, 628054, 215174, 628054], [361365, 481864, 361365, 481864], [424022, 484743, 358486, 484725], [271650, 633018, 271650, 633018], [681896, 226867, 616088, 226867], [222580, 686184, 222564, 686184], [144451, 698778, 209987, 698778], [532883, 310086, 532883, 310086], [628872, 279893, 628872, 279893], [533797, 374951, 533797, 374951], [91713, 817036, 91713, 817036], [427605, 477046, 431718, 477046], [145490, 689529, 145490, 689529], [551098, 291875, 551098, 291875], [349781, 558984, 349781, 558983], [205378, 703115, 205378, 703115], [362053, 546456, 362053, 546456], [612248, 226371, 678040, 226371]], dtype=jnp.int32)
         # fmt: on
@@ -118,14 +122,18 @@
     def version(self) -> str:
         return "alpha"
 
     @property
     def num_players(self) -> int:
         return 4
 
+    @property
+    def _illegal_action_penalty(self) -> float:
+        return -7600.0
+
 
 @jax.jit
 def init(rng: jax.random.KeyArray) -> State:
     rng1, rng2, rng3, rng4, rng5, rng6 = jax.random.split(rng, num=6)
     hand = jnp.arange(0, 52)
     hand = jax.random.permutation(rng2, hand)
     vul_NS = jax.random.randint(rng3, (1,), 0, 2)[0]
@@ -198,15 +206,15 @@
     team_b_players = jax.random.permutation(
         rng3, jnp.arange(2, 4, dtype=jnp.int8)
     )
     # decide which team is on
     # Randomly determine NSteam and EWteam
     # Arrange in order of NESW
     return jax.lax.cond(
-        jax.random.randint(rng4, (1,), 1, 2)[0] == 1,
+        jax.random.randint(rng4, (1,), 0, 2)[0] == 1,
         lambda: jnp.array(
             [
                 team_a_players[0],
                 team_b_players[0],
                 team_a_players[1],
                 team_b_players[1],
             ]
```

### Comparing `pgx-0.3.0/pgx/chess.py` & `pgx-0.3.1/pgx/chess.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,18 @@
         jnp.zeros((1001, 2), dtype=jnp.uint32)
         .at[0]
         .set(jnp.uint32([1429435994, 901419182]))
     )
     # index to possible piece positions for speeding up. Flips every turn.
     possible_piece_positions: jnp.ndarray = INIT_POSSIBLE_PIECE_POSITIONS
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "chess"
+
     @staticmethod
     def _from_fen(fen: str):
         return _from_fen(fen)
 
     def _to_fen(self) -> str:
         return _to_fen(self)
```

### Comparing `pgx-0.3.0/pgx/connect_four.py` & `pgx-0.3.1/pgx/connect_four.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     #  [14, 15, 16, 17, 18, 19, 20],
     #  [21, 22, 23, 24, 25, 26, 27],
     #  [28, 29, 30, 31, 32, 33, 34],
     #  [35, 36, 37, 38, 39, 40, 41]]
     board: jnp.ndarray = -jnp.ones(42, jnp.int8)  # -1 (empty), 0, 1
     blank_row: jnp.ndarray = jnp.full(7, 5)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "connect_four"
+
 
 class ConnectFour(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/core.py` & `pgx-0.3.1/pgx/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,28 +54,33 @@
     "shogi",
     "sparrow_mahjong",
     "tic_tac_toe",
 ]
 
 
 @dataclass
-class State:
+class State(abc.ABC):
     current_player: jnp.ndarray
     observation: jnp.ndarray
     reward: jnp.ndarray
     terminated: jnp.ndarray
     truncated: jnp.ndarray  # so far, not used as all Pgx environments are finite horizon
     legal_action_mask: jnp.ndarray
     # NOTE: _rng_key is
     #   - used for stochastic env and auto reset
     #   - updated only when actually used
     #   - supposed NOT to be used by agent
     _rng_key: jax.random.KeyArray
     _step_count: jnp.ndarray
 
+    @property
+    @abc.abstractmethod
+    def env_id(self) -> EnvId:
+        ...
+
     def _repr_html_(self) -> str:
         from pgx._visualizer import Visualizer
 
         v = Visualizer()
         return v.get_dwg(states=self).tostring()
 
     def save_svg(
@@ -85,18 +90,17 @@
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
         """
         color_theme: Default(None) is "light"
         scale: change image size. Default(None) is 1.0
         """
-        from pgx._visualizer import Visualizer
+        from pgx._visualizer import save_svg
 
-        v = Visualizer(color_theme=color_theme, scale=scale)
-        return v.save_svg(self, filename)
+        save_svg(self, filename, color_theme=color_theme, scale=scale)
 
 
 class Env(abc.ABC):
     def __init__(self):
         ...
 
     def init(self, key: jax.random.KeyArray) -> State:
```

### Comparing `pgx-0.3.0/pgx/experimental/gym.py` & `pgx-0.3.1/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/experimental/pettingzoo.py` & `pgx-0.3.1/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/experimental/visualize.py` & `pgx-0.3.1/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/experimental/wrappers.py` & `pgx-0.3.1/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/go.py` & `pgx-0.3.1/pgx/go.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         2, dtype=jnp.int32
     )  # [0]=black, [1]=white
     passed: jnp.ndarray = FALSE  # TRUE if last action is pass
     ko: jnp.ndarray = jnp.int32(-1)  # by SSK
     komi: jnp.ndarray = jnp.float32(7.5)
     black_player: jnp.ndarray = jnp.int8(0)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        try:
+            size = int(self.size.item())
+        except TypeError:
+            size = int(self.size[0].item())
+        return f"go-{size}x{size}"  # type: ignore
+
 
 class Go(core.Env):
     def __init__(
         self,
         *,
         size: int = 19,
         komi: float = 7.5,
```

### Comparing `pgx-0.3.0/pgx/hex.py` & `pgx-0.3.1/pgx/hex.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     #  .
     #  .
     #  [110, 111, 112, ...,  119, 120]]
     board: jnp.ndarray = -jnp.zeros(
         11 * 11, jnp.int32
     )  # <0(oppo), 0(empty), 0<(self)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "hex"
+
 
 class Hex(core.Env):
     def __init__(
         self,
         *,
         size: int = 11,
     ):
```

### Comparing `pgx-0.3.0/pgx/kuhn_poker.py` & `pgx-0.3.1/pgx/kuhn_poker.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     # --- Kuhn poker specific ---
     cards: jnp.ndarray = jnp.int8([-1, -1])
     # [(player 0),(player 1)]
     last_action: jnp.ndarray = jnp.int8(-1)
     # 0(Call)  1(Bet)  2(Fold)  3(Check)
     pot: jnp.ndarray = jnp.int8([0, 0])
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "kuhn_poker"
+
 
 class KuhnPoker(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/leduc_holdem.py` & `pgx-0.3.1/pgx/leduc_holdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
     # 0(Call)  1(Bet)  2(Fold)  3(Check)
     last_action: jnp.ndarray = INVALID_ACTION
 
     chips: jnp.ndarray = jnp.ones(2, dtype=jnp.int8)
     round: jnp.ndarray = jnp.int8(0)
     raise_count: jnp.ndarray = jnp.int8(0)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "leduc_holdem"
+
 
 class LeducHoldem(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/minatar/asterix.py` & `pgx-0.3.1/pgx/minatar/asterix.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     move_speed: jnp.ndarray = init_move_interval
     move_timer: jnp.ndarray = init_move_interval
     ramp_timer: jnp.ndarray = ramp_interval
     ramp_index: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
     terminal: jnp.ndarray = FALSE  # duplicated but necessary for checking the consistency to the original MinAtar
     last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "minatar/asterix"
+
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
```

### Comparing `pgx-0.3.0/pgx/minatar/breakout.py` & `pgx-0.3.1/pgx/minatar/breakout.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     )
     strike: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
     last_x: jnp.ndarray = ZERO
     last_y: jnp.ndarray = THREE
     terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
     last_action: jnp.ndarray = ZERO
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "minatar/breakout"
+
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
```

### Comparing `pgx-0.3.0/pgx/minatar/freeway.py` & `pgx-0.3.1/pgx/minatar/freeway.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     cars: jnp.ndarray = jnp.zeros((8, 4), dtype=jnp.int32)
     pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
     move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
     terminate_timer: jnp.ndarray = jnp.array(time_limit, dtype=jnp.int32)
     terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
     last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "minatar/freeway"
+
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
```

### Comparing `pgx-0.3.0/pgx/minatar/seaquest.py` & `pgx-0.3.1/pgx/minatar/seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,18 @@
     move_speed: jnp.ndarray = INIT_MOVE_INTERVAL
     ramp_index: jnp.ndarray = ZERO
     shot_timer: jnp.ndarray = ZERO
     surface: jnp.ndarray = TRUE
     terminal: jnp.ndarray = FALSE
     last_action: jnp.ndarray = ZERO
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "minatar/seaquest"
+
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
```

### Comparing `pgx-0.3.0/pgx/minatar/space_invaders.py` & `pgx-0.3.1/pgx/minatar/space_invaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     alien_move_timer: jnp.ndarray = ENEMY_MOVE_INTERVAL
     alien_shot_timer: jnp.ndarray = ENEMY_SHOT_INTERVAL
     ramp_index: jnp.ndarray = jnp.int32(0)
     shot_timer: jnp.ndarray = jnp.int32(0)
     terminal: jnp.ndarray = FALSE
     last_action: jnp.ndarray = jnp.int32(0)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "minatar/space_invaders"
+
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
```

### Comparing `pgx-0.3.0/pgx/minatar/utils.py` & `pgx-0.3.1/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/pgx/othello.py` & `pgx-0.3.1/pgx/othello.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     #  [32, 33, 34, 35, 36, 37, 38, 39],
     #  [40, 41, 42, 43, 44, 45, 46, 47],
     #  [48, 49, 50, 51, 52, 53, 54, 55],
     #  [56, 57, 58, 59, 60, 61, 62, 63]]
     board: jnp.ndarray = jnp.zeros(64, jnp.int8)  # -1(opp), 0(empty), 1(self)
     passed: jnp.ndarray = FALSE
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "othello"
+
 
 class Othello(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/play2048.py` & `pgx-0.3.1/pgx/play2048.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     #  [ 3,  6,  7,  9]]
     # means
     # [[ 0,  0,  2,  2],
     #  [ 2,  0,  2,  4],
     #  [ 8,  8, 64,128],
     #  [ 8, 64,128,512]]
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "2048"
+
 
 class Play2048(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/shogi.py` & `pgx-0.3.1/pgx/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     piece_board: jnp.ndarray = INIT_PIECE_BOARD  # (81,) 後手のときにはflipする
     hand: jnp.ndarray = jnp.zeros((2, 7), dtype=jnp.int8)  # 後手のときにはflipする
     # cache
     # Redundant information used only in _is_checked for speeding-up
     cache_m2b: jnp.ndarray = -jnp.ones(8, dtype=jnp.int8)
     cache_king: jnp.ndarray = jnp.int32(44)
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "shogi"
+
     @staticmethod
     def _from_board(turn, piece_board: jnp.ndarray, hand: jnp.ndarray):
         """Mainly for debugging purpose.
         terminated, reward, and current_player are not changed"""
         state = State(turn=turn, piece_board=piece_board, hand=hand)  # type: ignore
         # fmt: off
         state = jax.lax.cond(turn % 2 == 1, lambda: _flip(state), lambda: state)
```

### Comparing `pgx-0.3.0/pgx/sparrow_mahjong.py` & `pgx-0.3.1/pgx/sparrow_mahjong.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     draw_ix: jnp.ndarray = jnp.int32(N_PLAYER * 5)
     shuffled_players: jnp.ndarray = jnp.zeros(
         N_PLAYER, dtype=jnp.int8
     )  # 0: dealer, ...
     dora: jnp.ndarray = jnp.int32(0)  # tile type (0~10) is set
     scores: jnp.ndarray = jnp.zeros(3, dtype=jnp.int32)  # 0 = dealer
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "sparrow_mahjong"
+
 
 class SparrowMahjong(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx/tic_tac_toe.py` & `pgx-0.3.1/pgx/tic_tac_toe.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
     # --- Tic-tac-toe specific ---
     turn: jnp.ndarray = jnp.int8(0)
     # 0 1 2
     # 3 4 5
     # 6 7 8
     board: jnp.ndarray = -jnp.ones(9, jnp.int8)  # -1 (empty), 0, 1
 
+    @property
+    def env_id(self) -> core.EnvId:
+        return "tic_tac_toe"
+
 
 class TicTacToe(core.Env):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `pgx-0.3.0/pgx.egg-info/SOURCES.txt` & `pgx-0.3.1/pgx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 pgx/_dwg/images/sparrow_mahjong/b.svg
 pgx/_dwg/images/sparrow_mahjong/gd.svg
 pgx/_dwg/images/sparrow_mahjong/oya.svg
 pgx/_dwg/images/sparrow_mahjong/rd.svg
 pgx/_flax/__init__.py
 pgx/_flax/serialization.py
 pgx/_flax/struct.py
+pgx/_mahjong/__init__.py
+pgx/_mahjong/_action.py
+pgx/_mahjong/_hand.py
 pgx/experimental/__init__.py
 pgx/experimental/gym.py
 pgx/experimental/pettingzoo.py
 pgx/experimental/utils.py
 pgx/experimental/visualize.py
 pgx/experimental/wrappers.py
 pgx/minatar/__init__.py
@@ -107,14 +110,15 @@
 tests/test_chess.py
 tests/test_connect_four.py
 tests/test_freeway.py
 tests/test_go.py
 tests/test_hex.py
 tests/test_kuhn_poker.py
 tests/test_leduc_holdem.py
+tests/test_mahjong.py
 tests/test_othello.py
 tests/test_play2048.py
 tests/test_seaquest.py
 tests/test_shogi.py
 tests/test_space_invaders.py
 tests/test_sparrow_mahjong.py
 tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.3.0/setup.py` & `pgx-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pgx",
-    version="0.3.0",
+    version="0.3.1",
     long_description_content_type="text/markdown",
     description="",
     url="",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
```

### Comparing `pgx-0.3.0/tests/minatar_utils.py` & `pgx-0.3.1/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_animal_shogi.py` & `pgx-0.3.1/tests/test_animal_shogi.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 env = AnimalShogi()
 init = jax.jit(env.init)
 step = jax.jit(env.step)
 
 
 def visualize(state, fname="tests/assets/animal_shogi/xxx.svg"):
-    from pgx._visualizer import Visualizer
-    v = Visualizer(color_theme="dark")
-    v.save_svg(state, fname)
+    state.save_svg(fname, color_theme="dark")
 
 
 def test_step():
     state = init(jax.random.PRNGKey(0))
     visualize(state, "tests/assets/animal_shogi/test_step_000.svg")
     assert not state.terminated
     assert state.turn == 0
```

### Comparing `pgx-0.3.0/tests/test_asterix.py` & `pgx-0.3.1/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_backgammon.py` & `pgx-0.3.1/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_breakout.py` & `pgx-0.3.1/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_bridge_bidding.py` & `pgx-0.3.1/tests/test_bridge_bidding.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,22 @@
         )
         assert (
             init_state.shuffled_players[3]
             == duplicated_state.shuffled_players[2]
         )
 
 
+def test_illegal_action_penalty():
+    key = jax.random.PRNGKey(0)
+    state = init(key)
+    state = step(state, 36)
+    print(state.reward)
+    assert jnp.all(state.reward == jnp.array([22800, -7600, 22800, 22800]))
+
+
 def test_step():
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
```

### Comparing `pgx-0.3.0/tests/test_chess.py` & `pgx-0.3.1/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_connect_four.py` & `pgx-0.3.1/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_freeway.py` & `pgx-0.3.1/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_go.py` & `pgx-0.3.1/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_hex.py` & `pgx-0.3.1/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_kuhn_poker.py` & `pgx-0.3.1/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_leduc_holdem.py` & `pgx-0.3.1/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_othello.py` & `pgx-0.3.1/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_play2048.py` & `pgx-0.3.1/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_seaquest.py` & `pgx-0.3.1/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_shogi.py` & `pgx-0.3.1/tests/test_shogi.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     """
     i = (x - 1) * 9 + (y - 1)
     return i
 
 
 # check visualization results by image preview plugins
 def visualize(state, fname="tests/assets/shogi/xxx.svg"):
-    from pgx._visualizer import Visualizer
-    v = Visualizer(color_theme="dark")
-    v.save_svg(state, fname)
+    state.save_svg(fname, color_theme="dark")
 
 
 def update_board(state, piece_board, hand=None):
     state = state.replace(piece_board=piece_board)
     if hand is not None:
         state = state.replace(hand=hand)
     return state
```

### Comparing `pgx-0.3.0/tests/test_space_invaders.py` & `pgx-0.3.1/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_sparrow_mahjong.py` & `pgx-0.3.1/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.0/tests/test_tic_tac_toe.py` & `pgx-0.3.1/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

