# Comparing `tmp/pygeoweaver-0.6.2.tar.gz` & `tmp/pygeoweaver-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.2.tar", last modified: Sun Apr 16 21:25:08 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.4.tar", last modified: Sun Apr 16 23:36:45 2023, max compression
```

## Comparing `pygeoweaver-0.6.2.tar` & `pygeoweaver-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/test/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:36:45.108873 pygeoweaver-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-16 23:36:45.108873 pygeoweaver-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:36:45.104873 pygeoweaver-0.6.4/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:36:45.108873 pygeoweaver-0.6.4/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-16 23:36:45.000000 pygeoweaver-0.6.4/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-16 23:36:45.000000 pygeoweaver-0.6.4/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:36:45.000000 pygeoweaver-0.6.4/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 23:36:45.000000 pygeoweaver-0.6.4/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 23:36:45.108873 pygeoweaver-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:36:45.108873 pygeoweaver-0.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 23:36:34.000000 pygeoweaver-0.6.4/test/test_all.py
```

### Comparing `pygeoweaver-0.6.2/LICENSE` & `pygeoweaver-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.2/PKG-INFO` & `pygeoweaver-0.6.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.2
+Version: 0.6.4
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -37,65 +37,76 @@
 ```
 geoweaver.stop()
 ```
 
 3. To list the existing objects, please run:
 
 ```
-geoweaver.list("host")
-geoweaver.list("process")
-geoweaver.list("workflow")
+geoweaver.list_hosts()
+geoweaver.list_processes()
+geoweaver.list_workflows()
 ```
 
 4. To run a workflow, please run:
 ```
-geoweaver.run_workflow()
+geoweaver.run_workflow("workflow_id", "host_id_list", "password_list", "environment_list")
+```
+
+or
+
+```
+geoweaver.run_workflow("workflow_zip_file_path", "host_id_list", "password_list", "environment_list")
+```
+
+or 
+
+```
+geoweaver.run_workflow("workflow_local_folder_path", "host_id_list", "password_list", "environment_list")
 ```
 
 5. To export a workflow:
 
 ```
 geoweaver.export_workflow("workflow_id", "workflow_zip_save_path")
 ```
 
 6. To import a workflow:
 
 ```
-geoweaver.import_workflow("workflow_zip_file_path")
+geoweaver.import_workflow("<workflow_zip_file_path>")
 ```
 
 or
 
 ```
-geoweaver.import_workflow("workflow_folder_path")
+geoweaver.import_workflow("<workflow_folder_path>")
 ```
 
 7. To get history of a workflow run:
 
 ```
-geoweaver.history_workflow()
+geoweaver.history("<workflow_history_id>")
 ```
 
 8. To get history of a process run:
 
 ```
-geoweaver.history_process()
+geoweaver.history("<process_history_id>")
 ```
 
 9. To check the source code of a process
 
 ```
-geoweaver.detail_processs(process_id)
+geoweaver.detail_processs("<process_id>")
 ```
 
 10. To check the configuration of a workflow
 
 ```
-geoweaver.detail_workflow(workflow_id)
+geoweaver.detail_workflow("<workflow_id>")
 ```
 
 11. To check the details of a host:
 
 ```
-geoweaver.detail_host(host_id)
+geoweaver.detail_host("<host_id>")
 ```
-
```

### Comparing `pygeoweaver-0.6.2/README.md` & `pygeoweaver-0.6.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,65 +24,76 @@
 ```
 geoweaver.stop()
 ```
 
 3. To list the existing objects, please run:
 
 ```
-geoweaver.list("host")
-geoweaver.list("process")
-geoweaver.list("workflow")
+geoweaver.list_hosts()
+geoweaver.list_processes()
+geoweaver.list_workflows()
 ```
 
 4. To run a workflow, please run:
 ```
-geoweaver.run_workflow()
+geoweaver.run_workflow("workflow_id", "host_id_list", "password_list", "environment_list")
+```
+
+or
+
+```
+geoweaver.run_workflow("workflow_zip_file_path", "host_id_list", "password_list", "environment_list")
+```
+
+or 
+
+```
+geoweaver.run_workflow("workflow_local_folder_path", "host_id_list", "password_list", "environment_list")
 ```
 
 5. To export a workflow:
 
 ```
 geoweaver.export_workflow("workflow_id", "workflow_zip_save_path")
 ```
 
 6. To import a workflow:
 
 ```
-geoweaver.import_workflow("workflow_zip_file_path")
+geoweaver.import_workflow("<workflow_zip_file_path>")
 ```
 
 or
 
 ```
-geoweaver.import_workflow("workflow_folder_path")
+geoweaver.import_workflow("<workflow_folder_path>")
 ```
 
 7. To get history of a workflow run:
 
 ```
-geoweaver.history_workflow()
+geoweaver.history("<workflow_history_id>")
 ```
 
 8. To get history of a process run:
 
 ```
-geoweaver.history_process()
+geoweaver.history("<process_history_id>")
 ```
 
 9. To check the source code of a process
 
 ```
-geoweaver.detail_processs(process_id)
+geoweaver.detail_processs("<process_id>")
 ```
 
 10. To check the configuration of a workflow
 
 ```
-geoweaver.detail_workflow(workflow_id)
+geoweaver.detail_workflow("<workflow_id>")
 ```
 
 11. To check the details of a host:
 
 ```
-geoweaver.detail_host(host_id)
+geoweaver.detail_host("<host_id>")
 ```
