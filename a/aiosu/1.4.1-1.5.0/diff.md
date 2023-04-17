# Comparing `tmp/aiosu-1.4.1.tar.gz` & `tmp/aiosu-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosu-1.4.1.tar", max compression
+gzip compressed data, was "aiosu-1.5.0.tar", max compression
```

## Comparing `aiosu-1.4.1.tar` & `aiosu-1.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    35149 2023-03-19 13:43:48.454782 aiosu-1.4.1/LICENSE
--rw-r--r--   0        0        0     3855 2023-03-19 13:43:48.454782 aiosu-1.4.1/README.rst
--rw-r--r--   0        0        0      675 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/__init__.py
--rw-r--r--   0        0        0     2318 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/events.py
--rw-r--r--   0        0        0      736 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/exceptions.py
--rw-r--r--   0        0        0     1790 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/helpers.py
--rw-r--r--   0        0        0      664 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/__init__.py
--rw-r--r--   0        0        0     1112 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/artist.py
--rw-r--r--   0        0        0      406 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/backgrounds.py
--rw-r--r--   0        0        0      883 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/base.py
--rw-r--r--   0        0        0    13819 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/beatmap.py
--rw-r--r--   0        0        0     1954 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/changelog.py
--rw-r--r--   0        0        0     1639 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/chat.py
--rw-r--r--   0        0        0     1519 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/comment.py
--rw-r--r--   0        0        0     2280 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/common.py
--rw-r--r--   0        0        0     1624 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/event.py
--rw-r--r--   0        0        0     1633 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/forum.py
--rw-r--r--   0        0        0     1976 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/gamemode.py
--rw-r--r--   0        0        0      742 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/kudosu.py
--rw-r--r--   0        0        0     5058 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/lazer.py
--rw-r--r--   0        0        0       79 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/legacy/__init__.py
--rw-r--r--   0        0        0     3123 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/legacy/match.py
--rw-r--r--   0        0        0      272 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/legacy/replay.py
--rw-r--r--   0        0        0     6076 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/mods.py
--rw-r--r--   0        0        0     4487 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/multiplayer.py
--rw-r--r--   0        0        0     1038 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/news.py
--rw-r--r--   0        0        0     1808 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/oauthtoken.py
--rw-r--r--   0        0        0      843 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/performance.py
--rw-r--r--   0        0        0      672 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/rankings.py
--rw-r--r--   0        0        0     2845 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/replay.py
--rw-r--r--   0        0        0     1312 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/scopes.py
--rw-r--r--   0        0        0     7512 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/score.py
--rw-r--r--   0        0        0      480 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/search.py
--rw-r--r--   0        0        0      387 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/spotlight.py
--rw-r--r--   0        0        0     8983 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/user.py
--rw-r--r--   0        0        0      372 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/models/wiki.py
--rw-r--r--   0        0        0      241 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/utils/__init__.py
--rw-r--r--   0        0        0     8815 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/utils/accuracy.py
--rw-r--r--   0        0        0     2936 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/utils/auth.py
--rw-r--r--   0        0        0     7905 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/utils/binary.py
--rw-r--r--   0        0        0    22091 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/utils/performance.py
--rw-r--r--   0        0        0     6091 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/utils/replay.py
--rw-r--r--   0        0        0      106 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v1/__init__.py
--rw-r--r--   0        0        0    17864 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v1/client.py
--rw-r--r--   0        0        0      154 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v2/__init__.py
--rw-r--r--   0        0        0    86348 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v2/client.py
--rw-r--r--   0        0        0     7691 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v2/clientstorage.py
--rw-r--r--   0        0        0      103 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v2/repository/__init__.py
--rw-r--r--   0        0        0     1905 2023-03-19 13:43:48.454782 aiosu-1.4.1/aiosu/v2/repository/oauthtoken.py
--rw-r--r--   0        0        0        0 2023-03-19 13:43:48.458782 aiosu-1.4.1/py.typed
--rw-r--r--   0        0        0     1825 2023-03-19 13:43:48.458782 aiosu-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 aiosu-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-17 12:54:11.518455 aiosu-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3855 2023-04-17 12:54:11.518455 aiosu-1.5.0/README.rst
+-rw-r--r--   0        0        0      675 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/__init__.py
+-rw-r--r--   0        0        0     2318 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/events.py
+-rw-r--r--   0        0        0      736 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/exceptions.py
+-rw-r--r--   0        0        0     1790 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/helpers.py
+-rw-r--r--   0        0        0      664 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/artist.py
+-rw-r--r--   0        0        0      406 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/backgrounds.py
+-rw-r--r--   0        0        0      883 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/base.py
+-rw-r--r--   0        0        0    13819 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/beatmap.py
+-rw-r--r--   0        0        0     1954 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/changelog.py
+-rw-r--r--   0        0        0     1639 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/chat.py
+-rw-r--r--   0        0        0     1519 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/comment.py
+-rw-r--r--   0        0        0     2280 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/common.py
+-rw-r--r--   0        0        0     1624 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/event.py
+-rw-r--r--   0        0        0     1633 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/forum.py
+-rw-r--r--   0        0        0     1976 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/gamemode.py
+-rw-r--r--   0        0        0      742 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/kudosu.py
+-rw-r--r--   0        0        0     5058 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/lazer.py
+-rw-r--r--   0        0        0       79 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/legacy/__init__.py
+-rw-r--r--   0        0        0     3123 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/legacy/match.py
+-rw-r--r--   0        0        0      272 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/legacy/replay.py
+-rw-r--r--   0        0        0     6076 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/mods.py
+-rw-r--r--   0        0        0     4487 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/multiplayer.py
+-rw-r--r--   0        0        0     1038 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/news.py
+-rw-r--r--   0        0        0     1808 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/oauthtoken.py
+-rw-r--r--   0        0        0      843 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/performance.py
+-rw-r--r--   0        0        0      672 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/rankings.py
+-rw-r--r--   0        0        0     2845 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/replay.py
+-rw-r--r--   0        0        0     1241 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/scopes.py
+-rw-r--r--   0        0        0     7512 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/score.py
+-rw-r--r--   0        0        0      480 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/search.py
+-rw-r--r--   0        0        0      387 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/spotlight.py
+-rw-r--r--   0        0        0     8983 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/user.py
+-rw-r--r--   0        0        0      372 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/wiki.py
+-rw-r--r--   0        0        0      241 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/__init__.py
+-rw-r--r--   0        0        0     8815 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/accuracy.py
+-rw-r--r--   0        0        0     2936 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/auth.py
+-rw-r--r--   0        0        0     7905 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/binary.py
+-rw-r--r--   0        0        0    22091 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/performance.py
+-rw-r--r--   0        0        0     6091 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/replay.py
+-rw-r--r--   0        0        0      106 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v1/__init__.py
+-rw-r--r--   0        0        0    17864 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v1/client.py
+-rw-r--r--   0        0        0      154 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/__init__.py
+-rw-r--r--   0        0        0    88480 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/client.py
+-rw-r--r--   0        0        0     7691 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/clientstorage.py
+-rw-r--r--   0        0        0      103 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/repository/__init__.py
+-rw-r--r--   0        0        0     1905 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/repository/oauthtoken.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:54:11.522456 aiosu-1.5.0/py.typed
+-rw-r--r--   0        0        0     1845 2023-04-17 12:54:11.522456 aiosu-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 aiosu-1.5.0/PKG-INFO
```

### Comparing `aiosu-1.4.1/LICENSE` & `aiosu-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/README.rst` & `aiosu-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/__init__.py` & `aiosu-1.5.0/aiosu/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/events.py` & `aiosu-1.5.0/aiosu/events.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/exceptions.py` & `aiosu-1.5.0/aiosu/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/helpers.py` & `aiosu-1.5.0/aiosu/helpers.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/__init__.py` & `aiosu-1.5.0/aiosu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/artist.py` & `aiosu-1.5.0/aiosu/models/artist.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/base.py` & `aiosu-1.5.0/aiosu/models/base.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/beatmap.py` & `aiosu-1.5.0/aiosu/models/beatmap.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/changelog.py` & `aiosu-1.5.0/aiosu/models/changelog.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/chat.py` & `aiosu-1.5.0/aiosu/models/chat.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/comment.py` & `aiosu-1.5.0/aiosu/models/comment.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/common.py` & `aiosu-1.5.0/aiosu/models/common.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/event.py` & `aiosu-1.5.0/aiosu/models/event.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/forum.py` & `aiosu-1.5.0/aiosu/models/forum.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/gamemode.py` & `aiosu-1.5.0/aiosu/models/gamemode.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/kudosu.py` & `aiosu-1.5.0/aiosu/models/kudosu.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/lazer.py` & `aiosu-1.5.0/aiosu/models/lazer.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/legacy/match.py` & `aiosu-1.5.0/aiosu/models/legacy/match.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/mods.py` & `aiosu-1.5.0/aiosu/models/mods.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/multiplayer.py` & `aiosu-1.5.0/aiosu/models/multiplayer.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/news.py` & `aiosu-1.5.0/aiosu/models/news.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/oauthtoken.py` & `aiosu-1.5.0/aiosu/models/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/performance.py` & `aiosu-1.5.0/aiosu/models/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/rankings.py` & `aiosu-1.5.0/aiosu/models/rankings.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/replay.py` & `aiosu-1.5.0/aiosu/models/replay.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/scopes.py` & `aiosu-1.5.0/aiosu/models/scopes.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,25 @@
     "Scopes",
     "VALID_CLIENT_SCOPES",
 )
 
 
 @unique
 class Scopes(IntFlag):
