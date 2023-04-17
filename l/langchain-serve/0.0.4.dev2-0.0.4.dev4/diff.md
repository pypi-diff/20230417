# Comparing `tmp/langchain-serve-0.0.4.dev2.tar.gz` & `tmp/langchain-serve-0.0.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-serve-0.0.4.dev2.tar", last modified: Sat Apr 15 00:04:43 2023, max compression
+gzip compressed data, was "langchain-serve-0.0.4.dev4.tar", last modified: Mon Apr 17 05:38:02 2023, max compression
```

## Comparing `langchain-serve-0.0.4.dev2.tar` & `langchain-serve-0.0.4.dev4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.519154 langchain-serve-0.0.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-15 00:04:43.519154 langchain-serve-0.0.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.515154 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/langchain_serve.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.515154 langchain-serve-0.0.4.dev2/lcserve/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-15 00:04:43.000000 langchain-serve-0.0.4.dev2/lcserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/agent-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.511154 langchain-serve-0.0.4.dev2/lcserve/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.515154 langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.515154 langchain-serve-0.0.4.dev2/lcserve/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/agentexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.515154 langchain-serve-0.0.4.dev2/lcserve/backend/playground/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.519154 langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/langchain_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/customgateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/customgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.511154 langchain-serve-0.0.4.dev2/lcserve/playground/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:04:43.519154 langchain-serve-0.0.4.dev2/lcserve/playground/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/playground/babyagi/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/playground/babyagi/user_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/playgroundgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/servinggateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/lcserve/servinggateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 00:04:43.519154 langchain-serve-0.0.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-15 00:04:37.000000 langchain-serve-0.0.4.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.862613 langchain-serve-0.0.4.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-17 05:38:02.862613 langchain-serve-0.0.4.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.854613 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/langchain_serve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.854613 langchain-serve-0.0.4.dev4/lcserve/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-17 05:38:02.000000 langchain-serve-0.0.4.dev4/lcserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/agent-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.846613 langchain-serve-0.0.4.dev4/lcserve/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.858613 langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/babyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.858613 langchain-serve-0.0.4.dev4/lcserve/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/agentexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.858613 langchain-serve-0.0.4.dev4/lcserve/backend/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.862613 langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/langchain_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/customgateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/customgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.846613 langchain-serve-0.0.4.dev4/lcserve/playground/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:38:02.862613 langchain-serve-0.0.4.dev4/lcserve/playground/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/playground/babyagi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/playground/babyagi/user_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/playgroundgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/servinggateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/lcserve/servinggateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:38:02.862613 langchain-serve-0.0.4.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-17 05:37:57.000000 langchain-serve-0.0.4.dev4/setup.py
```

### Comparing `langchain-serve-0.0.4.dev2/LICENSE` & `langchain-serve-0.0.4.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/PKG-INFO` & `langchain-serve-0.0.4.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.4.dev2
+Version: 0.0.4.dev4
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

### Comparing `langchain-serve-0.0.4.dev2/README.md` & `langchain-serve-0.0.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/langchain_serve.egg-info/PKG-INFO` & `langchain-serve-0.0.4.dev4/langchain_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.4.dev2
+Version: 0.0.4.dev4
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

### Comparing `langchain-serve-0.0.4.dev2/langchain_serve.egg-info/SOURCES.txt` & `langchain-serve-0.0.4.dev4/langchain_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/__main__.py` & `langchain-serve-0.0.4.dev4/lcserve/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 from typing import List, Union
 
 import click
 from jcloud.constants import Phase
 from jina import Flow
 
