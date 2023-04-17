# Comparing `tmp/viur_cli-1.0.0rc2.tar.gz` & `tmp/viur_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-1.0.0rc2.tar", last modified: Fri Mar 31 12:15:35 2023, max compression
+gzip compressed data, was "viur_cli-1.0.2.tar", last modified: Mon Apr 17 17:15:37 2023, max compression
```

## Comparing `viur_cli-1.0.0rc2.tar` & `viur_cli-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.440485 viur_cli-1.0.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.440485 viur_cli-1.0.0rc2/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/npm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 17:15:29.000000 viur_cli-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-17 17:15:37.901606 viur_cli-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-17 17:15:29.000000 viur_cli-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 17:15:29.000000 viur_cli-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 17:15:37.901606 viur_cli-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-17 17:15:29.000000 viur_cli-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.897606 viur_cli-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/npm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-1.0.0rc2/LICENSE` & `viur_cli-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/setup.cfg` & `viur_cli-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/cli.py` & `viur_cli-1.0.2/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/conf.py` & `viur_cli-1.0.2/src/viur_cli/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,13 +283,22 @@
         del projectConfig["default"]["flare"]
 
     if projectConfig["default"]["format"] == "1.0.1":
         projectConfig["default"]["format"] = "1.1.0"
         echo_info("viur-cli tries to find npm applications")
         add_npm_apps()
 
+    ##################### Version 1.1.1
+
+    if projectConfig["default"]["format"] == "1.1.0":
+        projectConfig["default"]["format"] = "1.1.1"
+        builds = projectConfig["default"]["builds"].copy()
+        for k, v in builds.items():
+            if builds[k]["kind"] == "script":
+                builds[k]["kind"] = "exec"
+        projectConfig["default"]["builds"] = builds
     # conf updates must increase format version
     write_config(projectConfig, path)
```

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/deploy.py` & `viur_cli-1.0.2/src/viur_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/flare.py` & `viur_cli-1.0.2/src/viur_cli/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/install.py` & `viur_cli-1.0.2/src/viur_cli/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,40 +6,42 @@
 @cli.group()
 def install():
     """Install VIUR features"""
 
 @install.command()
 @click.argument("version", default="latest")
 @click.option('--next', '-n', 'next_',  is_flag=True, default=False)
-def vi(version, next_):
+@click.option('--target', '-t',  default="vi")
+def vi(version, target, next_):
     """Install VI administration interface."""
 
     if next_:
         downloadnextvi()
         return 0
 
     """download latest vi or a specific version"""
     projectConfig = get_config()
     distFolder = projectConfig["default"]["distribution_folder"]
 
     viRepo = "https://github.com/viur-framework/viur-vi"
-    viPath = os.path.join(distFolder, "vi")
+    viPath = os.path.join(distFolder, target)
+
     tempZipFile = "./vi.zip"
 
     if version == "latest":
         vibaseUrl = f"{viRepo}/releases/latest/download/viur-vi.zip"
     else:
         vibaseUrl = f"{viRepo}/releases/download/v{version}/viur-vi.zip"
 
     def get_version_info(version):
         url = "https://api.github.com/repos/viur-framework/viur-vi/releases"
         if version == "latest":
             try:
                 resp = json.loads(urllib.request.urlopen(url).read().decode("utf-8"))
-                projectConfig["default"]["vi"] = resp[0]["name"]
+                projectConfig["default"]["vi"] = resp[0]["name"][1:]
                 write_config(projectConfig)
             except:
                 echo_error("Error while fetching version info")
         else:
             projectConfig["default"]["vi"] = f'{version}'
             write_config(projectConfig)
```

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/local.py` & `viur_cli-1.0.2/src/viur_cli/local.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/npm.py` & `viur_cli-1.0.2/src/viur_cli/npm.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/cli.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,21 +94,21 @@
         skey = session.get(base_url + "/json/skey")
         username: str = config.get("username", "")
         if not username:
             username = click.prompt("Enter the username")
 
         password: str = click.prompt("Enter the password", hide_input=True)
 
-        response = session.post(base_url + "/vi/user/auth_userpassword/login", data={
+        response = session.post(base_url + "/json/user/auth_userpassword/login", data={
             "skey": skey.json(),
             "name": username,
             "password": password
         })
 
-        if response.text != "FAILURE":
+        if response.json() != "FAILURE":
             config["cookies"] = session.cookies.get_dict()
             click.echo("Setup done")
         else:
             if "cookies" in config:
                 del config["cookies"]
             click.echo("Failed to login. Did you maybe entered the wrong password?")
     except KeyboardInterrupt:
@@ -161,15 +161,15 @@
                     if force:
                         os.remove(_path)
                         create_file()
                     else:
                         with open(_path, "r") as f:
                             if hashlib.sha256(entry["script"].encode()).digest() \
                                     != hashlib.sha256(f.read().encode()).digest():
-                                if click.confirm(f"There is a difference with {entry['path']}. Override?"):
+                                if click.confirm(f"There is a difference with {entry['path']}. Overwrite?"):
                                     os.remove(_path)
                                     create_file()
 
                 else:
                     create_file()
 
         await tree.for_each(for_each)
@@ -222,15 +222,15 @@
                     with open(_real_file, "r") as f:
                         file_content = f.read()
 
                         if hashlib.sha256(entry["script"].encode("utf-8")).digest() \
                                 != hashlib.sha256(file_content.encode("utf-8")).digest():
                             _state = force
                             if not _state:
-                                _state = click.confirm(f"Content of {file} changed. Override?")
+                                _state = click.confirm(f"Content of {file} changed. Overwrite?")
 
                             if _state:
                                 click.echo(f"Push {_real_file}")
                                 await tree.edit(_type, entry["key"], {
                                     "script": file_content
                                 })
```

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scripts/flare.py` & `viur_cli-1.0.2/src/viur_cli/scripts/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-1.0.2/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-1.0.2/src/viur_cli/scripts/viur_2to3.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/setup.py` & `viur_cli-1.0.2/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/tool.py` & `viur_cli-1.0.2/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli/utils.py` & `viur_cli-1.0.2/src/viur_cli/utils.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc2/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-1.0.2/src/viur_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

