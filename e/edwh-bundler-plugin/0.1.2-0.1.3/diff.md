# Comparing `tmp/edwh_bundler_plugin-0.1.2.tar.gz` & `tmp/edwh_bundler_plugin-0.1.3.tar.gz`

## Comparing `edwh_bundler_plugin-0.1.2.tar` & `edwh_bundler_plugin-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    19160 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    19514 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/PKG-INFO
```

### Comparing `edwh_bundler_plugin-0.1.2/CHANGELOG.md` & `edwh_bundler_plugin-0.1.3/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.3 (2023-04-17)
+### Fix
+* **publish:** .db file moved to tmp ([`11613ca`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/11613caab17da02526358c5291a3f737c6d4b859))
+
 ## v0.1.2 (2023-04-11)
 ### Documentation
 * **changelog:** Manual fix changelog for missing version ([`68a71ed`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/68a71ed76ae53d758f45aca70fa2a61bbbff5a9d))
 ### Refactor
 * Changed dynamic imports to normal dependencies ([`5b0095f`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/5b0095f9121a92e1573415e08461561a8bd0e023))
 
 ## v0.1.1 (2023-04-11)
```

### Comparing `edwh_bundler_plugin-0.1.2/requirements-dev.txt` & `edwh_bundler_plugin-0.1.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,45 +9,47 @@
 import sys
 import typing
 from contextlib import contextmanager
 from datetime import datetime
 
 import invoke
 import yaml
-from invoke import task
+from invoke import task, Context
+from dotenv import load_dotenv
+from shutil import rmtree
 
 from .css import extract_contents_for_css
 from .js import extract_contents_for_js
 from .shared import truthy
-from dotenv import load_dotenv
 
 now = datetime.utcnow
 
 # prgram is created in __init__
 
 # defaults/consts
 DEFAULT_INPUT = "bundle.yaml"
 DEFAULT_INPUT_LTS = "bundle-lts.yaml"
 DEFAULT_OUTPUT_JS = "bundle.js"
 DEFAULT_OUTPUT_CSS = "bundle.css"
 TEMP_OUTPUT_DIR = "/tmp/bundle-build/"
 TEMP_OUTPUT = ".bundle_tmp"
-DEFAULT_ASSETS_DB = "py4web/apps/lts/databases/lts_assets.db"
+DEFAULT_ASSETS_DB = "/tmp/lts_assets.db"
+DEFAULT_ASSETS_SQL = "py4web/apps/lts/databases/lts_assets.sql"
 
 
 def load_config(fname: str = DEFAULT_INPUT, strict=False) -> dict:
     """
     Load yaml config from file name, default to empty or error if strict
     """
     if os.path.exists(fname):
         with open(fname) as f:
             return yaml.load(f, yaml.Loader)
+    elif strict:
+        raise FileNotFoundError(fname)
     else:
-        if strict:
-            raise FileNotFoundError(fname)
         return {}
 
 
 @contextmanager
 def start_buffer(temp: str | typing.IO = TEMP_OUTPUT) -> typing.IO:
     """
     Open a temp buffer file in append mode and first remove old version if that exists
@@ -82,19 +84,15 @@
         value: the value from cli, will override config if anything other than None
         config: the 'config' section of the config yaml
         key: config key to look in (under the 'config' section)
         bool: should the result alwasy be a boolean? Useful cli arguments such as --cache y,
                      but should probably be False for named arguments such as --filename ...
         default: if the option can be found in neither the cli arguments or the config file, what should the value be?
     """
-    return (
-        (truthy(value) if bool else value)
-        if value is not None
-        else config.get(key, default)
-    )
+    return (truthy(value) if bool else value) if value is not None else config.get(key, default)
 
 
 def _fill_variables(setting: str | dict, variables: dict[re.Pattern, str]) -> str:
     """
     Fill in $variables in a dynamic setting.
     E.g. "$in_app/path/to/css" + {'in_app': 'apps/cmsx'} -> 'apps/cmsx/path/to/css'
     """
