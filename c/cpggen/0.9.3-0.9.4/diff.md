# Comparing `tmp/cpggen-0.9.3.tar.gz` & `tmp/cpggen-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.9.3.tar", max compression
+gzip compressed data, was "cpggen-0.9.4.tar", max compression
```

## Comparing `cpggen-0.9.3.tar` & `cpggen-0.9.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-16 23:15:12.958443 cpggen-0.9.3/LICENSE
--rw-r--r--   0        0        0     6774 2023-04-16 23:15:12.958443 cpggen-0.9.3/README.md
--rw-r--r--   0        0        0        0 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/__init__.py
--rw-r--r--   0        0        0    12897 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/cli.py
--rw-r--r--   0        0        0    29008 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/logger.py
--rw-r--r--   0        0        0    11089 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-16 23:15:12.958443 cpggen-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     8102 1970-01-01 00:00:00.000000 cpggen-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 10:17:36.727332 cpggen-0.9.4/LICENSE
+-rw-r--r--   0        0        0     6972 2023-04-17 10:17:36.731332 cpggen-0.9.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/__init__.py
+-rw-r--r--   0        0        0    12908 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/cli.py
+-rw-r--r--   0        0        0    30379 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/logger.py
+-rw-r--r--   0        0        0    11089 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-17 10:17:36.731332 cpggen-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     8300 1970-01-01 00:00:00.000000 cpggen-0.9.4/PKG-INFO
```

### Comparing `cpggen-0.9.3/LICENSE` & `cpggen-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.3/README.md` & `cpggen-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 Bundled container image
 
 ```
 docker pull ghcr.io/appthreat/cpggen
 # podman pull ghcr.io/appthreat/cpggen
 ```
 
+Almalinux 9 requires the CPU to support SSE4.2. For kvm64 VM use the Almalinux 8 version instead.
+
+```
+docker pull ghcr.io/appthreat/cpggen-alma8
+# podman pull ghcr.io/appthreat/cpggen-alma8
+```
+
 Or use the nightly to always get the latest joern and tools.
 
 ```
 docker pull ghcr.io/appthreat/cpggen:nightly
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
@@ -106,15 +113,15 @@
 docker run --rm -it -v /tmp:/tmp -v $(pwd):/app:rw --cpus=4 --memory=16g -t ghcr.io/appthreat/cpggen cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
 ### Export graphs
 
 By passing `--export`, cpggen can export the various graphs to many formats using [joern-export](https://docs.joern.io/exporting/)
 
-Example to export `all` graphs in `dot` format
+Example to export `cpg14` graphs in `dot` format
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out
 ```
 
 To export `pdg` in `neo4jcsv` format
