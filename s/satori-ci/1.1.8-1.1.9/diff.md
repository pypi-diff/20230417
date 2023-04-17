# Comparing `tmp/satori-ci-1.1.8.tar.gz` & `tmp/satori-ci-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori-ci-1.1.8.tar", last modified: Fri Mar 31 17:37:01 2023, max compression
+gzip compressed data, was "satori-ci-1.1.9.tar", last modified: Thu Apr 13 16:55:44 2023, max compression
```

## Comparing `satori-ci-1.1.8.tar` & `satori-ci-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori-ci-1.1.8/LICENSE
--rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori-ci-1.1.8/README.md
--rw-r--r--   0        0        0      594 2023-03-31 17:36:00.119124 satori-ci-1.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori-ci-1.1.8/src/satorici/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori-ci-1.1.8/src/satorici/classes/__init__.py
--rw-r--r--   0        0        0     3079 2023-03-31 17:35:44.199910 satori-ci-1.1.8/src/satorici/classes/api.py
--rw-r--r--   0        0        0     1830 2023-03-28 19:49:33.588923 satori-ci-1.1.8/src/satorici/classes/bundler.py
--rw-r--r--   0        0        0    17071 2023-03-31 17:35:44.200212 satori-ci-1.1.8/src/satorici/classes/satori.py
--rw-r--r--   0        0        0     5865 2023-03-28 19:49:33.589279 satori-ci-1.1.8/src/satorici/classes/utils.py
--rwxr-xr-x   0        0        0     5890 2023-03-31 17:35:44.200461 satori-ci-1.1.8/src/satorici/satori_module.py
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 satori-ci-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori-ci-1.1.9/LICENSE
+-rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori-ci-1.1.9/README.md
+-rw-r--r--   0        0        0      594 2023-04-13 16:53:36.657115 satori-ci-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori-ci-1.1.9/src/satorici/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori-ci-1.1.9/src/satorici/classes/__init__.py
+-rw-r--r--   0        0        0     3307 2023-04-13 16:53:36.657556 satori-ci-1.1.9/src/satorici/classes/api.py
+-rw-r--r--   0        0        0     1830 2023-03-28 19:49:33.588923 satori-ci-1.1.9/src/satorici/classes/bundler.py
+-rw-r--r--   0        0        0    17164 2023-04-13 16:53:36.657899 satori-ci-1.1.9/src/satorici/classes/satori.py
+-rw-r--r--   0        0        0     5865 2023-03-28 19:49:33.589279 satori-ci-1.1.9/src/satorici/classes/utils.py
+-rwxr-xr-x   0        0        0     5890 2023-03-31 17:35:44.200461 satori-ci-1.1.9/src/satorici/satori_module.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 satori-ci-1.1.9/PKG-INFO
```

### Comparing `satori-ci-1.1.8/LICENSE` & `satori-ci-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.8/README.md` & `satori-ci-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.8/pyproject.toml` & `satori-ci-1.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.1.8"
+version = "1.1.9"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori-ci-1.1.8/src/satorici/classes/api.py` & `satori-ci-1.1.9/src/satorici/classes/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,96 @@
 import requests
 
 HOST = "https://api.satori-ci.com"
 
 
 class SatoriAPI:
-    def __init__(self, token: str):
+    def __init__(self, token: str, server: str):
         self.__session__ = requests.Session()
         self.__session__.headers.update(
             Authorization=f"Bearer {token}",
         )
         self.__session__.hooks = {
             "response": lambda r, *args, **kwargs: r.raise_for_status()
         }
+        self.server = server or HOST
 
     def debug_bridge(self, res: requests.Response, args) -> dict:
         if args.debug:
             print("Response headers:", res.headers)
         return res.json()
 
     def get_bundle_presigned_post(self, args):
-        res = self.__session__.get(f"{HOST}/run/bundle", data={"secrets": args.data})
+        res = self.__session__.get(
+            f"{self.server}/run/bundle", data={"secrets": args.data}
+        )
         return self.debug_bridge(res, args)
 
     def get_archive_presigned_post(self, args):
-        res = self.__session__.get(f"{HOST}/run/archive", data={"secrets": args.data})
+        res = self.__session__.get(
+            f"{self.server}/run/archive", data={"secrets": args.data}
+        )
         return self.debug_bridge(res, args)
 
     def repo_get(self, args, parameters):
         if args.action == "get":
             args.action = ""
-        res = self.__session__.get(f"{HOST}/repo/{args.action}", params=parameters)
+        res = self.__session__.get(
+            f"{self.server}/repo/{args.action}", params=parameters
+        )
         return self.debug_bridge(res, args)
 
     def monitor_get(self, action, parameters):
         if action == "get":
             action = ""
-        res = self.__session__.get(f"{HOST}/monitor/{action}", params=parameters)
+        res = self.__session__.get(f"{self.server}/monitor/{action}", params=parameters)
         return res.json()
 
     def monitor_delete(self, parameters):
-        res = self.__session__.delete(f"{HOST}/monitor", params=parameters)
+        res = self.__session__.delete(f"{self.server}/monitor", params=parameters)
         return res.json()
 
     def report_get(self, action, parameters):
         if action == "get":
             action = ""
