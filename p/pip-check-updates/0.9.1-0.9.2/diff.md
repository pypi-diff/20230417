# Comparing `tmp/pip-check-updates-0.9.1.tar.gz` & `tmp/pip-check-updates-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-check-updates-0.9.1.tar", last modified: Tue Feb 22 05:29:49 2022, max compression
+gzip compressed data, was "pip-check-updates-0.9.2.tar", last modified: Sat Mar 26 06:07:41 2022, max compression
```

## Comparing `pip-check-updates-0.9.1.tar` & `pip-check-updates-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.951958 pip-check-updates-0.9.1/
--rw-r--r--   0 zehengl    (501) staff       (20)     1001 2022-02-22 05:18:26.000000 pip-check-updates-0.9.1/.all-contributorsrc
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.948029 pip-check-updates-0.9.1/.github/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.949631 pip-check-updates-0.9.1/.github/workflows/
--rw-r--r--   0 zehengl    (501) staff       (20)      523 2021-11-19 16:53:49.000000 pip-check-updates-0.9.1/.github/workflows/pytest.yml
--rw-r--r--   0 zehengl    (501) staff       (20)       64 2021-11-12 02:39:27.000000 pip-check-updates-0.9.1/.gitignore
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.950057 pip-check-updates-0.9.1/.vscode/
--rw-r--r--   0 zehengl    (501) staff       (20)      437 2021-12-14 09:59:51.000000 pip-check-updates-0.9.1/.vscode/extensions.json
--rw-r--r--   0 zehengl    (501) staff       (20)      667 2021-12-14 10:00:21.000000 pip-check-updates-0.9.1/.vscode/settings.json
--rw-r--r--   0 zehengl    (501) staff       (20)     1066 2021-10-05 06:32:07.000000 pip-check-updates-0.9.1/LICENSE
--rw-r--r--   0 zehengl    (501) staff       (20)       25 2021-11-12 02:39:27.000000 pip-check-updates-0.9.1/MANIFEST.in
--rw-r--r--   0 zehengl    (501) staff       (20)     7425 2022-02-22 05:29:49.952058 pip-check-updates-0.9.1/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)     6570 2022-02-22 05:18:26.000000 pip-check-updates-0.9.1/README.md
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.950399 pip-check-updates-0.9.1/pip_check_updates/
--rw-r--r--   0 zehengl    (501) staff       (20)     2302 2022-02-22 04:05:37.000000 pip-check-updates-0.9.1/pip_check_updates/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)     7218 2022-02-22 05:28:44.000000 pip-check-updates-0.9.1/pip_check_updates/__main__.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.951155 pip-check-updates-0.9.1/pip_check_updates.egg-info/
--rw-r--r--   0 zehengl    (501) staff       (20)     7425 2022-02-22 05:29:49.000000 pip-check-updates-0.9.1/pip_check_updates.egg-info/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)      601 2022-02-22 05:29:49.000000 pip-check-updates-0.9.1/pip_check_updates.egg-info/SOURCES.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        1 2022-02-22 05:29:49.000000 pip-check-updates-0.9.1/pip_check_updates.egg-info/dependency_links.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       56 2022-02-22 05:29:49.000000 pip-check-updates-0.9.1/pip_check_updates.egg-info/entry_points.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       32 2022-02-22 05:29:49.000000 pip-check-updates-0.9.1/pip_check_updates.egg-info/requires.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       24 2022-02-22 05:29:49.000000 pip-check-updates-0.9.1/pip_check_updates.egg-info/top_level.txt
--rw-r--r--   0 zehengl    (501) staff       (20)      121 2022-02-22 05:03:53.000000 pip-check-updates-0.9.1/requirements-dev.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       32 2022-01-24 00:57:21.000000 pip-check-updates-0.9.1/requirements.txt
--rw-r--r--   0 zehengl    (501) staff       (20)      208 2022-02-22 05:29:49.952373 pip-check-updates-0.9.1/setup.cfg
--rw-r--r--   0 zehengl    (501) staff       (20)     1545 2021-12-14 10:00:13.000000 pip-check-updates-0.9.1/setup.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-02-22 05:29:49.951705 pip-check-updates-0.9.1/tests/
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2021-10-05 06:32:07.000000 pip-check-updates-0.9.1/tests/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2021-10-05 06:32:07.000000 pip-check-updates-0.9.1/tests/conftest.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1261 2021-10-05 06:32:07.000000 pip-check-updates-0.9.1/tests/test_compare_versions.py
--rw-r--r--   0 zehengl    (501) staff       (20)      513 2021-10-05 06:32:07.000000 pip-check-updates-0.9.1/tests/test_get_current_version.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.112159 pip-check-updates-0.9.2/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1001 2022-02-22 05:18:26.000000 pip-check-updates-0.9.2/.all-contributorsrc
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.106633 pip-check-updates-0.9.2/.github/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.108697 pip-check-updates-0.9.2/.github/workflows/
+-rw-r--r--   0 zehengl    (501) staff       (20)      516 2022-03-14 22:12:27.000000 pip-check-updates-0.9.2/.github/workflows/pytest.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)       64 2021-11-12 02:39:27.000000 pip-check-updates-0.9.2/.gitignore
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.109207 pip-check-updates-0.9.2/.vscode/
+-rw-r--r--   0 zehengl    (501) staff       (20)      437 2021-12-14 09:59:51.000000 pip-check-updates-0.9.2/.vscode/extensions.json
+-rw-r--r--   0 zehengl    (501) staff       (20)      667 2021-12-14 10:00:21.000000 pip-check-updates-0.9.2/.vscode/settings.json
+-rw-r--r--   0 zehengl    (501) staff       (20)     1066 2021-10-05 06:32:07.000000 pip-check-updates-0.9.2/LICENSE
+-rw-r--r--   0 zehengl    (501) staff       (20)       25 2021-11-12 02:39:27.000000 pip-check-updates-0.9.2/MANIFEST.in
+-rw-r--r--   0 zehengl    (501) staff       (20)     7458 2022-03-26 06:07:41.112273 pip-check-updates-0.9.2/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     6653 2022-03-26 06:00:30.000000 pip-check-updates-0.9.2/README.md
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.109794 pip-check-updates-0.9.2/pip_check_updates/
+-rw-r--r--   0 zehengl    (501) staff       (20)     2297 2022-03-26 05:52:59.000000 pip-check-updates-0.9.2/pip_check_updates/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     7431 2022-03-26 05:58:59.000000 pip-check-updates-0.9.2/pip_check_updates/__main__.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.110648 pip-check-updates-0.9.2/pip_check_updates.egg-info/
+-rw-r--r--   0 zehengl    (501) staff       (20)     7458 2022-03-26 06:07:40.000000 pip-check-updates-0.9.2/pip_check_updates.egg-info/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)      601 2022-03-26 06:07:41.000000 pip-check-updates-0.9.2/pip_check_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        1 2022-03-26 06:07:40.000000 pip-check-updates-0.9.2/pip_check_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       55 2022-03-26 06:07:40.000000 pip-check-updates-0.9.2/pip_check_updates.egg-info/entry_points.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       32 2022-03-26 06:07:40.000000 pip-check-updates-0.9.2/pip_check_updates.egg-info/requires.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       24 2022-03-26 06:07:40.000000 pip-check-updates-0.9.2/pip_check_updates.egg-info/top_level.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)      121 2022-03-26 05:59:28.000000 pip-check-updates-0.9.2/requirements-dev.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       32 2022-03-26 05:59:26.000000 pip-check-updates-0.9.2/requirements.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)      202 2022-03-26 06:07:41.112658 pip-check-updates-0.9.2/setup.cfg
+-rw-r--r--   0 zehengl    (501) staff       (20)     1496 2022-03-14 22:12:18.000000 pip-check-updates-0.9.2/setup.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2022-03-26 06:07:41.111792 pip-check-updates-0.9.2/tests/
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2021-10-05 06:32:07.000000 pip-check-updates-0.9.2/tests/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2021-10-05 06:32:07.000000 pip-check-updates-0.9.2/tests/conftest.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1261 2021-10-05 06:32:07.000000 pip-check-updates-0.9.2/tests/test_compare_versions.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      513 2021-10-05 06:32:07.000000 pip-check-updates-0.9.2/tests/test_get_current_version.py
```

### Comparing `pip-check-updates-0.9.1/.all-contributorsrc` & `pip-check-updates-0.9.2/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `pip-check-updates-0.9.1/.github/workflows/pytest.yml` & `pip-check-updates-0.9.2/.github/workflows/pytest.yml`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   pull_request:
     branches: [main]
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10"]
     steps:
       - name: Checkout
         uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `pip-check-updates-0.9.1/.vscode/settings.json` & `pip-check-updates-0.9.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pip-check-updates-0.9.1/LICENSE` & `pip-check-updates-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-check-updates-0.9.1/PKG-INFO` & `pip-check-updates-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pip-check-updates
-Version: 0.9.1
+Version: 0.9.2
 Summary: A tool to upgrade dependencies to the latest versions
 Home-page: https://github.com/zehengl/pip-check-updates
 Author: Zeheng Li
 Author-email: imzehengl@gmail.com
 Maintainer: Zeheng Li
 Maintainer-email: imzehengl@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -155,15 +154,17 @@
 
 Show the helper text:
 
 ```terminal
 pcu -h
 ```
 
-    usage: pcu [-h] [-u] [-f FILTER [FILTER ...]] [-t {latest,newest,greatest,minor,patch}] [-x] [-i] [--no_ssl_verify] [--no_recursive] [--ignore_warning] [path]
+    usage: pcu [-h] [-u] [-f FILTER [FILTER ...]] [-t {latest,newest,greatest,minor,patch}] [-x] [-i]
+           [--no_ssl_verify] [--no_recursive] [--ignore_warning] [--show_full_path]
+           [path]
 
     pip-check-updates.
 
     positional arguments:
     path                  specify path to a requirements file
 
     optional arguments:
@@ -174,14 +175,15 @@
     -t {latest,newest,greatest,minor,patch}, --target {latest,newest,greatest,minor,patch}
                             target version to upgrade to: latest, newest, greatest, minor, patch.
     -x, --txt             output new requirements file instead of human-readable message.
     -i, --interactive     enable interactive prompts for each dependency.
     --no_ssl_verify       disable SSL verification.
     --no_recursive        disable recursive checking.
     --ignore_warning      ignore warning.
+    --show_full_path      show full path.
 
 ## Test
 
     python setup.py test
 
 ## Credits
```

