# Comparing `tmp/eml_rename-0.2.0.tar.gz` & `tmp/eml_rename-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eml_rename-0.2.0.tar", last modified: Sat Nov 12 19:13:21 2022, max compression
+gzip compressed data, was "eml_rename-0.3.0.tar", max compression
```

## Comparing `eml_rename-0.2.0.tar` & `eml_rename-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.085879 eml_rename-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      118 2022-11-06 06:31:24.000000 eml_rename-0.2.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)    35149 2022-11-05 05:00:16.000000 eml_rename-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      179 2022-11-05 05:19:08.000000 eml_rename-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      676 2022-11-12 19:13:21.084879 eml_rename-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1206 2022-11-12 19:10:51.000000 eml_rename-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.078879 eml_rename-0.2.0/eml_rename/
--rw-r--r--   0 root         (0) root         (0)      146 2022-11-12 19:10:04.000000 eml_rename-0.2.0/eml_rename/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8737 2022-11-12 19:07:16.000000 eml_rename-0.2.0/eml_rename/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.082879 eml_rename-0.2.0/eml_rename/locale/
--rw-r--r--   0 root         (0) root         (0)     1684 2022-11-12 19:10:59.000000 eml_rename-0.2.0/eml_rename/locale/eml_rename.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.074879 eml_rename-0.2.0/eml_rename/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.082879 eml_rename-0.2.0/eml_rename/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      424 2022-11-12 19:10:59.000000 eml_rename-0.2.0/eml_rename/locale/en/LC_MESSAGES/eml_rename.mo
--rw-r--r--   0 root         (0) root         (0)      738 2022-04-25 13:52:57.000000 eml_rename-0.2.0/eml_rename/locale/en.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.074879 eml_rename-0.2.0/eml_rename/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.083879 eml_rename-0.2.0/eml_rename/locale/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     2338 2022-11-12 19:10:59.000000 eml_rename-0.2.0/eml_rename/locale/es/LC_MESSAGES/eml_rename.mo
--rw-r--r--   0 root         (0) root         (0)     2654 2022-11-06 06:29:19.000000 eml_rename-0.2.0/eml_rename/locale/es.po
--rw-r--r--   0 root         (0) root         (0)     2598 2022-11-06 06:20:41.000000 eml_rename-0.2.0/eml_rename/locale/es.po~
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.084879 eml_rename-0.2.0/eml_rename/reusing/
--rw-r--r--   0 root         (0) root         (0)    17619 2022-11-05 06:29:28.000000 eml_rename-0.2.0/eml_rename/reusing/datetime_functions.py
--rw-r--r--   0 root         (0) root         (0)     2584 2022-11-05 06:29:28.000000 eml_rename-0.2.0/eml_rename/reusing/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-12 19:13:21.080879 eml_rename-0.2.0/eml_rename.egg-info/
--rw-r--r--   0 root         (0) root         (0)      676 2022-11-12 19:13:20.000000 eml_rename-0.2.0/eml_rename.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      615 2022-11-12 19:13:20.000000 eml_rename-0.2.0/eml_rename.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-12 19:13:20.000000 eml_rename-0.2.0/eml_rename.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2022-11-12 19:13:20.000000 eml_rename-0.2.0/eml_rename.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-05 05:38:28.000000 eml_rename-0.2.0/eml_rename.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-12 19:13:20.000000 eml_rename-0.2.0/eml_rename.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-12 19:13:20.000000 eml_rename-0.2.0/eml_rename.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2764 2022-11-06 06:31:10.000000 eml_rename-0.2.0/eml_rename.epj
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-12 19:13:21.085879 eml_rename-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5746 2022-11-06 06:27:16.000000 eml_rename-0.2.0/setup.py
+-rw-r--r--   0        0        0    35149 2023-04-17 06:44:59.591346 eml_rename-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1291 2023-04-17 08:01:55.355302 eml_rename-0.3.0/README.md
+-rw-r--r--   0        0        0      145 2023-04-17 08:00:55.592251 eml_rename-0.3.0/eml_rename/__init__.py
+-rw-r--r--   0        0        0    10278 2023-04-17 07:49:33.411241 eml_rename-0.3.0/eml_rename/core.py
+-rw-r--r--   0        0        0     1684 2023-04-17 06:44:59.591346 eml_rename-0.3.0/eml_rename/locale/eml_rename.pot
+-rw-r--r--   0        0        0      424 2023-04-17 06:44:59.591346 eml_rename-0.3.0/eml_rename/locale/en/LC_MESSAGES/eml_rename.mo
+-rw-r--r--   0        0        0      738 2023-04-17 06:44:59.591346 eml_rename-0.3.0/eml_rename/locale/en.po
+-rw-r--r--   0        0        0     2338 2023-04-17 06:44:59.591346 eml_rename-0.3.0/eml_rename/locale/es/LC_MESSAGES/eml_rename.mo
+-rw-r--r--   0        0        0     2654 2023-04-17 06:44:59.591346 eml_rename-0.3.0/eml_rename/locale/es.po
+-rw-r--r--   0        0        0      756 2023-04-17 08:00:11.899251 eml_rename-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 eml_rename-0.3.0/PKG-INFO
```

### Comparing `eml_rename-0.2.0/LICENSE` & `eml_rename-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eml_rename-0.2.0/README.md` & `eml_rename-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -16,13 +16,17 @@
 - If you use --force parameter the script will overwrite all files even they have the 'YYYYMMDD HHMM [From]' format.
 - Length of the new name will have 140 character as maximum, although you can change it with the --length parameter
 - --save parameter renames files. If you don't use this parameter it will only pretend the result
 - It uses concurrency to make process faster
 
 ## Changelog
 
