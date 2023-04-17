# Comparing `tmp/gridappsd-2030_5-0.0.2a6.tar.gz` & `tmp/gridappsd-2030_5-0.0.2a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd-2030_5-0.0.2a6.tar", max compression
+gzip compressed data, was "gridappsd-2030_5-0.0.2a7.tar", max compression
```

## Comparing `gridappsd-2030_5-0.0.2a6.tar` & `gridappsd-2030_5-0.0.2a7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-04-05 21:00:20.871849 gridappsd-2030_5-0.0.2a6/LICENSE
--rw-r--r--   0        0        0    22262 2023-04-05 21:00:20.871849 gridappsd-2030_5-0.0.2a6/README.md
--rw-r--r--   0        0        0     9324 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/__main__.py
--rw-r--r--   0        0        0     5332 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/dcap.py
--rw-r--r--   0        0        0    33019 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/der.py
--rw-r--r--   0        0        0    13809 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/enddevices.py
--rw-r--r--   0        0        0     2172 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/fsa.py
--rw-r--r--   0        0        0     1938 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/log.py
--rw-r--r--   0        0        0    16470 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/mupupt.py
--rw-r--r--   0        0        0      687 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/timeadapter.py
--rw-r--r--   0        0        0     8680 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/basic_proxy.py
--rw-r--r--   0        0        0    13249 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/certs.py
--rw-r--r--   0        0        0       95 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/client/__init__.py
--rw-r--r--   0        0        0    10709 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/client/client.py
--rw-r--r--   0        0        0    10197 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/config.py
--rw-r--r--   0        0        0     3486 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/config_setup.py
--rw-r--r--   0        0        0    11071 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/control.py
--rw-r--r--   0        0        0      102 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/data/__init__.py
--rw-r--r--   0        0        0     2746 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/data/indexer.py
--rw-r--r--   0        0        0     1603 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/execute.py
--rw-r--r--   0        0        0    17604 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/flask_server.py
--rw-r--r--   0        0        0       61 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/gridappsd-2030_5.code-workspace
--rw-r--r--   0        0        0    18512 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/hrefs.py
--rw-r--r--   0        0        0    14061 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/__init__.py
--rw-r--r--   0        0        0     3715 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/constants.py
--rw-r--r--   0        0        0     3736 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/derforecasts.py
--rw-r--r--   0        0        0     3222 2023-04-05 21:00:20.875849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/enums.py
--rw-r--r--   0        0        0   281879 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/sep.py
--rw-r--r--   0        0        0        0 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/timetype.py
--rw-r--r--   0        0        0      171 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/tree.py
--rw-r--r--   0        0        0        0 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/persistance/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/persistance/points.py
--rw-r--r--   0        0        0      704 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/__init__.py
--rw-r--r--   0        0        0     9687 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/admin_endpoints.py
--rw-r--r--   0        0        0     3035 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/base_request.py
--rw-r--r--   0        0        0      533 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/dcapfs.py
--rw-r--r--   0        0        0     1361 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/derfs.py
--rw-r--r--   0        0        0     5021 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/enddevicesfs.py
--rw-r--r--   0        0        0      261 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/exceptions.py
--rw-r--r--   0        0        0     1080 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/logfs.py
--rw-r--r--   0        0        0     3303 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/meteringfs.py
--rw-r--r--   0        0        0    20710 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/server_constructs.py
--rw-r--r--   0        0        0     8857 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/server_endpoints.py
--rw-r--r--   0        0        0     1566 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/timefs.py
--rw-r--r--   0        0        0     6817 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/usage_pointfs.py
--rw-r--r--   0        0        0     2125 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/uuid_handler.py
--rw-r--r--   0        0        0     1070 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/service.py
--rw-r--r--   0        0        0        0 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/simulation/__init__.py
--rw-r--r--   0        0        0      467 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/simulation/auth_context.py
--rw-r--r--   0        0        0     6764 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/simulation/gridappsd_pump.py
--rw-r--r--   0        0        0     8909 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/simulation/inverter.py
--rw-r--r--   0        0        0     2964 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/types_/__init__.py
--rw-r--r--   0        0        0     2127 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/utils/__init__.py
--rw-r--r--   0        0        0     7829 2023-04-05 21:00:20.879849 gridappsd-2030_5-0.0.2a6/ieee_2030_5/utils/tls_wrapper.py
--rw-r--r--   0        0        0     1971 2023-04-05 21:03:51.069728 gridappsd-2030_5-0.0.2a6/pyproject.toml
--rw-r--r--   0        0        0    24823 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a6/setup.py
--rw-r--r--   0        0        0    23836 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 19:10:38.301839 gridappsd-2030_5-0.0.2a7/LICENSE
+-rw-r--r--   0        0        0    22262 2023-04-17 19:10:38.301839 gridappsd-2030_5-0.0.2a7/README.md
+-rw-r--r--   0        0        0     9324 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/__main__.py
+-rw-r--r--   0        0        0    12455 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/dcap.py
+-rw-r--r--   0        0        0    18247 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/der.py
+-rw-r--r--   0        0        0    23752 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/enddevices.py
+-rw-r--r--   0        0        0      450 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/fsa.py
+-rw-r--r--   0        0        0     1937 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/log.py
+-rw-r--r--   0        0        0    17398 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/mupupt.py
+-rw-r--r--   0        0        0      820 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/timeadapter.py
+-rw-r--r--   0        0        0     8680 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/basic_proxy.py
+-rw-r--r--   0        0        0    13249 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/certs.py
+-rw-r--r--   0        0        0       95 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/client/__init__.py
+-rw-r--r--   0        0        0    11681 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/client/client.py
+-rw-r--r--   0        0        0    10263 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/config.py
+-rw-r--r--   0        0        0     3486 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/config_setup.py
+-rw-r--r--   0        0        0    11071 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/control.py
+-rw-r--r--   0        0        0      102 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/data/__init__.py
+-rw-r--r--   0        0        0     2746 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/data/indexer.py
+-rw-r--r--   0        0        0     1603 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/execute.py
+-rw-r--r--   0        0        0    16684 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/flask_server.py
+-rw-r--r--   0        0        0       61 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/gridappsd-2030_5.code-workspace
+-rw-r--r--   0        0        0    21242 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/hrefs.py
+-rw-r--r--   0        0        0    14061 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/__init__.py
+-rw-r--r--   0        0        0     3715 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/constants.py
+-rw-r--r--   0        0        0     3736 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/derforecasts.py
+-rw-r--r--   0        0        0     3222 2023-04-17 19:10:38.305839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/enums.py
+-rw-r--r--   0        0        0   281879 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/sep.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/timetype.py
+-rw-r--r--   0        0        0      171 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/tree.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/persistance/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/persistance/points.py
+-rw-r--r--   0        0        0      704 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/__init__.py
+-rw-r--r--   0        0        0    10888 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/admin_endpoints.py
+-rw-r--r--   0        0        0     3035 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/base_request.py
+-rw-r--r--   0        0        0      533 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/dcapfs.py
+-rw-r--r--   0        0        0     2725 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/derfs.py
+-rw-r--r--   0        0        0     6670 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/enddevicesfs.py
+-rw-r--r--   0        0        0      261 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/exceptions.py
+-rw-r--r--   0        0        0     1080 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/logfs.py
+-rw-r--r--   0        0        0     3303 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/meteringfs.py
+-rw-r--r--   0        0        0    20710 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_constructs.py
+-rw-r--r--   0        0        0     8946 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_endpoints.py
+-rw-r--r--   0        0        0     1566 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/timefs.py
+-rw-r--r--   0        0        0     6817 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/usage_pointfs.py
+-rw-r--r--   0        0        0     2125 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/uuid_handler.py
+-rw-r--r--   0        0        0     1070 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/service.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/__init__.py
+-rw-r--r--   0        0        0      467 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/auth_context.py
+-rw-r--r--   0        0        0     6764 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/gridappsd_pump.py
+-rw-r--r--   0        0        0     8909 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/inverter.py
+-rw-r--r--   0        0        0     2964 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/types_/__init__.py
+-rw-r--r--   0        0        0     2220 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/__init__.py
+-rw-r--r--   0        0        0     7829 2023-04-17 19:10:38.309839 gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/tls_wrapper.py
+-rw-r--r--   0        0        0     2008 2023-04-17 19:15:42.017103 gridappsd-2030_5-0.0.2a7/pyproject.toml
+-rw-r--r--   0        0        0    24823 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a7/setup.py
+-rw-r--r--   0        0        0    23836 1970-01-01 00:00:00.000000 gridappsd-2030_5-0.0.2a7/PKG-INFO
```

### Comparing `gridappsd-2030_5-0.0.2a6/LICENSE` & `gridappsd-2030_5-0.0.2a7/LICENSE`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/README.md` & `gridappsd-2030_5-0.0.2a7/README.md`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/__main__.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/__main__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/dcap.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/dcap.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/enddevices.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/enddevices.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,330 +2,538 @@
 import uuid
 from ast import Dict
 from datetime import datetime
 from typing import List
 
 import ieee_2030_5.hrefs as hrefs
 import ieee_2030_5.models as m
-from ieee_2030_5.adapters import AdapterListProtocol, BaseAdapter, ready_signal
+from ieee_2030_5.adapters import (Adapter, AdapterListProtocol, BaseAdapter,
+                                  ready_signal)
 from ieee_2030_5.adapters.der import DERAdapter, DERProgramAdapter
 from ieee_2030_5.adapters.fsa import FSAAdapter
 from ieee_2030_5.adapters.timeadapter import TimeAdapter
 from ieee_2030_5.data.indexer import add_href
 from ieee_2030_5.models.enums import DeviceCategoryType
 from ieee_2030_5.types_ import Lfdi
+from ieee_2030_5.utils import uuid_2030_5
 
 _log = logging.getLogger(__file__)
 
-class _EndDeviceAdapter(BaseAdapter, AdapterListProtocol):
+# class _EndDeviceAdapter(BaseAdapter, AdapterListProtocol):
     
-    def __init__(self) -> None:
-        self._end_devices: List[m.EndDevice] = []
-        self._reg: Dict[int, m.Registration] = {}
-        self._fsa: List[m.FunctionSetAssignments] = []
-        self._edev_fsa: Dict[int, List[m.FunctionSetAssignments]] = {}
-        self._edev_derp: Dict[int, Dict[int, List[m.DERProgram]]] = {}
-        
-    def fetch_registration(self, edev_index: int) -> m.Registration:
-        return self._reg[edev_index]
-    
-    def fetch_fsa_list(self, edev_index: int, start: int = 0, after: int = 0, limit: int = 0) -> m.FunctionSetAssignmentsList:
-        fsa_list = m.FunctionSetAssignmentsList(
-            href=hrefs.fsa_href(edev_index=edev_index), 
-            FunctionSetAssignments=self._edev_fsa.get(edev_index, []))
-        return fsa_list
-    
-    def fetch_fsa(self, edev_index: int, fsa_index: int) -> m.FunctionSetAssignments:
-        return self._edev_fsa[edev_index][fsa_index]
-    
-    def fetch_derp_list(self, edev_index: int, fsa_index: int, start: int = 0, after: int = 0, limit: int = 0) -> m.DERProgramList:
-        derps = self._edev_derp[edev_index][fsa_index]
-        
-        derp = m.DERProgramList(href=hrefs.derp_href(edev_index=edev_index, fsa_index=fsa_index),
-                                DERProgram=derps,
-                                all=len(derps), results=len(derps))
-        
-        return derp
-        
-    def __initialize__(self, sender):
-        """ Intializes the following based upon the device configuration and the tlsrepository.
-        
-        Each EndDevice will have the following sub-components initialized:
-        - PowerStatus - PowerStatusLink
-        - DeviceStatus - DeviceStatusLink
-        - Registration - RegistrationLink
-        - MessagingProgramList - MessagingProgramListLink
-        - Log
-        Either FSA or DemandResponseProgram
-        - DemandResponseProgram - DemandResponseProgramListLink
-        
-        
-        As well as the following properties
-        - changedTime - Current time of initialization
-        - sFDI - The short form of the certificate for the system.
-        """
-        # assert EndDeviceAdapter.__tls_repository__ is not None
-        # EndDeviceAdapter.initialize_from_storage()
-        # programs = DERProgramAdapter.get_all()
-        # stored_devices = EndDeviceAdapter.get_all()
-        programs = DERProgramAdapter.fetch_edev_all()
-
-        for dev in BaseAdapter.device_configs():
-            edev = m.EndDevice()
-            edev.lFDI = BaseAdapter.__tls_repository__.lfdi(dev.id)
-            edev.sFDI = BaseAdapter.__tls_repository__.sfdi(dev.id)
-            # TODO handle enum eval in a better way.
-            edev.deviceCategory = eval(f"DeviceCategoryType.{dev.deviceCategory}")
-            edev.enabled = dev.enabled
-
-            # TODO remove subscribable
-            edev.subscribable = None
-            
-            # Add the end device to the list.
-            index = self.add(edev)
-            
-            ts = int(round(datetime.utcnow().timestamp()))
-            self._reg[index] = m.Registration(href=hrefs.registration_href(index),
-                                              pIN=dev.pin, 
-                                              dateTimeRegistered=ts)
-            edev.RegistrationLink = m.RegistrationLink(href=hrefs.registration_href(index))
-            #edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
-            
-            fsa_programs = []
-            for cfg_program in dev.programs:
-                for program in programs:
-                    program.mRID = str(uuid.uuid4())
-                    if cfg_program["description"] == program.description:
-                        fsa_programs.append(program)
+#     def __init__(self) -> None:
+#         self._end_devices: List[m.EndDevice] = []
+#         self._reg: Dict[int, m.Registration] = {}
+#         self._fsa: List[m.FunctionSetAssignments] = []
+#         self._edev_fsa: Dict[int, List[m.FunctionSetAssignments]] = {}
+#         self._edev_derp: Dict[int, Dict[int, List[m.DERProgram]]] = {}
+        
+#     def fetch_registration(self, edev_index: int) -> m.Registration:
+#         return self._reg[edev_index]
+    
+#     def fetch_fsa_list(self, edev_index: int, start: int = 0, after: int = 0, limit: int = 0) -> m.FunctionSetAssignmentsList:
+        
+#         fsa_list = FSAAdapter.fetch_all(m.FunctionSetAssignmentsList(href=hrefs.fsa_href(edev_index=edev_index)))
+        
+#         # fsa = FSAAdapter.fetch_edev_all()
+#         # fsa_list = m.FunctionSetAssignmentsList(
+#         #     href=hrefs.fsa_href(edev_index=edev_index), 
+#         #     FunctionSetAssignments=self._edev_fsa.get(edev_index, []))
+#         return fsa_list
+    
+#     def fetch_fsa(self, edev_index: int, fsa_index: int) -> m.FunctionSetAssignments:
+#         return self._edev_fsa[edev_index][fsa_index]
+    
+#     def fetch_derp_list(self, edev_index: int, fsa_index: int, start: int = 0, after: int = 0, limit: int = 0) -> m.DERProgramList:
+#         derps = self._edev_derp[edev_index][fsa_index]
+        
+#         derp = m.DERProgramList(href=hrefs.derp_href(edev_index=edev_index, fsa_index=fsa_index),
+#                                 DERProgram=derps,
+#                                 all=len(derps), results=len(derps))
+        
+#         return derp
+        
+#     def __initialize__(self, sender):
+#         """ Intializes the following based upon the device configuration and the tlsrepository.
+        
+#         Each EndDevice will have the following sub-components initialized:
+#         - PowerStatus - PowerStatusLink
+#         - DeviceStatus - DeviceStatusLink
+#         - Registration - RegistrationLink
+#         - MessagingProgramList - MessagingProgramListLink
+#         - Log
+#         Either FSA or DemandResponseProgram
+#         - DemandResponseProgram - DemandResponseProgramListLink
+        
+        
+#         As well as the following properties
+#         - changedTime - Current time of initialization
+#         - sFDI - The short form of the certificate for the system.
+#         """
+#         # assert EndDeviceAdapter.__tls_repository__ is not None
+#         # EndDeviceAdapter.initialize_from_storage()
+#         # programs = DERProgramAdapter.get_all()
+#         # stored_devices = EndDeviceAdapter.get_all()
+#         programs = DERProgramAdapter.fetch_all()
+
+#         for dev in BaseAdapter.device_configs():
+#             edev = m.EndDevice()
+#             edev.lFDI = BaseAdapter.__tls_repository__.lfdi(dev.id)
+#             edev.sFDI = BaseAdapter.__tls_repository__.sfdi(dev.id)
+#             # TODO handle enum eval in a better way.
+#             edev.deviceCategory = eval(f"DeviceCategoryType.{dev.deviceCategory}")
+#             edev.enabled = dev.enabled
+
+#             # TODO remove subscribable
+#             edev.subscribable = None
+            
+#             # Add the end device to the list.
+#             index = self.add(edev)
+            
+#             ts = int(round(datetime.utcnow().timestamp()))
+#             self._reg[index] = m.Registration(href=hrefs.registration_href(index),
+#                                               pIN=dev.pin, 
+#                                               dateTimeRegistered=ts)
+#             edev.RegistrationLink = m.RegistrationLink(href=hrefs.registration_href(index))
+#             #edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
+            
+#             fsa_programs = []
+#             for cfg_program in dev.programs:
+#                 for program in programs:
+#                     program.mRID = str(uuid.uuid4())
+#                     if cfg_program["description"] == program.description:
+#                         fsa_programs.append(program)
                     
