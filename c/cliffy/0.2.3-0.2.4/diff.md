# Comparing `tmp/cliffy-0.2.3.tar.gz` & `tmp/cliffy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.2.3.tar", max compression
+gzip compressed data, was "cliffy-0.2.4.tar", max compression
```

## Comparing `cliffy-0.2.3.tar` & `cliffy-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1060 2023-04-03 21:22:39.751862 cliffy-0.2.3/LICENSE
--rw-r--r--   0        0        0     1376 2023-04-03 21:22:39.751862 cliffy-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/__init__.py
--rw-r--r--   0        0        0     3422 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     4012 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      984 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1836 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     1342 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/helper.py
--rw-r--r--   0        0        0     1649 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/homer.py
--rw-r--r--   0        0        0     1354 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/loader.py
--rw-r--r--   0        0        0      280 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     5994 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/manifests/v1.py
--rw-r--r--   0        0        0     5334 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/parser.py
--rw-r--r--   0        0        0       47 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/run.py
--rw-r--r--   0        0        0      883 2023-04-03 21:22:39.751862 cliffy-0.2.3/cliffy/transformer.py
--rw-r--r--   0        0        0      880 2023-04-03 21:22:39.755862 cliffy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 cliffy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-17 03:30:13.681324 cliffy-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5040 2023-04-17 03:30:13.681324 cliffy-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 03:30:13.681324 cliffy-0.2.4/cliffy/__init__.py
+-rw-r--r--   0        0        0     4429 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     4010 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      984 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1836 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     1393 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/helper.py
+-rw-r--r--   0        0        0     3459 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/homer.py
+-rw-r--r--   0        0        0     1354 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/loader.py
+-rw-r--r--   0        0        0      297 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7130 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/merger.py
+-rw-r--r--   0        0        0     5179 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/parser.py
+-rw-r--r--   0        0        0       47 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/run.py
+-rw-r--r--   0        0        0     2484 2023-04-17 03:30:13.685325 cliffy-0.2.4/cliffy/transformer.py
+-rw-r--r--   0        0        0      919 2023-04-17 03:30:13.685325 cliffy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5866 1970-01-01 00:00:00.000000 cliffy-0.2.4/PKG-INFO
```

### Comparing `cliffy-0.2.3/LICENSE` & `cliffy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.3/cliffy/cli.py` & `cliffy-0.2.4/cliffy/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 ## CLI to generate CLIs
 from typing import TextIO
 
 import rich_click as click
 from rich.console import Console
 from rich.syntax import Syntax
+from rich_click.rich_group import RichGroup
 
 from .helper import print_rich_table, write_to_file
 from .homer import Homer
 from .loader import Loader
-from .manifests import get_cli_manifest
+from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
-@click.group(context_settings=CONTEXT_SETTINGS)
+class RichAliasedGroup(RichGroup):
+    def get_command(self, ctx, cmd_name):
+        try:
+            cmd_name = ALIASES[cmd_name].name
+        except KeyError:
+            pass
+        return super().get_command(ctx, cmd_name or "")
+
+
+@click.group(context_settings=CONTEXT_SETTINGS, cls=RichAliasedGroup)
 @click.version_option()
 def cli() -> None:
     pass
 
 
 @cli.command()
 @click.argument('manifests', type=click.File('rb'), nargs=-1)
@@ -30,14 +40,31 @@
         Homer.save_cli_metadata(manifest.name, T.cli)
         click.secho(f"~ Generated {T.cli.name} CLI v{T.cli.version} ~", fg="green")
         click.secho(click.style("$", fg="magenta"), nl=False)
         click.echo(f" {T.cli.name} -h")
 
 
 @cli.command()
+@click.argument('cli_names', type=str, nargs=-1)
+def update(cli_names: list[str]) -> None:
+    """Reloads CLI by name"""
+    for cli_name in cli_names:
+        cli_metadata = Homer.get_cli_metadata(cli_name)
+        if cli_metadata:
+            T = Transformer(open(cli_metadata.runner_path, "r"))
+            Loader.load_cli(T.cli)
+            Homer.save_cli_metadata(cli_metadata.runner_path, T.cli)
+            click.secho(f"~ Reloaded {T.cli.name} CLI v{T.cli.version} ~", fg="green")
+            click.secho(click.style("$", fg="magenta"), nl=False)
+            click.echo(f" {T.cli.name} -h")
+        else:
+            click.secho(f"~ {cli_name} not found", fg="red")
+
+
+@cli.command()
 @click.argument('manifest', type=click.File('rb'))
 def render(manifest: TextIO) -> None:
     """Render the CLI manifest generation as code"""
     T = Transformer(manifest)
     syntax = Syntax(T.cli.code, "python", theme="monokai", line_numbers=False)
     console = Console()
     console.print(syntax)
