# Comparing `tmp/tsd_api_client-3.5.7.tar.gz` & `tmp/tsd_api_client-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsd_api_client-3.5.7.tar", max compression
+gzip compressed data, was "tsd_api_client-3.5.8.tar", max compression
```

## Comparing `tsd_api_client-3.5.7.tar` & `tsd_api_client-3.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1454 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/LICENSE
--rw-r--r--   0        0        0      704 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/README.md
--rw-r--r--   0        0        0      865 2023-03-14 11:35:11.052536 tsd_api_client-3.5.7/pyproject.toml
--rw-r--r--   0        0        0       33 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/__init__.py
--rw-r--r--   0        0        0       61 2023-03-14 11:35:11.052536 tsd_api_client-3.5.7/tsdapiclient/_version.py
--rw-r--r--   0        0        0      679 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/administrator.py
--rw-r--r--   0        0        0     5273 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/authapi.py
--rw-r--r--   0        0        0      590 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/client_config.py
--rw-r--r--   0        0        0     4819 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/configurer.py
--rw-r--r--   0        0        0     1430 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/crypto.py
--rw-r--r--   0        0        0      127 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/exc.py
--rw-r--r--   0        0        0    36522 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/fileapi.py
--rw-r--r--   0        0        0     6070 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/guide.py
--rw-r--r--   0        0        0     3091 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/session.py
--rw-r--r--   0        0        0    26350 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/sync.py
--rw-r--r--   0        0        0    25614 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/tacl.py
--rw-r--r--   0        0        0     9546 2023-03-14 11:34:53.035262 tsd_api_client-3.5.7/tsdapiclient/tools.py
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 tsd_api_client-3.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1454 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/LICENSE
+-rw-r--r--   0        0        0      704 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/README.md
+-rw-r--r--   0        0        0      853 2023-04-17 07:13:54.457957 tsd_api_client-3.5.8/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-17 07:13:54.457957 tsd_api_client-3.5.8/tsdapiclient/_version.py
+-rw-r--r--   0        0        0      679 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/administrator.py
+-rw-r--r--   0        0        0     5273 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/authapi.py
+-rw-r--r--   0        0        0      590 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/client_config.py
+-rw-r--r--   0        0        0     4182 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/configurer.py
+-rw-r--r--   0        0        0     1430 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/crypto.py
+-rw-r--r--   0        0        0      127 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/exc.py
+-rw-r--r--   0        0        0    36522 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/fileapi.py
+-rw-r--r--   0        0        0     6070 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/guide.py
+-rw-r--r--   0        0        0     4642 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/session.py
+-rw-r--r--   0        0        0    26350 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/sync.py
+-rw-r--r--   0        0        0    25828 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/tacl.py
+-rw-r--r--   0        0        0     9546 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/tools.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 tsd_api_client-3.5.8/PKG-INFO
```

### Comparing `tsd_api_client-3.5.7/LICENSE` & `tsd_api_client-3.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/README.md` & `tsd_api_client-3.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/pyproject.toml` & `tsd_api_client-3.5.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsd-api-client"
-version = "3.5.7" # managed by poetry-dynamic-versioning
+version = "3.5.8" # managed by poetry-dynamic-versioning
 description = "A client for the TSD REST API"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
 ]
 maintainers = [
     "Eirik Haatveit <haatveit@uio.no>",
     "Milen Kouylekov <milen@uio.no>",
@@ -20,15 +20,14 @@
 [tool.poetry.dependencies]
 python = "^3.6"
 requests = "*"
 click = ">=8"
 PyYAML = "*"
 humanfriendly = "*"
 libnacl = "*"
-PyJWT = "*"
 rich = "*"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 bump = true
```

### Comparing `tsd_api_client-3.5.7/tsdapiclient/administrator.py` & `tsd_api_client-3.5.8/tsdapiclient/administrator.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/authapi.py` & `tsd_api_client-3.5.8/tsdapiclient/authapi.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/client_config.py` & `tsd_api_client-3.5.8/tsdapiclient/client_config.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/configurer.py` & `tsd_api_client-3.5.8/tsdapiclient/configurer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 
 """Module for managing tacl config."""
 
 import datetime
 import os
 
-import jwt
 import yaml
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.text import Text
 
-from tsdapiclient.tools import get_config_path
+from tsdapiclient.tools import get_config_path, get_claims, check_if_key_has_expired
 
 TACL_CONFIG = get_config_path() + '/config'
 
 
 def read_config(filename: str = TACL_CONFIG) -> dict:
     try:
         with open(filename, 'r') as f:
@@ -71,36 +70,35 @@
 
 def print_config(filename: str = TACL_CONFIG) -> None:
     """Print configuration overview and config file path/contents."""
     console = Console()
     config = read_config(filename=filename)
     if not os.path.exists(filename):
         print("No config found")
+        exit(1)
     else:
-        grid = Table.grid(expand=True)
-        grid.add_column()
-        grid.add_column(justify="right")
-
         table = Table(title=f"{__package__} configuration details")
         table.add_column("Environment")
         table.add_column("Project")
         table.add_column("User")
         table.add_column("Expiry")
 
         config = read_config(filename=filename)
         for env in config:
             for project in config[env].keys():
-                decoded_api_key = decode_api_key(api_key=config[env][project])
+                api_key = config[env][project]
+                decoded_api_key = get_claims(api_key)
                 exp = decoded_api_key['exp']
                 expiry = Text(datetime.datetime.fromtimestamp(exp).strftime('%Y-%m-%d %H:%M:%S'))
-                if api_key_is_expired(api_key=config[env][project]):
+                if check_if_key_has_expired(api_key):
                     expiry.stylize('bold red')
                 user = decoded_api_key.get('user')
                 table.add_row(env, project, user, expiry)
-        console.print(table)
+        if table.rows:
+            console.print(table)
     
         with open(filename, 'r') as f:
             syntax = Syntax(f.read(), 'yaml', line_numbers=True, word_wrap=True)
         console.print(f"Configuration file '[underline]{filename}[/underline]':")
         console.print(syntax)
 
 
@@ -114,29 +112,7 @@
 def print_config_tsd_2fa_key(env: str, pnum: str) -> None:
     try:
         with open(TACL_CONFIG, 'r') as f:
             cf = yaml.load(f, Loader=yaml.Loader)
             print(cf[env][pnum])
     except FileNotFoundError:
         print("No config found")
-
-def decode_api_key(api_key: str) -> dict:
-    """Decode a TSD API key.
-
-    Args:
-        api_key (str): The JWT format TSD API key.
-
-    Returns:
-        dict: The decoded TSD API key.
-    """
-    return jwt.decode(api_key, algorithms=['HS256'], options={'verify_signature': False})
-
-def api_key_is_expired(api_key: str) -> bool:
-    """Check if the API key is expired.
-
-    Args:
-        api_key (str): The JWT format TSD API key.
-
-    Returns:
-        bool: True if the API key is expired, False otherwise.
-    """
-    return decode_api_key(api_key=api_key)['exp'] < datetime.datetime.now().timestamp()
```

### Comparing `tsd_api_client-3.5.7/tsdapiclient/crypto.py` & `tsd_api_client-3.5.8/tsdapiclient/crypto.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/fileapi.py` & `tsd_api_client-3.5.8/tsdapiclient/fileapi.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/guide.py` & `tsd_api_client-3.5.8/tsdapiclient/guide.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/sync.py` & `tsd_api_client-3.5.8/tsdapiclient/sync.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/tsdapiclient/tacl.py` & `tsd_api_client-3.5.8/tsdapiclient/tacl.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from tsdapiclient.session import (
     session_is_expired,
     session_expires_soon,
     session_update,
     session_clear,
     session_token,
     session_refresh_token,
+    session_print,
 )
 from tsdapiclient.sync import (
     SerialDirectoryUploader,
     SerialDirectoryDownloader,
     SerialDirectoryUploadSynchroniser,
     SerialDirectoryDownloadSynchroniser,
     UploadCache,
@@ -69,15 +70,15 @@
 requests.utils.default_user_agent = user_agent
 
 API_ENVS = {
     'prod': 'api.tsd.usit.no',
     'alt': 'alt.api.tsd.usit.no',
     'test': 'test.api.tsd.usit.no',
     'ec-prod': 'api.fp.educloud.no',
-    'ec-test': 'test-api-educloud.uio.no',
+    'ec-test': 'test.api.fp.educloud.no',
     'dev': 'localhost',
 }
 
 TOKENS = {
     'prod': {
         'upload': 'import',
         'download': 'export'
@@ -328,14 +329,20 @@
 @click.option(
     '--config-delete',
     is_flag=True,
     required=False,
     help='Delete tacl config'
 )
 @click.option(
+    '--session-show',
+    is_flag=True,
+    required=False,
+    help='Show tacl login session data'
+)
+@click.option(
     '--session-delete',
     is_flag=True,
     required=False,
     help='Delete current tacl login session'
 )
 @click.option(
     '--register',
@@ -471,14 +478,15 @@
     download: str,
     download_id: str,
     download_list: bool,
     version: bool,
     verbose: bool,
     config_show: bool,
     config_delete: bool,
+    session_show: bool,
     session_delete: bool,
     register: bool,
     ignore_prefixes: str,
     ignore_suffixes: str,
     upload_cache_show: bool,
     upload_cache_delete: str,
     upload_cache_delete_all: bool,
@@ -750,14 +758,16 @@
         ) and not pnum:
             sys.exit('cache operations are project specific - missing pnum argument')
         # 4.1 Interact with config, sessions, and caches
         if config_show:
             print_config()
         elif config_delete:
             delete_config()
+        elif session_show:
+            session_print()
         elif session_delete:
             session_clear()
         elif upload_cache_show:
             cache = UploadCache(env, pnum)
             cache.print()
         elif upload_cache_delete:
             cache = UploadCache(env, pnum)
```

### Comparing `tsd_api_client-3.5.7/tsdapiclient/tools.py` & `tsd_api_client-3.5.8/tsdapiclient/tools.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.7/PKG-INFO` & `tsd_api_client-3.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsd-api-client
-Version: 3.5.7
+Version: 3.5.8
 Summary: A client for the TSD REST API
 Home-page: https://github.com/unioslo/tsd-api-client
 License: BSD-3-Clause
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Maintainer: Eirik Haatveit
 Maintainer-email: haatveit@uio.no
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyJWT
 Requires-Dist: PyYAML
 Requires-Dist: click (>=8)
 Requires-Dist: humanfriendly
 Requires-Dist: libnacl
 Requires-Dist: requests
 Requires-Dist: rich
 Project-URL: Repository, https://github.com/unioslo/tsd-api-client
```