-            if len(fsa_programs) > 0:
-                fsa = FSAAdapter.create(fsa_programs)
-                edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
-                self._fsa.append(fsa)
+#             if len(fsa_programs) > 0:
                 
-                if not self._edev_fsa.get(index):
-                    fsa_index = 0
-                    self._edev_fsa[index] = [fsa] 
-                else:
-                    fsa_index = len(self._edev_fsa)
-                    self._edev_fsa[index].append(fsa)
+#                 fsa = m.FunctionSetAssignments()
                 
-                if not self._edev_derp.get(index):
-                    self._edev_derp[index] = {}
+#                 FSAAdapter.add(fsa)
+                                
+#                 for derp in fsa_programs:                  
+#                     FSAAdapter.add_child(fsa, "fsa", derp)
+                    
+#                 edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
+                
+#                 # TODO we are hardcoding assuming only one fsa here.
+#                 fsa.DERProgramListLink = m.DERProgramListLink(href=f"{hrefs.fsa_href(index=0)}_derp")
+#                 # fsa = FSAAdapter.create(fsa_programs)
+#                 # edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
+#                 # self._fsa.append(fsa)
+                
+#                 if not self._edev_fsa.get(index):
+#                     fsa_index = 0
+#                     self._edev_fsa[index] = [fsa] 
+#                 else:
+#                     fsa_index = len(self._edev_fsa)
+#                     self._edev_fsa[index].append(fsa)
+                
+#                 if not self._edev_derp.get(index):
+#                     self._edev_derp[index] = {}
 
-                self._edev_derp[index][fsa_index] = fsa_programs
+#                 self._edev_derp[index][fsa_index] = fsa_programs
             
-            has_der = False
-            for der_indx, der in enumerate(dev.ders):                
-                DERAdapter.create(edev_index=index, der_index=der_indx, modesSupported=der["modesSupported"], deviceType=der["type"])
-                has_der = True
-            if has_der:
-                edev.DERListLink = m.DERListLink(hrefs.edev_der_href(edev_index=index))  # hrefs.der_sub_href(index=index))
+#             has_der = False
+#             for der_indx, der in enumerate(dev.ders):                
+#                 DERAdapter.create(edev_index=index, der_index=der_indx, modesSupported=der["modesSupported"], deviceType=der["type"])
+#                 has_der = True
+#             if has_der:
+#                 edev.DERListLink = m.DERListLink(hrefs.edev_der_href(edev_index=index))  # hrefs.der_sub_href(index=index))
                 
