# Comparing `tmp/redbuild-2.0.3.tar.gz` & `tmp/redbuild-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.0.3.tar", max compression
+gzip compressed data, was "redbuild-2.0.4.tar", max compression
```

## Comparing `redbuild-2.0.3.tar` & `redbuild-2.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.3/LICENSE
--rw-r--r--   0        0        0     2408 2023-04-17 00:28:40.042586 redbuild-2.0.3/README.md
--rw-r--r--   0        0        0      531 2023-04-17 00:41:32.388603 redbuild-2.0.3/pyproject.toml
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.3/redbuild/__main__.py
--rw-r--r--   0        0        0     6145 2023-04-17 00:41:21.261948 redbuild-2.0.3/redbuild/cli.py
--rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.3/redbuild/engine.py
--rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.3/redbuild/models.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.3/redbuild/util.py
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 redbuild-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.4/LICENSE
+-rw-r--r--   0        0        0     2408 2023-04-17 00:28:40.042586 redbuild-2.0.4/README.md
+-rw-r--r--   0        0        0      556 2023-04-17 00:58:33.035094 redbuild-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.4/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.4/redbuild/__main__.py
+-rw-r--r--   0        0        0     6782 2023-04-17 00:58:17.711653 redbuild-2.0.4/redbuild/cli.py
+-rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.4/redbuild/engine.py
+-rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.4/redbuild/models.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.4/redbuild/util.py
+-rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 redbuild-2.0.4/PKG-INFO
```

### Comparing `redbuild-2.0.3/LICENSE` & `redbuild-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.3/README.md` & `redbuild-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.3/redbuild/cli.py` & `redbuild-2.0.4/redbuild/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,44 +8,57 @@
 import sh
 import sys
 import os
 import typer
 import multiprocessing
 import psutil
 from loguru import logger
+from typing import List, Optional
 
+from . import __version__
 from .engine import (
     ContainerEngine,
     detect_container_engine,
     get_container_engine_command,
 )
 from .util import get_builder_image_name, parse_secondary_args
 
+APP_NAME = "redbuild"
 app = typer.Typer(
-    name="redbuild",
-    help="redbuild is a tool for easy magic containerized builds",
+    name=APP_NAME,
+    help=f"{APP_NAME}: a tool for easy magic containerized builds",
     no_args_is_help=True,
 )
 
-PWD_VOLUME_MOUNT_OPTIONS = ":z"
+# bind mount volume options
+VOLUME_OPTS = ":z"
 
 
 @app.command()
 def info():
+    app_info_logo = f"{APP_NAME} v{__version__}"
+    print(app_info_logo)
+    print("- " * (len(app_info_logo) // 2 + 1))
+
+    # show info about host
+    print("Host information:")
     host_os = sys.platform
     host_arch = sys.maxsize > 2**32 and "64bit" or "32bit"
     host_cores = multiprocessing.cpu_count()
     host_memory = int(psutil.virtual_memory().total / 1024**2)
-    print(f"Host OS: {host_os}")
-    print(f"Host architecture: {host_arch}")
-    print(f"Host cores: {host_cores}")
-    print(f"Host memory: {host_memory} MB")
+    print(f"  Host OS: {host_os}")
+    print(f"  Host architecture: {host_arch}")
+    print(f"  Host cores: {host_cores}")
+    print(f"  Host memory: {host_memory} MB")
 
+    # show info about container engine
     container_engine = detect_container_engine()
     print(f"Container engine: {container_engine}")
+    ctr_engine = get_container_engine_command(container_engine)
+    print(f"  Version: {ctr_engine('--version')}", end="")
 
 
 # build the build environment image
 @app.command()
 def image(
     dockerfile: str = typer.Option(
         "build.docker",
@@ -133,15 +146,15 @@
     )
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         # "-it",
         "-v",
-        f"{cwd}:/prj{PWD_VOLUME_MOUNT_OPTIONS}",
+        f"{cwd}:/prj{VOLUME_OPTS}",
         *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
         # _fg=True,
         # output formatting
         _out=lambda line: print(f"  {line}", end=""),
@@ -196,15 +209,15 @@
     print(f"Running interactive shell in [{builder_image_name}] in context [{cwd}]:")
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         "-it",
         "-v",
-        f"{cwd}:/prj{PWD_VOLUME_MOUNT_OPTIONS}",
+        f"{cwd}:/prj{VOLUME_OPTS}",
         *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
     )
 
     logger.debug(f"Running command: {run_cmd}")
@@ -213,17 +226,26 @@
         "/bin/bash",
         "-l",
         *parse_secondary_args(shell_args),
         _fg=True,
     )
 
 
+def version_callback(value: bool):
+    if value:
+        print(__version__)
+        raise typer.Exit()
+
+
 @app.callback()
 def app_callback(
-    verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output")
+    verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output"),
+    version: Optional[bool] = typer.Option(
+        None, "--version", "-V", callback=version_callback
+    ),
 ):
     # loguru setup
     logger.remove()
     if verbose:
         logger.add(sys.stderr, level="DEBUG")
     else:
         logger.add(sys.stderr, level="INFO")
```

### Comparing `redbuild-2.0.3/redbuild/engine.py` & `redbuild-2.0.4/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.3/redbuild/util.py` & `redbuild-2.0.4/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.3/PKG-INFO` & `redbuild-2.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.0.3
+Version: 2.0.4
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: sh (>=2.0.3,<3.0.0)
+Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 
 # redbuild
```

