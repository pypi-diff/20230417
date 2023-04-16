# Comparing `tmp/biobricks-0.1.59.tar.gz` & `tmp/biobricks-0.1.60.tar.gz`

## Comparing `biobricks-0.1.59.tar` & `biobricks-0.1.60.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks.svg
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.59/coverage.xml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.59/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.59/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/README.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.59/.vscode/tasks.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/api.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/brick.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/checks.py
--rwxr-xr-x   0        0        0     3986 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/cli.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/config.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/local_bb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/test_init.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.59/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.59/docker/test.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.59/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.59/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 biobricks-0.1.59/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.59/pyproject.toml
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 biobricks-0.1.59/PKG-INFO
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks.svg
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.60/coverage.xml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.60/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.60/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/README.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.60/.vscode/tasks.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/api.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/brick.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/checks.py
+-rwxr-xr-x   0        0        0     4514 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/cli.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/config.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/local_bb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/test_init.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.60/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.60/docker/test.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.60/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.60/LICENSE
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.60/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.60/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.60/PKG-INFO
```

### Comparing `biobricks-0.1.59/biobricks.svg` & `biobricks-0.1.60/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/coverage.xml` & `biobricks-0.1.60/coverage.xml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/.github/workflows/biobricks.yml` & `biobricks-0.1.60/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/biobricks/api.py` & `biobricks-0.1.60/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/biobricks/brick.py` & `biobricks-0.1.60/biobricks/brick.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/biobricks/checks.py` & `biobricks-0.1.60/biobricks/checks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 import urllib.request as request
 import json, urllib
 import os, tempfile, uuid, requests, pkg_resources
 from pathlib import Path
     
-def check_version():
-    current_version = pkg_resources.get_distribution('biobricks').version
-    pypi_url = 'https://pypi.org/pypi/biobricks/json'
-    response = requests.get(pypi_url)
-    latest_version = response.json()['info']['version']
-    if current_version != latest_version:
-        print(f"""A new version ({latest_version}) of biobricks is available. 
-              Please upgrade using 'pip install --upgrade biobricks'""")
-
 def check_url_available(url):
     try:
         code = request.urlopen(url).getcode()
         if code!=200:
             raise Exception(f"{url} not available")
     except Exception as e:
         raise Exception(f"{url} not available") from e
```

### Comparing `biobricks-0.1.59/biobricks/cli.py` & `biobricks-0.1.60/biobricks/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys, os
 import biobricks as bb
-import click, cloup
+import click, cloup, pkg_resources, requests
 from logger import logger
 from pathlib import Path
 from .config import read_config, write_config, init_bblib
-from .checks import check_token, check_version
+from .checks import check_token
 from .brick import Brick
 from .local_bb import LocalBB
 
 @cloup.group('biobricks')
 def cli():
     pass
 
@@ -102,15 +102,21 @@
 @cli.command(help="Show the status of the local brick",
     section=Sect.BRICK)
 def status():
     print("BBLIB: " + str(bb.bblib()))
     # print the dependencies file
     with open(local_bblib() / "dependencies.txt", "r") as f:
         print(f.read())
-
-if __name__ == "__main__":
-    try:
-        check_version()
-    except:
-        pass
+        
+@cli.command(help="Get version and check for updates", section=Sect.GLOBAL)
+def version():
+    current_version = pkg_resources.get_distribution('biobricks').version
+    response = requests.get('https://pypi.org/pypi/biobricks/json')
+    latest_version = response.json()['info']['version']
+    if current_version != latest_version:
+        print(f"\nA new version ({latest_version}) of biobricks is available. " 
+              f"\nPlease upgrade using 'pip install --upgrade biobricks'\n")
+    else:
+        print(f"biobricks version {current_version} is up to date.")
     
+if __name__ == "__main__":
     cli()
```

### Comparing `biobricks-0.1.59/biobricks/config.py` & `biobricks-0.1.60/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/biobricks/local_bb.py` & `biobricks-0.1.60/biobricks/local_bb.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/biobricks/tests/test_init.py` & `biobricks-0.1.60/biobricks/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/docker/Dockerfile` & `biobricks-0.1.60/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/LICENSE` & `biobricks-0.1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.59/README.md` & `biobricks-0.1.60/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 # initialize
 To get started configure biobricks with a path for bricks and a biobricks.ai token:
 ```
 biobricks configure
 > Choose path to store bricks: <input a local path>
-> Input a token from biobrick.ai/token: <this is your access token>
+> Input a token from biobricks.ai/token: <this is your access token>
 ```
 
 # Pull Bricks
 To download a brick and save it locally in your library use `bb.pull`. An example using the Tox21 dataset:  
 
 ```python
 import biobricks as bb
```

### Comparing `biobricks-0.1.59/pyproject.toml` & `biobricks-0.1.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.1.59"
+version = "0.1.60"
 authors = [
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" },
   { name="Thomas Luechtefeld", email="tom@insilica.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `biobricks-0.1.59/PKG-INFO` & `biobricks-0.1.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobricks
-Version: 0.1.59
+Version: 0.1.60
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Homepage, https://github.com/biobricks-ai/biobricks
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: "Jose A. Jaramillo" <jjv@utp.edu.co>, Thomas Luechtefeld <tom@insilica.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 ```
 
 # initialize
 To get started configure biobricks with a path for bricks and a biobricks.ai token:
 ```
 biobricks configure
 > Choose path to store bricks: <input a local path>
-> Input a token from biobrick.ai/token: <this is your access token>
+> Input a token from biobricks.ai/token: <this is your access token>
 ```
 
 # Pull Bricks
 To download a brick and save it locally in your library use `bb.pull`. An example using the Tox21 dataset:  
 
 ```python
 import biobricks as bb
```

