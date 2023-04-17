# Comparing `tmp/pndconf-0.4.5.tar.gz` & `tmp/pndconf-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pndconf-0.4.5.tar", max compression
+gzip compressed data, was "pndconf-0.5.0.tar", max compression
```

## Comparing `pndconf-0.4.5.tar` & `pndconf-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1070 2021-09-13 22:17:24.130422 pndconf-0.4.5/LICENSE
--rw-r--r--   0        0        0       22 2022-02-10 11:24:51.419060 pndconf-0.4.5/pndconf/__init__.py
--rw-r--r--   0        0        0       66 2021-09-14 00:57:13.327729 pndconf-0.4.5/pndconf/__main__.py
--rw-r--r--   0        0        0      410 2021-10-16 08:31:52.655231 pndconf-0.4.5/pndconf/colors.py
--rw-r--r--   0        0        0    10455 2021-10-17 23:53:28.100450 pndconf-0.4.5/pndconf/compilers.py
--rw-r--r--   0        0        0    22998 2022-02-10 11:21:26.102027 pndconf-0.4.5/pndconf/config.py
--rw-r--r--   0        0        0      935 2022-02-10 11:21:26.102027 pndconf-0.4.5/pndconf/config_default.ini
--rwxr-xr-x   0        0        0    14658 2022-02-10 11:21:26.102027 pndconf-0.4.5/pndconf/pndconf.py
--rw-r--r--   0        0        0        0 2021-09-13 22:32:39.945541 pndconf-0.4.5/pndconf/py.typed
--rw-r--r--   0        0        0     1706 2021-09-13 22:17:24.132422 pndconf-0.4.5/pndconf/table-filter.py
--rw-r--r--   0        0        0    13861 2022-02-10 11:21:26.103027 pndconf-0.4.5/pndconf/transforms.py
--rw-r--r--   0        0        0     8783 2022-02-10 11:21:26.103027 pndconf-0.4.5/pndconf/util.py
--rw-r--r--   0        0        0     3189 2021-09-26 09:13:20.040760 pndconf-0.4.5/pndconf/watcher.py
--rw-r--r--   0        0        0      530 2022-02-10 11:22:03.730300 pndconf-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      872 2022-02-10 11:24:51.949119 pndconf-0.4.5/setup.py
--rw-r--r--   0        0        0      709 2022-02-10 11:24:51.949372 pndconf-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-09-13 22:17:24.130422 pndconf-0.5.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-17 02:18:33.064953 pndconf-0.5.0/pndconf/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-14 14:22:34.808866 pndconf-0.5.0/pndconf/__main__.py
+-rw-r--r--   0        0        0     4887 2023-04-14 11:42:40.967407 pndconf-0.5.0/pndconf/bibliography.py
+-rw-r--r--   0        0        0    18948 2023-04-14 16:05:57.445572 pndconf-0.5.0/pndconf/commands.py
+-rw-r--r--   0        0        0    10368 2023-04-15 00:07:11.546107 pndconf-0.5.0/pndconf/compilers.py
+-rw-r--r--   0        0        0    13414 2023-04-15 00:39:01.645802 pndconf-0.5.0/pndconf/config.py
+-rw-r--r--   0        0        0      935 2022-02-10 11:21:26.102027 pndconf-0.5.0/pndconf/config_default.ini
+-rw-r--r--   0        0        0      621 2023-04-14 23:40:59.008115 pndconf-0.5.0/pndconf/const.py
+-rw-r--r--   0        0        0     3583 2023-04-15 00:27:22.648929 pndconf-0.5.0/pndconf/functions.py
+-rw-r--r--   0        0        0    15408 2023-04-14 23:41:06.564298 pndconf-0.5.0/pndconf/parser.py
+-rw-r--r--   0        0        0        0 2021-09-13 22:32:39.945541 pndconf-0.5.0/pndconf/py.typed
+-rw-r--r--   0        0        0    14885 2023-04-12 23:08:53.210645 pndconf-0.5.0/pndconf/transforms.py
+-rw-r--r--   0        0        0     6733 2023-04-15 00:17:53.833666 pndconf-0.5.0/pndconf/util.py
+-rw-r--r--   0        0        0     3189 2021-09-26 09:13:20.040760 pndconf-0.5.0/pndconf/watcher.py
+-rw-r--r--   0        0        0      481 2023-04-17 02:17:33.932059 pndconf-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      809 2023-04-17 02:19:48.594988 pndconf-0.5.0/setup.py
+-rw-r--r--   0        0        0      669 2023-04-17 02:19:48.595226 pndconf-0.5.0/PKG-INFO
```

### Comparing `pndconf-0.4.5/LICENSE` & `pndconf-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pndconf-0.4.5/pndconf/compilers.py` & `pndconf-0.5.0/pndconf/compilers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, Any, Union, List, Optional, cast
 import os
 import re
 import chardet
 import yaml
 from subprocess import Popen, PIPE
 
-from .util import get_now as now
-from .colors import COLORS
+from .util import get_now as now, logbbi
+from .const import COLORS
 
 
 PostProc = List[Dict[str, str]]
 
 
 # FIXME: Use log* for logging
 class TexCompiler:
@@ -179,23 +179,58 @@
 
 def is_tex_command(cmd: str) -> bool:
     splits = cmd.split("&&")
     return any([re.match("^pdflatex|pdftex|biber", s.strip(), flags=re.IGNORECASE)
                 for s in splits])
 
 
