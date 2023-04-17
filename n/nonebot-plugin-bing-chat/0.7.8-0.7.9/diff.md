# Comparing `tmp/nonebot-plugin-bing-chat-0.7.8.tar.gz` & `tmp/nonebot-plugin-bing-chat-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-bing-chat-0.7.8.tar", last modified: Sun Apr  2 10:20:05 2023, max compression
+gzip compressed data, was "nonebot-plugin-bing-chat-0.7.9.tar", last modified: Tue Apr 11 02:47:49 2023, max compression
```

## Comparing `nonebot-plugin-bing-chat-0.7.8.tar` & `nonebot-plugin-bing-chat-0.7.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.586597 nonebot-plugin-bing-chat-0.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.586597 nonebot-plugin-bing-chat-0.7.8/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.586597 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv12/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 10:19:51.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/telegram/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:20:05.590597 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-04-02 10:20:05.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-02 10:20:05.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 10:20:05.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-02 10:20:05.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-02 10:20:05.000000 nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv12/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:40.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/telegram/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:47:49.914441 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-11 02:47:49.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-11 02:47:49.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:47:49.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 02:47:49.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 02:47:49.000000 nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-bing-chat-0.7.8/LICENSE` & `nonebot-plugin-bing-chat-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/PKG-INFO` & `nonebot-plugin-bing-chat-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bing-chat
-Version: 0.7.8
+Version: 0.7.9
 Summary: 基于nonebot2的bing-chat软件
 Author-email: Harry <Harry0259@163.com>
 License: GPL-3
 Project-URL: Homepage, https://github.com/Harry-Jing/nonebot-plugin-bing-chat
 Classifier: Framework :: Pydantic
 Classifier: Topic :: Communications
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -44,15 +44,15 @@
 
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python" />
 
 </div>
 
 ## 📖 介绍
 
