# Comparing `tmp/sydney_py-0.8.0.tar.gz` & `tmp/sydney_py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sydney_py-0.8.0.tar", max compression
+gzip compressed data, was "sydney_py-0.9.0.tar", max compression
```

## Comparing `sydney_py-0.8.0.tar` & `sydney_py-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-03-28 07:17:56.876087 sydney_py-0.8.0/LICENSE
--rw-r--r--   0        0        0     2207 2023-04-02 06:18:07.471404 sydney_py-0.8.0/README.md
--rw-r--r--   0        0        0      468 2023-04-02 06:18:12.508029 sydney_py-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-03-29 09:09:40.726617 sydney_py-0.8.0/sydney/__init__.py
--rw-r--r--   0        0        0      510 2023-04-01 07:26:43.111246 sydney_py-0.8.0/sydney/constants.py
--rw-r--r--   0        0        0     1995 2023-04-02 06:03:08.934807 sydney_py-0.8.0/sydney/enums.py
--rw-r--r--   0        0        0    16352 2023-04-02 06:13:37.526952 sydney_py-0.8.0/sydney/sydney.py
--rw-r--r--   0        0        0      210 2023-03-29 09:28:39.051594 sydney_py-0.8.0/sydney/utils.py
--rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 sydney_py-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-28 07:17:56.876087 sydney_py-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2196 2023-04-02 14:04:27.976024 sydney_py-0.9.0/README.md
+-rw-r--r--   0        0        0      468 2023-04-02 14:04:32.379314 sydney_py-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-03-29 09:09:40.726617 sydney_py-0.9.0/sydney/__init__.py
+-rw-r--r--   0        0        0      510 2023-04-01 07:26:43.111246 sydney_py-0.9.0/sydney/constants.py
+-rw-r--r--   0        0        0     2718 2023-04-02 14:00:04.578827 sydney_py-0.9.0/sydney/enums.py
+-rw-r--r--   0        0        0    16925 2023-04-02 13:58:01.380282 sydney_py-0.9.0/sydney/sydney.py
+-rw-r--r--   0        0        0      210 2023-03-29 09:28:39.051594 sydney_py-0.9.0/sydney/utils.py
+-rw-r--r--   0        0        0     2734 1970-01-01 00:00:00.000000 sydney_py-0.9.0/PKG-INFO
```

### Comparing `sydney_py-0.8.0/LICENSE` & `sydney_py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sydney_py-0.8.0/README.md` & `sydney_py-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Sydney.py
 