-def exec_command(command: str, input: Optional[str] = None, noshell: bool = False):
+def exec_tex_command(command):
+    try:
+        # status = exec_tex_compile(command)
+        if "pdftex" in command or "pdflatex" in command:
+            tex_compiler.mode = "latex"
+        elif "biber" in command:
+            tex_compiler.mode = "biber"
+        else:
+            raise ValueError(f"Unknown tex command in {command}")
+        status = tex_compiler.compile(command)
+        return status
+    except Exception as e:
+        print(f"Error occured while compiling file {e}")
+        return False
+
+
+def success_message(out, err):
+    if out:
+        out = out.strip("\n")
+        print(f"Output from command: {out}")
+    if err:
+        err = err.strip("\n")
+        err = "\n".join([f"\t{e}" for e in err.split("\n")])
+        print(f"No error from command, but: {COLORS.ALT_RED}\n{err}{COLORS.ENDC}")
+
+
+def error_message(err, p):
+    if err:
+        print(f"Error occured : {err}")
+    elif "pdflatex" in p.args or "pdftex" in p.args:
+        print("Got err return from pdflatex. Check log in output directory")
+    else:
+        print("Some unknown error reported. If all outputs seem fine, then ignore it.")
+
+
+def exec_command(command: str, stdin: Optional[str] = None, noshell: bool = False):
     """Execute a command via :class:`Popen`.
 
     The command is exectued with `shell=True`. Use `noshell=True` for inverting
     that behaviour
 
     Args:
         command: The command to execute
-        input: Optional input to give to command via stdin
+        stdin: Optional input to give to command via stdin
         noshell: Whether not to use shell
 
     Aside from arbitrary shell commands, `pdftex`, `pdflatex` and `biber` are
     compiled via a separate :class:`TexCompiler` for printing legible color
     coded warnings and errors.
 
     """
