# Comparing `tmp/mlcube-0.0.8.tar.gz` & `tmp/mlcube-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcube-0.0.8.tar", last modified: Wed Sep 21 22:30:26 2022, max compression
+gzip compressed data, was "mlcube-0.0.9.tar", last modified: Mon Apr 17 18:10:18 2023, max compression
```

## Comparing `mlcube-0.0.8.tar` & `mlcube-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:30:26.896939 mlcube-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-21 22:30:26.896939 mlcube-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:30:26.892939 mlcube-0.0.8/mlcube/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16851 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9737 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4583 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)    11018 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/system_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:30:26.896939 mlcube-0.0.8/mlcube/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7007 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/tests/test_mlcommons_mlcube_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-09-21 22:30:19.000000 mlcube-0.0.8/mlcube/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:30:26.896939 mlcube-0.0.8/mlcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-21 22:30:26.000000 mlcube-0.0.8/mlcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-21 22:30:26.000000 mlcube-0.0.8/mlcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:30:26.000000 mlcube-0.0.8/mlcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-21 22:30:26.000000 mlcube-0.0.8/mlcube.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-21 22:30:26.000000 mlcube-0.0.8/mlcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-21 22:30:26.000000 mlcube-0.0.8/mlcube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:30:26.896939 mlcube-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-09-21 22:30:19.000000 mlcube-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:10:18.290923 mlcube-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 18:10:18.290923 mlcube-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:10:18.286923 mlcube-0.0.9/mlcube/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20443 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/system_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:10:18.290923 mlcube-0.0.9/mlcube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/test_mlcommons_mlcube_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-17 18:10:04.000000 mlcube-0.0.9/mlcube/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:10:18.286923 mlcube-0.0.9/mlcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 18:10:18.000000 mlcube-0.0.9/mlcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-17 18:10:18.000000 mlcube-0.0.9/mlcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:10:18.000000 mlcube-0.0.9/mlcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:10:18.000000 mlcube-0.0.9/mlcube.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 18:10:18.000000 mlcube-0.0.9/mlcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 18:10:18.000000 mlcube-0.0.9/mlcube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:10:18.290923 mlcube-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-17 18:10:04.000000 mlcube-0.0.9/setup.py
```

### Comparing `mlcube-0.0.8/mlcube/__main__.py` & `mlcube-0.0.9/mlcube/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,340 +1,513 @@
 """This requires the MLCube 2.0 that's located somewhere in one of dev branches."""
 import logging
 import os
+import shutil
 import sys
 import typing as t
 
 import click
 
 import coloredlogs
 
-from mlcube.config import MLCubeConfig
+from mlcube.parser import CliParser
+from mlcube.cli import (MLCubeCommand, MultiValueOption, Options, parse_cli_args, UsageExamples)
 from mlcube.errors import (ExecutionError, IllegalParameterValueError, MLCubeError)
-from mlcube.parser import (CliParser, MLCubeDirectory)
-from mlcube.platform import Platform
-from mlcube.runner import Runner
 from mlcube.shell import Shell
 from mlcube.system_settings import SystemSettings
-from mlcube.validate import Validate
 
-from omegaconf import (DictConfig, OmegaConf)
+from omegaconf import OmegaConf
 
 logger = logging.getLogger(__name__)
 
-
-class MultiValueOption(click.Option):
-    def __init__(self, *args, **kwargs) -> None:
-        super(MultiValueOption, self).__init__(*args, **kwargs)
-        self._previous_parser_process: t.Optional[t.Callable] = None
-        self._eat_all_parser: t.Optional[click.parser.Option] = None
-
-    def add_to_parser(self, parser: click.parser.OptionParser, ctx: click.core.Context):
-
-        def parser_process(value: str, state: click.parser.ParsingState):
-            values: t.List[str] = [value]
-            prefixes: t.Tuple[str] = tuple(self._eat_all_parser.prefixes)
-            while state.rargs:
-                if state.rargs[0].startswith(prefixes):
-                    break
-                values.append(state.rargs.pop(0))
-            self._previous_parser_process(tuple(values), state)
-
-        super(MultiValueOption, self).add_to_parser(parser, ctx)
-        for opt_name in self.opts:
-            our_parser: t.Optional[click.parser.Option] = \
-                parser._long_opt.get(opt_name) or parser._short_opt.get(opt_name)
-            if our_parser:
-                self._eat_all_parser = our_parser
-                self._previous_parser_process = our_parser.process
-                our_parser.process = parser_process
-                break
+_TERMINAL_WIDTH = shutil.get_terminal_size()[0]   # Since Python version 3.3
+"""Width of a user terminal. MLCube overrides default (80) character width to make usage examples look better."""
 
 
-def _parse_cli_args(ctx: t.Optional[click.core.Context], mlcube: str, platform: t.Optional[str],
-                    workspace: t.Optional[str],
-                    resolve: bool) -> t.Tuple[t.Optional[t.Type[Runner]], DictConfig]:
-    """Parse command line arguments.
+def add_to_parser(self, parser: click.parser.OptionParser, ctx: click.core.Context):
+    def parser_process(value: str, state: click.parser.ParsingState):
+        values: t.List[str] = [value]
+        prefixes: t.Tuple[str] = tuple(self._eat_all_parser.prefixes)
+        while state.rargs:
+            if state.rargs[0].startswith(prefixes):
+                break
+            values.append(state.rargs.pop(0))
+        self._previous_parser_process(tuple(values), state)
 
-    Args:
-        ctx: Click context. We need this to get access to extra CLI arguments.
-        mlcube: Path to MLCube root directory or mlcube.yaml file.
-        platform: Platform to use to run this MLCube (docker, singularity, gcp, k8s etc).
-        workspace: Workspace path to use. If not specified, default workspace inside MLCube directory is used.
-        resolve: if True, compute values in MLCube configuration.
-    """
-    mlcube_inst: MLCubeDirectory = CliParser.parse_mlcube_arg(mlcube)
-    Validate.validate_type(mlcube_inst, MLCubeDirectory)
-    if ctx is not None:
-        mlcube_cli_args, task_cli_args = CliParser.parse_extra_arg(*ctx.args)
-    else:
-        mlcube_cli_args, task_cli_args = None, None
-    if platform is not None:
-        system_settings = SystemSettings()
-        runner_config: t.Optional[DictConfig] = system_settings.get_platform(platform)
-        runner_cls: t.Optional[t.Type[Runner]] = Platform.get_runner(
-            system_settings.runners.get(runner_config.runner, None)
-        )
-    else:
-        runner_cls, runner_config = None, None
-    mlcube_config = MLCubeConfig.create_mlcube_config(
-        os.path.join(mlcube_inst.path, mlcube_inst.file), mlcube_cli_args, task_cli_args, runner_config, workspace,
-        resolve=resolve, runner_cls=runner_cls
-    )
-    return runner_cls, mlcube_config
+    super(MultiValueOption, self).add_to_parser(parser, ctx)
+    for opt_name in self.opts:
+        our_parser: t.Optional[click.parser.Option] = parser._long_opt.get(
+            opt_name
+        ) or parser._short_opt.get(opt_name)
+        if our_parser:
+            self._eat_all_parser = our_parser
+            self._previous_parser_process = our_parser.process
+            our_parser.process = parser_process
+            break
 
 
 log_level_option = click.option(
-    '--log-level', '--log_level', required=False, type=str, default='warning',
-    help="Log level to set, default is to do nothing."
+    "--log-level",
+    "--log_level",
+    required=False,
+    type=str,
+    default="warning",
+    help="Log level to set, default is to do nothing.",
 )
 mlcube_option = click.option(
-    '--mlcube', required=False, type=str, default=os.getcwd(),
+    "--mlcube",
+    required=False,
+    type=str,
+    default=os.getcwd(),
     help="Path to MLCube. This can be either a directory path that becomes MLCube's root directory, or path to MLCube"
-         "definition file (.yaml). In the latter case the MLCube's root directory becomes parent directory of the yaml"
-         "file. Default is current directory."
+    "definition file (.yaml). In the latter case the MLCube's root directory becomes parent directory of the yaml"
+    "file. Default is current directory.",
 )
 platform_option = click.option(
-    '--platform', required=False, type=str, default='docker',
-    help="Platform to run MLCube, default is 'docker' (that also supports podman)."
+    "--platform",
+    required=False,
+    type=str,
+    default="docker",
+    help="Platform to run MLCube, default is 'docker' (that also supports podman).",
 )
 task_option = click.option(
-    '--task', required=False, type=str, default=None,
+    "--task",
+    required=False,
+    type=str,
+    default=None,
     help="MLCube task name(s) to run, default is `main`. This parameter can take a list value, in which case task names"
-         "are separated with ','."
+    "are separated with ','.",
 )
 workspace_option = click.option(
-    '--workspace', required=False, type=str, default=None,
-    help="Workspace location that is used to store input/output artifacts of MLCube tasks."
+    "--workspace",
+    required=False,
+    type=str,
+    default=None,
+    help="Workspace location that is used to store input/output artifacts of MLCube tasks.",
+)
+network_option = click.option(
+    "--network",
+    required=False,
+    type=str,
+    default=None,
+    help="Networking options defined during MLCube container execution.",
+)
+security_option = click.option(
+    "--security",
+    required=False,
+    type=str,
+    default=None,
+    help="Security options defined during MLCube container execution.",
+)
+gpus_option = click.option(
+    "--gpus",
+    required=False,
+    type=str,
+    default=None,
+    help="GPU usage options defined during MLCube container execution.",
+)
+memory_option = click.option(
+    "--memory",
+    required=False,
+    type=str,
+    default=None,
+    help="Memory RAM options defined during MLCube container execution.",
+)
+cpu_option = click.option(
+    "--cpu",
+    required=False,
+    type=str,
+    default=None,
+    help="CPU options defined during MLCube container execution.",
 )
 
