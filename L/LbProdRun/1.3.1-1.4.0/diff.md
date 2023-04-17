# Comparing `tmp/LbProdRun-1.3.1.tar.gz` & `tmp/LbProdRun-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbProdRun-1.3.1.tar", last modified: Thu Aug 25 07:31:55 2022, max compression
+gzip compressed data, was "LbProdRun-1.4.0.tar", last modified: Mon Apr 17 15:58:42 2023, max compression
```

## Comparing `LbProdRun-1.3.1.tar` & `LbProdRun-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 07:31:55.264000 LbProdRun-1.3.1/
--rw-r--r--   0 root         (0) root         (0)     2055 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2482 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    16310 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      388 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35149 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2655 2022-08-25 07:31:55.264000 LbProdRun-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2233 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)      304 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1105 2022-08-25 07:31:55.264000 LbProdRun-1.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 07:31:55.260000 LbProdRun-1.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 07:31:55.264000 LbProdRun-1.3.1/src/LbProdRun/
--rw-r--r--   0 root         (0) root         (0)    11401 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/src/LbProdRun/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1281 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/src/LbProdRun/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4652 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/src/LbProdRun/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 07:31:55.264000 LbProdRun-1.3.1/src/LbProdRun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2655 2022-08-25 07:31:55.000000 LbProdRun-1.3.1/src/LbProdRun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2022-08-25 07:31:55.000000 LbProdRun-1.3.1/src/LbProdRun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-25 07:31:55.000000 LbProdRun-1.3.1/src/LbProdRun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2022-08-25 07:31:55.000000 LbProdRun-1.3.1/src/LbProdRun.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      155 2022-08-25 07:31:55.000000 LbProdRun-1.3.1/src/LbProdRun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-08-25 07:31:55.000000 LbProdRun-1.3.1/src/LbProdRun.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-25 07:31:55.264000 LbProdRun-1.3.1/tests/
--rw-r--r--   0 root         (0) root         (0)     4749 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3028 2022-08-25 07:31:39.000000 LbProdRun-1.3.1/tests/test_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    16310 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-17 15:58:42.928000 LbProdRun-1.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.920000 LbProdRun-1.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/src/LbProdRun/
+-rw-r--r--   0 root         (0) root         (0)    12037 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/src/LbProdRun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/src/LbProdRun/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/src/LbProdRun/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/src/LbProdRun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/tests/test_options.py
```

### Comparing `LbProdRun-1.3.1/.gitignore` & `LbProdRun-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/.gitlab-ci.yml` & `LbProdRun-1.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/.pre-commit-config.yaml` & `LbProdRun-1.4.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 # See https://pre-commit.com/hooks.html for more hooks
 
 default_language_version:
   python: python3.9
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: no-commit-to-branch
         args: [--branch, main]
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/pycQA/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-bugbear]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.960
+    rev: v1.0.1
     hooks:
       - id: mypy
         args: [--strict-optional, --ignore-missing-imports]
         additional_dependencies: [types-PyYAML, pydantic]
 
   - repo: "https://gitlab.cern.ch/lhcb-core/LbDevTools.git"
-    rev: 2.0.34
+    rev: 2.0.38
     hooks:
       - id: lb-add-copyright
```

### Comparing `LbProdRun-1.3.1/.pylintrc` & `LbProdRun-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/LICENSE` & `LbProdRun-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/PKG-INFO` & `LbProdRun-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.3.1
+Version: 1.4.0
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.3.1/README.md` & `LbProdRun-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/setup.cfg` & `LbProdRun-1.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 [options.entry_points]
 console_scripts = 
 	lb-prod-run = LbProdRun.__main__:app
 
 [flake8]
 max-line-length = 80
-ignore = E501,W503,B950,B008,R0903
+ignore = E501,W503,B950,B008,B905
 extend-ignore = 
 	E203,
 select = C,E,F,W,B,B9
 exclude = 
 	.pyre/
 
 [isort]
```

### Comparing `LbProdRun-1.3.1/src/LbProdRun/__init__.py` & `LbProdRun-1.4.0/src/LbProdRun/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 import os
 import re
 import shlex
+import shutil
 from pathlib import Path
 from pprint import pformat
 from typing import Union
 
 import typer
 import yaml
 from packaging.version import Version
 
 from .models import JobSpecV1, read_jobspec
 
 
-def run_job(spec_file: Path, dry_run=False, verbose=False, interactive=False):
+def run_job(
+    spec_file: Path, dry_run=False, verbose=False, interactive=False, prmon=False
+):
     job_spec = read_jobspec(spec_file)
     if verbose:
         typer.secho("Expanded spec file as:", fg=typer.colors.GREEN)
         typer.secho(pformat(job_spec.dict()))
