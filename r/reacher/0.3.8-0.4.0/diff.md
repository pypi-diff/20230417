# Comparing `tmp/reacher-0.3.8-py2.py3-none-any.whl.zip` & `tmp/reacher-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 7985 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       52 b- defN 23-Mar-26 10:19 reacher/__init__.py
--rw-rw-r--  2.0 unx    19231 b- defN 23-Apr-10 15:22 reacher/reacher.py
--rw-rw-r--  2.0 unx     7010 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      448 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/RECORD
-6 files, 26859 bytes uncompressed, 7177 bytes compressed:  73.3%
+Zip file size: 8459 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx    21950 b- defN 23-Apr-17 17:10 reacher/reacher.py
+-rw-rw-r--  2.0 unx     7010 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      374 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/RECORD
+5 files, 29452 bytes uncompressed, 7765 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: reacher/__init__.py
-Comment: 
-
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.3.8.dist-info/METADATA
+Filename: reacher-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.3.8.dist-info/WHEEL
+Filename: reacher-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.3.8.dist-info/top_level.txt
+Filename: reacher-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.3.8.dist-info/RECORD
+Filename: reacher-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -8,14 +8,15 @@
 from paramiko import AutoAddPolicy, RSAKey, SSHClient
 from paramiko.auth_handler import AuthenticationException, SSHException
 from scp import SCPClient, SCPException
 import logging
 import socket
 import select
 import sys
+import time
 
 try:
     import SocketServer
 except ImportError:
     import socketserver as SocketServer
 
 # Define progress callback that prints the current percentage completed for the file
@@ -91,72 +92,129 @@
 
     def disconnect(self):
         if self.connection:
             self.client.close()
         if self.scp:
             self.scp.close()
 
-    def upload_dir(self, filepath: str, remote_path: str):
-        
+    def upload_file(self, filepath: str, remote_path: str, excluded_exts: List[str] = [".pyc"]):
+
+        if not any(filepath.endswith(ext) for ext in excluded_exts):
+            self.scp.put(filepath, remote_path)
+            logging.info(f"Finished uploading {filepath} to {remote_path} on {self.host}")
+        else:
+            logging.info(f"Skipping {filepath} due to excluded extension")
+    
+    def _upload(self, filepath: str, remote_path: str, excluded_exts: List[str] = [".pyc"]):
+
+        # Execute command to create the remote directory
         self.execute_command(f"mkdir -p {remote_path}")
+
+        if os.path.isfile(filepath):
+            self.upload_file(filepath, remote_path, excluded_exts)
+        else:
         
-        try:
-            self.scp.put(filepath, remote_path=remote_path, recursive=True)
-            logging.info(
-                f"Finished uploading {filepath} files to {remote_path} on {self.host}"
-            )
-        except SCPException as e:
-            logging.error(f"SCPException during bulk upload: {e}")
-        except Exception as e:
-            logging.error(f"Unexpected exception during bulk upload: {e}")
+            try:
+                # Traverse the directory tree
+                for dirpath, _, filenames in os.walk(filepath):
+
+                    remote_dirpath = os.path.join(remote_path, dirpath)
+
+                    # Create remote directories if they don't exist
+                    self.execute_command(f"mkdir -p {remote_dirpath}")
+
+                    # Iterate through files
+                    for filename in filenames:
+                        local_path = os.path.join(dirpath, filename)
+                        # Upload the file
+                        self.upload_file(local_path, remote_dirpath, excluded_exts)
+                      
+                logging.info(
+                    f"Finished uploading {filepath} files to {remote_path} on {self.host}"
+                )
+
+            except Exception as e:
+                logging.error(f"Unexpected exception during bulk upload: {e}")
+
+    def upload(self, filepaths: List[str], remote_path: str, excluded_exts: List[str] = [".pyc"]):
+
+        if not isinstance(filepaths, list):
+            filepaths = [filepaths]
+
+        for filepath in filepaths:
+            self._upload(filepath, remote_path, excluded_exts)
 
     def download_file(self, remote_filepath: str, local_path: str):
 
         os.makedirs(local_path, exist_ok=True)
 
         self.scp.get(remote_filepath, local_path=local_path, recursive=True)
 
-    def execute_command(self, command: str, stream: bool = False, suppress: bool = False):
+    def execute_command(
+        self,
+        command: str,
+        stream: bool = False,
+        suppress: bool = False,
+        ignore_output: bool = False,
+        timeout: int = None,
+    ):
 
         stdin, stdout, stderr = self.connection.exec_command(command, get_pty=True)
 
+        if ignore_output:
+            return
+
         stdout._set_mode('rb')
 
+        last_recieved = time.time()
+
         if stream:
             
             response = ""
 
             for line in iter(stdout.readline, ""):