+@click.group(name='mlcube', add_help_option=False)
+@Options.loglevel
+@Options.help
+def cli(log_level: t.Optional[str]):
+    """MLCube 📦 is a tool for packaging, distributing and running Machine Learning (ML) projects and models.
+
+    \b
+    - GitHub: https://github.com/mlcommons/mlcube
+    - Documentation: https://mlcommons.github.io/mlcube/
+    - Example MLCubes: https://github.com/mlcommons/mlcube_examples
+    """
 
-@click.group(name='mlcube', help="MLCube 📦 is a packaging tool for ML models")
-@log_level_option
-def cli(log_level: str):
     if log_level:
         log_level = log_level.upper()
         logging.basicConfig(level=log_level)
         coloredlogs.install(level=log_level)
         logging.info("Setting Log Level from CLI argument to '%s'.", log_level)
     _ = SystemSettings().update_installed_runners()
 
 
-@cli.command(name='show_config', help='Show MLCube configuration.',
-             context_settings={'ignore_unknown_options': True, 'allow_extra_args': True})
-@mlcube_option
-@platform_option
-@workspace_option
-@click.option('--resolve', is_flag=True, help="Resolve MLCube parameters.")
+@cli.command(
+    name='show_config', cls=MLCubeCommand, add_help_option=False, epilog=UsageExamples.show_config,
+    context_settings={'ignore_unknown_options': True, 'allow_extra_args': True, 'max_content_width': _TERMINAL_WIDTH}
+)
+@Options.mlcube
+@Options.platform
+@Options.workspace
+@Options.resolve
+@Options.parameter
+@Options.help
 @click.pass_context
-def show_config(ctx: click.core.Context, mlcube: str, platform: str, workspace: str, resolve: bool) -> None:
-    """Show MLCube configuration.
+def show_config(ctx: click.core.Context, mlcube: t.Optional[str], platform: str, workspace: str,
+                resolve: bool, p: t.Tuple[str]) -> None:
+    """Show effective MLCube configuration.
+
+    Effective MLCube configuration is the one used by one of MLCube runners to run this MLCube. This configuration is
+    built by merging (1) default runner configuration retrieved from system settings, (2) MLCube project configuration
+    and (3) configuration parameters passed by a user on a command line (CONFIG_PARAM).
 
+    \f
     Args:
-        ctx: Click context. We need this to get access to extra CLI arguments.
+        ctx: Click context for unknown options
         mlcube: Path to MLCube root directory or mlcube.yaml file.
         platform: Platform to use to run this MLCube (docker, singularity, gcp, k8s etc).
         workspace: Workspace path to use. If not specified, default workspace inside MLCube directory is used.
         resolve: if True, compute values in MLCube configuration.
+        p: Additional configuration parameters.
     """
-    _, mlcube_config = _parse_cli_args(ctx, mlcube, platform, workspace, resolve)
+    if mlcube is None:
+        mlcube = os.getcwd()
+    _, mlcube_config = parse_cli_args(
+        unparsed_args=ctx.args + ['-P' + param for param in p],
+        parsed_args={"mlcube": mlcube, "platform": platform, "workspace": workspace},
+        resolve=resolve
+    )
     print(OmegaConf.to_yaml(mlcube_config))
 
 
-@cli.command(name='configure', help='Configure MLCube.',
-             context_settings={'ignore_unknown_options': True, 'allow_extra_args': True})
-@mlcube_option
-@platform_option
-@click.pass_context
-def configure(ctx: click.core.Context, mlcube: str, platform: str) -> None:
+@cli.command(
+    name='configure', cls=MLCubeCommand, add_help_option=False, epilog=UsageExamples.configure,
+    context_settings={'ignore_unknown_options': True, 'allow_extra_args': True, 'max_content_width': _TERMINAL_WIDTH}
+)
+@Options.mlcube
+@Options.platform
+@Options.parameter
+@Options.help
+def configure(mlcube: t.Optional[str], platform: str, p: t.Tuple[str]) -> None:
     """Configure MLCube.
 
+    Some MLCube projects need to be configured first. For instance, docker-based MLCubes distributed via GitHub with
+    source code most likely will provide a `Dockerfile` to build a docker image. In this case, the process of building
+    a docker image before MLCube runner can run it, is called a configuration phase. In general, users do not need to
+    run this command manually - MLCube runners should be able to figure out when they need to run it, and will run it
+    as part of `mlcube run` command.
+
+    \f
     Args:
-        ctx: Click context. We need this to get access to extra CLI arguments.
         mlcube: Path to MLCube root directory or mlcube.yaml file.
         platform: Platform to use to configure this MLCube for (docker, singularity, gcp, k8s etc).