@@ -203,69 +238,45 @@
     splits = command.split(" ")
     splits = [splits[i*4:(i+1)*4] for i in range(len(splits)//4 + 1)]  # type: ignore
     cmd = ("\n" + " "*len(prefix)).join([" ".join(x) for x in splits])
     shell = not noshell
     print(f"{prefix}{cmd}")
     os.chdir(os.path.abspath(os.getcwd()))
     if is_tex_command(command):
-        try:
-            # NOTE: Changed to TexCompiler
-            # status = exec_tex_compile(command)
-            if "pdftex" in command or "pdflatex" in command:
-                tex_compiler.mode = "latex"
-            elif "biber" in command:
-                tex_compiler.mode = "biber"
-            else:
-                raise ValueError(f"Unknown tex command in {command}")
-            status = tex_compiler.compile(command)
-            return status
-        except Exception as e:
-            print(f"Error occured while compiling file {e}")
-            return False
+        return exec_tex_command(command)
+
+    if stdin:
+        p = Popen(command, stdin=PIPE, stdout=PIPE, stderr=PIPE, shell=shell)
+        output = p.communicate(input=stdin.encode())
     else:
-        if input:
-            p = Popen(command, stdin=PIPE, stdout=PIPE, stderr=PIPE, shell=shell)
-            output = p.communicate(input=input.encode())
-        else:
-            p = Popen(command, stdout=PIPE, stderr=PIPE, shell=shell)
-            output = p.communicate()
-        out = output[0].decode("utf-8")
-        err = output[1].decode("utf-8")
-        success = not p.returncode
-        if success:
-            if out:
-                out = out.strip("\n")
-                print(f"Output from command: {out}")
-            if err:
-                err = err.strip("\n")
-                err = "\n".join([f"\t{e}" for e in err.split("\n")])
-                print(f"No error from command, but: {COLORS.ALT_RED}\n{err}{COLORS.ENDC}")
-            return True
-        else:
-            if err:
-                print(f"Error occured : {err}")
-            elif "pdflatex" in p.args or "pdftex" in p.args:
-                print(f"Got err return from pdflatex. Check log in output directory")
-            else:
-                print(f"Some unknown error reported. If all outputs seem fine, then ignore it.")
-            return False
+        p = Popen(command, stdout=PIPE, stderr=PIPE, shell=shell)
+        output = p.communicate()
+    out = output[0].decode("utf-8")
+    err = output[1].decode("utf-8")
+    success = not p.returncode
+    if success:
+        success_message(out, err)
+        return True
+    else:
+        error_message(err, p)
+        return False
 
 
 def markdown_compile(commands: Dict[str, Dict[str, Union[List[str], str]]],
                      md_file: str) -> Optional[PostProc]:  # FIXME: Actually it's a path
     """Compile markdown to output format with pandoc.
 
     Args:
         commands: :class:`dict` of commands with output filetypes as keys
         md_file: The markdown input file to compile
     """
     if not isinstance(md_file, str) or not md_file.endswith('.md'):
         print(f"Not markdown file {md_file}")
         return None
-    print(f"\n{COLORS.BRIGHT_BLUE}Compiling {md_file} at {now()}{COLORS.ENDC}")
+    logbbi(f"\nCompiling {md_file} at {now()}")
     postprocess = []
     # NOTE: commands' values are either strings or lists of strings
     for filetype, command_dict in commands.items():
         command = command_dict["command"]
         out_file: str = cast(str, command_dict["out_file"])
         pandoc_opts = command_dict["in_file_opts"]
         file_text: str = cast(str, command_dict["text"])
```

### Comparing `pndconf-0.4.5/pndconf/config_default.ini` & `pndconf-0.5.0/pndconf/config_default.ini`

 * *Files identical despite different names*

### Comparing `pndconf-0.4.5/pndconf/pndconf.py` & `pndconf-0.5.0/pndconf/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,326 +1,357 @@
-#! /usr/bin/python3
+from typing import List, Optional, Tuple
 
-from typing import Optional
-
-import os
 import sys
-import time
 import shlex
 from pathlib import Path
 from subprocess import Popen, PIPE
 import argparse
-from watchdog.observers import Observer
-from types import SimpleNamespace
-
-from common_pyutil.system import hierarchical_parser
 
 from .config import Configuration
-from .watcher import ChangeHandler
 from .util import which, logd, loge, logi, logbi, logw
+from .functions import watch, convert
+from .const import gentypes, log_levels
 from . import __version__
 
+
 usage = """
     pndconf [global_opts] CMD [opts] [pandoc_opts]
 
     Pandoc options must be entered in '--opt=value' format.
 
-    Example:
-        # To watch in current directory and generate pdf and html outputs
-        pndconf watch -g pdf,html
+    See individual CMD help for usage of that command.
 
-        # To watch in some input directory and generate pdf and beamer outputs
-        # to some other output directory
-        pndconf watch -g pdf,beamer -d /path/to/watch_dir -o output_dir
+    \"pndconf -h/--help\" to print help
+
+    \"pndconf --long-help\" to print all global options
 """
-gentypes = ["html", "pdf", "reveal", "beamer", "latex"]
 
 
 def pandoc_version_and_path(pandoc_path: Optional[Path]):
     pandoc_path = Path(pandoc_path or which("pandoc"))
     if not (pandoc_path.exists() and pandoc_path.is_file()):
-        loge("'pandoc' executable not available.\n" +
+        loge("'pandoc' executable not available.\n"
              "Please install pandoc. Exiting!")
-        exit(1)
+        sys.exit(1)
     try:
         pandoc_version = Popen(shlex.split(f"{pandoc_path} --version"), stdout=PIPE).\
             communicate()[0].decode("utf-8").split()[1]
     except Exception as e:
         loge(f"Error checking pandoc version {e}")
         sys.exit(1)
     return pandoc_path, pandoc_version
 
 
-def get_config(args: SimpleNamespace, extra: SimpleNamespace) -> Configuration:
-    pandoc_path, pandoc_version = pandoc_version_and_path(args.pandoc_path)
-    logi(f"Pandoc path is {pandoc_path}")
-    if args.print_pandoc_opts:
-        out, err = Popen([str(pandoc_path), "--help"], stdout=PIPE, stderr=PIPE).communicate()
-        if err:
-            loge(f"Pandoc exited with error {err.decode('utf-8')}")
-        else:
-            loge(f"Pandoc options are \n{out.decode('utf-8')}")
-        sys.exit(0)
-    config = Configuration(args.watch_dir, args.output_dir,
-                           config_file=args.config_file,
-                           pandoc_path=pandoc_path,
-                           pandoc_version=pandoc_version,
-                           no_citeproc=args.no_citeproc,
-                           csl_dir=args.csl_dir,
-                           templates_dir=args.templates_dir,
-                           post_processor=args.post_processor,
-                           same_output_dir=args.same_output_dir,
-                           dry_run=args.dry_run)
-    # FIXME: No other args should be given with this
-    if args.print_generation_opts:
-        for ft in filter(None, args.generation.split(",")):  # type: ignore
-            opts = config._conf[ft]
+def get_pandoc_help_output(pandoc_path):
+    return Popen([str(pandoc_path), "--help"], stdout=PIPE, stderr=PIPE).communicate()
+
+
+def print_pandoc_opts(stdout, stderr):
+    if stderr:
+        loge(f"Pandoc exited with error {stderr.decode('utf-8')}")
+    else:
+        loge(f"Pandoc options are \n{stdout.decode('utf-8')}")
+
+
+def print_generation_opts(args, config):
+    for ft in filter(None, args.generation.split(",")):  # type: ignore
+        opts = config.conf[ft]
+        if opts:
             logi(f"Generation options for {ft} are:\n\t{[*opts.items()]}")
-            sys.exit(0)
         else:
             loge(f"No generation options for {ft}")
-    # NOTE: The program assumes that extensions startwith '.'
-    if args.exclude_regexp:
-        logi("Excluding files for given filters",
-             str(args.exclude_regexp.split(',')))
-        config.set_excluded_regexp(args.exclude_regexp.split(','),
-                                   args.exclude_ignore_case)
-    if args.inclusions:
-        inclusions = args.inclusions
-        inclusions = inclusions.split(",")
-        config.set_included_extensions(
-            [value for value in inclusions if value.startswith(".")])
-        if args.excluded_files:
-            for ef in args.excluded_files.split(','):
-                assert type(ef) == str
-            config.set_excluded_files(args.excluded_files.split(','))
-    if args.exclusions:
-        exclusions = args.exclusions
-        exclusions = exclusions.split(",")
-        excluded_extensions = [value for value in exclusions if value.startswith(".")]
-        excluded_folders = list(set(exclusions) - set(excluded_extensions))
-        config.set_excluded_extensions(excluded_extensions)
-        config.set_excluded_folders(excluded_folders)
-    if not args.generation:
-        loge("Generation options cannot be empty")
-        sys.exit(1)
+
+
+def maybe_exit_for_unknown_generation_type(args):
     diff = set(args.generation.split(",")) - set(gentypes)
     if diff:
         loge(f"Unknown generation type {diff}")
         loge(f"Choose from {gentypes}")
         sys.exit(1)
 
+
+def set_log_levels_and_maybe_log_pandoc_output(args, config, out):
     config.log_level = args.log_level
     if config.log_level > 2:
-        logi("\n".join(out.split("\n")[:3]))
-        logi("-" * len(out.split("\n")[2]))
+        logi("\n".join(out.decode().split("\n")[:3]))
+        logi("-" * len(out.decode().split("\n")[2]))
     if args.log_file:
-        config.log_file = args.log_file
+        config._log_file = args.log_file
         logw("Log file isn't implemented yet. Will output to stdout")
-    # TODO: Need Better checks
-    # NOTE: These options will override pandoc options in all the sections of
-    #       the config file
+
+
+# TODO: Need Better checks
+# NOTE: These options will override pandoc options in all the sections of
+#       the config file
+def validate_extra_args(extra):
     for i, arg in enumerate(extra):
-        if not arg.startswith('-'):
-            if not (i >= 1 and extra[i-1] == "-V"):
-                loge(f"pandoc option {arg} must be preceded with -, e.g. -{arg} or --{arg}=some_val")
-                sys.exit(1)
+        if not arg.startswith('-') and not (i >= 1 and extra[i-1] == "-V"):
+            loge(f"Unknown pdfconf option {arg}.\n"
+                 f"If it's a pandoc option {arg}, it must be preceded with -"
+                 f", e.g. -{arg} or --{arg}=some_val")
+            sys.exit(1)
         if arg.startswith('--') and '=' not in arg:
-            loge(f"pandoc option {arg} must be joined with =. e.g. {arg}=some_val")
+            loge(f"Unknown pdfconf option {arg}.\n"
+                 f"If it's a pandoc option {arg}, it must be joined with \"=\". "
+                 f"e.g. {arg}=some_val")
             sys.exit(1)
-    logbi(f"Will generate for {args.generation.upper()}")
-    logbi(f"Extra pandoc args are {extra}")
-    config.set_cmdline_opts(args.generation.split(','), extra)
-    return config
+
+
+# CHECK: Since the options like these are really commmon options and not usually
+#        specified in the config.ini (which only contains generation) options
+#        anyway. Perhaps they should be moved to separate config classes.
+def get_config_and_pandoc_output(args: argparse.Namespace)\
+        -> Tuple[Configuration, Tuple[str, str]]:
+    pandoc_path, pandoc_version = pandoc_version_and_path(args.pandoc_path)
+    out, err = get_pandoc_help_output(pandoc_path)
+    logi(f"Pandoc path is {pandoc_path}\n")
+    # NOTE: This one is only watch specific
+    watch_dir = getattr(args, "watch_dir", None)
+    # NOTE: these options are common and added by subcommand parsers
+    output_dir = Path(getattr(args, "output_dir", "."))
+    no_citeproc = getattr(args, "no_citeproc", None)
+    same_pdf_output_dir = getattr(args, "same_pdf_output_dir", False)
+    config = Configuration(watch_dir=watch_dir,
+                           output_dir=output_dir,
+                           config_file=args.config_file,
+                           pandoc_path=pandoc_path,
+                           pandoc_version=pandoc_version,
+                           no_citeproc=no_citeproc,
+                           csl_dir=args.csl_dir,
+                           templates_dir=args.templates_dir,
+                           post_processor=args.post_processor,
+                           same_pdf_output_dir=same_pdf_output_dir,
+                           dry_run=args.dry_run)
+    set_log_levels_and_maybe_log_pandoc_output(args, config, out)
+    return config, (out, err)
 
 
 def add_common_args(parser):
-    parser.add_argument(
-        "--pandoc-path", dest="pandoc_path",
-        required=False,
-        help="Provide custom pandoc path. Must be full path to executable")
-    parser.add_argument(
-        "-o", "--output-dir", dest="output_dir", default=".",
-        help="Directory for output files. Defaults to current directory")
-    parser.add_argument(
-        "--no-citeproc", action="store_true", dest="no_citeproc",
-        help="Whether to process the citations via citeproc.")
-    parser.add_argument(
-        "-g", "--generation", dest="generation",
-        default="pdf",
-        help=f"Which formats to output. Can be one of [{', '.join(gentypes)}].\n" +
-        "Defaults to pdf. You can choose multiple generation at once.\n" +
-        "E.g., 'pndconf -g pdf,html' or 'pndconf -g beamer,reveal'")
-    parser.add_argument(
-        "-p", "--post-processor", default="",
-        help="python module (or filename, must be in path) from which to load\n" +
-        "post_processor function should be named \"post_processor\"")
-    parser.add_argument(
-        "--templates-dir",
-        help="Directory where templates are placed")
-    parser.add_argument("--csl-dir",
-                        help="Directory where csl files are placed")
-    parser.add_argument("--config-file", "-c", dest="config_file",
-                        help="Config file to read.\n" +
-                        "A default configuration is provided with the distribution.\n" +
-                        "Print \"pndconf --dump-default-config\" to view the default config.")
-    parser.add_argument("-po", "--print-pandoc-opts", dest="print_pandoc_opts",
-                        action="store_true",
-                        help="Print pandoc options and exit")
-    parser.add_argument("-pg", "--print-generation-opts",
-                        action="store_true",
-                        help="Print pandoc options for filetype (e.g., for 'pdf') and exit")
-    parser.add_argument("-L", "--log-file", dest="log_file",
-                        type=str,
-                        default="",
-                        help="Log file to output instead of stdout. Optional")
-    parser.add_argument("-l", "--log-level", dest="log_level",
-                        default="warning",
-                        help="Debug Level. One of: error, warning, info, debug")
-    parser.add_argument("--same-output-dir", action="store_true", dest="same_output_dir",
-                        help="Output tex files and pdf to same dir as markdown file.\n" +
+    parser.add_argument("-o", "--output-dir",
+                        dest="output_dir", default=".",
+                        help="Directory for output files. Defaults to current directory")
+    parser.add_argument("--no-citeproc", action="store_true", dest="no_citeproc",
+                        help="Whether to process the citations via citeproc.")
+    parser.add_argument("--shell-pdflatex", action="store_true", dest="shell_pdflatex",
+                        help="Use pdflatex via shell command instead of pandoc interface.\n"
+                        "pandoc's internal compilation system with pdflatex doesn't ignore")
+    parser.add_argument("-g", "--generation",
+                        dest="generation", default="pdf",
+                        help=f"Which formats to output. Can be [{', '.join(gentypes)}].\n"
+                        "Defaults to pdf. You can choose multiple generation at once.\n"
+                        "E.g., 'pndconf -g pdf,html' or 'pndconf -g beamer,reveal'")
+    parser.add_argument("--same-pdf-output-dir", action="store_true", dest="same_pdf_output_dir",
+                        help="Output tex files and pdf to same dir as markdown file.\n"
                         "Default is to create a separate folder with a \"_files\" suffix")
 
 
-def convert(arglist, gopts=None):
+def common_args_parser():
+    """Hacky common args parser.
+
+    Only to generate default arguments before actual commands are called, all
+    because I didn't want to put the generation/output etc. opts before the
+    commands.
+
+    """
+    parser = MyParser(allow_abbrev=False,
+                      add_help=False,
+                      formatter_class=argparse.RawTextHelpFormatter)
+    add_common_args(parser)
+    return parser
+
+
+def add_convert_parser(subparsers):
     description = "Convert files with pandoc"
-    parser = argparse.ArgumentParser(
-        usage=usage,
-        description=description,
-        allow_abbrev=False,
-        formatter_class=argparse.RawTextHelpFormatter)
+    convert_usage = """
+    pndconf [global_opts] convert [opts] [pandoc_opts]
+
+    Example:
+        # To convert a single file yourfile.md to yourfile.pdf
+        pndconf convert -g pdf yourfile.md
+
+        # To convert a multiple files
+        pndconf convert -g pdf yourfile.md,otherfile.md
+
+        # To convert to multiple formats
+
+        pndconf convert -g pdf,html yourfile.md
+"""
+    parser = subparsers.add_parser("convert",
+                                   usage=convert_usage,
+                                   description=description,
+                                   allow_abbrev=False,
+                                   formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("input_files", help="Comma separated list of input files.")
-    add_common_args(parser)
     parser.add_argument("--no-cite-cmd",
                         action="store_true",
-                        help="Don't run extra bibtex or biber commands for citations.\n" +
-                        "Helpful when pdflatex is run with bibtex etc. and references need not be updated.")
-    args, extra = parser.parse_known_args(arglist)
-    args.watch_dir = None
-    args.dry_run = gopts and gopts.dry_run
-    args.exclude_regexp = None
-    args.inclusions = None
-    args.exclusions = None
-    config = get_config(args, extra)
-    config.no_cite_cmd = args.no_cite_cmd
-    input_files = args.input_files.split(",")
-    not_input_files = [x for x in input_files if not os.path.exists(x)]
-    if not_input_files:
-        loge(f"{not_input_files} don't exist. Ignoring")
-    input_files = [x for x in input_files if os.path.exists(x)]
-    if not input_files:
-        loge("Error! No input files present or given")
-    elif not all(x.endswith(".md") for x in input_files):
-        loge("Error! Some input files not markdown")
-    else:
-        logbi(f"Will compile {input_files} to {config.output_dir} once.")
-        config.compile_files(input_files)
+                        help="Don't run extra bibtex or biber commands for citations.\n"
+                        "Helpful when pdflatex is run with bibtex etc."
+                        "and references need not be updated.")
+    add_common_args(parser)
 
 
-def watch(arglist, gopts=None):
+def add_watch_parser(subparsers):
     description = "Watch files for changes and convert with pandoc"
-    parser = argparse.ArgumentParser(
-        usage=usage,
-        description=description,
-        allow_abbrev=False,
-        formatter_class=argparse.RawTextHelpFormatter)
-    add_common_args(parser)
+    watch_usage = """
+    pndconf [global_opts] watch [opts] [pandoc_opts]
+
+    Example:
+        # To watch in current directory and generate pdf and html outputs
+        pndconf watch -g pdf,html
+
+        # To watch in some input directory and generate pdf and beamer outputs
+        # to some other output directory
+        pndconf watch -g pdf,beamer -w /path/to/watch_dir -o output_dir
+"""
+    parser = subparsers.add_parser("watch",
+                                   description=description,
+                                   allow_abbrev=False,
+                                   usage=watch_usage,
+                                   formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("-i", "--input-files", default="",
-                        help="Comma separated list of input files.\n" +
-                        "If given, only these files are watched.")
+                              help="Comma separated list of input files.\n"
+                              "If given, only these files are watched.")
     parser.add_argument("-w", "--watch-dir", default=".", dest="watch_dir",
-                        help="Directory to watch. Watch current directory if not specified.")
+                              help="Directory to watch. Watch current directory if not specified.")
     parser.add_argument("--ignore-extensions", dest="exclusions",
-                        default=".pdf,.tex,doc,bin,common", required=False,
-                        help="The extensions (.pdf for pdf files) or the folders to " +
-                        "exclude from watch operations separated with commas")
+                              default=".pdf,.tex,doc,bin,common", required=False,
+                              help="The extensions (.pdf for pdf files) or the folders to"
+                              " exclude from watch operations separated with commas")
     parser.add_argument("--watch-extensions", dest="inclusions",
-                        default=".md", required=False,
-                        help="The extensions to watch. Only markdown (.md) is supported for now")
+                              default=".md", required=False,
+                              help="The extensions to watch. Only markdown (.md) is supported for now")
     parser.add_argument("--exclude-regexp", dest="exclude_regexp",
-                        default="#,~,readme.md,changelog.md", required=False,
-                        help="Files with specific regex to exclude. Should not contain ','")
-    parser.add_argument("--no-exclude-ignore-case", action="store_false", dest="exclude_ignore_case",
-                        help="Whether the exclude regexp should ignore case or not.")
+                              default="#,~,readme.md,changelog.md", required=False,
+                              help="Files with specific regex to exclude. Should not contain ','")
+    parser.add_argument("--no-exclude-ignore-case", action="store_false",
+                              dest="exclude_ignore_case",
+                              help="Whether the exclude regexp should ignore case or not.")
     parser.add_argument("--exclude-files", dest="excluded_files",
-                        default="",
-                        help="Specific files to exclude from watching")
-    args, extra = parser.parse_known_args(arglist)
-    args.dry_run = gopts and gopts.dry_run
-    config = get_config(args, extra)
-    input_files = args.input_files.split(",")
-    logi(f"\nWatching in {os.path.abspath(config.watch_dir)}")
-    if input_files:
-        watched_elements = input_files
+                              default="",
+                              help="Specific files to exclude from watching")
+    add_common_args(parser)
 