+### 0.3.0 (2023-04-17)
+- setup.py migrated to poetry
+- Fix bug with CEST time zones
+
 ### 0.2.0 (2022-11-12)
 -  Now mail datetime uses local system time zone
 
 ### 0.1.0 (2022-11-06)
 - First version
 - Added main features
```

### Comparing `eml_rename-0.2.0/eml_rename/core.py` & `eml_rename-0.3.0/eml_rename/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from colorama import init as colorama_init, Fore, Style
 
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from datetime import datetime
 from email.parser import HeaderParser
 from email.utils import parsedate_to_datetime, parseaddr
 from email.header import decode_header
-from eml_rename.reusing.datetime_functions import dtaware2string
 from gettext import translation
 from glob import glob
 from importlib.resources import files
 from os import rename
 
 from multiprocessing import cpu_count
 from signal import signal,  SIGINT
@@ -43,14 +42,57 @@
 def yellow(s):
     return Style.BRIGHT + Fore.YELLOW + str(s) + Style.RESET_ALL
 def blue(s):
     return Style.BRIGHT + Fore.BLUE + str(s) + Style.RESET_ALL
 def white(s):
     return Style.BRIGHT + Fore.WHITE + str(s) + Style.RESET_ALL
 
+
+## Returns if a datetime is aware
+def is_aware(dt):
+    if dt.tzinfo is None or dt.tzinfo.utcoffset(dt) is None:
+        return False
+    return True
+
+## Returns if a datetime is naive
+def is_naive(dt):
+    return not is_aware(dt)
+
+## Returns a formated string of a dtaware string formatting with a zone name
+## @param dt datetime aware object
+## @return String
+def dtaware2string(dt, format):
+    if is_naive(dt)==True:
+        print("A dtaware is needed for {}".format(dt))
+    else:
+        return dtnaive2string(dt, format)
+
+## Returns a formated string of a dtaware string formatting with a zone name
+## @param dt datetime aware object
+## @param format String in ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y%m%d %H%M", "%Y%m%d%H%M"]
+## @return String
+def dtnaive2string(dt, format):
+    allowed=["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y%m%d %H%M", "%Y%m%d%H%M", "JsUtcIso"]
+    if dt==None:
+        return "None"
+    elif format in allowed:
+        if format=="%Y-%m-%d":
+            return dt.strftime("%Y-%m-%d")
+        elif format=="%Y-%m-%d %H:%M:%S": 
+            return dt.strftime("%Y-%m-%d %H:%M:%S")
+        elif format=="%Y%m%d %H%M": 
+            return dt.strftime("%Y%m%d %H%M")
+        elif format=="%Y%m%d%H%M":
+            return dt.strftime("%Y%m%d%H%M")
+        elif format=="JsUtcIso":
+            return dt.strftime("%Y-%m-%dT%H:%M:%SZ")
+    else:
+        print("I can't convert this format '{}'. I only support this {}".format(format, allowed))
+
+
 def get_system_localzone_name():
     return datetime.now().astimezone().tzname()
 
 ## Class to work with eml file
 class EmlFile():
     def __init__(self, path):
         self.path=path
@@ -60,19 +102,20 @@
         #Guessing file chart
         with open(path, "rb") as f:
             self.detected=detect(f.read(10000))
         
         #Parse file and load used metadata            
         with open(path, "r", encoding=self.detected["encoding"]) as f:
             try:
-                system_timezone=get_system_localzone_name()
-
                 metadata=HeaderParser().parse(f)
                 self.from_=parseaddr(metadata["From"])[1]
                 dt_mail=parsedate_to_datetime(metadata["Date"])
+                system_timezone=get_system_localzone_name()
+                if system_timezone in ["CEST", "CET"]: #Cest wasn't recognized by ZoneInfo
+                    system_timezone="Europe/Madrid"
                 self.dt=dt_mail.astimezone(ZoneInfo(system_timezone))
                 self.subject=self.parse_subject(metadata["Subject"])
             except Exception as e:
                 self.error_message=e
```

### Comparing `eml_rename-0.2.0/eml_rename/locale/eml_rename.pot` & `eml_rename-0.3.0/eml_rename/locale/eml_rename.pot`

 * *Files identical despite different names*

### Comparing `eml_rename-0.2.0/eml_rename/locale/en.po` & `eml_rename-0.3.0/eml_rename/locale/en.po`

 * *Files identical despite different names*

### Comparing `eml_rename-0.2.0/eml_rename/locale/es/LC_MESSAGES/eml_rename.mo` & `eml_rename-0.3.0/eml_rename/locale/es/LC_MESSAGES/eml_rename.mo`

 * *Files identical despite different names*

### Comparing `eml_rename-0.2.0/eml_rename/locale/es.po` & `eml_rename-0.3.0/eml_rename/locale/es.po`

 * *Files identical despite different names*