+        p: Additional MLCube configuration parameters (these parameters are those parameters that normally start with
+            `-P` prefix). Here, due to original implementation, we need to `unparse` by adding `-P` prefix.
     """
+    logger.debug("mlcube::configure, mlcube=%s, platform=%s, p=%s", mlcube, platform, str(p))
+    if mlcube is None:
+        mlcube = os.getcwd()
     logger.info("Configuring MLCube (`%s`) for `%s` platform.", os.path.abspath(mlcube), platform)
     try:
-        runner_cls, mlcube_config = _parse_cli_args(ctx, mlcube, platform, workspace=None, resolve=True)
+        runner_cls, mlcube_config = parse_cli_args(
+            unparsed_args=['-P' + param for param in p],
+            parsed_args={"mlcube": mlcube, "platform": platform},
+            resolve=True
+        )
         runner = runner_cls(mlcube_config, task=None)
         runner.configure()
     except MLCubeError as err:
-        exit_code = err.context.get('code', 1) if isinstance(err, ExecutionError) else 1
+        exit_code = err.context.get("code", 1) if isinstance(err, ExecutionError) else 1
         logger.exception(f"Failed to configure MLCube with error code {exit_code}.")
         if isinstance(err, ExecutionError):
             print(err.describe())
         sys.exit(exit_code)
-    logger.info("MLCube (%s) has been successfully configured for `%s` platform.", os.path.abspath(mlcube), platform)
+    logger.info(
+        "MLCube (%s) has been successfully configured for `%s` platform.",
+        os.path.abspath(mlcube),
+        platform,
+    )
 
 
-@cli.command(name='run', help='Run MLCube ML task.',
-             context_settings={'ignore_unknown_options': True, 'allow_extra_args': True})
+@cli.command(
+    name='run', cls=MLCubeCommand, add_help_option=False, epilog=UsageExamples.run,
+    context_settings={'ignore_unknown_options': True, 'allow_extra_args': True, 'max_content_width': _TERMINAL_WIDTH}
+)
 @mlcube_option
 @platform_option
 @task_option
 @workspace_option
+@network_option
+@security_option
+@gpus_option
+@memory_option
+@cpu_option
+@Options.help
 @click.pass_context
-def run(ctx: click.core.Context, mlcube: str, platform: str, task: str, workspace: str) -> None:
+def run(
+    ctx: click.core.Context,
+    mlcube: str,
+    platform: str,
+    task: str,
+    workspace: str,
+    network: str,
+    security: str,
+    gpus: str,
+    memory: str,
+    cpu: str,
+) -> None:
     """Run MLCube task(s).
 
+    \f
     Args:
-        ctx: Click context. We need this to get access to extra CLI arguments.
+        ctx: Click context for unknown options
         mlcube: Path to MLCube root directory or mlcube.yaml file.
         platform: Platform to use to run this MLCube (docker, singularity, gcp, k8s etc).
         task: Comma separated list of tasks to run.
         workspace: Workspace path to use. If not specified, default workspace inside MLCube directory is used.
+        network: Networking options defined during MLCube container execution.
+        security: Security options defined during MLCube container execution.
+        gpus: GPU usage options defined during MLCube container execution.
+        memory: Memory RAM options defined during MLCube container execution.
+        cpu: CPU options defined during MLCube container execution.
     """
-    runner_cls, mlcube_config = _parse_cli_args(ctx, mlcube, platform, workspace, resolve=True)
-    mlcube_tasks: t.List[str] = list((mlcube_config.get('tasks', None) or {}).keys())  # Tasks in this MLCube.
-    tasks: t.List[str] = CliParser.parse_list_arg(task, default=None)                  # Requested tasks.
+    runner_cls, mlcube_config = parse_cli_args(
+        unparsed_args=ctx.args,
+        parsed_args={
+            "mlcube": mlcube, "platform": platform, "workspace": workspace,
+            "network": network, "security": security, "gpus": gpus, "memory": memory, "cpu": cpu
+        },
+        resolve=True
+    )
+    mlcube_tasks: t.List[str] = list(
+        (mlcube_config.get("tasks", None) or {}).keys()
+    )  # Tasks in this MLCube.
+    tasks: t.List[str] = CliParser.parse_list_arg(
+        task, default=None
+    )  # Requested tasks.
 
     if len(tasks) == 0:
-        logger.warning("Missing required task name (--task=COMMA_SEPARATED_LIST_OF_TASK_NAMES).")
+        logger.warning(
+            "Missing required task name (--task=COMMA_SEPARATED_LIST_OF_TASK_NAMES)."
+        )
         if len(mlcube_tasks) != 1:
-            logger.error("Task name could not be automatically resolved (supported tasks = %s).", str(mlcube_tasks))
+            logger.error(
+                "Task name could not be automatically resolved (supported tasks = %s).",
+                str(mlcube_tasks),
+            )
             exit(1)
-        logger.info("Task name has been automatically resolved to %s (supported tasks = %s).",
-                    mlcube_tasks[0], str(mlcube_tasks))
+        logger.info(
+            "Task name has been automatically resolved to %s (supported tasks = %s).",
+            mlcube_tasks[0],
+            str(mlcube_tasks),
+        )
         tasks = mlcube_tasks
 
     unknown_tasks: t.List[str] = [name for name in tasks if name not in mlcube_tasks]
     if len(unknown_tasks) > 0:
-        logger.error("Unknown tasks have been requested: supported tasks = %s, requested tasks = %s, "
-                     "unknown tasks = %s.", str(mlcube_tasks), str(tasks), str(unknown_tasks))
+        logger.error(
+            "Unknown tasks have been requested: supported tasks = %s, requested tasks = %s, "
+            "unknown tasks = %s.",
+            str(mlcube_tasks),
+            str(tasks),
+            str(unknown_tasks),
+        )
         exit(1)
 
     try:
         # TODO: Sergey - Can we have one instance for all tasks?
         for task in tasks:
             logger.info("Task = %s", task)
             runner = runner_cls(mlcube_config, task=task)
             runner.run()
     except MLCubeError as err:
-        exit_code = err.context.get('code', 1) if isinstance(err, ExecutionError) else 1
+        exit_code = err.context.get("code", 1) if isinstance(err, ExecutionError) else 1
         logger.exception(f"Failed to run MLCube with error code {exit_code}.")
         if isinstance(err, ExecutionError):
             print(err.describe())
         sys.exit(exit_code)
 
 
-@cli.command(name='describe', help='Describe MLCube.')
-@mlcube_option
-def describe(mlcube: str) -> None:
+@cli.command(
+    name='describe', cls=MLCubeCommand, add_help_option=False, epilog=UsageExamples.describe,
+    context_settings={'max_content_width': _TERMINAL_WIDTH}
+)
+@Options.mlcube
+@Options.help
+def describe(mlcube: t.Optional[str]) -> None:
     """Describe this MLCube.
 
