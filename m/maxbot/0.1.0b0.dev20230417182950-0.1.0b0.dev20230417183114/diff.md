# Comparing `tmp/maxbot-0.1.0b0.dev20230417182950.tar.gz` & `tmp/maxbot-0.1.0b0.dev20230417183114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxbot-0.1.0b0.dev20230417182950.tar", max compression
+gzip compressed data, was "maxbot-0.1.0b0.dev20230417183114.tar", max compression
```

## Comparing `maxbot-0.1.0b0.dev20230417182950.tar` & `maxbot-0.1.0b0.dev20230417183114.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      162 2023-02-15 19:48:36.383070 maxbot-0.1.0b0.dev20230417182950/maxbot/__init__.py
--rw-r--r--   0        0        0       75 2023-02-15 19:48:36.383149 maxbot-0.1.0b0.dev20230417182950/maxbot/__main__.py
--rw-r--r--   0        0        0     2724 2023-04-06 19:54:36.491470 maxbot-0.1.0b0.dev20230417182950/maxbot/_download.py
--rw-r--r--   0        0        0      787 2023-04-06 19:54:36.491593 maxbot-0.1.0b0.dev20230417182950/maxbot/_hooks.py
--rw-r--r--   0        0        0    12772 2023-04-06 19:54:36.491733 maxbot-0.1.0b0.dev20230417182950/maxbot/bot.py
--rw-r--r--   0        0        0    14553 2023-04-06 19:54:36.491856 maxbot-0.1.0b0.dev20230417182950/maxbot/builder.py
--rw-r--r--   0        0        0      186 2023-04-06 19:54:36.491956 maxbot-0.1.0b0.dev20230417182950/maxbot/channels/__init__.py
--rw-r--r--   0        0        0     7515 2023-04-06 19:54:36.492045 maxbot-0.1.0b0.dev20230417182950/maxbot/channels/_manager.py
--rw-r--r--   0        0        0     9338 2023-04-06 19:54:36.492354 maxbot-0.1.0b0.dev20230417182950/maxbot/channels/facebook.py
--rw-r--r--   0        0        0     5772 2023-04-06 19:54:36.492466 maxbot-0.1.0b0.dev20230417182950/maxbot/channels/telegram.py
--rw-r--r--   0        0        0     8940 2023-04-06 19:54:36.492593 maxbot-0.1.0b0.dev20230417182950/maxbot/channels/viber.py
--rw-r--r--   0        0        0    11077 2023-04-06 19:54:36.492718 maxbot-0.1.0b0.dev20230417182950/maxbot/channels/vk.py
--rw-r--r--   0        0        0      383 2023-04-06 19:54:36.492827 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/__init__.py
--rw-r--r--   0        0        0     1882 2023-04-06 19:54:36.492893 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_bot.py
--rw-r--r--   0        0        0     2061 2023-04-13 11:42:37.915066 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_journal.py
--rw-r--r--   0        0        0     1638 2023-04-06 19:54:36.493044 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_logging.py
--rw-r--r--   0        0        0     1963 2023-04-06 19:54:36.493111 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_ngrok.py
--rw-r--r--   0        0        0     7245 2023-04-13 11:42:37.915176 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_rich.py
--rw-r--r--   0        0        0     5448 2023-04-06 19:54:36.493289 maxbot-0.1.0b0.dev20230417182950/maxbot/cli/run.py
--rw-r--r--   0        0        0    18478 2023-04-06 19:54:36.493487 maxbot-0.1.0b0.dev20230417182950/maxbot/context.py
--rw-r--r--   0        0        0     5087 2023-04-06 19:54:36.493584 maxbot-0.1.0b0.dev20230417182950/maxbot/dialog_manager.py
--rw-r--r--   0        0        0    10096 2023-04-13 11:42:37.915305 maxbot-0.1.0b0.dev20230417182950/maxbot/errors.py
--rw-r--r--   0        0        0      139 2023-04-06 19:54:36.493703 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/__init__.py
--rw-r--r--   0        0        0     4185 2023-04-06 19:54:36.493777 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/_manager.py
--rw-r--r--   0        0        0     2738 2023-04-06 19:54:36.493894 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/datetime.py
--rw-r--r--   0        0        0     2568 2023-04-06 19:54:36.494005 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/format.py
--rw-r--r--   0        0        0     1043 2023-04-06 19:54:36.494122 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/jinja_loader.py
--rw-r--r--   0        0        0     5515 2023-04-06 19:54:36.494243 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/rasa.py
--rw-r--r--   0        0        0     5592 2023-04-06 19:54:36.494389 maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/rest.py
--rw-r--r--   0        0        0       33 2023-04-06 19:54:36.494500 maxbot-0.1.0b0.dev20230417182950/maxbot/flows/__init__.py
--rw-r--r--   0        0        0     1189 2023-02-15 19:48:36.387288 maxbot-0.1.0b0.dev20230417182950/maxbot/flows/_base.py
--rw-r--r--   0        0        0     2053 2023-04-06 19:54:36.494565 maxbot-0.1.0b0.dev20230417182950/maxbot/flows/dialog_flow.py
--rw-r--r--   0        0        0    24789 2023-04-13 11:42:37.915461 maxbot-0.1.0b0.dev20230417182950/maxbot/flows/dialog_tree.py
--rw-r--r--   0        0        0    12228 2023-04-13 11:42:37.915591 maxbot-0.1.0b0.dev20230417182950/maxbot/flows/slot_filling.py
--rw-r--r--   0        0        0     7448 2023-04-13 11:42:37.915711 maxbot-0.1.0b0.dev20230417182950/maxbot/jinja_env.py
--rw-r--r--   0        0        0     4603 2023-04-13 11:42:37.915831 maxbot-0.1.0b0.dev20230417182950/maxbot/markdown.py
--rw-r--r--   0        0        0    20628 2023-04-06 19:54:36.495666 maxbot-0.1.0b0.dev20230417182950/maxbot/nlu.py
--rw-r--r--   0        0        0    10536 2023-04-06 19:54:36.495773 maxbot-0.1.0b0.dev20230417182950/maxbot/resources.py
--rw-r--r--   0        0        0     4728 2023-04-06 19:54:36.495920 maxbot-0.1.0b0.dev20230417182950/maxbot/rpc.py
--rw-r--r--   0        0        0     8753 2023-04-13 11:42:37.915981 maxbot-0.1.0b0.dev20230417182950/maxbot/scenarios.py
--rw-r--r--   0        0        0    16810 2023-04-13 11:42:37.916125 maxbot-0.1.0b0.dev20230417182950/maxbot/schemas.py
--rw-r--r--   0        0        0     4164 2023-04-06 19:54:36.496507 maxbot-0.1.0b0.dev20230417182950/maxbot/state_store.py
--rw-r--r--   0        0        0     1051 2023-04-06 19:54:36.496579 maxbot-0.1.0b0.dev20230417182950/maxbot/user_locks.py
--rw-r--r--   0        0        0    14851 2023-04-13 11:42:37.916226 maxbot-0.1.0b0.dev20230417182950/maxbot/xml.py
--rw-r--r--   0        0        0     1596 2023-04-17 15:29:51.270350 maxbot-0.1.0b0.dev20230417182950/pyproject.toml
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 maxbot-0.1.0b0.dev20230417182950/setup.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 maxbot-0.1.0b0.dev20230417182950/PKG-INFO
+-rw-r--r--   0        0        0      162 2023-02-15 19:48:36.383070 maxbot-0.1.0b0.dev20230417183114/maxbot/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-15 19:48:36.383149 maxbot-0.1.0b0.dev20230417183114/maxbot/__main__.py
+-rw-r--r--   0        0        0     2724 2023-04-06 19:54:36.491470 maxbot-0.1.0b0.dev20230417183114/maxbot/_download.py
+-rw-r--r--   0        0        0      787 2023-04-06 19:54:36.491593 maxbot-0.1.0b0.dev20230417183114/maxbot/_hooks.py
+-rw-r--r--   0        0        0    12772 2023-04-06 19:54:36.491733 maxbot-0.1.0b0.dev20230417183114/maxbot/bot.py
+-rw-r--r--   0        0        0    14553 2023-04-06 19:54:36.491856 maxbot-0.1.0b0.dev20230417183114/maxbot/builder.py
+-rw-r--r--   0        0        0      186 2023-04-06 19:54:36.491956 maxbot-0.1.0b0.dev20230417183114/maxbot/channels/__init__.py
+-rw-r--r--   0        0        0     7515 2023-04-06 19:54:36.492045 maxbot-0.1.0b0.dev20230417183114/maxbot/channels/_manager.py
+-rw-r--r--   0        0        0     9338 2023-04-06 19:54:36.492354 maxbot-0.1.0b0.dev20230417183114/maxbot/channels/facebook.py
+-rw-r--r--   0        0        0     5772 2023-04-06 19:54:36.492466 maxbot-0.1.0b0.dev20230417183114/maxbot/channels/telegram.py
+-rw-r--r--   0        0        0     8940 2023-04-06 19:54:36.492593 maxbot-0.1.0b0.dev20230417183114/maxbot/channels/viber.py
+-rw-r--r--   0        0        0    11077 2023-04-06 19:54:36.492718 maxbot-0.1.0b0.dev20230417183114/maxbot/channels/vk.py
+-rw-r--r--   0        0        0      383 2023-04-06 19:54:36.492827 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/__init__.py
+-rw-r--r--   0        0        0     1882 2023-04-06 19:54:36.492893 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_bot.py
+-rw-r--r--   0        0        0     2061 2023-04-13 11:42:37.915066 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_journal.py
+-rw-r--r--   0        0        0     1638 2023-04-06 19:54:36.493044 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_logging.py
+-rw-r--r--   0        0        0     1963 2023-04-06 19:54:36.493111 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_ngrok.py
+-rw-r--r--   0        0        0     7245 2023-04-13 11:42:37.915176 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_rich.py
+-rw-r--r--   0        0        0     5448 2023-04-06 19:54:36.493289 maxbot-0.1.0b0.dev20230417183114/maxbot/cli/run.py
+-rw-r--r--   0        0        0    18478 2023-04-06 19:54:36.493487 maxbot-0.1.0b0.dev20230417183114/maxbot/context.py
+-rw-r--r--   0        0        0     5087 2023-04-06 19:54:36.493584 maxbot-0.1.0b0.dev20230417183114/maxbot/dialog_manager.py
+-rw-r--r--   0        0        0    10096 2023-04-13 11:42:37.915305 maxbot-0.1.0b0.dev20230417183114/maxbot/errors.py
+-rw-r--r--   0        0        0      139 2023-04-06 19:54:36.493703 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/__init__.py
+-rw-r--r--   0        0        0     4185 2023-04-06 19:54:36.493777 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/_manager.py
+-rw-r--r--   0        0        0     2738 2023-04-06 19:54:36.493894 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/datetime.py
+-rw-r--r--   0        0        0     2568 2023-04-06 19:54:36.494005 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/format.py
+-rw-r--r--   0        0        0     1043 2023-04-06 19:54:36.494122 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/jinja_loader.py
+-rw-r--r--   0        0        0     5515 2023-04-06 19:54:36.494243 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/rasa.py
+-rw-r--r--   0        0        0     5592 2023-04-06 19:54:36.494389 maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/rest.py
+-rw-r--r--   0        0        0       33 2023-04-06 19:54:36.494500 maxbot-0.1.0b0.dev20230417183114/maxbot/flows/__init__.py
+-rw-r--r--   0        0        0     1189 2023-02-15 19:48:36.387288 maxbot-0.1.0b0.dev20230417183114/maxbot/flows/_base.py
+-rw-r--r--   0        0        0     2053 2023-04-06 19:54:36.494565 maxbot-0.1.0b0.dev20230417183114/maxbot/flows/dialog_flow.py
+-rw-r--r--   0        0        0    24789 2023-04-13 11:42:37.915461 maxbot-0.1.0b0.dev20230417183114/maxbot/flows/dialog_tree.py
+-rw-r--r--   0        0        0    12228 2023-04-13 11:42:37.915591 maxbot-0.1.0b0.dev20230417183114/maxbot/flows/slot_filling.py
+-rw-r--r--   0        0        0     7448 2023-04-13 11:42:37.915711 maxbot-0.1.0b0.dev20230417183114/maxbot/jinja_env.py
+-rw-r--r--   0        0        0     4603 2023-04-13 11:42:37.915831 maxbot-0.1.0b0.dev20230417183114/maxbot/markdown.py
+-rw-r--r--   0        0        0    20628 2023-04-06 19:54:36.495666 maxbot-0.1.0b0.dev20230417183114/maxbot/nlu.py
+-rw-r--r--   0        0        0    10536 2023-04-06 19:54:36.495773 maxbot-0.1.0b0.dev20230417183114/maxbot/resources.py
+-rw-r--r--   0        0        0     4728 2023-04-06 19:54:36.495920 maxbot-0.1.0b0.dev20230417183114/maxbot/rpc.py
+-rw-r--r--   0        0        0     8753 2023-04-13 11:42:37.915981 maxbot-0.1.0b0.dev20230417183114/maxbot/scenarios.py
+-rw-r--r--   0        0        0    16810 2023-04-13 11:42:37.916125 maxbot-0.1.0b0.dev20230417183114/maxbot/schemas.py
+-rw-r--r--   0        0        0     4164 2023-04-06 19:54:36.496507 maxbot-0.1.0b0.dev20230417183114/maxbot/state_store.py
+-rw-r--r--   0        0        0     1051 2023-04-06 19:54:36.496579 maxbot-0.1.0b0.dev20230417183114/maxbot/user_locks.py
+-rw-r--r--   0        0        0    14851 2023-04-13 11:42:37.916226 maxbot-0.1.0b0.dev20230417183114/maxbot/xml.py
+-rw-r--r--   0        0        0     1596 2023-04-17 15:31:14.985381 maxbot-0.1.0b0.dev20230417183114/pyproject.toml
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 maxbot-0.1.0b0.dev20230417183114/setup.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 maxbot-0.1.0b0.dev20230417183114/PKG-INFO
```

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/_download.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/_download.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/_hooks.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/_hooks.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/bot.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/bot.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/builder.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/builder.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/channels/_manager.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/channels/_manager.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/channels/facebook.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/channels/facebook.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/channels/telegram.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/channels/viber.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/channels/viber.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/channels/vk.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/channels/vk.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_bot.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_bot.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_journal.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_journal.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_logging.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_logging.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_ngrok.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_ngrok.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/cli/_rich.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/cli/_rich.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/cli/run.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/cli/run.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/context.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/context.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/dialog_manager.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/dialog_manager.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/errors.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/errors.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/_manager.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/_manager.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/datetime.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/datetime.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/format.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/format.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/jinja_loader.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/jinja_loader.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/rasa.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/rasa.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/extensions/rest.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/flows/_base.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/flows/_base.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/flows/dialog_flow.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/flows/dialog_flow.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/flows/dialog_tree.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/flows/dialog_tree.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/flows/slot_filling.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/flows/slot_filling.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/jinja_env.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/jinja_env.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/markdown.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/markdown.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/nlu.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/nlu.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/resources.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/resources.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/rpc.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/rpc.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/scenarios.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/scenarios.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/schemas.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/schemas.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/state_store.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/state_store.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/user_locks.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/user_locks.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/maxbot/xml.py` & `maxbot-0.1.0b0.dev20230417183114/maxbot/xml.py`

 * *Files identical despite different names*

