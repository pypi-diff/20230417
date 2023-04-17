# Comparing `tmp/hikari-lightbulb-2.3.2.tar.gz` & `tmp/hikari-lightbulb-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-lightbulb-2.3.2.tar", last modified: Sat Mar  4 13:27:28 2023, max compression
+gzip compressed data, was "hikari-lightbulb-2.3.3.tar", last modified: Mon Apr 17 17:34:58 2023, max compression
```

## Comparing `hikari-lightbulb-2.3.2.tar` & `hikari-lightbulb-2.3.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.080152 hikari-lightbulb-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-03-04 13:27:28.080152 hikari-lightbulb-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/crontrigger_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.072152 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-03-04 13:27:28.000000 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-04 13:27:28.000000 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 13:27:28.000000 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 13:27:28.000000 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-04 13:27:28.000000 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-04 13:27:28.000000 hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.072152 hikari-lightbulb-2.3.2/lightbulb/
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53239 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.076152 hikari-lightbulb-2.3.2/lightbulb/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35888 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/commands/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/commands/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/commands/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.076152 hikari-lightbulb-2.3.2/lightbulb/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/context/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/context/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/context/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/context/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.076152 hikari-lightbulb-2.3.2/lightbulb/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/converters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/converters/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/cooldown_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.068152 hikari-lightbulb-2.3.2/lightbulb/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.076152 hikari-lightbulb-2.3.2/lightbulb/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/ext/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/help_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:27:28.080152 hikari-lightbulb-2.3.2/lightbulb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/utils/data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    19435 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/utils/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/utils/pag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/lightbulb/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 13:27:28.080152 hikari-lightbulb-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-04 13:27:17.000000 hikari-lightbulb-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.687457 hikari-lightbulb-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-17 17:34:58.687457 hikari-lightbulb-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/crontrigger_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.679457 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-17 17:34:58.000000 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-17 17:34:58.000000 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:34:58.000000 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:34:58.000000 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 17:34:58.000000 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 17:34:58.000000 hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.683457 hikari-lightbulb-2.3.3/lightbulb/
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.683457 hikari-lightbulb-2.3.3/lightbulb/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35989 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/commands/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/commands/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/commands/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/commands/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.683457 hikari-lightbulb-2.3.3/lightbulb/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/context/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/context/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/context/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/context/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.683457 hikari-lightbulb-2.3.3/lightbulb/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/converters/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/cooldown_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.679457 hikari-lightbulb-2.3.3/lightbulb/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.683457 hikari-lightbulb-2.3.3/lightbulb/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/ext/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:34:58.687457 hikari-lightbulb-2.3.3/lightbulb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/utils/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/utils/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/utils/pag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/lightbulb/utils/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:34:58.687457 hikari-lightbulb-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-17 17:34:48.000000 hikari-lightbulb-2.3.3/setup.py
```

### Comparing `hikari-lightbulb-2.3.2/COPYING.LESSER.md` & `hikari-lightbulb-2.3.3/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/COPYING.md` & `hikari-lightbulb-2.3.3/COPYING.md`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/PKG-INFO` & `hikari-lightbulb-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-lightbulb
-Version: 2.3.2
+Version: 2.3.3
 Summary: A simple to use command handler for Hikari
 Home-page: https://github.com/tandemdude/hikari-lightbulb
 Author: tandemdude
 Author-email: tandemdude1@gmail.com
 License: LGPL-3.0-ONLY
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
```

### Comparing `hikari-lightbulb-2.3.2/README.md` & `hikari-lightbulb-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/PKG-INFO` & `hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-lightbulb
-Version: 2.3.2
+Version: 2.3.3
 Summary: A simple to use command handler for Hikari
 Home-page: https://github.com/tandemdude/hikari-lightbulb
 Author: tandemdude
 Author-email: tandemdude1@gmail.com
 License: LGPL-3.0-ONLY
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
```

### Comparing `hikari-lightbulb-2.3.2/hikari_lightbulb.egg-info/SOURCES.txt` & `hikari-lightbulb-2.3.3/hikari_lightbulb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/__init__.py` & `hikari-lightbulb-2.3.3/lightbulb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,8 +187,8 @@
 from lightbulb.decorators import *
 from lightbulb.errors import *
 from lightbulb.events import *
 from lightbulb.help_command import *
 from lightbulb.parser import *
 from lightbulb.plugins import *
 