### Comparing `pip-check-updates-0.9.1/README.md` & `pip-check-updates-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,17 @@
 
 Show the helper text:
 
 ```terminal
 pcu -h
 ```
 
-    usage: pcu [-h] [-u] [-f FILTER [FILTER ...]] [-t {latest,newest,greatest,minor,patch}] [-x] [-i] [--no_ssl_verify] [--no_recursive] [--ignore_warning] [path]
+    usage: pcu [-h] [-u] [-f FILTER [FILTER ...]] [-t {latest,newest,greatest,minor,patch}] [-x] [-i]
+           [--no_ssl_verify] [--no_recursive] [--ignore_warning] [--show_full_path]
+           [path]
 
     pip-check-updates.
 
     positional arguments:
     path                  specify path to a requirements file
 
     optional arguments:
@@ -151,14 +153,15 @@
     -t {latest,newest,greatest,minor,patch}, --target {latest,newest,greatest,minor,patch}
                             target version to upgrade to: latest, newest, greatest, minor, patch.
     -x, --txt             output new requirements file instead of human-readable message.
     -i, --interactive     enable interactive prompts for each dependency.
     --no_ssl_verify       disable SSL verification.
     --no_recursive        disable recursive checking.
     --ignore_warning      ignore warning.
+    --show_full_path      show full path.
 
 ## Test
 
     python setup.py test
 
 ## Credits
