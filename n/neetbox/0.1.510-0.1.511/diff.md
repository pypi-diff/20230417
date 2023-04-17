# Comparing `tmp/neetbox-0.1.510.tar.gz` & `tmp/neetbox-0.1.511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.510.tar", max compression
+gzip compressed data, was "neetbox-0.1.511.tar", max compression
```

## Comparing `neetbox-0.1.510.tar` & `neetbox-0.1.511.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0     1067 2023-04-15 15:55:16.060901 neetbox-0.1.510/LICENSE
--rw-r--r--   0        0        0      397 2023-04-15 15:55:16.060901 neetbox-0.1.510/README.md
--rw-r--r--   0        0        0     2827 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/config/_config.py
--rw-r--r--   0        0        0       66 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/core/__init__.py
--rw-r--r--   0        0        0     5864 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/core/registry.py
--rw-r--r--   0        0        0     2878 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      608 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     1938 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     4946 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0     3226 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/daemon/_win_service.py
--rw-r--r--   0        0        0      378 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     4875 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8493 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0    12181 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18647 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/logging/logger.py
--rw-r--r--   0        0        0        0 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      277 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0        0 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      108 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2312 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4474 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/torch/profile.py
--rw-r--r--   0        0        0       76 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/utils/framing.py
--rw-r--r--   0        0        0     4780 2023-04-15 15:55:16.068901 neetbox-0.1.510/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1264 2023-04-15 15:55:16.068901 neetbox-0.1.510/pyproject.toml
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 neetbox-0.1.510/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-17 14:12:50.884822 neetbox-0.1.511/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-17 14:12:50.884822 neetbox-0.1.511/README.md
+-rw-r--r--   0        0        0     2827 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/config/_config.py
+-rw-r--r--   0        0        0       66 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/core/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/core/registry.py
+-rw-r--r--   0        0        0     2999 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      872 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     2161 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     8061 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0     3226 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/daemon/_win_service.py
+-rw-r--r--   0        0        0      337 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     3960 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/integrations/environment/hardware.py
+-rw-r--r--   0        0        0     1746 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/integrations/environment/platform.py
+-rw-r--r--   0        0        0     8536 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0    12181 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18762 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/logging/logger.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:12:50.888821 neetbox-0.1.511/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      275 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      108 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5636 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6703 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2400 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2699 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4702 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/torch/profile.py
+-rw-r--r--   0        0        0       78 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2669 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/utils/_package.py
+-rw-r--r--   0        0        0     1019 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/utils/format.py
+-rw-r--r--   0        0        0     2303 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     1238 2023-04-17 14:12:50.892822 neetbox-0.1.511/neetbox/utils/mvc.py
+-rw-r--r--   0        0        0     1271 2023-04-17 14:12:50.892822 neetbox-0.1.511/pyproject.toml
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 neetbox-0.1.511/PKG-INFO
```

### Comparing `neetbox-0.1.510/LICENSE` & `neetbox-0.1.511/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/__init__.py` & `neetbox-0.1.511/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/cli/parse.py` & `neetbox-0.1.511/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/config/__init__.py` & `neetbox-0.1.511/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/config/_config.py` & `neetbox-0.1.511/neetbox/config/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230413
 
 import collections