-__version__ = "2.3.2"
+__version__ = "2.3.3"
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/__main__.py` & `hikari-lightbulb-2.3.3/lightbulb/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/app.py` & `hikari-lightbulb-2.3.3/lightbulb/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 # str is by definition a sequence of str so these type hints are correct
 def _default_get_prefix(_: BotApp, __: hikari.Message, *, prefixes: t.Sequence[str]) -> t.Sequence[str]:
     return prefixes
 
 
 class BotApp(hikari.GatewayBot):
     """
-    A subclassed implementation of the :obj:`~hikari.impl.bot.GatewayBot` class containing a command
+    A subclassed implementation of the :obj:`~hikari.impl.gateway_bot.GatewayBot` class containing a command
     handler. This should be instantiated instead of the superclass if you wish to use the command
     handler implementation provided.
 
     Args:
         token (:obj:`str`): The bot account's token.
         prefix (Optional[PrefixT]): The command prefix to use for prefix commands, or ``None`` if prefix commands
             will not be used.
@@ -164,15 +164,15 @@
             to the bot by default.
         help_slash_command (:obj:`bool`): Whether or not the help command should be implemented as a slash command
             as well as a prefix command. Defaults to ``False``.
         delete_unbound_commands (:obj:`bool`): Whether or not the bot should delete application commands that it cannot
             find an implementation for when the bot starts. Defaults to ``True``.
         case_insensitive_prefix_commands (:obj:`bool`): Whether or not prefix command names should be case-insensitive.
             Defaults to ``False``.
-        **kwargs (Any): Additional keyword arguments passed to the constructor of the :obj:`~hikari.impl.bot.GatewayBot`
+        **kwargs (Any): Additional keyword arguments passed to the constructor of the :obj:`~hikari.impl.gateway_bot.GatewayBot`
             class.
     """
 
     __slots__ = (
         "get_prefix",
         "ignore_bots",
         "owner_ids",
@@ -1258,21 +1258,24 @@
 
         # Invoke the autocomplete callback
         response = await callback(option, event.interaction)
         if not response:
             await event.interaction.create_response([])
             return
 
-        def convert_response_value(val: t.Union[str, int, float, hikari.CommandChoice]) -> hikari.CommandChoice:
+        def convert_response_value(
+            val: t.Union[str, int, float, hikari.api.AutocompleteChoiceBuilder]
+        ) -> hikari.api.AutocompleteChoiceBuilder:
             if isinstance(val, (str, int, float)):
-                return hikari.CommandChoice(name=str(val), value=val)
+                return hikari.impl.AutocompleteChoiceBuilder(name=str(val), value=val)
+
             return val
 
-        resp_to_send: t.List[hikari.CommandChoice] = []
-        if isinstance(response, (str, int, float, hikari.CommandChoice)):
+        resp_to_send: t.List[hikari.api.AutocompleteChoiceBuilder] = []
+        if isinstance(response, (str, int, float, hikari.api.AutocompleteChoiceBuilder)):
             resp_to_send.append(convert_response_value(response))
         elif isinstance(response, collections.abc.Sequence):
             for item in response:
                 resp_to_send.append(convert_response_value(item))
         else:
             _LOGGER.error("Invalid response returned from autocomplete handler %r", callback.__name__)  # type: ignore[unreachable]
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/buckets.py` & `hikari-lightbulb-2.3.3/lightbulb/buckets.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/checks.py` & `hikari-lightbulb-2.3.3/lightbulb/checks.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/commands/__init__.py` & `hikari-lightbulb-2.3.3/lightbulb/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/commands/base.py` & `hikari-lightbulb-2.3.3/lightbulb/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     bound=t.Callable[
         ...,
         t.Coroutine[
             t.Any,
             t.Any,
             t.Union[
                 _AutocompleteableOptionT,
-                hikari.CommandChoice,
-                t.Sequence[t.Union[_AutocompleteableOptionT, hikari.CommandChoice]],
+                hikari.api.AutocompleteChoiceBuilder,
+                t.Sequence[t.Union[_AutocompleteableOptionT, hikari.api.AutocompleteChoiceBuilder]],
             ],
         ],
     ],
 )
 ErrorHandlerCallbackT = t.TypeVar(
     "ErrorHandlerCallbackT", bound=t.Callable[..., t.Coroutine[t.Any, t.Any, t.Optional[bool]]]
 )