-    PUBLIC = 0
-    IDENTIFY = 1 << 0
-    FRIENDS_READ = 1 << 1
-    FORUM_WRITE = 1 << 2
-    DELEGATE = 1 << 3
-    CHAT_WRITE = 1 << 4
-    LAZER = 1 << 5  # unused, lazer endpoints are not planned for support
+    NONE = 0
+    PUBLIC = 1 << 0
+    IDENTIFY = 1 << 1
+    FRIENDS_READ = 1 << 2
+    FORUM_WRITE = 1 << 3
+    DELEGATE = 1 << 4
+    CHAT_WRITE = 1 << 5
+    LAZER = 1 << 6  # unused, lazer endpoints are not planned for support
 
     def __flags__(self) -> list[Scopes]:
         scopes_list = [scope for scope in Scopes if self & scope]
-        if self.PUBLIC not in scopes_list:
-            scopes_list.append(Scopes.PUBLIC)
         return scopes_list
 
     def __str__(self) -> str:
         return " ".join(
             scope_name
             for scope_name, scope in API_SCOPE_NAMES.items()
             if scope in self.__flags__()
```

### Comparing `aiosu-1.4.1/aiosu/models/score.py` & `aiosu-1.5.0/aiosu/models/score.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/models/user.py` & `aiosu-1.5.0/aiosu/models/user.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/utils/accuracy.py` & `aiosu-1.5.0/aiosu/utils/accuracy.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/utils/auth.py` & `aiosu-1.5.0/aiosu/utils/auth.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/utils/binary.py` & `aiosu-1.5.0/aiosu/utils/binary.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/utils/performance.py` & `aiosu-1.5.0/aiosu/utils/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/utils/replay.py` & `aiosu-1.5.0/aiosu/utils/replay.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/v1/client.py` & `aiosu-1.5.0/aiosu/v1/client.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/v2/client.py` & `aiosu-1.5.0/aiosu/v2/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -349,25 +349,24 @@
     async def _refresh(self) -> None:
         r"""INTERNAL: Refreshes the client's token
 
         :raises APIException: Contains status code and error message
         """
         old_token = await self.get_current_token()
         url = f"{self.base_url}/oauth/token"
-        headers = {"Content-Type": "application/x-www-form-urlencoded"}
 
         data = {}
         if old_token.can_refresh:
             data = await self._refresh_auth_data()
         else:
             data = self._refresh_guest_data()
 
-        async with aiohttp.ClientSession(headers=headers) as temp_session:
+        async with aiohttp.ClientSession() as temp_session:
             async with self._limiter:
-                async with temp_session.post(url, data=data) as resp:
+                async with temp_session.post(url, json=data) as resp:
                     try:
                         body = await resp.read()
                         content_type = get_content_type(
                             resp.headers.get("content-type", ""),
                         )
                         if content_type != "application/json":
                             raise APIException(
@@ -678,14 +677,15 @@
         if resp.cursor_string:  # Unused: API does not return cursor_string
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_comments, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def search(self, query: str, **kwargs: Any) -> SearchResponse:
         r"""Searches for a user, beatmap, beatmapset, or wiki page.
 
         :param query: The query to search for
         :type query: str
         :param \**kwargs:
             See below
@@ -707,15 +707,15 @@
         }
         add_param(params, kwargs, key="page")
         json = await self._request("GET", url, params=params)
         return SearchResponse.parse_obj(json)
 
     @prepare_token
     @check_token
-    @requires_scope(Scopes.IDENTIFY)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_me(self, **kwargs: Any) -> User:
         r"""Gets the user who owns the current token
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -732,27 +732,29 @@
             url += f"/{mode}"
         json = await self._request("GET", url)
         return User.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FRIENDS_READ)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_own_friends(self) -> list[User]:
         r"""Gets the token owner's friend list
 
         :raises APIException: Contains status code and error message
         :return: List of friends
         :rtype: list[aiosu.models.user.User]
         """
         url = f"{self.base_url}/api/v2/friends"
         json = await self._request("GET", url)
         return from_list(User.parse_obj, json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_user(self, user_query: Union[str, int], **kwargs: Any) -> User:
         r"""Gets a user by a query.
 
         :param user_query: Username or ID to search by
         :type user_query: Union[str, int]
         :param \**kwargs:
             See below
@@ -780,14 +782,15 @@
             converter=lambda x: UserQueryType(x).new_api_name,
         )
         json = await self._request("GET", url, params=params)
         return User.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_users(self, user_ids: list[int]) -> list[User]:
         r"""Get multiple user data.
 
         :param user_ids: The IDs of the users
         :type user_ids: list[int]
         :raises APIException: Contains status code and error message
         :return: List of user data objects
@@ -798,14 +801,15 @@
             "ids": user_ids,
         }
         json = await self._request("GET", url, params=params)
         return from_list(User.parse_obj, json.get("users", []))
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_user_kudosu(self, user_id: int, **kwargs: Any) -> list[KudosuHistory]:
         r"""Get a user's kudosu history.
 
         :param user_id: User ID to search by
         :type user_id: int
         :param \**kwargs:
             See below
@@ -825,14 +829,15 @@
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
         return from_list(KudosuHistory.parse_obj, json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def __get_type_scores(
         self, user_id: int, request_type: str, **kwargs: Any
     ) -> list[Union[Score, LazerScore]]:
         r"""INTERNAL: Get a user's scores by type
 
         :param user_id: User ID to search by
         :type user_id: int
@@ -959,14 +964,15 @@
         :return: List of requested scores
         :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
         """
         return await self.__get_type_scores(user_id, "firsts", **kwargs)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_user_beatmap_scores(
         self, user_id: int, beatmap_id: int, **kwargs: Any
     ) -> list[Score]:
         r"""Get a user's scores on a specific beatmap.
 
         :param user_id: User ID to search by
         :type user_id: int
@@ -989,14 +995,15 @@
         json = await self._request("GET", url, params=params)
         return from_list(Score.parse_obj, json.get("scores", []))
 
     UserBeatmapType = Literal["favourite", "graveyard", "loved", "ranked", "pending"]
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_user_beatmaps(
         self, user_id: int, type: UserBeatmapType, **kwargs: Any
     ) -> list[Beatmapset]:
         r"""Get a user's beatmaps.
 
         :param user_id: ID of the user
         :type user_id: int
@@ -1020,14 +1027,15 @@
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
         return from_list(Beatmapset.parse_obj, json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_user_most_played(
         self, user_id: int, **kwargs: Any
     ) -> list[BeatmapUserPlaycount]:
         r"""Get a user's most played beatmaps.
 
         :param user_id: ID of the user
         :type user_id: int
@@ -1049,14 +1057,15 @@
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
         return from_list(BeatmapUserPlaycount.parse_obj, json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_user_recent_activity(
         self, user_id: int, **kwargs: Any
     ) -> list[Event]:
         r"""Get a user's recent activity.
 
         :param user_id: ID of the user
         :type user_id: int
@@ -1078,14 +1087,15 @@
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
         return from_list(Event.parse_obj, json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmap_scores(self, beatmap_id: int, **kwargs: Any) -> list[Score]:
         r"""Get scores submitted on a specific beatmap.
 
         :param beatmap_id: Beatmap ID to search by
         :type beatmap_id: int
         :param \**kwargs:
             See below
@@ -1108,14 +1118,15 @@
         add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
         add_param(params, kwargs, key="type")
         json = await self._request("GET", url, params=params)
         return from_list(Score.parse_obj, json.get("scores", []))
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmap(self, beatmap_id: int) -> Beatmap:
         r"""Get beatmap data.
 
         :param beatmap_id: The ID of the beatmap
         :type beatmap_id: int
         :raises APIException: Contains status code and error message
         :return: Beatmap data object
@@ -1123,14 +1134,15 @@
         """
         url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}"
         json = await self._request("GET", url)
         return Beatmap.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmaps(self, beatmap_ids: list[int]) -> list[Beatmap]:
         r"""Get multiple beatmap data.
 
         :param beatmap_ids: The IDs of the beatmaps
         :type beatmap_ids: list[int]
         :raises APIException: Contains status code and error message
         :return: List of beatmap data objects
@@ -1141,14 +1153,15 @@
             "ids": beatmap_ids,
         }
         json = await self._request("GET", url, params=params)
         return from_list(Beatmap.parse_obj, json.get("beatmaps", []))
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def lookup_beatmap(self, **kwargs: Any) -> Beatmap:
         r"""Lookup beatmap data.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -1172,14 +1185,15 @@
         if not params:
             raise ValueError("One of checksum, filename or id must be provided.")
         json = await self._request("GET", url, params=params)
         return Beatmap.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmap_attributes(
         self, beatmap_id: int, **kwargs: Any
     ) -> BeatmapDifficultyAttributes:
         r"""Gets difficulty attributes for a beatmap.
 
         :param beatmap_id: The ID of the beatmap
         :type beatmap_id: int
@@ -1207,14 +1221,15 @@
         )
         add_param(data, kwargs, key="mods", converter=lambda x: int(Mods(x)))
         json = await self._request("POST", url, json=data)
         return BeatmapDifficultyAttributes.parse_obj(json.get("attributes"))
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset(self, beatmapset_id: int) -> Beatmapset:
         r"""Get beatmapset data.
 
         :param beatmapset_id: The ID of the beatmapset
         :type beatmapset_id: int
         :raises APIException: Contains status code and error message
         :return: Beatmapset data object
@@ -1222,14 +1237,15 @@
         """
         url = f"{self.base_url}/api/v2/beatmapsets/{beatmapset_id}"
         json = await self._request("GET", url)
         return Beatmapset.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def lookup_beatmapset(self, beatmap_id: int) -> Beatmapset:
         r"""Lookup beatmap data.
 
         :param beatmap_id: The ID of a beatmap in the set
         :type beatmap_id: int
 
         :raises APIException: Contains status code and error message
@@ -1241,14 +1257,15 @@
             "beatmap_id": beatmap_id,
         }
         json = await self._request("GET", url, params=params)
         return Beatmapset.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def search_beatmapsets(
         self,
         search_filter: Optional[str] = "",
         **kwargs: Any,
     ) -> BeatmapsetSearchResponse:
         r"""Search beatmapset by filter.
 
@@ -1273,14 +1290,15 @@
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.search_beatmapsets, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_events(self, **kwargs: Any) -> list[BeatmapsetEvent]:
         r"""Get beatmapset events.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -1310,14 +1328,15 @@
         add_param(params, kwargs, key="max_date")
         add_param(params, kwargs, key="types")
         json = await self._request("GET", url, params=params)
         return from_list(BeatmapsetEvent.parse_obj, json.get("events", []))
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_discussions(
         self, **kwargs: Any
     ) -> BeatmapsetDiscussionResponse:
         r"""Get beatmapset discussions.
 
         :param \**kwargs:
             See below
@@ -1368,14 +1387,15 @@
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_beatmapset_discussions, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_discussion_posts(
         self, **kwargs: Any
     ) -> BeatmapsetDiscussionPostResponse:
         r"""Get beatmapset discussion posts.
 
         :param \**kwargs:
             See below