-    execute(job_spec, dry_run=dry_run, interactive=interactive)
+    execute(job_spec, dry_run=dry_run, interactive=interactive, prmon=prmon)
 
 
 def _write_prod_conf_options(job_spec, path: Path, verbose=False):
     """Write an options file for the ProdConf data package"""
     data = {
         "Application": job_spec.application.name,
         "AppVersion": job_spec.application.version,
@@ -60,24 +63,39 @@
 
     if verbose:
         typer.secho(f"Going to write in {path}", fg=typer.colors.GREEN)
         typer.secho(string)
     path.write_text(string)
 
 
-def execute(job_spec, dry_run=False, interactive=False):
+def execute(job_spec, dry_run=False, interactive=False, prmon=False):
+    command = []
+    new_style = _is_new_style(job_spec.application.name, job_spec.application.version)
+
+    if not prmon:
+        pass
+    elif interactive:
+        typer.secho("Not using prmon as this is an interactive run!", fg="yellow")
+    elif shutil.which("prmon") is None:
+        typer.secho("Not using prmon as it wasn't found on $PATH!", fg="yellow")
+    else:
+        command += ["prmon", "--interval", "60"]
+        command += ["--filename", f"prmon_{job_spec.output.prefix}.txt"]
+        command += ["--"]
+
     if isinstance(job_spec.application, JobSpecV1.FullDevApplication):
-        command = [str(job_spec.application.run_script.absolute())]
+        command += [str(job_spec.application.run_script.absolute())]
     else:
-        command = ["lb-run"]
+        command += ["lb-run"]
         command += ["--siteroot=/cvmfs/lhcb.cern.ch/lib/"]
         command += ["-c", f"{job_spec.application.binary_tag}"]
         for ep in job_spec.application.data_pkgs:
             command += [f"--use={ep}"]
-        command += ["--use=ProdConf"]
+        if not new_style:
+            command += ["--use=ProdConf"]
 
         if isinstance(job_spec.application, JobSpecV1.ReleaseApplication):
             typer.secho(
                 f"Executing application {job_spec.application.name} "
                 f"{job_spec.application.version} for binary tag configuration "
                 f"{job_spec.application.binary_tag}"
             )
@@ -95,15 +113,15 @@
             )
 
             command += ["--path-to-project"]
             command += [str(job_spec.application.project_base.absolute())]
         else:
             raise NotImplementedError(type(job_spec.application))
 
-    if _is_new_style(job_spec.application.name, job_spec.application.version):
+    if new_style:
         inner_command = _make_lbexec_command(job_spec)
     else:
         inner_command = _make_gaudirun_command(job_spec)
 
     if interactive:
         command += ["bash", "--norc", "--noprofile"]
         typer.secho("Starting application environment with:")
@@ -132,16 +150,17 @@
     options_yaml_fn = Path(f"lbexec_options_{job_spec.output.prefix}.yaml")
     _write_options_yaml(job_spec, options_yaml_fn, verbose=False)
     command = ["lbexec", job_spec.options.entrypoint, str(options_yaml_fn)]
     return command + job_spec.options.extra_args
 
 
 def _write_options_yaml(job_spec, path: Path, verbose=False):
-    """Write an options file for the ProdConf data package"""
+    """Write an options file for lbexec"""
     options = job_spec.options.extra_options.copy()
+    options["write_decoding_keys_to_git"] = False
 
     if job_spec.input.files:
         options["input_files"] = job_spec.input.files
     if job_spec.db_tags.dddb_tag:
         options["dddb_tag"] = job_spec.db_tags.dddb_tag
     if job_spec.db_tags.conddb_tag:
         options["conddb_tag"] = job_spec.db_tags.conddb_tag
@@ -238,14 +257,16 @@
 
 def _is_new_style(name: str, version: str) -> bool:
     """Determine if a given application/version combination should use lbexec"""
     try:
         parsed_version = Version(re.sub(r"[^\d]+", ".", version).strip("."))
     except Exception:  # pylint: disable=broad-except
         typer.secho(f"Failed to parse {version!r}", fg="red")
+        if version == "HEAD":
+            return True
         return False
 
     version_compatibility: dict[str, Union[bool, Version]] = {
         "Analysis": Version("40"),
         "DaVinci": Version("60"),
         "Lbcom": Version("33"),
         "LHCb": Version("53"),
```

### Comparing `LbProdRun-1.3.1/src/LbProdRun/__main__.py` & `LbProdRun-1.4.0/src/LbProdRun/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 app = typer.Typer()
 
 
 @app.command()
 def main(
     job_spec: Path = typer.Argument(..., exists=True, dir_okay=False, readable=True),
     dry_run: bool = False,
+    prmon: bool = False,
     verbose: bool = False,
     interactive: bool = False,
 ):
     typer.echo(f"Reading specification from {job_spec}")
-    run_job(job_spec, dry_run=dry_run, verbose=verbose, interactive=interactive)
+    run_job(
+        job_spec, dry_run=dry_run, prmon=prmon, verbose=verbose, interactive=interactive
+    )
 
 
 if __name__ == "__main__":
     app()  # pragma: no cover
```

### Comparing `LbProdRun-1.3.1/src/LbProdRun/models.py` & `LbProdRun-1.4.0/src/LbProdRun/models.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/src/LbProdRun.egg-info/PKG-INFO` & `LbProdRun-1.4.0/src/LbProdRun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.3.1
+Version: 1.4.0
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.3.1/tests/test_cli.py` & `LbProdRun-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.3.1/tests/test_options.py` & `LbProdRun-1.4.0/tests/test_options.py`

 * *Files identical despite different names*

