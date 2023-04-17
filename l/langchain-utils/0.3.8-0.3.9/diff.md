# Comparing `tmp/langchain_utils-0.3.8.tar.gz` & `tmp/langchain_utils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.3.8.tar", max compression
+gzip compressed data, was "langchain_utils-0.3.9.tar", max compression
```

## Comparing `langchain_utils-0.3.8.tar` & `langchain_utils-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7895 2023-04-12 05:34:44.784594 langchain_utils-0.3.8/README.md
--rw-r--r--   0        0        0       22 2023-04-12 05:34:49.338575 langchain_utils-0.3.8/langchain_utils/__init__.py
--rw-r--r--   0        0        0      222 2023-04-12 05:33:55.491462 langchain_utils-0.3.8/langchain_utils/config.py
--rwxr-xr-x   0        0        0     2630 2023-04-12 05:34:17.215880 langchain_utils-0.3.8/langchain_utils/get_html_prompt.py
--rwxr-xr-x   0        0        0     3373 2023-04-12 04:42:32.076969 langchain_utils-0.3.8/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2660 2023-04-12 05:30:43.018177 langchain_utils-0.3.8/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     2528 2023-04-12 05:21:34.707838 langchain_utils-0.3.8/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.8/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1922 2023-04-12 05:00:54.153184 langchain_utils-0.3.8/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.8/langchain_utils/prompts.py
--rw-r--r--   0        0        0     7841 2023-04-12 05:25:48.783743 langchain_utils-0.3.8/langchain_utils/utils.py
--rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.8/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     1747 2023-04-12 05:34:49.338114 langchain_utils-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     8933 1970-01-01 00:00:00.000000 langchain_utils-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     7895 2023-04-12 05:34:44.784594 langchain_utils-0.3.9/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 05:41:16.700285 langchain_utils-0.3.9/langchain_utils/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-12 05:33:55.491462 langchain_utils-0.3.9/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     2632 2023-04-12 05:40:57.099678 langchain_utils-0.3.9/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     3373 2023-04-12 04:42:32.076969 langchain_utils-0.3.9/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2662 2023-04-12 05:41:02.430563 langchain_utils-0.3.9/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     2528 2023-04-12 05:21:34.707838 langchain_utils-0.3.9/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.9/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1922 2023-04-12 05:00:54.153184 langchain_utils-0.3.9/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.9/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     7841 2023-04-12 05:25:48.783743 langchain_utils-0.3.9/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.9/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     1747 2023-04-12 05:41:16.699453 langchain_utils-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     8933 1970-01-01 00:00:00.000000 langchain_utils-0.3.9/PKG-INFO
```

### Comparing `langchain_utils-0.3.8/README.md` & `langchain_utils-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/langchain_utils/get_html_prompt.py` & `langchain_utils-0.3.9/langchain_utils/get_html_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         '--merge',
         help='Merge contents of all pages before processing',
         action='store_true',
     )
 
     args = parser.parse_args()
     if not args.path:
-        args.path = save_stdin_to_tempfile()
+        args.path = [save_stdin_to_tempfile()]
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
```

### Comparing `langchain_utils-0.3.8/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.3.9/langchain_utils/get_pdf_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/langchain_utils/get_text_prompt.py` & `langchain_utils-0.3.9/langchain_utils/get_text_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         '--merge',
         help='Merge contents of all pages before processing',
         action='store_true',
     )
 
     args = parser.parse_args()
     if not args.path:
-        args.path = save_stdin_to_tempfile()
+        args.path = [save_stdin_to_tempfile()]
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
```

### Comparing `langchain_utils-0.3.8/langchain_utils/get_url_prompt.py` & `langchain_utils-0.3.9/langchain_utils/get_url_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.3.9/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/langchain_utils/loaders.py` & `langchain_utils-0.3.9/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/langchain_utils/utils.py` & `langchain_utils-0.3.9/langchain_utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/langchain_utils/utils_argparse.py` & `langchain_utils-0.3.9/langchain_utils/utils_argparse.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.8/pyproject.toml` & `langchain_utils-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.3.8/PKG-INFO` & `langchain_utils-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