-            #self._end_devices.append(edev)
+#             #self._end_devices.append(edev)
                             
 
-            # log = m.LogEventList(href=hrefs.get_log_list_href(index),
-            #                      all=0,
-            #                      results=0,
-            #                      pollRate=BaseAdapter.server_config().log_event_list_poll_rate)
-            # edev.LogEventListLink = m.LogEventListLink(href=log.href)
-            # add_href(log.href, log)
-
-            # cfg = m.Configuration(href=hrefs.get_configuration_href(index))
-            # add_href(cfg.href, cfg)
-            # edev.ConfigurationLink = m.ConfigurationLink(cfg.href)
-
-            # ps = m.PowerStatus(href=hrefs.get_power_status_href(index))
-            # add_href(ps.href, ps)
-            # edev.PowerStatusLink = m.PowerStatusLink(href=ps.href)
-
-            # ds = m.DeviceStatus(href=hrefs.get_device_status(index))
-            # add_href(ds.href, ds)
-            # edev.DeviceStatusLink = m.DeviceStatusLink(href=ds.href)
-
-            # di = m.DeviceInformation(href=hrefs.get_device_information(index))
-            # add_href(di.href, di)
-            # edev.DeviceInformationLink = m.DeviceInformationLink(href=di.href)
-
-            # ts = int(round(datetime.utcnow().timestamp()))
-            # reg = m.Registration(href=hrefs.get_registration_href(index),
-            #                      pIN=dev.pin,
-            #                      dateTimeRegistered=ts)
-            # add_href(reg.href, reg)
-            # edev.RegistrationLink = m.RegistrationLink(reg.href)
-
-            # log = m.LogEventList(href=hrefs.get_log_list_href(index), all=0)
-            # add_href(log.href, log)
-            # edev.LogEventListLink = m.LogEventListLink(log.href)
-
-            # fsa_list = m.FunctionSetAssignmentsList(href=hrefs.get_fsa_list_href(edev.href))
-
-            # fsa = m.FunctionSetAssignments(href=hrefs.get_fsa_href(fsa_list_href=fsa_list.href,
-            #                                                        index=0),
-            #                                mRID="0F")
-            # edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(fsa_list.href)
-
-            # der_program_list = m.DERProgramList(href=hrefs.get_der_program_list(fsa_href=fsa.href),
-            #                                     all=0,
-            #                                     results=0)
-
-            # fsa.DERProgramListLink = m.DERProgramListLink(href=der_program_list.href)
-            # fsa_list.FunctionSetAssignments.append(fsa)
-
-            # for cfg_program in dev.programs:
-            #     for program in programs:
-            #         program.mRID = "1F"
-            #         if cfg_program["description"] == program.description:
-            #             der_program_list.all += 1
-            #             der_program_list.results += 1
-            #             der_program_list.DERProgram.append(program)
-            #             break
-
-            # # Allow der list here
-            # # # TODO: instantiate from config file.
-            # der_list = m.DERList(
-            #     href=hrefs.get_der_list_href(index),
-            # #pollRate=900,
-            #     results=0,
-            #     all=0)
-            # edev.DERListLink = m.DERListLink(der_list.href)
-
-            # self._end_devices.append(edev)
-
-            # edev_list.EndDevice.append(edev)
-        
-    def fetch_edev_all(self) -> List:
-        return self._end_devices
-    
-    def fetch_list(self, start: int = 0, after: int = 0, limit: int = 0) -> m.EndDeviceList:
-        enddevice_list = m.EndDeviceList(href=hrefs.get_enddevice_list_href(),
-                                         EndDevice=self._end_devices,
-                                         all = len(self._end_devices), results=len(self._end_devices))
-        return enddevice_list
-    
-    def get_at(self, index: int) -> m.EndDevice:
-        return self._end_devices[index]
-    
-    def add(self, end_device: m.EndDevice) -> int:
-        """Add and return the index of the newly added end device.
-        
-        This method will also update the href to be the current location of the resource
-        """
-        end_device.href = hrefs.get_enddevice_href(len(self._end_devices))
-        self._end_devices.append(end_device)
-        return len(self._end_devices) - 1
-    
-    def fetch_by_lfdi(self, lfdi: Lfdi) -> m.EndDevice:
-        try:
-            ed =  next(filter(lambda x: x.lFDI == lfdi, self._end_devices))
-            
-        except StopIteration:
-            ed = None
-        
-        return ed
-    
-    def fetch_list_by_lfdi(self, lfdi: Lfdi) -> m.EndDeviceList:
-        try:
-            ed =  next(filter(lambda x: x.lFDI == lfdi, self._end_devices))
-            edl = m.EndDeviceList(href=hrefs.get_enddevice_list_href(),
-                            EndDevice=[ed],
-                            all=1, results=1)
-        except StopIteration:
-            edl = m.EndDeviceList(all=0, results=0)
-        
-        return edl
-    
-    @staticmethod
-    def get_list(lfdi: Lfdi, s: int = 0, l: int = 1) -> m.EndDeviceList:
-        ed_list = m.EndDeviceList(href=hrefs.get_enddevice_list_href(), all=0, results=0)
-
-        # TODO remove as we test oeg_client.
-        ed_list.pollRate = None
-        ed_list.subscribable = None
-
-        for ed in EndDeviceAdapter.get_all():
-            if ed.lFDI == lfdi:
-                ed_list.all += 1
-                ed_list.results += 1
-                ed_list.EndDevice.append(ed)
-
-        return ed_list
-
-    @staticmethod
-    def initialize_from_storage():
-        hrefs_found = get_href_filtered(hrefs.get_enddevice_href(hrefs.NO_INDEX))
-        EndDeviceAdapter.__count__ = len(hrefs_found)
-
-    @staticmethod
-    def build(**kwargs) -> m.EndDevice:
-        ed = m.EndDevice()
-        populate_from_kwargs(ed, **kwargs)
-        return ed
-
-    @staticmethod
-    def find_index(end_device: m.EndDevice) -> int:
-        for i in range(EndDeviceAdapter.__count__ + 1):
-            if end_device.href == hrefs.get_enddevice_href(i):
-                return i
-
-        raise KeyError(f"End device not found for {end_device.href}")
-
-    @staticmethod
-    def get_by_index(index: int) -> m.EndDevice:
-        return get_href(hrefs.get_enddevice_href(index))
-
-    @staticmethod
-    def get_next_href() -> str:
-        return hrefs.get_enddevice_href(EndDeviceAdapter.get_next_index())
-
-
-    @staticmethod
-    def get_by_lfdi(lfdi: Lfdi) -> m.EndDevice:
-        for ed in EndDeviceAdapter.get_all():
-            if ed.lFDI == lfdi:
-                return ed
-        return None
-
-    @staticmethod
-    def store(device_id: str, value: m.EndDevice) -> m.EndDevice:
-        """Store the end device into temporary/permanant storage.
-        
-        The device_id is necessary to map the configured device into the linked registration
-        
-        This function will add the href and registration link to the end device.  
-        
-        """
-        if not value.href:
-            value.href = EndDeviceAdapter.get_next_href()
-        if not value.RegistrationLink:
-            reg_time = datetime.now(timezone.utc)
-            pin = None
-            for dev in BaseAdapter.__device_configurations__:
-                if dev.id == device_id:
-                    pin = dev.pin
-                    break
-
-            mreg = m.Registration(href=hrefs.get_registration_href(
-                EndDeviceAdapter.find_index(value)),
-                                  pIN=pin,
-                                  dateTimeRegistered=format_time(reg_time))
-            add_href(mreg.href, mreg)
-            value.RegistrationLink = m.RegistrationLink(mreg.href)
-
-        add_href(value.href, value)
-        return value
-
-    @staticmethod
-    def get_all() -> List[m.EndDevice]:
-        end_devices: List[m.EndDevice] = []
-        href_prefix = hrefs.get_enddevice_href(hrefs.NO_INDEX)
-        cpl = re.compile(f"{href_prefix}{hrefs.SEP}[0-9]+$")
-        for ed in get_href_filtered(href_prefix=href_prefix):
-            if cpl.match(ed.href):
-                end_devices.append(ed)
+#             # log = m.LogEventList(href=hrefs.get_log_list_href(index),
+#             #                      all=0,
+#             #                      results=0,
+#             #                      pollRate=BaseAdapter.server_config().log_event_list_poll_rate)
+#             # edev.LogEventListLink = m.LogEventListLink(href=log.href)
+#             # add_href(log.href, log)
+
+#             # cfg = m.Configuration(href=hrefs.get_configuration_href(index))
+#             # add_href(cfg.href, cfg)
+#             # edev.ConfigurationLink = m.ConfigurationLink(cfg.href)
+
+#             # ps = m.PowerStatus(href=hrefs.get_power_status_href(index))
+#             # add_href(ps.href, ps)
+#             # edev.PowerStatusLink = m.PowerStatusLink(href=ps.href)
+
+#             # ds = m.DeviceStatus(href=hrefs.get_device_status(index))
+#             # add_href(ds.href, ds)
+#             # edev.DeviceStatusLink = m.DeviceStatusLink(href=ds.href)
+
+#             # di = m.DeviceInformation(href=hrefs.get_device_information(index))
+#             # add_href(di.href, di)
+#             # edev.DeviceInformationLink = m.DeviceInformationLink(href=di.href)
+
+#             # ts = int(round(datetime.utcnow().timestamp()))
+#             # reg = m.Registration(href=hrefs.get_registration_href(index),
+#             #                      pIN=dev.pin,
+#             #                      dateTimeRegistered=ts)
+#             # add_href(reg.href, reg)
+#             # edev.RegistrationLink = m.RegistrationLink(reg.href)
+
+#             # log = m.LogEventList(href=hrefs.get_log_list_href(index), all=0)
+#             # add_href(log.href, log)
+#             # edev.LogEventListLink = m.LogEventListLink(log.href)
+
+#             # fsa_list = m.FunctionSetAssignmentsList(href=hrefs.get_fsa_list_href(edev.href))
+
+#             # fsa = m.FunctionSetAssignments(href=hrefs.get_fsa_href(fsa_list_href=fsa_list.href,
+#             #                                                        index=0),
+#             #                                mRID="0F")
+#             # edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(fsa_list.href)
+
+#             # der_program_list = m.DERProgramList(href=hrefs.get_der_program_list(fsa_href=fsa.href),
+#             #                                     all=0,
+#             #                                     results=0)
+
+#             # fsa.DERProgramListLink = m.DERProgramListLink(href=der_program_list.href)
+#             # fsa_list.FunctionSetAssignments.append(fsa)
+
+#             # for cfg_program in dev.programs:
+#             #     for program in programs:
+#             #         program.mRID = "1F"
+#             #         if cfg_program["description"] == program.description:
+#             #             der_program_list.all += 1
+#             #             der_program_list.results += 1
+#             #             der_program_list.DERProgram.append(program)
+#             #             break
+
+#             # # Allow der list here
+#             # # # TODO: instantiate from config file.
+#             # der_list = m.DERList(
+#             #     href=hrefs.get_der_list_href(index),
+#             # #pollRate=900,
+#             #     results=0,
+#             #     all=0)
+#             # edev.DERListLink = m.DERListLink(der_list.href)
+
+#             # self._end_devices.append(edev)
+
+#             # edev_list.EndDevice.append(edev)
+        
+#     def fetch_edev_all(self) -> List:
+#         return self._end_devices
+    
+#     def fetch_list(self, start: int = 0, after: int = 0, limit: int = 0) -> m.EndDeviceList:
+#         enddevice_list = m.EndDeviceList(href=hrefs.get_enddevice_list_href(),
+#                                          EndDevice=self._end_devices,
+#                                          all = len(self._end_devices), results=len(self._end_devices))
+#         return enddevice_list
+    
+#     def get_at(self, index: int) -> m.EndDevice:
+#         return self._end_devices[index]
+    
+#     def add(self, end_device: m.EndDevice) -> int:
+#         """Add and return the index of the newly added end device.
+        
+#         This method will also update the href to be the current location of the resource
+#         """
+#         end_device.href = hrefs.get_enddevice_href(len(self._end_devices))
+#         self._end_devices.append(end_device)
+#         return len(self._end_devices) - 1
+    
+#     def fetch_by_lfdi(self, lfdi: Lfdi) -> m.EndDevice:
+#         try:
+#             ed =  next(filter(lambda x: x.lFDI == lfdi, self._end_devices))
+            
+#         except StopIteration:
+#             ed = None
+        
+#         return ed
+    
+#     def fetch_list_by_lfdi(self, lfdi: Lfdi) -> m.EndDeviceList:
+#         try:
+#             ed =  next(filter(lambda x: x.lFDI == lfdi, self._end_devices))
+#             edl = m.EndDeviceList(href=hrefs.get_enddevice_list_href(),
+#                             EndDevice=[ed],
+#                             all=1, results=1)
+#         except StopIteration:
+#             edl = m.EndDeviceList(all=0, results=0)
+        
+#         return edl
+    
+#     @staticmethod
+#     def get_list(lfdi: Lfdi, s: int = 0, l: int = 1) -> m.EndDeviceList:
+#         ed_list = m.EndDeviceList(href=hrefs.get_enddevice_list_href(), all=0, results=0)
+
+#         # TODO remove as we test oeg_client.
+#         ed_list.pollRate = None
+#         ed_list.subscribable = None
+
+#         for ed in EndDeviceAdapter.get_all():
+#             if ed.lFDI == lfdi:
+#                 ed_list.all += 1
+#                 ed_list.results += 1
+#                 ed_list.EndDevice.append(ed)
+
+#         return ed_list
+
+#     @staticmethod
+#     def initialize_from_storage():
+#         hrefs_found = get_href_filtered(hrefs.get_enddevice_href(hrefs.NO_INDEX))
+#         EndDeviceAdapter.__count__ = len(hrefs_found)
+
+#     @staticmethod
+#     def build(**kwargs) -> m.EndDevice:
+#         ed = m.EndDevice()
+#         populate_from_kwargs(ed, **kwargs)
+#         return ed
+
+#     @staticmethod
+#     def find_index(end_device: m.EndDevice) -> int:
+#         for i in range(EndDeviceAdapter.__count__ + 1):
+#             if end_device.href == hrefs.get_enddevice_href(i):
+#                 return i
+
+#         raise KeyError(f"End device not found for {end_device.href}")
+
+#     @staticmethod
+#     def get_by_index(index: int) -> m.EndDevice:
+#         return get_href(hrefs.get_enddevice_href(index))
+
+#     @staticmethod
+#     def get_next_href() -> str:
+#         return hrefs.get_enddevice_href(EndDeviceAdapter.get_next_index())
+
+
+#     @staticmethod
+#     def get_by_lfdi(lfdi: Lfdi) -> m.EndDevice:
+#         for ed in EndDeviceAdapter.get_all():
+#             if ed.lFDI == lfdi:
+#                 return ed
+#         return None
+
+#     @staticmethod
+#     def store(device_id: str, value: m.EndDevice) -> m.EndDevice:
+#         """Store the end device into temporary/permanant storage.
+        
+#         The device_id is necessary to map the configured device into the linked registration
+        
+#         This function will add the href and registration link to the end device.  
+        
+#         """
+#         if not value.href:
+#             value.href = EndDeviceAdapter.get_next_href()
+#         if not value.RegistrationLink:
+#             reg_time = datetime.now(timezone.utc)
+#             pin = None
+#             for dev in BaseAdapter.__device_configurations__:
+#                 if dev.id == device_id:
+#                     pin = dev.pin
+#                     break
+
+#             mreg = m.Registration(href=hrefs.get_registration_href(
+#                 EndDeviceAdapter.find_index(value)),
+#                                   pIN=pin,
+#                                   dateTimeRegistered=format_time(reg_time))
+#             add_href(mreg.href, mreg)
+#             value.RegistrationLink = m.RegistrationLink(mreg.href)
+
+#         add_href(value.href, value)
+#         return value
+
+#     @staticmethod
+#     def get_all() -> List[m.EndDevice]:
+#         end_devices: List[m.EndDevice] = []
+#         href_prefix = hrefs.get_enddevice_href(hrefs.NO_INDEX)
+#         cpl = re.compile(f"{href_prefix}{hrefs.SEP}[0-9]+$")
+#         for ed in get_href_filtered(href_prefix=href_prefix):
+#             if cpl.match(ed.href):
+#                 end_devices.append(ed)
+
+#         return sorted(end_devices, key=lambda k: k.href)
+
+# EndDeviceAdapter = _EndDeviceAdapter()
+# ready_signal.connect(EndDeviceAdapter.__initialize__, DERProgramAdapter)
+
+EndDeviceAdapter = Adapter[m.EndDevice](hrefs.get_enddevice_href(), generic_type=m.EndDevice)
+def initialize_end_device_adapter(sender):
+    """ Intializes the following based upon the device configuration and the tlsrepository.
+        
+    Each EndDevice will have the following sub-components initialized:
+    - PowerStatus - PowerStatusLink
+    - DeviceStatus - DeviceStatusLink
+    - Registration - RegistrationLink
+    - MessagingProgramList - MessagingProgramListLink
+    - Log
+    Either FSA or DemandResponseProgram
+    - DemandResponseProgram - DemandResponseProgramListLink
+    
+    
+    As well as the following properties
+    - changedTime - Current time of initialization
+    - sFDI - The short form of the certificate for the system.
+    """
+    # assert EndDeviceAdapter.__tls_repository__ is not None
+    # EndDeviceAdapter.initialize_from_storage()
+    # programs = DERProgramAdapter.get_all()
+    # stored_devices = EndDeviceAdapter.get_all()
+    programs = DERProgramAdapter.fetch_all()
+
+    for dev in BaseAdapter.device_configs():
+        ts = int(round(datetime.utcnow().timestamp()))
+        
+        edev = m.EndDevice()
+        edev.lFDI = BaseAdapter.__tls_repository__.lfdi(dev.id)
+        edev.sFDI = BaseAdapter.__tls_repository__.sfdi(dev.id)
+        # TODO handle enum eval in a better way.
+        edev.deviceCategory = eval(f"DeviceCategoryType.{dev.deviceCategory}")
+        edev.enabled = dev.enabled
+        edev.changedTime = ts
+
+        # TODO remove subscribable
+        edev.subscribable = None
+        
+        
+        EndDeviceAdapter.add(edev)
+        
+        # Add the end device to the list.
+        index = EndDeviceAdapter.fetch_index(edev)
+        
+        
+        EndDeviceAdapter.add_child(edev, hrefs.END_DEVICE_REGISTRATION, 
+                                   m.Registration(href=hrefs.registration_href(index), pIN=dev.pin, dateTimeRegistered=ts))
+        edev.RegistrationLink = m.RegistrationLink(href=hrefs.registration_href(index))
+        
+        di = hrefs.EdevHref(edev_index=index, edev_subtype=hrefs.EDevSubType.DeviceInformation)
+        EndDeviceAdapter.add_child(edev, hrefs.END_DEVICE_INFORMATION, m.DeviceInformation(href=str(di)))
+        edev.DeviceInformationLink = m.DeviceInformationLink(str(di))
+        
+        ds = hrefs.EdevHref(edev_index=index, edev_subtype=hrefs.EDevSubType.DeviceStatus)
+        EndDeviceAdapter.add_child(edev, hrefs.END_DEVICE_STATUS, m.DeviceStatus(str(ds)))
+        edev.DeviceStatusLink = m.DeviceStatusLink(str(ds))
+        
+        #edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
+        
+        fsa_programs = []
+        for cfg_program in dev.programs:
+            for program in programs:
+                program.mRID = uuid_2030_5()
+                if cfg_program["description"] == program.description:
+                    fsa_programs.append(program)
+                
+        if len(fsa_programs) > 0:
+            
+            fsa = m.FunctionSetAssignments()
+            
+            FSAAdapter.add(fsa)
+                            
+            for derp in fsa_programs:                  
+                FSAAdapter.add_child(fsa, hrefs.FSA, derp)
+                
+            edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
+            
+            # TODO we are hardcoding assuming only one fsa here.
+            fsa.DERProgramListLink = m.DERProgramListLink(href=f"{hrefs.fsa_href(index=0)}_{hrefs.DER_PROGRAM}")
+            # fsa = FSAAdapter.create(fsa_programs)
+            # edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(href=hrefs.fsa_href(edev_index=index))
+            # self._fsa.append(fsa)
+            EndDeviceAdapter.add_child(edev, hrefs.FSA, fsa)
+            
+        has_der = False
+        for der_indx, der_cfg in enumerate(dev.ders):
+            der_href = hrefs.EdevHref(edev_index=index, edev_subtype=hrefs.EDevSubType.DER, edev_subtype_index=der_indx)
+            der = m.DER(href=str(der_href))
+            der_href.edev_der_subtype = hrefs.DERSubType.Availability
+            der.DERAvailabilityLink = m.DERAvailabilityLink(str(der_href))
+            
+            der_href.edev_der_subtype = hrefs.DERSubType.Capability
+            der.DERCapabilityLink = m.DERCapabilityLink(str(der_href))
+            
+            der_href.edev_der_subtype = hrefs.DERSubType.Settings
+            der.DERSettingsLink = m.DERSettingsLink(str(der_href))
+            
+            der_href.edev_der_subtype = hrefs.DERSubType.Status
+            der.DERStatusLink = m.DERStatusLink(str(der_href))
+            
+            # Configure a link to the current program for the der.
+            cfg_der_program = der_cfg.get("program")
+            if cfg_der_program:
+                for derp_index, derp in enumerate(programs):
+                    if cfg_der_program == derp.description:
+                        der.CurrentDERProgramLink = derp.href
+                        break
+            
+            
+            EndDeviceAdapter.add_child(edev, hrefs.DER, der)
+            has_der = True
+            
+        if has_der:
+            edev.DERListLink = m.DERListLink(hrefs.edev_der_href(edev_index=index))  # hrefs.der_sub_href(index=index))
+    
+    ready_signal.send(EndDeviceAdapter)
+        #self._end_devices.append(edev)
+                        
+
+        # log = m.LogEventList(href=hrefs.get_log_list_href(index),
+        #                      all=0,
+        #                      results=0,
+        #                      pollRate=BaseAdapter.server_config().log_event_list_poll_rate)
+        # edev.LogEventListLink = m.LogEventListLink(href=log.href)
+        # add_href(log.href, log)
+
+        # cfg = m.Configuration(href=hrefs.get_configuration_href(index))
+        # add_href(cfg.href, cfg)
+        # edev.ConfigurationLink = m.ConfigurationLink(cfg.href)
+
+        # ps = m.PowerStatus(href=hrefs.get_power_status_href(index))
+        # add_href(ps.href, ps)
+        # edev.PowerStatusLink = m.PowerStatusLink(href=ps.href)
+
+        # ds = m.DeviceStatus(href=hrefs.get_device_status(index))
+        # add_href(ds.href, ds)
+        # edev.DeviceStatusLink = m.DeviceStatusLink(href=ds.href)
+
+        # di = m.DeviceInformation(href=hrefs.get_device_information(index))
+        # add_href(di.href, di)
+        # edev.DeviceInformationLink = m.DeviceInformationLink(href=di.href)
+
+        # ts = int(round(datetime.utcnow().timestamp()))
+        # reg = m.Registration(href=hrefs.get_registration_href(index),
+        #                      pIN=dev.pin,
+        #                      dateTimeRegistered=ts)
+        # add_href(reg.href, reg)
+        # edev.RegistrationLink = m.RegistrationLink(reg.href)
+
+        # log = m.LogEventList(href=hrefs.get_log_list_href(index), all=0)
+        # add_href(log.href, log)
+        # edev.LogEventListLink = m.LogEventListLink(log.href)
+
+        # fsa_list = m.FunctionSetAssignmentsList(href=hrefs.get_fsa_list_href(edev.href))
+
+        # fsa = m.FunctionSetAssignments(href=hrefs.get_fsa_href(fsa_list_href=fsa_list.href,
+        #                                                        index=0),
+        #                                mRID="0F")
+        # edev.FunctionSetAssignmentsListLink = m.FunctionSetAssignmentsListLink(fsa_list.href)
+
+        # der_program_list = m.DERProgramList(href=hrefs.get_der_program_list(fsa_href=fsa.href),
+        #                                     all=0,
+        #                                     results=0)
+
+        # fsa.DERProgramListLink = m.DERProgramListLink(href=der_program_list.href)
+        # fsa_list.FunctionSetAssignments.append(fsa)
+
+        # for cfg_program in dev.programs:
+        #     for program in programs:
+        #         program.mRID = "1F"
+        #         if cfg_program["description"] == program.description:
+        #             der_program_list.all += 1
+        #             der_program_list.results += 1
+        #             der_program_list.DERProgram.append(program)
+        #             break
+
+        # # Allow der list here
+        # # # TODO: instantiate from config file.
+        # der_list = m.DERList(
+        #     href=hrefs.get_der_list_href(index),
+        # #pollRate=900,
+        #     results=0,
+        #     all=0)
+        # edev.DERListLink = m.DERListLink(der_list.href)
 
