# Comparing `tmp/dataplaybook-1.0.8.tar.gz` & `tmp/dataplaybook-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataplaybook-1.0.8.tar", last modified: Thu Sep 30 19:30:54 2021, max compression
+gzip compressed data, was "dataplaybook-1.0.9.tar", last modified: Fri Mar  4 04:46:33 2022, max compression
```

## Comparing `dataplaybook-1.0.8.tar` & `dataplaybook-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.208011 dataplaybook-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7681 2021-09-30 19:30:54.208011 dataplaybook-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7337 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.200012 dataplaybook-1.0.8/dataplaybook/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/config_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/const.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.200012 dataplaybook-1.0.8/dataplaybook/everything/
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/everything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7114 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5973 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.204012 dataplaybook-1.0.8/dataplaybook/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     7030 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.204012 dataplaybook-1.0.8/dataplaybook/tasks/aio_oauth/
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/aio_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/aio_oauth/oauth_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     7867 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/fnb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/fuzzy.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/gis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5590 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/ietf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/io_mail.py
--rw-r--r--   0 runner    (1001) docker     (121)     5339 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/io_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6336 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/io_mongo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/io_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7533 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/io_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/tasks/io_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     9045 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/dataplaybook/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.208011 dataplaybook-1.0.8/dataplaybook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      996 2021-09-30 19:30:54.000000 dataplaybook-1.0.8/dataplaybook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-09-30 19:30:54.208011 dataplaybook-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.200012 dataplaybook-1.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.204012 dataplaybook-1.0.8/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:54.204012 dataplaybook-1.0.8/tests/tasks/aio_oauth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/aio_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/aio_oauth/test_oauth_server.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_all.py
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_ietf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_init.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_io_mail.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_io_mongo.py
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_io_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (121)     6418 2021-09-30 19:30:42.000000 dataplaybook-1.0.8/tests/tasks/test_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8166 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7337 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/dataplaybook/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/config_validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/const.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/dataplaybook/everything/
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/everything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7114 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5973 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/dataplaybook/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/dataplaybook/tasks/aio_oauth/
+-rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/aio_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/aio_oauth/oauth_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7867 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/fnb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/fuzzy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/gis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5590 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/ietf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/io_mail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5339 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/io_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6625 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/io_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/io_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7533 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/io_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/tasks/io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9281 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/dataplaybook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/dataplaybook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-03-04 04:46:33.000000 dataplaybook-1.0.9/dataplaybook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-03-04 04:46:33.377305 dataplaybook-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.369305 dataplaybook-1.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/tests/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:33.373305 dataplaybook-1.0.9/tests/tasks/aio_oauth/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/aio_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/aio_oauth/test_oauth_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_ietf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_io_mail.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_io_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_io_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6418 2022-03-04 04:46:24.000000 dataplaybook-1.0.9/tests/tasks/test_templates.py
```

### Comparing `dataplaybook-1.0.8/LICENSE` & `dataplaybook-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/PKG-INFO` & `dataplaybook-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: dataplaybook
-Version: 1.0.8
-Summary: Playbooks for data. Open, process and save table based data.
-Home-page: https://github.com/kellerza/data-playbook
-Author: Johann Kellerman
-Author-email: kellerza@gmail.com
-License: Apache License 2.0
-Platform: any
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Data Playbook
 
 :book: Playbooks for data. Open, process and save table based data.
 [![Workflow Status](https://github.com/kellerza/data-playbook/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/kellerza/data-playbook/actions)
 [![codecov](https://codecov.io/gh/kellerza/data-playbook/branch/master/graph/badge.svg)](https://codecov.io/gh/kellerza/data-playbook)
 
 Automate repetitive tasks on table based data. Include various input and output tasks.
@@ -135,9 +123,7 @@
 
 - They are mostly not idempotent, since the intention is to modify tables as we go along,
 - they can return lists containing rows or be Python iterators (that `yield` rows of a table)
 - if they dont return any tabular data (a list), the return value will be added to the `var` table in the environment
 - Each have a strict voluptuous schema, evaluated when loading and during runtime (e.g. to expand templates) to allow quick troubleshooting
 
 You could argue I can do this with Ansible, but it won't be as elegant with single item hosts files, `gather_facts: no` and `delegate_to: localhost` throughout the playbooks. It will likely only be half as much fun trying to force it into my way of thinking.
-
-
```

### Comparing `dataplaybook-1.0.8/README.md` & `dataplaybook-1.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: dataplaybook
+Version: 1.0.9
+Summary: Playbooks for data. Open, process and save table based data.
+Home-page: https://github.com/kellerza/data-playbook
+Author: Johann Kellerman
+Author-email: kellerza@gmail.com
+License: Apache License 2.0
+Keywords: data,tables,excel,mongodb,generators
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: mongodb
+License-File: LICENSE
+
 # Data Playbook
 
 :book: Playbooks for data. Open, process and save table based data.
 [![Workflow Status](https://github.com/kellerza/data-playbook/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/kellerza/data-playbook/actions)
 [![codecov](https://codecov.io/gh/kellerza/data-playbook/branch/master/graph/badge.svg)](https://codecov.io/gh/kellerza/data-playbook)
 
 Automate repetitive tasks on table based data. Include various input and output tasks.
@@ -123,7 +146,9 @@
 
 - They are mostly not idempotent, since the intention is to modify tables as we go along,
 - they can return lists containing rows or be Python iterators (that `yield` rows of a table)
 - if they dont return any tabular data (a list), the return value will be added to the `var` table in the environment
 - Each have a strict voluptuous schema, evaluated when loading and during runtime (e.g. to expand templates) to allow quick troubleshooting
 
 You could argue I can do this with Ansible, but it won't be as elegant with single item hosts files, `gather_facts: no` and `delegate_to: localhost` throughout the playbooks. It will likely only be half as much fun trying to force it into my way of thinking.
+
+
```

### Comparing `dataplaybook-1.0.8/dataplaybook/config_validation.py` & `dataplaybook-1.0.9/dataplaybook/config_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Data validation helpers for voluptuous."""
 import logging
 import os
-import re
 from typing import Any, Callable, Sequence, TypeVar, Union
 
 import voluptuous as vol
 
+from dataplaybook.utils import slugify as util_slugify
+
 # typing typevar
 T = TypeVar("T")  # pylint: disable=invalid-name
-RE_SLUGIFY = re.compile(r"[^a-z0-9_]+")
 _LOGGER = logging.getLogger(__name__)
 _LOGGER.setLevel(logging.INFO)
 
 
 class AttrKeyError(KeyError):
     """Key not found in dict."""
 
@@ -77,25 +77,14 @@
 def ensure_list(value: Union[T, Sequence[T], None]) -> Sequence[T]:
     """Wrap value in list if it is not one."""
     if value is None:
         return []
     return value if isinstance(value, list) else [value]  # typing: ignore
 
 
-def util_slugify(text: str) -> str:
-    """Slugify a given text."""
-    # text = normalize('NFKD', text)
-    text = text.lower()
-    text = text.replace(" ", "_")
-    # text = text.translate(TBL_SLUGIFY)
-    text = RE_SLUGIFY.sub("", text)
-
-    return text
-
-
 def endswith(parts: str) -> Callable[[Any], Any]:
     """Ensure a string ends with specified part."""
 
     def _check(_str: str) -> str:
         """Return the validator."""
         if _str.endswith(parts):
             return _str
```

### Comparing `dataplaybook-1.0.8/dataplaybook/everything/__init__.py` & `dataplaybook-1.0.9/dataplaybook/everything/__init__.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/helper.py` & `dataplaybook-1.0.9/dataplaybook/helper.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/main.py` & `dataplaybook-1.0.9/dataplaybook/main.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Dataplaybook tasks."""
 import argparse
 import atexit
-from functools import wraps
-from inspect import isgeneratorfunction, signature
 import logging
 import os
-from pathlib import Path
 import sys
+from functools import wraps
+from inspect import isgeneratorfunction, signature
+from pathlib import Path
 from typing import Callable, Dict, Optional, Sequence, get_type_hints
 
 from icecream import colorizedStderrPrint, ic  # noqa pylint: disable=unused-import
 from typeguard import _CallMemo, check_argument_types, check_return_type
 
 from dataplaybook.const import VERSION, ATable, Table, Tables
 from dataplaybook.utils import (
```

### Comparing `dataplaybook-1.0.8/dataplaybook/task.py` & `dataplaybook-1.0.9/dataplaybook/task.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/__init__.py` & `dataplaybook-1.0.9/dataplaybook/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/aio_oauth/__init__.py` & `dataplaybook-1.0.9/dataplaybook/tasks/aio_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/aio_oauth/oauth_server.py` & `dataplaybook-1.0.9/dataplaybook/tasks/aio_oauth/oauth_server.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/fnb.py` & `dataplaybook-1.0.9/dataplaybook/tasks/fnb.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Merge FNB statement."""
 # pylint: disable=consider-using-f-string
-from calendar import monthrange
 import csv
-from datetime import datetime
 import logging
 import os
-from pathlib import Path
 import re
 import traceback
+from calendar import monthrange
+from datetime import datetime
+from pathlib import Path
 from typing import Dict, Optional
 
 from dataplaybook import Table, task
 
 _LOGGER = logging.getLogger(__name__)
 
 RE_CARD = re.compile(r"\d{6}\*\d{4}")
```

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/fuzzy.py` & `dataplaybook-1.0.9/dataplaybook/tasks/fuzzy.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/gis.py` & `dataplaybook-1.0.9/dataplaybook/tasks/gis.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/ietf.py` & `dataplaybook-1.0.9/dataplaybook/tasks/ietf.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/io_mail.py` & `dataplaybook-1.0.9/dataplaybook/tasks/io_mail.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Sending files."""
+import smtplib
 from email import encoders
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from pathlib import Path
-import smtplib
 from socket import gaierror
 from typing import List, Optional, Union
 
 from dataplaybook import task
 
 
 @task
```

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/io_misc.py` & `dataplaybook-1.0.9/dataplaybook/tasks/io_misc.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Misc IO tasks."""
+import time
+import urllib.request
 from csv import DictReader, DictWriter
 from json import dump, load, loads
 from json.decoder import JSONDecodeError
 from os import getenv
 from pathlib import Path
-import time
 from typing import List, Optional, Pattern, Sequence
 from urllib.parse import urlparse
-import urllib.request
 
 from icecream import ic
 
 from dataplaybook import Columns, Table, task
 
 
 @task
```

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/io_mongo.py` & `dataplaybook-1.0.9/dataplaybook/tasks/io_mongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """MongoDB IO tasks."""
 import logging
 from typing import List, Optional, Sequence
 from urllib.parse import urlparse
 
 import attr
+import voluptuous as vol
 from icecream import ic  # noqa pylint: disable=unused-import
 from pymongo import MongoClient
 from pymongo.errors import ServerSelectionTimeoutError
-import voluptuous as vol
 
 from dataplaybook import Columns, Table, task
 from dataplaybook.utils import PlaybookError
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -33,15 +33,15 @@
     netloc = attr.ib(converter=_clean_netloc)
     database = attr.ib()
     collection = attr.ib()
     set_id = attr.ib(default="")
 
     @staticmethod
     def new_from_string(db_uri: str, set_id=None):
-        """new mongodb uri."""
+        """Mongodb URI from a string."""
         try:
             res = urlparse(db_uri)
         except AttributeError as err:
             _LOGGER.error("could not parse URL: %s: %s", db_uri, err)
             raise err
         if res.scheme not in ["mdb", "mongodb", "db"]:
             raise vol.Invalid("mdb://host:port/database/collection/[set_id]")
@@ -63,14 +63,15 @@
     # def validate(opt):
     #     """Validate MongoDB URI."""
     #     if not isinstance(opt.get("mdb"), MongoURI):
     #         opt["mdb"] = MongoURI.new_from_string(opt["mdb"], opt.pop("set_id", None))
     #     return opt
 
     def __str__(self) -> str:
+        """As string."""
         return f"{self.netloc}/{self.database}/{self.collection}/{self.set_id}"
 
     def get_client(self, connect=True) -> MongoClient:
         """Return a MongoClient."""
         return MongoClient(self.netloc, connect=connect)
 
 
@@ -108,15 +109,15 @@
         col = client[mdb.database][mdb.collection]
         if not set_id:
             _LOGGER.info("Writing %s documents", len(table))
             client[mdb.database][mdb.collection].insert_many(table)
             return
 
         filtr = {"_sid": set_id}
-        existing_count = col.count(filtr)
+        existing_count = col.count_documents(filtr)
         if not force and existing_count > 0 and not table:
             _LOGGER.error(
                 "Trying to replace %s documents with an empty set", existing_count
             )
             return
         _LOGGER.info(
             "Replacing %s documents matching %s, %s new",
@@ -150,15 +151,15 @@
             if col in row[list_column]:
                 row[col] = True
         del row[list_column]
 
 
 @task
 def mongo_list_sids(mdb: MongoURI) -> List[str]:
-    """Return a list of _sid's"""
+    """Return a list of _sids."""
     client = MongoClient(mdb.netloc, connect=True)
     cursor = client[mdb.database][mdb.collection]
     # non = cursor.find_one({"_sid": {"$exists": False}})
     # print(non)
     other = cursor.distinct("_sid")
     # print(other)
     return other
@@ -174,32 +175,44 @@
             cursor.delete_many({"_sid": {"$exists": False}})
         else:
             cursor.delete_many({"_sid": sid})
 
 
 @task
 def mongo_sync_sids(
-    *, mdb_local: MongoURI, mdb_remote: MongoURI, ignore_remote: Sequence[str] = None
+    *,
+    mdb_local: MongoURI,
+    mdb_remote: MongoURI,
+    ignore_remote: Sequence[str] = None,
+    only_sync_sids: Sequence[str] = None,
 ):
-    """Sync two MongoDB collections. Only sync _sid's where the count is different.
+    """Sync two MongoDB collections.
+
+    Only sync _sid's where the count is different.
     Dont delete additional SIDs from th remote if in ignore_remote
     """
     agg = [{"$group": {"_id": "$_sid", "count": {"$sum": 1}}}]
     # get local
     l_db = mdb_local.get_client()[mdb_local.database][mdb_local.collection]
     lsc = {i["_id"]: i["count"] for i in l_db.aggregate(agg)}
     # get remote
     r_db = mdb_remote.get_client()[mdb_remote.database][mdb_remote.collection]
     rsc = {i["_id"]: i["count"] for i in r_db.aggregate(agg)}
 
     for sid, lval in lsc.items():
         rval = rsc.pop(sid, None)
         if rval != lval:
+            if only_sync_sids and sid not in only_sync_sids:
+                continue
             # counts are different!
             mdb_local.set_id = sid
             lcl = read_mongo(mdb=mdb_local)
             write_mongo(mdb=mdb_remote, table=lcl, set_id=sid)
 
+    if only_sync_sids:
+        _LOGGER.info("Will not remove extra remote _sids")
+        return
+
     extra = list(set(rsc.keys()) - set(ignore_remote or []))
     ic(extra)
     if extra:
         mongo_delete_sids(mdb=mdb_remote, sids=extra)
```

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/io_pdf.py` & `dataplaybook-1.0.9/dataplaybook/tasks/io_pdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """PDF IO Tasks."""
 import functools
 import logging
 import os
+import tempfile
 from pathlib import Path
 from subprocess import call
-import tempfile
 
 from dataplaybook import Table, task
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def _myreadlines(fobj, newline):
@@ -34,17 +34,22 @@
         return
     try:
         _fd, to_name = tempfile.mkstemp()
         params = ["pdftotext", "-layout", filename, to_name]
         _LOGGER.info("Converting %s", filename)
         _LOGGER.debug("Calling with %s", params)
         call(params, shell=False)
-        with open(to_name, "r", encoding="utf8") as __f:
+        with open(to_name, "r", encoding="utf-8", errors="replace") as __f:
             for _no, text in enumerate(_myreadlines(__f, chr(12)), 1):
                 yield {"page": _no, "text": text}
+    except FileNotFoundError:
+        _LOGGER.error(
+            "Could not find pdftotext executable. "
+            "Download from https://www.xpdfreader.com/download.html"
+        )
     finally:
         os.close(_fd)
         os.remove(to_name)
 
 
 @task
 def read_pdf_files(folder: str, pattern: str = "*.pdf") -> Table:
```

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/io_xlsx.py` & `dataplaybook-1.0.9/dataplaybook/tasks/io_xlsx.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Read helpers."""
-from collections import OrderedDict
-from json import dumps
 import logging
 import os
+from collections import OrderedDict
+from json import dumps
 from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 import openpyxl
+import voluptuous as vol
 from openpyxl.utils import get_column_letter
 from openpyxl.worksheet.worksheet import Worksheet
-import voluptuous as vol
 
-from dataplaybook import Tables, task
 import dataplaybook.config_validation as cv
+from dataplaybook import Tables, task
 from dataplaybook.const import ATable
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @task(
     validator=vol.Schema(
```

### Comparing `dataplaybook-1.0.8/dataplaybook/tasks/io_xml.py` & `dataplaybook-1.0.9/dataplaybook/tasks/io_xml.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Read XML files."""
-from collections import defaultdict
 import json
 import logging
+from collections import defaultdict
 from typing import List
 from xml.etree import ElementTree
 
 from dataplaybook import Tables, task
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `dataplaybook-1.0.8/dataplaybook/utils.py` & `dataplaybook-1.0.9/dataplaybook/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """DataEnvironment class."""
+import logging
+import re
+import sys
 from configparser import ConfigParser
 from contextlib import contextmanager
 from functools import wraps
 from importlib import import_module
-import logging
 from os import getenv
 from pathlib import Path
-import sys
 from timeit import default_timer
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Optional, Sequence
 
-from dataplaybook.config_validation import util_slugify
-
 _LOGGER = logging.getLogger(__name__)
-
+RE_SLUGIFY = re.compile(r"[^a-z0-9_]+")
 Table = List[Dict[str, Any]]
 
 
+def slugify(text: str) -> str:
+    """Slugify a given text."""
+    # text = normalize('NFKD', text)
+    text = text.lower()
+    text = text.replace(" ", "_")
+    # text = text.translate(TBL_SLUGIFY)
+    text = RE_SLUGIFY.sub("", text)
+
+    return text
+
+
 class PlaybookError(Exception):
     """Playbook Exception. These typically have warnings and can be ignored."""
 
 
 class DataVars(dict):
     """DataVars supports key access to variables."""
 
@@ -39,16 +49,16 @@
         """Set attribute."""
         self[key] = val
 
     def __setitem__(self, key: str, val: Any) -> None:
         """Ensure key is slug."""
         if key == "env":
             raise KeyError("var.env is read-only")
-        if key != util_slugify(key):
-            raise KeyError(f"Invalid variable name '{key}' use '{util_slugify(key)}")
+        if key != slugify(key):
+            raise KeyError(f"Invalid variable name '{key}' use '{slugify(key)}")
         dict.__setitem__(self, key, val)
 
     def as_table(self) -> List[Dict[str, Any]]:
         """Return as a table."""
         return [{"name": k, "value": v} for k, v in self.items()]
```

### Comparing `dataplaybook-1.0.8/dataplaybook.egg-info/SOURCES.txt` & `dataplaybook-1.0.9/dataplaybook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/setup.cfg` & `dataplaybook-1.0.9/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,55 @@
 [metadata]
 name = dataplaybook
+version = attr: dataplaybook.const.VERSION
 description = Playbooks for data. Open, process and save table based data.
-license = Apache License 2.0
-license_file = LICENSE
-author = Johann Kellerman
-author_email = kellerza@gmail.com
-url = https://github.com/kellerza/data-playbook
-platforms = any
-python_requires = >=3.5.3
 long_description = file: README.md
 long_description_content_type = text/markdown
+url = https://github.com/kellerza/data-playbook
+author = Johann Kellerman
+author_email = kellerza@gmail.com
+license = Apache License 2.0
+license_file = LICENSE
+classifiers = 
+	Development Status :: 2 - Pre-Alpha
+	Intended Audience :: Developers
+	Natural Language :: English
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+keywords = data, tables, excel, mongodb, generators
 
 [options]
+python_requires = >=3.8
 include_package_data = True
 packages = find:
+tests_requires = file: requirements_test.txt
+install_requires = 
+	colorlog
+	attrs>=21
+	voluptuous>=0.11.5
+	jinja2>=3,<4
+	openpyxl>=3,<4
+	typeguard
+	icecream
+	fuzzywuzzy
+	python-Levenshtein
+	requests
 zip_safe = False
 
+[entry_points]
+console_scripts = 
+	dataplaybook = dataplaybook.__main__:main
+
+[options.extras_require]
+mongodb = 
+	pymongo
+
 [options.packages.find]
 exclude = 
 	tests
 
 [tool:pytest]
 testpaths = tests
 norecursedirs = .git testing_config
@@ -32,23 +62,15 @@
 ignore = 
 	E501,
 	W503,
 	E203,
 	D202
 
 [isort]
-multi_line_output = 3
-include_trailing_comma = True
-force_grid_wrap = 0
-use_parentheses = True
-line_length = 88
-indent = "    "
-force_sort_within_sections = true
-forced_separate = tests
-combine_as_imports = true
+profile = black
 
 [mypy]
 python_version = 3.6
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
```

### Comparing `dataplaybook-1.0.8/tests/tasks/test_ietf.py` & `dataplaybook-1.0.9/tests/tasks/test_ietf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests for ietf.py"""
 from pathlib import Path
 
-from dataplaybook.const import ATable
 import dataplaybook.tasks.ietf as ietf
+from dataplaybook.const import ATable
 
 
 def test_extract_standards():
     """Test starting from string."""
     txt = "IEEE 802.3ah"
     std = list(ietf.extract_standards(txt))
```

### Comparing `dataplaybook-1.0.8/tests/tasks/test_init.py` & `dataplaybook-1.0.9/tests/tasks/test_init.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/tests/tasks/test_io_mongo.py` & `dataplaybook-1.0.9/tests/tasks/test_io_mongo.py`

 * *Files identical despite different names*

### Comparing `dataplaybook-1.0.8/tests/tasks/test_templates.py` & `dataplaybook-1.0.9/tests/tasks/test_templates.py`

 * *Files identical despite different names*

