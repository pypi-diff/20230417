# Comparing `tmp/aiogram-ext-0.0.8.tar.gz` & `tmp/aiogram-ext-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.0.8.tar", last modified: Thu Apr 13 14:08:35 2023, max compression
+gzip compressed data, was "aiogram-ext-0.0.9.tar", last modified: Thu Apr 13 14:15:48 2023, max compression
```

## Comparing `aiogram-ext-0.0.8.tar` & `aiogram-ext-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      855 2023-04-13 14:00:40.168816 aiogram-ext-0.0.8/aiogram_ext/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.8/aiogram_ext/buttons.py
--rw-r--r--   0        0        0      269 2023-04-13 14:01:13.830112 aiogram-ext-0.0.8/aiogram_ext/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.8/aiogram_ext/context.py
--rw-r--r--   0        0        0     1483 2023-04-13 14:00:40.159310 aiogram-ext-0.0.8/aiogram_ext/deps.py
--rw-r--r--   0        0        0     5887 2023-04-12 11:08:56.310732 aiogram-ext-0.0.8/aiogram_ext/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.0.8/aiogram_ext/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.8/aiogram_ext/filters.py
--rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.8/aiogram_ext/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.0.8/aiogram_ext/keyboards.py
--rw-r--r--   0        0        0      810 2023-04-13 14:08:18.534155 aiogram-ext-0.0.8/aiogram_ext/loader.py
--rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.8/aiogram_ext/middlewares/__init__.py
--rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.8/aiogram_ext/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.8/aiogram_ext/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.8/aiogram_ext/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.8/aiogram_ext/middlewares/throttling.py
--rw-r--r--   0        0        0      594 2023-04-13 13:42:05.708666 aiogram-ext-0.0.8/aiogram_ext/texts.py
--rw-r--r--   0        0        0      367 2023-04-13 14:08:32.244323 aiogram-ext-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.8/README.md
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      855 2023-04-13 14:00:40.168816 aiogram-ext-0.0.9/aiogram_ext/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.9/aiogram_ext/buttons.py
+-rw-r--r--   0        0        0      269 2023-04-13 14:01:13.830112 aiogram-ext-0.0.9/aiogram_ext/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.9/aiogram_ext/context.py
+-rw-r--r--   0        0        0     1483 2023-04-13 14:00:40.159310 aiogram-ext-0.0.9/aiogram_ext/deps.py
+-rw-r--r--   0        0        0     5981 2023-04-13 14:15:39.821528 aiogram-ext-0.0.9/aiogram_ext/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.0.9/aiogram_ext/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.9/aiogram_ext/filters.py
+-rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.9/aiogram_ext/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.0.9/aiogram_ext/keyboards.py
+-rw-r--r--   0        0        0      810 2023-04-13 14:08:18.534155 aiogram-ext-0.0.9/aiogram_ext/loader.py
+-rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.9/aiogram_ext/middlewares/__init__.py
+-rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.9/aiogram_ext/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.9/aiogram_ext/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.9/aiogram_ext/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.9/aiogram_ext/middlewares/throttling.py
+-rw-r--r--   0        0        0      594 2023-04-13 13:42:05.708666 aiogram-ext-0.0.9/aiogram_ext/texts.py
+-rw-r--r--   0        0        0      367 2023-04-13 14:15:43.996408 aiogram-ext-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.9/README.md
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.9/PKG-INFO
```

### Comparing `aiogram-ext-0.0.8/aiogram_ext/__init__.py` & `aiogram-ext-0.0.9/aiogram_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/buttons.py` & `aiogram-ext-0.0.9/aiogram_ext/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/context.py` & `aiogram-ext-0.0.9/aiogram_ext/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/deps.py` & `aiogram-ext-0.0.9/aiogram_ext/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/dispatcher.py` & `aiogram-ext-0.0.9/aiogram_ext/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,17 @@
     ):
         payload = self._gen_payload(locals(), exclude=["custom_filters"])
         return super().inline_handler(*custom_filters, **payload)
 
     def command(self, command: str, state: str = None):
         return self.message_handler(commands=command, state=state)
 
+    def start(self, state: str | None = "*"):
+        return self.command("start", state)
+
     def button(self, button: CallbackButton):
         return self.callback_query_handler(button=button)
 
     def text(self, text: str = None, state: str | State = None):
         return self.message_handler(button=text, state=state)
 
     def contact(self, state: str | State = None):
```

### Comparing `aiogram-ext-0.0.8/aiogram_ext/env.py` & `aiogram-ext-0.0.9/aiogram_ext/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/filters.py` & `aiogram-ext-0.0.9/aiogram_ext/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/keyboards.py` & `aiogram-ext-0.0.9/aiogram_ext/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/loader.py` & `aiogram-ext-0.0.9/aiogram_ext/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/middlewares/_conversation.py` & `aiogram-ext-0.0.9/aiogram_ext/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/middlewares/_membership.py` & `aiogram-ext-0.0.9/aiogram_ext/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/middlewares/misc.py` & `aiogram-ext-0.0.9/aiogram_ext/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/middlewares/throttling.py` & `aiogram-ext-0.0.9/aiogram_ext/middlewares/throttling.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.8/aiogram_ext/texts.py` & `aiogram-ext-0.0.9/aiogram_ext/texts.py`

 * *Files identical despite different names*