-        return sorted(end_devices, key=lambda k: k.href)
+        # self._end_devices.append(edev)
 
-EndDeviceAdapter = _EndDeviceAdapter()
-ready_signal.connect(EndDeviceAdapter.__initialize__, DERProgramAdapter)
+        # edev_list.EndDevice.append(edev)
+ready_signal.connect(initialize_end_device_adapter, DERProgramAdapter)
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/log.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 _log = logging.getLogger(__name__)
 class _LogAdapter:
     
     def __init__(self):
         pass        
     
-    def __after_base_init__(self, sender):
-        
+    def __after_base_init__(self, sender):        
         print("after base init")
         print(sender)
 
     @staticmethod
     def store(path: str, logevent: m.LogEvent):
         """Store a logevent to the given path.
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/mupupt.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/mupupt.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,35 @@
 @dataclass
 class _UsagePointWrapper:
     usage_point: m.UsagePoint   
     meter_readings: List[m.MeterReading] = field(default_factory=list)
     mirror_meter_readings: List[m.MirrorMeterReading] = field(default_factory=list)
     
     def fetch_reading_by_mRID(self, mRID) -> m.MeterReading:
-        return next(filter(lambda x: x.mRID == mRID, self.meter_readings))
+        for x in self.meter_readings:
+            if x.mRID == mRID:
+                return x
+        raise StopIteration()
+        #return next(filter(lambda x: x.mRID == mRID, self.meter_readings))
     
     def fetch_mirror_meter_reading_index(self, mRID: str) -> int:
-        return next(i for i, v in enumerate(self.mirror_meter_readings) if v.mRID == mRID)
+        for i, v in enumerate(self.mirror_meter_readings):
+            if v.mRID == mRID:
+                return i
+        raise StopIteration()
+        # return next(i for i, v in enumerate(self.mirror_meter_readings) if v.mRID == mRID)
     
     
 @dataclass
 class _UsagePointContainer(Container, Sized):
     __usage_points__: List[_UsagePointWrapper] = field(default_factory=list)
     
     def create_or_replace_reading(self, usage_point: m.UsagePoint, mirror_meter_reading: m.MirrorMeterReading) -> Tuple[ReturnCode, str]:
         
-        assert usage_point in self, "Passed usage_point not contained within container/"
+        assert usage_point in self, "Passed usage_point not contained within container"
         
         try:
             wrapper = self._fetch_wrapper_by_mRID(usage_point.mRID)
         except StopIteration:
             _log.error(f"Wrapper not found for usage point {usage_point}")
         else:
             try:
@@ -70,18 +78,19 @@
                 
     
     def create_or_replace(self, mirror_usage_point: m.MirrorUsagePoint) -> m.UsagePoint:
         
         if mirror_usage_point in self:
             
             upt = self.fetch_by_mRID(mirror_usage_point.mRID)
+            if not isinstance(upt, m.UsagePoint):
+                raise ValueError("blah")
             upt.description=mirror_usage_point.description,
             upt.deviceLFDI=mirror_usage_point.deviceLFDI,
             upt.version=mirror_usage_point.version,
-            upt.mRID=mirror_usage_point.mRID,
             upt.serviceCategoryKind=mirror_usage_point.serviceCategoryKind,
             upt.status=mirror_usage_point.status
             
         else:
             # 1. Since creating we can use the length of the __usage_points__ for determining the 
             #    next href
             upt = m.UsagePoint(href=hrefs.usage_point_href(len(UsagePointContainer)),
@@ -89,15 +98,15 @@
                             deviceLFDI=mirror_usage_point.deviceLFDI,
                             version=mirror_usage_point.version,
                             mRID=mirror_usage_point.mRID,
                             serviceCategoryKind=mirror_usage_point.serviceCategoryKind,
                             status=mirror_usage_point.status)
                         
             wrapper = _UsagePointWrapper(usage_point=upt)            
-            UsagePointContainer.__usage_points__.append(wrapper)
+            self.__usage_points__.append(wrapper)
             
         if mirror_usage_point.MirrorMeterReading:
             wrapper = self._fetch_wrapper_by_mRID(mirror_usage_point.mRID)
             for reading in mirror_usage_point.MirrorMeterReading:
                 self.create_or_replace_reading(upt, reading)
                 
         return upt
@@ -113,32 +122,50 @@
         uptl = m.UsagePointList(href=hrefs.usage_point_href(),
                                 UsagePoint=[upw.usage_point for upw in self.__usage_points__],
                                 all=len(self.__usage_points__),
                                 results=len(self.__usage_points__))
         return uptl
     
     def fetch_by_href(self, href: str) -> m.UsagePoint:
-        return next(filter(lambda x: x.href == href, [y.usage_point for y in self.__usage_points__]))
+        for x in self.__usage_points__:
+            if x.usage_point.href == href:
+                return x.usage_point
+        raise StopIteration()
+        # return next(filter(lambda x: x.href == href, [y.usage_point for y in self.__usage_points__]))
     
     def fetch_by_mRID(self, mRID: str) -> m.UsagePoint:
-        return next(filter(lambda x: x.mRID == mRID, [y.usage_point for y in self.__usage_points__]))
+        for x in self.__usage_points__:
+            if x.usage_point.mRID == mRID:
+                return x.usage_point
+        
+        raise StopIteration()
+        # return next(filter(lambda x: x.mRID == mRID, [y.usage_point for y in self.__usage_points__]))
     
     def _fetch_wrapper_by_mRID(self, mRID: str) -> _UsagePointWrapper:
-        print(self.__usage_points__)
         for x in self.__usage_points__:
+            print(f"Comparing {x.usage_point.mRID} to {mRID}")
             if x.usage_point.mRID == mRID:
                 return x
         
         raise StopIteration()
     
     def _fetch_wrapper_by_href(self, href: str) -> _UsagePointWrapper:
-        return next(filter(lambda x: x.usage_point.href == href, self.__usage_points__))
+        for x in self.__usage_points__:
+            if x.usage_point.href == href:
+                return x
+        
+        raise StopIteration()
+        #return next(filter(lambda x: x.usage_point.href == href, self.__usage_points__))
 
     def __contains__(self, other: object) -> bool:
-        return list(filter(lambda x: x.usage_point.mRID == other.mRID, self.__usage_points__))
+        for x in self.__usage_points__:
+            if x.usage_point.mRID == other.mRID:
+                return True
+        return False
+        # return list(filter(lambda x: x.usage_point.mRID == other.mRID, self.__usage_points__))
     
     def __len__(self) -> int:
         return len(self.__usage_points__)
 
 UsagePointContainer = _UsagePointContainer()
 
 @dataclass
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/adapters/timeadapter.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/adapters/timeadapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from threading import Thread
 
 from blinker import Signal
 
 
 class _TimeAdapter(Thread):
     tick = Signal("tick")
-    def __init__(self):
-        super().__init__()
-        self._tick = 0
-        
+            
     @staticmethod
-    def user_readable(timestamp: int):
+    def user_readable(timestamp: int) -> str:
         dt = datetime.fromtimestamp(timestamp)
-        return dt.strftime("%m/%d/%Y, %H:%M:%S")
+        return dt.isoformat() # .strftime("%m/%d/%Y, %H:%M:%S")
+    
+    @staticmethod
+    def from_iso(iso_fmt_date: str) -> int:
+        dt = datetime.strptime(iso_fmt_date, "%Y-%m-%dT%H:%M:%S")
+        return int(time.mktime(dt.timetuple()))
     
     def run(self) -> None:
         
         while True:
             self._tick = int(time.mktime(datetime.utcnow().timetuple()))
             _TimeAdapter.tick.send(self._tick)
             time.sleep(1)
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/basic_proxy.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/basic_proxy.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/certs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/certs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/client/client.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,25 +85,30 @@
 
         if response.status in (200, 201):
             return response.headers.get("Location")
 
         raise werkzeug.exceptions.Forbidden()
 
 
+    def get(self, href):
+        return self.__get_request__(href)
 
 
     def is_end_device_registered(self, end_device: m.EndDevice, pin: int) -> bool:
         reg = self.registration(end_device)
         return reg.pIN == pin
 
     def new_uuid(self, url: str = "/uuid") -> str:
         res = self.__get_request__(url)
         return res
 
     def end_devices(self) -> m.EndDeviceListLink:
+        if not self._device_cap:
+            self.device_capability()
+            
         self._end_devices = self.__get_request__(self._device_cap.EndDeviceListLink.href)
         return self._end_devices
 
     def end_device(self, index: Optional[int] = 0) -> m.EndDevice:
         if not self._end_devices:
             self.end_devices()
 
@@ -111,17 +116,25 @@
 
     def self_device(self) -> m.EndDevice:
         if not self._device_cap:
             self.device_capability()
 
         return self.__get_request__(self._device_cap.SelfDeviceLink.href)
 
-    def function_set_assignment(self) -> m.FunctionSetAssignmentsListLink:
-        fsa_list = self.__get_request__(self.end_device().FunctionSetAssignmentsListLink.href)
+    def function_set_assignment_list(self, edev_index: Optional[int] = 0) -> m.FunctionSetAssignmentsList:
+        fsa_list = self.__get_request__(self.end_device(edev_index).FunctionSetAssignmentsListLink.href)
         return fsa_list
+        
+    def function_set_assignment(self, edev_index: Optional[int] = 0, fsa_index: Optional[int] = 0) -> m.FunctionSetAssignments:
+        fsa_list = self.function_set_assignment_list(edev_index)
+        return fsa_list.FunctionSetAssignments[fsa_index]
+    
+    def der_list(self, edev_index: Optional[int] = 0) -> m.DERList:
+        der_list = self.__get_request__(self.end_device(edev_index).DERListLink.href)
+        return der_list
 
     def poll_timer(self, fn, args):
         if not self._disconnect:
             _log.debug(threading.currentThread().name)
             fn(args)
             threading.currentThread().join()
 
@@ -139,19 +152,23 @@
         # self._dcap_timer.start()
         return self._device_cap
 
     def time(self) -> m.Time:
         timexml = self.__get_request__(self._device_cap.TimeLink.href)
         return timexml
 
-    def der_program_list(self, device: m.EndDevice) -> m.DERProgramList:
-        fsa: m.FunctionSetAssignments = self.__get_request__(device.FunctionSetAssignmentsListLink.href)
-        der_programs_list: m.DERProgramList = self.__get_request__(fsa.DERProgramListLink.href)
-
-        return der_programs_list
+    def der_program_list(self, edev_index: Optional[int] = 0, fsa_index: Optional[int] = 0) -> m.DERProgramList:
+        fsa = self.function_set_assignment(edev_index, fsa_index)
+        derp_list = self.__get_request__(fsa.DERProgramListLink.href)
+        return derp_list
+    
+    def der_program(self, edev_index: Optional[int] = 0, fsa_index: Optional[int] = 0, derp_index: Optional[int] = 0) -> m.DERProgram:
+        derp_list = self.der_program_list(edev_index, fsa_index)
+        return derp_list.DERProgram[derp_index]
+    
 
     def mirror_usage_point_list(self) -> m.MirrorUsagePointList:
         self._mup = self.__get_request__(self._device_cap.MirrorUsagePointListLink.href)
         return self._mup
 
     def usage_point_list(self) -> m.UsagePointList:
         self._upt = self.__get_request__(self._device_cap.UsagePointListLink.href)
@@ -164,29 +181,30 @@
     def timelink(self):
         if self._device_cap is None:
             raise ValueError("Request device capability first")
         return self.__get_request__(url=self._device_cap.TimeLink.href)
 
     def disconnect(self):
         self._disconnect = True
-        self._dcap_timer.cancel()
+        if self._dcap_timer:
+            self._dcap_timer.cancel()
         IEEE2030_5_Client.clients.remove(self)
 
     def request(self, endpoint: str, body: dict = None, method: str = "GET",
                 headers: dict = None):
 
         if method.upper() == 'GET':
             return self.__get_request__(endpoint, body, headers=headers)
 
         if method.upper() == 'POST':
             print("Doing post")
             return self.__post__(endpoint, body, headers=headers)
 
     def create_mirror_usage_point(self, mirror_usage_point: m.MirrorUsagePoint) -> Tuple[int, str]:
-        data = dataclass_to_xml(mirror_usage_point)
+        data = utils.dataclass_to_xml(mirror_usage_point)
         resp = self.__post__(self._device_cap.MirrorUsagePointListLink.href, data=data)
         return resp.status, resp.headers['Location']
 
     def __post__(self, url: str, data=None, headers: Optional[Dict[str, str]]=None):
         if not headers:
             headers = {'Content-Type': 'text/xml'}
 
@@ -249,36 +267,38 @@
 #                       cert_file=str(CERT_FILE),
 #                       context=ssl_context)
 # con.request("GET", "/dcap")
 # print(con.getresponse().read())
 # con.close()
 
 if __name__ == '__main__':
-    SERVER_CA_CERT = Path("~/tls/certs/ca.crt").expanduser().resolve()
+    SERVER_CA_CERT = Path("~/tls/certs/ca.pem").expanduser().resolve()
     KEY_FILE = Path("~/tls/private/dev1.pem").expanduser().resolve()
-    CERT_FILE = Path("~/tls/certs/dev1.crt").expanduser().resolve()
+    CERT_FILE = Path("~/tls/certs/dev1.pem").expanduser().resolve()
 
     headers = {'Connection': 'Keep-Alive',
                'Keep-Alive': "max=1000,timeout=30"}
 
     h = IEEE2030_5_Client(cafile=SERVER_CA_CERT,
                           server_hostname="127.0.0.1",
-                          server_ssl_port=8070,
+                          server_ssl_port=8443,
                           keyfile=KEY_FILE,
                           certfile=CERT_FILE,
                           debug=True)
     # h2 = IEEE2030_5_Client(cafile=SERVER_CA_CERT, server_hostname="me.com", ssl_port=8000,
     #                        keyfile=KEY_FILE, certfile=KEY_FILE)
     dcap = h.device_capability()
     end_devices = h.end_devices()
 
     if not end_devices.all > 0:
         print("registering end device.")
         ed_href = h.register_end_device()
     my_ed = h.end_devices()
+    my_fsa = h.function_set_assignment()
+    my_program = h.der_program()
 
 
     # ed = h.end_devices()[0]
     # resp = h.request("/dcap", headers=headers)
     # print(resp)
     # resp = h.request("/dcap", headers=headers)
     # print(resp)
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/config.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,16 +175,14 @@
         Literal["enddevices_create_on_start"],
         Literal["enddevices_register_access_only"]] = "enddevices_register_access_only"
 
     lfdi_mode: Union[
         Literal["lfdi_mode_from_file"],
         Literal["lfdi_mode_from_cert_fingerprint"]] = "lfdi_mode_from_cert_fingerprint"
 
-    # Can include ip address as well
-    server_hostname: str = None
 
     programs: List[DERProgramConfiguration] = field(default_factory=list)
     controls: List[DERControlConfiguration] = field(default_factory=list)
     curves: List[DERCurveConfiguration] = field(default_factory=list)
     events: List[Dict] = field(default_factory=list)
 
     # # map into program_lists array for programs for specific
@@ -194,21 +192,28 @@
     # fsa_list: List[FunctionSetAssignments] = field(default_factory=list)
     # curve_list: List[DERCurve] = field(default_factory=list)
 
     proxy_hostname: Optional[str] = None
     gridappsd: Optional[GridappsdConfiguration] = None
     # DefaultDERControl: Optional[DefaultDERControl] = None
     # DERControlList: Optional[DERControl] = field(default=list)
+    
+    @property
+    def server_hostname(self) -> str:
+        server = self.server
+        if self.https_port:
+            server = server + f":{self.https_port}"
+            
+        return server
 
     @classmethod
     def from_dict(cls, env):
         return cls(**{k: v for k, v in env.items() if k in inspect.signature(cls).parameters})
 
     def __post_init__(self):
-        self.server_hostname = f"{self.server}:{self.https_port}"
         self.curves = [DERCurveConfiguration.from_dict(x) for x in self.curves]
         self.controls = [DERControlConfiguration.from_dict(x) for x in self.controls]
         self.programs = [DERProgramConfiguration.from_dict(x) for x in self.programs]
         self.devices = [DeviceConfiguration.from_dict(x) for x in self.devices]
         for d in self.devices:
             d.deviceCategory = eval(f"m.DeviceCategoryType.{d.deviceCategory}").name
             #d.device_category_type = eval(f"m.DeviceCategoryType.{d.device_category_type}")
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/config_setup.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/config_setup.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/control.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/control.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/data/indexer.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/data/indexer.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/execute.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/execute.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/flask_server.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/flask_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,17 +100,17 @@
                 cert, key = self.tlsrepo.get_file_pair("admin")
                 x509 = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert)
             else:
                 x509_binary = self.connection.getpeercert(True)
                 x509 = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_ASN1, x509_binary)
             environ['ieee_2030_5_peercert'] = x509
             environ['ieee_2030_5_serial_number'] = x509.get_serial_number()
-            if self.config.lfdi_mode == "lfdi_mode_from_file":
+            if PeerCertWSGIRequestHandler.config.lfdi_mode == "lfdi_mode_from_file":
                 _log.debug("Using hash from combined file.")
-                pth = self.tlsrepo.__get_combined_file__(x509.get_subject().CN)
+                pth = PeerCertWSGIRequestHandler.tlsrepo.__get_combined_file__(x509.get_subject().CN)
                 sha256hash = hashlib.sha256(pth.read_text().encode('utf-8')).hexdigest()
                 environ['ieee_2030_5_lfdi'] = lfdi_from_fingerprint(sha256hash)
             else:
                 environ['ieee_2030_5_lfdi'] = lfdi_from_fingerprint(
                     x509.digest("sha256").decode('ascii'))
             environ['ieee_2030_5_sfdi'] = sfdi_from_lfdi(environ['ieee_2030_5_lfdi'])
 
@@ -392,60 +392,29 @@
         http_app = __build_http_app__(config=config)
 
     PeerCertWSGIRequestHandler.config = config
     PeerCertWSGIRequestHandler.tlsrepo = tlsrepo
 
     run_app(app=app, host=host, ssl_context=ssl_context, port=port, request_handler=PeerCertWSGIRequestHandler, **kwargs)
     
-    # # kwargs['ssl_context'] = ssl_context
-    # # kwargs['request_handler'] = PeerCertWSGIRequestHandler,
-    # # kwargs['port'] = port
-    # #kwargs.pop('debug', None)
-    # https_thread = threading.Thread(
-    #     target=run_app,
-    #     args=[app, host, ssl_context, PeerCertWSGIRequestHandler, port],
-    #     kwargs=kwargs)
-    # https_thread.daemon = True
-    # https_thread.start()
-
-    # if config.http_port:
-
-    #     http_thread = threading.Thread(target=run_app,
-    #                                    args=[app, host, None, None, config.http_port],
-    #                                    kwargs=kwargs)
-
-    #     http_thread.daemon = True
-    #     http_thread.start()
-
-    #     while http_thread.isAlive() and https_thread.isAlive():
-    #         time.sleep(0.05)
-    # else:
-    #     while https_thread.is_alive():
-    #         time.sleep(0.05)
-
-    # app.run(host=host,
-    #         ssl_context=ssl_context,
-    #         request_handler=PeerCertWSGIRequestHandler,
-    #         port=port,
-    #         **kwargs)
-
-    print("Woot?")
-
 
 def build_server(config: ServerConfiguration, tlsrepo: TLSRepository, **kwargs) -> BaseWSGIServer:
 
     app = __build_app__(config, tlsrepo)
     ssl_context = __build_ssl_context__(tlsrepo)
 
     try:
         host, port = config.server_hostname.split(":")
     except ValueError:
         # host and port not available
         host = config.server_hostname
         port = 8443
+        
+    PeerCertWSGIRequestHandler.config = config
+    PeerCertWSGIRequestHandler.tlsrepo = tlsrepo
 
     return make_server(app=app,
                        host=host,
                        ssl_context=ssl_context,
                        request_handler=PeerCertWSGIRequestHandler,
                        port=port,
                        **kwargs)
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/hrefs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/hrefs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,83 +14,111 @@
 MSG = "msg"
 DER = "der"
 CURVE = "dc"
 RSPS = "rsps"
 LOG = "log"
 DERC = "derc"
 DDERC = "dderc"
-FSA = "fsa"
-DERP = "derp"
 DERCA = "derca"
+FSA = "fsa"
+
+DER_PROGRAM = "derp"
+# DER Available
+DER_AVAILABILITY = "dera"
+# DER Status
+DER_STATUS = "ders"
+DER_CONTROL_ACTIVE = DERCA
+# Settings
+DER_SETTINGS = "derg"
+END_DEVICE_REGISTRATION = "rg"
+END_DEVICE_STATUS = "dstat"
+END_DEVICE_FSA = FSA
+END_DEVICE_POWER_STATUS = "ps"
+END_DEVICE_LOG_EVENT_LIST = "lel"
+END_DEVICE_INFORMATION = "di"
 
 DEFAULT_DCAP_ROOT = f"/{DCAP}"
 DEFAULT_EDEV_ROOT = f"/{EDEV}"
 DEFAULT_UPT_ROOT = f"/{UTP}"
 DEFAULT_MUP_ROOT = f"/{MUP}"
 DEFAULT_DRP_ROOT = f"/{DRP}"
 DEFAULT_SELF_ROOT = f"/{SDEV}"
 DEFAULT_MESSAGE_ROOT = f"/{MSG}"
 DEFAULT_DER_ROOT = f"/{DER}"
 DEFAULT_CURVE_ROOT = f"/{CURVE}"
 DEFAULT_RSPS_ROOT = f"/{RSPS}"
 DEFAULT_LOG_EVENT_ROOT = f"/{LOG}"
 DEFAULT_FSA_ROOT = f"/{FSA}"
-DEFAULT_DERP_ROOT = f"/{DERP}"
+DEFAULT_DERP_ROOT = f"/{DER_PROGRAM}"
 
 SEP = "_"
 MATCH_REG = "[a-zA-Z0-9_]*"
 
 # Used as a sentinal value when we only want the href of the root
 NO_INDEX = -1
 
 class DERSubType(Enum):
     Capability = "dercap"
-    Settings = "derg"
-    Status = "ders"
-    Availability = "dera"
-    CurrentProgram = "derp"
+    Settings = DER_SETTINGS
+    Status = DER_STATUS
+    Availability = DER_AVAILABILITY
+    CurrentProgram = DER_PROGRAM
+    None_Available = NO_INDEX
 
 class FSASubType(Enum):
     DERProgram = "derp"
     
 class DERProgramSubType(Enum):
     NoLink = 0
     ActiveDERControlListLink = 1
     DefaultDERControlLink = 2
     DERControlListLink = 3
     DERCurveListLink= 4
     DERControlReplyTo = 5
+    DERControl = 6
     
 class DERProgramHref(NamedTuple):
     root: str
     index: int
+    derp_subtype: DERProgramSubType = DERProgramSubType.NoLink
+    derp_subtype_index: int = NO_INDEX
+    
     
     @staticmethod
-    def parse(href: str):
+    def parse(href: str) -> DERProgramHref:
         parsed = href.split(SEP)
         if len(parsed) == 1:
             return DERProgramHref(parsed[0], NO_INDEX)
         elif len(parsed) == 2:
             return DERProgramHref(parsed[0], int(parsed[1]))
+        else:
+            mapped = dict(
+                derc=DERProgramSubType.DERControlListLink,
+                derca=DERProgramSubType.ActiveDERControlListLink,
+                dderc=DERProgramSubType.DefaultDERControlLink,
+            )
+            if len(parsed) == 4:
+                return DERProgramHref(parsed[0], int(parsed[1]), mapped[parsed[2]], int(parsed[3]))
+            return DERProgramHref(parsed[0], int(parsed[1]), mapped[parsed[2]])
     
 def der_program_parse(href: str) -> DERProgramHref:
     return DERProgramHref.parse(href)
     
 def der_program_href(index: int = NO_INDEX, sub: DERProgramSubType = DERProgramSubType.NoLink, subindex: int = NO_INDEX) -> str:
     if index == NO_INDEX:
         return DEFAULT_DERP_ROOT
     
     if sub == DERProgramSubType.NoLink:
         return SEP.join([DEFAULT_DERP_ROOT, str(index)])
     
     if sub == DERProgramSubType.ActiveDERControlListLink:
         if subindex == NO_INDEX:
-            return SEP.join([DEFAULT_DERP_ROOT, str(index), DERCA])
+            return SEP.join([DEFAULT_DERP_ROOT, str(index), DER_CONTROL_ACTIVE])
         else:
-            return SEP.join([DEFAULT_DERP_ROOT, str(index), DERCA, str(subindex)])
+            return SEP.join([DEFAULT_DERP_ROOT, str(index), DER_CONTROL_ACTIVE, str(subindex)])
     
     if sub == DERProgramSubType.DefaultDERControlLink:
         if subindex == NO_INDEX:
             return SEP.join([DEFAULT_DERP_ROOT, str(index), DDERC])
         else:
             return SEP.join([DEFAULT_DERP_ROOT, str(index), DDERC, str(subindex)])
 
@@ -134,54 +162,95 @@
         return SEP.join([DEFAULT_FSA_ROOT, str(index)])
     elif index == NO_INDEX and edev_index != NO_INDEX:
         return SEP.join([DEFAULT_EDEV_ROOT, str(edev_index), FSA])
     else:
         return SEP.join([DEFAULT_EDEV_ROOT, str(edev_index), FSA, str(index)])
 
 def derp_href(edev_index: int, fsa_index: int) -> str:
-    return SEP.join([DEFAULT_EDEV_ROOT, str(edev_index), FSA, str(fsa_index), DERP])
+    return SEP.join([DEFAULT_EDEV_ROOT, str(edev_index), FSA, str(fsa_index), DER_PROGRAM])
 
 def der_href(index: int = NO_INDEX, fsa_index: int = NO_INDEX, edev_index: int = NO_INDEX):
     if index == NO_INDEX and fsa_index == NO_INDEX and edev_index == NO_INDEX:
         return DEFAULT_DER_ROOT
     elif index != NO_INDEX and fsa_index == NO_INDEX and edev_index == NO_INDEX:
         return SEP.join([DEFAULT_DER_ROOT, str(index)])
     elif index == NO_INDEX and fsa_index != NO_INDEX and edev_index == NO_INDEX:
-        return SEP.join([DEFAULT_FSA_ROOT, str(fsa_index), DERP])
+        return SEP.join([DEFAULT_FSA_ROOT, str(fsa_index), DER_PROGRAM])
     elif edev_index != NO_INDEX and fsa_index == NO_INDEX and index == NO_INDEX:
         return SEP.join([DEFAULT_EDEV_ROOT, int(edev_index), FSA])
     elif edev_index != NO_INDEX and fsa_index != NO_INDEX and index == NO_INDEX:
         return SEP.join([DEFAULT_EDEV_ROOT, int(edev_index), FSA, int(fsa_index)])
     else:
         raise ValueError(f"index={index}, fsa_index={fsa_index}, edev_index={edev_index}")
     
 def edev_der_href(edev_index: int, der_index: int = NO_INDEX) -> str:
     if der_index == NO_INDEX:
         return SEP.join([DEFAULT_EDEV_ROOT, str(edev_index), DER])
     return SEP.join([DEFAULT_EDEV_ROOT, str(edev_index), DER, str(der_index)])
 
-class EdevHref(NamedTuple):
+
+class EDevSubType(Enum):
+    None_Available = NO_INDEX
+    Registration = END_DEVICE_REGISTRATION
+    DeviceStatus = END_DEVICE_STATUS
+    PowerStatus = END_DEVICE_POWER_STATUS
+    FunctionSetAssignments = END_DEVICE_FSA
+    LogEventList = END_DEVICE_LOG_EVENT_LIST
+    DeviceInformation = END_DEVICE_INFORMATION
+    DER = DER
+    
+
+
+@dataclass
+class EdevHref:
     edev_index: int
-    der_index: int = NO_INDEX
-    der_sub: DERSubType = None
+    edev_subtype: EDevSubType = EDevSubType.None_Available
+    edev_subtype_index: int = NO_INDEX
+    edev_der_subtype: DERSubType = DERSubType.None_Available
+    
+    def __str__(self) -> str:
+        value = "edev"
+        if self.edev_index != NO_INDEX:
+            value = f"{value}{SEP}{self.edev_index}"
+        
+        if self.edev_subtype != EDevSubType.None_Available:
+            value = f"{value}{SEP}{self.edev_subtype.value}"
+            
+        if self.edev_subtype_index != NO_INDEX:
+            value = f"{value}{SEP}{self.edev_subtype_index}"
+            
+        if self.edev_der_subtype != DERSubType.None_Available:
+            value = f"{value}{SEP}{self.edev_der_subtype.value}"
+        
+        return value
+           
     
-def edev_parse(path: str) -> EdevHref:
-    split_pth = path.split(SEP)
+    def parse(path: str) -> EdevHref:
+        split_pth = path.split(SEP)
+        
+        if split_pth[0] != EDEV:
+            raise ValueError(f"Must start with {EDEV}")
     
-    if len(split_pth) == 1:
-        return EdevHref(NO_INDEX)
-    elif len(split_pth) == 2:
-        return EdevHref(int(split_pth[1]))
-    elif len(split_pth) == 3:
-        return EdevHref(int(split_pth[1]))
-    elif len(split_pth) == 4:
-        return EdevHref(int(split_pth[1]), int(split_pth[3]))
-    elif len(split_pth) == 5:
-        return EdevHref(int(split_pth[1]), int(split_pth[3]), split_pth[4])
-
+        if len(split_pth) == 1:
+            return EdevHref(NO_INDEX)
+        elif len(split_pth) == 2:
+            return EdevHref(int(split_pth[1]))
+        elif len(split_pth) == 3:
+            return EdevHref(int(split_pth[1]), edev_subtype=EDevSubType(split_pth[2]))        
+        elif len(split_pth) == 4:
+            return EdevHref(int(split_pth[1]), edev_subtype=EDevSubType(split_pth[2]), edev_subtype_index=int(split_pth[3]))
+        elif len(split_pth) == 5:
+            return EdevHref(int(split_pth[1]), edev_subtype=EDevSubType(split_pth[2]), edev_subtype_index=int(split_pth[3]), edev_der_subtype=DERSubType(split_pth[4]))
+        else:
+            raise ValueError("Out of bounds parsing.")
+        
+    def __eq__(self, other: object) -> bool:
+        return other.edev_index == self.edev_index and other.edev_subtype == self.edev_subtype, \
+            other.edev_subtype_index == self.edev_subtype_index and other.edev_der_subtype == self.edev_der_subtype
+        
 class FSAHref(NamedTuple):
     fsa_index: NO_INDEX
     fsa_sub: FSASubType = None
     
 def fsa_parse(path: str) -> FSAHref:
     split_pth = path.split(SEP)
     
@@ -323,15 +392,15 @@
         ret = DEFAULT_DER_ROOT
     else:
         ret = SEP.join([DEFAULT_DER_ROOT, str(index)])
     return ret
 
 
 @lru_cache()
-def get_enddevice_href(edev_indx: int, subref: str = None) -> str:
+def get_enddevice_href(edev_indx: int = NO_INDEX, subref: str = None) -> str:
     if edev_indx == NO_INDEX:
         ret = DEFAULT_EDEV_ROOT
     elif subref:
         ret = SEP.join([DEFAULT_EDEV_ROOT, f"{edev_indx}", f"{subref}"])
     else:
         ret = SEP.join([DEFAULT_EDEV_ROOT, f"{edev_indx}"])
     return ret
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/__init__.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/constants.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/constants.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/derforecasts.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/derforecasts.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/enums.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/enums.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/models/sep.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/models/sep.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/persistance/points.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/persistance/points.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/__init__.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/admin_endpoints.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/admin_endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,17 +103,17 @@
             return Response(dataclass_to_xml(program))
             
             
         
         
     def _admin_derp(self, index: int = -1) -> Response:
         if request.method == 'GET' and index < 0:
-            return Response(dataclass_to_xml(DERProgramAdapter.fetch_list()))
+            return Response(dataclass_to_xml(DERProgramAdapter.fetch_all(m.DERProgramList())))
         elif request.method == 'GET':
-            return Response(dataclass_to_xml(DERProgramAdapter.fetch_edev_all()[index]))
+            return Response(dataclass_to_xml(DERProgramAdapter.fetch_at(index)))
         
         if request.method == 'POST':
             xml = request.data.decode('utf-8')
             data = xml_to_dataclass(request.data.decode('utf-8'))
             
             response = DERProgramAdapter.create(data)
             
@@ -123,26 +123,49 @@
         return Response(f"I am {index}, {request.method}")
 
     def _admin_derp_derca(self, derp_index: int) -> Response:
         ctrl_list = DERProgramAdapter.fetch_der_active_control_list(derp_index)
         return Response(dataclass_to_xml(ctrl_list))
         
     def _admin_derp_derc(self, derp_index: int) -> Response:
+        derp = DERProgramAdapter.fetch(derp_index)
+        
         if request.method == "POST":
             xml = request.data.decode('utf-8')
             data = xml_to_dataclass(request.data.decode('utf-8'))
             
             if isinstance(data, m.DefaultDERControl):
-                results = DERProgramAdapter.create_default_der_control(derp_index, data)
-                return Response(headers={'Location': results.href}, status=results.statusint)
+                status_code = 201
+                # data.href = hrefs.der_program_href(derp_index, hrefs.DERProgramSubType.DefaultDERControlLink)
+                if DERProgramAdapter.size_children(derp, hrefs.DDERC) > 0:
+                    status_code = 204
+                    DERProgramAdapter.remove_child(derp, hrefs.DDERC)
+                
+                DERProgramAdapter.add_child(derp, hrefs.DDERC, data)
+                
+                return Response(headers={'Location': data.href}, status=status_code)
             elif isinstance(data, m.DERControl):
-                results = DERProgramAdapter.create_der_control(derp_index, data)
-                return Response(headers={'Location': results.href}, status=results.statusint)
+                status_code = 201
+                # data.href = hrefs.der_program_href(derp_index, hrefs.DERProgramSubType.DERControlListLink)
+                try:
+                    index = DERProgramAdapter.fetch_child_index_by_mrid(derp, hrefs.DERC, data.mRID)
+                    DERProgramAdapter.replace_child(derp, hrefs.DERC, index, data)
+                    status_code = 204
+                except KeyError:
+                    DERProgramAdapter.add_child(derp, hrefs.DERC, data)
+                                        
+                return Response(headers={'Location': data.href}, status=status_code)
+        
+        if request.path.endswith("dderc"):
+            results = DERProgramAdapter.fetch_child(derp_index, "dderc")
+        elif request.path.endswith("derc"):
+            results = DERProgramAdapter.fetch_children(derp, "derc", m.DERControlList(href=request.path))
+        elif request.path.endswith("derca"):
+            results = DERProgramAdapter.fetch_children(derp, "derca", m.DERControlList(href=request.path))
             
-        results = DERProgramAdapter.fetch_der_control_list(derp_index)
         return Response(dataclass_to_xml(results))
         
 
     def _admin(self) -> Response:
         arg_path = request.args.get('path')
         device = request.args.get('device')
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/base_request.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/base_request.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/dcapfs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/dcapfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/enddevicesfs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/enddevicesfs.py`

 * *Files 24% similar despite different names*

```diff
@@ -93,24 +93,39 @@
 
         if not pth.startswith(hrefs.DEFAULT_EDEV_ROOT):
             raise ValueError(f"Invalid path for {self.__class__} {request.path}")
 
         pth_split = pth.split(hrefs.SEP)
         
         if len(pth_split) == 1:
-            retval = adpt.EndDeviceAdapter.fetch_list_by_lfdi(self.lfdi)
+            for ed in adpt.EndDeviceAdapter.fetch_all():
+                if ed.lFDI == self.lfdi:
+                    retval = m.EndDeviceList(EndDevice=[ed], all=1, results=1, href=pth)
+                    break
+                                
         elif len(pth_split) == 3:
-            if pth_split[2] == "rg":
-                retval = adpt.EndDeviceAdapter.fetch_registration(edev_index=int(pth_split[1]))
-            elif pth_split[2] == "di":
-                retval = "foo"
-            elif pth_split[2] == "fsa":
-                retval = adpt.EndDeviceAdapter.fetch_fsa_list(edev_index=int(pth_split[1]))
-            elif pth_split[2] == "der":
-                retval = adpt.DERAdapter.fetch_list(edev_index=int(pth_split[1]))
+            try:
+                ed = adpt.EndDeviceAdapter.fetch(int(pth_split[1]))
+                # FSA is a list off the end device, the rest are singleton items.
+                if pth_split[2] == hrefs.FSA:                   
+                    retval = adpt.EndDeviceAdapter.fetch_children(ed, hrefs.FSA, m.FunctionSetAssignmentsList(href=request.path))
+                elif pth_split[2] == hrefs.DER:
+                    retval = adpt.EndDeviceAdapter.fetch_children(ed, hrefs.DER, m.DERList(href=request.path))
+                else:
+                    retval = adpt.EndDeviceAdapter.fetch_child(ed, pth_split[2], 0)
+            except KeyError:
+                raise werkzeug.exceptions.NotFound("Missing Resource")
+            # if pth_split[2] == "rg":
+            #     retval = adpt.EndDeviceAdapter.fetch_registration(edev_index=int(pth_split[1]))
+            # elif pth_split[2] == "di":
+            #     retval = "foo"
+            # elif pth_split[2] == "fsa":
+            #     retval = adpt.EndDeviceAdapter.fetch_fsa_list(edev_index=int(pth_split[1]))
+            # elif pth_split[2] == "der":
+            #     retval = adpt.DERAdapter.fetch_list(edev_index=int(pth_split[1]))
             
         return self.build_response_from_dataclass(retval)
 
 
 class SDevRequests(RequestOp):
     """
     SelfDevice is an alias for the end device of a client.