+    \f
     Args:
         mlcube: Path to MLCube root directory or mlcube.yaml file.
     """
-    _, mlcube_config = _parse_cli_args(None, mlcube, None, None, resolve=True)
+    if mlcube is None:
+        mlcube = os.getcwd()
+    _, mlcube_config = parse_cli_args(
+        unparsed_args=[],
+        parsed_args={"mlcube": mlcube},
+        resolve=True
+    )
     print("MLCube")
     print(f"  path = {mlcube_config.runtime.root}")
     print(f"  name = {mlcube_config.name}:{mlcube_config.get('version', 'latest')}")
     print()
     print(f"  workspace = {mlcube_config.runtime.workspace}")
     print(f"  system settings = {SystemSettings.system_settings_file()}")
     print()
     print("  Tasks:")
     for task_name, task_def in mlcube_config.tasks.items():
         description = f"name = {task_name}"
         if len(task_def.parameters.inputs) > 0:
-            description = f"{description}, inputs = {list(task_def.parameters.inputs.keys())}"
+            description = (
+                f"{description}, inputs = {list(task_def.parameters.inputs.keys())}"
+            )
         if len(task_def.parameters.outputs) > 0:
-            description = f"{description}, outputs = {list(task_def.parameters.outputs.keys())}"
+            description = (
+                f"{description}, outputs = {list(task_def.parameters.outputs.keys())}"
+            )
         print(f"    {description}")
     print()
     print("Run this MLCube:")
     print("  Configure MLCube:")
-    print(f"    mlcube configure --mlcube={mlcube_config.runtime.root} --platform=docker")
+    print(
+        f"    mlcube configure --mlcube={mlcube_config.runtime.root} --platform=docker"
+    )
     print("  Run MLCube tasks:")
     for task_name in mlcube_config.tasks.keys():
-        print(f"    mlcube run --mlcube={mlcube_config.runtime.root} --task={task_name} --platform=docker")
+        print(
+            f"    mlcube run --mlcube={mlcube_config.runtime.root} --task={task_name} --platform=docker"
+        )
     print()
 
 
-@cli.command(name='config', help='Perform various operations with system settings file.',
-             context_settings={'ignore_unknown_options': True, 'allow_extra_args': True})
-@click.option('--list', 'list_all', is_flag=True, help="List configuration in MLCube system settings file.")
-@click.option('--get', required=False, type=str, default=None,
-              help="Return value of the key (use OmegaConf notation, e.g. --get runners.docker).")
-@click.option('--create_platform', '--create-platform', required=False, cls=MultiValueOption, type=tuple, default=None,
-              help="Create a new platform instance for this runner")
-@click.option('--remove_platform', '--remove-platform', required=False, type=str, default=None,
-              help="Remove this platform from list of platforms in system settings file.")
-@click.option('--rename_platform', '--rename-platform', required=False, cls=MultiValueOption, type=tuple, default=None,
-              help="Rename existing platform. If default platform is to be renamed (like docker), it will be recreated "
-                   "(with default values) next time mlcube runs")
-@click.option('--copy_platform', '--copy-platform', required=False, cls=MultiValueOption, type=tuple, default=None,
-              help="Copy existing platform.")
-@click.option('--rename_runner', '--rename-runner', required=False, cls=MultiValueOption, type=tuple, default=None,
-              help="Rename existing runner. If platforms exist that reference this runner, users must explicitly "
-                   "provide `--update-platforms` flag to confirm they want to update platforms' description too.")
-@click.option('--remove_runner', '--remove-runner', required=False, type=str, default=None,
-              help="Remove existing runner from the list. If platforms exist that reference this runner, users must "
-                   "explicitly provide `--remove-platforms` flag to confirm they want to remove platforms too.")
+@cli.command(
+    name='config', cls=MLCubeCommand, add_help_option=False, epilog=UsageExamples.config,
+    context_settings={'ignore_unknown_options': True, 'allow_extra_args': True, 'max_content_width': _TERMINAL_WIDTH}
+)
+@click.option(
+    '--list', 'list_all', is_flag=True,
+    help="Print out the content of system settings file."
+)
+@click.option(
+    '--get', required=False, type=str, default=None,
+    help="Return value of the key (use OmegaConf notation, e.g. `mlcube config --get runners.docker`)."
+)
+@click.option(
+    '--create_platform', '--create-platform', required=False, cls=MultiValueOption, type=tuple, default=None,
+    help="Create a new platform instance for this runner. Default runner parameters are used to initialize this new "
+         "platform."
+)
+@click.option(
+    '--remove_platform', '--remove-platform', required=False, type=str, default=None,
+    help="Remove this platform. If this is one of the default platforms (e.g., `docker`), it will be recreated (with "
+         "default values) next time `mlcube` runs."
+)
+@click.option(
+    '--rename_platform', '--rename-platform', required=False, cls=MultiValueOption, type=tuple, default=None,
+    help="Rename existing platform. If default platform is to be renamed (e.g., `docker`), it will be recreated "
+         "(with default values) next time `mlcube` runs."
+)
+@click.option(
+    '--copy_platform', '--copy-platform', required=False, cls=MultiValueOption, type=tuple, default=None,
+    help="Copy existing platform. This can be useful for creating new platforms off existing platforms, for instance,"
+         "creating a new SSH runner configuration that runs MLCubes on a new remote server."
+)
+@click.option(
+    '--rename_runner', '--rename-runner', required=False, cls=MultiValueOption, type=tuple, default=None,
+    help="Rename existing MLCube runner. If platforms exist that reference this runner, users must explicitly provide "
+         "`--update-platforms` flag to confirm they want to update platforms' description too."
+)
+@click.option(
+    '--remove_runner', '--remove-runner', required=False, type=str, default=None,
+    help="Remove existing runner. If platforms exist that reference this runner, users must explicitly provide "
+         "`--remove-platforms` flag to confirm they want to remove platforms too."
+)
+@Options.help
 @click.pass_context
 def config(ctx: click.core.Context,
            list_all: bool,                          # mlcube config --list
            get: t.Optional[str],                    # mlcube config --get KEY
            create_platform: t.Optional[t.Tuple],    # mlcube config --create-platform RUNNER PLATFORM
            remove_platform: t.Optional[str],        # mlcube config --remove-platform NAME
            rename_platform: t.Optional[t.Tuple],    # mlcube config --rename-platform OLD_NAME NEW_NAME
            copy_platform: t.Optional[t.Tuple],      # mlcube config --copy-platform EXISTING_PLATFORM NEW_PLATFORM
            rename_runner: t.Optional[t.Tuple],      # mlcube config --rename-runner OLD_NAME NEW_NAME
            remove_runner: t.Optional[str]           # mlcube config --remove-runner NAME
            ) -> None:
-    """Work with MLCube system settings (similar to `git config`)."""
+    """Work with MLCube [system settings](https://mlcommons.github.io/mlcube/getting-started/system-settings/) similar
+    to `git config`.
+
+    Manage MLCube system settings (these settings define global configuration common for all MLCube runners and
+    platforms). When this command runs without arguments, a path to system settings file is printed out. This is useful
+    to automate certain operations with system settings. Alternatively, it may be easier to manipulate system settings
+    file directly (it is a yaml file).
+    """
     print(f"System settings file path = {SystemSettings.system_settings_file()}")
     settings = SystemSettings()
 
-    def _check_tuple(_tuple: t.Tuple, _name: str, _expected_size: int, _expected_value: str) -> None:
+    def _check_tuple(
+        _tuple: t.Tuple, _name: str, _expected_size: int, _expected_value: str
+    ) -> None:
         if len(_tuple) != _expected_size:
-            raise IllegalParameterValueError(f'--{_name}', ' '.join(_tuple), f"\"{_expected_value}\"")
+            raise IllegalParameterValueError(
+                f"--{_name}", " ".join(_tuple), f'"{_expected_value}"'
+            )
 
     try:
         if list_all:
             print(OmegaConf.to_yaml(settings.settings))
         elif get:
             print(OmegaConf.to_yaml(OmegaConf.select(settings.settings, get)))
         elif create_platform:
-            _check_tuple(create_platform, 'create_platform', 2, 'RUNNER_NAME PLATFORM_NAME')
+            _check_tuple(
+                create_platform, "create_platform", 2, "RUNNER_NAME PLATFORM_NAME"
+            )
             settings.create_platform(create_platform)
         elif remove_platform:
             settings.remove_platform(remove_platform)
         elif rename_platform:
-            _check_tuple(rename_platform, 'rename_platform', 2, 'OLD_NAME NEW_NAME')
+            _check_tuple(rename_platform, "rename_platform", 2, "OLD_NAME NEW_NAME")
             settings.copy_platform(rename_platform, delete_source=True)
         elif copy_platform:
-            _check_tuple(copy_platform, 'copy_platform', 2, 'EXISTING_PLATFORM NEW_PLATFORM')
+            _check_tuple(
+                copy_platform, "copy_platform", 2, "EXISTING_PLATFORM NEW_PLATFORM"
+            )
             settings.copy_platform(rename_platform, delete_source=False)
         elif rename_runner:
-            _check_tuple(rename_runner, 'rename_runner', 2, 'OLD_NAME NEW_NAME')
-            update_platforms: bool = '--update-platforms' in ctx.args or '--update_platforms' in ctx.args
+            _check_tuple(rename_runner, "rename_runner", 2, "OLD_NAME NEW_NAME")
+            update_platforms: bool = "--update-platforms" in ctx.args or "--update_platforms" in ctx.args
             settings.rename_runner(rename_runner, update_platforms=update_platforms)
         elif remove_runner:
-            remove_platforms: bool = '--remove-platforms' in ctx.args or '--remove_platforms' in ctx.args
+            remove_platforms: bool = "--remove-platforms" in ctx.args or "--remove_platforms" in ctx.args
             settings.remove_runner(remove_runner, remove_platforms=remove_platforms)
     except MLCubeError as e:
-        logger.error("Command failed, command = '%s' error = '%s'", ' '.join(sys.argv), str(e))
+        logger.error(
+            "Command failed, command = '%s' error = '%s'", " ".join(sys.argv), str(e)
+        )
 
 
-@cli.command(name='create',
-             help='Create a new MLCube using cookiecutter.')
+@cli.command(
+    name='create', add_help_option=False, cls=MLCubeCommand, epilog=UsageExamples.create,
+    context_settings={'max_content_width': _TERMINAL_WIDTH}
+)
+@Options.help
 def create() -> None:
-    """Create a new MLCube using cookiecutter template.
+    """Create a new Python project from the MLCube cookiecutter template.
 
-    - MLCube cookiecutter: https://github.com/mlcommons/mlcube_cookiecutter
-    - Example: https://mlcommons.github.io/mlcube/tutorials/create-mlcube/
+    MLCube uses the [cookiecutter](https://cookiecutter.readthedocs.io/) library with the
+    [mlcube_cookiecutter](https://github.com/mlcommons/mlcube_cookiecutter) template. The library is not installed
+    automatically: install it with `pip install cookiecutter`.
     """
-    mlcube_cookiecutter_url = 'https://github.com/mlcommons/mlcube_cookiecutter'
+    mlcube_cookiecutter_url = "https://github.com/mlcommons/mlcube_cookiecutter"
     try:
         from cookiecutter.main import cookiecutter
+
         proj_dir: str = cookiecutter(mlcube_cookiecutter_url)
-        if proj_dir and os.path.isfile(os.path.join(proj_dir, 'mlcube.yaml')):
-            Shell.run(['mlcube', 'describe', '--mlcube', proj_dir], on_error='die')
+        if proj_dir and os.path.isfile(os.path.join(proj_dir, "mlcube.yaml")):
+            Shell.run(["mlcube", "describe", "--mlcube", proj_dir], on_error="die")
     except ImportError:
         print("Cookiecutter library not found.")
         print("\tInstall it: pip install cookiecutter")
         print(f"\tMore details: {mlcube_cookiecutter_url}")
 
 
 if __name__ == "__main__":
```

### Comparing `mlcube-0.0.8/mlcube/config.py` & `mlcube-0.0.9/mlcube/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from mlcube.runner import Runner
 
 from omegaconf import (DictConfig, OmegaConf)
 
 
 logger = logging.getLogger(__name__)
 
-__all__ = ['IOType', 'ParameterType', 'MLCubeConfig']
+__all__ = ['IOType', 'ParameterType', 'MountType', 'MLCubeConfig']
 
 
 class IOType(object):
     """Input/output type of MLCube task parameter."""
 
     INPUT = 'input'
     """This parameter is input parameter (e.g., path to data)."""
@@ -99,19 +99,24 @@
                              runner_cls: t.Optional[t.Type[Runner]] = None) -> DictConfig:
         """Create MLCube configuration merging different configs - base, global, local and cli.
 
         Args:
             mlcube_config_file: Path to mlcube.yaml file.
             mlcube_cli_args: MLCube parameters from command line.
             task_cli_args: Task parameters from command line.
-            runner_config: MLCube runner configuration, usually comes from system settings file.
+            runner_config: MLCube runner configuration from system settings file. Can theoretically be None if
+                runner (or, to be more correct, associated platform instance) is not specified in system settings. If
+                None, empty config will be used.
             workspace: Workspace path to use in this MLCube run.
             resolve: If true, compute all values (some of them may reference other parameters or environmental
                 variables).
-            runner_cls: A python class for the runner type specified in `runner_config`.
+            runner_cls: A python class for the runner type specified in `runner_config`. Can also be None if no runner
+                is specified in system settings (see `runner_config` above). If not None, we'll use it to get parameters
+                not present in system settings (e.g., outdated version)and to validate to overall configuration.
+                TODO: This class should also be used to do runner-specific parsing of input parameters.
         """
         if mlcube_cli_args is None:
             mlcube_cli_args = OmegaConf.create({})
         if task_cli_args is None:
             task_cli_args = {}
         if runner_config is None:
             runner_config = OmegaConf.create({})
