# Comparing `tmp/python-matter-server-3.2.0.tar.gz` & `tmp/python-matter-server-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.2.0.tar", last modified: Wed Mar 29 13:42:06 2023, max compression
+gzip compressed data, was "python-matter-server-3.3.0.tar", last modified: Mon Apr 17 15:06:08 2023, max compression
```

## Comparing `python-matter-server-3.2.0.tar` & `python-matter-server-3.3.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.835660 python-matter-server-3.2.0/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-29 13:41:55.000000 python-matter-server-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-03-29 13:42:06.000000 python-matter-server-3.2.0/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-29 13:42:06.000000 python-matter-server-3.2.0/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:42:06.000000 python-matter-server-3.2.0/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-29 13:42:06.000000 python-matter-server-3.2.0/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:42:04.000000 python-matter-server-3.2.0/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-29 13:42:06.000000 python-matter-server-3.2.0/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 13:42:06.000000 python-matter-server-3.2.0/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-29 13:42:06.839661 python-matter-server-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.416754 python-matter-server-3.3.0/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-17 15:06:07.000000 python-matter-server-3.3.0/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:06:07.000000 python-matter-server-3.3.0/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:06:06.000000 python-matter-server-3.3.0/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/setup.cfg
```

### Comparing `python-matter-server-3.2.0/LICENSE` & `python-matter-server-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/PKG-INFO` & `python-matter-server-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.2.0/README.md` & `python-matter-server-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/client/client.py` & `python-matter-server-3.3.0/matter_server/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import asyncio
 import logging
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Callable, Dict, Final, Optional, cast
 import uuid
 
 from aiohttp import ClientSession
+from chip.clusters import Objects as Clusters
 
 from matter_server.common.errors import ERROR_MAP
 
 from ..common.helpers.util import dataclass_from_dict, dataclass_to_dict
 from ..common.models import (
     APICommand,
     CommandMessage,
@@ -23,15 +24,15 @@
     ResultMessageBase,
     ServerDiagnostics,
     ServerInfoMessage,
     SuccessResultMessage,
 )
 from .connection import MatterClientConnection
 from .exceptions import ConnectionClosed, InvalidServerVersion, InvalidState
-from .models.node import MatterNode
+from .models.node import MatterFabricData, MatterNode
 
 if TYPE_CHECKING:
     from chip.clusters.Objects import ClusterCommand
 
 SUB_WILDCARD: Final = "*"
 
 
@@ -152,14 +153,55 @@
                 timeout=timeout,
                 iteration=iteration,
                 option=option,
                 discriminator=discriminator,
             ),
         )
 
