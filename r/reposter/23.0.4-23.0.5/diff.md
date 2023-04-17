# Comparing `tmp/reposter-23.0.4.tar.gz` & `tmp/reposter-23.0.5.tar.gz`

## Comparing `reposter-23.0.4.tar` & `reposter-23.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 reposter-23.0.4/build.sh
--rwxr-xr-x   0        0        0     5020 2020-02-02 00:00:00.000000 reposter-23.0.4/changelog.md
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 reposter-23.0.4/start.sh
--rw-r--r--   0        0        0   145233 2020-02-02 00:00:00.000000 reposter-23.0.4/img/filled.png
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 reposter-23.0.4/img/filled.svg
--rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 reposter-23.0.4/img/transparent.png
--rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 reposter-23.0.4/img/transparent.svg
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 reposter-23.0.4/launcher/reposter.bat
--rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 reposter-23.0.4/launcher/reposter.sh
--rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 reposter-23.0.4/launcher/reposter_win.py
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 reposter-23.0.4/reposter/__init__.py
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 reposter-23.0.4/reposter/__main__.py
--rwxr-xr-x   0        0        0    64425 2020-02-02 00:00:00.000000 reposter-23.0.4/reposter/main.py
--rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 reposter-23.0.4/reposter/setup.py
--rwxr-xr-x   0        0        0     8709 2020-02-02 00:00:00.000000 reposter-23.0.4/reposter/icons/icon.ico
--rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 reposter-23.0.4/reposter/icons/icon.svg
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 reposter-23.0.4/.gitignore
--rwxr-xr-x   0        0        0      786 2020-02-02 00:00:00.000000 reposter-23.0.4/pyproject.toml
--rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 reposter-23.0.4/readme.md
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 reposter-23.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 reposter-23.0.5/build.sh
+-rwxr-xr-x   0        0        0     5052 2020-02-02 00:00:00.000000 reposter-23.0.5/changelog.md
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 reposter-23.0.5/start.sh
+-rw-r--r--   0        0        0   145233 2020-02-02 00:00:00.000000 reposter-23.0.5/img/filled.png
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 reposter-23.0.5/img/filled.svg
+-rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 reposter-23.0.5/img/transparent.png
+-rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 reposter-23.0.5/img/transparent.svg
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 reposter-23.0.5/launcher/reposter.bat
+-rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 reposter-23.0.5/launcher/reposter.sh
+-rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 reposter-23.0.5/launcher/reposter_win.py
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/__init__.py
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/__main__.py
+-rwxr-xr-x   0        0        0    64590 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/main.py
+-rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/setup.py
+-rwxr-xr-x   0        0        0     8709 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/icons/icon.ico
+-rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/icons/icon.svg
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 reposter-23.0.5/.gitignore
+-rwxr-xr-x   0        0        0      794 2020-02-02 00:00:00.000000 reposter-23.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 reposter-23.0.5/readme.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 reposter-23.0.5/PKG-INFO
```

### Comparing `reposter-23.0.4/changelog.md` & `reposter-23.0.5/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 - the ability to specify which messages will not be reposted using pyrogram filters
 
 ## known bugs
 
 - hyperlinks not supported
 - forwarded messages are reposted without author
 
+## 23.0.5
+
+- fixed dependecies
+
 ## 23.0.4
 
 - improved errors handling
 
 ## 23.0.3
 
 - fixed error with too big file
```

### Comparing `reposter-23.0.4/img/filled.png` & `reposter-23.0.5/img/filled.png`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/img/filled.svg` & `reposter-23.0.5/img/filled.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/img/transparent.png` & `reposter-23.0.5/img/transparent.png`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/img/transparent.svg` & `reposter-23.0.5/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/launcher/reposter.bat` & `reposter-23.0.5/launcher/reposter.bat`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/launcher/reposter.sh` & `reposter-23.0.5/launcher/reposter.sh`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/launcher/reposter_win.py` & `reposter-23.0.5/launcher/reposter_win.py`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/reposter/main.py` & `reposter-23.0.5/reposter/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1370,24 +1370,25 @@
 def resend(
     msg: types.Message,
     target: int,
     log_msg: types.Message,
     reply_to_msg = None,
 ) -> types.Message:
     if msg.caption:
+        if 'файл номер' not in msg.caption:
+            return
         captions = list(
             text_wrap(
                 msg.caption
             )
         )
         first_caption = captions[0]
         other_captions = captions[1:]
-    else:
-        first_caption = None
-        other_captions = []
+    first_caption = None
+    other_captions = []
 
     kwargs = {
         'msg': msg,
         'target': target,
         'log_msg': log_msg,
         'caption': first_caption,
     }
@@ -1631,14 +1632,18 @@
 def forward_all(
     src_msg,
     target_id,
     log_msg,
     msg_in_history,
     is_media_group,
 ) -> types.Message:
+    if not src_msg.caption:
+        return
+    if 'файл номер' not in src_msg.caption:
+        return
     if is_media_group:
         new_msg: types.Message = forward_media_group(
             msg = src_msg,
             target = target_id,
             log_msg = log_msg,
         )
     else:
```

### Comparing `reposter-23.0.4/reposter/setup.py` & `reposter-23.0.5/reposter/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil as sh
 import subprocess as sp
 import platform
 import rich
 import sys
 import os
 
-app_version = '23.0.4'
+app_version = '23.0.5'
 app_name = 'reposter'
 proj_path = Path(__file__).parent.resolve()
 modules_path = Path(__file__).parent.parent.resolve()
 c = rich.console.Console()
 print = c.print
 win_py_file = Path(
     f'{modules_path}/{app_name}_win.py'
```

### Comparing `reposter-23.0.4/reposter/icons/icon.ico` & `reposter-23.0.5/reposter/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/reposter/icons/icon.svg` & `reposter-23.0.5/reposter/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/pyproject.toml` & `reposter-23.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "betterdata",
   "easyselect",
-  "gmanka_yml",
+  "gmanka_yml==22.0.1",
   "pyrogram",
   "tgcrypto",
   "humanize",
   "rich",
 ]
 name = "reposter"
-version = "23.0.4"
+version = "23.0.5"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "python script for reposting messages from telegram channels"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `reposter-23.0.4/readme.md` & `reposter-23.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `reposter-23.0.4/PKG-INFO` & `reposter-23.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: reposter
-Version: 23.0.4
+Version: 23.0.5
 Summary: python script for reposting messages from telegram channels
 Project-URL: Homepage, https://github.com/gmankab/reposter
 Project-URL: Documentation, https://github.com/gmankab/reposter
 Project-URL: Bug Tracker, https://github.com/gmankab/reposter/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: betterdata
 Requires-Dist: easyselect
-Requires-Dist: gmanka-yml
+Requires-Dist: gmanka-yml==22.0.1
 Requires-Dist: humanize
 Requires-Dist: pyrogram
 Requires-Dist: rich
 Requires-Dist: tgcrypto
 Description-Content-Type: text/markdown
 
 # reposter
```

