# Comparing `tmp/mlcube_singularity-0.0.8.tar.gz` & `tmp/mlcube_singularity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcube_singularity-0.0.8.tar", last modified: Wed Sep 21 22:31:27 2022, max compression
+gzip compressed data, was "mlcube_singularity-0.0.9.tar", last modified: Mon Apr 17 18:11:26 2023, max compression
```

## Comparing `mlcube_singularity-0.0.8.tar` & `mlcube_singularity-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:27.256505 mlcube_singularity-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-21 22:31:27.256505 mlcube_singularity-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:27.252505 mlcube_singularity-0.0.8/mlcube_singularity/
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11931 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/singularity_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:27.256505 mlcube_singularity-0.0.8/mlcube_singularity/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/tests/test_factory_fn.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/tests/test_mlcommons_box_singularity_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/mlcube_singularity/tests/test_singularity_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:27.256505 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-21 22:31:27.000000 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-21 22:31:27.000000 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:31:27.000000 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-21 22:31:27.000000 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-21 22:31:27.000000 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-21 22:31:27.000000 mlcube_singularity-0.0.8/mlcube_singularity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:31:27.256505 mlcube_singularity-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-09-21 22:31:19.000000 mlcube_singularity-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:26.067803 mlcube_singularity-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 18:11:26.067803 mlcube_singularity-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:26.063802 mlcube_singularity-0.0.9/mlcube_singularity/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/singularity_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:26.067803 mlcube_singularity-0.0.9/mlcube_singularity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/tests/test_factory_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/mlcube_singularity/tests/test_singularity_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:26.063802 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 18:11:25.000000 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 18:11:26.000000 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:11:25.000000 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 18:11:25.000000 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 18:11:25.000000 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 18:11:25.000000 mlcube_singularity-0.0.9/mlcube_singularity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:11:26.067803 mlcube_singularity-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-17 18:11:15.000000 mlcube_singularity-0.0.9/setup.py
```

### Comparing `mlcube_singularity-0.0.8/mlcube_singularity/__init__.py` & `mlcube_singularity-0.0.9/mlcube_singularity/__init__.py`

 * *Files identical despite different names*

### Comparing `mlcube_singularity-0.0.8/mlcube_singularity/singularity_run.py` & `mlcube_singularity-0.0.9/mlcube_singularity/singularity_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,19 @@
             "image_dir": "${runtime.workspace}/.image",  # Root image directory for the image.
             "singularity": "singularity",  # Executable file for singularity runtime.
             "build_args": "--fakeroot",  # Image build arguments.
             "run_args": "",  # Container run arguments, example: -C --net.
             # Sergey: there seems to be a better name for this parameter. Originally, the only source was a singularity
             # recipe (build file). Later, MLCube started to support other sources, such as docker images.
             "build_file": "Singularity.recipe",  # Source for the image build process.
+            "--network": None,  # Networking options defined during MLCube container execution.
+            "--security": None,  # Security options defined during MLCube container execution.
+            "--nv": None,  # usage options defined during MLCube container execution.
+            "--vm-ram": None,  # RAM options defined during MLCube container execution.
+            "--vm-cpu": None  # CPU options defined during MLCube container execution.
         }
     )
 
     @staticmethod
     def merge(mlcube: DictConfig) -> None:
         """Merge current (mostly default) configuration with configuration from MLCube yaml file.
         Args:
@@ -44,17 +49,20 @@
                 platform-specific configuration sections (docker/singularity). In addition, this dictionary contains
                 'runtime' configuration (`root` and `workspace`), and `runner` configuration that contains default
                 runner configuration (Singularity in this case) from system settings file (it is exact or modified
                 version of `Config.DEFAULT` dictionary to account for user local environment).
         Idea is that if mlcube contains `singularity` section, then it means that we use it as is. Else, we can try
         to run this MLCube using information from `docker` section if it exists.
         """
+        # The `runner` section will contain effective runner configuration. At this point, it may contain configuration
+        # from system settings file.
         if 'runner' not in mlcube:
             mlcube['runner'] = {}
 
+        # We need to merge with the user-provided configuration.
         s_cfg: t.Optional[DictConfig] = mlcube.get("singularity", None)
         if not s_cfg:
             # Singularity runner will try to use docker section. At this point, it will work as long as we assume we
             # pull docker images from a docker hub.
             logger.warning(
                 "SingularityRun singularity configuration not found in MLCube file (singularity=%s).",
                 str(s_cfg),
@@ -68,16 +76,19 @@
                 )
                 return
 
             # The idea is that we can use the remote docker image as a source for the build process, automatically
             # generating an image name in a local environment. Key here is that the source has a scheme - `docker://`
             # The --fakeroot switch is useful and is supported in singularity version >= 3.5
             build_args = ""