@@ -120,31 +125,36 @@
         logger.debug("task_cli_args = %s", task_cli_args)
         logger.debug("runner_config = %s", str(runner_config))
         logger.debug("workspace = %s", workspace)
 
         # Load MLCube configuration and maybe override parameters from command line (like -Pdocker.build_strategy=...).
         actual_workspace = '${runtime.root}/workspace' if workspace is None else MLCubeConfig.get_uri(workspace)
         mlcube_config = OmegaConf.merge(
-            OmegaConf.load(mlcube_config_file),
-            mlcube_cli_args,
-            OmegaConf.create({
+            OmegaConf.load(mlcube_config_file),                     # MLCube configuration file.
+            mlcube_cli_args,                                        # MLCube parameters from command line.
+            OmegaConf.create({                                      # Section defining runtime parameters.
                 'runtime': {
                     'root': os.path.dirname(mlcube_config_file),
                     'workspace': actual_workspace
                 },
-                'runner': runner_config
+                'runner': runner_config                             # Effective (final) runner configuration.
             })
         )
         # Maybe this is not the best idea, but originally MLCube used $WORKSPACE token to refer to the internal
         # workspace. So, this value is here to simplify access to workspace value. BTW, in general, if files are to be
         # located inside workspace (internal or custom), users are encouraged not to use ${runtime.workspace} or
         # ${workspace} in their MLCube configuration files.
         mlcube_config['workspace'] = actual_workspace
         # Merge, for instance, docker runner config from system settings with docker config from MLCube config.
         if runner_cls:
+            # Make sure all default parameters are present - this can be done automatically for all runners (so that
+            # those runners do not check if certain fields are present).
+            MLCubeConfig.merge_with_logging(mlcube_config, runner_cls.CONFIG.DEFAULT)
+            # The goal is to take runner-specific parameters from MLCube config and merge them into `runner` section.
+            # This maybe runner-specific, so runners are responsible for this.
             runner_cls.CONFIG.merge(mlcube_config)
         # Need to apply CLI arguments again just in case users provided something like -Prunner.build_strategy=...
         mlcube_config = OmegaConf.merge(mlcube_config, mlcube_cli_args)
         if runner_cls:
             runner_cls.CONFIG.validate(mlcube_config)
 
         for task_name in mlcube_config.tasks.keys():
@@ -162,22 +172,57 @@
             MLCubeConfig.check_parameters(outputs, task_cli_args)
 
         if resolve:
             OmegaConf.resolve(mlcube_config)
         return mlcube_config
 
     @staticmethod
+    def merge_with_logging(mlcube_config: DictConfig, default_runner_config: DictConfig) -> None:
+        """Merge default runner config with current effective runner config.
+
+        The goal is to make sure the effective configuration contains all parameters accepted by the runner so that this
+        runner does not need to check if certain parameters are present.
+
+        Args:
+             mlcube_config: Current effective MLCube configuration.
+             default_runner_config: Default runner configuration.
+        """
+        params_to_merge = [k for k in default_runner_config.keys() if k not in mlcube_config['runner']]
+        if params_to_merge:
+            logger.warning(
+                "Default runner config contains parameters that are not present in the effective runner config "
+                "(params=%s). This probably means that a new version of a runner was installed that introduced "
+                "new parameters.",
+                str(params_to_merge)
+            )
+            current_effective_cfg = mlcube_config['runner']
+            mlcube_config["runner"] = default_runner_config.copy()
+            mlcube_config.merge_with({'runner': current_effective_cfg})
+
+    @staticmethod
     def check_parameters(parameters: DictConfig, task_cli_args: t.Dict) -> None:
         """Check that task parameters are defined according to MLCube schema.
 
         Args:
             parameters: Task parameters (`inputs` or `outputs`).
             task_cli_args: Task parameters from command line.
         This function does not set `type` of parameters (if not present) in all cases.
         """
+        # Path separators that users can use in the MLCube configuration files. This function uses the presence of
+        # a path separator at the end of the parameter value as a hint that the type of this parameter is a directory
+        # (when not specified by a user). We should not relly on `os.sep` since MLCubes are expected to run in different
+        # environments (e.g., Unix and Windows).
+        separators = ('/', '\\')
+        if os.sep not in separators:
+            logger.warning("The os-specific path separator ('%s') not in list of standard separators.", os.sep)
+        if os.altsep is not None and os.altsep not in separators:
+            logger.warning(
+                "The os-specific alternative path separator ('%s') not in list of standard separators.", os.altsep
+            )
+        #
         for name in parameters.keys():
             # The `_param_name` is anyway there, so check it's not None.
             [param_def] = MLCubeConfig.ensure_values_exist(parameters, name, dict)
             # Deal with the case when value is a string (default value).
             if isinstance(param_def, str):
                 parameters[name] = {'default': param_def}
                 param_def = parameters[name]
@@ -185,24 +230,24 @@
             _ = MLCubeConfig.ensure_values_exist(param_def, 'default', lambda: name)
             # One challenge is how to identify type (file, directory) of input/output parameters if users have
             # not provided these types. The below is a kind of rule-based system that tries to infer types.
 
             # Make sure every parameter definition contains 'type' field. Also, if it's unknown, we can assume it's a
             # directory if a value ends with forward/backward slash.
             _ = MLCubeConfig.ensure_values_exist(param_def, 'type', lambda: ParameterType.UNKNOWN)
-            if param_def.type == ParameterType.UNKNOWN and param_def.default.endswith(os.sep):
+            if param_def.type == ParameterType.UNKNOWN and param_def.default.endswith(separators):
                 param_def.type = ParameterType.DIRECTORY
             # See if there is value on a command line
             param_def.default = task_cli_args.get(name, param_def.default)
             # Check again parameter type. Users in certain number of cases will not be providing final slash on a
             # command line for directories, so we tried to infer types above using default values. Just in case, see
             # if we can do the same with user-provided values.
             # TODO: what if a parameter in mlcube.yaml is declared to be a file, but users provided something with
             #       slash at the end.
-            if param_def.type == ParameterType.UNKNOWN and param_def.default.endswith(os.sep):
+            if param_def.type == ParameterType.UNKNOWN and param_def.default.endswith(separators):
                 param_def.type = ParameterType.DIRECTORY
 
             # TODO: For some input parameters, that generally speaking must exist, we can figure out types later,
             #       when we actually use them (in one of the runners). One problem is when inputs are optional. In this
             #       case, we need to know their type in advance.
 
             # It probably does not make too much sense to see, let's say, if an input parameter exists and set its
```

### Comparing `mlcube-0.0.8/mlcube/errors.py` & `mlcube-0.0.9/mlcube/errors.py`

 * *Files identical despite different names*

### Comparing `mlcube-0.0.8/mlcube/platform.py` & `mlcube-0.0.9/mlcube/platform.py`

 * *Files identical despite different names*

### Comparing `mlcube-0.0.8/mlcube/runner.py` & `mlcube-0.0.9/mlcube/runner.py`

 * *Files identical despite different names*

### Comparing `mlcube-0.0.8/mlcube/shell.py` & `mlcube-0.0.9/mlcube/shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -134,86 +134,138 @@
             source: Source directory.
             dest: Destination directory.
             on_error: Action to perform if an error occurs.
         """
         return Shell.run(f"rsync -e 'ssh' '{source}' '{dest}'", on_error=on_error)
 
     @staticmethod
-    def generate_mounts_and_args(mlcube: DictConfig, task: str) -> t.Tuple[t.Dict, t.List]:
-        """Generate mount points and arguments for the given task.
+    def get_host_path(workspace_path: str, path_from_config: str) -> str:
+        """Return host path for a task parameter.
 
+        Args:
+            workspace_path: Workspace directory path for this MLCube.
+            path_from_config: Parameter path as specified by a user in an MLCube configuration file (e.g., mlcube.yaml).
+
+        Returns:
+            Absolute host path.
+        """
+        # Omega conf will resolve any variables defined in MLCube configuration file. We need to take care about `~`
+        # (user home directory) and environment variables.
+        host_path = Path(
+            os.path.expandvars(os.path.expanduser(path_from_config))
+        )
+        # According to MLCube contract, relative paths are relative to MLCube workspace directory.
+        if not host_path.is_absolute():
+            host_path = Path(workspace_path) / host_path
+        return host_path.as_posix()
+
+    @staticmethod
+    def generate_mounts_and_args(mlcube: DictConfig, task: str,
+                                 make_dirs: bool = True) -> t.Tuple[t.Dict, t.List, t.Dict]:
+        """Generate mount points, task arguments and mount options for the given task.
+
+        Args:
+            mlcube: MLCube configuration (e.g., coming from `mlcube.yaml` file).
+            task: Task name for which mount points need to be generated.
+            make_dirs: If true, make host directories recursively if they do not exist. We need this to actually make
+                unit tests work (that set this value to false).
         Return:
-            A tuple containing two elements:
-                -  A mapping from host path to path inside container.
-                -  A list of task arguments.
+            A tuple containing three elements:
+                - A mapping from host path to path inside container.
+                - A list of task arguments.
+                - A mapping from host paths to mount options (optional).
         """
         # First task argument is always the task name.
-        mounts, args, mounts_opts = {}, [task], {}
+        mounts: t.Dict[str, str] = {}         # Mapping from host paths to container paths.
+        args: t.List[str] = [task]            # List of arguments for the given task.
+        mounts_opts: t.Dict[str, str] = {}    # Mapping from host paths to mount options (rw/ro).
 
         def _generate(_params: DictConfig, _io: str) -> None:
-            """_params here is a dictionary containing input or output parameters.
+            """Process parameters (could be inputs or outputs).
+
+            This function updates `mounts`, `args` and `mounts_opts`.
 
-            It maps parameter name to DictConfig(type, default)
+            Args:
+                _params: Dictionary of input or output parameters.
+                _io: Specifies if these parameters are input our output parameters.
             """
             if not IOType.is_valid(_io):
                 raise ConfigurationError(f"Invalid IO = {_io}")
             for _param_name, _param_def in _params.items():
+                assert isinstance(_param_def, DictConfig), f"Unexpected parameter definition: {_param_def}."
                 if not ParameterType.is_valid(_param_def.type):
-                    raise ConfigurationError(f"Invalid task: task={task}, param={_param_name}, "
-                                             f"type={_param_def.type}. Type is invalid.")
-                _host_path = Path(mlcube.runtime.workspace) / _param_def.default
+                    raise ConfigurationError(
+                        f"Invalid task: task={task}, param={_param_name}, type={_param_def.type}. Type is invalid."
+                    )
+
+                # MLCube contract says relative paths in MLCube configuration files are relative with respect to MLCube
+                # workspace directory. In certain cases it makes sense to use absolute paths too. This maybe the case
+                # when we want to reuse host cache directories that many machine learning frameworks use to cache models
+                # and datasets. We also need to be able to resolve `~` (user home directory), as well as environment
+                # variables (BTW, this is probably needs some discussion at some point in time). This environment
+                # variable could be, for instance, `${HOME}`.
+                _host_path: str = Shell.get_host_path(mlcube.runtime.workspace, _param_def.default)
 
                 if _param_def.type == ParameterType.UNKNOWN:
                     if _io == IOType.OUTPUT:
-                        raise ConfigurationError(f"Invalid task: task={task}, param={_param_name}, "
-                                                 f"type={_param_def.type}. Type is unknown.")
+                        raise ConfigurationError(
+                            f"Invalid task: task={task}, param={_param_name}, type={_param_def.type}. "
+                            "Type cannot be unknown for output parameters."
+                        )
                     else:
                         if os.path.isdir(_host_path):
                             _param_def.type = ParameterType.DIRECTORY
                         elif os.path.isfile(_host_path):
                             _param_def.type = ParameterType.FILE
                         else:
-                            raise ConfigurationError(f"Invalid task: task={task}, param={_param_name}, "
-                                                     f"type={_param_def.type}. Type is unknown and unable to identify "
-                                                     f"it ({_host_path}).")
+                            raise ConfigurationError(
+                                f"Invalid task: task={task}, param={_param_name}, type={_param_def.type}. "
+                                f"Type is unknown and unable to identify it ({_host_path})."
+                            )
 
                 if _param_def.type == ParameterType.DIRECTORY:
-                    os.makedirs(_host_path, exist_ok=True)
-                    mounts[_host_path] = mounts.get(
-                        _host_path,
-                        '/mlcube_io{}/{}'.format(len(mounts), os.path.basename(_host_path))
-                    )
+                    if make_dirs:
+                        os.makedirs(_host_path, exist_ok=True)
+                    mounts[_host_path] = mounts.get(_host_path, f"/mlcube_io{len(mounts)}")
                     args.append('--{}={}'.format(_param_name, mounts[_host_path]))
                 elif _param_def.type == ParameterType.FILE:
                     _host_path, _file_name = os.path.split(_host_path)
-                    os.makedirs(_host_path, exist_ok=True)
-                    new_mount = mounts.get(
-                        _host_path,
-                        '/mlcube_io{}/{}'.format(len(mounts), _host_path)
-                    )
-                    windows_match = ':\\'
-                    if windows_match in new_mount:
-                        index = new_mount.index(windows_match)
-                        substring = new_mount[index - 1: index + 2]
-                        new_mount = new_mount.replace(substring, '').replace('\\', '/')
-                    mounts[_host_path] = new_mount
+                    if make_dirs:
+                        os.makedirs(_host_path, exist_ok=True)
+                    mounts[_host_path] = mounts.get(_host_path, f"/mlcube_io{len(mounts)}")
                     args.append('--{}={}'.format(_param_name, mounts[_host_path] + '/' + _file_name))
 
-                if "opts" in _param_def:
-                    if MountType.is_valid(_param_def.opts):
-                        mounts_opts[_host_path] = _param_def.opts
-                    else:
-                        raise ConfigurationError(f"Invalid mount options: mount={task}, param={_param_name}, "
-                                                     f"opts={_param_def.opts}. Option is unknown and unable to identify")
-                else:
-                    mounts_opts[_host_path] = MountType.RW
-
-        params = mlcube.tasks[task].parameters
-        _generate(params.inputs, IOType.INPUT)
-        _generate(params.outputs, IOType.OUTPUT)
+                mount_type: t.Optional[str] = _param_def.get('opts', None)
+                if mount_type:
+                    if not MountType.is_valid(_param_def.opts):
+                        raise ConfigurationError(
+                            f"Invalid mount options: mount={task}, param={_param_name}, opts={_param_def.opts}."
+                        )
+                    if mount_type == MountType.RO and _io == IOType.OUTPUT:
+                        logger.warning(
+                            "Task's (%s) parameter (%s) is OUTPUT and requested to mount as RO.", task, _param_name
+                        )
+                    if _host_path in mounts_opts and mounts_opts[_host_path] != mount_type:
+                        logger.warning(
+                            "Conflicting mount options found. Host path (%s) has already been requested to mount as "
+                            "'%s', but new parameter (%s) requests to mount as '%s'.",
+                            _host_path, mounts_opts[_host_path], _param_name, mount_type
+                        )
+                        # Since we can only have `ro`/`rw`, we'll set the mount option to `rw`.
+                        mount_type = MountType.RW
+
+                    mounts_opts[_host_path] = mount_type
+                    logger.info(
+                        "Host path (%s) for parameter '%s' will be mounted with '%s' option.",
+                        _host_path, _param_name, mount_type
+                    )
+
+        params = mlcube.tasks[task].parameters     # Dictionary of input and output parameters for the task.
+        _generate(params.inputs, IOType.INPUT)     # Process input parameters.
+        _generate(params.outputs, IOType.OUTPUT)   # Process output parameters.
 
         return mounts, args, mounts_opts
 
     @staticmethod
     def to_cli_args(args: t.Mapping[str, t.Any], sep: str = '=', parent_arg: t.Optional[str] = None) -> str:
         """Convert dict to CLI arguments.
```

### Comparing `mlcube-0.0.8/mlcube/system_settings.py` & `mlcube-0.0.9/mlcube/system_settings.py`

 * *Files identical despite different names*

### Comparing `mlcube-0.0.8/mlcube/tests/test_config.py` & `mlcube-0.0.9/mlcube/tests/test_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 tasks:
   download:
     {DOWNLOAD_ENTRY_POINT}
     parameters:
       inputs:
         data_config: {type: file, default: data.yaml}
       outputs:
-        data_dir: {type: directory, default: data}
+        data_dir: data/
         log_dir: {type: directory, default: logs}
   train:
     parameters:
       inputs:
         data_dir: {type: directory, default: data}
         train_config: {type: file, default: train.yaml}
       outputs:
-        log_dir: {type: directory, default: logs}
-        model_dir: {type: directory, default: model}
+        log_dir: logs/
+        model_dir: model\\
 """
 
 _DOWNLOAD_TASK_ENTRY_POINT = '/workspace/mnist/download.py'
 
 _MLCUBE_MNIST_CONFIG = _MLCUBE_MNIST_CONFIG_TEMPLATE.replace(
     '{DOWNLOAD_ENTRY_POINT}',
     ''
@@ -56,14 +56,17 @@
     '{DOWNLOAD_ENTRY_POINT}',
     f'entrypoint: {_DOWNLOAD_TASK_ENTRY_POINT}'
 )
 
 
 class TestConfig(TestCase):
 
+    def setUp(self) -> None:
+        self.maxDiff = None
+
     def _check_standard_config(self, mlcube: DictConfig, entry_points: bool = False) -> None:
         self.assertIsInstance(mlcube, DictConfig)
 
         for key in ('name', 'description', 'authors',
                     'platform',
                     'docker', 'singularity',
                     'tasks',
@@ -100,28 +103,28 @@
         expected_task_specs = {
             'download': {
                 'parameters': {
                     'inputs': {
                         'data_config': {'type': 'file', 'default': 'data.yaml'}
                     },
                     'outputs': {
-                        'data_dir': {'type': 'directory', 'default': 'data'},
+                        'data_dir': {'type': 'directory', 'default': 'data/'},
                         'log_dir': {'type': 'directory', 'default': 'logs'}
                     }
                 },
             },
             'train': {
                 'parameters': {
                     'inputs': {
                         'data_dir': {'type': 'directory', 'default': 'data'},
                         'train_config': {'type': 'file', 'default': 'train.yaml'}
                     },
                     'outputs': {
-                        'log_dir': {'type': 'directory', 'default': 'logs'},
-                        'model_dir': {'type': 'directory', 'default': 'model'}
+                        'log_dir': {'type': 'directory', 'default': 'logs/'},
+                        'model_dir': {'type': 'directory', 'default': 'model\\'}
                     }
                 }
             }
         }
         if entry_points:
             expected_task_specs['download']['entrypoint'] = _DOWNLOAD_TASK_ENTRY_POINT
         self.assertDictEqual(OmegaConf.to_container(mlcube.tasks), expected_task_specs)
@@ -183,7 +186,66 @@
 
     def test_mount_type(self) -> None:
         self.assertEqual(MountType.RW, 'rw')
         self.assertTrue(MountType.is_valid('rw'))
 
         self.assertEqual(MountType.RO, 'ro')
         self.assertTrue(MountType.is_valid('ro'))
+
+    def test_check_with_logging(self) -> None:
+        mlcube_config = DictConfig({
+            "singularity": {
+                "image": "mnist-0.0.1.sif"
+            },
+            "runtime": {
+                "workspace": "/some/path/to/workspace"
+            },
+            "runner": {
+                "runner": "singularity",
+                "image": "${singularity.image}",
+                "image_dir": "${runtime.workspace}/.image",
+                "singularity": "singularity",
+                "build_args": "--fakeroot",
+                "run_args": "-C --net",
+                "build_file": "Singularity2.recipe"
+            }
+        })
+        default_runner_config = DictConfig({
+            "runner": "singularity",
+            "image": "${singularity.image}",
+            "image_dir": "${runtime.workspace}/.image",
+            "singularity": "singularity",
+            "build_args": "--fakeroot",
+            "run_args": "",
+            "build_file": "Singularity.recipe",
+            "--network": None,
+            "--security": None,
+            "--nv": None,
+            "--vm-ram": None,
+            "--vm-cpu": None
+        })
+        MLCubeConfig.merge_with_logging(mlcube_config, default_runner_config)
+        self.assertDictEqual(
+            OmegaConf.to_container(mlcube_config, resolve=True),
+            {
+                "singularity": {
+                    "image": "mnist-0.0.1.sif"
+                },
+                "runtime": {
+                    "workspace": "/some/path/to/workspace"
+                },
+                "runner": {
+                    "runner": "singularity",
+                    "image": "mnist-0.0.1.sif",
+                    "image_dir": "/some/path/to/workspace/.image",
+                    "singularity": "singularity",
+                    "build_args": "--fakeroot",
+                    "run_args": "-C --net",
+                    "build_file": "Singularity2.recipe",
+                    "--network": None,
+                    "--security": None,
+                    "--nv": None,
+                    "--vm-ram": None,
+                    "--vm-cpu": None
+                }
+            }
+        )
```

### Comparing `mlcube-0.0.8/mlcube/tests/test_errors.py` & `mlcube-0.0.9/mlcube/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `mlcube-0.0.8/mlcube/validate.py` & `mlcube-0.0.9/mlcube/validate.py`

 * *Files identical despite different names*

### Comparing `mlcube-0.0.8/mlcube.egg-info/SOURCES.txt` & `mlcube-0.0.9/mlcube.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 setup.py
 mlcube/__init__.py
 mlcube/__main__.py
+mlcube/cli.py
 mlcube/config.py
 mlcube/errors.py
 mlcube/parser.py
 mlcube/platform.py
 mlcube/runner.py
 mlcube/shell.py
 mlcube/system_settings.py
@@ -12,11 +13,13 @@
 mlcube.egg-info/PKG-INFO
 mlcube.egg-info/SOURCES.txt
 mlcube.egg-info/dependency_links.txt
 mlcube.egg-info/entry_points.txt
 mlcube.egg-info/requires.txt
 mlcube.egg-info/top_level.txt
 mlcube/tests/__init__.py
+mlcube/tests/test_cli.py
 mlcube/tests/test_config.py
 mlcube/tests/test_errors.py
 mlcube/tests/test_mlcommons_mlcube_cli.py
-mlcube/tests/test_parser.py
+mlcube/tests/test_parser.py
+mlcube/tests/test_shell.py
```

### Comparing `mlcube-0.0.8/setup.py` & `mlcube-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 extra_files = schemas()
 
 
 setup(
     name="mlcube",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     license="Apache 2.0",
     entry_points='''
         [console_scripts]
         mlcube=mlcube.__main__:cli
     ''',
     install_requires=requires,
```

