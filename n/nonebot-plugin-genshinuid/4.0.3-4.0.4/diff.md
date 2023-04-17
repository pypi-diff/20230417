# Comparing `tmp/nonebot_plugin_genshinuid-4.0.3.tar.gz` & `tmp/nonebot_plugin_genshinuid-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshinuid-4.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshinuid-4.0.4.tar", max compression
```

## Comparing `nonebot_plugin_genshinuid-4.0.3.tar` & `nonebot_plugin_genshinuid-4.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14731 2023-04-15 16:16:49.431629 nonebot_plugin_genshinuid-4.0.3/GenshinUID/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-14 17:44:32.922572 nonebot_plugin_genshinuid-4.0.3/GenshinUID/auto_install.py
--rw-r--r--   0        0        0    23262 2023-04-15 16:24:47.352109 nonebot_plugin_genshinuid-4.0.3/GenshinUID/client.py
--rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.3/GenshinUID/models.py
--rw-r--r--   0        0        0      336 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.3/GenshinUID/path.py
--rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.3/LICENSE
--rw-r--r--   0        0        0     1652 2023-04-15 16:27:28.995575 nonebot_plugin_genshinuid-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     3318 2023-04-14 17:44:32.924573 nonebot_plugin_genshinuid-4.0.3/README.md
--rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    15002 2023-04-17 18:41:54.366553 nonebot_plugin_genshinuid-4.0.4/GenshinUID/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-17 18:40:04.757027 nonebot_plugin_genshinuid-4.0.4/GenshinUID/auto_install.py
+-rw-r--r--   0        0        0    23514 2023-04-17 18:42:03.040685 nonebot_plugin_genshinuid-4.0.4/GenshinUID/client.py
+-rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.4/GenshinUID/models.py
+-rw-r--r--   0        0        0      336 2023-04-17 18:40:04.758052 nonebot_plugin_genshinuid-4.0.4/GenshinUID/path.py
+-rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.4/LICENSE
+-rw-r--r--   0        0        0     1652 2023-04-17 18:42:29.621770 nonebot_plugin_genshinuid-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3318 2023-04-17 18:40:04.759072 nonebot_plugin_genshinuid-4.0.4/README.md
+-rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_genshinuid-4.0.3/GenshinUID/__init__.py` & `nonebot_plugin_genshinuid-4.0.4/GenshinUID/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,20 @@
     )
     logger.info(f'【发送】[gsuid-core]: {msg.bot_id}')
     await gsclient._input(msg)
 
 
 @get_message.handle()
 async def get_all_message(bot: Bot, ev: Event):
-    if gsclient is None or not gsclient.is_alive:
+    if gsclient is None:
+        return await connect()
+
+    try:
+        await gsclient.ws.ping()
+    except ConnectionClosed:
         return await connect()
 
     # 通用字段获取
     group_id = None
     user_id = ev.get_user_id()
     messages = ev.get_message()
     logger.debug(ev)
@@ -146,14 +151,18 @@
                     pm = 3
                 elif 5 in ev.member.roles:
                     pm = 5
             msg_id = ev.id
         else:
             logger.debug('[gsuid] 不支持该 QQ Guild 事件...')
             return
+
+        if ev.message_reference:
+            reply_msg_id = ev.message_reference.message_id
+            message.append(Message('reply', reply_msg_id))
     # telegram
     elif bot.adapter.get_name() == 'Telegram':
         from nonebot.adapters.telegram.event import (
             GroupMessageEvent,
             PrivateMessageEvent,
         )
 
@@ -387,14 +396,15 @@
         await connect()
 
 
 async def connect():
     global gsclient
     try:
         gsclient = await GsClient().async_connect()
+        await gsclient.start()
     except ConnectionRefusedError:
         logger.error('Core服务器连接失败...请稍后使用[启动core]命令启动...')
 
 
 @scheduler.scheduled_job('cron', second='*/10')
 async def repeat_connect():
     if is_repeat:
```

### Comparing `nonebot_plugin_genshinuid-4.0.3/GenshinUID/auto_install.py` & `nonebot_plugin_genshinuid-4.0.4/GenshinUID/auto_install.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.3/GenshinUID/client.py` & `nonebot_plugin_genshinuid-4.0.4/GenshinUID/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,26 @@
 if hasattr(driver.config, 'gsuid_core_port'):
     PORT = driver.config.gsuid_core_port
 else:
     PORT = '8765'
 
 
 def _get_bot(bot_id: str) -> Bot:
-    if 'onebot' in bot_id:
-        bot_id = 'onebot'
+    if 'v12' in bot_id:
+        bot_id = 'onebotv12'
+    # bots: Dict[str, str] 以适配器名称为键、bot_self_id为值的字典
     if bot_id not in bots:
         for _bot_id in bots.keys():
             if bot_id in _bot_id:
                 bot_id = _bot_id
                 break
+        else:
+            logger.warning('未获取到正确的Bot实例,将使用默认Bot...')
+            logger.warning(f'当前bot_id: {bot_id}, bots: {bots}')
+            return get_bot()
     bot_real_id = bots[bot_id]
     bot = get_bot(bot_real_id)
     return bot
 
 
 class GsClient:
     _instance = None
@@ -59,15 +64,14 @@
         logger.info(f'Bot_ID: {BOT_ID}连接至[gsuid-core]: {self.ws_url}...')
         cls.ws = await websockets.client.connect(
             cls.ws_url, max_size=2**26, open_timeout=60, ping_timeout=60
         )
         logger.success(f'与[gsuid-core]成功连接! Bot_ID: {BOT_ID}')
         cls.msg_list = asyncio.queues.Queue()
         cls.pending = []
-        await self.start()
         return self
 
     def __new__(cls, *args, **kwargs):
         # 判断sv是否已经被初始化
         if cls._instance is None:
             cls._instance = super(GsClient, cls).__new__(cls, *args, **kwargs)
         return cls._instance
```

### Comparing `nonebot_plugin_genshinuid-4.0.3/GenshinUID/models.py` & `nonebot_plugin_genshinuid-4.0.4/GenshinUID/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.3/LICENSE` & `nonebot_plugin_genshinuid-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.3/pyproject.toml` & `nonebot_plugin_genshinuid-4.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nonebot-plugin-genshinuid"
-version = "4.0.3"
+version = "4.0.4"
 description = "支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件"
 authors = ["KimigaiiWuyi <444835641@qq.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2"
 repository = "https://github.com/KimigaiiWuyi/GenshinUID"
 documentation = "https://docs.gsuid.gbots.work/#/"
```

### Comparing `nonebot_plugin_genshinuid-4.0.3/README.md` & `nonebot_plugin_genshinuid-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.3/PKG-INFO` & `nonebot_plugin_genshinuid-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshinuid
-Version: 4.0.3
+Version: 4.0.4
 Summary: 支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later
 Author: KimigaiiWuyi
 Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.4 Summary:
 æ¯æOneBot
 (QQ)ãOneBotV12ãQQé¢éãå¾®ä¿¡ãKOOKï¼å¼é»å¦ï¼ãTelegramï¼çµæ¥ï¼ãFeiShuï¼é£ä¹¦ï¼çå¨åè½NoneBot2åç¥æä»¶
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later Author: KimigaiiWuyi Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