@@ -157,21 +157,21 @@
     default: hikari.UndefinedOr[t.Any] = hikari.UNDEFINED
     """The default value for this option."""
     modifier: OptionModifier = OptionModifier.NONE
     """Additional modifier controlling how the option should be parsed. This only affects prefix commands."""
     min_value: t.Optional[t.Union[float, int]] = None
     """
     The minimum value permitted for this option (inclusive). The option must be ``INTEGER`` or ``FLOAT`` to use this.
-    
+
     .. versionadded:: 2.1.3
     """
     max_value: t.Optional[t.Union[float, int]] = None
     """
     The maximum value permitted for this option (inclusive). The option must be ``INTEGER`` or ``FLOAT`` to use this.
-    
+
     .. versionadded:: 2.1.3
     """
     min_length: t.Optional[int] = None
     """
     The minimum length permitted for this option. The option must be ``STRING`` to use this.
 
     .. versionadded:: 2.3.2
@@ -313,73 +313,73 @@
     hidden: bool = False
     """Whether or not the command should be hidden from the help command."""
     inherit_checks: bool = False
     """Whether or not the command should inherit checks from the parent group."""
     pass_options: bool = False
     """
     Whether or not the command will have its options passed as keyword arguments when invoked.
-    
+
     .. versionadded:: 2.2.1
     """
     max_concurrency: t.Optional[t.Tuple[int, t.Type[buckets.Bucket]]] = None
     """
     The max concurrency rule for the command.
-    
+
     .. versionadded:: 2.2.1
     """
     app_command_default_member_permissions: t.Optional[hikari.Permissions] = None
     """
     The default member permissions for this command, if an application command.
-    
+
     .. versionadded:: 2.2.3
     """
     app_command_dm_enabled: bool = True
     """
     Whether this command will be enabled in DMs, if an application command.
-    
+
     .. versionadded:: 2.2.3
     """
     app_command_bypass_author_permission_checks: bool = False
     """
     Whether invocations of this command will bypass author permission checks, if an application command.
-    
+
     .. versionadded:: 2.2.3
     """
     name_localizations: t.Mapping[t.Union[hikari.Locale, str], str] = dataclasses.field(default_factory=dict)
     """
     A mapping of locale to name localizations for this command
-    
+
     .. versionadded:: 2.3.0
     """
     description_localizations: t.Mapping[t.Union[hikari.Locale, str], str] = dataclasses.field(default_factory=dict)
     """
     A mapping of locale to description localizations for this command
-    
+
     .. versionadded:: 2.3.0
     """
     nsfw: bool = False
     """
     Whether the command should only be enabled in NSFW channels.
-    
+
     For prefix commands, this will add an NSFW-channel only check to the command automatically.
     For slash commands, this will behave as specified in the Discord documentation.
