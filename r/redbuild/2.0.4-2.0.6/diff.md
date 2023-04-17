# Comparing `tmp/redbuild-2.0.4.tar.gz` & `tmp/redbuild-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.0.4.tar", max compression
+gzip compressed data, was "redbuild-2.0.6.tar", max compression
```

## Comparing `redbuild-2.0.4.tar` & `redbuild-2.0.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.4/LICENSE
--rw-r--r--   0        0        0     2408 2023-04-17 00:28:40.042586 redbuild-2.0.4/README.md
--rw-r--r--   0        0        0      556 2023-04-17 00:58:33.035094 redbuild-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.4/redbuild/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.4/redbuild/__main__.py
--rw-r--r--   0        0        0     6782 2023-04-17 00:58:17.711653 redbuild-2.0.4/redbuild/cli.py
--rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.4/redbuild/engine.py
--rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.4/redbuild/models.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.4/redbuild/util.py
--rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 redbuild-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.6/LICENSE
+-rw-r--r--   0        0        0     2408 2023-04-17 00:28:40.042586 redbuild-2.0.6/README.md
+-rw-r--r--   0        0        0      604 2023-04-17 01:34:09.601405 redbuild-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.6/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.6/redbuild/__main__.py
+-rw-r--r--   0        0        0     8906 2023-04-17 01:33:20.815068 redbuild-2.0.6/redbuild/cli.py
+-rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.6/redbuild/engine.py
+-rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.6/redbuild/models.py
+-rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.0.6/redbuild/res.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.6/redbuild/util.py
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 redbuild-2.0.6/PKG-INFO
```

### Comparing `redbuild-2.0.4/LICENSE` & `redbuild-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.4/README.md` & `redbuild-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.4/pyproject.toml` & `redbuild-2.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "redbuild"
-version = "2.0.4"
+version = "2.0.6"
 description = "magic containerized builds"
 authors = ["redthing1 <redthing1@alt.icu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-typer = "^0.7.0"
+typer = {extras = ["rich"], version = "^0.7.0"}
 sh = "^2.0.3"
 toml = "^0.10.2"
 ordered-set = "^4.1.0"
 loguru = "^0.7.0"
 psutil = "^5.9.4"
 single-source = "^0.3.0"
+rich = "^13.3.4"
 
 [tool.poetry.group.dev.dependencies]
 nuitka = "^1.5.5"
 zstandard = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `redbuild-2.0.4/redbuild/cli.py` & `redbuild-2.0.6/redbuild/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 from . import __version__
 from .engine import (
     ContainerEngine,
     detect_container_engine,
     get_container_engine_command,
 )
 from .util import get_builder_image_name, parse_secondary_args
+from .res import DEFAULT_BUILDENV_DOCKERFILE
 
 APP_NAME = "redbuild"
 app = typer.Typer(
     name=APP_NAME,
     help=f"{APP_NAME}: a tool for easy magic containerized builds",
     no_args_is_help=True,
 )
 
-# bind mount volume options
-VOLUME_OPTS = ":z"
+DEFAULT_DOCKERFILE = (
+    "build.docker"  # filename of default dockerfile for build environment
+)
+VOLUME_OPTS = ":z"  # bind mount volume options
 
 
 @app.command()
 def info():
     app_info_logo = f"{APP_NAME} v{__version__}"
     print(app_info_logo)
     print("- " * (len(app_info_logo) // 2 + 1))
@@ -53,19 +56,18 @@
     # show info about container engine
     container_engine = detect_container_engine()
     print(f"Container engine: {container_engine}")
     ctr_engine = get_container_engine_command(container_engine)
     print(f"  Version: {ctr_engine('--version')}", end="")
 
 
-# build the build environment image
-@app.command()
+@app.command(help="Build a container image for the build environment")
 def image(
     dockerfile: str = typer.Option(
-        "build.docker",
+        DEFAULT_DOCKERFILE,
         "--dockerfile",
         "-f",
         help="Dockerfile to use for defining the build environment",
     ),
     cwd: str = typer.Option(
         ".", "--cwd", "-C", help="Directory to use as the build context"
     ),
@@ -77,17 +79,18 @@
 
     # full path to dockerfile
     dockerfile = os.path.join(cwd, dockerfile)
 
     # 2. build builder image
     # ensure dockerfile exists
     if not os.path.isfile(dockerfile):
-        raise Exception(
-            f"Dockerfile {dockerfile} not found. Create it or pass a specific path with -f."
+        print(
+            f"Dockerfile [{dockerfile}] not found. Create it or pass a specific path with -f."
         )
+        raise typer.Exit(1)
 
     # $CONTAINER_ENGINE build -t $BUILDER_TAG $CBUILD_ARGS -f $DOCKERFILE | sed 's/^/  /'
     print(f"Building builder image [{builder_image_name}] in context [{cwd}]:")
     build_cmd = ctr_engine.bake(
         "build",
         cwd,
         # podman build args
@@ -96,21 +99,25 @@
         # _fg=True,
         # output formatting
         _out=lambda line: print(f"  {line}", end=""),
         _err=lambda line: print(f"  {line}", end=""),
     )
 
     logger.debug(f"Running command: {build_cmd}")
-    build_proc = build_cmd()
+    try:
+        build_proc = build_cmd()
+    except sh.ErrorReturnCode as e:
+        print(f"Build failed with error code {e.exit_code}")
+        raise typer.Exit(1)
 
 
-@app.command()
+@app.command(help="Run a build script in the build environment")
 def build(
     dockerfile: str = typer.Option(
-        "build.docker",
+        DEFAULT_DOCKERFILE,
         "--dockerfile",
         "-f",
         help="Dockerfile to use for defining the build environment",
     ),
     buildscript: str = typer.Option(
         "build.sh", "--buildscript", "-s", help="Build script to run in the container"
     ),
@@ -136,14 +143,21 @@
     # 1. get name for builder image
     builder_image_name = get_builder_image_name(cwd)
 
     # 2. build builder image
     image(dockerfile=dockerfile, cwd=cwd)
 
     # 3. run build
+    buildscript_path = os.path.join(cwd, buildscript)
+    # ensure buildscript exists
+    if not os.path.isfile(buildscript_path):
+        print(
+            f"Build script [{buildscript_path}] not found. Create it or pass a specific path with -s."
+        )
+        raise typer.Exit(1)
     # $CONTAINER_ENGINE run --rm -it -v $(pwd):/prj $CRUN_ARGS $BUILDER_TAG /bin/bash -l -c "cd /prj && $BUILDSCRIPT $ARGS" | sed 's/^/  /'
     print(
         f"Running build in [{builder_image_name}] with buildscript [{buildscript}] in context [{cwd}]:"
     )
     run_cmd_args = [
         "run",
         # podman run args
@@ -159,27 +173,32 @@
         # output formatting
         _out=lambda line: print(f"  {line}", end=""),
         _err=lambda line: print(f"  {line}", end=""),
     )
 
     relative_buildscript = f"./{buildscript}"
     logger.debug(f"Running command: {run_cmd}")
-    run_proc = run_cmd(
-        builder_image_name,
-        "/bin/bash",
-        "-l",
-        "-c",
-        f"cd /prj && {relative_buildscript} {build_args}",
-    )
 
+    try:
+        run_proc = run_cmd(
+            builder_image_name,
+            "/bin/bash",
+            "-l",
+            "-c",
+            f"cd /prj && {relative_buildscript} {build_args}",
+        )
+    except sh.ErrorReturnCode as e:
+        print(f"Build failed with error code {e.exit_code}")
+        raise typer.Exit(1)
 
-@app.command()
+
+@app.command(help="Run a shell in the build environment")
 def shell(
     dockerfile: str = typer.Option(
-        "build.docker",
+        DEFAULT_DOCKERFILE,
         "--dockerfile",
         "-f",
         help="Dockerfile to use for defining the build environment",
     ),
     cwd: str = typer.Option(
         ".", "--cwd", "-C", help="Directory to use as the build context"
     ),
@@ -217,21 +236,57 @@
         *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
     )
 
     logger.debug(f"Running command: {run_cmd}")
-    run_proc = run_cmd(
-        builder_image_name,
-        "/bin/bash",
-        "-l",
-        *parse_secondary_args(shell_args),
-        _fg=True,
-    )
+
+    try:
+        run_proc = run_cmd(
+            builder_image_name,
+            "/bin/bash",
+            "-l",
+            *parse_secondary_args(shell_args),
+            _fg=True,
+        )
+    except sh.ErrorReturnCode as e:
+        print(f"Shell failed with error code {e.exit_code}")
+        raise typer.Exit(1)
+
+
+@app.command(help="Initialize a build environment")
+def init(
+    dockerfile: str = typer.Option(
+        DEFAULT_DOCKERFILE,
+        "--dockerfile",
+        "-f",
+        help="Dockerfile to use for defining the build environment",
+    ),
+    cwd: str = typer.Option(
+        ".", "--cwd", "-C", help="Directory to use as the build context"
+    ),
+    force: bool = typer.Option(
+        False, "--force", "-f", help="Force initialization even if Dockerfile exists"
+    ),
+):
+    # first, ensure that no build environment already exists
+    dockerfile_path = os.path.join(cwd, dockerfile)
+    if os.path.exists(dockerfile_path) and not force:
+        # logger.error(f"{dockerfile} already exists in {cwd}")
+        print(
+            f"Failed to initialize build environment dockerfile: [{dockerfile}] already exists in [{cwd}]."
+        )
+        raise typer.Exit(1)
+
+    # write out a default Dockerfile
+    with open(dockerfile_path, "w") as f:
+        f.write(DEFAULT_BUILDENV_DOCKERFILE)
+
+    print(f"Initialized build environment dockerfile: Created [{dockerfile_path}].")
 
 
 def version_callback(value: bool):
     if value:
         print(__version__)
         raise typer.Exit()
```

### Comparing `redbuild-2.0.4/redbuild/engine.py` & `redbuild-2.0.6/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.4/redbuild/util.py` & `redbuild-2.0.6/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.4/PKG-INFO` & `redbuild-2.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.0.4
+Version: 2.0.6
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
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: sh (>=2.0.3,<3.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer[rich] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 
 # redbuild
 
 magic containerized builds
```