@@ -131,21 +146,36 @@
         return self.build_response_from_dataclass(end_device)
 
 class FSARequests(RequestOp):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         
     def get(self):
-        pth_split = request.path.split(hrefs.SEP)
+        """ Retrieve a FSA or Program List
+        """
         
-        if len(pth_split) == 1:
-            retval = FSAAdapter.fetch_list()
-        elif len(pth_split) == 2:
-            retval = FSAAdapter.fetch_at(int(pth_split[1]))
-        elif len(pth_split) == 3:
-            retval = EndDeviceAdapter.fetch_fsa_list(edev_index=int(pth_split[1]))
-        elif len(pth_split) == 4:
-            retval = EndDeviceAdapter.fetch_fsa(edev_index=int(pth_split[1]), fsa_index=int(pth_split[3]))
+        fsa_href = hrefs.fsa_parse(request.path)
+        
+        if fsa_href.fsa_index == hrefs.NO_INDEX:
+            retval = FSAAdapter.fetch_all(m.FunctionSetAssignmentsList(), "FunctionSetAssignments")
+        elif fsa_href.fsa_sub == hrefs.FSASubType.DERProgram.value:
+            fsa = FSAAdapter.fetch(fsa_href.fsa_index)
+            retval = FSAAdapter.fetch_children(fsa, "fsa", m.DERProgramList())
+            # retval = FSAAdapter.fetch_children_list_container(fsa_href.fsa_index, m.DERProgram, m.DERProgramList(href="/derp"), "DERProgram")
         else:
-            raise ValueError(f"Path split is {pth_split}")
+            retval = FSAAdapter.fetch(fsa_href.fsa_index)
+            
+        # pth_split = request.path.split(hrefs.SEP)
+        
+        
+        # if len(pth_split) == 1:
+        #     retval = FSAAdapter.fetch_list()
+        # elif len(pth_split) == 2:
+        #     retval = FSAAdapter.fetch_at(int(pth_split[1]))
+        # elif len(pth_split) == 3:
+        #     retval = EndDeviceAdapter.fetch_fsa_list(edev_index=int(pth_split[1]))
+        # elif len(pth_split) == 4:
+        #     retval = EndDeviceAdapter.fetch_fsa(edev_index=int(pth_split[1]), fsa_index=int(pth_split[3]))
+        # else:
+        #     raise ValueError(f"Path split is {pth_split}")
             
         return self.build_response_from_dataclass(retval)
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/logfs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/logfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/meteringfs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/meteringfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/server_constructs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_constructs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/server_endpoints.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/server_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,29 +101,31 @@
         # app.add_url_rule(hrefs.derp, view_func=self._derp)
 
         # All the energy devices
         #app.add_url_rule(f"/{hrefs.EDEV}", methods=["GET", "POST", "PUT"], view_func=self._edev)
         app.add_url_rule(f"/<regex('{hrefs.EDEV}{hrefs.MATCH_REG}'):path>",
                          view_func=self._edev,
                          methods=["GET", "PUT", "POST"])
