# Comparing `tmp/discordwrap-0.6.2.tar.gz` & `tmp/discordwrap-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordwrap-0.6.2.tar", max compression
+gzip compressed data, was "discordwrap-0.7.0.tar", max compression
```

## Comparing `discordwrap-0.6.2.tar` & `discordwrap-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       74 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/Auth/Auth.py
--rw-r--r--   0        0        0       20 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/Auth/__init__.py
--rw-r--r--   0        0        0      584 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/Errors/Errors.py
--rw-r--r--   0        0        0       22 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/Errors/__init__.py
--rw-r--r--   0        0        0       85 2023-03-31 00:47:05.679048 discordwrap-0.6.2/discordwrap/__init__.py
--rw-r--r--   0        0        0       23 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/core/__init__.py
--rw-r--r--   0        0        0     5712 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/core/request.py
--rw-r--r--   0        0        0       22 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/methods/__init__.py
--rw-r--r--   0        0        0      682 2023-03-31 00:46:38.354778 discordwrap-0.6.2/discordwrap/methods/channel.py
--rw-r--r--   0        0        0      783 2023-03-31 00:47:05.687048 discordwrap-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 discordwrap-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/Auth/Auth.py
+-rw-r--r--   0        0        0       20 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/Auth/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/Errors/Errors.py
+-rw-r--r--   0        0        0       22 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/Errors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-17 04:02:51.787876 discordwrap-0.7.0/discordwrap/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/core/__init__.py
+-rw-r--r--   0        0        0     5712 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/core/request.py
+-rw-r--r--   0        0        0       22 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/methods/__init__.py
+-rw-r--r--   0        0        0      682 2023-04-17 04:02:24.923615 discordwrap-0.7.0/discordwrap/methods/channel.py
+-rw-r--r--   0        0        0      783 2023-04-17 04:02:51.795876 discordwrap-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 discordwrap-0.7.0/PKG-INFO
```

### Comparing `discordwrap-0.6.2/discordwrap/Errors/Errors.py` & `discordwrap-0.7.0/discordwrap/Errors/Errors.py`

 * *Files identical despite different names*

### Comparing `discordwrap-0.6.2/discordwrap/core/request.py` & `discordwrap-0.7.0/discordwrap/core/request.py`

 * *Files identical despite different names*

### Comparing `discordwrap-0.6.2/discordwrap/methods/channel.py` & `discordwrap-0.7.0/discordwrap/methods/channel.py`

 * *Files identical despite different names*

### Comparing `discordwrap-0.6.2/pyproject.toml` & `discordwrap-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordwrap"
-version = "0.6.2"
+version = "0.7.0"
 description = ""
 authors = ["josh <josh@brunuslabs.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
```