@@ -1417,14 +1437,15 @@
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_beatmapset_discussion_posts, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_discussion_votes(
         self, **kwargs: Any
     ) -> BeatmapsetDiscussionVoteResponse:
         r"""Get beatmapset discussion votes.
 
         :param \**kwargs:
             See below
@@ -1469,14 +1490,15 @@
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_beatmapset_discussion_votes, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_score(
         self,
         score_id: int,
         mode: Gamemode,
     ) -> Score:
         r"""Gets data about a score.
 
@@ -1491,14 +1513,15 @@
         """
         url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}"
         json = await self._request("GET", url)
         return Score.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_score_replay(
         self,
         score_id: int,
         mode: Gamemode,
     ) -> BytesIO:
         r"""Gets the replay file for a score.
@@ -1513,14 +1536,15 @@
         :rtype: io.BytesIO
         """
         url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}/download"
         return await self._request("GET", url)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_rankings(
         self, mode: Gamemode, type: RankingType, **kwargs: Any
     ) -> Rankings:
         r"""Get rankings.
 
         :param mode: The gamemode to search for
         :type mode: aiosu.models.gamemode.Gamemode
@@ -1557,27 +1581,29 @@
         if resp.cursor_string:  # Unused: API does not return cursor_string
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_rankings, mode=mode, type=type, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_spotlights(self) -> list[Spotlight]:
         r"""Gets the current spotlights.
 
         :raises APIException: Contains status code and error message
         :return: List of spotlights
         :rtype: list[aiosu.models.spotlight.Spotlight]
         """
         url = f"{self.base_url}/api/v2/spotlights"
         json = await self._request("GET", url)
         return from_list(Spotlight.parse_obj, json.get("spotlights", []))
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_forum_topic(self, topic_id: int, **kwargs: Any) -> ForumTopicResponse:
         r"""Gets a forum topic.
 
         :param topic_id: The ID of the topic
         :type topic_id: int
         :param \**kwargs:
             See below
@@ -1614,14 +1640,15 @@
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_forum_topic, topic_id, **kwargs)
         return resp
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FORUM_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def create_forum_topic(
         self, forum_id: int, title: str, content: str, **kwargs: Any
     ) -> ForumCreateTopicResponse:
         r"""Creates a forum topic.
 
         :param forum_id: The ID of the forum to create the topic in
         :type forum_id: int
