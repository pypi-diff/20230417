# Comparing `tmp/khoj_assistant-0.6.1.dev3.tar.gz` & `tmp/khoj_assistant-0.6.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Apr 16 13:22:51 2023, max compression
+gzip compressed data, last modified: Mon Apr 17 09:55:33 2023, max compression
```

## Comparing `khoj_assistant-0.6.1.dev3.tar` & `khoj_assistant-0.6.1.dev5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/__init__.py
--rw-r--r--   0        0        0     9136 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/configure.py
--rw-r--r--   0        0        0     4911 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2904 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      861 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    15746 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9631 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    11635 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      438 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      406 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4515 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     3515 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     8972 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     5182 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3930 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5701 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     5898 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6116 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0     9613 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10755 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2325 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2381 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     4258 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/models.py
--rw-r--r--   0        0        0     3463 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0      977 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/.gitignore
--rw-r--r--   0        0        0    32472 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/LICENSE
--rw-r--r--   0        0        0    21780 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/README.md
--rw-r--r--   0        0        0     2650 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/pyproject.toml
--rw-r--r--   0        0        0    23925 2023-04-16 13:22:51.000000 khoj_assistant-0.6.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/__init__.py
+-rw-r--r--   0        0        0     9136 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2904 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      861 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    15746 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9631 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    11635 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      438 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      406 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4515 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     3515 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     8972 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     5182 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3930 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5701 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     5898 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6116 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0     9613 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10755 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2325 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2381 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     4258 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     3463 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0      977 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/.gitignore
+-rw-r--r--   0        0        0    32472 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/LICENSE
+-rw-r--r--   0        0        0    21780 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/README.md
+-rw-r--r--   0        0        0     2650 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0    23925 2023-04-17 09:55:33.000000 khoj_assistant-0.6.1.dev5/PKG-INFO
```

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/configure.py` & `khoj_assistant-0.6.1.dev5/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/main.py` & `khoj_assistant-0.6.1.dev5/src/khoj/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     # Set Logging Level
     if args.verbose == 0:
         logger.setLevel(logging.INFO)
     elif args.verbose >= 1:
         logger.setLevel(logging.DEBUG)
 
     # Set Log File
-    fh = logging.FileHandler(state.config_file.parent / "khoj.log")
+    fh = logging.FileHandler(state.config_file.parent / "khoj.log", encoding="utf-8")
     fh.setLevel(logging.DEBUG)
     logger.addHandler(fh)
 
     logger.info("🌘 Starting Khoj")
 
     if args.no_gui:
         # Setup task scheduler
```

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/config.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.1.dev5/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.1.dev5/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/routers/api.py` & `khoj_assistant-0.6.1.dev5/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.1.dev5/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.1.dev5/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.1.dev5/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.1.dev5/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.1.dev5/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.1.dev5/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.1.dev5/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/cli.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/config.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/constants.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/models.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/state.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.1.dev5/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/.gitignore` & `khoj_assistant-0.6.1.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/LICENSE` & `khoj_assistant-0.6.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/README.md` & `khoj_assistant-0.6.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/pyproject.toml` & `khoj_assistant-0.6.1.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.1.dev3/PKG-INFO` & `khoj_assistant-0.6.1.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.1.dev3
+Version: 0.6.1.dev5
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

