# Comparing `tmp/wks-0.2.6.tar.gz` & `tmp/wks-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wks-0.2.6.tar", last modified: Fri Jul  1 19:45:52 2022, max compression
+gzip compressed data, was "wks-0.2.7.tar", last modified: Mon Apr 17 12:00:16 2023, max compression
```

## Comparing `wks-0.2.6.tar` & `wks-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2022-07-01 19:45:52.091231 wks-0.2.6/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      321 2022-07-01 19:45:52.091231 wks-0.2.6/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2306 2022-04-07 19:47:19.000000 wks-0.2.6/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2022-07-01 19:45:52.091231 wks-0.2.6/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2022-07-01 19:45:43.000000 wks-0.2.6/setup.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2021-08-17 09:01:24.000000 wks-0.2.6/wks
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2022-07-01 19:45:52.087231 wks-0.2.6/wks.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      321 2022-07-01 19:45:51.000000 wks-0.2.6/wks.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      489 2022-07-01 19:45:51.000000 wks-0.2.6/wks.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2022-07-01 19:45:51.000000 wks-0.2.6/wks.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2022-07-01 19:45:51.000000 wks-0.2.6/wks.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2022-07-01 19:45:51.000000 wks-0.2.6/wks.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2022-07-01 19:45:52.091231 wks-0.2.6/workspace/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4235 2022-05-24 14:46:25.000000 wks-0.2.6/workspace/cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2022-06-15 05:53:43.000000 wks-0.2.6/workspace/command_build.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/command_cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/command_cmd.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/command_graph.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/command_help.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/command_install.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-06-22 10:43:05.000000 wks-0.2.6/workspace/command_pull.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/command_status.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      378 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/commands.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/env.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5446 2022-07-01 19:45:36.000000 wks-0.2.6/workspace/git.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-05-24 14:46:35.000000 wks-0.2.6/workspace/message.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-17 12:00:16.637341 wks-0.2.7/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-04-17 12:00:16.637341 wks-0.2.7/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2306 2022-03-24 13:57:35.000000 wks-0.2.7/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-04-17 12:00:16.637341 wks-0.2.7/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2023-04-17 11:58:08.000000 wks-0.2.7/setup.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2021-06-24 13:33:28.000000 wks-0.2.7/wks
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-17 12:00:16.633340 wks-0.2.7/wks.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      489 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-17 12:00:16.637341 wks-0.2.7/workspace/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4235 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2023-04-17 11:59:39.000000 wks-0.2.7/workspace/command_build.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_cmd.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_graph.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_help.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_install.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-10-20 08:37:11.000000 wks-0.2.7/workspace/command_pull.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_status.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      378 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/commands.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/env.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5695 2023-04-17 11:59:13.000000 wks-0.2.7/workspace/git.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/message.py
```

### Comparing `wks-0.2.6/README.md` & `wks-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/setup.py` & `wks-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wks",
-    version="0.2.6",
+    version="0.2.7",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Simple dependencies manager for cmake projects in your workspace",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/rhoban/wks/",
     packages=setuptools.find_packages(),
```

### Comparing `wks-0.2.6/wks` & `wks-0.2.7/wks`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/workspace/cmake.py` & `wks-0.2.7/workspace/cmake.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/workspace/command_build.py` & `wks-0.2.7/workspace/command_build.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/workspace/command_graph.py` & `wks-0.2.7/workspace/command_graph.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/workspace/command_help.py` & `wks-0.2.7/workspace/command_help.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/workspace/command_status.py` & `wks-0.2.7/workspace/command_status.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.6/workspace/git.py` & `wks-0.2.7/workspace/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             if scan_dependencies(directory):
                 changed = True
 
 
 def global_command(command, vendor_filter=None):
     message.bright("* Running global command: %s" % command)
 
+    use_threads = os.getenv('WKS_NO_THREADS') is None
     directories = get_directories()
 
     threads: list[threading.Thread] = [None] * len(directories)
     processes: list[subprocess.CompletedProcess] = threads.copy()
 
     def thread_func(index: int, dir: str, cmd: str):
         processes[index] = subprocess.run(cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=dir)
@@ -137,21 +138,26 @@
     for index, directory in enumerate(directories):
         if vendor_filter is not None:
             parts = directory.split("/")
             vendor = parts[-2]
             if vendor.lower() != vendor_filter.lower():
                 continue
 
-        threads[index] = threading.Thread(None, thread_func, args=(index, directory, command))
-        threads[index].start()
-
-    for index, thread in enumerate(threads):
-        thread.join()
-        message.bright("- In %s ..." % os.path.realpath(directory))
-        print(processes[index].stdout.decode())
+        if use_threads:
+            threads[index] = threading.Thread(None, thread_func, args=(index, directory, command))
+            threads[index].start()
+        else:
+            message.bright("> %s" % directory)
+            thread_func(index, directory, command)
+
+    if use_threads:
+        for index, directory in enumerate(directories):
+            threads[index].join()
+            message.bright("- In %s ..." % os.path.realpath(directory))
+            print(processes[index].stdout.decode())
 
     print("")
 
 
 def status(directory):
     output = subprocess.getoutput("cd %s; git status --porcelain=v1" % directory)
     return output
```

### Comparing `wks-0.2.6/workspace/message.py` & `wks-0.2.7/workspace/message.py`

 * *Files identical despite different names*