+    async def get_matter_fabrics(self, node_id: int) -> list[MatterFabricData]:
+        """
+        Get Matter fabrics from a device.
+
+        Returns a list of MatterFabricData objects.
+        """
+
+        node = await self.get_node(node_id)
+        fabrics: list[
+            Clusters.OperationalCredentials.Structs.FabricDescriptor
+        ] = node.get_attribute_value(
+            0, None, Clusters.OperationalCredentials.Attributes.Fabrics
+        )
+
+        vendors_map = await self.send_command(
+            APICommand.GET_VENDOR_NAMES,
+            require_schema=3,
+            filter_vendors=[f.vendorId for f in fabrics],
+        )
+
+        return [
+            MatterFabricData(
+                fabric_id=f.fabricId,
+                vendor_id=f.vendorId,
+                fabric_index=f.fabricIndex,
+                fabric_label=f.label if f.label else None,
+                vendor_name=vendors_map.get(f.vendorId),
+            )
+            for f in fabrics
+        ]
+
+    async def remove_matter_fabric(self, node_id: int, fabric_index: int) -> None:
+        """Remove Matter fabric from a device."""
+        await self.send_device_command(
+            node_id,
+            0,
+            Clusters.OperationalCredentials.Commands.RemoveFabric(
+                fabricIndex=fabric_index,
+            ),
+        )
+
     async def send_device_command(
         self,
         node_id: int,
         endpoint_id: int,
         command: ClusterCommand,
         response_type: Any | None = None,
         timed_request_timeout_ms: int | None = None,
```

### Comparing `python-matter-server-3.2.0/matter_server/client/connection.py` & `python-matter-server-3.3.0/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/client/exceptions.py` & `python-matter-server-3.3.0/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/client/models/device_types.py` & `python-matter-server-3.3.0/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/client/models/node.py` & `python-matter-server-3.3.0/matter_server/client/models/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Matter node."""
 from __future__ import annotations
 
+from dataclasses import dataclass
 import logging
 from typing import Any, TypeVar, cast
 
 from chip.clusters import Objects as Clusters
 from chip.clusters.ClusterObjects import ALL_ATTRIBUTES, ALL_CLUSTERS
 
 from matter_server.common.helpers.util import (
@@ -36,14 +37,25 @@
     """Parse label/key and type for an object from the descriptors, given the raw object id."""
     for desc in descriptor.Fields:
         if desc.Tag == object_id:
             return (desc.Label, desc.Type)
     raise KeyError(f"No descriptor found for object {object_id}")
 
 
+@dataclass
+class MatterFabricData:
+    """Data about a Matter fabric."""
+
+    fabric_id: int
+    vendor_id: int
+    fabric_index: int
+    fabric_label: str | None = None
+    vendor_name: str | None = None
+
+
 class MatterEndpoint:
     """Representation of a Matter Endpoint."""
 
     def __init__(
         self,
         endpoint_id: int,
         attributes_data: dict[str, Any],
```

### Comparing `python-matter-server-3.2.0/matter_server/common/errors.py` & `python-matter-server-3.3.0/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/common/helpers/api.py` & `python-matter-server-3.3.0/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/common/helpers/json.py` & `python-matter-server-3.3.0/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/common/helpers/util.py` & `python-matter-server-3.3.0/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/common/models.py` & `python-matter-server-3.3.0/matter_server/common/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,22 +33,35 @@
     SET_WIFI_CREDENTIALS = "set_wifi_credentials"
     SET_THREAD_DATASET = "set_thread_dataset"
     OPEN_COMMISSIONING_WINDOW = "open_commissioning_window"
     DISCOVER = "discover"
     INTERVIEW_NODE = "interview_node"
     DEVICE_COMMAND = "device_command"
     REMOVE_NODE = "remove_node"
+    GET_VENDOR_NAMES = "get_vendor_names"
 
 
 EventCallBackType = Callable[[EventType, Any], None]
 
 # Generic model(s)
 
 
 @dataclass
+class VendorInfo:
+    """Vendor info as received from the CSA."""
+
+    vendor_id: int
+    vendor_name: str
+    company_legal_name: str
+    company_preferred_name: str
+    vendor_landing_page_url: str
+    creator: str
+
+
+@dataclass
 class MatterNodeData:
     """Matter node data as received from (and stored on) the server."""
 
     node_id: int
     date_commissioned: datetime
     last_interview: datetime
     interview_version: int
```

### Comparing `python-matter-server-3.2.0/matter_server/server/__main__.py` & `python-matter-server-3.3.0/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/server/client_handler.py` & `python-matter-server-3.3.0/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/server/const.py` & `python-matter-server-3.3.0/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/server/device_controller.py` & `python-matter-server-3.3.0/matter_server/server/device_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from __future__ import annotations
 
 import asyncio
 from collections import deque
 from datetime import datetime
 from functools import partial
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Deque, Type, TypeVar, cast
+import time
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, Deque, Type, TypeVar, cast
 
 from chip.ChipDeviceCtrl import CommissionableNode
 from chip.clusters import Attribute, Objects as Clusters
 from chip.clusters.ClusterObjects import ALL_CLUSTERS, Cluster
 from chip.exceptions import ChipStackError
 
 from ..common.const import SCHEMA_VERSION
@@ -38,14 +39,15 @@
 
 _T = TypeVar("_T")
 
 DATA_KEY_NODES = "nodes"
 DATA_KEY_LAST_NODE_ID = "last_node_id"
 
 LOGGER = logging.getLogger(__name__)
+INTERVIEW_TASK_LIMIT = 10
 
 
 class MatterDeviceController:
     """Class that manages the Matter devices."""
 
     chip_controller: ChipDeviceController | None
 
@@ -372,24 +374,24 @@
 
         attribute_path = create_attribute_path_from_attribute(
             0,
             Clusters.OperationalCredentials.Attributes.CurrentFabricIndex,
         )
         fabric_index = node.attributes[attribute_path]
 
+        self.server.signal_event(EventType.NODE_DELETED, node_id)
+
         await self.chip_controller.SendCommand(
             nodeid=node_id,
             endpoint=0,
             payload=Clusters.OperationalCredentials.Commands.RemoveFabric(
                 fabricIndex=fabric_index,
             ),
         )
 
-        self.server.signal_event(EventType.NODE_DELETED, node_id)
-
     async def subscribe_node(self, node_id: int) -> None:
         """
         Subscribe to all node state changes/events for an individual node.
 
         Note that by using the listen command at server level, you will receive all node events.
         """
         if self.chip_controller is None:
@@ -523,56 +525,94 @@
                 None,
                 partial(func, *args, **kwargs),
             ),
         )
 
     async def _check_subscriptions_and_interviews(self) -> None:
         """Run subscriptions (and interviews) for known nodes."""
+        # Set default resubscribe interval to 1 hour
+        reschedule_interval = 3600
+        start_time = time.time()
+        tasks: list[Coroutine[Any, Any, None]] = []
+        task_limit: asyncio.Semaphore = asyncio.Semaphore(INTERVIEW_TASK_LIMIT)
+
         for node_id, node in self._nodes.items():
             # (re)interview node (only) if needed
             if (
                 node is None
                 or node.interview_version < SCHEMA_VERSION
                 or (datetime.utcnow() - node.last_interview).days > 30
             ):
+
+                async def _interview_node(node_id: int) -> None:
+                    """Run interview for node."""
+                    try:
+                        await self.interview_node(node_id)
+                    except NodeInterviewFailed as err:
+                        LOGGER.warning(
+                            "Unable to interview Node %s, we will retry later in the background.",
+                            node_id,
+                            exc_info=err,
+                        )
+                        raise err
+
+                tasks.append(_interview_node(node_id))
+                continue
+
+            # setup subscriptions for the node
+            if node_id in self._subscriptions:
+                continue
+
+            async def _subscribe_node(node_id: int) -> None:
+                """Subscribe to node events."""
                 try:
-                    await self.interview_node(node_id)
-                except NodeInterviewFailed as err:
+                    await self.subscribe_node(node_id)
+                except NodeNotResolving as err:
                     LOGGER.warning(
-                        "Unable to interview Node %s, we will retry later in the background.",
+                        "Unable to subscribe to Node %s, "
+                        "we will retry later in the background.",
                         node_id,
                         exc_info=err,
                     )
-                    continue
+                    raise err
 
-            # setup subscriptions for the node
-            if node_id in self._subscriptions:
-                continue
-            try:
-                await self.subscribe_node(node_id)
-            except NodeNotResolving as err:
-                # If the node is unreachable on the network now,
-                # it will throw a NodeNotResolving exception, catch this,
-                # log this and just try to resolve this node in the next run.
-                LOGGER.warning(
-                    "Unable to contact Node %s,"
-                    " we will retry later in the background.",
-                    node_id,
-                    exc_info=err,
-                )
+            tasks.append(_subscribe_node(node_id))
+
+        async def _run_task(task: Coroutine[Any, Any, None]) -> None:
+            """Run coroutine and release semaphore."""
+            async with task_limit:
+                await task
+
+        LOGGER.debug("Running %s tasks", len(tasks))
+        # wait for all tasks to finish
+        results: list[Exception | None] = await asyncio.gather(
+            *(_run_task(task) for task in tasks), return_exceptions=True
+        )
+        LOGGER.debug(
+            "Done running %s tasks in %s seconds",
+            len(results),
+            start_time - time.time(),
+        )
+        # check if any of the tasks failed
+        for result in results:
+            if isinstance(result, Exception):
+                # if any of the tasks failed, reschedule in 5 minutes
+                reschedule_interval = 300
+                break
 
         # reschedule self to run every hour
         def _schedule() -> None:
             """Schedule task."""
             self._interview_task = asyncio.create_task(
                 self._check_subscriptions_and_interviews()
             )
 
+        LOGGER.debug("Rescheduling interviews in %s seconds", reschedule_interval)
         loop = cast(asyncio.AbstractEventLoop, self.server.loop)
-        loop.call_later(3600, _schedule)
+        loop.call_later(reschedule_interval, _schedule)
 
     @staticmethod
     def _parse_attributes_from_read_result(
         read_result: dict[int, dict[Type, dict[Type, Any]]]
     ) -> dict[str, Any]:
         """Parse attributes from ReadResult."""
         result = {}
```

### Comparing `python-matter-server-3.2.0/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.3.0/matter_server/server/helpers/paa_certificates.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 from cryptography.hazmat.primitives import serialization
 
 from matter_server.server.const import PAA_ROOT_CERTS_DIR
 
 LOGGER = logging.getLogger(__name__)
 PRODUCTION_URL = "https://on.dcl.csa-iot.org"
 TEST_URL = "https://on.test-net.dcl.csa-iot.org"
-
+GIT_URL = "https://github.com/project-chip/connectedhomeip/raw/master/credentials/development/paa-root-certs"  # pylint: disable=line-too-long
+GIT_CERTS = [
+    "Chip-Test-PAA-FFF1-Cert",
+    "Chip-Test-PAA-NoVID-Cert",
+]
 LAST_CERT_IDS: set[str] = set()
 
 
 async def write_paa_root_cert(certificate: str, subject: str) -> None:
     """Write certificate from string to file."""
 
     def _write() -> None:
@@ -45,19 +49,19 @@
         with open(file_path_der, "wb+") as outfile:
             der_certificate = pem_certificate.public_bytes(serialization.Encoding.DER)
             outfile.write(der_certificate)
 
     return await asyncio.get_running_loop().run_in_executor(None, _write)
 
 
-async def fetch_certificates(
+async def fetch_dcl_certificates(
     fetch_test_certificates: bool = True,
     fetch_production_certificates: bool = True,
 ) -> int:
-    """Fetch PAA Certificates."""
+    """Fetch DCL PAA Certificates."""
     LOGGER.info("Fetching the latest PAA root certificates from DCL.")
     if not PAA_ROOT_CERTS_DIR.is_dir():
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, makedirs, PAA_ROOT_CERTS_DIR)
     fetch_count: int = 0
     base_urls = set()
     # determine which url's need to be queried.
@@ -101,8 +105,51 @@
                     fetch_count += 1
     except ClientError as err:
         LOGGER.warning(
             "Fetching latest certificates failed: error %s", err, exc_info=err
         )
     else:
         LOGGER.info("Fetched %s PAA root certificates from DCL.", fetch_count)
+
+    return fetch_count
+
+
+async def fetch_git_certificates() -> int:
+    """Fetch Git PAA Certificates."""
+    fetch_count = 0
+    LOGGER.info("Fetching the latest PAA root certificates from Git.")
+    try:
+        async with ClientSession(raise_for_status=True) as http_session:
+            for cert in GIT_CERTS:
+                if cert in LAST_CERT_IDS:
+                    continue
+
+                async with http_session.get(f"{GIT_URL}/{cert}.pem") as response:
+                    certificate = await response.text()
+                await write_paa_root_cert(certificate, cert)
+                LAST_CERT_IDS.add(cert)
+                fetch_count += 1
+    except ClientError as err:
+        LOGGER.warning(
+            "Fetching latest certificates failed: error %s", err, exc_info=err
+        )
+
+    LOGGER.info("Fetched %s PAA root certificates from Git.", fetch_count)
+
+    return fetch_count
+
+
+async def fetch_certificates(
+    fetch_test_certificates: bool = True,
+    fetch_production_certificates: bool = True,
+) -> int:
+    """Fetch PAA Certificates."""
+
+    fetch_count = await fetch_dcl_certificates(
+        fetch_test_certificates=fetch_test_certificates,
+        fetch_production_certificates=fetch_production_certificates,
+    )
+
+    if fetch_test_certificates:
+        fetch_count += await fetch_git_certificates()
+
     return fetch_count
```

### Comparing `python-matter-server-3.2.0/matter_server/server/server.py` & `python-matter-server-3.3.0/matter_server/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ServerInfoMessage,
 )
 from ..server.client_handler import WebsocketClientHandler
 from .const import MIN_SCHEMA_VERSION
 from .device_controller import MatterDeviceController
 from .stack import MatterStack
 from .storage import StorageController
+from .vendor_info import VendorInfo
 
 
 def mount_websocket(server: MatterServer, path: str) -> None:
     """Mount the websocket endpoint."""
     clients: weakref.WeakSet[WebsocketClientHandler] = weakref.WeakSet()
 
     async def _handle_ws(request: web.Request) -> web.WebSocketResponse:
@@ -71,14 +72,15 @@
         self.loop: asyncio.AbstractEventLoop | None = None
         # Instantiate the Matter Stack using the SDK using the given storage path
         self.stack = MatterStack(self)
         # Initialize our (intermediate) device controller which keeps track
         # of Matter devices and their subscriptions.
         self.device_controller = MatterDeviceController(self)
         self.storage = StorageController(self)
+        self.vendor_info = VendorInfo(self)
         # we dynamically register command handlers
         self.command_handlers: dict[str, APICommandHandler] = {}
         self._subscribers: Set[EventCallBackType] = set()
         self._register_api_commands()
 
     async def start(self) -> None:
         """Start running the Matter server."""
@@ -88,14 +90,15 @@
             raise VersionMismatch(
                 "CHIP Core version does not match CHIP Clusters version."
             )
         self.loop = asyncio.get_running_loop()
         await self.device_controller.initialize()
         await self.storage.start()
         await self.device_controller.start()
+        await self.vendor_info.start()
         mount_websocket(self, "/ws")
         self.app.router.add_route("GET", "/", self._handle_info)
         self._runner = web.AppRunner(self.app, access_log=None)
         await self._runner.setup()
         # set host to None to bind to all addresses on both IPv4 and IPv6
         self._http = web.TCPSite(self._runner, host=None, port=self.port)
         await self._http.start()
@@ -170,15 +173,15 @@
     ) -> None:
         """Dynamically register a command on the API."""
         assert command not in self.command_handlers, "Command already registered"
         self.command_handlers[command] = APICommandHandler.parse(command, handler)
 
     def _register_api_commands(self) -> None:
         """Register all methods decorated as api_command."""
-        for cls in (self, self.device_controller):
+        for cls in (self, self.device_controller, self.vendor_info):
             for attr_name in dir(cls):
                 if attr_name.startswith("__"):
                     continue
                 val = getattr(cls, attr_name)
                 if not hasattr(val, "api_cmd"):
                     continue
                 if hasattr(val, "mock_calls"):
```

### Comparing `python-matter-server-3.2.0/matter_server/server/stack.py` & `python-matter-server-3.3.0/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/matter_server/server/storage.py` & `python-matter-server-3.3.0/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.2.0/pyproject.toml` & `python-matter-server-3.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.2.0"
+version = "3.3.0"
 license     = {text = "Apache-2.0"}
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
@@ -22,30 +22,30 @@
 ]
 dependencies = [
   "aiohttp",
   "aiorun",
   "coloredlogs",
   "dacite",
   "orjson",
-  "home-assistant-chip-clusters==2023.2.2"
+  "home-assistant-chip-clusters==2023.4.0"
 ]
 
 [project.optional-dependencies]
 server = [
-  "home-assistant-chip-core==2023.2.2",
-  "cryptography==39.0.1"
+  "home-assistant-chip-core==2023.4.0",
+  "cryptography==40.0.2"
 ]
 test = [
-  "black==23.1.0",
+  "black==23.3.0",
   "flake8==6.0.0",
   "flake8-docstrings==1.7.0",
   "isort==5.12.0",
-  "mypy==1.1.1",
-  "pylint==2.17.1",
-  "pytest==7.2.2",
+  "mypy==1.2.0",
+  "pylint==2.17.2",
+  "pytest==7.3.1",
   "pytest-aiohttp==1.0.4",
   "pytest-cov==4.0.0",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
```

### Comparing `python-matter-server-3.2.0/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.3.0/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.2.0/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.3.0/python_matter_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 matter_server/server/__main__.py
 matter_server/server/client_handler.py
 matter_server/server/const.py
 matter_server/server/device_controller.py
 matter_server/server/server.py
 matter_server/server/stack.py
 matter_server/server/storage.py
+matter_server/server/vendor_info.py
 matter_server/server/helpers/__init__.py
 matter_server/server/helpers/paa_certificates.py
 python_matter_server.egg-info/PKG-INFO
 python_matter_server.egg-info/SOURCES.txt
 python_matter_server.egg-info/dependency_links.txt
 python_matter_server.egg-info/entry_points.txt
 python_matter_server.egg-info/not-zip-safe
```

