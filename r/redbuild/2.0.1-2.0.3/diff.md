# Comparing `tmp/redbuild-2.0.1.tar.gz` & `tmp/redbuild-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.0.1.tar", max compression
+gzip compressed data, was "redbuild-2.0.3.tar", max compression
```

## Comparing `redbuild-2.0.1.tar` & `redbuild-2.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.1/LICENSE
--rw-r--r--   0        0        0     2159 2023-04-16 01:37:14.306507 redbuild-2.0.1/README.md
--rw-r--r--   0        0        0      543 2023-04-17 00:22:15.265993 redbuild-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.1/redbuild/__main__.py
--rw-r--r--   0        0        0     5881 2023-04-16 01:16:13.779330 redbuild-2.0.1/redbuild/cli.py
--rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.1/redbuild/engine.py
--rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.1/redbuild/models.py
--rw-r--r--   0        0        0      751 2023-04-16 00:49:50.747661 redbuild-2.0.1/redbuild/util.py
--rw-r--r--   0        0        0     2801 1970-01-01 00:00:00.000000 redbuild-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2408 2023-04-17 00:28:40.042586 redbuild-2.0.3/README.md
+-rw-r--r--   0        0        0      531 2023-04-17 00:41:32.388603 redbuild-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.3/redbuild/__main__.py
+-rw-r--r--   0        0        0     6145 2023-04-17 00:41:21.261948 redbuild-2.0.3/redbuild/cli.py
+-rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.3/redbuild/engine.py
+-rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.3/redbuild/models.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.3/redbuild/util.py
+-rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 redbuild-2.0.3/PKG-INFO
```

### Comparing `redbuild-2.0.1/LICENSE` & `redbuild-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.1/README.md` & `redbuild-2.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 
 ## overview
 
 redbuild is a super simple drop-in script enabling software to be built in pre-defined containers. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
 
 `redbuild`: just add water!
 
-## build redbuild2 using redbuild1
+## install stable version from pypi
+
+```sh
+pip install redbuild
+```
+
+## build from source
 
 To build redbuild2, we will use the redbuild1 shell script to bootstrap the build environment and build redbuild2.
     
 ```sh
 ./bootstrap/redbuild.sh
 ```
 
@@ -36,34 +42,35 @@
 ```
 
 ## detailed usage
 
 ### creating the build environment and build script
 
 1. create a `build.docker` file in the project root. this file should contain a `FROM` directive for the base image to use for the build environment. the build environment should contain all the tools necessary to build the project.
+it's also very important that the last line of the dockerfile is `CMD ["/bin/bash", "-l"]`. this is necessary for redbuild to work.
 
-    `build.docker`:
+    an example `build.docker`:
 
     ```dockerfile
-    FROM debian:buster-slim
+    FROM debian:bookworm-slim
 
     # install dependencies
     RUN apt-get update && apt-get install -y \
