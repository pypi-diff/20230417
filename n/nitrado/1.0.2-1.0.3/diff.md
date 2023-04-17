# Comparing `tmp/nitrado-1.0.2.tar.gz` & `tmp/nitrado-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.2.tar", last modified: Sun Apr 16 10:27:27 2023, max compression
+gzip compressed data, was "nitrado-1.0.3.tar", last modified: Mon Apr 17 02:44:25 2023, max compression
```

## Comparing `nitrado-1.0.2.tar` & `nitrado-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.723296 nitrado-1.0.2/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3435 2023-04-16 10:27:27.724299 nitrado-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.2/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1135 2023-04-16 10:27:27.729295 nitrado-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.691856 nitrado-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.699283 nitrado-1.0.2/src/nitrado/
--rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.2/src/nitrado/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-25 08:45:32.000000 nitrado-1.0.2/src/nitrado/ark_server.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.717295 nitrado-1.0.2/src/nitrado/lib/
--rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.2/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.2/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0    21890 2023-04-16 09:32:56.000000 nitrado-1.0.2/src/nitrado/lib/game_server.py
--rw-rw-rw-   0        0        0     3887 2023-04-16 10:26:22.000000 nitrado-1.0.2/src/nitrado/lib/service.py
--rw-rw-rw-   0        0        0     2836 2023-04-16 10:18:35.000000 nitrado-1.0.2/src/nitrado/nitrado_api.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.2/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.719295 nitrado-1.0.2/src/nitrado/tools/
--rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.2/src/nitrado/tools/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.2/src/nitrado/tools/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.713300 nitrado-1.0.2/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     3435 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.722297 nitrado-1.0.2/tests/
--rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.2/tests/test_connection.py
--rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.2/tests/test_game_server.py
--rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.2/tests/test_nitrado_api.py
--rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.2/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.132794 nitrado-1.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3435 2023-04-17 02:44:25.132794 nitrado-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.3/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1135 2023-04-17 02:44:25.137796 nitrado-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.099798 nitrado-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.106793 nitrado-1.0.3/src/nitrado/
+-rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.3/src/nitrado/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.123794 nitrado-1.0.3/src/nitrado/games/
+-rw-rw-rw-   0        0        0        0 2023-04-16 22:12:29.000000 nitrado-1.0.3/src/nitrado/games/__init__.py
+-rw-rw-rw-   0        0        0     3454 2023-04-17 02:38:37.000000 nitrado-1.0.3/src/nitrado/games/ark_survival.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.126794 nitrado-1.0.3/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.3/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.3/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0    22391 2023-04-17 02:38:37.000000 nitrado-1.0.3/src/nitrado/lib/game_server.py
+-rw-rw-rw-   0        0        0     3889 2023-04-17 00:46:43.000000 nitrado-1.0.3/src/nitrado/lib/service.py
+-rw-rw-rw-   0        0        0     3156 2023-04-17 01:07:27.000000 nitrado-1.0.3/src/nitrado/nitrado_api.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.3/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.128795 nitrado-1.0.3/src/nitrado/tools/
+-rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.3/src/nitrado/tools/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.3/src/nitrado/tools/client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.121793 nitrado-1.0.3/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3435 2023-04-17 02:44:25.000000 nitrado-1.0.3/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2023-04-17 02:44:25.000000 nitrado-1.0.3/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:44:25.000000 nitrado-1.0.3/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-17 02:44:25.000000 nitrado-1.0.3/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 02:44:25.000000 nitrado-1.0.3/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 02:44:25.131795 nitrado-1.0.3/tests/
+-rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.3/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.3/tests/test_game_server.py
+-rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.3/tests/test_nitrado_api.py
+-rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.3/tests/test_service.py
```

### Comparing `nitrado-1.0.2/LICENSE` & `nitrado-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/PKG-INFO` & `nitrado-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.2
+Version: 1.0.3
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
```

### Comparing `nitrado-1.0.2/README.md` & `nitrado-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/pyproject.toml` & `nitrado-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/setup.cfg` & `nitrado-1.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 320d 0a74 6573  ion = 1.0.2..tes
+00000020: 696f 6e20 3d20 312e 302e 330d 0a74 6573  ion = 1.0.3..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
-00000040: 330d 0a70 726f 6475 6374 696f 6e5f 7665  3..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 320d 0a61  rsion = 1.0.2..a
+00000040: 340d 0a70 726f 6475 6374 696f 6e5f 7665  4..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 330d 0a61  rsion = 1.0.3..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
```

### Comparing `nitrado-1.0.2/src/nitrado/lib/errors.py` & `nitrado-1.0.3/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/src/nitrado/lib/game_server.py` & `nitrado-1.0.3/src/nitrado/lib/game_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from nitrado.lib.errors import assert_response_is_ok
+from nitrado.lib.service import Service
 from nitrado.tools import Client
 import requests
 from pathlib import Path
 import json
 
 
 class GameServer:
@@ -38,41 +39,49 @@
         self.credentials = None
         self.settings = None
         self.quota = None
         self.query = None
         for k, v in data.items():
             self.__dict__[k] = v
 
+    def service(self) -> Service:
+        response = self.__client.get(path=f'/services/{self.service_id}')
+        data: dict = response.json()['data']
+        return Service(self.__client, data['service'])
+
     def cluster_id(self) -> str:
         path = f'/services/{self.service_id}/gameservers/games/arkse/gen_cluster_id'
         response = self.__client.get(path=path)
         data: dict = response.json()['data']
         return data['clusterid']
 
     def logs_shooter_game(self) -> str:
+        """ Refreshes about every 15+/- minutes """
         path = f'/services/{self.service_id}/gameservers/file_server/download'
         params = {'file': f"/games/{self.username}/noftp/arkxb/ShooterGame/Saved/Logs/ShooterGame.log"}
         response = self.__client.get(path=path, params=params)
         data: dict = response.json()['data']
         url = data['token']['url']
         log_response = requests.get(url)
         assert_response_is_ok(log_response)
         return log_response.text.replace("\r\n", "\n")
 
     def logs_restart(self) -> str:
+        """ Refreshes about every 15+/- minutes """
         path = f'/services/{self.service_id}/gameservers/file_server/download'
         params = {'file': f"/games/{self.username}/ftproot/restart.log"}
         response = self.__client.get(path=path, params=params)
         data: dict = response.json()['data']
         url = data['token']['url']
         log_response = requests.get(url)
         assert_response_is_ok(log_response)
         return log_response.text.replace("\r\n", "\n")
 
     def logs_shooter_game_last(self) -> str:
+        """ Refreshes about every 15+/- minutes """
         path = f'/services/{self.service_id}/gameservers/file_server/download'
         params = {'file': f"/games/{self.username}/noftp/arkxb/ShooterGame/Saved/Logs/ShooterGame_Last.log"}
         response = self.__client.get(path=path, params=params)
         data: dict = response.json()['data']
         url = data['token']['url']
         log_response = requests.get(url)
         assert_response_is_ok(log_response)
@@ -85,15 +94,16 @@
         with open(location / Path('shooter_games.txt'), 'w') as w:
             w.write(self.logs_shooter_game())
         with open(location / Path('shooter_games_last.txt'), 'w') as w:
             w.write(self.logs_shooter_game_last())
         with open(location / Path('restart.txt'), 'w') as w:
             w.write(self.logs_restart())
 
-    def start(self, game) -> bool:
+    def start(self, game: str) -> bool:
+        """ :param game: Provide the Folder Short of the specific game. """
         path = f'/services/{self.service_id}/gameservers/games/start'
         params = {'game': game}
         response = self.__client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def is_gameserver_restorable(self, folder, backup_id) -> bool:
@@ -152,15 +162,15 @@
 
     def players(self) -> list:
         path = f'/services/{self.service_id}/gameservers/games/players'
         response = self.__client.get(path=path)
         data: dict = response.json()['data']
         return data['players']
 
-    def white_list_player(self, gamertag) -> bool:
+    def white_list_player(self, gamertag: str) -> bool:
         """
         Player_Management - Add Player to Whitelist
         :param gamertag: Player unique identifier.
         """
         params = {"identifer": gamertag}
         path = f'/services/{self.service_id}/gameservers/games/whitelist'
         response = self.__client.put(path=path, params=params)
```

### Comparing `nitrado-1.0.2/src/nitrado/lib/service.py` & `nitrado-1.0.3/src/nitrado/lib/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         params = {'action_method': action_method, 'action_data': action_data, 'minute': minute,
                   'hour': hour, 'day': day, 'month': month, 'weekday': weekday}
         response = self.__client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def update_task(self, task_id=None, action_method=None, month="*", day="*", hour="*", minute="*", weekday="*", action_data=None) -> bool:
-        path = f'/services{self.id}/tasks/task_id'
+        path = f'/services{self.id}/tasks/{task_id}'
         params = {'action_method': action_method, 'action_data': action_data, 'minute': minute,
                   'hour': hour, 'day': day, 'month': month, 'weekday': weekday}
         response = self.__client.put(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def delete_task(self, task_id) -> bool:
```

### Comparing `nitrado-1.0.2/src/nitrado/nitrado_api.py` & `nitrado-1.0.3/src/nitrado/nitrado_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from nitrado.lib.errors import assert_response_is_ok, assert_response_is_json
 from nitrado.tools import Client
 from nitrado.lib import GameServer, Service
+from nitrado.games.ark_survival import ArkSurvival
 import requests
 import os
 
 
 class NitradoAPI:
     NITRADO_API_URL = "https://api.nitrado.net/"
 
@@ -25,49 +26,57 @@
     @classmethod
     def banned_list(cls) -> list:
         response = requests.get("http://arkdedicated.com/xboxbanlist.txt")
         assert_response_is_ok(response)
         return response.text.split('\r\n')
 
     def __init__(self, key: str = None, url: str = None):
-        self.client = Client(url or NitradoAPI.NITRADO_API_URL, key or os.getenv('NITRADO_KEY'))
+        self.__client = Client(url or NitradoAPI.NITRADO_API_URL, key or os.getenv('NITRADO_KEY'))
 
-    def services(self) -> list:
-        response = self.client.get(path='/services')
+    def services(self) -> list[Service]:
+        response = self.__client.get(path='/services')
         data: dict = response.json()['data']
         servers = data['services']
-        return [Service(self.client, data) for data in servers]
+        return [Service(self.__client, data) for data in servers]
 
-    def game_servers(self) -> list:
-        response = self.client.get(path='/services')
+    def game_servers(self) -> list[GameServer]:
+        response = self.__client.get(path='/services')
         data: dict = response.json()['data']
         service_ids = [service['id'] for service in data['services']]
         game_servers = []
         for id in service_ids:
             game_server = self.find_game_by_service_id(id)
             game_servers.append(game_server)
         return game_servers
-    
+
+    def ark_xbox_servers(self) -> list[ArkSurvival]:
+        games = []
+        for game in self.game_servers():
+            if game.game == 'arkxb':
+                games.append(ArkSurvival(game))
+        return games
+
     def find_game_by_service_id(self, service_id: str) -> GameServer:
-        response = self.client.get(path=f'/services/{service_id}/gameservers')
+        response = self.__client.get(path=f'/services/{service_id}/gameservers')
         data: dict = response.json()['data']
-        return GameServer(self.client, data['gameserver'])
+        return GameServer(self.__client, data['gameserver'])
 
     def find_service_by_id(self, service_id: str) -> Service:
-        response = self.client.get(path=f'/services/{service_id}')
+        response = self.__client.get(path=f'/services/{service_id}')
         data: dict = response.json()['data']
-        return Service(self.client, data['service'])
+        return Service(self.__client, data['service'])
 
     def health_check(self) -> bool:
-        response = self.client.get('/ping')
+        response = self.__client.get('/ping')
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def maintenance_status(self) -> dict:
-        response = self.client.get('/maintenance')
+        response = self.__client.get('/maintenance')
         data: dict = response.json()['data']
         return data['maintenance']
 
     def version(self) -> str:
-        response = self.client.get('/version')
+        response = self.__client.get('/version')
         data: dict = response.json()
         return data['message']
+
```

### Comparing `nitrado-1.0.2/src/nitrado/tools/client.py` & `nitrado-1.0.3/src/nitrado/tools/client.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.3/src/nitrado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.2
+Version: 1.0.3
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
```

### Comparing `nitrado-1.0.2/src/nitrado.egg-info/SOURCES.txt` & `nitrado-1.0.3/src/nitrado.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/nitrado/__init__.py
-src/nitrado/ark_server.py
 src/nitrado/nitrado_api.py
 src/nitrado/py.typed
 src/nitrado.egg-info/PKG-INFO
 src/nitrado.egg-info/SOURCES.txt
 src/nitrado.egg-info/dependency_links.txt
 src/nitrado.egg-info/requires.txt
 src/nitrado.egg-info/top_level.txt
+src/nitrado/games/__init__.py
+src/nitrado/games/ark_survival.py
 src/nitrado/lib/__init__.py
 src/nitrado/lib/errors.py
 src/nitrado/lib/game_server.py
 src/nitrado/lib/service.py
 src/nitrado/tools/__init__.py
 src/nitrado/tools/client.py
 tests/test_connection.py
```

### Comparing `nitrado-1.0.2/tests/test_connection.py` & `nitrado-1.0.3/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/tests/test_game_server.py` & `nitrado-1.0.3/tests/test_game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.2/tests/test_service.py` & `nitrado-1.0.3/tests/test_service.py`

 * *Files identical despite different names*

