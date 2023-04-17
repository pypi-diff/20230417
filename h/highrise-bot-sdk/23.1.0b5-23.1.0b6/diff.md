# Comparing `tmp/highrise_bot_sdk-23.1.0b5.tar.gz` & `tmp/highrise_bot_sdk-23.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.1.0b5.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-23.1.0b6.tar", max compression
```

## Comparing `highrise_bot_sdk-23.1.0b5.tar` & `highrise_bot_sdk-23.1.0b6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2227 2023-04-11 15:28:48.858654 highrise_bot_sdk-23.1.0b5/README.md
--rw-r--r--   0        0        0      941 2023-04-05 10:55:11.593090 highrise_bot_sdk-23.1.0b5/pyproject.toml
--rw-r--r--   0        0        0     7970 2023-04-11 15:27:49.521691 highrise_bot_sdk-23.1.0b5/src/highrise/__init__.py
--rw-r--r--   0        0        0     6923 2023-04-11 15:27:49.521577 highrise_bot_sdk-23.1.0b5/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b5/src/highrise/_unions.py
--rw-r--r--   0        0        0     7386 2023-04-11 15:27:49.521650 highrise_bot_sdk-23.1.0b5/src/highrise/models.py
--rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b5/src/highrise/py.typed
--rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b5/setup.py
--rw-r--r--   0        0        0     2766 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0     2281 2023-04-17 15:53:00.038558 highrise_bot_sdk-23.1.0b6/README.md
+-rw-r--r--   0        0        0      992 2023-04-17 15:53:00.038518 highrise_bot_sdk-23.1.0b6/pyproject.toml
+-rw-r--r--   0        0        0     7982 2023-04-17 14:59:33.153106 highrise_bot_sdk-23.1.0b6/src/highrise/__init__.py
+-rw-r--r--   0        0        0     7172 2023-04-17 14:59:33.153149 highrise_bot_sdk-23.1.0b6/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b6/src/highrise/_unions.py
+-rw-r--r--   0        0        0     7386 2023-04-11 15:27:49.521650 highrise_bot_sdk-23.1.0b6/src/highrise/models.py
+-rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b6/src/highrise/py.typed
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b6/setup.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b6/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.1.0b5/README.md` & `highrise_bot_sdk-23.1.0b6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b5
+$ pip install highrise-bot-sdk==23.1.0b6
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -28,14 +28,18 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b6 (2023-04-17)
+
+- Add Python 3.10 support
+
 ### 23.1.0b5 (2023-04-11)
 
 - Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).
 - Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).
 - Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). 
 - Rework how keepalive is handled
```

### Comparing `highrise_bot_sdk-23.1.0b5/pyproject.toml` & `highrise_bot_sdk-23.1.0b6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.1.0.b5"
+version = "23.1.0.b6"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 aiohttp = ">= 3.8.4"
 click = ">= 8.1.3"
 cattrs = "^22.2.0"
+quattro = "^22.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 mypy = "^1.1.1"
 flake8 = "^6.0.0"
+types-setuptools = "^67.6.0.7"
 
 
 [tool.poetry.scripts]
 highrise = "highrise.__main__:run"
 
 [tool.isort]
 profile = "black"
```

### Comparing `highrise_bot_sdk-23.1.0b5/src/highrise/__init__.py` & `highrise_bot_sdk-23.1.0b6/src/highrise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """The Highrise bot SDK."""
 from __future__ import annotations
 
-from asyncio import Queue, TaskGroup, sleep
+from asyncio import Queue, sleep
 from itertools import count
 from typing import TYPE_CHECKING, Any, Callable, Literal, Protocol, TypeVar, Union
 
 from aiohttp import ClientWebSocketResponse
 from cattrs.preconf.json import make_converter
+from quattro import TaskGroup
 
 from ._unions import configure_tagged_union
 from .models import (
     AnchorPosition,
     ChangeRoomPrivilegeRequest,
     ChannelEvent,
     ChannelRequest,
@@ -180,17 +181,15 @@
         user_id: str,
         action: Literal["kick", "ban", "unban", "mute"],
         action_length: int | None = None,
     ) -> None:
         """Moderate a user in the room."""
         await _do_req_no_resp(self, ModerateRoomRequest(user_id, action, action_length))
 
-    async def get_room_privilege(
-        self, user_id: str
-    ) -> RoomPermissions | Error:
+    async def get_room_privilege(self, user_id: str) -> RoomPermissions | Error:
         """Fetch the room privilege for given user_id."""
         resp = await do_req_resp(self, GetRoomPrivilegeRequest(user_id))
         if isinstance(resp, Error):
             return resp
         return resp.content
 
     async def change_room_privilege(
@@ -272,12 +271,15 @@
     | EmoteEvent
     | ReactionEvent
     | UserJoinedEvent
     | UserLeftEvent
     | ChannelEvent
     | TipReactionEvent
 )
