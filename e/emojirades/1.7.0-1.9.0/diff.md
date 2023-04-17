# Comparing `tmp/emojirades-1.7.0.tar.gz` & `tmp/emojirades-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emojirades-1.7.0.tar", last modified: Sat Jul 16 10:32:26 2022, max compression
+gzip compressed data, was "emojirades-1.9.0.tar", last modified: Sat Dec  3 21:22:16 2022, max compression
```

## Comparing `emojirades-1.7.0.tar` & `emojirades-1.9.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.122842 emojirades-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-07-16 10:32:15.000000 emojirades-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8178 2022-07-16 10:32:26.122842 emojirades-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-07-16 10:32:15.000000 emojirades-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.110842 emojirades-1.7.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3197 2022-07-16 10:32:15.000000 emojirades-1.7.0/bin/emojirades
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.114842 emojirades-1.7.0/emojirades/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.114842 emojirades-1.7.0/emojirades/analytics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/analytics/scoreboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/analytics/time_range.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/analytics/time_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     8931 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.114842 emojirades-1.7.0/emojirades/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/commands/gamestate_commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/correct_guess_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/fixwinner_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/game_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/inferred_correct_guess_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/newgame_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/remove_admin_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/set_admin_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/gamestate_commands/set_emojirade_command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/commands/general_commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/general_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/general_commands/help_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/commands/scorekeeper_commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/scorekeeper_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/scorekeeper_commands/history_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/scorekeeper_commands/minusminus_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/scorekeeper_commands/scoreboard_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/commands/scorekeeper_commands/set_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     8969 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/gamestate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/persistence/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/handlers/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/handlers/gamestate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/handlers/scorekeeper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/handlers/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/persistence/models/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.118842 emojirades-1.7.0/emojirades/persistence/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.122842 emojirades-1.7.0/emojirades/persistence/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/alembic/versions/2a7a559e761b_initial_models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/gamestate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/models/scorekeeper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/persistence/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.122842 emojirades-1.7.0/emojirades/printers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/printers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/printers/scoreboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/scorekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.122842 emojirades-1.7.0/emojirades/slack/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/slack/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/slack/slack_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4584 2022-07-16 10:32:15.000000 emojirades-1.7.0/emojirades/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 10:32:26.114842 emojirades-1.7.0/emojirades.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8178 2022-07-16 10:32:26.000000 emojirades-1.7.0/emojirades.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-07-16 10:32:26.000000 emojirades-1.7.0/emojirades.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-16 10:32:26.000000 emojirades-1.7.0/emojirades.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-07-16 10:32:26.000000 emojirades-1.7.0/emojirades.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-16 10:32:26.000000 emojirades-1.7.0/emojirades.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-16 10:32:15.000000 emojirades-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-07-16 10:32:26.122842 emojirades-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.603934 emojirades-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-03 21:22:06.000000 emojirades-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2022-12-03 21:22:16.603934 emojirades-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2022-12-03 21:22:06.000000 emojirades-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.595934 emojirades-1.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3197 2022-12-03 21:22:06.000000 emojirades-1.9.0/bin/emojirades
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.595934 emojirades-1.9.0/emojirades/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.595934 emojirades-1.9.0/emojirades/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/analytics/scoreboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/analytics/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/analytics/time_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.595934 emojirades-1.9.0/emojirades/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/commands/gamestate_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/correct_guess_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/fixwinner_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/game_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/inferred_correct_guess_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/newgame_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/remove_admin_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/set_admin_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/gamestate_commands/set_emojirade_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/commands/general_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/general_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/general_commands/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/commands/scorekeeper_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/scorekeeper_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/scorekeeper_commands/history_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/scorekeeper_commands/minusminus_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/scorekeeper_commands/scoreboard_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/commands/scorekeeper_commands/set_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/gamestate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/persistence/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/handlers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/handlers/gamestate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/handlers/scorekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/handlers/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/persistence/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/persistence/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/persistence/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/alembic/versions/2a7a559e761b_initial_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/gamestate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/models/scorekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/persistence/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.599934 emojirades-1.9.0/emojirades/printers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/printers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/printers/scoreboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/scorekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.603934 emojirades-1.9.0/emojirades/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/slack/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/slack/slack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2022-12-03 21:22:06.000000 emojirades-1.9.0/emojirades/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:22:16.595934 emojirades-1.9.0/emojirades.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2022-12-03 21:22:16.000000 emojirades-1.9.0/emojirades.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2022-12-03 21:22:16.000000 emojirades-1.9.0/emojirades.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 21:22:16.000000 emojirades-1.9.0/emojirades.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2022-12-03 21:22:16.000000 emojirades-1.9.0/emojirades.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-03 21:22:16.000000 emojirades-1.9.0/emojirades.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-03 21:22:06.000000 emojirades-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2022-12-03 21:22:16.603934 emojirades-1.9.0/setup.cfg
```

### Comparing `emojirades-1.7.0/LICENSE` & `emojirades-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/PKG-INFO` & `emojirades-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: emojirades
-Version: 1.7.0
+Version: 1.9.0
 Summary: Slack bot that understands the Emojirades game!
 Home-page: https://github.com/emojirades/emojirades
 Author: The Emojirades Team
 Author-email: support@emojirades.io
 License: AGPLv3
 Keywords: slack slackbot emojirades plusplus game
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Games/Entertainment
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `emojirades-1.7.0/README.md` & `emojirades-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/bin/emojirades` & `emojirades-1.9.0/bin/emojirades`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/analytics/scoreboard.py` & `emojirades-1.9.0/emojirades/analytics/scoreboard.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/analytics/time_range.py` & `emojirades-1.9.0/emojirades/analytics/time_range.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/bot.py` & `emojirades-1.9.0/emojirades/bot.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/__init__.py` & `emojirades-1.9.0/emojirades/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/correct_guess_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/correct_guess_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/fixwinner_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/fixwinner_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/game_status.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/game_status.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/inferred_correct_guess_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/inferred_correct_guess_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/newgame_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/newgame_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/remove_admin_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/remove_admin_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/set_admin_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/set_admin_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/gamestate_commands/set_emojirade_command.py` & `emojirades-1.9.0/emojirades/commands/gamestate_commands/set_emojirade_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/general_commands/help_command.py` & `emojirades-1.9.0/emojirades/commands/general_commands/help_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/registry.py` & `emojirades-1.9.0/emojirades/commands/registry.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/scorekeeper_commands/history_command.py` & `emojirades-1.9.0/emojirades/commands/scorekeeper_commands/history_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/scorekeeper_commands/minusminus_command.py` & `emojirades-1.9.0/emojirades/commands/scorekeeper_commands/minusminus_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/scorekeeper_commands/scoreboard_command.py` & `emojirades-1.9.0/emojirades/commands/scorekeeper_commands/scoreboard_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/commands/scorekeeper_commands/set_command.py` & `emojirades-1.9.0/emojirades/commands/scorekeeper_commands/set_command.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/gamestate.py` & `emojirades-1.9.0/emojirades/gamestate.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/helpers.py` & `emojirades-1.9.0/emojirades/helpers.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/handlers/auth.py` & `emojirades-1.9.0/emojirades/persistence/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/handlers/gamestate.py` & `emojirades-1.9.0/emojirades/persistence/handlers/gamestate.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/handlers/scorekeeper.py` & `emojirades-1.9.0/emojirades/persistence/handlers/scorekeeper.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/handlers/workspace.py` & `emojirades-1.9.0/emojirades/persistence/handlers/workspace.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/models/alembic/env.py` & `emojirades-1.9.0/emojirades/persistence/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/models/alembic/versions/2a7a559e761b_initial_models.py` & `emojirades-1.9.0/emojirades/persistence/models/alembic/versions/2a7a559e761b_initial_models.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/models/alembic.ini` & `emojirades-1.9.0/emojirades/persistence/models/alembic.ini`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/models/gamestate.py` & `emojirades-1.9.0/emojirades/persistence/models/gamestate.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/models/scorekeeper.py` & `emojirades-1.9.0/emojirades/persistence/models/scorekeeper.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/persistence/orm.py` & `emojirades-1.9.0/emojirades/persistence/orm.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/printers/scoreboard.py` & `emojirades-1.9.0/emojirades/printers/scoreboard.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/scorekeeper.py` & `emojirades-1.9.0/emojirades/scorekeeper.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/slack/event.py` & `emojirades-1.9.0/emojirades/slack/event.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/slack/slack_client.py` & `emojirades-1.9.0/emojirades/slack/slack_client.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades/wrappers.py` & `emojirades-1.9.0/emojirades/wrappers.py`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/emojirades.egg-info/PKG-INFO` & `emojirades-1.9.0/emojirades.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: emojirades
-Version: 1.7.0
+Version: 1.9.0
 Summary: Slack bot that understands the Emojirades game!
 Home-page: https://github.com/emojirades/emojirades
 Author: The Emojirades Team
 Author-email: support@emojirades.io
 License: AGPLv3
 Keywords: slack slackbot emojirades plusplus game
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Games/Entertainment
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `emojirades-1.7.0/emojirades.egg-info/SOURCES.txt` & `emojirades-1.9.0/emojirades.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emojirades-1.7.0/setup.cfg` & `emojirades-1.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -9,48 +9,49 @@
 	License :: OSI Approved :: GNU Affero General Public License v3
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Communications :: Chat
 	Topic :: Games/Entertainment
 license = AGPLv3
 description = Slack bot that understands the Emojirades game!
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 keywords = slack slackbot emojirades plusplus game
 
 [options]
 install_requires = 
-	slack_sdk~=3.17.2
+	slack_sdk~=3.19.5
 	requests~=2.28.1
-	boto3~=1.24.31
-	Unidecode~=1.3.4
+	boto3~=1.26.22
+	Unidecode~=1.3.6
 	pendulum~=2.1.2
 	expiringdict~=1.2.2
-	SQLAlchemy~=1.4.39
+	SQLAlchemy~=1.4.44
 	alembic~=1.8.1
-	psycopg2-binary~=2.9.3
+	psycopg2-binary~=2.9.5
 	python-json-logger~=2.0.4
 python_requires = >=3.8
 scripts = 
 	bin/emojirades
 packages = find:
 
 [options.packages.find]
 exclude = 
 	tests
 
 [options.extras_require]
 dev = 
-	pytest~=7.1.2
-	pylint~=2.14.4
-	black~=22.6.0
+	pytest~=7.2.0
+	pylint~=2.15.7
+	black~=22.10.0
 	websockets~=10.3
 
 [options.package_data]
 * = *.ini
 
 [egg_info]
 tag_build =
```

