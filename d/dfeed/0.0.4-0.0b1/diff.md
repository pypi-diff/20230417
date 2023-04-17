# Comparing `tmp/dfeed-0.0.4.tar.gz` & `tmp/dfeed-0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfeed-0.0.4.tar", last modified: Mon Apr 17 05:19:43 2023, max compression
+gzip compressed data, was "dfeed-0.0b1.tar", last modified: Tue Apr 11 17:49:32 2023, max compression
```

## Comparing `dfeed-0.0.4.tar` & `dfeed-0.0b1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 05:19:43.416359 dfeed-0.0.4/
--rw-r--r--   0 anon      (1000) wheel      (998)    34946 2023-04-11 17:54:43.000000 dfeed-0.0.4/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)      602 2023-04-17 05:19:43.416359 dfeed-0.0.4/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      292 2023-04-14 05:24:00.000000 dfeed-0.0.4/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      531 2023-04-17 04:54:20.000000 dfeed-0.0.4/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-17 05:19:43.416359 dfeed-0.0.4/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 05:19:43.413025 dfeed-0.0.4/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 05:19:43.416359 dfeed-0.0.4/src/dfeed/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dfeed-0.0.4/src/dfeed/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      994 2023-04-14 06:35:15.000000 dfeed-0.0.4/src/dfeed/__main__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     1098 2023-04-14 06:36:00.000000 dfeed-0.0.4/src/dfeed/args.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1353 2023-04-14 06:01:00.000000 dfeed-0.0.4/src/dfeed/config.py
--rw-r--r--   0 anon      (1000) wheel      (998)     2769 2023-04-14 02:59:37.000000 dfeed-0.0.4/src/dfeed/list_feed.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      200 2023-04-11 17:46:36.000000 dfeed-0.0.4/src/dfeed/media.py
--rw-r--r--   0 anon      (1000) wheel      (998)     1289 2023-04-13 22:59:40.000000 dfeed-0.0.4/src/dfeed/opener.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2787 2023-04-14 06:35:30.000000 dfeed-0.0.4/src/dfeed/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1180 2023-04-14 00:34:56.000000 dfeed-0.0.4/src/dfeed/prompts.py
--rw-r--r--   0 anon      (1000) wheel      (998)     9054 2023-04-15 15:48:31.000000 dfeed-0.0.4/src/dfeed/sfeed.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2622 2023-04-17 05:17:32.000000 dfeed-0.0.4/src/dfeed/system.py
--rw-r--r--   0 anon      (1000) wheel      (998)     1793 2023-04-13 22:59:40.000000 dfeed-0.0.4/src/dfeed/user.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4517 2023-04-13 18:56:57.000000 dfeed-0.0.4/src/dfeed/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 05:19:43.416359 dfeed-0.0.4/src/dfeed.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      602 2023-04-17 05:19:43.000000 dfeed-0.0.4/src/dfeed.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      494 2023-04-17 05:19:43.000000 dfeed-0.0.4/src/dfeed.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-17 05:19:43.000000 dfeed-0.0.4/src/dfeed.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       46 2023-04-17 05:19:43.000000 dfeed-0.0.4/src/dfeed.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       24 2023-04-17 05:19:43.000000 dfeed-0.0.4/src/dfeed.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        6 2023-04-17 05:19:43.000000 dfeed-0.0.4/src/dfeed.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34935 2023-04-11 17:49:00.000000 dfeed-0.0b1/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)      495 2023-04-11 17:49:32.033579 dfeed-0.0b1/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      185 2023-04-11 07:21:35.000000 dfeed-0.0b1/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      525 2023-04-11 17:46:18.000000 dfeed-0.0b1/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-11 17:49:32.033579 dfeed-0.0b1/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.030245 dfeed-0.0b1/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/src/dfeed/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dfeed-0.0b1/src/dfeed/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      962 2023-04-11 17:48:09.000000 dfeed-0.0b1/src/dfeed/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      881 2023-04-11 07:28:03.000000 dfeed-0.0b1/src/dfeed/config.py
+-rw-r--r--   0 anon      (1000) wheel      (998)      275 2023-04-11 17:33:52.000000 dfeed-0.0b1/src/dfeed/list_feed.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      200 2023-04-11 17:46:36.000000 dfeed-0.0b1/src/dfeed/media.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/src/dfeed/not_needed/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 dfeed-0.0b1/src/dfeed/not_needed/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 dfeed-0.0b1/src/dfeed/not_needed/g_dl.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 dfeed-0.0b1/src/dfeed/not_needed/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 dfeed-0.0b1/src/dfeed/not_needed/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      694 2023-04-11 07:24:52.000000 dfeed-0.0b1/src/dfeed/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1190 2023-04-11 17:47:13.000000 dfeed-0.0b1/src/dfeed/prompts.py
+-rw-r--r--   0 anon      (1000) wheel      (998)      350 2023-04-11 17:41:04.000000 dfeed-0.0b1/src/dfeed/sfeed.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1801 2023-04-11 17:32:45.000000 dfeed-0.0b1/src/dfeed/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2026 2023-04-11 17:30:42.000000 dfeed-0.0b1/src/dfeed/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/src/dfeed.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)      495 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      566 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       46 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       17 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        6 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/top_level.txt
```

### Comparing `dfeed-0.0.4/LICENSE` & `dfeed-0.0b1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -556,15 +556,15 @@
 everyone can redistribute and change under these terms.
 
 To do so, attach the following notices to the program. It is safest to attach
 them to the start of each source file to most effectively state the exclusion of
 warranty; and each file should have at least the “copyright” line and a pointer
 to where the full notice is found.
 