-[![Latest Release](https://img.shields.io/github/v/release/vsakkas/sydney.py.svg)](https://github.com/vsakkas/sydney.py/releases/tag/v0.8.0)
+[![Latest Release](https://img.shields.io/github/v/release/vsakkas/sydney.py.svg)](https://github.com/vsakkas/sydney.py/releases/tag/v0.9.0)
 [![Python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://github.com/vsakkas/sydney.py/blob/master/LICENSE)
 
 Python Client for Bing Chat, also known as Sydney.
 
 > **Note**
 > This is an **unofficial** client.
@@ -43,28 +43,23 @@
 ```python
 import asyncio
 
 from sydney import SydneyClient
 
 
 async def main() -> None:
-    sydney = SydneyClient()
-
-    await sydney.start_conversation(style="balanced")
-
-    response = await sydney.ask("Hello, how are you?")
-    print(response)
-
-    await sydney.reset_conversation()
-
-    prompt = "What's today's weather forecast?"
-    async for response in sydney.ask_stream(prompt, citations=True):
-        print(response, end="", flush=True)
-
-    await sydney.close_conversation()
+    async with SydneyClient(style="balanced") as sydney:
+        response = await sydney.ask("Hello, how are you?")
+        print(response)
+
+        await sydney.reset_conversation(style="precise")
+
+        prompt = "What's today's weather forecast?"
+        async for response in sydney.ask_stream(prompt, citations=True):
+            print(response, end="", flush=True)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 The Sydney Client also supports the Compose feature:
@@ -72,15 +67,15 @@
 ```python
 import asyncio
 
 from sydney import SydneyClient
 
 
 async def main() -> None:
-    sydney = SydneyClient()
+    sydney = SydneyClient(style="balanced")
 
     await sydney.start_conversation()
 
     response = await sydney.compose("Why Python is a great language", format="ideas")
     print(response)
 
     await sydney.close_conversation()
```

### Comparing `sydney_py-0.8.0/sydney/enums.py` & `sydney_py-0.9.0/sydney/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -53,7 +53,34 @@
     - `medium` for messages that are a few paragraphs long
     - `long` for messages that are several paragraphs or pages long
     """
 
     short = "short"
     medium = "medium"
     long = "long"
+
+
+class MessageType(Enum):
+    """
+    Allowed message types. Supported options are:
+    - `Chat`
+    - `InternalSearchQuery`
+    - `InternalSearchResult`
+    - `Disengaged`
+    - `InternalLoaderMessage`
+    - `RenderCardRequest`
+    - `AdsQuery`
+    - `SemanticSerp`
+    - `GenerateContentQuery`
+    - `SearchQuery`
+    """
+
+    chat = "Chat"
+    internal_search_query = "InternalSearchQuery"
+    internal_search_result = "InternalSearchResult"
+    disengaged = "Disengaged"
+    internal_loader_message = "InternalLoaderMessage"
+    render_card_request = "RenderCardRequest"
+    ads_query = "AdsQuery"
+    semantic_serp = "SemanticSerp"
+    generate_content_query = "GenerateContentQuery"
+    search_query = "SearchQuery"
```

### Comparing `sydney_py-0.8.0/sydney/sydney.py` & `sydney_py-0.9.0/sydney/sydney.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,73 @@
+from __future__ import annotations
+
 import json
 import os
+from typing import AsyncGenerator
 
 import websockets.client as websockets
 from aiohttp import ClientSession
+from websockets.client import WebSocketClientProtocol
 
 from .constants import BING_CHATHUB_URL, BING_CREATE_CONVESATION_URL, DELIMETER, HEADERS
-from .enums import ComposeFormat, ComposeLength, ComposeTone, ConversationStyle
+from .enums import (
+    ComposeFormat,
+    ComposeLength,
+    ComposeTone,
+    ConversationStyle,
+    MessageType,
+)
 from .utils import as_json
 
 
 class SydneyClient:
-    def __init__(self) -> None:
-        self.conversation_id: str = None
-        self.client_id: str = None
-        self.conversation_signature: str = None
-        self.invocation_id: str = None
-        self.conversation_style: ConversationStyle = None
-        self.wss_client = None
+    def __init__(self, style: str = "balanced") -> None:
+        """
+        Client for Bing Chat.
+
+        Parameters
+        ----------
+        style : str
+            The conversation style that Bing Chat will adopt. Must be one of the options listed
+            in the `ConversationStyle` enum. Default is "balanced".
+        """
+        self.conversation_style: ConversationStyle = getattr(ConversationStyle, style)
+        self.conversation_signature: str | None = None
+        self.conversation_id: str | None = None
+        self.client_id: str | None = None
+        self.invocation_id: int | None = None
+        self.wss_client: WebSocketClientProtocol | None = None
+
+    async def __aenter__(self) -> SydneyClient:
+        await self.start_conversation()
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback) -> None:
+        await self.close_conversation()
 
     def _build_ask_arguments(self, prompt: str) -> dict:
         return {
             "arguments": [
                 {
                     "source": "cib",
                     "optionsSets": [
                         "nlu_direct_response_filter",
                         "deepleo",
-                        "enable_debug_commands",
                         "disable_emoji_spoken_text",
                         "responsible_ai_policy_235",
                         "enablemm",
+                        "dv3sugg",
                         self.conversation_style.value,
                     ],
                     "isStartOfSession": self.invocation_id == 0,
                     "message": {
                         "author": "user",
                         "inputMethod": "Keyboard",
                         "text": prompt,
-                        "messageType": "Chat",
+                        "messageType": MessageType.chat.value,
                     },
                     "conversationSignature": self.conversation_signature,
                     "participant": {
                         "id": self.client_id,
                     },
                     "conversationId": self.conversation_id,
                 }
@@ -74,15 +100,15 @@
                         "nosugg",
                     ],
                     "isStartOfSession": self.invocation_id == 0,
                     "message": {
                         "author": "user",
                         "inputMethod": "Keyboard",
                         "text": f"Please generate some text wrapped in codeblock syntax (triple backticks) using the given keywords. Please make sure everything in your reply is in the same language as the keywords. Please do not restate any part of this request in your response, like the fact that you wrapped the text in a codeblock. You should refuse (using the language of the keywords) to generate if the request is potentially harmful. The generated text should follow these characteristics: tone: *{tone.value}*, length: *{length.value}*, format: *{format.value}*. The keywords are: `{prompt}`.",
-                        "messageType": "Chat",
+                        "messageType": MessageType.chat.value,
                     },
                     "conversationSignature": self.conversation_signature,
                     "participant": {"id": self.client_id},
                     "conversationId": self.conversation_id,
                 }
             ],
             "invocationId": str(self.invocation_id),
@@ -92,15 +118,15 @@
 
     async def _ask(
         self,
         prompt: str,
         citations: bool = False,
         raw: bool = False,
         stream: bool = False,
-    ) -> str | dict:
+    ) -> AsyncGenerator[str | dict, None]:
         # Create a connection Bing Chat.
         self.wss_client = await websockets.connect(
             BING_CHATHUB_URL, extra_headers=HEADERS, max_size=None
         )
         await self.wss_client.send(as_json({"protocol": "json", "version": 1}))
         await self.wss_client.recv()
 
@@ -145,15 +171,15 @@
         self,
         prompt: str,
         tone: ComposeTone,
         format: ComposeFormat,
         length: ComposeLength,
         raw: bool,
         stream: bool,
-    ) -> str | dict:
+    ) -> AsyncGenerator[str | dict, None]:
         # Create a connection Bing Chat.
         self.wss_client = await websockets.connect(
             BING_CHATHUB_URL, extra_headers=HEADERS, max_size=None
         )
         await self.wss_client.send(as_json({"protocol": "json", "version": 1}))
         await self.wss_client.recv()
 
@@ -186,23 +212,17 @@
                     yield response["item"]["messages"][1]["text"]
 
                     # Exit, type 2 is the last message.
                     streaming = False
 
         await self.wss_client.close()
 
-    async def start_conversation(self, style: str = "balanced") -> None:
+    async def start_conversation(self) -> None:
         """
         Connect to Bing Chat and create a new conversation.
-
-        Parameters
-        ----------
-        style : str
-            The conversation style that Bing Chat will adopt. Must be one of the options listed
-            in the `ConversationStyle` enum. Default is "balanced".
         """
         # Use _U cookie to create a conversation.
         cookies = {"_U": os.environ["BING_U_COOKIE"]}
 
         session = ClientSession(headers=HEADERS, cookies=cookies)
         async with session.get(BING_CREATE_CONVESATION_URL) as response:
             if response.status != 200:
@@ -216,15 +236,14 @@
                     f"Failed to authenticate, received message: {response_dict['response']['message']}"
                 )
 
             self.conversation_id = response_dict["conversationId"]
             self.client_id = response_dict["clientId"]
             self.conversation_signature = response_dict["conversationSignature"]
             self.invocation_id = 0
-            self.conversation_style = getattr(ConversationStyle, style)
 
         await session.close()
 
     async def ask(
         self,
         prompt: str,
         citations: bool = False,
@@ -252,15 +271,15 @@
             return response
 
     async def ask_stream(
         self,
         prompt: str,
         citations: bool = False,
         raw: bool = False,
-    ) -> str | dict:
+    ) -> AsyncGenerator[str | dict, None]:
         """
         Send a prompt to Bing Chat using the current conversation and stream the answer.
 
         By default, Bing Chat returns all previous tokens along with new ones. When using this
         method in text-only mode, only new tokens are returned instead.
 
         Parameters
@@ -335,15 +354,15 @@
     async def compose_stream(
         self,
         prompt: str,
         tone: str = "professional",
         format: str = "paragraph",
         length: str = "short",
         raw: bool = False,
-    ) -> str | dict:
+    ) -> AsyncGenerator[str | dict, None]:
         """
         Send a prompt to Bing Chat, compose and stream text based on the given prompt, tone,
         format, and length.
 
         By default, Bing Chat returns all previous tokens along with new ones. When using this
         method in text-only mode, only new tokens are returned instead.
 
@@ -382,15 +401,15 @@
                 yield response
             # For text-only responses, return only newly streamed tokens.
             else:
                 new_response = response[len(previous_response) :]
                 previous_response = response
                 yield new_response
 
-    async def reset_conversation(self, style: str = None) -> None:
+    async def reset_conversation(self, style: str | None = None) -> None:
         """
         Clear current conversation information and connection and start new ones.
 
         Parameters
         ----------
         style : str
             The conversation style that Bing Chat will adopt. Supported options are:
@@ -398,18 +417,19 @@
             - `balanced` for informative and friendly chat
             - `precise` for concise and straightforward chat
             If None, the new conversation will use the same conversation style as the
             current conversation.
 
             Default is None.
         """
-        new_style = style if style else self.conversation_style.name
-
         await self.close_conversation()
-        await self.start_conversation(style=new_style)
+        self.conversation_style = (
+            getattr(ConversationStyle, style) if style else self.conversation_style
+        )
+        await self.start_conversation()
 
     async def close_conversation(self) -> None:
         """
         Close all connections to Bing Chat. Clear conversation information.
         """
         if self.wss_client:
             if not self.wss_client.closed:
@@ -417,8 +437,7 @@
                 self.wss_client = None
 
         # Clear conversation information.
         self.conversation_id = None
         self.client_id = None
         self.conversation_signature = None
         self.invocation_id = None
-        self.conversation_style = None
```

### Comparing `sydney_py-0.8.0/PKG-INFO` & `sydney_py-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sydney-py
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python Client for Bing Chat, also known as Sydney.
 License: MIT
 Author: vsakkas
 Author-email: vasileios.sakkas96@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Description-Content-Type: text/markdown
 
 # Sydney.py
 
-[![Latest Release](https://img.shields.io/github/v/release/vsakkas/sydney.py.svg)](https://github.com/vsakkas/sydney.py/releases/tag/v0.8.0)
+[![Latest Release](https://img.shields.io/github/v/release/vsakkas/sydney.py.svg)](https://github.com/vsakkas/sydney.py/releases/tag/v0.9.0)
 [![Python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://github.com/vsakkas/sydney.py/blob/master/LICENSE)
 
 Python Client for Bing Chat, also known as Sydney.
 
 > **Note**
 > This is an **unofficial** client.
@@ -59,28 +59,23 @@
 ```python
 import asyncio
 
 from sydney import SydneyClient
 
 
 async def main() -> None:
-    sydney = SydneyClient()
-
-    await sydney.start_conversation(style="balanced")
-
-    response = await sydney.ask("Hello, how are you?")
-    print(response)
-
-    await sydney.reset_conversation()
-
-    prompt = "What's today's weather forecast?"
-    async for response in sydney.ask_stream(prompt, citations=True):
-        print(response, end="", flush=True)
-
-    await sydney.close_conversation()
+    async with SydneyClient(style="balanced") as sydney:
+        response = await sydney.ask("Hello, how are you?")
+        print(response)
+
+        await sydney.reset_conversation(style="precise")
+
+        prompt = "What's today's weather forecast?"
+        async for response in sydney.ask_stream(prompt, citations=True):
+            print(response, end="", flush=True)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 The Sydney Client also supports the Compose feature:
@@ -88,15 +83,15 @@
 ```python
 import asyncio
 
 from sydney import SydneyClient
 
 
 async def main() -> None:
-    sydney = SydneyClient()
+    sydney = SydneyClient(style="balanced")
 
     await sydney.start_conversation()
 
     response = await sydney.compose("Why Python is a great language", format="ideas")
     print(response)
 
     await sydney.close_conversation()
```