```

### Comparing `pip-check-updates-0.9.1/pip_check_updates/__init__.py` & `pip-check-updates-0.9.2/pip_check_updates/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,14 @@
                     )
                 )
                 continue
             if dep.startswith("-f"):
                 continue
             try:
                 name, current_version, op = get_current_version(dep)
-                deps.append([str(p), name, current_version, op])
+                deps.append([p, name, current_version, op])
             except:
                 pass
 
     deps = list(dep for dep, _ in itertools.groupby(deps))
 
     return deps
```

### Comparing `pip-check-updates-0.9.1/pip_check_updates/__main__.py` & `pip-check-updates-0.9.2/pip_check_updates/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,20 @@
     )
     parser.add_argument(
         "--ignore_warning",
         action="store_true",
         default=False,
         help="ignore warning.",
     )
+    parser.add_argument(
+        "--show_full_path",
+        action="store_true",
+        default=False,
+        help="show full path.",
+    )
 
     args = parser.parse_args()
 
     return args
 
 
 def styled_version(latest_version, change):
@@ -101,14 +107,15 @@
     target = args.target
     no_ssl_verify = args.no_ssl_verify
     filter_ = args.filter
     txt_output = args.txt
     interactive = args.interactive
     no_recursive = args.no_recursive
     ignore_warning = args.ignore_warning