-一个可以使用新版Bing进行聊天的插件 (现在又不需要代理了）
+一个可以使用新版Bing进行聊天的插件 (现在又**不需要**代理了）
 
 目前支持[go-cqhttp](https://docs.go-cqhttp.org/)与[onebot v11](https://onebot.adapters.nonebot.dev/)适配器和[nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-patch)
 
 QQ群：366731501
 
 给个star🌟?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bing-chat Version: 0.7.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bing-chat Version: 0.7.9 Summary:
 åºäºnonebot2çbing-chatè½¯ä»¶ Author-email: Harry
 163.com> License: GPL-3 Project-URL: Homepage, https://github.com/Harry-Jing/
 nonebot-plugin-bing-chat Classifier: Framework :: Pydantic Classifier: Topic ::
 Communications Classifier: License :: OSI Approved :: GNU General Public
 License (GPL) Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
@@ -12,15 +12,15 @@
 File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                         # nonebot-plugin-bing-chat _â¨
 ä¸ä¸ªå¯ä»¥ä½¿ç¨æ°çBingè¿è¡èå¤©çæä»¶ â¨_ [license] [pypi] [PyPI_-
                               Downloads] [python]
 ## ð ä»ç» ä¸ä¸ªå¯ä»¥ä½¿ç¨æ°çBingè¿è¡èå¤©çæä»¶
-(ç°å¨åä¸éè¦ä»£çäºï¼ ç®åæ¯æ[go-cqhttp](https://docs.go-
+(ç°å¨å**ä¸éè¦**ä»£çäºï¼ ç®åæ¯æ[go-cqhttp](https://docs.go-
 cqhttp.org/)ä¸[onebot v11](https://onebot.adapters.nonebot.dev/)ééå¨å
 [nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-
 patch) QQç¾¤ï¼366731501 ç»ä¸ªstarð? >
 5æä»½æèè¯ï¼ææ¶éç¼æ´æ° > > å¦æä½ ææ´å¤éæ±ï¼è¯·åå¸
 [issue](https://github.com/Harry-Jing/nonebot-plugin-bing-chat/issues/
 new)è®©æç¥é ## ð¿ å®è£ä¸æ´æ°   ä½¿ç¨ nb-cli å®è£ä¸æ´æ°
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
```

### Comparing `nonebot-plugin-bing-chat-0.7.8/README.md` & `nonebot-plugin-bing-chat-0.7.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python" />
 
 </div>
 
 ## 📖 介绍
 
-一个可以使用新版Bing进行聊天的插件 (现在又不需要代理了）
+一个可以使用新版Bing进行聊天的插件 (现在又**不需要**代理了）
 
 目前支持[go-cqhttp](https://docs.go-cqhttp.org/)与[onebot v11](https://onebot.adapters.nonebot.dev/)适配器和[nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-patch)
 
 QQ群：366731501
 
 给个star🌟?
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                         # nonebot-plugin-bing-chat _â¨
 ä¸ä¸ªå¯ä»¥ä½¿ç¨æ°çBingè¿è¡èå¤©çæä»¶ â¨_ [license] [pypi] [PyPI_-
                               Downloads] [python]
 ## ð ä»ç» ä¸ä¸ªå¯ä»¥ä½¿ç¨æ°çBingè¿è¡èå¤©çæä»¶
-(ç°å¨åä¸éè¦ä»£çäºï¼ ç®åæ¯æ[go-cqhttp](https://docs.go-
+(ç°å¨å**ä¸éè¦**ä»£çäºï¼ ç®åæ¯æ[go-cqhttp](https://docs.go-
 cqhttp.org/)ä¸[onebot v11](https://onebot.adapters.nonebot.dev/)ééå¨å
 [nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-
 patch) QQç¾¤ï¼366731501 ç»ä¸ªstarð? >
 5æä»½æèè¯ï¼ææ¶éç¼æ´æ° > > å¦æä½ ææ´å¤éæ±ï¼è¯·åå¸
 [issue](https://github.com/Harry-Jing/nonebot-plugin-bing-chat/issues/
 new)è®©æç¥é ## ð¿ å®è£ä¸æ´æ°   ä½¿ç¨ nb-cli å®è£ä¸æ´æ°
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
```

### Comparing `nonebot-plugin-bing-chat-0.7.8/pyproject.toml` & `nonebot-plugin-bing-chat-0.7.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bing-chat"
-version = "0.7.8"
+version = "0.7.9"
 description = "基于nonebot2的bing-chat软件"
 authors = [{ name = "Harry", email = "Harry0259@163.com" }]
 readme = "README.md"
 license = { text = "GPL-3" }
 requires-python = ">=3.10"
 dependencies = [
   "EdgeGPT>=0.1.20",
```

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/__init__.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,31 +84,32 @@
     plugin_data.current_cookies_file_path = plugin_data.cookies_file_path_list[0]
 
     # 创建log文件夹
     plugin_log_directory = plugin_directory / 'log'
     plugin_log_directory.mkdir(parents=True, exist_ok=True)
 
     # 检查依赖
+    require('nonebot_plugin_apscheduler')
     if any(i == 'image' for i, _ in plugin_config.bingchat_display_content_types):
-        require('nonebot_plugin_apscheduler')
         try:
             require('nonebot_plugin_htmlrender')
         except Exception as exc:
             raise RuntimeError(
                 '请使用 pip install nonebot-plugin-bing-chat[image] markdown渲染插件'
             ) from exc
 
 
 init()
 
-
+"""
 from nonebot_plugin_apscheduler import scheduler
 
 
 @scheduler.scheduled_job('cron', hour=2)  # type: ignore
 async def _del_log_file() -> None:
     print('del_log_file')
     current_time = datetime.now()
     plugin_log_directory = plugin_config.bingchat_plugin_directory / 'log'
     for child_dir in plugin_log_directory.iterdir():
         if current_time - datetime.fromisoformat(child_dir.name) > timedelta(days=7):
             shutil.rmtree(child_dir)
+"""
```

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/data_model.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/data_model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/exceptions.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/common/utils.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/common/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/check.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/check.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/main.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/main.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat/onebotv11/utils.py` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat/onebotv11/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/PKG-INFO` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bing-chat
-Version: 0.7.8
+Version: 0.7.9
 Summary: 基于nonebot2的bing-chat软件
 Author-email: Harry <Harry0259@163.com>
 License: GPL-3
 Project-URL: Homepage, https://github.com/Harry-Jing/nonebot-plugin-bing-chat
 Classifier: Framework :: Pydantic
 Classifier: Topic :: Communications
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -44,15 +44,15 @@
 
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python" />
 
 </div>
 
 ## 📖 介绍
 
-一个可以使用新版Bing进行聊天的插件 (现在又不需要代理了）
+一个可以使用新版Bing进行聊天的插件 (现在又**不需要**代理了）
 
 目前支持[go-cqhttp](https://docs.go-cqhttp.org/)与[onebot v11](https://onebot.adapters.nonebot.dev/)适配器和[nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-patch)
 
 QQ群：366731501
 
 给个star🌟?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bing-chat Version: 0.7.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bing-chat Version: 0.7.9 Summary:
 åºäºnonebot2çbing-chatè½¯ä»¶ Author-email: Harry
 163.com> License: GPL-3 Project-URL: Homepage, https://github.com/Harry-Jing/
 nonebot-plugin-bing-chat Classifier: Framework :: Pydantic Classifier: Topic ::
 Communications Classifier: License :: OSI Approved :: GNU General Public
 License (GPL) Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
@@ -12,15 +12,15 @@
 File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                         # nonebot-plugin-bing-chat _â¨
 ä¸ä¸ªå¯ä»¥ä½¿ç¨æ°çBingè¿è¡èå¤©çæä»¶ â¨_ [license] [pypi] [PyPI_-
                               Downloads] [python]
 ## ð ä»ç» ä¸ä¸ªå¯ä»¥ä½¿ç¨æ°çBingè¿è¡èå¤©çæä»¶
-(ç°å¨åä¸éè¦ä»£çäºï¼ ç®åæ¯æ[go-cqhttp](https://docs.go-
+(ç°å¨å**ä¸éè¦**ä»£çäºï¼ ç®åæ¯æ[go-cqhttp](https://docs.go-
 cqhttp.org/)ä¸[onebot v11](https://onebot.adapters.nonebot.dev/)ééå¨å
 [nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-
 patch) QQç¾¤ï¼366731501 ç»ä¸ªstarð? >
 5æä»½æèè¯ï¼ææ¶éç¼æ´æ° > > å¦æä½ ææ´å¤éæ±ï¼è¯·åå¸
 [issue](https://github.com/Harry-Jing/nonebot-plugin-bing-chat/issues/
 new)è®©æç¥é ## ð¿ å®è£ä¸æ´æ°   ä½¿ç¨ nb-cli å®è£ä¸æ´æ°
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
```

### Comparing `nonebot-plugin-bing-chat-0.7.8/src/plugins/nonebot_plugin_bing_chat.egg-info/SOURCES.txt` & `nonebot-plugin-bing-chat-0.7.9/src/plugins/nonebot_plugin_bing_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

