# Comparing `tmp/kiki_utils_ssh-1.0.1.tar.gz` & `tmp/kiki_utils_ssh-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiki_utils_ssh-1.0.1.tar", last modified: Fri Nov 25 14:19:34 2022, max compression
+gzip compressed data, was "kiki_utils_ssh-1.0.2.tar", last modified: Mon Apr 17 11:20:49 2023, max compression
```

## Comparing `kiki_utils_ssh-1.0.1.tar` & `kiki_utils_ssh-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-25 14:19:34.643777 kiki_utils_ssh-1.0.1/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2022-11-25 08:13:40.000000 kiki_utils_ssh-1.0.1/LICENSE.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      247 2022-11-25 14:19:34.643777 kiki_utils_ssh-1.0.1/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-25 08:13:09.000000 kiki_utils_ssh-1.0.1/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-25 14:19:34.643777 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      247 2022-11-25 14:19:34.000000 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      278 2022-11-25 14:19:34.000000 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2022-11-25 14:19:34.000000 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        9 2022-11-25 14:19:34.000000 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       14 2022-11-25 14:19:34.000000 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2022-11-25 14:19:34.000000 kiki_utils_ssh-1.0.1/kiki_utils_ssh.egg-info/zip-safe
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-25 14:19:34.643777 kiki_utils_ssh-1.0.1/kikiutils_ssh/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     3760 2022-11-25 14:18:32.000000 kiki_utils_ssh-1.0.1/kikiutils_ssh/__init__.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2022-11-25 14:19:34.643777 kiki_utils_ssh-1.0.1/setup.cfg
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      453 2022-11-25 14:19:22.000000 kiki_utils_ssh-1.0.1/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 11:20:49.263413 kiki_utils_ssh-1.0.2/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2023-04-17 11:16:53.000000 kiki_utils_ssh-1.0.2/LICENSE.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      247 2023-04-17 11:20:49.263413 kiki_utils_ssh-1.0.2/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 11:16:53.000000 kiki_utils_ssh-1.0.2/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 11:20:49.263413 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      247 2023-04-17 11:20:49.000000 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      278 2023-04-17 11:20:49.000000 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-04-17 11:20:49.000000 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        9 2023-04-17 11:20:49.000000 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       14 2023-04-17 11:20:49.000000 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-04-17 11:20:49.000000 kiki_utils_ssh-1.0.2/kiki_utils_ssh.egg-info/zip-safe
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 11:20:49.263413 kiki_utils_ssh-1.0.2/kikiutils_ssh/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     3634 2023-04-17 11:19:08.000000 kiki_utils_ssh-1.0.2/kikiutils_ssh/__init__.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-04-17 11:20:49.263413 kiki_utils_ssh-1.0.2/setup.cfg
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      453 2023-04-17 11:20:32.000000 kiki_utils_ssh-1.0.2/setup.py
```

### Comparing `kiki_utils_ssh-1.0.1/LICENSE.txt` & `kiki_utils_ssh-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kiki_utils_ssh-1.0.1/kikiutils_ssh/__init__.py` & `kiki_utils_ssh-1.0.2/kikiutils_ssh/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,20 +73,15 @@
         return await self.s.isfile(path)
 
     async def mkdir(self, remotepath: str, **kwargs):
         """Make remote directory."""
 
         await self.s.mkdir(remotepath, **kwargs)
 
-    async def mkdirs(
-        self,
-        remotepath: str,
-        exist_ok: bool = True,
-        **kwargs
-    ):
+    async def mkdirs(self, remotepath: str, exist_ok: bool = True, **kwargs):
         """Make remote directories."""
 
         await self.s.makedirs(remotepath, exist_ok=exist_ok, **kwargs)
 
     async def putdir(self, localpath: str, remotepath: str, **kwargs):
         """Upload dir."""
 
@@ -111,40 +106,28 @@
         """Force remove remote dir.
 
         @param `kwargs` - sftp rmtree other parameters.
         """
 
         await self.s.rmtree(remotepath, **kwargs)
 
-    async def run(
-        self,
-        command: str,
-        get_std_out: bool = True,
-        **kwargs
-    ):
+    async def run(self, command: str, get_std_out: bool = True, **kwargs):
         """Run command and return stdout or `SSHCompletedProcess`."""
 
         result = await self.c.run(command, **kwargs)
 
         if get_std_out:
             return str(result.stdout)
 
         return result
 
-    async def run_and_show(
-        self,
-        command: str,
-        **kwargs
-    ):
+    async def run_and_show(self, command: str, **kwargs):
         """Run command and instant display result, then return all result."""
 
-        results = ''
-        process = await self.c.create_process(
-            command,
-            **kwargs
-        )
+        results = []
+        process = await self.c.create_process(command, **kwargs)
 
         async for line in process.stdout:
-            results += str(line)
+            results.append(str(line))
             print(line, end='')
 
-        return results
+        return ''.join(results)
```

