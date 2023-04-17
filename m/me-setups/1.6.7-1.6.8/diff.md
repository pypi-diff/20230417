# Comparing `tmp/me_setups-1.6.7.tar.gz` & `tmp/me_setups-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.6.7.tar", last modified: Sun Apr 16 12:28:05 2023, max compression
+gzip compressed data, was "me_setups-1.6.8.tar", last modified: Mon Apr 17 15:08:22 2023, max compression
```

## Comparing `me_setups-1.6.7.tar` & `me_setups-1.6.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-16 12:28:05.650299 me_setups-1.6.7/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-16 12:28:05.651262 me_setups-1.6.7/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.7/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-16 12:28:05.654250 me_setups-1.6.7/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.7/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-16 12:28:05.610325 me_setups-1.6.7/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-16 12:28:05.623495 me_setups-1.6.7/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.7/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-16 12:28:05.641227 me_setups-1.6.7/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.7/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.7/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    10534 2023-04-04 16:39:15.000000 me_setups-1.6.7/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.7/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-16 12:28:05.648541 me_setups-1.6.7/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.7/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8629 2023-04-13 08:32:16.000000 me_setups-1.6.7/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11841 2023-04-16 12:25:40.000000 me_setups-1.6.7/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.7/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.7/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.7/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-16 12:28:05.633242 me_setups-1.6.7/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-16 12:28:05.000000 me_setups-1.6.7/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-16 12:28:05.000000 me_setups-1.6.7/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-16 12:28:05.000000 me_setups-1.6.7/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-16 12:28:05.000000 me_setups-1.6.7/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-16 12:28:05.000000 me_setups-1.6.7/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.125926 me_setups-1.6.8/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-17 15:08:22.126908 me_setups-1.6.8/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.8/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-17 15:08:22.128933 me_setups-1.6.8/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.8/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.083221 me_setups-1.6.8/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.095888 me_setups-1.6.8/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.8/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.114887 me_setups-1.6.8/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.8/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.8/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    10582 2023-04-17 15:06:51.000000 me_setups-1.6.8/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.8/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.124907 me_setups-1.6.8/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.8/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8506 2023-04-17 14:42:22.000000 me_setups-1.6.8/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11841 2023-04-16 12:25:40.000000 me_setups-1.6.8/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.8/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.8/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.8/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.108563 me_setups-1.6.8/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-17 15:08:22.000000 me_setups-1.6.8/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.6.7/PKG-INFO` & `me_setups-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.6.7
+Version: 1.6.8
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.7/setup.cfg` & `me_setups-1.6.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.6.7
+version = 1.6.8
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.6.7/src/me_setups/boards/default_boards.py` & `me_setups-1.6.8/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.7/src/me_setups/boards/gas52.py` & `me_setups-1.6.8/src/me_setups/boards/gas52.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import pathlib
 import sys
 import time
 from concurrent.futures import as_completed
 from concurrent.futures import ThreadPoolExecutor
 from subprocess import CompletedProcess
+from typing import Any
 from typing import Generator
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -171,25 +172,25 @@
                 conn.serial.open()
 
     def restart_serials(self) -> None:
         """restart all serials conns, close and open"""
         self.close_serials()
         self.open_serials()
 
-    def run_ssh_cmd_all(self, cmd: str) -> list[CompletedProcess[str]]:
+    def run_ssh_cmd_all(self, cmd: str, **kwargs: Any) -> list[CompletedProcess[str]]:
         """run ssh command on all eqs.
 
         Args:
             cmd (str): the command to run
 
         Returns:
             list[CompletedProcess[str]]: list off all commands proccesses
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
-            fs = [executor.submit(eq.run_ssh_cmd, cmd) for eq in self.eqs]
+            fs = [executor.submit(eq.run_ssh_cmd, cmd, **kwargs) for eq in self.eqs]
         return [f.result() for f in fs]
 
     def run_serial_cmd_all(self, cmd: str) -> None:
         """run serial command on all eqs.
 
         Args:
             cmd (str): the command to run