-        def is_watched(x):
-            return os.path.abspath(x) in watched_elements
 
-        def get_watched(x):
-            return [os.path.abspath(x) for x in input_files]
-    else:
-        watched_elements = [os.path.basename(w) for w in config.get_watched()]
-        is_watched = config.is_watched
-        get_watched = config.get_watched
-    logi(f"Watching: {watched_elements}")
-    logi(f"Will output to {os.path.abspath(config.output_dir)}")
-    logi("Starting pandoc watcher...")
-    event_handler = ChangeHandler(config.watch_dir, is_watched,
-                                  get_watched, config.compile_files,
-                                  config.log_level)
-    observer = Observer()
-    observer.schedule(event_handler, str(config.watch_dir), recursive=True)
-    observer.start()
-    try:
-        while True:
-            time.sleep(1)
-    except KeyboardInterrupt as err:
-        logi(str(err))
-        # NOTE: Start simple server here when added and asked
-        observer.stop()
-    logi("Stopping pandoc watcher ...")
-    exit(0)
+def check_and_dispatch_command(args, extra, short_help):
+    config, out_err = get_config_and_pandoc_output(args)
 
+    common_args, _ = common_args_parser().parse_known_args()
 
-def gopts_parser(arglist):
-    parser = argparse.ArgumentParser("File watcher", add_help=False)
+    if args.dump_default_config:
+        with open(Path(__file__).parent.joinpath("config_default.ini")) as f:
+            print(f.read())
+        sys.exit(0)
+    if args.print_pandoc_opts:
+        print_pandoc_opts(*out_err)
+        sys.exit(0)
+    if args.print_generation_opts:
+        print_generation_opts(common_args, config)
+        sys.exit(0)
+    if not args.command:
+        loge("No command given. Issue a command or a switch.\n")
+        print(short_help)
+        sys.exit(1)
+    if not common_args.generation:
+        loge("Generation options cannot be empty")
+        sys.exit(1)
+
+    maybe_exit_for_unknown_generation_type(args)
+    validate_extra_args(extra)
+    logbi(f"Will generate for {args.generation.upper()}")
+    logbi(f"Extra pandoc args are {extra}")
+
+    # Update generation options, it'll generate everything by default
+    config.update_generation_options(args.generation.split(','), extra)
+
+    if args.command == "watch":
+        watch(args, config)
+    elif args.command == "convert":
+        convert(args, config)
+
+
+class MyParser(argparse.ArgumentParser):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def error(self, message):
+        loge(message)
+        print("")
+        self.print_usage(sys.stderr)
+        sys.exit(1)
+
+
+def main():
+    description = "pndconf: Pandoc Configuration Manager and File Watcher"
+    # parser = argparse.ArgumentParser(description,
+    parser = MyParser(description,
+                      usage=usage,
+                      allow_abbrev=False,
+                      add_help=False,
+                      formatter_class=argparse.RawTextHelpFormatter)
+    shorter_help = parser.format_help()
     parser.add_argument("-h", "--help", action="store_true",
                         help="Display help and exit")