-     dfeed - dmenu + sfeed (works with fzf, and rofi too)
+     dfeed - a useful dmenu wrapper for sfeed.
      read.  Copyright (C) 2022 John Dovern
 
      This program is free software: you can redistribute it and/or modify it
      under the terms of the GNU General Public License as published by the Free
      Software Foundation, either version 3 of the License, or (at your option)
      any later version.
```

### Comparing `dfeed-0.0.4/pyproject.toml` & `dfeed-0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfeed"
-version = "0.0.4"
+version = "0.0.b1"
 description = "dfeed - dmenu + sfeed (works with fzf, and rofi too)"
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv", "sfeed", "dmenu" ]
 dependencies = [
     "loadconf",
-    "promptx>=0.0.6"
+    "promptx"
 ]
 
 [project.optional-dependencies]
 
 [project.scripts]
 dfeed = "dfeed.__main__:main"
```

### Comparing `dfeed-0.0.4/src/dfeed/__main__.py` & `dfeed-0.0b1/src/dfeed/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python3
 import shlex
 import sys
 
-from .args import Args
 from .config import get_user_settings
+from .sfeed import get_feeds
+
+# from .media import
 from .options import get_opts
-from .sfeed import get_feed_files
 from .system import open_process
-from .user import User
 from .utils import cprint
-from .list_feed import show_list
 
 
 __license__ = "GPL-v3.0"
 __program__ = "dfeed"
 
 
-def process_opts():
+def process_opts(user, args):
     """
     Opts handler for main
     """
-    return show_list()
+    if args.list:
+        return get_feeds(user, args)
+    else:
+        return 1
 
 
 def main():
     """
     Command line application to integrate dmenu into sfeed
     """
     # Set and get command line args
     args = get_opts(__program__)
 
     # Creates a UserSettings object. This will be used by various function
     # to access file paths, settings, filters, and command line args
     user, args = get_user_settings(program=__program__, args=args)
 
-    User.define_user(user)
-    Args.define_args(args)
     # Execute the appropriate function based on command line options