```

### Comparing `cpggen-0.9.3/cpggen/cli.py` & `cpggen-0.9.4/cpggen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,17 +97,17 @@
         action="store_true",
         default=True if os.getenv("CPG_EXPORT") in ("true", "1") else False,
         dest="export",
         help="Export CPG as a graph",
     )
     parser.add_argument(
         "--export-repr",
-        default=os.getenv("CPG_EXPORT_REPR", "all"),
+        default=os.getenv("CPG_EXPORT_REPR", "cpg14"),
         dest="export_repr",
-        choices=["ast", "cfg", "cdg", "ddg", "pdg", "cpg", "all"],
+        choices=["ast", "cfg", "cdg", "ddg", "pdg", "cpg", "cpg14", "all"],
         help="Graph representation to export",
     )
     parser.add_argument(
         "--export-format",
         default=os.getenv("CPG_EXPORT_FORMAT", "dot"),
         dest="export_format",
         choices=["neo4jcsv", "graphml", "graphson", "dot"],
```

### Comparing `cpggen-0.9.3/cpggen/executor.py` & `cpggen-0.9.4/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
     "export": "%(joern_home)sjoern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
     "qwiet": "sl analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
+    "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "java": {
         "maven": [
             get("MVN_CMD", "%(maven_cmd)s"),
@@ -218,14 +219,40 @@
                 LOG.info(cp.stderr)
             else:
                 LOG.info(f"{app_manifest['app']} uploaded successfully")
     except Exception as e:
         LOG.error(e)
 
 
+def dot_convert(export_out_dir, env):
+    if check_command("dot"):
+        dot_files = find_files(export_out_dir, ".dot", False, False)
+        for df in dot_files:
+            convert_cmd_with_args = cpg_tools_map["dot2png"] % dict(
+                dot_file=df, png_out=df.replace(".dot", ".png")
+            )
+            try:
+                subprocess.run(
+                    convert_cmd_with_args.split(" "),
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                    cwd=export_out_dir,
+                    env=env,
+                    check=False,
+                    shell=False,
+                    encoding="utf-8",
+                )
+            except Exception as e:
+                LOG.debug(e)
+    else:
+        LOG.debug(
+            f"Install graphviz package and ensure the command `dot` is available in the PATH to convert to png automatically"
+        )
+
+
 def do_x_build(src, env, build_artefacts, tool_lang):
     tool_lang = tool_lang.split("-")[0]
     build_crashes = {}
     for k, v in build_artefacts.items():
         failed_modules = 0
         crashed_modules = 0
         build_sets = build_tools_map.get(tool_lang)
@@ -409,15 +436,15 @@
                     cmd_with_args = f"""{container_cli} run --rm -w {amodule} -v {tempfile.gettempdir()}:/tmp -v {amodule}:{amodule}:rw -v {os.path.abspath(cpg_out_dir)}:{os.path.abspath(cpg_out_dir)}:rw -t {os.getenv("CPGGEN_IMAGE", "ghcr.io/appthreat/cpggen")} {cmd_with_args}"""
                     # We need to fix joern_home to the directory inside the container
                     joern_home = ""
                 sbom_cmd_with_args = cpg_tools_map.get("sbom")
                 sbom_out = ""
                 manifest_out = ""
                 if tool_lang == "export":
-                    cpg_out = cpg_out_dir
+                    cpg_out = os.path.abspath(cpg_out_dir)
                 else:
                     cpg_out = (
                         cpg_out_dir
                         if cpg_out_dir.endswith(".bin.zip")
                         or cpg_out_dir.endswith(".bin")
                         or cpg_out_dir.endswith(".cpg")
                         else os.path.abspath(
@@ -508,18 +535,25 @@
                                 LOG.info("------------------------------")
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
                                     "Please report the above error to https://github.com/joernio/joern/issues"
                                 )
                         else:
-                            if os.path.exists(src):
+                            if os.path.exists(cpg_out_dir):
                                 LOG.info(
                                     f"CPG {src} successfully exported to {cpg_out_dir}"
                                 )
+                                progress.update(
+                                    task,
+                                    description="Convert exported graph to png",
+                                    completed=95,
+                                    total=100,
+                                )
+                                dot_convert(cpg_out_dir, env)
                             else:
                                 LOG.warn(
                                     f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually using the command {' '.join(cmd_list_with_args)}"
                                 )
                     except Exception as e:
                         LOG.warn(f"Unable to export {src} to {cpg_out_dir}")
                         LOG.error(e)
```

### Comparing `cpggen-0.9.3/cpggen/logger.py` & `cpggen-0.9.4/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.3/cpggen/utils.py` & `cpggen-0.9.4/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.3/pyproject.toml` & `cpggen-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.9.3"
+version = "0.9.4"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.9.3/PKG-INFO` & `cpggen-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.9.3
+Version: 0.9.4
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -61,14 +61,21 @@
 Bundled container image
 
 ```
 docker pull ghcr.io/appthreat/cpggen
 # podman pull ghcr.io/appthreat/cpggen
 ```
 
+Almalinux 9 requires the CPU to support SSE4.2. For kvm64 VM use the Almalinux 8 version instead.
+
+```
+docker pull ghcr.io/appthreat/cpggen-alma8
+# podman pull ghcr.io/appthreat/cpggen-alma8
+```
+
 Or use the nightly to always get the latest joern and tools.
 
 ```
 docker pull ghcr.io/appthreat/cpggen:nightly
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
@@ -138,15 +145,15 @@
 docker run --rm -it -v /tmp:/tmp -v $(pwd):/app:rw --cpus=4 --memory=16g -t ghcr.io/appthreat/cpggen cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
 ### Export graphs
 
 By passing `--export`, cpggen can export the various graphs to many formats using [joern-export](https://docs.joern.io/exporting/)
 
-Example to export `all` graphs in `dot` format
+Example to export `cpg14` graphs in `dot` format
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out
 ```
 
 To export `pdg` in `neo4jcsv` format
```