+            # There's no `singularity` section, so we do not know what singularity executable to use. Let's assume
+            # it's just `singularity`.
+            singularity = "singularity"
             try:
-                SingularityRun.check_install()
+                SingularityRun.check_install(singularity)
                 version: semver.VersionInfo = get_singularity_version_info()
                 logger.info("SingularityRun singularity version %s", str(version))
                 if version >= semver.VersionInfo(major=3, minor=5):
                     logger.info(
                         "SingularityRun will use --fakeroot CLI switch (version >= 3.5)."
                     )
                     build_args = "--fakeroot"
@@ -97,15 +108,15 @@
             run_args = d_cfg.get("run_args", "")
             s_cfg = OmegaConf.create(
                 dict(
                     image="".join(c for c in d_cfg["image"] if c.isalnum()) + ".sif",
                     build_file=build_file,
                     build_args=build_args,
                     run_args=run_args,
-                    singularity="singularity",
+                    singularity=singularity,
                 )
             )
             logger.info(
                 f"SingularityRun singularity runner has converted docker configuration to singularity (%s).",
                 str(OmegaConf.to_container(s_cfg)),
             )
 
@@ -131,36 +142,65 @@
                 "SingularityRun check_install returned false ('singularity --version' failed to run). MLCube cannot "
                 "run singularity images unless this check passes. Singularity runner uses `check_install` function "
                 "from singularity-cli python library (https://github.com/singularityhub/singularity-cli).",
                 function='check_singularity_installed',
                 args={'software': singularity_exec}
             )
 
+    def _get_extra_args(self) -> str:
+        """Temporary solution to take into account run arguments provided by users."""
+        # Collect all parameters that start with '--' and have a non-None value.
+        extra_args = [
+            f'{key}={value}' for key, value in self.mlcube.runner.items() if key.startswith('--') and value is not None
+        ]
+        return ' '.join(extra_args)
+
     def __init__(self, mlcube: t.Union[DictConfig, t.Dict], task: t.Optional[str]) -> None:
         super().__init__(mlcube, task)
+        if self.mlcube.runner.singularity != 'singularity':
+            logger.warning(
+                "Singularity executable is not exactly 'singularity' (singularity=%s). The MLCube singularity runner "
+                "will use this executable, however the version of the `spython` library that the runner uses (which is "
+                "`0.2.1`) does not allow specifying a custom singularity executable when checking the singularity "
+                "version. It's OK if `singularity` resolves to` %s`, in other cases this may cause issues.",
+                self.mlcube.runner.singularity, self.mlcube.runner.singularity
+            )
         try:
             # Check version and log a warning message if fakeroot is used with singularity version < 3.5
             version: semver.VersionInfo = get_singularity_version_info()
             logger.info("SingularityRun singularity version = %s", str(version))
             if version < semver.VersionInfo(major=3, minor=5) and "--fakeroot" in (
                 self.mlcube.runner.build_args or ""
             ):
                 logger.warning(
                     "SingularityRun singularity version < 3.5, and it probably does not support --fakeroot "
                     "parameter that is present in MLCube configuration."
                 )
         except Exception as err:
+            # It's correct to use `singularity` here, since the function that identifies the singularity version
+            # does not allow specifying a custom singularity executable (at least in spython == 0.2.1).
+            ver_cmd = f"singularity --version"
+            try:
+                self.check_install(self.mlcube.runner.singularity)
+                msg = "The runner has been able to successfully run the singularity executable (which is "\
+                      f"`{self.mlcube.runner.singularity}`). Most likely, the output of `{ver_cmd}` could not be "\
+                      "parsed. Please, create an issue in MLCube repository and provide the output of "\
+                      f"this command ({ver_cmd})"
+            except:
+                # And here we use the correct executable, since check_install supports user-provided executable.
+                msg = f"The runner has not been able to run this command (`{self.mlcube.runner.singularity} --help`)." \
+                      f"Please check that this executable is in PATH, or specify a custom path in ~/mlcube.yaml."
             logger.warning(
-                "SingularityRun can't get singularity version (do you have singularity installed?). "
-                "Source=SingularityRun.__init__. Exception=%s.", str(err), exc_info=True
+                "Singularity runner (cmd=%s) can't detect singularity version. %s. "
+                "Source=SingularityRun.__init__. Exception=%s.", ver_cmd, msg, str(err), exc_info=True
             )
 
     def configure(self) -> None:
         """Build Singularity Image on a current host."""
