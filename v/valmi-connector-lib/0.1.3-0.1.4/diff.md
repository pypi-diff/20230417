# Comparing `tmp/valmi_connector_lib-0.1.3.tar.gz` & `tmp/valmi_connector_lib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.3.tar", last modified: Mon Apr 17 11:33:33 2023, max compression
+gzip compressed data, was "valmi_connector_lib-0.1.4.tar", last modified: Mon Apr 17 11:39:16 2023, max compression
```

## Comparing `valmi_connector_lib-0.1.3.tar` & `valmi_connector_lib-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.582954 valmi_connector_lib-0.1.3/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:33:33.583013 valmi_connector_lib-0.1.3/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.3/pyproject.toml
--rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 11:33:33.583299 valmi_connector_lib-0.1.3/setup.cfg
--rw-r--r--   0 raj        (501) staff       (20)      600 2023-04-17 11:33:18.000000 valmi_connector_lib-0.1.3/setup.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.579686 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/SOURCES.txt
--rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/dependency_links.txt
--rw-r--r--   0 raj        (501) staff       (20)       48 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/requires.txt
--rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/top_level.txt
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.579790 valmi_connector_lib-0.1.3/valmi_lib/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.3/valmi_lib/__init__.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.581070 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)     6006 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-15 12:32:17.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/engine.py
--rw-r--r--   0 raj        (501) staff       (20)     5403 2023-04-15 12:33:27.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)     3556 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0 raj        (501) staff       (20)     2448 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/read_handlers.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.581435 valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/source_container_wrapper.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.581932 valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/
--rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/valmi_destination.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.582759 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/
--rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/valmi_event.py
--rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/valmi_protocol.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.929419 valmi_connector_lib-0.1.4/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:39:16.929462 valmi_connector_lib-0.1.4/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.4/pyproject.toml
+-rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 11:39:16.929690 valmi_connector_lib-0.1.4/setup.cfg
+-rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-17 11:39:11.000000 valmi_connector_lib-0.1.4/setup.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.926445 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/requires.txt
+-rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/top_level.txt
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.926546 valmi_connector_lib-0.1.4/valmi_lib/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.4/valmi_lib/__init__.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.927717 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/engine.py
+-rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/read_handlers.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.928029 valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/source_container_wrapper.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.928577 valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/
+-rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/valmi_destination.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.929294 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/
+-rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/valmi_protocol.py
```

### Comparing `valmi_connector_lib-0.1.3/setup.py` & `valmi_connector_lib-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import find_packages, setup
 
 MAIN_REQUIREMENTS = [
     "requests",
     "valmi_airbyte_cdk",
+    "pydantic",
 ]
 
 TEST_REQUIREMENTS = [
     "pytest~=6.2",
 ]
 
 setup(
     name="valmi_connector_lib",
-    version="0.1.3",
+    version="0.1.4",
     description="Connector library for valmi connectors.",
     long_description="Connector library for valmi connectors.",
     author="Rajashekar Varkala @ valmi.io",
     author_email="contact@valmi.io",
     packages=find_packages(),
     install_requires=MAIN_REQUIREMENTS,
     package_data={"": ["*.json", "*.yaml"]},
```

### Comparing `valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/SOURCES.txt` & `valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 """
 
 import json
 import os
 import sys
 import subprocess
 import io
-from proc_stdout_handler import ProcStdoutHandlerThread
-from proc_stdout_event_handlers import (
+from .proc_stdout_handler import ProcStdoutHandlerThread
+from .proc_stdout_event_handlers import (
     Engine,
     StoreReader,
     NullEngine,
 )
-from read_handlers import ReadCheckpointHandler, ReadDefaultHandler, ReadLogHandler, ReadRecordHandler
-from proc_stdout_handler import handlers as stdout_handlers
+from .read_handlers import ReadCheckpointHandler, ReadDefaultHandler, ReadLogHandler, ReadRecordHandler
+from .proc_stdout_handler import handlers as stdout_handlers
 
 handlers = {
     "LOG": ReadLogHandler,
     "STATE": ReadCheckpointHandler,
     "RECORD": ReadRecordHandler,
     "default": ReadDefaultHandler,
 }
```

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 SOFTWARE.
 """
 
 import json
 import os
 from os.path import join
 import time
-from engine import NullEngine, ConnectorState, Engine
+from .engine import NullEngine, ConnectorState, Engine
 
 # TODO: Constants - need to become env vars
 MAGIC_NUM = 0x7FFFFFFF
 
 
 class StoreWriter:
     def __init__(self) -> None:
```

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 SOFTWARE.
 """
 
 import json
 import os
 import io
 import threading
-from proc_stdout_event_handlers import LogHandler, CheckpointHandler, DefaultHandler, Engine, TraceHandler
+from .proc_stdout_event_handlers import LogHandler, CheckpointHandler, DefaultHandler, Engine, TraceHandler
 import logging
 
 handlers = {
     "LOG": LogHandler,
     "STATE": CheckpointHandler,
     "default": DefaultHandler,
     "TRACE": TraceHandler,
```

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/read_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from proc_stdout_event_handlers import (
+from .proc_stdout_event_handlers import (
     Engine,
     StoreWriter,
     StoreReader,
     StdoutWriter,
 )
```

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/source_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/valmi_destination.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/valmi_protocol.py`

 * *Files identical despite different names*