+                
+                if timeout is not None and (time.time() - last_recieved > timeout):
+                    break
+
                 if line == b"": # finsihed
                     break
                 try:
                     line = line.decode("utf-8")
                 except Exception as e:
                     line = ""
 
                 if not suppress: print(line, end="")
                 response += line
 
+                last_recieved = time.time()
+
             response = None
                         
         else:
 
             stdout.channel.recv_exit_status()
             response = ""
             for line in stdout.readlines():
+
+                if timeout is not None and (time.time() - last_recieved > timeout):
+                    break
+
                 if line == b"": # finsihed
                     break
                 try:
                     line = line.decode("utf-8")
                 except Exception as e:
                     line = ""
 
                 response += line
                 if not suppress: print(line)
 
+                last_recieved = time.time()
+
         stderr.channel.recv_exit_status()
         for line in stderr.readlines():
             print(line)
 
         return response
 
 class Reacher(object):
@@ -257,15 +315,15 @@
                 continue
             if x == "" or x == "." or x == "..":
                 continue
             files_pruned.append(x)
 
         if len(files_pruned) > 0:
             cmd = f"rm -r {' '.join(files_pruned)}"
-            self.execute_command(cmd)
+            self.execute_command(cmd, suppress=True)
 
         self.setup()
 
     def ls(self, folder: str = None):
 
         if folder is None:
             folder = self.build_path
@@ -278,31 +336,38 @@
             stream=False,
         ).replace("\n", "").split("\r")
 
         r = [x for x in r if x != "" and x != "."]
 
         return r
 
-    def put(self, path: str, destination_folder: str = None):
+    def put(self, path: str, destination_folder: str = None, excluded_exts: list = [".pyc"]):
         
         if destination_folder is None:
             destination_folder = self.build_path
         else:
             destination_folder = os.path.join(self.build_path, destination_folder)
 
         if not isinstance(path, list):
             path = [path]
 
         for p in path:
-            self._client.upload_dir(p, destination_folder)
+            self._client.upload(p, destination_folder, excluded_exts=excluded_exts)
+
+        # make sure all files are owned by the user
+        self._client.execute_command(
+            f"find {self.build_path}" + " -user $(whoami) -exec chmod 777 {} \;",
+            stream=False,
+            suppress=False,
+        )
 
     def get(self, path: Union[List[str], str], destination_folder: str = None):
 
         if destination_folder is None:
-            destination_folder = os.path.join(".reacher", self._build_name)
+            destination_folder = "."
 
         if not isinstance(path, list):
             path = [path]
 
         for p in path:
             self._client.download_file(os.path.join(self.build_path, p), destination_folder)
 
@@ -321,59 +386,65 @@
         named_session = named_session if named_session is not None else uuid.uuid4()
 
         return f"screen -S {named_session} {command}"
     
     def _wrap_command_in_prefix(self, command: str):
         
         return f"{self._prefix_cmd};{command}"
+    
+    def execute(
+        self,
+        command: str,
+        context: Union[str, List[str]] = None,
+        named_session: str = None,
+        cleanup_before: bool = False,
+        wrap_in_screen: bool = True,
+        excluded_exts: list = [".pyc"],
+    ):  
+
+        if cleanup_before:
+            self.cleanup()
+
+        if context is not None:
+            self._client.upload(context, self.build_path, excluded_exts)
+
+        self.execute_command(
+            command,
+            named_session=named_session,
+            wrap_in_screen=wrap_in_screen
+        )
+
 
     def execute_command(
         self,
         command,
         stream: bool = True,
         suppress: bool = False,
         named_session: str = None,
         wrap_in_screen: bool = False,
+        ignore_output: bool = False,
+        timeout: int = None,
     ):  
 
         if wrap_in_screen:
             command = self._wrap_command_in_screen(command, named_session=named_session)
 
         if self._prefix_cmd is not None:
             command = self._wrap_command_in_prefix(command)
 
         command = f"cd {self.build_path} && {command}"
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
+            ignore_output=ignore_output,
+            timeout=timeout,
         )
-
-    def execute(
-        self,
-        command: str,
-        context: Union[str, List[str]] = None,
-        named_session: str = None,
-        wrap_in_screen: bool = True,
-        cleanup_before: bool = True,
-    ):      
-        
-        if cleanup_before:
-            self.cleanup()
-
-        if context is not None:
-            self._client.upload_dir(context, self.build_path)
-
-        self.execute_command(
-            command,
-            named_session=named_session,
-            wrap_in_screen=wrap_in_screen,
-        )
-
+    
     def list_named_sessions(self):
 
         self.execute_command(f"screen -list")
 
     def attach_named_session(self, named_session: str):
 
         self.execute_command(f"screen -r -d {named_session}")
@@ -417,15 +488,15 @@
         self._image_name = image_name
         self._build_context = build_context 
 
     def _setup_remote(self):
 
         super()._setup_remote()
 