-
```

### Comparing `pygeoweaver-0.6.2/pygeoweaver/__main__.py` & `pygeoweaver-0.6.4/test/test_all.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 from pygeoweaver import detail_host, detail_process, detail_workflow
 from pygeoweaver import export_workflow
 from pygeoweaver import show_history
 from pygeoweaver import import_workflow
 from pygeoweaver import list_hosts, list_processes, list_workflows
 from pygeoweaver import start, stop
 
-def main():
-    # start geoweaver
-    start()
-    # stop geoweaver
-    # stop()
-    # list resources
-    #list_hosts()
-    #list_processes()
-    # list_workflows()
-    # show history
-    #show_history("ll3u3W78eOEfklxhBJ")
-    # detail host
-    # detail_host("100001")
-    # detail process
-    # detail_process("7pxu8c")
-    #detail_workflow("5jnhcrq33znbu2mue9v2")
-    # import workflow
-    #import_workflow("/Users/joe/Downloads/gr3ykr8dynu12vrwq11oy.zip")
-    # export workflow
-    # export_workflow("gr3ykr8dynu12vrwq11oy", "4", "/Users/joe/Downloads/test_pygeoweaver_export.zip")
-    # run workflow
+import unittest
+
+class Testing(unittest.TestCase):
+
+    def test_main():
+        # start geoweaver
+        #start()
+        # stop geoweaver
+        # stop()
+        # list resources
+        #list_hosts()
+        #list_processes()
+        list_workflows()
+        # show history
+        #show_history("ll3u3W78eOEfklxhBJ")
+        # detail host
+        # detail_host("100001")
+        # detail process
+        # detail_process("7pxu8c")
+        #detail_workflow("5jnhcrq33znbu2mue9v2")
+        # import workflow
+        #import_workflow("/Users/joe/Downloads/gr3ykr8dynu12vrwq11oy.zip")
+        # export workflow
+        export_workflow("gr3ykr8dynu12vrwq11oy", "4", "/Users/joe/Downloads/test_pygeoweaver_export.zip")
 
 
 if __name__ == "__main__":
-     main()
+    unittest.main()
```

### Comparing `pygeoweaver-0.6.2/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.4/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.2/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.4/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.2/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.4/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.2/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.4/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.2/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.4/pygeoweaver/sc_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 import subprocess
 from pygeoweaver.utils import download_geoweaver_jar, get_geoweaver_jar_path, get_root_dir
 
 
-def run_process(*, process_id, host_id, password, environment):
-    if not host_id:
-        raise RuntimeError("Host id is missing")
+def run_process(*, process_id: str, host_id: str, password: str, environment: str=None):
+    """
+    Run a process
+
+    Args: process_id - required
+        host_id - required
+        password - required
+        environment - optional
+    """
     download_geoweaver_jar()
     subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "run", "process", f"--host={host_id}",
                     f"--password={password}", f"--environment={environment}", process_id],
                    cwd=f"{get_root_dir()}/")
 
-def run_worklfow(*, workflow_id, workflow_folder_path, workflow_zip_file_path, environments, host, password):
+def run_worklfow(*, workflow_id: str, workflow_folder_path: str=None, workflow_zip_file_path: str=None, 
+                 environment_list: str=None, host_list: str, password_list: str):
     """
-    Missing required parameter: '<workflowId>'
     Usage: <main class> run workflow [-d=<workflowFolderPath>]
                                     [-f=<workflowZipPath>] [-e=<envs>]...
                                     [-h=<hostStrings>]... [-p=<passes>]...
                                     <workflowId>
         <workflowId>           workflow id to run
     -d, --workflow-folder-path=<workflowFolderPath>
                                 geoweaver workflow folder path
-    -e, --environments=<envs>  environments to run on
+    -e, --environments=<envs>  environments to run on. List of environment ids with comma as separator
     -f, --workflow-zip-file-path=<workflowZipPath>
                                 workflow package or path to workflow zip to run
-    -h, --hosts=<hostStrings>  hosts to run on
-    -p, --passwords=<passes>   passwords to the target hosts
+    -h, --hosts=<hostStrings>  hosts to run on. list of host ids with comma as separator.
+    -p, --passwords=<passes>   passwords to the target hosts. list of passwords with comma as separator. 
     """
     download_geoweaver_jar()
 