+    show_full_path = args.show_full_path
 
     if upgrade and txt_output:
         print("Oops, cannot specify both -u and -x. Please pick one.")
         return
 
     if no_ssl_verify:
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -181,15 +188,16 @@
                 if keep
             ]
         results = {path: tuple_ for path, tuple_ in results.items() if tuple_}
 
     if results and not txt_output:
         print()
         for path in results:
-            print("In", Fore.BLUE + path + Style.RESET_ALL)
+            _path = str(path) if show_full_path else path.name
+            print("In", Fore.BLUE + _path + Style.RESET_ALL)
             print()
 
             table = []
             for name, current_version, latest_version, change, op in results[path]:
                 table.append(
                     (
                         name,
@@ -199,27 +207,26 @@
                     )
                 )
 
             print(tabulate(table, tablefmt="plain", disable_numparse=True))
 
             print()
 
-        styled_path = [Fore.BLUE + key + Style.RESET_ALL for key in results.keys()]
         if upgrade:
             print(
                 "Run",
                 Fore.YELLOW + f"pip install -r {req_path}" + Style.RESET_ALL,
                 "to install new versions",
             )
         else:
             print(
                 "Run",
-                Fore.YELLOW + "pcu -u" + Style.RESET_ALL,
-                "to upgrade",
-                f"{' and '.join(styled_path)}",
+                Fore.YELLOW + f"pcu {req_path} -u" + Style.RESET_ALL,
+                "to upgrade versions",
+                f"in {len(results)} file{'s' if len(results) > 1 else ''}",
             )
     elif not txt_output:
         print()
         print(
             "All dependencies match the latest package versions",
             Fore.GREEN + ":)" + Style.RESET_ALL,
         )
```

### Comparing `pip-check-updates-0.9.1/pip_check_updates.egg-info/PKG-INFO` & `pip-check-updates-0.9.2/pip_check_updates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pip-check-updates
-Version: 0.9.1
+Version: 0.9.2
 Summary: A tool to upgrade dependencies to the latest versions
 Home-page: https://github.com/zehengl/pip-check-updates
 Author: Zeheng Li
 Author-email: imzehengl@gmail.com
 Maintainer: Zeheng Li
 Maintainer-email: imzehengl@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -155,15 +154,17 @@
 
 Show the helper text:
 
 ```terminal
 pcu -h
 ```
 
-    usage: pcu [-h] [-u] [-f FILTER [FILTER ...]] [-t {latest,newest,greatest,minor,patch}] [-x] [-i] [--no_ssl_verify] [--no_recursive] [--ignore_warning] [path]
+    usage: pcu [-h] [-u] [-f FILTER [FILTER ...]] [-t {latest,newest,greatest,minor,patch}] [-x] [-i]
+           [--no_ssl_verify] [--no_recursive] [--ignore_warning] [--show_full_path]
+           [path]
 
     pip-check-updates.
 
     positional arguments:
     path                  specify path to a requirements file
 
     optional arguments:
@@ -174,14 +175,15 @@
     -t {latest,newest,greatest,minor,patch}, --target {latest,newest,greatest,minor,patch}
                             target version to upgrade to: latest, newest, greatest, minor, patch.
     -x, --txt             output new requirements file instead of human-readable message.
     -i, --interactive     enable interactive prompts for each dependency.
     --no_ssl_verify       disable SSL verification.
     --no_recursive        disable recursive checking.
     --ignore_warning      ignore warning.
+    --show_full_path      show full path.
 
 ## Test
 
     python setup.py test
 
 ## Credits
```

### Comparing `pip-check-updates-0.9.1/pip_check_updates.egg-info/SOURCES.txt` & `pip-check-updates-0.9.2/pip_check_updates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-check-updates-0.9.1/setup.py` & `pip-check-updates-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,13 @@
     long_description_content_type="text/markdown",
     url="https://github.com/zehengl/pip-check-updates",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `pip-check-updates-0.9.1/tests/test_compare_versions.py` & `pip-check-updates-0.9.2/tests/test_compare_versions.py`

 * *Files identical despite different names*

### Comparing `pip-check-updates-0.9.1/tests/test_get_current_version.py` & `pip-check-updates-0.9.2/tests/test_get_current_version.py`

 * *Files identical despite different names*