-        res = self.__session__.get(f"{HOST}/report/{action}", params=parameters)
+        res = self.__session__.get(f"{self.server}/report/{action}", params=parameters)
         return res.json()
 
     def report_delete(self, parameters):
-        res = self.__session__.delete(f"{HOST}/report", params=parameters)
+        res = self.__session__.delete(f"{self.server}/report", params=parameters)
         return res.json()
 
     def dashboard(self):
-        res = self.__session__.get(f"{HOST}/dashboard")
+        res = self.__session__.get(f"{self.server}/dashboard")
         return res.json()
 
     def playbook_get(self, parameters):
-        res = self.__session__.get(f"{HOST}/playbook", params=parameters)
+        res = self.__session__.get(f"{self.server}/playbook", params=parameters)
         return res.json()
 
     def playbook_delete(self, parameters):
-        res = self.__session__.delete(f"{HOST}/playbook", params=parameters)
+        res = self.__session__.delete(f"{self.server}/playbook", params=parameters)
         return res.json()
 
     def team_get(self, parameters):
-        res = self.__session__.get(f"{HOST}/team", params=parameters)
+        res = self.__session__.get(f"{self.server}/team", params=parameters)
         return res.json()
 
     def team_post(self, parameters):
-        res = self.__session__.post(f"{HOST}/team", params=parameters)
+        res = self.__session__.post(f"{self.server}/team", params=parameters)
         return res.json()
 
     def team_members_get(self, parameters):
-        res = self.__session__.get(f"{HOST}/team/members", params=parameters)
+        res = self.__session__.get(f"{self.server}/team/members", params=parameters)
         return res.json()
 
     def team_members_put(self, parameters):
-        res = self.__session__.put(f"{HOST}/team/members", params=parameters)
+        res = self.__session__.put(f"{self.server}/team/members", params=parameters)
         return res.json()
 
     def team_repos_get(self, parameters):
-        res = self.__session__.get(f"{HOST}/team/repos", params=parameters)
+        res = self.__session__.get(f"{self.server}/team/repos", params=parameters)
         return res.json()
 
     def team_repos_put(self, parameters):
-        res = self.__session__.put(f"{HOST}/team/repos", params=parameters)
+        res = self.__session__.put(f"{self.server}/team/repos", params=parameters)
         return res.json()
```

### Comparing `satori-ci-1.1.8/src/satorici/classes/bundler.py` & `satori-ci-1.1.9/src/satorici/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.8/src/satorici/classes/satori.py` & `satori-ci-1.1.9/src/satorici/classes/satori.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.config_paths = [
             f"{Path.home()}/.satori_credentials.yml",
             ".satori_credentials.yml",
         ]
         self.verbose = False
         if not config:
             self.load_config()
-            self.api = SatoriAPI(self.token)
+            self.api = SatoriAPI(self.token, self.server)
 
     def load_config(self):
         """Load the config file and set the token on the headers"""
         config_file = None
         for file in self.config_paths:
             if Path(file).is_file():
                 config_file = Path(file)
@@ -76,14 +76,15 @@
             if not profile.get("token"):
                 puts(FAIL_COLOR, f"No token in profile: {self.profile}\n")
                 print("satori-cli [-p PROFILE] config token TOKEN")
                 sys.exit(1)
 
             self.config = config
             self.token = profile["token"]
+            self.server = profile.get("server")
 
     def save_config(self, key: str, value: str):
         """Save the token into the config file"""
         config_file = None
         for file in self.config_paths:
             if Path(file).is_file():
                 config_file = Path(file)
@@ -100,15 +101,15 @@
             config_file = self.config_paths[0]
 
         config.setdefault(self.profile, {})[key] = value
 
         with open(config_file, "w") as f:
             f.write(yaml.safe_dump(config))
 
-        print("Token saved")
+        puts(Fore.LIGHTGREEN_EX, key.capitalize() + " saved")
 
     def run(self, args):
         exec_data = None
         if os.path.isdir(args.path):
             exec_data = self.run_folder(args)
         elif os.path.isfile(args.path):
             exec_data = self.run_file(args)
@@ -342,15 +343,15 @@
             else:
                 autoformat(res, jsonfmt=args.json)
             if not args.json:
                 print(f"Current page: {args.page}")
         elif args.action == "output":
             self.output(args, params)
         elif args.action == "stop":
-            res = self.api.report_stop(args.action, params)
+            res = self.api.report_get(args.action, params)
             autoformat(res, jsonfmt=args.json)
         elif args.action == "delete":
             res = self.api.report_delete(params)
             autoformat(res, jsonfmt=args.json)
         else:
             print("Unknown subcommand")
             sys.exit(1)
```

### Comparing `satori-ci-1.1.8/src/satorici/classes/utils.py` & `satori-ci-1.1.9/src/satorici/classes/utils.py`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.8/src/satorici/satori_module.py` & `satori-ci-1.1.9/src/satorici/satori_module.py`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.8/PKG-INFO` & `satori-ci-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.1.8
+Version: 1.1.9
 Summary: Satori CI - Automated Software Testing Platform
 Author-email: Satori CI CLI <info@satori-ci.com>
 Requires-Python: >=3.9
 Project-URL: Homepage, https://www.satori-ci.com
 Description-Content-Type: text/markdown
 
 # 1. Five Ws (and one H)
```