+        # This rule must be before der
+        app.add_url_rule(f"/<regex('{hrefs.DER_PROGRAM}{hrefs.MATCH_REG}'):path>",
+                         view_func=self._derp,
+                         methods=["GET"])
         app.add_url_rule(f"/<regex('{hrefs.DER}{hrefs.MATCH_REG}'):path>",
                          view_func=self._der,
                          methods=["GET", "PUT"])
         app.add_url_rule(f"/<regex('{hrefs.MUP}{hrefs.MATCH_REG}'):path>",
                          view_func=self._mup,
                          methods=["GET", "POST"])
         app.add_url_rule(f"/<regex('{hrefs.UTP}{hrefs.MATCH_REG}'):path>",
                          view_func=self._upt,
                          methods=["GET", "POST"])
         app.add_url_rule(f"/<regex('{hrefs.CURVE}{hrefs.MATCH_REG}'):path>",
                          view_func=self._curves,
                          methods=["GET"])
-        app.add_url_rule(f"/<regex('{hrefs.DERP}{hrefs.MATCH_REG}'):path>",
-                         view_func=self._derp,
-                         methods=["GET"])
+        
         app.add_url_rule(f"/<regex('{hrefs.FSA}{hrefs.MATCH_REG}'):path>",
                          view_func=self._fsa,
                          methods=["GET"])
         app.add_url_rule(f"/<regex('{hrefs.LOG}{hrefs.MATCH_REG}'):path>",
                          view_func=self._log,
                          methods=["GET", "POST"])
         # rulers = (
@@ -178,14 +180,18 @@
         return FSARequests(server_endpoints=self).execute()
 
     def _upt(self, path) -> Response:
         return UsagePointRequest(server_endpoints=self).execute()
 
     def _mup(self, path) -> Response:
         return MirrorUsagePointRequest(server_endpoints=self).execute()
+    
+    # Needs to be before der
+    def _derp(self, path) -> Response:
+        return DERProgramRequests(server_endpoints=self).execute()
 
     def _der(self, path) -> Response:
         _log.debug(request.method)
         return DERRequests(server_endpoints=self).execute()
 
     def _dcap(self) -> Response:
         return Dcap(server_endpoints=self).execute()
@@ -198,16 +204,14 @@
 
     def _sdev(self) -> Response:
         return SDevRequests(server_endpoints=self).execute()
 
     def _tm(self) -> Response:
         return TimeRequest(server_endpoints=self).execute()
 
