# Comparing `tmp/cloudnet-submit-0.0.4.tar.gz` & `tmp/cloudnet-submit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudnet-submit-0.0.4.tar", last modified: Thu Apr  6 08:23:43 2023, max compression
+gzip compressed data, was "cloudnet-submit-0.0.5.tar", last modified: Mon Apr 17 11:16:46 2023, max compression
```

## Comparing `cloudnet-submit-0.0.4.tar` & `cloudnet-submit-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:23:43.058066 cloudnet-submit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-06 08:23:43.058066 cloudnet-submit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-06 08:23:43.058066 cloudnet-submit-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:23:43.054066 cloudnet-submit-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:23:43.058066 cloudnet-submit-0.0.4/src/cloudnet_submit/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/Submission.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/cloudnet-config-example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/dateutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/src/cloudnet_submit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:23:43.058066 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-06 08:23:43.000000 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-06 08:23:43.000000 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:23:43.000000 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 08:23:43.000000 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-06 08:23:43.000000 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 08:23:43.000000 cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:23:43.058066 cloudnet-submit-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-06 08:23:28.000000 cloudnet-submit-0.0.4/tests/test_cloudnet_submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:16:46.590494 cloudnet-submit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-17 11:16:46.590494 cloudnet-submit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 11:16:46.590494 cloudnet-submit-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:16:46.586493 cloudnet-submit-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:16:46.590494 cloudnet-submit-0.0.5/src/cloudnet_submit/
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/Submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/cloudnet-config-example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/dateutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/src/cloudnet_submit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:16:46.590494 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-17 11:16:46.000000 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-17 11:16:46.000000 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:16:46.000000 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 11:16:46.000000 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-17 11:16:46.000000 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 11:16:46.000000 cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:16:46.590494 cloudnet-submit-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-17 11:16:28.000000 cloudnet-submit-0.0.5/tests/test_cloudnet_submit.py
```

### Comparing `cloudnet-submit-0.0.4/LICENSE` & `cloudnet-submit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/PKG-INFO` & `cloudnet-submit-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnet-submit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cloudnet data submission tool
 Home-page: https://github.com/actris-cloudnet/cloudnet-submit
 Author: Niko Leskinen
 Author-email: niko.leskinen@fmi.fi
 Project-URL: Bug Tracker, https://github.com/actris-cloudnet/cloudnet-submit/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloudnet-submit-0.0.4/README.md` & `cloudnet-submit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/setup.cfg` & `cloudnet-submit-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit/Submission.py` & `cloudnet-submit-0.0.5/src/cloudnet_submit/Submission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import datetime
 import hashlib
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
 from sys import stdout
 from typing import Union
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
@@ -40,15 +40,15 @@
 class Status:
     metadata_ok: bool = False
     data_ok: bool = False
     metadata: Union[int, None] = None
     data: Union[int, None] = None
     metadata_msg: Union[str, None] = None
     data_msg: Union[str, None] = None
-    proxies: ProxyConfig = ProxyConfig()
+    proxies: ProxyConfig = field(default_factory=lambda: ProxyConfig())
 
 
 class Submission:
     def __init__(
         self,
         path: Path,
         metadata: Union[InstrumentMetadata, ModelMetadata],
```

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit/cfg.py` & `cloudnet-submit-0.0.5/src/cloudnet_submit/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,14 @@
         )
         exit(1)
     config = toml.load(path)
     user_conf = get_user_account_config(config)
     instrument_conf = get_instrument_config(config)
     model_conf = get_model_config(config)
     proxy_conf = get_proxy_config(config)
-    print(proxy_conf)
     return Config(
         user_account=user_conf,
         proxies=proxy_conf,
         instrument=instrument_conf,
         model=model_conf,
         dry_run=args.dry_run,
         dates=get_dates(args),
@@ -196,20 +195,21 @@
         last_three_days = [today - i * one_day for i in range(3)]
         return last_three_days
     dates = set()
     # Dates from --date argument
     for date in args.date if args.date else []:
         dates.add(date)
     # Date range from --from-date --to-date arguments
-    to_date = args.to_date if args.to_date else today
-    from_date = args.from_date if args.from_date else min(to_date, today)
-    idate = from_date
-    while idate <= to_date:
-        dates.add(idate)
-        idate += one_day
+    if not (args.from_date is None and args.to_date is None):
+        to_date = args.to_date if args.to_date else today
+        from_date = args.from_date if args.from_date else min(to_date, today)
+        idate = from_date
+        while idate <= to_date:
+            dates.add(idate)
+            idate += one_day
     # Dates from --last-ndays argument
     if args.last_ndays:
         idate = today - datetime.timedelta(days=args.last_ndays - 1)
         while idate <= today:
             dates.add(idate)
             idate += one_day
     non_future_dates = [date for date in dates if date <= today]
```

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit/cloudnet-config-example.toml` & `cloudnet-submit-0.0.5/src/cloudnet_submit/cloudnet-config-example.toml`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit/generate_config.py` & `cloudnet-submit-0.0.5/src/cloudnet_submit/generate_config.py`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit/utils.py` & `cloudnet-submit-0.0.5/src/cloudnet_submit/utils.py`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/PKG-INFO` & `cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnet-submit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cloudnet data submission tool
 Home-page: https://github.com/actris-cloudnet/cloudnet-submit
 Author: Niko Leskinen
 Author-email: niko.leskinen@fmi.fi
 Project-URL: Bug Tracker, https://github.com/actris-cloudnet/cloudnet-submit/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloudnet-submit-0.0.4/src/cloudnet_submit.egg-info/SOURCES.txt` & `cloudnet-submit-0.0.5/src/cloudnet_submit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudnet-submit-0.0.4/tests/test_cloudnet_submit.py` & `cloudnet-submit-0.0.5/tests/test_cloudnet_submit.py`

 * *Files identical despite different names*