@@ -56,44 +83,43 @@
     is_flag=True,
     show_default=True,
     default=False,
     help="Raw template without boilerplate helpers and examples.",
 )
 def init(cli_name: str, version: str, render: bool, raw: bool) -> None:
     """Generate a CLI manifest template"""
-    manifest = get_cli_manifest(version)
-    template = manifest.get_raw_template(cli_name) if raw else manifest.get_template(cli_name)
+    set_manifest_version(version)
+    template = Manifest.get_raw_template(cli_name) if raw else Manifest.get_template(cli_name)
 
     if render:
         syntax = Syntax(template, "yaml", theme="monokai", line_numbers=False)
         console = Console()
         console.print(syntax)
     else:
         write_to_file(f'{cli_name}.yaml', text=template)
+        click.secho(f"+ {cli_name}.yaml", fg="green")
 
 
 @cli.command("list")
 def list_clis() -> None:
-    "List of CLIs loaded"
-    metadata_paths = Homer.get_cli_metadata_paths()
+    "List all CLIs loaded"
     cols = ["Name", "Version", "Manifest"]
     rows = []
-    for path in metadata_paths:
-        runnerpath, metadata = Homer.get_cli_metadata(path)
-        rows.append([path.name, metadata.get("version", "error"), runnerpath])
+    for metadata in Homer.get_clis():
+        rows.append([metadata.cli_name, metadata.version, metadata.runner_path])
 
     print_rich_table(cols, rows, styles=["cyan", "magenta", "green"])
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
-def unload(cli_names: list[str]) -> None:
+def remove(cli_names: list[str]) -> None:
     "Remove a loaded CLI by name"
     for cli_name in cli_names:
-        if Homer.is_cliffy_cli(cli_name):
+        if Homer.get_cliffy_cli(cli_name):
             Homer.remove_cli_metadata(cli_name)
             Loader.unload_cli(cli_name)
             click.secho(f"~ {cli_name} unloaded", fg="green")
         else:
             click.secho(f"~ {cli_name} not found", fg="red")
 
 
@@ -103,7 +129,13 @@
     click.echo("# TODO")
 
 
 @cli.command()
 @click.argument('cli_name', type=str)
 def disable(cli_name) -> None:
     click.echo("# TODO")
+
+
+ALIASES = {
+    "rm": remove,
+    "ls": list_clis,
+}
```

### Comparing `cliffy-0.2.3/cliffy/commander.py` & `cliffy-0.2.4/cliffy/commander.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def add_greedy_commands(self) -> None:
         """Greedy commands get lazy-loaded. Only supported for group-commands currently"""
         for greedy_command in self.greedy:
             if greedy_command.name.startswith('(*)'):
                 for group in self.groups:
                     # make it lazy and interpolate
                     lazy_command_name = greedy_command.name.replace('(*)', group)
-                    lazy_command_script = greedy_command.script.replace('{{(*)}}', group)
+                    lazy_command_script = greedy_command.script.replace('{(*)}', group)
 
                     # lazy load the greedy args
                     greedy_command_args = self.manifest.args.get(greedy_command.name)
                     if greedy_command_args:
                         self.manifest.args[lazy_command_name] = greedy_command_args
 
                     # lazy parse
```

### Comparing `cliffy-0.2.3/cliffy/commanders/click.py` & `cliffy-0.2.4/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.3/cliffy/commanders/typer.py` & `cliffy-0.2.4/cliffy/commanders/typer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.3/cliffy/helper.py` & `cliffy-0.2.4/cliffy/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
-import pathlib
 import sys
+from pathlib import Path
 from typing import Optional
 
 from rich.console import Console
 from rich.table import Table
 
