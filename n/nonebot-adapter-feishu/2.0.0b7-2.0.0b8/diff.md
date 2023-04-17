# Comparing `tmp/nonebot_adapter_feishu-2.0.0b7.tar.gz` & `tmp/nonebot_adapter_feishu-2.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_feishu-2.0.0b7.tar", max compression
+gzip compressed data, was "nonebot_adapter_feishu-2.0.0b8.tar", max compression
```

## Comparing `nonebot_adapter_feishu-2.0.0b7.tar` & `nonebot_adapter_feishu-2.0.0b8.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/LICENSE
--rw-r--r--   0        0        0      259 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/README.md
--rw-r--r--   0        0        0      597 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/__init__.py
--rw-r--r--   0        0        0    12438 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/adapter.py
--rw-r--r--   0        0        0     6489 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/bot.py
--rw-r--r--   0        0        0     1393 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/config.py
--rw-r--r--   0        0        0    19770 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/event.py
--rw-r--r--   0        0        0     1373 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/exception.py
--rw-r--r--   0        0        0     8305 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/message.py
--rw-r--r--   0        0        0     1499 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/utils.py
--rw-r--r--   0        0        0     1670 2023-02-11 07:52:17.942254 nonebot_adapter_feishu-2.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.0.0b7/setup.py
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/LICENSE
+-rw-r--r--   0        0        0      259 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/README.md
+-rw-r--r--   0        0        0      597 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/__init__.py
+-rw-r--r--   0        0        0    12438 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/adapter.py
+-rw-r--r--   0        0        0     6489 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/bot.py
+-rw-r--r--   0        0        0     1393 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/config.py
+-rw-r--r--   0        0        0    19848 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/event.py
+-rw-r--r--   0        0        0     1373 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/exception.py
+-rw-r--r--   0        0        0     8305 2023-04-17 02:24:39.702280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/message.py
+-rw-r--r--   0        0        0     1499 2023-04-17 02:24:39.702280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/utils.py
+-rw-r--r--   0        0        0     1944 2023-04-17 02:24:39.702280 nonebot_adapter_feishu-2.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.0.0b8/PKG-INFO
```

### Comparing `nonebot_adapter_feishu-2.0.0b7/LICENSE` & `nonebot_adapter_feishu-2.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/__init__.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/adapter.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/bot.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/config.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/event.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from typing import Any, Dict, List, Literal, Optional
 
 from nonebot.typing import overrides
+from nonebot.utils import escape_tag
 from pydantic import Field, BaseModel, root_validator
 
 from nonebot.adapters import Event as BaseEvent
 
 from .message import Message, MessageDeserializer
 
 
@@ -39,15 +40,15 @@
 
     @overrides(BaseEvent)
     def get_event_name(self) -> str:
         return self.header.event_type
 
     @overrides(BaseEvent)
     def get_event_description(self) -> str:
-        return str(self.dict())
+        return escape_tag(str(self.dict()))
 
     @overrides(BaseEvent)
     def get_message(self) -> Message:
         raise ValueError("Event has no message!")
 
     @overrides(BaseEvent)
     def get_plaintext(self) -> str:
@@ -186,15 +187,15 @@
         return f"{self.get_type()}.{self.event.message.chat_type}"
 
     @overrides(Event)
     def get_event_description(self) -> str:
         return (
             f"{self.event.message.message_id} from {self.get_user_id()}"
             f"@[{self.event.message.chat_type}:{self.event.message.chat_id}]"
-            f" {self.get_message()}"
+            f" {escape_tag(str(self.get_message()))}"
         )
 
     @overrides(Event)
     def get_message(self) -> Message:
         return self.event.message.content
 
     @overrides(Event)
@@ -236,15 +237,15 @@
 
     @overrides(Event)
     def get_event_name(self) -> str:
         return self.header.event_type
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        return str(self.dict())
+        return escape_tag(str(self.dict()))
 
     @overrides(Event)
     def get_message(self) -> Message:
         raise ValueError("Event has no message!")
 
     @overrides(Event)
     def get_plaintext(self) -> str:
```

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/exception.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/message.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/nonebot/adapters/feishu/utils.py` & `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b7/pyproject.toml` & `nonebot_adapter_feishu-2.0.0b8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-feishu"
-version = "2.0.0-beta.7"
+version = "2.0.0-beta.8"
 description = "feishu(larksuite) adapter for nonebot2"
 authors = ["StarHeartHunt <starheart233@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://feishu.adapters.nonebot.dev/"
 repository = "https://github.com/nonebot/adapter-feishu"
 documentation = "https://feishu.adapters.nonebot.dev/"
@@ -21,44 +21,61 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pycryptodome = "^3.10.1"
 httpx = ">=0.18.0, <1.0.0"
 nonebot2 = ">=2.0.0-beta.1"
-cashews = "^4.0.0"
+cashews = ">=5,<7"
 
-[tool.poetry.dev-dependencies]
-isort = "^5.12.0"
+[tool.poetry.group.dev.dependencies]
+pycln = "^2.1.2"
+isort = "^5.10.1"
 black = "^23.1.0"
-pytest-cov = "^3.0.0"
-pytest-asyncio = "^0.18.1"
-nonebug = { git = "https://github.com/nonebot/nonebug.git" }
+nonemoji = "^0.1.2"
+pre-commit = "^3.0.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
+
+[tool.poetry.group.test.dependencies]
+pytest-cov = "^4.0.0"
+pytest-xdist = "^3.0.2"
+pytest-asyncio = ">=0.20,<0.22"
+nonebug = { git = "https://github.com/nonebot/nonebug.git" }
+
+[tool.poetry.group.docs.dependencies]
 nb-autodoc = { git = "https://github.com/nonebot/nb-autodoc.git" }
-pre-commit = "^3.0.4"
-Jinja2 = "^3.1.2"
 
 [tool.black]
 line-length = 88
-target-version = ["py37", "py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310", "py311"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
-src_paths = ["nonebot", "tests"]
 extra_standard_library = ["typing_extensions"]
 
+[tool.pycln]
+path = "."
+all = false
+
 [tool.pyright]
-exclude = ["**/node_modules",
-    "**/__pycache__"
+reportShadowedImports = false
+pythonVersion = "3.8"
+pythonPlatform = "All"
+executionEnvironments = [
+  { root = "./" },
+]
+exclude = [
+  "**/node_modules",
+  "**/__pycache__",
+  "**/tests"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_adapter_feishu-2.0.0b7/PKG-INFO` & `nonebot_adapter_feishu-2.0.0b8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-feishu
-Version: 2.0.0b7
+Version: 2.0.0b8
 Summary: feishu(larksuite) adapter for nonebot2
 Home-page: https://feishu.adapters.nonebot.dev/
 License: MIT
 Keywords: bot,feishu,larksuite
 Author: StarHeartHunt
 Author-email: starheart233@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: cashews (>=4.0.0,<5.0.0)
+Requires-Dist: cashews (>=5,<7)
 Requires-Dist: httpx (>=0.18.0,<1.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.1)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Project-URL: Documentation, https://feishu.adapters.nonebot.dev/
 Project-URL: Repository, https://github.com/nonebot/adapter-feishu
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.0.0b7 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.0.0b8 Summary:
 feishu(larksuite) adapter for nonebot2 Home-page: https://
 feishu.adapters.nonebot.dev/ License: MIT Keywords: bot,feishu,larksuite
 Author: StarHeartHunt Author-email: starheart233@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Framework :: Robot Framework Classifier: Framework :: Robot Framework ::
 Library Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Requires-Dist: cashews (>=4.0.0,<5.0.0) Requires-Dist:
-httpx (>=0.18.0,<1.0.0) Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist:
+Language :: Python :: 3 Requires-Dist: cashews (>=5,<7) Requires-Dist: httpx
+(>=0.18.0,<1.0.0) Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist:
 pycryptodome (>=3.10.1,<4.0.0) Project-URL: Documentation, https://
 feishu.adapters.nonebot.dev/ Project-URL: Repository, https://github.com/
 nonebot/adapter-feishu Description-Content-Type: text/markdown
                                    [nonebot]
              # NoneBot-Adapter-Feishu _â¨ é£ä¹¦åè®®éé â¨_
```