-    if workflow_folder_path and workflow_zip_file_path:
-        raise RuntimeError("Please provide either Folder path or Zip path")
+    if not workflow_id and not workflow_folder_path and not workflow_zip_file_path:
+        raise RuntimeError("Please provide at least one of the three options: workflow id, " \
+                           "folder path or zip path")
+    
+    if workflow_id and not workflow_folder_path and not workflow_zip_file_path:
+        subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "run", "workflow", workflow_id,
+                        "-e", environment_list,
+                        "-h", host_list,
+                        "-p", password_list],
+                       cwd=f"{get_root_dir()}/")
 
     if workflow_folder_path and not workflow_zip_file_path:
         # command to run workflow from folder
         subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "run", "workflow", workflow_id,
                         "-d", workflow_folder_path,
-                        "-e", environments,
-                        "-h", host,
-                        "-p", password],
+                        "-e", environment_list,
+                        "-h", host_list,
+                        "-p", password_list],
                        cwd=f"{get_root_dir()}/")
 
     if not workflow_folder_path and workflow_zip_file_path:
         subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "run", "workflow", workflow_id,
-                        "-e", environments,
+                        "-e", environment_list,
                         "-f", workflow_zip_file_path,
-                        "-h", host,
-                        "-p", password],
+                        "-h", host_list,
+                        "-p", password_list],
                        cwd=f"{get_root_dir()}/")
-
-    raise RuntimeError("Please provide either zip path or directory path to run workflow.")
+
```

### Comparing `pygeoweaver-0.6.2/pygeoweaver/utils.py` & `pygeoweaver-0.6.4/pygeoweaver/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import subprocess
 import requests
-
+import platform
 
 def get_home_dir():
     return os.path.expanduser('~')
 
 
 def get_root_dir():
     head, tail = os.path.split(__file__)
@@ -35,7 +35,16 @@
         f.write(r.content)
 
     if check_geoweaver_jar():
         print("Geoweaver.jar is downloaded")
 
     else:
         raise RuntimeError("Fail to download geoweaver.jar")
+
+
+def checkOS():
+    if platform.system() == "Linux" or platform == "Linux2":
+        return 1
+    elif platform.system() == "Darwin":
+        return 2
+    elif platform == "Windows":
+        return 3
```

### Comparing `pygeoweaver-0.6.2/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.4/pygeoweaver.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.2
+Version: 0.6.4
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -37,65 +37,76 @@
 ```
 geoweaver.stop()
 ```
 
 3. To list the existing objects, please run:
 
 ```
-geoweaver.list("host")
-geoweaver.list("process")
-geoweaver.list("workflow")
+geoweaver.list_hosts()
+geoweaver.list_processes()
+geoweaver.list_workflows()
 ```
 
 4. To run a workflow, please run:
 ```
-geoweaver.run_workflow()
+geoweaver.run_workflow("workflow_id", "host_id_list", "password_list", "environment_list")
+```
+
+or
+
+```
+geoweaver.run_workflow("workflow_zip_file_path", "host_id_list", "password_list", "environment_list")
+```
+
+or 
+
+```
+geoweaver.run_workflow("workflow_local_folder_path", "host_id_list", "password_list", "environment_list")
 ```
 
 5. To export a workflow:
 
 ```
 geoweaver.export_workflow("workflow_id", "workflow_zip_save_path")
 ```
 
 6. To import a workflow:
 
 ```
-geoweaver.import_workflow("workflow_zip_file_path")
+geoweaver.import_workflow("<workflow_zip_file_path>")
 ```
 
 or
 
 ```
-geoweaver.import_workflow("workflow_folder_path")
+geoweaver.import_workflow("<workflow_folder_path>")
 ```
 
 7. To get history of a workflow run:
 
 ```
-geoweaver.history_workflow()
+geoweaver.history("<workflow_history_id>")
 ```
 
 8. To get history of a process run:
 
 ```
-geoweaver.history_process()
+geoweaver.history("<process_history_id>")
 ```
 
 9. To check the source code of a process
 
 ```
-geoweaver.detail_processs(process_id)
+geoweaver.detail_processs("<process_id>")
 ```
 
 10. To check the configuration of a workflow
 
 ```
-geoweaver.detail_workflow(workflow_id)
+geoweaver.detail_workflow("<workflow_id>")
 ```
 
 11. To check the details of a host:
 
 ```
-geoweaver.detail_host(host_id)
+geoweaver.detail_host("<host_id>")
 ```
-
```

### Comparing `pygeoweaver-0.6.2/pyproject.toml` & `pygeoweaver-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.2"
+version = "0.6.4"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