@@ -196,32 +194,23 @@
     Build the JS bundle (cli only)
     """
     config = load_config(input)
 
     files = files or config.get("js")
 
     if not files:
-        raise ValueError(
-            "Please specify either --files or the js key in a config yaml (e.g. bundle.yaml)"
-        )
+        raise ValueError("Please specify either --files or the js key in a config yaml (e.g. bundle.yaml)")
 
     settings = config.get("config", {})
 
     minify = cli_or_config(minify, settings, "minify")
     cache = cli_or_config(cache, settings, "cache", default=True)
-    output = (
-        sys.stdout
-        if stdout
-        else cli_or_config(output, settings, "output_js", bool=False)
-             or DEFAULT_OUTPUT_JS
-    )
+    output = sys.stdout if stdout else cli_or_config(output, settings, "output_js", bool=False) or DEFAULT_OUTPUT_JS
 
-    settings["version"] = cli_or_config(
-        version, settings, "version", bool=False, default="latest"
-    )
+    settings["version"] = cli_or_config(version, settings, "version", bool=False, default="latest")
 
     return _handle_files(
         files,
         extract_contents_for_js,
         output,
         verbose=verbose,
         cache=cache,
@@ -261,20 +250,20 @@
         output,
         verbose=verbose,
         cache=cache,
         minify=minify,
         settings=settings,
     )
 
-    if isinstance(output, io.StringIO):
-        output.seek(0)
-        return output.read()
-    else:
+    if not isinstance(output, io.StringIO):
         return output
 
+    output.seek(0)
+    return output.read()
+
 
 @task(iterable=["files"])
 def build_css(
     c,
     files=None,
     input=DEFAULT_INPUT,
     verbose=False,
@@ -290,31 +279,20 @@
     """
     config = load_config(input)
     settings = config.get("config", {})
 
     minify = cli_or_config(minify, settings, "minify")
     cache = cli_or_config(cache, settings, "cache", default=True)
 
-    settings["version"] = cli_or_config(
-        version, settings, "version", bool=False, default="latest"
-    )
-
-    output = (
-        sys.stdout
-        if stdout
-        else cli_or_config(output, settings, "output_css", bool=False)
-             or DEFAULT_OUTPUT_CSS
-    )
+    settings["version"] = cli_or_config(version, settings, "version", bool=False, default="latest")
 
-    files = files or config.get("css")
+    output = sys.stdout if stdout else cli_or_config(output, settings, "output_css", bool=False) or DEFAULT_OUTPUT_CSS
 
-    if not files:
-        raise ValueError(
-            "Please specify either --files or the css key in a config yaml (e.g. bundle.yaml)"
-        )
+    if not (files := (files or config.get("css"))):
+        raise ValueError("Please specify either --files or the css key in a config yaml (e.g. bundle.yaml)")
 
     return _handle_files(
         files,
         extract_contents_for_css,
         output,
         verbose=verbose,
         cache=cache,
@@ -354,20 +332,20 @@
         output,
         verbose=verbose,
         cache=cache,
         minify=minify,
         settings=settings,
     )
 
-    if isinstance(output, io.StringIO):
-        output.seek(0)
-        return output.read()
-    else:
+    if not isinstance(output, io.StringIO):
         return output
 