-    
+
     .. versionadded:: 2.3.1
     """
     _autocomplete_callbacks: t.Dict[
         str,
         t.Callable[
             [hikari.CommandInteractionOption, hikari.AutocompleteInteraction],
             t.Coroutine[
                 t.Any,
                 t.Any,
                 t.Union[
                     _AutocompleteableOptionT,
-                    hikari.CommandChoice,
-                    t.Sequence[t.Union[_AutocompleteableOptionT, hikari.CommandChoice]],
+                    hikari.api.AutocompleteChoiceBuilder,
+                    t.Sequence[t.Union[_AutocompleteableOptionT, hikari.api.AutocompleteChoiceBuilder]],
                 ],
             ],
         ],
     ] = dataclasses.field(default_factory=dict, init=False)
 
     async def __call__(self, context: context_.base.Context) -> None:
         await self.callback(context)
@@ -518,15 +518,15 @@
                 @lightbulb.implements(lightbulb.SlashCommand)
                 async def foo(ctx: lightbulb.Context) -> None
                     ...
 
                 @foo.autocomplete("foo")  # Name of the option you want to autocomplete
                 async def foo_autocomplete(
                     opt: hikari.AutocompleteInteractionOption, inter: hikari.AutocompleteInteraction
-                ) -> Union[str, Sequence[str], hikari.CommandChoice, Sequence[hikari.CommandChoice]]:
+                ) -> Union[str, Sequence[str], hikari.api.AutocompleteChoiceBuilder, Sequence[hikari.api.AutocompleteChoiceBuilder]]:
                     ...
         """
 
         def decorate(func: AutocompleteCallbackT) -> AutocompleteCallbackT:
             for opt in [opt1, *opts]:
                 self._autocomplete_callbacks[opt] = func
             return func
@@ -768,15 +768,16 @@
             return
         bucket_hash = self.max_concurrency[1].extract_hash(context)
         if bucket_hash not in self._max_concurrency_semaphores:
             self._max_concurrency_semaphores[bucket_hash] = asyncio.Semaphore(self.max_concurrency[0])
         if self._max_concurrency_semaphores[bucket_hash].locked():
             assert context.invoked is not None
             raise errors.MaxConcurrencyLimitReached(
-                f"Maximum concurrency limit for command '{context.invoked.qualname}' exceeded"
+                f"Maximum concurrency limit for command '{context.invoked.qualname}' exceeded",
+                bucket=self.max_concurrency[1],
             )
         await self._max_concurrency_semaphores[bucket_hash].acquire()
 
     def _release_max_concurrency(self, context: context_.base.Context) -> None:
         if self.max_concurrency is None:
             return
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/commands/message.py` & `hikari-lightbulb-2.3.3/lightbulb/commands/message.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/commands/prefix.py` & `hikari-lightbulb-2.3.3/lightbulb/commands/prefix.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/commands/slash.py` & `hikari-lightbulb-2.3.3/lightbulb/commands/slash.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/commands/user.py` & `hikari-lightbulb-2.3.3/lightbulb/commands/user.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/context/__init__.py` & `hikari-lightbulb-2.3.3/lightbulb/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/context/base.py` & `hikari-lightbulb-2.3.3/lightbulb/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/context/message.py` & `hikari-lightbulb-2.3.3/lightbulb/context/message.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/context/prefix.py` & `hikari-lightbulb-2.3.3/lightbulb/context/prefix.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/context/slash.py` & `hikari-lightbulb-2.3.3/lightbulb/context/slash.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/context/user.py` & `hikari-lightbulb-2.3.3/lightbulb/context/user.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/converters/__init__.py` & `hikari-lightbulb-2.3.3/lightbulb/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/converters/base.py` & `hikari-lightbulb-2.3.3/lightbulb/converters/base.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/converters/special.py` & `hikari-lightbulb-2.3.3/lightbulb/converters/special.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/cooldown_algorithms.py` & `hikari-lightbulb-2.3.3/lightbulb/cooldown_algorithms.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/cooldowns.py` & `hikari-lightbulb-2.3.3/lightbulb/cooldowns.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/decorators.py` & `hikari-lightbulb-2.3.3/lightbulb/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,21 @@
 if t.TYPE_CHECKING:
     from lightbulb import context
 
 T = t.TypeVar("T")
 CommandCallbackT = t.TypeVar("CommandCallbackT", bound=t.Callable[..., t.Coroutine[t.Any, t.Any, None]])
 AutocompleteCallbackT = t.Callable[
     [hikari.CommandInteractionOption, hikari.AutocompleteInteraction],
-    t.Coroutine[t.Any, t.Any, t.Union[str, hikari.CommandChoice, t.Sequence[t.Union[str, hikari.CommandChoice]]]],
+    t.Coroutine[
+        t.Any,
+        t.Any,
+        t.Union[
+            str, hikari.api.AutocompleteChoiceBuilder, t.Sequence[t.Union[str, hikari.api.AutocompleteChoiceBuilder]]
+        ],
+    ],
 ]
 
 
 def implements(
     *command_types: t.Type[commands.base.Command],
 ) -> t.Callable[[CommandCallbackT], CommandCallbackT]:
     """
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/errors.py` & `hikari-lightbulb-2.3.3/lightbulb/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 import typing as t
 import warnings
 
 import hikari
 
 if t.TYPE_CHECKING:
+    from lightbulb import buckets
     from lightbulb import commands
 
 
 class LightbulbError(Exception):
     """
     Base lightbulb exception class. All errors raised by lightbulb will be a subclass
     of this exception.