-HOME_PATH = str(pathlib.Path.home())
+HOME_PATH = str(Path.home())
 PYTHON_BIN = f"{sys.exec_prefix}/bin"
 PYTHON_EXECUTABLE = sys.executable
-CLIFFY_CLI_DIR = f"{pathlib.Path(__file__).parent.resolve()}/clis"
+CLIFFY_CLI_DIR = f"{Path(__file__).parent.resolve()}/clis"
 CLIFFY_HOME_PATH = f"{HOME_PATH}/.cliffy"
 
 
 def write_to_file(path: str, text: str, executable: bool = False) -> bool:
     try:
-        output_file = pathlib.Path(path)
+        output_file = Path(path)
         output_file.parent.mkdir(exist_ok=True, parents=True)
         output_file.write_text(text)
     except Exception as e:
         print("write_to_file", e)
         return False
 
     if executable:
@@ -37,14 +37,16 @@
 def wrap_as_comment(text: str, split_on: Optional[str] = None) -> str:
     if split_on:
         joiner = "\n# "
         return "# " + joiner.join(text.split(split_on))
 
     return f"# {text}"
 
+def wrap_as_var(text: str) -> str:
+    return '{{' + text + '}}'
 
 def print_rich_table(cols: list[str], rows: list[list[str]], styles: list[str]) -> None:
     table = Table()
     for style, col in zip(styles, cols):
         table.add_column(col, style=style)
     for row in rows:
         table.add_row(*row)
```

### Comparing `cliffy-0.2.3/cliffy/loader.py` & `cliffy-0.2.4/cliffy/loader.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.3/cliffy/manifests/v1.py` & `cliffy-0.2.4/cliffy/manifests/v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from datetime import datetime
 from typing import Literal, Union
 
 from pydantic import BaseModel, Field
 
-from ..helper import wrap_as_comment
+from ..helper import wrap_as_comment, wrap_as_var
 
 
 class CLIManifest(BaseModel):
     name: str = Field(
         description="The name of the CLI. "
         "This will be used as the script name when invoking the CLI from the command line."
     )
@@ -16,21 +17,28 @@
     )
     help: str = Field(
         "",
         description="A brief description of the CLI that is displayed when the user invokes the --help or -h option.",
     )
     includes: list[str] = Field(
         [],
-        description="!TODO! List of external CLI manifest paths to include into the main manifest. "
+        description="List of external CLI manifest paths to include into the main manifest. "
         "Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest "
         "and finally, deep merges the merged manifest with the main manifest.",
     )
+    vars: dict[str, str] = Field(
+        {},
+        description="A mapping defining manifest variables that can be referenced in any other blocks. "
+        "Environments variables can be used in this section with ${some_env_var} for dynamic parsing. "
+        "Supports jinja2 formatted expressions as values. "
+        "Interpolate defined vars in other blocks jinja2-styled {{ var_name }}.",
+    )
     commands: dict[str, Union[str, list[Union[str, dict[Literal['help'], str]]]]] = Field(
         {},
-        description="A dictionary containing the command definitions for the CLI. "
+        description="A mapping containing the command definitions for the CLI. "
         "Each command should have a unique key- which can be either a group command or nested subcommands. "
         "Nested subcommands are joined by '.' in between each level. "
         "A special (*) wildcard can be used to spread the subcommand to all group-level commands. "
         "The value is the python code to run when the command is called "
         "OR a list of bash commands to run (prefixed with $).",
     )
     imports: Union[str, list[str]] = Field(
@@ -42,27 +50,27 @@
         [],
         description="A list containing any helper functions. "
         "Each element of the list can be a separate function. "
         "These functions should be defined as strings that can be executed by the Python interpreter.",
     )
     args: dict[str, list] = Field(
         {},
-        description="A dictionary containing the arguments and options for each command. "
-        "Each key in the dictionary should correspond to a command in the commands section. "
-        "The value should be a list of dictionaries representing the params and options for that command.",
+        description="A mapping containing the arguments and options for each command. "
+        "Each key in the mapping should correspond to a command in the commands section. "
+        "The value should be a list of mappings representing the params and options for that command.",
     )
     types: dict[str, str] = Field(
         {},
-        description="A dictionary containing any shared type definitions. "
+        description="A mapping containing any shared type definitions. "
         "These types can be referenced by name in the args section to provide type annotations "
         "for params and options defined in the args section.",
     )
     cli_options: dict[str, str] = Field(
         {},
-        Description="A dictionary for any additional options that can be used to customize the behavior of the CLI.",
+        Description="A mapping for any additional options that can be used to customize the behavior of the CLI.",
     )
 
     @classmethod
     def get_field_description(cls, field_name: str, as_comment: bool = False) -> str:
         field = cls.__fields__.get(field_name)
         if field and field.field_info.description:
             if as_comment:
@@ -80,14 +88,18 @@
 
 {cls.get_field_description('version', as_comment=True)}
 version: 0.1.0
 
 {cls.get_field_description('includes', as_comment=True)}
 includes: []
 
+{cls.get_field_description('vars', as_comment=True)}
+vars:
+    default_mood: happy
+
 {cls.get_field_description('imports', as_comment=True)}
 imports:
     - import os
     - |
         from collections import defaultdict
         import re
 
@@ -102,15 +114,15 @@
     Language: str = typer.Option("english", "-l", help="Language to greet in", prompt=True)
 
 {cls.get_field_description('args', as_comment=True)}
 args:
     world: [--name|-n: str!]                      # a REQUIRED option
     greet.all: 
         - names: str!                             # a REQUIRED param as denoted by the ! at the end
-        - mood: str = "happy"                     # an OPTIONAL param that defaults to "happy"
+        - mood: str = "{wrap_as_var("default_mood")}"          # an OPTIONAL param that uses a manifest var as default
         - --language: Language                    # an option with a default that uses Language type as arg definition
 
 {cls.get_field_description('commands', as_comment=True)}
 commands:
     # this is a parent command that will get invoked with: hello world
     world: 
         - |
@@ -140,14 +152,17 @@
 
 {cls.get_field_description('version', as_comment=True)}
 version: 0.1.0
 
 {cls.get_field_description('includes', as_comment=True)}
 includes: []
 
+{cls.get_field_description('vars', as_comment=True)}
+vars: {{}}
+
 {cls.get_field_description('imports', as_comment=True)}
 imports: []
 
 {cls.get_field_description('functions', as_comment=True)}
 functions: []
 
 {cls.get_field_description('types', as_comment=True)}
@@ -156,7 +171,28 @@
 {cls.get_field_description('args', as_comment=True)}
 args: {{}}
 
 {cls.get_field_description('commands', as_comment=True)}
 commands: {{}}
 
 """
+
+
+class IncludeManifest(BaseModel):
+    """Special manifest specifically to define the allowed named objects that can be included"""
+
+    commands: dict[str, Union[str, list[Union[str, dict[Literal['help'], str]]]]] = {}
+    imports: Union[str, list[str]] = []
+    functions: list[str] = []
+    args: dict[str, list] = {}
+    types: dict[str, str] = {}
+    cli_options: dict[str, str] = {}
+
+
+class CLIMetadata(BaseModel):
+    """Metadata model"""
+
+    cli_name: str
+    runner_path: str
+    version: str
+    loaded: datetime
+    manifest: str
```

### Comparing `cliffy-0.2.3/cliffy/parser.py` & `cliffy-0.2.4/cliffy/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,15 @@
     ) -> str:
         parsed_arg_type = f"{arg_name}: {arg_type} = typer.{typer_cls}"
 
         if not default_val:
             # Required param needs ...
             parsed_arg_type += "(..." if is_required else "(None"
         else:
-            # Optional if default_val given
-            if arg_type == "str":
-                parsed_arg_type += f"('{default_val}'"
-            else:
-                parsed_arg_type += f"({default_val}"
+            parsed_arg_type += f"({default_val}"
 
         if aliases:
             parsed_arg_type += f', "--{arg_name}"'
             for alias in aliases:
                 parsed_arg_type += f', "{alias}"'
 
         parsed_arg_type += '),'
```

### Comparing `cliffy-0.2.3/pyproject.toml` & `cliffy-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.2.3"
+version = "0.2.4"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich-click = "^1.6.1"
 pybash = "^0.2.3"
 pyyaml = "^6.0"
 typer = "^0.7.0"
 shellingham = "^1.5.0.post1"
 pydantic = "^1.10.6"
+deepmerge = "^1.1.0"
+jinja2 = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 autoflake = "^2.0.0"
```