```

### Comparing `me_setups-1.6.7/src/me_setups/components/comp.py` & `me_setups-1.6.8/src/me_setups/components/comp.py`

 * *Files 14% similar despite different names*

```diff
@@ -123,24 +123,23 @@
         if exc_type or exc or traceback:
             return False
         else:
             return None
 
 
 class SerialSniffer(Serial):
-    sniff_thread: ReaderThread
     timeout: float
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """\
             Serial port with built in Sniffer.
         """
         super().__init__(*args, **kwargs)
         self.protocol = Sniffer()
-        self._sniffing = False
+        self.sniff_thread = ReaderThread(self)
 
     def read(self, size: int = 1) -> bytes:
         """read from serial and call the Sniffer protocol.
 
         Args:
             size (int, optional): size to read. Defaults to 1.
 
@@ -170,28 +169,25 @@
 
     def start_sniffing(self) -> ReaderThread:
         """start the sniffing thread
 
         Returns:
             ReaderThread: The sniffing thread
         """
-        self.sniff_thread = ReaderThread(self)
+        if not self.sniff_thread.is_alive():
+            self.sniff_thread = ReaderThread(self)
         self.sniff_thread.start()
-        self._sniffing = True
         return self.sniff_thread
 
     def stop_sniffing(self) -> None:
         """\
             Stops the Sniffing thread
         """
-        if not self._sniffing:
-            return None
-
-        self.sniff_thread.stop()
-        self._sniffing = False
+        if self.sniff_thread.alive.is_set():
+            self.sniff_thread.stop()
 
     def config_sniffer(
         self,
         *,
         clean_line: bool = True,
         add_timestamp: bool = True,
     ) -> None:
@@ -230,20 +226,17 @@
         Args:
             log_file (pathlib.Path | str): path to log file.
             mode (Literal['w', 'a'], optional): like open(). Defaults to 'a'.
         """
         self.config_serial_log_file(log_file, mode)
         try:
             self.serial.start_sniffing()
-            self.serial._sniffing = True
             yield
         finally:
-            if self.serial._sniffing:
-                self.serial.stop_sniffing()
-            self.serial._sniffing = False
+            self.serial.stop_sniffing()
 
     def run_serial_cmd(self, cmd: str) -> None:
         """run command on the serial port. adds '\\n' at the end.
 
         Args:
             cmd (str): the command to run
         """
@@ -262,15 +255,15 @@
     ) -> None:
         """config log file for the sniffer.
 
         Args:
             log_file (pathlib.Path | str): path for the log file.
             mode (Literal['w', 'a'], optional): like open(). Defaults to 'a'.
         """
-        if self.serial._sniffing:
+        if self.serial.sniff_thread.alive.is_set():
             self.serial.stop_sniffing()
             assert self.serial.protocol.log_file
             self.serial.protocol.log_file.close()
 
         self.logger.debug(f"configuring log file for serial - {str(log_file)!r}")
         log_file = pathlib.Path(log_file)
         log_file.parent.mkdir(parents=True, exist_ok=True)
@@ -286,15 +279,15 @@
 
         Returns:
             bytes: all data that been read while waiting for the msg.
         """
         self.logger.debug(f"waiting for msg {msg.decode()!r}")
 
         restart_sniffing = False
-        if self.serial._sniffing:
+        if self.serial.sniff_thread.alive.is_set():
             restart_sniffing = True
             self.serial.stop_sniffing()
 
         with self.serial.change_timeout_ctx(timeout):
             if not self.serial.is_open:
                 self.serial.open()
             res = self.serial.read_until(msg)
```

### Comparing `me_setups-1.6.7/src/me_setups/components/eqs.py` & `me_setups-1.6.8/src/me_setups/components/eqs.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.7/src/me_setups/components/mcu.py` & `me_setups-1.6.8/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.7/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.6.8/src/me_setups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.6.7
+Version: 1.6.8
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.7/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.6.8/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