-    return process_opts()
+    return process_opts(user, args=args)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `dfeed-0.0.4/src/dfeed/prompts.py` & `dfeed-0.0b1/src/dfeed/prompts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 #!/usr/bin/env python3
 from promptx import PromptX
-from typing import List
-
-from .user import User
-
-# from .utils import cprint
+from .utils import cprint
 
 
 class InvalidCmdPrompt(Exception):
     """Exception raised when user has invalid command prompt"""
 
     def __init__(self, error, message="ERROR: prompt_cmd not recognized"):
         self.error = error
@@ -27,23 +23,28 @@
         self.message = message
 
     def __str__(self):
         return f"{self.prefix}{self.message}{self.error}"
 
 
 def user_choice(
-    options: List[str],
-    # cmd: str,
-    # cmd_args: str,
-    prompt: str,
+    options,
+    user,
+    prompt,
 ):
     """
     Give user a prompt to choose from a list of options.  Uses dmenu, fzf, or
     rofi
     """
-    p = PromptX(prompt_cmd=User.settings_str("prompt_cmd"))
+    cmd = user.settings["prompt_cmd"]
+    cmd_args = user.settings["prompt_args"]
+    p = PromptX(prompt_cmd=cmd)
+    if cmd == "dmenu" and cmd_args == "":
+        cmd_args = "-l 20 -i"
+
     choice = p.ask(
         options=options,
         prompt=prompt,
-        additional_args=User.settings_str("prompt_args"),
+        additional_args=cmd_args,
     )
+
     return choice
```

### Comparing `dfeed-0.0.4/src/dfeed/system.py` & `dfeed-0.0b1/src/dfeed/system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,55 @@
 #!/usr/bin/env python3
+import mimetypes
 import os
 import pathlib
 import re
 import requests
 import subprocess
+import sys
+import shlex
+import shutil
 import time
-from typing import List
 
 
 class OpenerError(Exception):
     """Exception raised when command fails"""
 
     def __init__(self, error, message="ERROR: Failed to run"):
         self.error = error
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return f"{self.message} {self.error}"
 
 
-def curl_links(
-    raw_links: List[str],
-    curl_regexs: List[str],
-    temp_dir: str,
-) -> List[str]:
-    links = []
-    for link in raw_links:
-        match_found = False
-        for regex in curl_regexs:
-            link_match = re.search(regex, link)
-            if link_match is not None:
-                match_found = True
-                break
-        if match_found:
-            links.append(curl_url(link, temp_dir))
-        else:
-            links.append(link)
-    return links
-
-
-def curl_url(url: str, temp_dir: str) -> str:
-    result = re.search(r"/(.[^/]+$)", url)
+def curl_torrent(torrent_url, user):
+    result = re.search(r"/(.[^/]+\.torrent$)", torrent_url)
     if result is None or len(result.groups()) == 0:
-        return url
-    temp_path = pathlib.Path(temp_dir)
-    if not temp_path.exists():
-        temp_path.mkdir(mode=0o700, parents=True)
-    possible_dups = list(temp_path.glob(f"*_{result.group(1)}"))
-    if len(possible_dups) == 0:
-        curl_file = str(time.time()) + "_" + result.group(1)
-        response = requests.get(url)
-        curl_path = temp_path / curl_file
-        with curl_path.open("wb") as out_file:
-            out_file.write(response.content)
-        return_path = curl_path
-    else:
-        return_path = possible_dups[0]
-    return f"{return_path}"
+        return
+    torrent_file = str(int(time.time())) + "_" + result.group(1)
+    response = requests.get(torrent_url)
+    with open(f'{user.settings["temp_dir"]}/{torrent_file}', "wb") as out_file:
+        out_file.write(response.content)
 
 
-def get_files(path: pathlib.Path) -> List[pathlib.Path]:
+def get_files(path: pathlib.Path):
     # list all files and directories under the given path
     entries = os.listdir(path)
     # filter out the directories
     files = [
         pathlib.Path(path, entry)
         for entry in entries
         if os.path.isfile(pathlib.Path(path, entry))
     ]
     return files
 
 
-def open_process(opener: List[str], out=subprocess.DEVNULL, err=subprocess.STDOUT):
+def open_process(opener, out=subprocess.DEVNULL, err=subprocess.STDOUT):
     """Open a program with the given opener list"""
     try:
         subprocess.Popen(opener, stdout=out, stderr=err)
     except (subprocess.CalledProcessError, FileNotFoundError):
         raise OpenerError(opener)
```