-Incoming = IncomingEvents | Union[*(r.Response for r in Outgoing.__args__)]  # type: ignore
+
+
+Incoming = IncomingEvents | Union[tuple(r.Response for r in Outgoing.__args__)]  # type: ignore
+
 
 configure_tagged_union(SessionMetadata | Error, converter)
 configure_tagged_union(Incoming, converter)
 configure_tagged_union(Outgoing, converter)
```

### Comparing `highrise_bot_sdk-23.1.0b5/src/highrise/__main__.py` & `highrise_bot_sdk-23.1.0b6/src/highrise/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
-from asyncio import TaskGroup
 from asyncio import run as arun
 from asyncio import sleep
 from asyncio.exceptions import TimeoutError
 from importlib import import_module
 from math import ceil
 from os import environ, getcwd
 from sys import path
 from time import monotonic
 from typing import Any, AsyncGenerator, Final
 
+import pkg_resources
 from aiohttp import ClientSession, WebSocketError, WSServerHandshakeError
 from click import argument, command
+from quattro import TaskGroup
 
 from . import BaseBot, Highrise, Incoming, IncomingEvents, converter
 from .models import (
     ChannelEvent,
     ChatEvent,
     EmoteEvent,
     Error,
@@ -44,14 +45,15 @@
     """
     path.append(getcwd())
     mod, name = bot_path.split(":")
     return arun(main(getattr(import_module(mod), name)(), room_id, api_token))
 
 
 async def main(bot: BaseBot, room_id: str, api_key: str) -> None:
+    version = pkg_resources.get_distribution("highrise-bot-sdk").version
     async with TaskGroup() as tg:
         t = throttler(5, 5)
         while True:
             await anext(t)
             try:
                 async with ClientSession() as session:
                     async with session.ws_connect(
@@ -77,14 +79,18 @@
                             ka_task.cancel()
                             return
                         bot_id = str(session_metadata.user_id)
                         chat = Highrise()
                         chat.ws = ws
                         chat.tg = tg
 
+                        print(
+                            f"Connected using The Highrise Python Bot SDK version: '{version}'."
+                        )
+
                         bot.highrise = chat
                         tg.create_task(bot.on_start(session_metadata))
                         while True:
                             frame = await ws.receive(READ_TIMEOUT)
                             if isinstance(frame.data, WebSocketError):
                                 print("Websocket error, exiting.")
                                 return
```

### Comparing `highrise_bot_sdk-23.1.0b5/src/highrise/_unions.py` & `highrise_bot_sdk-23.1.0b6/src/highrise/_unions.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.1.0b5/src/highrise/models.py` & `highrise_bot_sdk-23.1.0b6/src/highrise/models.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.1.0b5/setup.py` & `highrise_bot_sdk-23.1.0b6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,32 +7,35 @@
 packages = \
 ['highrise']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiohttp>=3.8.4', 'cattrs>=22.2.0,<23.0.0', 'click>=8.1.3']
+['aiohttp>=3.8.4',
+ 'cattrs>=22.2.0,<23.0.0',
+ 'click>=8.1.3',
+ 'quattro>=22.1.0,<23.0.0']
 
 entry_points = \
 {'console_scripts': ['highrise = highrise.__main__:run']}
 
 setup_kwargs = {
     'name': 'highrise-bot-sdk',
-    'version': '23.1.0b5',
+    'version': '23.1.0b6',
     'description': 'The Highrise Bot SDK, for running Highrise bots written in Python.',
-    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b5\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
+    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b6\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
     'author': 'Pocket Worlds Inc',
     'author_email': 'server@high.rs',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `highrise_bot_sdk-23.1.0b5/PKG-INFO` & `highrise_bot_sdk-23.1.0b6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: highrise-bot-sdk
-Version: 23.1.0b5
+Version: 23.1.0b6
 Summary: The Highrise Bot SDK, for running Highrise bots written in Python.
 License: Proprietary
 Author: Pocket Worlds Inc
 Author-email: server@high.rs
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4)
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: click (>=8.1.3)
+Requires-Dist: quattro (>=22.1.0,<23.0.0)
 Description-Content-Type: text/markdown
 
 # The Highrise Python Bot SDK
 
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b5
+$ pip install highrise-bot-sdk==23.1.0b6
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -44,14 +46,18 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b6 (2023-04-17)
+
+- Add Python 3.10 support
+
 ### 23.1.0b5 (2023-04-11)
 
 - Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).
 - Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).
 - Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). 
 - Rework how keepalive is handled
```

