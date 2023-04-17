# Comparing `tmp/promptx-0.0.5.tar.gz` & `tmp/promptx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptx-0.0.5.tar", last modified: Fri Apr 14 00:37:15 2023, max compression
+gzip compressed data, was "promptx-0.0.6.tar", last modified: Mon Apr 17 02:28:30 2023, max compression
```

## Comparing `promptx-0.0.5.tar` & `promptx-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:37:15.776136 promptx-0.0.5/
--rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.5/LICENSE.md
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-14 00:37:15.776136 promptx-0.0.5/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.5/README.md
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:37:15.772803 promptx-0.0.5/promptx/
--rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.5/promptx/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     5056 2023-04-14 00:35:36.000000 promptx-0.0.5/promptx/promptx.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:37:15.776136 promptx-0.0.5/promptx.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/top_level.txt
--rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-14 00:35:50.000000 promptx-0.0.5/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:37:15.776136 promptx-0.0.5/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 02:28:30.159267 promptx-0.0.6/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.6/LICENSE.md
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-17 02:28:30.159267 promptx-0.0.6/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.6/README.md
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 02:28:30.159267 promptx-0.0.6/promptx/
+-rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.6/promptx/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     5090 2023-04-17 02:26:29.000000 promptx-0.0.6/promptx/promptx.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 02:28:30.159267 promptx-0.0.6/promptx.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/top_level.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-17 02:26:45.000000 promptx-0.0.6/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-17 02:28:30.159267 promptx-0.0.6/setup.cfg
```

### Comparing `promptx-0.0.5/LICENSE.md` & `promptx-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.5/PKG-INFO` & `promptx-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `promptx-0.0.5/README.md` & `promptx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.5/promptx/promptx.py` & `promptx-0.0.6/promptx/promptx.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,22 +128,23 @@
 
         # Reset temp_args
         self.temp_args = []
         # Create one long string similar to choice=$(printf '%s\n' "$@" | dmenu) in bash
         opts_str = deliminator.join(map(str, options))
         # Open stdin and populate choices
         outs, errs = proc.communicate(input=opts_str)
+        ret_list = outs.rstrip().splitlines()
         if proc.wait() != 0:
             # If no err return None as user hit escape
             if errs == "":
-                return []
+                return ret_list
             # Otherwise some error occured
             raise PromptXError(cmd, errs)
 
-        return outs.rstrip().splitlines()
+        return ret_list
 
     def add_args(
         self,
         additional_args: List,
         default_args: bool = False,
     ):
         """
```

### Comparing `promptx-0.0.5/promptx.egg-info/PKG-INFO` & `promptx-0.0.6/promptx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