-    def _derp(self, path) -> Response:
-        return DERProgramRequests(server_endpoints=self).execute()
 
     def _curves(self, path) -> Response:
         pth = request.environ['PATH_INFO']
         obj = get_href(pth)
         # if index is None:
         #     items = get_href_filtered(hrefs.curve)
         #     curve_list = DERCurveList(DERCurve=items, all=len(items), href=request.path, results=len(items))
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/timefs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/timefs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/usage_pointfs.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/usage_pointfs.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/server/uuid_handler.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/server/uuid_handler.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/service.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/service.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/simulation/gridappsd_pump.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/gridappsd_pump.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/simulation/inverter.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/simulation/inverter.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/types_/__init__.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/types_/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/utils/__init__.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import uuid
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Type, Optional
+from typing import Optional, Type
 
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.xml import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
@@ -64,7 +65,10 @@
         lfdi:
 
     Returns:
 
     """
     from ieee_2030_5.certs import sfdi_from_lfdi
     return sfdi_from_lfdi(lfdi)
+
+def uuid_2030_5() -> str:
+    return str(uuid.uuid4()).replace('-', '').upper()
```

### Comparing `gridappsd-2030_5-0.0.2a6/ieee_2030_5/utils/tls_wrapper.py` & `gridappsd-2030_5-0.0.2a7/ieee_2030_5/utils/tls_wrapper.py`

 * *Files identical despite different names*

### Comparing `gridappsd-2030_5-0.0.2a6/pyproject.toml` & `gridappsd-2030_5-0.0.2a7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-2030_5"
-version = "0.0.2a6"
+version = "0.0.2a7"
 description = ""
 authors = ["C. Allwardt <3979063+craig8@users.noreply.github.com>"]
 packages = [
     { include = "ieee_2030_5" }
 ]
 license = "BSD-3-Clause"
 maintainers = [
@@ -40,19 +40,21 @@
 nicegui = "^1.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 m2r2 = "^0.3.2"
 pytest = "^7.1.3"
 pycallgraph2 = "^1.1.3"
-
-[tool.poetry.dev-dependencies]
+pytest-describe = "^2.1.0"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 
+ [tool.pytest.ini_options]
+ addopts="-s"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.yapfignore]
 ignore_patterns = [
     ".venv/**",
```

### Comparing `gridappsd-2030_5-0.0.2a6/setup.py` & `gridappsd-2030_5-0.0.2a7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                      '2030_5_gridappsd = ieee_2030_5.config_setup:_main',
                      '2030_5_proxy = ieee_2030_5.basic_proxy:_main',
                      '2030_5_server = ieee_2030_5.__main__:_main',
                      '2030_5_shutdown = ieee_2030_5.__main__:_shutdown']}
 
 setup_kwargs = {
     'name': 'gridappsd-2030-5',
-    'version': '0.0.2a6',
+    'version': '0.0.2a7',
     'description': '',
     'long_description': '# GridAPPS-D IEEE 2030.5 Server\n\n## Overview\n\nThe GridAPPS-D IEEE 2030.5 Server implements the Common Smart Inverter Profile (CSIP).  The server\ncan work in both in-band and out-of-band registration models detailed in  CCIP Implementation Guide v2\nsection 6.1.3 and 6.1.4 respectively.  \n\n## Setup\n\n## Installing from pypi\n\nThe recommended way to install this project from pypi is in a virtual environment.  Create a virtual environment and install\n2030.5 server as follows.\n\n```shell\n# creates an environment \'env\' in the current directory\npython3 -m venv env\n\n# Activate the environment in the current shell\nsource env/bin/activate\n\n# Install 2030.5 server\npip install gridappsd_2030_5\n```\n\n## Configuration\n\nThe server requires two configuration files.  The first is for generation of certificates and keys for the system (openssl.cnf).  Currently\nwe shell out to openssl for key/cert/ca generation during runtime.  Each time the server is started up it will attempt to regenerate\nkey/certs/ca unless --no-create-certs is passed to the server startup method.  The second is the configuration for the server itself.  \nThe configuration file holds the definitions for controls, der, end devices and other settings that will be used during the runtime\nof the server.\n\nBoth of these configuration files should be placed in the current working directory where you will start the server.\n\n### Example openssl.cnf\n\n```ini\n#\n# OpenSSL example configuration file.\n# This is mostly being used for generation of certificate requests.\n#\n\n# This definition stops the following lines choking if HOME isn\'t\n# defined.\nHOME                    = .\nRANDFILE                = $ENV::HOME/.rnd\n\n# Extra OBJECT IDENTIFIER info:\n#oid_file               = $ENV::HOME/.oid\noid_section             = new_oids\n\n# To use this configuration file with the "-extfile" option of the\n# "openssl x509" utility, name here the section containing the\n# X.509v3 extensions to use:\n# extensions            =\n# (Alternatively, use a configuration file that has only\n# X.509v3 extensions in its main [= default] section.)\n\n[ new_oids ]\n\n# We can add new OIDs in here for use by \'ca\', \'req\' and \'ts\'.\n# Add a simple OID like this:\n# testoid1=1.2.3.4\n# Or use config file substitution like this:\n# testoid2=${testoid1}.5.6\n\n# Policies used by the TSA examples.\ntsa_policy1 = 1.2.3.4.1\ntsa_policy2 = 1.2.3.4.5.6\ntsa_policy3 = 1.2.3.4.5.7\n\n####################################################################\n[ ca ]\ndefault_ca      = CA_default            # The default ca section\n\n[ CA_default ]\ndir             = /home/gridappsd/tls             # Where everything is kept\ncerts           = $dir/certs            # Where the issued certs are kept\ndatabase        = $dir/index.txt        # database index file.\n                                        # several certs with same subject.\nnew_certs_dir   = $dir/certs            # default place for new certs.\ncertificate     = $dir/certs/ec-cacert.pem       # The CA certificate\nserial          = $dir/serial           # The current serial number\ncrlnumber       = $dir/crlnumber        # the current crl number\n                                        # must be commented out to leave a V1 CRL\nprivate_key     = $dir/private/ec-cakey.pem # The private key\n\nname_opt        = ca_default            # Subject Name options\ncert_opt        = ca_default            # Certificate field options\n\ndefault_days    = 365                   # how long to certify for\ndefault_crl_days= 30                    # how long before next CRL\ndefault_md      = sha256                # use SHA-256 by default\npreserve        = no                    # keep passed DN ordering\npolicy          = policy_match\n\n# For the CA policy\n[ policy_match ]\ncountryName             = optional\nstateOrProvinceName     = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = optional\nemailAddress            = optional\n\n[ policy_anything ]\ncountryName             = optional\nstateOrProvinceName     = optional\nlocalityName            = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = optional\nemailAddress            = optional\n\n####################################################################\n[ req ]\ndefault_bits            = 2048\ndefault_md              = sha256\ndefault_keyfile         = privkey.pem\n#distinguished_name      = req_distinguished_name\n#attributes              = req_attributes\nx509_extensions = v3_ca # The extentions to add to the self signed cert\n\n[ req_distinguished_name ]\n#countryName                     = Country Name (2 letter code)\n#countryName_default             = US\n#countryName_min                 = 2\n#countryName_max                 = 2\n#stateOrProvinceName             = State or Province Name (full name)\n#stateOrProvinceName_default     = Washington\n#localityName                    = Locality Name (eg, city)\n#localityName_default            = Richland\n#0.organizationName              = Organization Name (eg, company)\n#0.organizationName_default      =\n#organizationalUnitName          = Organizational Unit Name (eg, section)\n#commonName                      = Common Name (eg, your name or your server\\\'s hostname)\n#commonName_max                  = 64\n#emailAddress                    = Email Address\n#emailAddress_max                = 64\n\n[ req_attributes ]\nchallengePassword               = A challenge password\nchallengePassword_min           = 4\nchallengePassword_max           = 20\nunstructuredName                = An optional company name\n\n\n[ v3_req ]\n# Extensions to add to a certificate request\nbasicConstraints = CA:FALSE\nkeyUsage = nonRepudiation, digitalSignature, keyEncipherment\n\n[ v3_ca ]\n# Extensions for a typical CA\nsubjectKeyIdentifier=hash\nauthorityKeyIdentifier=keyid:always,issuer\nbasicConstraints = critical,CA:true\n\n[ crl_ext ]\n# issuerAltName=issuer:copy\nauthorityKeyIdentifier=keyid:always#\n# OpenSSL example configuration file.\n# This is mostly being used for generation of certificate requests.\n#\n\n# This definition stops the following lines choking if HOME isn\'t\n# defined.\nHOME                    = .\nRANDFILE                = $ENV::HOME/.rnd\n\n# Extra OBJECT IDENTIFIER info:\n#oid_file               = $ENV::HOME/.oid\noid_section             = new_oids\n\n# To use this configuration file with the "-extfile" option of the\n# "openssl x509" utility, name here the section containing the\n# X.509v3 extensions to use:\n# extensions            =\n# (Alternatively, use a configuration file that has only\n# X.509v3 extensions in its main [= default] section.)\n\n[ new_oids ]\n\n# We can add new OIDs in here for use by \'ca\', \'req\' and \'ts\'.\n# Add a simple OID like this:\n# testoid1=1.2.3.4\n# Or use config file substitution like this:\n# testoid2=${testoid1}.5.6\n\n# Policies used by the TSA examples.\ntsa_policy1 = 1.2.3.4.1\ntsa_policy2 = 1.2.3.4.5.6\ntsa_policy3 = 1.2.3.4.5.7\n\n####################################################################\n[ ca ]\ndefault_ca      = CA_default            # The default ca section\n\n[ CA_default ]\ndir             = /home/gridappsd/tls   # Where everything is kept\ncerts           = $dir/certs            # Where the issued certs are kept\ndatabase        = $dir/index.txt        # database index file.\n                                        # several certs with same subject.\nnew_certs_dir   = $dir/certs            # default place for new certs.\ncertificate     = $dir/certs/ec-cacert.pem       # The CA certificate\nserial          = $dir/serial           # The current serial number\ncrlnumber       = $dir/crlnumber        # the current crl number\n                                        # must be commented out to leave a V1 CRL\nprivate_key     = $dir/private/ec-cakey.pem # The private key\n\nname_opt        = ca_default            # Subject Name options\ncert_opt        = ca_default            # Certificate field options\n\ndefault_days    = 365                   # how long to certify for\ndefault_crl_days= 30                    # how long before next CRL\ndefault_md      = sha256                # use SHA-256 by default\npreserve        = no                    # keep passed DN ordering\npolicy          = policy_match\n\n# For the CA policy\n[ policy_match ]\ncountryName             = optional\nstateOrProvinceName     = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = supplied\nemailAddress            = optional\n\n[ policy_anything ]\ncountryName             = optional\nstateOrProvinceName     = optional\nlocalityName            = optional\norganizationName        = optional\norganizationalUnitName  = optional\ncommonName              = supplied\nemailAddress            = optional\n\n####################################################################\n[ req ]\ndefault_bits            = 2048\ndefault_md              = sha256\ndefault_keyfile         = privkey.pem\ndistinguished_name      = req_distinguished_name\nattributes              = req_attributes\nx509_extensions = v3_ca # The extentions to add to the self signed cert\n\n[ req_distinguished_name ]\ncountryName                     = Country Name (2 letter code)\ncountryName_default             = IN\ncountryName_min                 = 2\ncountryName_max                 = 2\nstateOrProvinceName             = State or Province Name (full name)\nstateOrProvinceName_default     = Some-State\nlocalityName                    = Locality Name (eg, city)\nlocalityName_default            = BANGALORE\n0.organizationName              = Organization Name (eg, company)\n0.organizationName_default      = GoLinuxCloud\norganizationalUnitName          = Organizational Unit Name (eg, section)\ncommonName                      = Common Name (eg, your name or your server\\\'s hostname)\ncommonName_max                  = 64\nemailAddress                    = Email Address\nemailAddress_max                = 64\n\n[ req_attributes ]\nchallengePassword               = A challenge password\nchallengePassword_min           = 4\nchallengePassword_max           = 20\nunstructuredName                = An optional company name\n\n\n[ v3_req ]\n# Extensions to add to a certificate request\nbasicConstraints = CA:FALSE\nkeyUsage = nonRepudiation, digitalSignature, keyEncipherment\n\n[ v3_ca ]\n# Extensions for a typical CA\nsubjectKeyIdentifier=hash\nauthorityKeyIdentifier=keyid:always,issuer\nbasicConstraints = critical,CA:true\n\n[ crl_ext ]\n# issuerAltName=issuer:copy\nauthorityKeyIdentifier=keyid:always\n```\n\n```yaml\n\n### Example config.yml\n---\n#server_hostname: 0.0.0.0:8443\n\nserver: 127.0.0.1\n# Only include if we need to have dcap be available\n# http_port: 8080\nhttps_port: 7443\n\nproxy_hostname: 0.0.0.0:8443\n#server_hostname: 0.0.0.0:7443\n# server_hostname: gridappsd_dev_2004:7443\n\ntls_repository: "./tls"\nopenssl_cnf: "openssl.cnf"\n\n#server_mode: enddevices_register_access_only\nserver_mode: enddevices_create_on_start\n\n# lfdi_mode: Determines what piece of information is used to calculate the lfdi\n#\n# Options:\n#   lfdi_mode_from_file             - sha256 hash of certificate file\'s content.\n#   lfdi_mode_from_cert_fingerprint - sha256 hash of the certificates fingerprint.\n#\n# default: lfdi_mode_from_cert_fingerprint\n#lfdi_mode: lfdi_mode_from_file\nlfdi_mode: lfdi_mode_from_cert_fingerprint\n\n# Create an administrator certificate that can be used from\n# browser/api to connect to the platform.\ngenerate_admin_cert: True\n\nlog_event_list_poll_rate: 60\ndevice_capability_poll_rate: 60\n\n# End Device\ndevices:\n  # SolarEdge SE6000H HD-Wave SetApp Enabled Inverter\n  - id: dev1\n    # DeviceCategoryType from ieee_2030_5.models.device_category\n    deviceCategory: FUEL_CELL\n    pin: 111115\n\n    programs:\n      - description: Program 1\n\n    # nameplate:\n    #   rtgMaxW: 6000\n    ders:\n      - capabilities:\n        modesSupported: "1110000000000000"\n        type: 83\n\n      - capabilities:\n        # Bitmask with the following structure.\n        # Indication of support for each control mode function DERCapability::modesSupported\n        #\n        # 0 - Charge mode\n        # 1 - Discharge mode\n        # 2 - opModConnect (Connect / Disconnect -\n        # implies galvanic isolation)\n        # 3 - opModEnergize (Energize / De-Energize)\n        # 4 - opModFixedPFAbsorbW (Fixed Power\n        # Factor Setpoint when absorbing active\n        # power)\n        # 5 - opModFixedPFInjectW (Fixed Power\n        # Factor Setpoint when injecting active\n        # power)\n        # 6 - opModFixedVar (Reactive Power\n        # Setpoint)\n        # 7 - opModFixedW (Charge / Discharge\n        # Setpoint)\n        # 8 - opModFreqDroop (Frequency-Watt\n        # Parameterized Mode)\n        # 9 - opModFreqWatt (Frequency-Watt\n        # Curve Mode)\n        # 10 - opModHFRTMayTrip (High Frequency\n        # Ride Through, May Trip Mode)\n        # 11 - opModHFRTMustTrip (High\n        # Frequency Ride Through, Must Trip Mode)\n        # 12 - opModHVRTMayTrip (High Voltage\n        # Ride Through, May Trip Mode)\n        # 13 - opModHVRTMomentaryCessation\n        # (High Voltage Ride Through, Momentary\n        # Cessation Mode)\n        # 14 - opModHVRTMustTrip (High Voltage\n        # Ride Through, Must Trip Mode)\n        # 15 - opModLFRTMayTrip (Low Frequency\n        # Ride Throu\n        modesSupported: "1110000000000000"\n\n        # Item type for the DER.\n        # 0 - Not applicable / Unknown\n        # 1 - Virtual or mixed DER\n        # 2 - Reciprocating engine\n        # 3 - Fuel cell\n        # 4 - Photovoltaic system\n        # 5 - Combined heat and power\n        # 6 - Other generation system\n        # 80 - Other storage system\n        # 81 - Electric vehicle\n        # 82 - EVSE\n        # 83 - Combined PV and storage\n        type: 83\n\n        # Default available nameplate options where at a manufacturer\'s set.\n        # Active power rating in watts an unity power factor\n        rtgMaxW: 600\n\n        # Active power rating in watts at specified over-excited power factor\n        # rtgOverExcitedW:\n\n        # Over-excited power factor DERCapability::rtgOverExcitedPF\n        # rtgOverExcitedPF:\n\n        # Active power rating in watts at specified under-excited power factor DERCapability::rtgUnderExcitedW\n        # rtgUnderExcitedW:\n\n        # Under-excited power factor DERCapability::rtgUnderExcitedPF\n        # rtgUnderExcitedPF:\n\n        # Maximum apparent power rating in voltamperes DERCapability::rtgMaxVA\n        rtgMaxVA: 600\n\n        # Indication of reactive power and voltage/power control capability DERCapability::rtgNormalCategory\n        rtgNormalCategory: 1\n\n        # Indication of voltage and frequencyride-through capability category I, II, or III DERCapability::rtgAbnormalCategory\n        rtgAbnormalCategory: 1\n\n        # Maximum injected reactive power rating in vars DERCapability::rtgMaxVar\n        rtgMaxVar: 600\n\n        # Maximum absorbed reactive power rating in vars DERCapability::rtgMaxVarNeg\n        rtgMaxVarNeg: 600\n\n        # Maximum active power charge rating in watts DERCapability::rtgMaxChargeRateW\n        rtgMaxChargeRateW: 600\n\n        # Maximum apparent power charge rating in voltamperes; may differ from the apparent power maximum rating\n        # DERCapability::rtgMaxChargeRateVA\n        rtgMaxChargeRateVA: 600\n\n        # Nominal ac voltage rating in rms volts DERCapability::rtgVNom\n        rtgVNom: 120\n\n        # Maximum ac voltage rating in rms volts DERCapability::rtgMaxV\n        rtgMaxV: 128\n\n        # Minimum ac voltage rating in rms volts DERCapability::rtgMinV\n        rtgMinV: 116\n\n        # Reactive susceptance that remains connected to the Area EPS in the cease to energize and trip state\n        # DERCapability::rtgReactiveSusceptance\n        # rtgReactiveSusceptance:\n\n        # # Manufacturer DeviceInformation::mfID\n        # mfID:\n\n        # # Model DeviceInformation::mfModel\n        # mfModel:\n\n        # # Serial number DeviceInformation::mfSerNum\n        # mfSerNum:\n\n        # # Version DeviceInformation::mfHwVer DeviceInformation::swVer\n        # mfHwVer:\n        # swVer:\n\n  - id: dev2\n    deviceCategory: FUEL_CELL\n    pin: 12345\n    nameplate:\n\nprograms:\n  - description: Program 1\n    default_control: Control 1\n    controls:\n      - Control 2\n      - Control 3\n    curves:\n      - Curve 1\n    primacy: 89\n\ncontrols:\n  - description: Control 1\n    setESDelay: 30\n    base:\n      opModConnect: True\n      opModMaxLimW: 9500\n\n      # setESHighFreq: UInt16 [0..1]\n      # setESHighVolt: Int16 [0..1]\n      # setESLowFreq: UInt16 [0..1]\n      # setESLowVolt: Int16 [0..1]\n      # setESRampTms: UInt32 [0..1]\n      # setESRandomDelay: UInt32 [0..1]\n      # setGradW: UInt16 [0..1]\n      # setSoftGradW: UInt16 [0..1]\n  - description: Control 2\n  - description: Control 3\n\nevents:\n  - control: 0\n\ncurves:\n  # Each element will can have the following structure.\n  # autonomousVRefEnable: If the curveType is opModVoltVar, then\n  #   this field MAY be present. If the curveType is not opModVoltVar,\n  #   then this field SHALL NOT be present. Enable/disable autonomous\n  #   vRef adjustment. When enabled, the Volt-Var curve characteristic\n  #   SHALL be adjusted autonomously as vRef changes and\n  #   autonomousVRefTimeConstant SHALL be present. If a DER is able to\n  #   support Volt-Var mode but is unable to support autonomous vRef\n  #   adjustment, then the DER SHALL execute the curve without\n  #   autonomous vRef adjustment. If not specified, then the value is\n  #   false.\n  # autonomousVRefTimeConstant: If the curveType is opModVoltVar,\n  #   then this field MAY be present. If the curveType is not\n  #   opModVoltVar, then this field SHALL NOT be present. Adjustment\n  #   range for vRef time constant, in hundredths of a second.\n  # creationTime: The time at which the object was created.\n  # CurveData:\n  # curveType: Specifies the associated curve-based control mode.\n  # openLoopTms: Open loop response time, the time to ramp up to\n  #   90% of the new target in response to the change in voltage, in\n  #   hundredths of a second. Resolution is 1/100 sec. A value of 0 is\n  #   used to mean no limit. When not present, the device SHOULD\n  #   follow its default behavior.\n  # rampDecTms: Decreasing ramp rate, interpreted as a percentage\n  #   change in output capability limit per second (e.g. %setMaxW /\n  #   sec).  Resolution is in hundredths of a percent/second. A value\n  #   of 0 means there is no limit. If absent, ramp rate defaults to\n  #   setGradW.\n  # rampIncTms: Increasing ramp rate, interpreted as a percentage\n  #   change in output capability limit per second (e.g. %setMaxW /\n  #   sec).  Resolution is in hundredths of a percent/second. A value\n  #   of 0 means there is no limit. If absent, ramp rate defaults to\n  #   rampDecTms.\n  # rampPT1Tms: The configuration parameter for a low-pass filter,\n  #   PT1 is a time, in hundredths of a second, in which the filter\n  #   will settle to 95% of a step change in the input value.\n  #   Resolution is 1/100 sec.\n  # vRef: If the curveType is opModVoltVar, then this field MAY be\n  #   present. If the curveType is not opModVoltVar, then this field\n  #   SHALL NOT be present. The nominal AC voltage (RMS) adjustment to\n  #   the voltage curve points for Volt-Var curves.\n  # xMultiplier: Exponent for X-axis value.\n  # yMultiplier: Exponent for Y-axis value.\n  # yRefType: The Y-axis units context.\n  # Each curve MUST have between 1 and 10 elements in the curve_data list.\n  #\n  # DERCurve Type for each curve.\n  # 0 - opModFreqWatt (Frequency-Watt Curve Mode)\n  # 1 - opModHFRTMayTrip (High Frequency Ride Through, May Trip Mode)\n  # 2 - opModHFRTMustTrip (High Frequency Ride Through, Must Trip Mode)\n  # 3 - opModHVRTMayTrip (High Voltage Ride Through, May Trip Mode)\n  # 4 - opModHVRTMomentaryCessation (High Voltage Ride Through, Momentary Cessation\n  # Mode)\n  # 5 - opModHVRTMustTrip (High Voltage Ride Through, Must Trip Mode)\n  # 6 - opModLFRTMayTrip (Low Frequency Ride Through, May Trip Mode)\n  # 7 - opModLFRTMustTrip (Low Frequency Ride Through, Must Trip Mode)\n  # 8 - opModLVRTMayTrip (Low Voltage Ride Through, May Trip Mode)\n  # 9 - opModLVRTMomentaryCessation (Low Voltage Ride Through, Momentary Cessation\n  # Mode)\n  # 10 - opModLVRTMustTrip (Low Voltage Ride Through, Must Trip Mode)\n  # 11 - opModVoltVar (Volt-Var Mode)\n  # 12 - opModVoltWatt (Volt-Watt Mode)\n  # 13 - opModWattPF (Watt-PowerFactor Mode)\n  # 14 - opModWattVar (Watt-Var Mode)\n  - description: Curve 1\n    curveType: opModVoltVar\n    CurveData:\n      - xvalue: 5\n        yvalue: 5\n\n  - description: Curve 2\n    curveType: opModFreqWatt\n    CurveData:\n      # exitation is only available if yvalue is power factor\n      - exitation: 10\n        xvalue: 5\n        yvalue: 5\n```\n\n## Installing from source\n\nThe installation requires poetry version 1.2 or greater.  <https://python-poetry.org/docs/#installation>\n\n 1. Clone the repository\n 2. run `poetry install` from the root of the repository directory.\n\n### Clone the repository\n\n```shell\ngit clone https://github.com/GRIDAPPSD/gridappsd-2030_5 -b develop\ncd gridappsd-2030_5\n```\n\n### Install Requirements\n\n```shell\npoetry install\n```\n\n### Run the Server\n\n```shell\nusage: 2030_5_server [-h] [--no-validate] [--no-create-certs] [--debug] config\n\npositional arguments:\n  config             Configuration file for the server.\n\noptional arguments:\n  -h, --help         show this help message and exit\n  --no-validate      Allows faster startup since the resolving of addresses for devices is not done.\n  --no-create-certs  If specified certificates for for client and server will not be created.\n  --debug            Put server in debug mode (more logging)\n```\n\n### Using the 2030.5 proxy\n\nThe proxy is used to keep a http 1.1 connection alive rather than doing the tls setup\nmore than one time.\n\n```shell\nusage: 2030_5_proxy [-h] [--debug] config\n\npositional arguments:\n  config      Configuration file for the server.\n\noptional arguments:\n  -h, --help  show this help message and exit\n  --debug     Turns debugging on for logging of the proxy.\n```\n\n## Client Connectivity\n\nThe server will expose an endpoint of beginning with <https://myserver/dcap>.  From there\na client will be able to traverse and do any PUT, POST, GET, and DELETE operations specified\nin the 2030.5 test procedures.\n\n## Function Sets Implemented\n',
     'author': 'C. Allwardt',
     'author_email': '3979063+craig8@users.noreply.github.com',
     'maintainer': 'C. Allwardt',
     'maintainer_email': '3979063+craig8@users.noreply.github.com',
     'url': 'https://github.com/GRIDAPPSD/gridappsd-2030_5',
```

### Comparing `gridappsd-2030_5-0.0.2a6/PKG-INFO` & `gridappsd-2030_5-0.0.2a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridappsd-2030-5
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: 
 Home-page: https://github.com/GRIDAPPSD/gridappsd-2030_5
 License: BSD-3-Clause
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Maintainer: C. Allwardt
 Maintainer-email: 3979063+craig8@users.noreply.github.com
```