@@ -1676,14 +1703,15 @@
             data["forum_topic_poll"] = forum_topic_poll
         json = await self._request("POST", url, json=data)
         return ForumCreateTopicResponse.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FORUM_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def reply_forum_topic(self, topic_id: int, content: str) -> ForumPost:
         r"""Replies to a forum topic.
 
         :param topic_id: The ID of the topic
         :type topic_id: int
         :param content: The content of the post
         :type content: str
@@ -1741,14 +1769,15 @@
         }
         json = await self._request("PUT", url, json=data)
         return ForumPost.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_chat_ack(self, **kwargs: Any) -> list[ChatUserSilence]:
         r"""Gets chat acknowledgement.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -1767,14 +1796,15 @@
         add_param(data, kwargs, key="silence_id_since", param_name="history_since")
         json = await self._request("POST", url, json=data)
         return from_list(ChatUserSilence.parse_obj, json.get("silences", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_chat_updates(self, since: int, **kwargs: Any) -> ChatUpdateResponse:
         r"""Gets chat updates.
 
         :param since: The last message ID received
         :type since: int
         :param \**kwargs:
             See below
@@ -1806,14 +1836,15 @@
         add_param(params, kwargs, key="silence_id_since", param_name="history_since")
         json = await self._request("GET", url, params=params)
         return ChatUpdateResponse.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_channel(self, channel_id: int) -> ChatChannelResponse:
         r"""Gets channel.
 
         :param channel_id: The channel ID to get
         :type channel_id: int
         :raises APIException: Contains status code and error message
         :return: Chat channel object
@@ -1822,28 +1853,30 @@
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}"
         json = await self._request("GET", url)
         return ChatChannelResponse.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_channels(self) -> list[ChatChannel]:
         r"""Gets a list of joinable public channels.
 
         :raises APIException: Contains status code and error message
         :return: List of chat channel objects
         :rtype: list[aiosu.models.chat.ChatChannel]
         """
         url = f"{self.base_url}/api/v2/chat/channels"
         json = await self._request("GET", url)
         return from_list(ChatChannel.parse_obj, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_channel_messages(
         self, channel_id: int, **kwargs: Any
     ) -> list[ChatMessage]:
         r"""Gets channel messages.
 
         :param channel_id: The channel ID to get messages from
         :type channel_id: int
@@ -1873,14 +1906,15 @@
         add_param(params, kwargs, key="until")
         json = await self._request("GET", url, params=params)
         return from_list(ChatMessage.parse_obj, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.CHAT_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def create_chat_channel(
         self, type: ChatChannelTypes, **kwargs: Any
     ) -> ChatChannel:
         r"""Creates a chat channel.
 
         :param type: The type of the channel.
         :type type: aiosu.models.chat.ChatChannelType
@@ -1924,14 +1958,15 @@
             data["channel"] = channel
         json = await self._request("POST", url, json=data)
         return ChatChannel.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def join_channel(self, channel_id: int, user_id: int) -> ChatChannel:
         r"""Joins a channel.
 
         :param channel_id: The channel ID to join
         :type channel_id: int
         :param user_id: The user ID to join as
         :type user_id: int
@@ -1942,14 +1977,15 @@
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
         json = await self._request("PUT", url)
         return ChatChannel.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def leave_channel(self, channel_id: int, user_id: int) -> None:
         r"""Leaves a channel.
 
         :param channel_id: The channel ID to leave
         :type channel_id: int
         :param user_id: The user ID to leave as
         :type user_id: int
@@ -1957,14 +1993,15 @@
         """
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
         await self._request("DELETE", url)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def mark_read(self, channel_id: int, message_id: int) -> None:
         r"""Marks a channel as read.
 
         :param channel_id: The channel ID to mark as read
         :type channel_id: int
         :param message_id: The message ID to mark as read up to
         :type message_id: int
@@ -1972,14 +2009,15 @@
         """
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/mark-as-read/{message_id}"
         await self._request("PUT", url)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def send_message(
         self,
         channel_id: int,
         message: str,
         is_action: bool,
     ) -> ChatMessage:
         r"""Sends a message to a channel.
@@ -2001,14 +2039,15 @@
         }
         json = await self._request("POST", url, json=data)
         return ChatMessage.parse_obj(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.CHAT_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def send_private_message(
         self, user_id: int, message: str, is_action: bool, **kwargs: Any
     ) -> ChatMessageCreateResponse:
         r"""Sends a message to a user.
 
         :param user_id: The ID of the user
         :type user_id: int
@@ -2035,14 +2074,15 @@
         }
         add_param(data, kwargs, key="uuid")
         json = await self._request("POST", url, json=data)
         return ChatMessageCreateResponse.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_matches(
         self, **kwargs: Any
     ) -> MultiplayerMatchesResponse:
         r"""Gets the multiplayer matches.
 
         :param \**kwargs:
             See below
@@ -2072,14 +2112,15 @@
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_multiplayer_matches, **kwargs)
         return resp
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_match(
         self, match_id: int, **kwargs: Any
     ) -> MultiplayerMatchResponse:
         r"""Gets a multiplayer match.
 
         :param match_id: The ID of the match
         :type match_id: int
@@ -2108,14 +2149,16 @@
         add_param(params, kwargs, key="before")
         add_param(params, kwargs, key="after")
         json = await self._request("GET", url)
         return MultiplayerMatchResponse.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_multiplayer_rooms(self, **kwargs: Any) -> list[MultiplayerRoom]:
         r"""Gets the multiplayer rooms.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -2148,14 +2191,15 @@
         add_param(params, kwargs, key="category")
         add_param(params, kwargs, key="type", param_name="type_group")
         json = await self._request("GET", url, params=params)
         return from_list(MultiplayerRoom.parse_obj, json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_room(self, room_id: int) -> MultiplayerRoom:
         r"""Gets a multiplayer room.
 
         :param room_id: The ID of the room
         :type room_id: int
 
         :raises APIException: Contains status code and error message
@@ -2164,14 +2208,16 @@
         """
         url = f"{self.base_url}/api/v2/rooms/{room_id}"
         json = await self._request("GET", url)
         return MultiplayerRoom.parse_obj(json)
 
     @prepare_token
     @check_token
+    @requires_scope(Scopes.PUBLIC)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_multiplayer_leaderboard(
         self, room_id: int, **kwargs: Any
     ) -> MultiplayerLeaderboardResponse:
         r"""Gets the multiplayer leaderboard for a room.
 
         :param room_id: The ID of the room
         :type room_id: int
@@ -2194,15 +2240,15 @@
             "limit": limit,
         }
         json = await self._request("GET", url, params=params)
         return MultiplayerLeaderboardResponse.parse_obj(json)
 
     @prepare_token
     @check_token
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_scores(
         self, room_id: int, playlist_id: int, **kwargs: Any
     ) -> MultiplayerScoresResponse:
         r"""Gets the multiplayer scores for a room.
 
         :param room_id: The ID of the room
         :type room_id: int
```

### Comparing `aiosu-1.4.1/aiosu/v2/clientstorage.py` & `aiosu-1.5.0/aiosu/v2/clientstorage.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/aiosu/v2/repository/oauthtoken.py` & `aiosu-1.5.0/aiosu/v2/repository/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.4.1/pyproject.toml` & `aiosu-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 files = ["aiosu"]
 disallow_untyped_defs = true
 disallow_any_unimported = true
 no_implicit_optional = true
 check_untyped_defs = true
 warn_unused_ignores = true
 show_error_codes = true
-
 [tools.pytest.ini_options]
 testpaths = ["tests"]
-
 [tool.poetry]
 name = "aiosu"
-version = "1.4.1"
+version = "1.5.0"
 description = "Simple and fast osu! API v1 and v2 library"
 authors = ["Nice Aesthetics <nice@aesth.dev>"]
 license = "GPLv3+"
 readme = "README.rst"
 repository = "https://github.com/NiceAesth/aiosu"
 documentation = "https://aiosu.readthedocs.io/"
 keywords = ["osu!", "osu", "api"]
@@ -52,14 +50,15 @@
 mypy = "^1.0"
 toml = "^0.10.2"
 types-toml = "^0.10.8.1"
 sphinx = "^6.0.0"
 sphinx-rtd-theme = "^1.2.0"
 pytest-cov = "^4.0.0"
 black = {version = "^23.0.0", allow-prereleases = true}
+pre-commit = "^3.2.2"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-asyncio", "pytest-mock", "toml", "types-toml"]
 docs = ["Sphinx", "sphinx-rtd-theme", "toml"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `aiosu-1.4.1/PKG-INFO` & `aiosu-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosu
-Version: 1.4.1
+Version: 1.5.0
 Summary: Simple and fast osu! API v1 and v2 library
 Home-page: https://github.com/NiceAesth/aiosu
 License: GPLv3+
 Keywords: osu!,osu,api
 Author: Nice Aesthetics
 Author-email: nice@aesth.dev
 Requires-Python: >=3.9,<4.0
```