-        SingularityRun.check_install()
+        SingularityRun.check_install(self.mlcube.runner.singularity)
 
         s_cfg: DictConfig = self.mlcube.runner
 
         # Get full path to a singularity image. By design, we compute it relative to {mlcube.root}/workspace.
         image_file = Path(s_cfg.image_dir, s_cfg.image)
         if image_file.exists():
             logger.info(
@@ -198,15 +238,15 @@
 
     def run(self) -> None:
         """ """
         image_file = Path(self.mlcube.runner.image_dir) / self.mlcube.runner.image
         if not image_file.exists():
             self.configure()
         else:
-            SingularityRun.check_install()
+            SingularityRun.check_install(self.mlcube.runner.singularity)
 
         # Deal with user-provided workspace
         try:
             Shell.sync_workspace(self.mlcube, self.task)
         except Exception as err:
             raise ExecutionError.mlcube_run_error(
                 self.__class__.__name__,
@@ -226,26 +266,34 @@
                 self.__class__.__name__,
                 "Error occurred while generating mount points for singularity run command. See context for more "
                 "details and check your MLCube configuration file.",
                 error=str(err)
             )
 
         volumes = Shell.to_cli_args(mounts, sep=":", parent_arg="--bind")
+        print(OmegaConf.to_container(self.mlcube.runner))
+        run_args = self.mlcube.runner.run_args
+
+        # Temporary solution
+        extra_args = self._get_extra_args()
+        if extra_args:
+            run_args += " " + extra_args
+
         try:
             entrypoint: t.Optional[str] = self.mlcube.tasks[self.task].get('entrypoint', None)
             if entrypoint:
                 logger.info(
                     "Using custom task entrypoint: task=%s, entrypoint='%s'",
                     self.task, self.mlcube.tasks[self.task].entrypoint
                 )
-                Shell.run([self.mlcube.runner.singularity, 'exec', self.mlcube.runner.run_args, volumes,
+                Shell.run([self.mlcube.runner.singularity, 'exec', run_args, volumes,
                            str(image_file), entrypoint, ' '.join(task_args[1:])])
             else:
                 Shell.run([
-                    self.mlcube.runner.singularity, 'run', self.mlcube.runner.run_args, volumes,
+                    self.mlcube.runner.singularity, 'run', run_args, volumes,
                     str(image_file), ' '.join(task_args)
                 ])
         except ExecutionError as err:
             raise ExecutionError.mlcube_run_error(
                 self.__class__.__name__,
                 f"Error occurred while running MLCube task (task={self.task}). See context for more details.",
                 **err.context
```

### Comparing `mlcube_singularity-0.0.8/mlcube_singularity/tests/test_config.py` & `mlcube_singularity-0.0.9/mlcube_singularity/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mlcube_singularity-0.0.8/mlcube_singularity/tests/test_singularity_runner.py` & `mlcube_singularity-0.0.9/mlcube_singularity/tests/test_singularity_runner.py`

 * *Files identical despite different names*

### Comparing `mlcube_singularity-0.0.8/mlcube_singularity.egg-info/SOURCES.txt` & `mlcube_singularity-0.0.9/mlcube_singularity.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 mlcube_singularity.egg-info/dependency_links.txt
 mlcube_singularity.egg-info/entry_points.txt
 mlcube_singularity.egg-info/requires.txt
 mlcube_singularity.egg-info/top_level.txt
 mlcube_singularity/tests/__init__.py
 mlcube_singularity/tests/test_config.py
 mlcube_singularity/tests/test_factory_fn.py
-mlcube_singularity/tests/test_mlcommons_box_singularity_cli.py
 mlcube_singularity/tests/test_singularity_runner.py
```

### Comparing `mlcube_singularity-0.0.8/setup.py` & `mlcube_singularity-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 extra_files = schemas()
 
 
 setup(
     name="mlcube_singularity",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     license="Apache 2.0",
     entry_points='''
         [console_scripts]
         mlcube_singularity=mlcube_singularity.__main__:cli
     ''',
     install_requires=requires,
```