+    output.seek(0)
+    return output.read()
+
 
 @task(iterable=["files"])
 def build(
     c,
     input=DEFAULT_INPUT,
     verbose=False,
     # defaults from config, can be overwritten:
@@ -396,43 +374,50 @@
     for item in extra:
         result ^= bool(item)
 
     return result
 
 
 def dict_factory(cursor, row):
-    # https://stackoverflow.com/questions/3300464/how-can-i-get-dict-from-sqlite-query
+    return {col[0]: row[idx] for idx, col in enumerate(cursor.description)}
 
-    d = {}
-    for idx, col in enumerate(cursor.description):
-        d[col[0]] = row[idx]
-    return d
 
+def assert_chmod_777(c: Context, filepath: str | list[str]):
+    if isinstance(filepath, str):
+        filepaths = [filepath]
+    else:
+        filepaths = filepath
 
-def assert_chmod_777(c: invoke.context.Context, filepath: str):
-    resp = c.run(f'stat --format "%a  %n" {filepath}', hide=True)
-    chmod = resp.stdout.split(" ")[0]
-    if chmod != 777:
-        c.sudo(f"chmod 777 {filepath}")
+    for filepath in filepaths:
+        resp = c.run(f'stat --format "%a  %n" {filepath}', hide=True)
+        chmod = resp.stdout.split(" ")[0]
+        if chmod != 777:
+            c.sudo(f"chmod 777 {filepath}")
+
+
+def assert_file_exists(c: Context, db_filepath: str, sql_filepath: str):
+    if not os.path.exists(db_filepath):
+        # load existing
+        c.run(f"sqlite3 {db_filepath} < {sql_filepath}")
 
 
 def config_setting(key, default=None, config=None, config_path=None):
     if not config:
         config = load_config(config_path or DEFAULT_INPUT_LTS)
     re_settings = _regexify_settings(config)
     var = config.get(key, default)
     return _fill_variables(var, re_settings)
 
 
-def setup_db(
-    c: invoke.context.Context, config_path=DEFAULT_INPUT_LTS
-) -> sqlite3.Connection:
+def setup_db(c: invoke.context.Context, config_path=DEFAULT_INPUT_LTS) -> sqlite3.Connection:
     db_path = config_setting("output_db", DEFAULT_ASSETS_DB, config_path=config_path)
+    sql_path = config_setting("output_sql", DEFAULT_ASSETS_SQL, config_path=config_path)
 
-    assert_chmod_777(c, db_path)
+    assert_file_exists(c, db_path, sql_path)
+    assert_chmod_777(c, [db_path, sql_path])
     con = sqlite3.connect(db_path)
     con.row_factory = dict_factory
     return con
 
 
 def get_latest_version(db: sqlite3.Connection, type=None) -> dict:
     query = ["SELECT *", "FROM bundle_version"]
@@ -449,17 +434,18 @@
 def _update_assets_sql(c: invoke.context.Context):
     """
     ... todo docs ...
     Should be done after each db.commit()
     """
     # for line in db.iterdump():
     db_path = config_setting("output_db", DEFAULT_ASSETS_DB)
+    sql_path = config_setting("output_sql", DEFAULT_ASSETS_SQL)
+
     sql: invoke.Result = c.run(f"sqlite3 {db_path} .dump", hide=True)
 
-    sql_path = db_path.replace(".db", ".sql")
     with open(sql_path, "w", encoding="UTF-8") as f:
         f.write(sql.stdout)
 
 
 @task
 def update_assets_sql(c):
     # db = setup_db(c)
@@ -474,27 +460,23 @@
 
     db.execute(query.format(columns, placeholders), values)
     db.commit()
     _update_assets_sql(c)
 
 
 def version_exists(db: sqlite3.Connection, filetype: str, version: str):
-    query = (
-        "SELECT COUNT(*) as c FROM bundle_version WHERE filetype = ? AND version = ?;"
-    )
+    query = "SELECT COUNT(*) as c FROM bundle_version WHERE filetype = ? AND version = ?;"
 
     return db.execute(query, (filetype, version)).fetchone()["c"] > 0
 
 
 def prompt_changelog(db: sqlite3.Connection, filetype: str, version: str):
     load_dotenv()
 
-    query = (
-        "SELECT id, changelog FROM bundle_version WHERE filetype = ? AND version = ?;"
-    )
+    query = "SELECT id, changelog FROM bundle_version WHERE filetype = ? AND version = ?;"
     row = db.execute(query, (filetype, version)).fetchone()
     if row["changelog"]:
         print("Changelog already filled in! ", "It can be updated at:")
     else:
         print(f"Please fill in a changelog for this {filetype} publication at: ")
 
     idx = row["id"]
@@ -510,102 +492,91 @@
     prompt_changelog(db, filetype, version)
 
 
 def confirm(prompt: str, force=False) -> bool:
     return force or truthy(input(prompt))
 
 
-@task()
-def publish(
-    c,
-    version=None,
-    major=False,
-    minor=False,
-    patch=False,
-    filename=None,
-    js=True,
-    css=True,
-    verbose=False,
-    config=DEFAULT_INPUT_LTS,
-    force=False,
-):
-    c: invoke.context.Context
-    db = setup_db(c)
-    previous = get_latest_version(db, "js")
-
-    if not os.path.exists(TEMP_OUTPUT_DIR):
-        os.mkdir(TEMP_OUTPUT_DIR)
-
+def _decide_new_version(major: int, minor: int, patch: int, previous: dict, version: str):
     if not any((version, major, minor, patch)):
         print("Previous version is:", previous.get("version", "0.0.0"))
         version = input("Which version would you like to publish? ")
     elif not XOR(version, major, minor, patch):
         # error on more than one:
-        raise ValueError(
-            "Please specify only one of --version, --major, --minor or --patch"
-        )
+        raise ValueError("Please specify only one of --version, --major, --minor or --patch")
     elif major:
         new_major = previous.get("major", 0) + 1
         version = f"{new_major}.0.0"
     elif minor:
         major = previous.get("major", 0)
         new_minor = previous.get("minor", 0) + 1
         version = f"{major}.{new_minor}.0"
     elif patch:
         major = previous.get("major", 0)
         minor = previous.get("minor", 0)
         new_patch = previous.get("patch", 0) + 1
         version = f"{major}.{minor}.{new_patch}"
-
     version_re = re.compile(r"^(\d{1,3})(\.\d{1,3})?(\.\d{1,3})?$")
     if not (groups := version_re.findall(version)):
-        raise ValueError(
-            f"Invalid version {version}. Please use the format major.major.patch (e.g. 3.5.0)"
-        )
-
+        raise ValueError(f"Invalid version {version}. Please use the format major.major.patch (e.g. 3.5.0)")
     major, minor, patch = (
         int(groups[0][0]),
         int(groups[0][1].strip(".") or 0),
         int(groups[0][2].strip(".") or 0),
     )
-
     version = f"{major}.{minor}.{patch}"
+    return major, minor, patch, version
+
+
+def file_hash(c: Context, filename: str):
+    return c.run(f"sha1sum {filename}", hide=True).stdout.split(" ")[0]
+
+
+@task()
+def publish(
+    c,
+    version=None,
+    major=False,
+    minor=False,
+    patch=False,
+    filename=None,
+    js=True,
+    css=True,
+    verbose=False,
+    config=DEFAULT_INPUT_LTS,
+    force=False,
+):
+    c: invoke.context.Context
+    db = setup_db(c)
+    previous = get_latest_version(db, "js")
+
+    if not os.path.exists(TEMP_OUTPUT_DIR):
+        os.mkdir(TEMP_OUTPUT_DIR)
+
+    major, minor, patch, version = _decide_new_version(major, minor, patch, previous, version)
 
     if js and version_exists(db, "js", version):
         print(f"JS Version {version} already exists!")
         js = confirm("Are you sure you want to overwrite it? ", force)
 
     if css and version_exists(db, "css", version):
         print(f"CSS Version {version} already exists!")
         css = confirm("Are you sure you want to overwrite it? ", force)
 
+    output_js = output_css = None
     if js and css:
         output_js, output_css = build(c, input=config, version=version, verbose=verbose)
     elif js:
         output_js = build_js(c, input=config, version=version, verbose=verbose)
-        output_css = None
     elif css:
         output_css = build_css(c, input=config, version=version, verbose=verbose)
-        output_js = None
-    else:
-        # no build
-        output_css = output_js = None
+    # else: no build
 
     if output_js:
-        with open(output_js, "r", encoding="UTF-8") as f:
-            file_contents = f.read()
-
-        filename = output_js.split("/")[-1]
-        hash = c.run(f"sha1sum {output_js}", hide=True).stdout.split(" ")[0]
-
-        if hash == previous.get("hash"):
-            print("JS hash matches previous version.")
-            go = confirm("Are you sure you want to release a new version? ", force)
-        else:
-            go = True
+        go, hash, filename, file_contents = _should_publish(c, force, output_js, previous.get("hash"), "JS")
 
         if go:
             insert_version(
                 c,
                 db,
                 {
                     "filetype": "js",
@@ -620,27 +591,16 @@
                     "contents": file_contents,
                 },
             )
             print(f"JS version {version} published.")
             prompt_changelog(db, "js", version)
 
     if output_css:
-        with open(output_css, "r", encoding="UTF-8") as f:
-            file_contents = f.read()
-
         previous_css = get_latest_version(db, "css")
-
-        filename = output_css.split("/")[-1]
-        hash = c.run(f"sha1sum {output_css}", hide=True).stdout.split(" ")[0]
-
-        if hash == previous_css.get("hash"):
-            print("CSS hash matches previous version.")
-            go = confirm("Are you sure you want to release a new version? ", force)
-        else:
-            go = True
+        go, hash, filename, file_contents = _should_publish(c, force, output_css, previous_css.get("hash"), "CSS")
 
         if go:
             insert_version(
                 c,
                 db,
                 {
                     "filetype": "css",
@@ -654,22 +614,40 @@
                     "changelog": "",
                     "contents": file_contents,
                 },
             )
             print(f"CSS version {version} published.")
             prompt_changelog(db, "css", version)
 
-    from shutil import rmtree
-
     rmtree(TEMP_OUTPUT_DIR)
 
     # after publish: run `up -s py4web` so the bjoerns are all updated
     c.run("inv up -s py4web")
 
 
+def _should_publish(c: Context, force: bool, output_path: str, previous_hash: str, type: typing.Literal["JS", "CSS"]):
+    hash = file_hash(c, output_path)
+    if hash == previous_hash:
+        print(f"{type} hash matches previous version.")
+        go = confirm("Are you sure you want to release a new version? ", force)
+    else:
+        go = True
+    if not go:
+        return False, None, None, None
+
+    # if go:
+
+    with open(output_path, "r", encoding="UTF-8") as f:
+        file_contents = f.read()
+
+    filename = output_path.split("/")[-1]
+
+    return True, hash, filename, file_contents
+
+
 @task
 def list(c):
     db = setup_db(c)
     for row in db.execute(
         "SELECT filetype, version FROM bundle_version ORDER BY major DESC, minor DESC, patch DESC"
     ).fetchall():
         print(row)
@@ -684,14 +662,15 @@
 
     db.execute("DELETE FROM bundle_version;")
     db.commit()
     _update_assets_sql(c)
 
     assert db.execute("SELECT COUNT(*) as c FROM bundle_version;").fetchone()["c"] == 0
 
+
 # DEV:
 
 #
 # @task
 # def update_dependencies(c):
 #     # invoke update-dependencies
 #     c.run("pip-compile requirements.in")
```

### Comparing `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/css.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -100,8 +100,8 @@
     # more options?
 
     if scss:
         contents = convert_scss(contents, minify)
     elif minify:
         contents = _del_whitespace(contents)
 
-    return contents
+    return contents
```

### Comparing `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/js.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,20 +76,15 @@
     raise NotImplementedError("dict for JS entries is not supported yet")
 
 
 def _include_hyperscript(contents: str) -> str:
     """
     Execute the _hs file with the '_hyperscript' function, escaping some characters
     """
-    contents = (
-        contents.replace("\\", "\\\\")
-        .replace("`", "\\`")
-        .replace("$", "\\$")
-        .replace("{", "\\{")
-    )
+    contents = contents.replace("\\", "\\\\").replace("`", "\\`").replace("$", "\\$").replace("{", "\\{")
 
     return f"_hyperscript(`{contents}`)"
 
 
 def _append_to_dom(html: str) -> str:
     """
     Append some html fragment at the end of the page
@@ -98,20 +93,15 @@
     return f"""document.body.innerHTML += `{html}`"""
 
 
 def _append_to_head(css: str) -> str:
     """
     Append some CSS fragment at the end of the head of the page
     """
-    css = (
-        css.replace("\\", "\\\\")
-        .replace("`", "\\`")
-        .replace("$", "\\$")
-        .replace("{", "\\{")
-    )
+    css = css.replace("\\", "\\\\").replace("`", "\\`").replace("$", "\\$").replace("{", "\\{")
     return f"document.head.innerHTML += `<style>{css}</style>`"
 
 
 def hsmin(contents: str) -> str:
     """
     Minify hyperscript code by removing comments and minimizing whitespace
     """
```

### Comparing `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/shared.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
 
 
 @truthy.register
 def _(val: int):
     """
     Negative numbers are often not truthy
     """
-    return val > 0
+    return val > 0
```

### Comparing `edwh_bundler_plugin-0.1.2/LICENSE.txt` & `edwh_bundler_plugin-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.2/README.md` & `edwh_bundler_plugin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.2/pyproject.toml` & `edwh_bundler_plugin-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.2/PKG-INFO` & `edwh_bundler_plugin-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-bundler-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