+    parser.add_argument("--long-help", action="store_true",
+                        help="Display all the global options")
+    parser.add_argument("-c", "--config-file", dest="config_file",
+                        help="Config file to read. "
+                        "A default configuration is provided with the distribution.\n"
+                        "Print \"pndconf --dump-default-config\" to view the default config.")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="Verbose output")
     parser.add_argument("-vv", "--loud", action="store_true",
                         help="More verbose")
-    parser.add_argument("--dry-run", "-n", action="store_true",
+    parser.add_argument("-vvv", "--shout", action="store_true",
+                        help="Even more verbose")
+    parser.add_argument("-n", "--dry-run", action="store_true",
                         help="Dry run. Don't actually do anything.")
     parser.add_argument("--dump-default-config", action="store_true",
                         help="Dump given config or default config.")
-    # parser.add_argument(
-    #     "--pandoc-path", dest="pandoc_path",
-    #     required=False,
-    #     help="Provide custom pandoc path. Must be full path to executable")
-    # parser.add_argument("-po", "--print-pandoc-opts", dest="print_pandoc_opts",
-    #                     action="store_true",
-    #                     help="Print pandoc options and exit")
-    args = parser.parse_args(arglist)
-    if args.dump_default_config:
-        with open(Path(__file__).parent.joinpath("config_default.ini")) as f:
-            print(f.read())
+    short_help = parser.format_help()
+    parser.add_argument("--pandoc-path", dest="pandoc_path",
+                        default="/usr/bin/pandoc",
+                        help="Provide custom pandoc path. Must be full path to executable")
+    parser.add_argument("-po", "--print-pandoc-opts", dest="print_pandoc_opts",
+                        action="store_true",
+                        help="Print pandoc options and exit")
+    parser.add_argument("-p", "--post-processor",
+                        dest="post_processor", default="",
+                        help="python module (or filename, must be in path) from which to load\n"
+                        "post_processor function should be named \"post_processor\"")
+    parser.add_argument("--templates-dir",
+                        help="Directory where templates are placed")
+    parser.add_argument("--csl-dir",
+                        help="Directory where csl files are placed")
+    parser.add_argument("-pg", "--print-generation-opts",
+                        action="store_true",
+                        help="Print pandoc options for filetype (e.g., for 'pdf') and exit")
+    parser.add_argument("-L", "--log-file",
+                        dest="log_file", default="",
+                        help="Log file to output instead of stdout. Optional")
+    parser.add_argument("-l", "--log-level",
+                        dest="log_level", default="warning",
+                        choices=log_levels,
+                        help="Debug Level")
+    parser.add_argument("--version",
+                        action="store_true",
+                        help="Print version and exit")
+    long_help = parser.format_help()
+    subparsers = parser.add_subparsers(help="Sub Commands", dest="command")
+    add_watch_parser(subparsers)
+    add_convert_parser(subparsers)
+    args, extra = parser.parse_known_args()
+    if args.help:
+        print(description)
+        print("\n", short_help)
         sys.exit(0)
-    parser.usage = ""
-    args.help = parser.format_help().replace("usage: \n\n", "").replace("optional arguments:\n", "")
-    # import ipdb; ipdb.set_trace()
-    # if args.print_pandoc_opts:
-    #     out, err = Popen([str(pandoc_path), "--help"], stdout=PIPE, stderr=PIPE).communicate()
-    #     out = out.decode("utf-8")
-    #     err = err.decode("utf-8")
-    #     if err:
-    #         loge(f"Pandoc exited with error {err}")
-    #     else:
-    #         loge(f"Pandoc options are \n{out}")
-    #     sys.exit(0)
-    return args
+    if args.long_help:
+        print(description, "\n")
+        print("Global options:\n" + long_help.replace(shorter_help, ""))
+        sys.exit(0)
+    if args.version:
+        print(f"pndconf version {__version__}")
+        sys.exit(0)
+    check_and_dispatch_command(args, extra, short_help)
 
 
-def main():
-    cmds = {"convert": convert, "watch": watch}
-    parser = hierarchical_parser("pndconf", usage, cmds, gopts_parser, __version__)
-    parser()
+if __name__ == '__main__':
+    main()
```

### Comparing `pndconf-0.4.5/pndconf/transforms.py` & `pndconf-0.5.0/pndconf/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -242,16 +242,16 @@
 def load_abbrevs(abbrevs_file):
     import csv
     lines = []
     with open(abbrevs_file) as f:
         reader = csv.reader(f, delimiter=";")
         for line in reader:
             lines.append(line)
-    return dict((re.sub("-$", ".+", x[0].lower()), x[1].lower())
-                for x in lines if "eng" in x[-1] or x[-1] == "mul")
+    return {re.sub("-$", ".+", x[0].lower()): x[1].lower()
+            for x in lines if "eng" in x[-1] or x[-1] == "mul"}
 
 
 def get_abbrev(abbrev_regexps, word):
     for k, v in abbrev_regexps.items():
         if re.match(k, word, flags=re.IGNORECASE):
             return v
 
@@ -262,29 +262,33 @@
         if not match and w not in abbrevs or abbrevs[w] is None:
             abbrev = get_abbrev(abbrev_regexps, w)
             if abbrev:
                 abbrevs[w.lower()] = abbrev.lower()
                 abbrevs[w.capitalize()] = abbrev.capitalize()
 
 
+def fix_cvf(x: str):
+    if "ieee/cvf" in x.lower():
+        return x.replace("ieee/cvf", "IEEE").replace("IEEE/CVF", "IEEE")
+
+
 def normalize(ent: Dict[str, str]):
     """Replaces newlines in entries with a space. (for now)"""
     for k, v in ent.items():
         ent[k] = v.replace("\n", " ")
     return ent
 
 
-def fix_cvf(x):
-    if "ieee/cvf" in x.lower():
-        return x.replace("ieee/cvf", "IEEE").replace("IEEE/CVF", "IEEE")
-
-
-def fix_venue(ent, contract=False):
+def fix_venue(ent: Dict[str, str], contract: bool = False):
     """Fix venue if it's a known venue.
 
+    Args:
+        ent: Bibtex Entry as a dictionary. It's modified in place.
+        contract: Flag to signal contraction of venue.
+
     Fix name of conference or journal to standard nomenclature for that venue
     and also change the venue type to correct one of \"inproceedings\" or
     "journal".
 
     E.g., CVPR is often listed as "CVPR", "Computer Vision and Pattern Recognition",
     "IEEE Internation Conference on Computer Vision and Pattern Recognition",
     "IEEE/CVF Internation Conference on Computer Vision and Pattern Recognition" etc.
@@ -292,15 +296,15 @@
     Instead, if the abbreviation or the some version of the venue is found, then
     replace with the canonical version.
 
     If :code:`contract` is given, then Change the venue name to a contraction
     instead.
 
     """
-    venue = ent.get("booktitle", None) or ent.get("journal", None)
+    venue = ent.get("booktitle", None) or ent.get("journal", None) or ent.get("venue", None)
     if venue:
         venue = venue.replace("{", "").replace("}", "")
         for k, v in venues.items():
             rule = v["rule"]
             vtype = v["type"]
             if rule(venue):
                 vname = v["contraction"] if contract else v["name"]
@@ -316,30 +320,30 @@
                     ent["journal"] = vname
                 else:
                     raise AttributeError(f"Unknown venue type of {ent['ENTRYTYPE']}")
                 break
     return ent
 
 
-def standardize_venue(ent):
+def standardize_venue(ent: Dict[str, str]):
     """Change the venue name to a standard name.
 
     See :func:`fix_venue`.
 
     """
     return fix_venue(ent)
 
 
-def contract_venue(ent):
+def contract_venue(ent: Dict[str, str]):
     """Change the venue name to a contraction.
 
     See :func:`fix_venue`.
 
     """
-    return fix_venue(ent, True)
+    return fix_venue(ent, contract=True)
 
 
 def change_to_title_case(ent: Dict[str, str]) -> Dict[str, str]:
     """Change some values in a bibtex entry to title case.
 
     Title, Booktitle, and Journal are changed.
 
@@ -350,45 +354,67 @@
     for key in ["title", "booktitle", "journal"]:
         if key in ent:
             val = ent[key]
             temp: List[str] = []
             capitalize_next = False
             for i, x in enumerate(filter(lambda x: x and not re.match(r"^ +$", x),
                                          re.split(r"( +|-)", val))):
-                if x.startswith("{") or x.upper() == x:
-                    temp.append(x)
-                elif i == 0 or capitalize_next:
-                    temp.append(x.capitalize())
-                elif not (x in stop_words_set):
-                    temp.append(x.capitalize())
-                else:
-                    temp.append(x)
-                if x.endswith(".") or x.endswith(":"):
-                    capitalize_next = True
-                else:
-                    capitalize_next = False
+                cap = (not i) or capitalize_next or x not in stop_words_set
+                y = x.capitalize() if cap else x
+                temp.append(y)
+                capitalize_next = bool(x.endswith((".", ":")))
             ent[key] = " ".join([x if x.startswith("{") else "{" + x + "}" for x in temp])
     return ent
 
 
-def abbreviate_venue(ent):
+def abbreviate_venue(ent: Dict[str, str]) -> Dict[str, str]:
     if ent["ENTRYTYPE"] == "inproceedings":
         vkey = "booktitle"
     elif ent["ENTRYTYPE"] == "article":
         vkey = "journal"
     else:
         return ent
     try:
         words = ent[vkey].split()
     except Exception:
-        import ipdb; ipdb.set_trace()
+        raise AttributeError(f"{vkey} not in entry")
     for i, w in enumerate(words):
         term = re.sub(r"{(.+)}", r"\1", w)
         found = term in abbrevs and abbrevs[term] != "n.a." and abbrevs[term]
         if found:
             words[i] = "{" + found + "}"
     ent[vkey] = " ".join(words)
     return ent
 
 
-def check_author_names(ent):
+def date_to_year_month(ent: Dict[str, str]) -> Dict[str, str]:
+    months = dict(zip(range(1, 13), [x[:3] for x in ["January", "February",
+                                                     "March", "April", "May", "June", "July", "August",
+                                                     "September", "October", "November", "December"]]))
+    if "date" in ent:
+        date = ent.pop("date").split("-")
+        if len(date) == 1:
+            ent["year"] = date[0]
+        else:
+            year, month = date[0], date[1]
+            ent["year"] = year
+            ent["month"] = months[int(month)]
+    return ent
+
+
+def remove_keys(ent: Dict[str, str], keys: List[str]) -> Dict[str, str]:
+    for key in keys:
+        if key in ent:
+            ent.pop(key)
+    return ent
+
+
+def remove_url(ent: Dict[str, str]) -> Dict[str, str]:
+    if "url" in ent:
+        url = ent.pop("url")
+        if ent["ENTRYTYPE"] == "misc" and "howpublished" not in ent:
+            ent["howpublished"] = f'\\url{{{url}}}'
+    return ent
+
+
+def check_author_names(ent: Dict[str, str]):
     check_for_unicode = None
```

### Comparing `pndconf-0.4.5/pndconf/watcher.py` & `pndconf-0.5.0/pndconf/watcher.py`

 * *Files identical despite different names*

### Comparing `pndconf-0.4.5/setup.py` & `pndconf-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bibtexparser>=1.2.0,<2.0.0',
  'chardet>=4.0.0,<5.0.0',
  'common-pyutil>=0.8.0,<0.9.0',
- 'pandoc-eqnos>=2.5.0,<3.0.0',
- 'pandocfilters>=1.5.0,<2.0.0',
  'pyyaml>=5.4.0,<6.0.0',
  'watchdog>=2.1.5,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['pndconf = pndconf.__main__:main']}
 
 setup_kwargs = {
     'name': 'pndconf',
-    'version': '0.4.5',
+    'version': '0.5.0',
     'description': '',
     'long_description': None,
     'author': 'Akshay',
     'author_email': 'akshay.badola.cs@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pndconf-0.4.5/PKG-INFO` & `pndconf-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pndconf
-Version: 0.4.5
+Version: 0.5.0
 Summary: 
 License: MIT
 Author: Akshay
 Author-email: akshay.badola.cs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: bibtexparser (>=1.2.0,<2.0.0)
 Requires-Dist: chardet (>=4.0.0,<5.0.0)
 Requires-Dist: common-pyutil (>=0.8.0,<0.9.0)
-Requires-Dist: pandoc-eqnos (>=2.5.0,<3.0.0)
-Requires-Dist: pandocfilters (>=1.5.0,<2.0.0)
 Requires-Dist: pyyaml (>=5.4.0,<6.0.0)
 Requires-Dist: watchdog (>=2.1.5,<3.0.0)
```