-from neetbox.utils.utils import patch
+from neetbox.utils.mvc import patch
 from multiprocessing import current_process
 
 DEFAULT_CONFIG = {
     "name": None,
     "version": None,
     "logging": {"logdir": None},
     "pipeline": {},
```

### Comparing `neetbox-0.1.510/neetbox/core/registry.py` & `neetbox-0.1.511/neetbox/core/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230413
 
 from neetbox.logging import logger
-from neetbox.utils.utils import *
+from neetbox.utils.format import *
 from typing import Optional, Union, Sequence
-import inspect
 import json
 import functools
-from typing import Any, Callable, Dict, List, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Sequence, Union
 
 
 class _RegEndpoint:
     def __init__(self, what, tags=None):
         """Generate a massive type which contains both the regietered object and it's tags
 
         Args:
@@ -38,15 +37,15 @@
     # class level
     _registry_pool: Dict[str, "Registry"] = dict()  # all registeres are stored here
 
     def __new__(cls, name: str) -> "Registry":
         assert is_pure_ansi(name), "Registry name should not contain non-ansi char."
         if name in cls._registry_pool:
             return cls._registry_pool[name]
-        logger.log(f"Creating Registry for '{name}'")
+        # logger.log(f"Creating Registry for '{name}'")
         instance = dict.__new__(cls)
         cls._registry_pool[name] = instance
         return instance
 
     # not compatible with python below 3.8
     def __init__(self, name, *args, **kwargs) -> None:
         if not "initialized" in self:
@@ -193,7 +192,9 @@
             dict(self.items()),
             indent=4,
             ensure_ascii=False,
             sort_keys=False,
             separators=(",", ":"),
             default=str,
         )
+        
+    __repr__ = __str__
```

### Comparing `neetbox-0.1.510/neetbox/daemon/__init__.py` & `neetbox-0.1.511/neetbox/daemon/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
-from neetbox.daemon._daemon_client import connect_daemon, watch
-from neetbox.daemon._daemon import daemon_process
+from neetbox.daemon._daemon_client import connect_daemon, watch, listen
 from neetbox.logging import logger
 from neetbox.utils import pkg
 import platform
 import time
 import os
 
 
 def __attach_daemon(daemon_config):
     if not daemon_config["allowIpython"]:
         try:
-            __IPYTHON__
+            eval("__IPYTHON__")
         except NameError:
             pass
         else:
             logger.log(
                 "NEETBOX DAEMON won't start when debugging in ipython console. If you want to allow daemon run in "
                 "ipython, try to set 'allowIpython' to True."
             )
             return False  # ignore if debugging in ipython
     _online_status = connect_daemon(daemon_config)  # try to connect daemon
     if not _online_status:  # if no daemon online
         logger.log(
             f"No daemon running at {daemon_config['server']}:{daemon_config['port']}, trying to create daemon..."
         )
-        if platform.system() == "Windows": # running on windows
+        if platform.system() == "Windows":  # running on windows
             try:
-                assert pkg.is_installed('win32api', try_install_if_not='pywin32'), "Please install 'pywin32' before using NEETBOX daemon"
-                assert pkg.is_installed('win32serviceutil', try_install_if_not='pypiwin32'), "Please install 'pywin32' before using NEETBOX daemon"
+                assert pkg.is_installed(
+                    "win32api", try_install_if_not="pywin32"
+                ), "Please install 'pywin32' before using NEETBOX daemon"
+                assert pkg.is_installed(
+                    "win32serviceutil", try_install_if_not="pypiwin32"
+                ), "Please install 'pywin32' before using NEETBOX daemon"
                 from neetbox.daemon._win_service import installService
+
                 installService(cfg=daemon_config)
             except Exception as e:
                 logger.err(f"Could not install Windows service because {e}.")
                 return False
-        else: # not on windows 
+        else:  # not on windows
             pid = os.fork()
             if pid == 0:  # child process
-                pkg.is_installed('daemon', try_install_if_not='python-daemon')
+                pkg.is_installed("daemon", try_install_if_not="python-daemon")
                 import daemon
+                from neetbox.daemon._daemon import daemon_process
+
                 with daemon.DaemonContext():
                     daemon_process(daemon_config)  # create daemon
             elif pid < 0:
                 logger.err(
                     "Faild to spawn daemon process using os.fork. NEETBOX daemon will not start."
                 )
                 return False
@@ -69,8 +75,8 @@
     from neetbox.config import get_module_level_config
 
     _cfg = get_module_level_config()
     if _cfg["enable"]:
         __attach_daemon(_cfg)
 
 
-__all__ = ["watch", "_try_attach_daemon"]
+__all__ = ["watch", "listen", "_try_attach_daemon"]
```

### Comparing `neetbox-0.1.510/neetbox/daemon/_daemon.py` & `neetbox-0.1.511/neetbox/daemon/_daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
 from neetbox.utils import pkg
+from neetbox.utils.framing import get_frame_module_traceback
+module_name = get_frame_module_traceback().__name__
+assert pkg.is_installed('flask', try_install_if_not=True), f"{module_name} requires flask which is not installed"
+from flask import Flask, json, abort, request
 from neetbox.config import get_module_level_config
 from threading import Thread
 import time
 import sys
 
 _STAT_POOL = {}
 __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC = 60 * 60
@@ -17,15 +21,14 @@
 
 
 def daemon_process(daemon_config=None):
     import setproctitle
 
     setproctitle.setproctitle(__DAEMON_NAME)
     daemon_config = daemon_config or get_module_level_config()
-    from flask import Flask, json, abort, request
     api = Flask(__DAEMON_NAME)
 
     @api.route("/hello", methods=["GET"])
     def just_send_hello():
         return json.dumps({"hello": "hello"})
 
     @api.route("/status", methods=["GET"], defaults={"name": None})
```

### Comparing `neetbox-0.1.510/neetbox/daemon/_win_service.py` & `neetbox-0.1.511/neetbox/daemon/_win_service.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/integrations/engine.py` & `neetbox-0.1.511/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/integrations/resource.py` & `neetbox-0.1.511/neetbox/integrations/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
 from random import random
 import os
-import asyncio
+from neetbox.utils import pkg
+assert pkg.is_installed('numpy', try_install_if_not=True)
 import numpy as np
 import threading
-from neetbox.utils import pkg
 from neetbox.logging import logger
 from neetbox.integrations import engine
 from typing import Dict
 import pathlib
 import urllib.request
 from tqdm import tqdm
 from typing import List, Union, Dict, Any
```

### Comparing `neetbox-0.1.510/neetbox/logging/_colorama.py` & `neetbox-0.1.511/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.511/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.511/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.511/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.511/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.511/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/formatting.py` & `neetbox-0.1.511/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/logging/logger.py` & `neetbox-0.1.511/neetbox/logging/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 # Date:   20230315
 
 import os
 import io
 from datetime import date, datetime
 from enum import Enum
 from neetbox.utils.framing import *
-from pyfiglet import Figlet, FigletFont
-from neetbox.utils import utils
+from neetbox.utils import format
 from neetbox.logging.formatting import *
 from inspect import isclass, iscoroutinefunction, isgeneratorfunction
 import functools
 import pathlib
 from random import randint
 from typing import *
 
@@ -450,15 +449,20 @@
                             return function(*args, **kwargs)
 
                 functools.update_wrapper(catch_wrapper, function)
                 return catch_wrapper
 
         return Catcher(False)
 
-    def banner(self, text, font: Optional[str] = None):        
+    def banner(self, text, font: Optional[str] = None):
+        from neetbox.utils import pkg
+
+        assert pkg.is_installed("pyfiglet", try_install_if_not=True)
+        from pyfiglet import Figlet, FigletFont
+
         builtin_font_list = [
             "ansiregular",
             "ansishadow",
             "isometrixc2",
             "nscripts",
             "nvscript",
         ]
@@ -467,15 +471,15 @@
 
         if font not in FigletFont.getFonts():
             if font in builtin_font_list:  # builtin but not installed
                 module_path = os.path.dirname(__file__)
                 FigletFont.installFonts(f"{module_path}/flfs/{font}.flf")
             else:  # path?
                 assert os.path.isfile(
-                font
+                    font
                 ), "The provided font is not a fontname or a font file path."
                 file_name = os.path.basename(font)
                 file = os.path.splitext(file_name)
                 if (
                     file[0] not in FigletFont.getFonts()
                 ):  # no installed file match the file name
                     try:
@@ -542,15 +546,15 @@
             return self
         if not path:
             self.file_writer = None
             return self
         log_file_identity = os.path.abspath(path)
         if os.path.isdir(log_file_identity):
             raise Exception("Target path is not a file.")
-        filename = utils.legal_file_name_of(os.path.basename(path))
+        filename = format.legal_file_name_of(os.path.basename(path))
         dirname = os.path.dirname(path) if len(os.path.dirname(path)) != 0 else "."
         if not os.path.exists(dirname):
             raise Exception(f"Could not find dictionary {dirname}")
         real_path = os.path.join(dirname, filename)
         if log_file_identity not in writers_dict:
             # todo add fflush buffer size or time
             writers_dict[log_file_identity] = open(
```

### Comparing `neetbox-0.1.510/neetbox/plotting/plot.py` & `neetbox-0.1.511/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/torch/arch/canny.py` & `neetbox-0.1.511/neetbox/torch/arch/canny.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,48 @@
+from neetbox.utils import pkg
+
+assert pkg.is_installed("numpy", try_install_if_not=True)
+from neetbox.utils.framing import get_frame_module_traceback
+
+module_name = get_frame_module_traceback().__name__
+assert pkg.is_installed(
+    "torch", try_install_if_not=False
+), f"{module_name} requires torch which is not installed."
 import numpy as np
 import torch
 import torch.nn as nn
 from neetbox.torch.arch.kernels import *
 
 
 class CannyFilter(nn.Module):
-    def __init__(self, k_gaussian=3, mu=0, sigma=1, k_sobel=3, padding=True, use_cuda=False,):
+    def __init__(
+        self,
+        k_gaussian=3,
+        mu=0,
+        sigma=1,
+        k_sobel=3,
+        padding=True,
+        use_cuda=False,
+    ):
         super(CannyFilter, self).__init__()
         # device
         self.device = "cuda" if use_cuda else "cpu"
         # gaussian
         gaussian_2D = get_gaussian_kernel(k_gaussian, mu, sigma)
         # gaussian_2D = gaussian_2D[None, None, :]
         self.gaussian_filter = nn.Conv2d(
             in_channels=1,
             out_channels=1,
             kernel_size=k_gaussian,
             padding=k_gaussian // 2 if padding else 0,
             bias=False,
         )
-        self.gaussian_filter.weight.data.copy_(torch.from_numpy(gaussian_2D[None, None, :]))
+        self.gaussian_filter.weight.data.copy_(
+            torch.from_numpy(gaussian_2D[None, None, :])
+        )
 
         # sobel
         sobel_2D = get_sobel_kernel(k_sobel)
         self.sobel_filter_x = nn.Conv2d(
             in_channels=1,
             out_channels=1,
             kernel_size=k_sobel,
@@ -73,23 +92,23 @@
         grad_y = torch.zeros((B, 1, H, W)).to(self.device)
         grad_magnitude = torch.zeros((B, 1, H, W)).to(self.device)
         grad_orientation = torch.zeros((B, 1, H, W)).to(self.device)
 
         # gaussian
 
         for c in range(C):
-            blurred[:, c: c + 1] = self.gaussian_filter(img[:, c: c + 1])
+            blurred[:, c : c + 1] = self.gaussian_filter(img[:, c : c + 1])
 
-            grad_x = grad_x + self.sobel_filter_x(blurred[:, c: c + 1])
-            grad_y = grad_y + self.sobel_filter_y(blurred[:, c: c + 1])
+            grad_x = grad_x + self.sobel_filter_x(blurred[:, c : c + 1])
+            grad_y = grad_y + self.sobel_filter_y(blurred[:, c : c + 1])
 
         # thick edges
 
         grad_x, grad_y = grad_x / C, grad_y / C
-        grad_magnitude = (grad_x ** 2 + grad_y ** 2) ** 0.5
+        grad_magnitude = (grad_x**2 + grad_y**2) ** 0.5
         grad_orientation = torch.atan(grad_y / grad_x)
         grad_orientation = grad_orientation * (360 / np.pi) + 180  # convert to degree
         grad_orientation = torch.round(grad_orientation / 45) * 45  # keep a split by 45
 
         # thin edges
 
         directional = self.directional_filter(grad_magnitude)
```

### Comparing `neetbox-0.1.510/neetbox/torch/arch/cnn.py` & `neetbox-0.1.511/neetbox/torch/arch/cnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
+from neetbox.utils import pkg
+from neetbox.utils.framing import get_frame_module_traceback
+
+module_name = get_frame_module_traceback().__name__
+assert pkg.is_installed(
+    "torch", try_install_if_not=False
+), f"{module_name} requires torch which is not installed."
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 def ConvNxN(
     inplanes,
```

### Comparing `neetbox-0.1.510/neetbox/torch/arch/kernels.py` & `neetbox-0.1.511/neetbox/torch/arch/kernels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from neetbox.utils import pkg
+assert pkg.is_installed('numpy', try_install_if_not=True)
 import numpy as np
 from neetbox.utils import pkg
 
 
 def get_gaussian_kernel(k=3, mu=0, sigma=1, normalize=True):
     # compute 1 dimension gaussian
     gaussian_1D = np.linspace(-1, 1, k)
```

### Comparing `neetbox-0.1.510/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.511/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from neetbox.utils import pkg
+from neetbox.utils.framing import get_frame_module_traceback
+module_name = get_frame_module_traceback().__name__
+assert pkg.is_installed('torch', try_install_if_not=False), f"{module_name} requires torch which is not installed."
 import torch
 import torch.nn.functional as F
 
 class MaskEdgeDetecter(torch.nn.Module):
     """generate the 'edge bar' for a 0-1 mask Groundtruth of a image
     Algorithm is based on 'Morphological Dilation and Difference Reduction'
```

### Comparing `neetbox-0.1.510/neetbox/torch/nlp.py` & `neetbox-0.1.511/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/neetbox/torch/profile.py` & `neetbox-0.1.511/neetbox/torch/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
 from neetbox.utils import pkg
+from neetbox.utils.framing import get_frame_module_traceback
+module_name = get_frame_module_traceback().__name__
+assert pkg.is_installed('torch', try_install_if_not=False), f"{module_name} requires torch which is not installed."
 import time
 from tqdm import tqdm
 import torch
-
 from neetbox.logging import logger
 
 
 def profile(
     model,
     input_shape=(1, 3, 1280, 720),
     specific_input=None,
```

### Comparing `neetbox-0.1.510/neetbox/utils/framing.py` & `neetbox-0.1.511/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.510/pyproject.toml` & `neetbox-0.1.511/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.510"
+version = "0.1.511"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
@@ -29,25 +29,26 @@
 # [[tool.poetry.source]]
 # name = "pypi"
 # url = "https://pypi.org/simple"
 # default = true
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-numpy = ">=1"
 tqdm = ">=4"
 colorama = ">=0.3"
 toml = ">0.10"
-gputil = ">=1.4"
-psutil = ">=5.0"
 injector = ">=0.20"
-pyfiglet = ">=0.8"
-flask = "^2.2.3"
 setproctitle = "^1.3.2"
+rich = "^13.3.4"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^6.0.0"
 requests = "^2.28.2"
+flask = "^2.2.3"
+
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
 neet = 'neetbox.cli.parse:parse'
```

