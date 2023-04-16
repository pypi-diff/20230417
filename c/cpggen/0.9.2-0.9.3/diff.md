# Comparing `tmp/cpggen-0.9.2.tar.gz` & `tmp/cpggen-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.9.2.tar", max compression
+gzip compressed data, was "cpggen-0.9.3.tar", max compression
```

## Comparing `cpggen-0.9.2.tar` & `cpggen-0.9.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-15 00:43:28.683513 cpggen-0.9.2/LICENSE
--rw-r--r--   0        0        0     6774 2023-04-15 00:43:28.683513 cpggen-0.9.2/README.md
--rw-r--r--   0        0        0        0 2023-04-15 00:43:28.683513 cpggen-0.9.2/cpggen/__init__.py
--rw-r--r--   0        0        0    12893 2023-04-15 00:43:28.683513 cpggen-0.9.2/cpggen/cli.py
--rw-r--r--   0        0        0    28621 2023-04-15 00:43:28.683513 cpggen-0.9.2/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-15 00:43:28.687514 cpggen-0.9.2/cpggen/logger.py
--rw-r--r--   0        0        0    10937 2023-04-15 00:43:28.687514 cpggen-0.9.2/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-15 00:43:28.687514 cpggen-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8102 1970-01-01 00:00:00.000000 cpggen-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 23:15:12.958443 cpggen-0.9.3/LICENSE
+-rw-r--r--   0        0        0     6774 2023-04-16 23:15:12.958443 cpggen-0.9.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/__init__.py
+-rw-r--r--   0        0        0    12897 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/cli.py
+-rw-r--r--   0        0        0    29008 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/logger.py
+-rw-r--r--   0        0        0    11089 2023-04-16 23:15:12.958443 cpggen-0.9.3/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-16 23:15:12.958443 cpggen-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     8102 1970-01-01 00:00:00.000000 cpggen-0.9.3/PKG-INFO
```

### Comparing `cpggen-0.9.2/LICENSE` & `cpggen-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.2/README.md` & `cpggen-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.2/cpggen/cli.py` & `cpggen-0.9.3/cpggen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,17 +137,17 @@
     )
 
 
 @app.route("/cpg", methods=["GET", "POST"])
 async def generate_cpg():
     q = request.args
     params = await request.get_json()
-    url = None
-    src = None
-    languages = None
+    url = ""
+    src = ""
+    languages = "autodetect"
     cpg_out_dir = None
     is_temp_dir = False
     if not params:
         params = {}
     if q.get("url"):
         url = q.get("url")
     if q.get("src"):
```

### Comparing `cpggen-0.9.2/cpggen/executor.py` & `cpggen-0.9.3/cpggen/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         with zipfile.ZipFile(joern_bundled, "r") as zip_ref:
             zip_ref.extractall(local_bin_dir)
             try:
                 # Add execute permissions
                 for dirname, subdirs, files in os.walk(local_bin_dir):
                     for filename in files:
                         if not filename.endswith(".jar") and (
-                            filename.endswith(".sh") or "2cpg" in filename
+                            filename.endswith(".sh")
+                            or "2cpg" in filename
+                            or "joern-" in filename
                         ):
                             os.chmod(os.path.join(dirname, filename), 0o755)
                 LOG.debug(f"Extracted {joern_bundled}")
                 os.environ["JOERN_HOME"] = os.path.join(local_bin_dir, "joern-cli")
                 os.environ["CPGGEN_BIN_DIR"] = local_bin_dir
                 os.environ["PATH"] += os.sep + os.environ["JOERN_HOME"] + os.sep
             except Exception:
@@ -109,24 +111,24 @@
     "js": "%(joern_home)sjssrc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "python": "%(joern_home)spysrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-tests -l error",