@@ -156,15 +157,15 @@
     def __init__(self, *args: t.Any, opt: commands.base.OptionLike, raw: str) -> None:
         super().__init__(*args)
         self.option: commands.base.OptionLike = opt
         """The option that could not be converted."""
         self.raw_value: str = raw
         """
         The value that could not be converted.
-        
+
         .. versionadded:: 2.2.1
         """
 
 
 class NotEnoughArguments(LightbulbError):
     """
     Error raised when a prefix command expects more options than could be parsed from the user's input.
@@ -193,14 +194,25 @@
 
 class MaxConcurrencyLimitReached(LightbulbError):
     """
     Error raised when the maximum number of allowed concurrent invocations for a command
     has been exceeded.
     """
 
+    __slots__ = ("bucket",)
+
+    def __init__(self, *args: t.Any, bucket: t.Type[buckets.Bucket]) -> None:
+        super().__init__(*args)
+        self.bucket = bucket
+        """
+        The bucket type that triggered the max concurrency limit.
+
+        .. versionadded:: 2.3.3
+        """
+
 
 class CheckFailure(LightbulbError):
     """
     Error raised when a check fails before command invocation. If another error caused this
     to be raised then you can access it using ``CheckFailure.__cause__``, or in the case of
     multiple checks failing, via ``CheckFailure.causes`` (since version `2.2.1`).
     """
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/events.py` & `hikari-lightbulb-2.3.3/lightbulb/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 import abc
 import types
 import typing as t
 
 import attr
 import hikari
-from hikari.events import base_events
 
 if t.TYPE_CHECKING:
     from lightbulb import app as app_
     from lightbulb import commands
     from lightbulb import context as context_
     from lightbulb import errors
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/ext/tasks/__init__.py` & `hikari-lightbulb-2.3.3/lightbulb/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/ext/tasks/triggers.py` & `hikari-lightbulb-2.3.3/lightbulb/ext/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/help_command.py` & `hikari-lightbulb-2.3.3/lightbulb/help_command.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/internal.py` & `hikari-lightbulb-2.3.3/lightbulb/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Lightbulb. If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ["serialise_command", "manage_application_commands"]
 
-import collections
 import logging
 import typing as t
 
 import hikari
 
 if t.TYPE_CHECKING:
     from lightbulb import app as app_
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/parser.py` & `hikari-lightbulb-2.3.3/lightbulb/parser.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/plugins.py` & `hikari-lightbulb-2.3.3/lightbulb/plugins.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/utils/__init__.py` & `hikari-lightbulb-2.3.3/lightbulb/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/utils/data_store.py` & `hikari-lightbulb-2.3.3/lightbulb/utils/data_store.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/utils/nav.py` & `hikari-lightbulb-2.3.3/lightbulb/utils/nav.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         """
         Check if the button is pressed in a given event.
 
         Args:
             event (:obj:`~hikari.events.message.MessageReactionEvent`): The event to check the button is pressed in.
 
         Returns:
-            :obj:`bool`: Whether or not the button is pressed in the given event.
+            :obj:`bool`: Whether the button is pressed in the given event.
         """
         if event.emoji_id is not None and isinstance(self.emoji, hikari.CustomEmoji):
             return event.emoji_id == self.emoji.id
         return event.emoji_name == self.emoji.name
 
     def press(self, nav: ReactionNavigator[T], event: hikari.ReactionAddEvent) -> t.Coroutine[t.Any, t.Any, None]:
         """
@@ -90,26 +90,26 @@
     A component-based navigator button. Contains the custom_id linked to the button as well as
     the coroutine to be called when the button is pressed.
 
     Args:
         label (:obj:`str`): The label of the button.
         label_is_emoji (:obj:`bool`): Whether the label is an emoji or not. This affects whether ``set_label`` or
             ``set_emoji`` is called when building the button.
-        style (:obj:`hikari.ButtonStyle`): The style of the button.
+        style (:obj:`hikari.InteractiveButtonTypesT`): The style of the button.
         custom_id (:obj:`str`): The custom ID of the button.
         callback: The coroutine function to be called on button press.
     """
 
     __slots__ = ("custom_id", "callback", "label", "style", "label_is_emoji")
 
     def __init__(
         self,
         label: str,
         label_is_emoji: bool,
-        style: ButtonStyle,
+        style: hikari.InteractiveButtonTypesT,
         custom_id: str,
         callback: t.Callable[[ButtonNavigator[T], hikari.InteractionCreateEvent], t.Coroutine[t.Any, t.Any, None]],
     ) -> None:
         self.label = label
         self.label_is_emoji = label_is_emoji
         self.style = style
         self.custom_id = custom_id
@@ -117,23 +117,25 @@
 
     def build(self, container: MessageActionRowBuilder, disabled: bool = False) -> None:
         """
         Build and add the button to the given container.
 
         Args:
             container (:obj:`hikari.api.special_endpoints.MessageActionRowBuilder`): The container to add the button to.
-            disabled (:obj:`bool`): Whether or not to display the button as disabled.
+            disabled (:obj:`bool`): Whether to display the button as disabled.
 
         Returns:
             ``None``
         """
-        btn = container.add_button(self.style, self.custom_id)
-        btn.set_is_disabled(disabled)
-        getattr(btn, f"set_{'emoji' if self.label_is_emoji else 'label'}")(self.label)
-        btn.add_to_container()
+        container.add_interactive_button(
+            self.style,
+            self.custom_id,
+            is_disabled=disabled,
+            **{"emoji" if self.label_is_emoji else "label": self.label},
+        )
 
     def is_pressed(self, event: hikari.InteractionCreateEvent) -> bool:
         """
         Check if the button is pressed in a given event.
 
         Args:
             event (:obj:`~hikari.InteractionCreateEvent`): The event to check the button is pressed in.
```

### Comparing `hikari-lightbulb-2.3.2/lightbulb/utils/pag.py` & `hikari-lightbulb-2.3.3/lightbulb/utils/pag.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/utils/permissions.py` & `hikari-lightbulb-2.3.3/lightbulb/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/lightbulb/utils/search.py` & `hikari-lightbulb-2.3.3/lightbulb/utils/search.py`

 * *Files identical despite different names*

### Comparing `hikari-lightbulb-2.3.2/setup.py` & `hikari-lightbulb-2.3.3/setup.py`

 * *Files identical despite different names*