-        self._client.upload_dir(
+        self._client.upload(
             self._build_context,
             self.build_path,
         )
 
     def clear(self):
 
         if self.is_running:
@@ -434,16 +505,14 @@
             )
 
         if self.exists:
             self._client.execute_command(
                 f"docker rm {self._build_name}", suppress=True,
             )
 
-        super().clear()
-
     def ls(self, folder: str = None):
 
         if folder is None:
             folder = "."
 
         r = self.execute_command(
             f"find {folder} -mindepth 1 -print",
@@ -467,55 +536,27 @@
     def execute_command(
         self,
         command,
         stream: bool = True,
         suppress: bool = False,
         named_session: str = None,
         wrap_in_screen: bool = False,
+        ignore_output: bool = False,
     ):  
 
         if wrap_in_screen or named_session is not None:
             command = self._wrap_command_in_screen(command, named_session=named_session)
 
         command = f"docker exec -it {self._build_name} {command}"
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
-        )
-
-    def execute(
-        self,
-        command: str,
-        context: Union[str, List[str]] = None,
-        named_session: str = None,
-        cleanup_before: bool = False,
-        wrap_in_screen: bool = True,
-    ):  
-
-        if cleanup_before:
-            self.cleanup()
-
-        tmp_path = os.path.join(self.build_path, "tmp")
-        self._client.execute_command(f"mkdir -p {tmp_path}")
-
-        if context is not None:
-            self._client.upload_dir(context, tmp_path)
-
-        self._client.execute_command(
-            f"docker cp {tmp_path}/. {self._build_name}:/{ReacherDocker.CON_WORKSPACE_PATH}"
-        )
-
-        self._client.execute_command(f"rm -r {tmp_path}")
-
-        self.execute_command(
-            command,
-            named_session=named_session,
-            wrap_in_screen=wrap_in_screen
+            ignore_output=ignore_output,
         )
 
     def setup(
         self,
         ports: List[int] = None,
         envs: Dict[str, str] = None,
         command: str = "sleep infinity",
@@ -527,16 +568,15 @@
         extra_args = ""
 
         if gpu:
             extra_args = "--runtime=nvidia --gpus all"
 
         ctx = f"docker run -dt {extra_args} -w {ReacherDocker.CON_WORKSPACE_PATH} --name {self._build_name}"
 
-        ctx = f"{ctx} -v {self.artifact_path}:{ReacherDocker.CON_WORKSPACE_PATH}/{Reacher.ARTIFACATS_PATH}"
-        ctx = f"{ctx} -v  {self.log_path}:{ReacherDocker.CON_WORKSPACE_PATH}/{Reacher.LOGS_PATH}"
+        ctx = f"{ctx} -v {self.build_path}:{ReacherDocker.CON_WORKSPACE_PATH}"
 
         if ports is not None:
             for p in ports:
                 ctx = f"{ctx} -p {p}:{p}"
 
         if envs is not None:
             for k, v in envs.items():
@@ -695,8 +735,56 @@
                 target=forward_tunnel_system,
                 args=(local_port, remote_port, self._client),
                 daemon=True
             )
 
         self._threads.append(x)
         
-        self._threads[-1].start()
+        self._threads[-1].start()
+
+
+## Some helper functions for creating notebooks and tensorboards
+
+def create_notebook(
+        reacher: Reacher,
+        remote_port: int,
+        local_port: int,
+        paramiko: bool = False
+    ):
+
+    reacher.execute_command(
+        f"jupyter notebook --ip 0.0.0.0 --allow-root --port {remote_port}",
+        wrap_in_screen=True,
+        named_session="notebook",
+        ignore_output=True,
+        timeout=1,
+    )
+
+    reacher.add_port_forward(remote_port=remote_port, local_port=local_port, paramiko=paramiko)
+
+    r = reacher.execute_command("jupyter notebook list", stream=False, suppress=True)
+
+    r = r.replace(str(remote_port), str(local_port))
+
+    print(r)
+
+def create_tensorboard(
+    reacher: Reacher,
+    remote_port: int,
+    local_port: int,
+    paramiko: bool = False,
+    logdir: str = "artifacts"
+):
+    
+    reacher.execute_command(f"mkdir -p {logdir}")
+
+    reacher.execute_command(
+        f"tensorboard --host 0.0.0.0 --port {remote_port} --logdir {logdir}",
+        wrap_in_screen=True,
+        named_session="tensorboard",
+        ignore_output=True,
+        timeout=1,
+    )
+
+    reacher.add_port_forward(remote_port=remote_port, local_port=local_port, paramiko=paramiko)
+
+    print(f"tensorboard running on\nhttp://0.0.0.0:{local_port}/")
```

## Comparing `reacher-0.3.8.dist-info/METADATA` & `reacher-0.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.3.8
+Version: 0.4.0
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