+    "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --collect-js-files %(src)s --ignore-errors --no-log-file --ignore-tests -l error",
     "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --collect-js-files %(src)s --ignore-errors --no-log-file --ignore-tests -l error",
     "go": "%(joern_home)sgo2cpg generate -o %(cpg_out)s ./...",
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
-    "export": "joern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
+    "export": "%(joern_home)sjoern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
     "qwiet": "sl analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "java": {
         "maven": [
@@ -344,16 +346,19 @@
         transient=True,
         redirect_stderr=False,
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
         task = None
         lang_build_crashes = {}
-        if cwd and os.path.isfile(cwd):
-            cwd = os.path.dirname(cwd)
+        if cwd:
+            if os.path.isfile(cwd):
+                cwd = os.path.dirname(cwd)
+            else:
+                cwd = os.path.abspath(cwd)
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
         try:
             stderr = subprocess.DEVNULL
             if LOG.isEnabledFor(DEBUG):
                 stdout = subprocess.PIPE
                 stderr = stdout
@@ -411,32 +416,34 @@
                     cpg_out = cpg_out_dir
                 else:
                     cpg_out = (
                         cpg_out_dir
                         if cpg_out_dir.endswith(".bin.zip")
                         or cpg_out_dir.endswith(".bin")
                         or cpg_out_dir.endswith(".cpg")
-                        else os.path.join(
-                            cpg_out_dir,
-                            f"{os.path.basename(amodule)}-{tool_lang}-cpg.bin.zip",
+                        else os.path.abspath(
+                            os.path.join(
+                                cpg_out_dir,
+                                f"{os.path.basename(amodule)}-{tool_lang}-cpg.bin.zip",
+                            )
                         )
                     )
                     sbom_out = (
                         cpg_out.replace(".bin.zip", ".bom.xml")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.bom.xml"
                     )
                     manifest_out = (
                         cpg_out.replace(".bin.zip", ".manifest.json")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.manifest.json"
                     )
                     LOG.debug(f"CPG file for {tool_lang} is {cpg_out}")
                 cmd_with_args = cmd_with_args % dict(
-                    src=amodule,
+                    src=os.path.abspath(amodule),
                     cpg_out=cpg_out,
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
@@ -448,15 +455,15 @@
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
                 ):
                     sbom_lang = "java"
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
-                    src=src,
+                    src=os.path.abspath(src),
                     tool_lang=sbom_lang,
                     cwd=cwd,
                     sbom_out=sbom_out,
                     cdxgen_cmd=cdxgen_cmd,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     **extra_args,
                 )
@@ -509,16 +516,17 @@
                                 LOG.info(
                                     f"CPG {src} successfully exported to {cpg_out_dir}"
                                 )
                             else:
                                 LOG.warn(
                                     f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually using the command {' '.join(cmd_list_with_args)}"
                                 )
-                    except Exception:
+                    except Exception as e:
                         LOG.warn(f"Unable to export {src} to {cpg_out_dir}")
+                        LOG.error(e)
                     progress.update(task, completed=100, total=100)
                     continue
                 LOG.info(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
                         tool_lang,
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
```

### Comparing `cpggen-0.9.2/cpggen/logger.py` & `cpggen-0.9.3/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.2/cpggen/utils.py` & `cpggen-0.9.3/cpggen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,17 @@
     for root, dirs, files in os.walk(src):
         filter_ignored_dirs(dirs)
         if not is_ignored_dir(src, root):
             for file in files:
                 if is_ignored_file(file):
                     continue
                 if file == src_ext_name or file.endswith(src_ext_name):
-                    result.append(os.path.join(root, file))
+                    result.append(os.path.abspath(os.path.join(root, file)))
                 elif use_start and file.startswith(src_ext_name):
-                    result.append(os.path.join(root, file))
+                    result.append(os.path.abspath(os.path.join(root, file)))
                 if quick and result:
                     return result
     return result
 
 
 def find_java_artifacts(search_dir):
     """
@@ -185,28 +185,30 @@
                 if not is_ignored_dir(search_dir, dirname):
                     for filename in files:
                         if (
                             filename.endswith(".jar")
                             or filename.endswith(".war")
                             or filename.endswith(".ear")
                         ):
-                            jlist.append(os.path.join(dirname, filename))
+                            jlist.append(
+                                os.path.abspath(os.path.join(dirname, filename))
+                            )
                             zf.write(os.path.join(dirname, filename))
-    return jlist if len(jlist) == 1 else [zfile.name]
+    return jlist if len(jlist) == 1 else [os.path.abspath(zfile.name)]
 
 
 def find_csharp_artifacts(search_dir):
     """
     Method to find .Net solution and csproj files in the given directory
     :param src: Directory to search
     :return: List of war or ear or jar files
     """
-    result = [p.as_posix() for p in Path(search_dir).rglob("*.sln")]
+    result = [p.as_posix() for p in Path(search_dir).absolute().rglob("*.sln")]
     if not result:
-        result = [p.as_posix() for p in Path(search_dir).rglob("*.csproj")]
+        result = [p.as_posix() for p in Path(search_dir).absolute().rglob("*.csproj")]
     return result
 
 
 def find_go_mods(search_dir):
     return find_files(search_dir, "go.mod", False, False)
```

### Comparing `cpggen-0.9.2/pyproject.toml` & `cpggen-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.9.2"
+version = "0.9.3"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.9.2/PKG-INFO` & `cpggen-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
```