-    bash \
-    curl wget xz-utils \
-    gcc make libc6-dev libcurl4 \
-    git libxml2 \
-    && rm -rf /var/lib/apt/lists/* && apt autoremove -y && apt clean
+        bash \
+        curl wget xz-utils \
+        gcc make libc6-dev libcurl4 \
+        git libxml2 \
+        && rm -rf /var/lib/apt/lists/* && apt autoremove -y && apt clean
 
 
     # install dlang
     RUN curl -fsS https://dlang.org/install.sh | bash -s install ldc-1.30.0 \
-    && echo "source ~/dlang/ldc-1.30.0/activate" >> ~/.bashrc
+        && echo "source ~/dlang/ldc-1.30.0/activate" >> ~/.bashrc
 
-    # set up main to run bash
+    # set up main to run bash (necessary for redbuild)
     CMD ["/bin/bash", "-l"]
     ```
 
 2. create a `build.sh` file in the project root. this file should contain the steps necessary to build the project. the build script should be written to be run in the build environment.
 
     `build.sh`:
```

### Comparing `redbuild-2.0.1/redbuild/cli.py` & `redbuild-2.0.3/redbuild/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 from loguru import logger
 
 from .engine import (
     ContainerEngine,
     detect_container_engine,
     get_container_engine_command,
 )
-from .util import get_builder_image_name
+from .util import get_builder_image_name, parse_secondary_args
 
 app = typer.Typer(
     name="redbuild",
     help="redbuild is a tool for easy magic containerized builds",
     no_args_is_help=True,
 )
 
+PWD_VOLUME_MOUNT_OPTIONS = ":z"
+
 
 @app.command()
 def info():
     host_os = sys.platform
     host_arch = sys.maxsize > 2**32 and "64bit" or "32bit"
     host_cores = multiprocessing.cpu_count()
     host_memory = int(psutil.virtual_memory().total / 1024**2)
@@ -131,16 +133,16 @@
     )
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         # "-it",
         "-v",
-        f"{cwd}:/prj",
-        *[arg for arg in crun_args.split(" ") if arg],
+        f"{cwd}:/prj{PWD_VOLUME_MOUNT_OPTIONS}",
+        *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
         # _fg=True,
         # output formatting
         _out=lambda line: print(f"  {line}", end=""),
         _err=lambda line: print(f"  {line}", end=""),
@@ -170,14 +172,20 @@
     ),
     crun_args=typer.Option(
         "",
         "--crun-args",
         "-R",
         help="Additional arguments to pass to container engine",
     ),
+    shell_args=typer.Option(
+        "",
+        "--shell-args",
+        "-A",
+        help="Additional arguments to pass to shell",
+    ),
 ):
     # 0. get container engine
     ctr_engine = get_container_engine_command(detect_container_engine())
 
     # 1. get name for builder image
     builder_image_name = get_builder_image_name(cwd)
 
@@ -188,26 +196,27 @@
     print(f"Running interactive shell in [{builder_image_name}] in context [{cwd}]:")
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         "-it",
         "-v",
-        f"{cwd}:/prj",
-        *[arg for arg in crun_args.split(" ") if arg],
+        f"{cwd}:/prj{PWD_VOLUME_MOUNT_OPTIONS}",
+        *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
     )
 
     logger.debug(f"Running command: {run_cmd}")
     run_proc = run_cmd(
         builder_image_name,
         "/bin/bash",
         "-l",
+        *parse_secondary_args(shell_args),
         _fg=True,
     )
 
 
 @app.callback()
 def app_callback(
     verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output")
```

### Comparing `redbuild-2.0.1/redbuild/engine.py` & `redbuild-2.0.3/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.1/redbuild/util.py` & `redbuild-2.0.3/redbuild/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,7 +19,11 @@
     cwd_dirname = "".join([c for c in cwd_dirname if c.isalnum()])
 
     cwd_hash = hashlib.sha256(cwd.encode("utf-8")).hexdigest()[:8]
 
     builder_tag = f"redbuild_builder_{cwd_dirname}_{cwd_hash}"
 
     return builder_tag
+
+
+def parse_secondary_args(args):
+    return [arg for arg in args.split(" ") if arg]
```

### Comparing `redbuild-2.0.1/PKG-INFO` & `redbuild-2.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.0.1
+Version: 2.0.3
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,15 +24,21 @@
 
 ## overview
 
 redbuild is a super simple drop-in script enabling software to be built in pre-defined containers. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
 
 `redbuild`: just add water!
 
-## build redbuild2 using redbuild1
+## install stable version from pypi
+
+```sh
+pip install redbuild
+```
+
+## build from source
 
 To build redbuild2, we will use the redbuild1 shell script to bootstrap the build environment and build redbuild2.
     
 ```sh
 ./bootstrap/redbuild.sh
 ```
 
@@ -55,34 +61,35 @@
 ```
 
 ## detailed usage
 
 ### creating the build environment and build script
 
 1. create a `build.docker` file in the project root. this file should contain a `FROM` directive for the base image to use for the build environment. the build environment should contain all the tools necessary to build the project.
+it's also very important that the last line of the dockerfile is `CMD ["/bin/bash", "-l"]`. this is necessary for redbuild to work.
 
-    `build.docker`:
+    an example `build.docker`:
 
     ```dockerfile
-    FROM debian:buster-slim
+    FROM debian:bookworm-slim
 
     # install dependencies
     RUN apt-get update && apt-get install -y \
-    bash \
-    curl wget xz-utils \
-    gcc make libc6-dev libcurl4 \
-    git libxml2 \
-    && rm -rf /var/lib/apt/lists/* && apt autoremove -y && apt clean
+        bash \
+        curl wget xz-utils \
+        gcc make libc6-dev libcurl4 \
+        git libxml2 \
+        && rm -rf /var/lib/apt/lists/* && apt autoremove -y && apt clean
 
 
     # install dlang
     RUN curl -fsS https://dlang.org/install.sh | bash -s install ldc-1.30.0 \
-    && echo "source ~/dlang/ldc-1.30.0/activate" >> ~/.bashrc
+        && echo "source ~/dlang/ldc-1.30.0/activate" >> ~/.bashrc
 
-    # set up main to run bash
+    # set up main to run bash (necessary for redbuild)
     CMD ["/bin/bash", "-l"]
     ```
 
 2. create a `build.sh` file in the project root. this file should contain the steps necessary to build the project. the build script should be written to be run in the build environment.
 
     `build.sh`:
```