### Comparing `maxbot-0.1.0b0.dev20230417182950/pyproject.toml` & `maxbot-0.1.0b0.dev20230417183114/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Maxbot"
-version = "0.1.0b.dev20230417182950"
+version = "0.1.0b.dev20230417183114"
 description = "Maxbot is an open source library and framework for creating conversational apps."
 authors = ["Maxbot team <hello@maxbot.ai>"]
 
 [tool.poetry.scripts]
 maxbot = "maxbot.cli:main"
 
 [tool.poetry.dependencies]
```

### Comparing `maxbot-0.1.0b0.dev20230417182950/setup.py` & `maxbot-0.1.0b0.dev20230417183114/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'viberbot>=1.0,<2.0']
 
 entry_points = \
 {'console_scripts': ['maxbot = maxbot.cli:main']}
 
 setup_kwargs = {
     'name': 'maxbot',
-    'version': '0.1.0b0.dev20230417182950',
+    'version': '0.1.0b0.dev20230417183114',
     'description': 'Maxbot is an open source library and framework for creating conversational apps.',
     'long_description': 'None',
     'author': 'Maxbot team',
     'author_email': 'hello@maxbot.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `maxbot-0.1.0b0.dev20230417182950/PKG-INFO` & `maxbot-0.1.0b0.dev20230417183114/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxbot
-Version: 0.1.0b0.dev20230417182950
+Version: 0.1.0b0.dev20230417183114
 Summary: Maxbot is an open source library and framework for creating conversational apps.
 Author: Maxbot team
 Author-email: hello@maxbot.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