+from . import __version__
 from .flow import (
     APP_NAME,
     BABYAGI_APP_NAME,
     deploy_app_on_jcloud,
     get_app_status_on_jcloud,
     get_flow_dict,
     get_flow_yaml,
@@ -29,23 +30,25 @@
 
 
 async def serve_on_jcloud(
     module: Union[str, List[str]],
     name: str = APP_NAME,
     requirements: List[str] = None,
     app_id: str = None,
+    version: str = 'latest',
     verbose: bool = False,
 ):
     from .backend.playground.utils.helper import get_random_tag
 
     tag = get_random_tag()
     gateway_id_wo_tag, is_websocket = push_app_to_hubble(
         module,
         requirements=requirements,
         tag=tag,
+        version=version,
         verbose=verbose,
     )
     app_id, endpoint = await deploy_app_on_jcloud(
         flow_dict=get_flow_dict(
             module=module,
             jcloud=True,
             port=8080,
@@ -60,27 +63,31 @@
     await get_app_status_on_jcloud(app_id=app_id)
 
 
 async def serve_babyagi_on_jcloud(
     name: str = BABYAGI_APP_NAME,
     requirements: List[str] = None,
     app_id: str = None,
+    version: str = 'latest',
     verbose: bool = False,
 ):
     await serve_on_jcloud(
         module='lcserve.apps.babyagi.app',
         name=name,
         requirements=requirements,
         app_id=app_id,
+        version=version,
         verbose=verbose,
     )
 
 
 @click.group()
+@click.version_option(__version__, '-v', '--version', prog_name='lc-serve')
 @click.help_option('-h', '--help')
+@click.pass_context
 def serve():
     pass
 
 
 @serve.group(help='Deploy the app.')
 @click.help_option('-h', '--help')
 def deploy():
@@ -121,23 +128,36 @@
     '--app-id',
     type=str,
     default=None,
     help='AppID of the deployed agent to be updated.',
     show_default=True,
 )
 @click.option(
+    '--version',
+    type=str,
+    default='latest',
+    help='Version of serving gateway to be used.',
+    show_default=False,
+)
+@click.option(
     '--verbose',
     is_flag=True,
     help='Verbose mode.',
     show_default=True,
 )
 @click.help_option('-h', '--help')
 @syncify
-async def jcloud(module, name, app_id, verbose):
-    await serve_on_jcloud(module, name=name, app_id=app_id, verbose=verbose)
+async def jcloud(module, name, app_id, version, verbose):
+    await serve_on_jcloud(
+        module,
+        name=name,
+        app_id=app_id,
+        version=version,
+        verbose=verbose,
+    )
 
 
 @deploy.command(help='Deploy babyagi on JCloud.')
 @click.option(
     '--name',
     type=str,
     default=BABYAGI_APP_NAME,
@@ -154,26 +174,34 @@
     '--app-id',
     type=str,
     default=None,
     help='AppID of the deployed agent to be updated.',
     show_default=True,
 )
 @click.option(
+    '--version',
+    type=str,
+    default='latest',
+    help='Version of serving gateway to be used.',
+    show_default=False,
+)
+@click.option(
     '--verbose',
     is_flag=True,
     help='Verbose mode.',
     show_default=True,
 )
 @click.help_option('-h', '--help')
 @syncify
-async def babyagi(name, requirements, app_id, verbose):
+async def babyagi(name, requirements, app_id, version, verbose):
     await serve_babyagi_on_jcloud(
         name=name,
         requirements=requirements,
         app_id=app_id,
+        version=version,
         verbose=verbose,
     )
 
 
 @serve.command(help='List all deployed apps.')
 @click.option(
     '--phase',
```

### Comparing `langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/app.py` & `langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/apps/babyagi/babyagi.py` & `langchain-serve-0.0.4.dev4/lcserve/apps/babyagi/babyagi.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/agentexecutor.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/agentexecutor.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/decorators.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/decorators.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/gateway.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/nginx.conf` & `langchain-serve-0.0.4.dev4/lcserve/backend/nginx.conf`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/playground/app.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/playground/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/helper.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/langchain_helper.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/langchain_helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/talk.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/talk.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/backend/playground/utils/tools.py` & `langchain-serve-0.0.4.dev4/lcserve/backend/playground/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/customgateway.Dockerfile` & `langchain-serve-0.0.4.dev4/lcserve/customgateway.Dockerfile`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/flow.py` & `langchain-serve-0.0.4.dev4/lcserve/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         sys.path.append(os.path.join(os.path.dirname(__file__), 'apps', app))
 
 
 def push_app_to_hubble(
     mod: str,
     tag: str = 'latest',
     requirements: Tuple[str] = None,
+    version: str = 'latest',
     verbose: Optional[bool] = False,
 ) -> Tuple[str, bool]:
     from hubble.executor.hubio import HubIO
     from hubble.executor.parsers import set_hub_push_parser
 
     from .backend.playground.utils.helper import get_random_name
 
@@ -213,15 +214,15 @@
 
         with open(os.path.join(tmpdir, 'requirements.txt'), 'w') as f:
             f.write('\n'.join(requirements))
 
     # Create the Dockerfile
     with open(os.path.join(tmpdir, 'Dockerfile'), 'w') as f:
         dockerfile = [
-            'FROM jinawolf/serving-gateway:latest',
+            f'FROM jinawolf/serving-gateway:{version}',
             'COPY . /appdir/',
             'RUN if [ -e /appdir/requirements.txt ]; then pip install -r /appdir/requirements.txt; fi',
             'ENTRYPOINT [ "jina", "gateway", "--uses", "config.yml" ]',
         ]
         f.write('\n\n'.join(dockerfile))
 
     # Create the config.yml
```

### Comparing `langchain-serve-0.0.4.dev2/lcserve/flow.yml` & `langchain-serve-0.0.4.dev4/lcserve/flow.yml`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/playground/babyagi/playground.py` & `langchain-serve-0.0.4.dev4/lcserve/playground/babyagi/playground.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/lcserve/playground/babyagi/user_input.py` & `langchain-serve-0.0.4.dev4/lcserve/playground/babyagi/user_input.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.4.dev2/setup.py` & `langchain-serve-0.0.4.dev4/setup.py`

 * *Files identical despite different names*

