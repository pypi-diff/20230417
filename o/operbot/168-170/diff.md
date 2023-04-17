# Comparing `tmp/operbot-168.tar.gz` & `tmp/operbot-170.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operbot-168.tar", last modified: Thu Apr 13 21:20:32 2023, max compression
+gzip compressed data, was "operbot-170.tar", last modified: Mon Apr 17 15:53:45 2023, max compression
```

## Comparing `operbot-168.tar` & `operbot-170.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-13 21:20:32.826808 operbot-168/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-13 20:09:14.000000 operbot-168/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.822808 operbot-168/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2528 2023-04-13 20:30:08.000000 operbot-168/bin/operbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)      950 2023-04-13 20:18:15.000000 operbot-168/bin/operbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-13 20:44:02.000000 operbot-168/bin/operbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-13 20:17:12.000000 operbot-168/bin/operbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.822808 operbot-168/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-13 20:41:39.000000 operbot-168/files/operbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/operbot/
--rw-r--r--   0 bart      (1000) bart      (1001)       91 2023-04-13 20:37:44.000000 operbot-168/operbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-13 20:14:50.000000 operbot-168/operbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5943 2023-04-13 20:14:50.000000 operbot-168/operbot/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/operbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 20:14:58.000000 operbot-168/operbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-13 20:14:58.000000 operbot-168/operbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-13 20:22:31.000000 operbot-168/operbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-13 20:22:44.000000 operbot-168/operbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1130 2023-04-13 20:23:05.000000 operbot-168/operbot/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    16376 2023-04-13 21:02:22.000000 operbot-168/operbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      894 2023-04-13 20:23:30.000000 operbot-168/operbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7720 2023-04-13 20:24:16.000000 operbot-168/operbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-13 20:24:29.000000 operbot-168/operbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)      997 2023-04-13 20:24:42.000000 operbot-168/operbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      991 2023-04-13 20:25:06.000000 operbot-168/operbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-13 20:25:19.000000 operbot-168/operbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2632 2023-04-13 20:25:32.000000 operbot-168/operbot/modules/usr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4838 2023-04-13 20:14:50.000000 operbot-168/operbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-13 20:14:50.000000 operbot-168/operbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-13 20:14:50.000000 operbot-168/operbot/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-13 20:14:50.000000 operbot-168/operbot/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-13 20:14:50.000000 operbot-168/operbot/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/operbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      782 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-13 21:20:32.826808 operbot-168/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-13 20:43:46.000000 operbot-168/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-13 20:09:14.000000 operbot-168/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-13 20:09:14.000000 operbot-168/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-13 20:09:14.000000 operbot-168/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-13 20:09:14.000000 operbot-168/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-13 20:09:14.000000 operbot-168/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-17 15:53:45.140474 operbot-170/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-13 20:09:14.000000 operbot-170/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.136474 operbot-170/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2680 2023-04-17 15:49:49.000000 operbot-170/bin/operbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      950 2023-04-13 20:18:15.000000 operbot-170/bin/operbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-13 20:44:02.000000 operbot-170/bin/operbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-13 20:17:12.000000 operbot-170/bin/operbotd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.136474 operbot-170/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-13 20:41:39.000000 operbot-170/files/operbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.136474 operbot-170/operbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)       91 2023-04-13 20:37:44.000000 operbot-170/operbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-13 20:14:50.000000 operbot-170/operbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-16 22:43:23.000000 operbot-170/operbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1713 2023-04-17 15:52:54.000000 operbot-170/operbot/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/operbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 20:14:58.000000 operbot-170/operbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-13 20:14:58.000000 operbot-170/operbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-13 20:22:31.000000 operbot-170/operbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-13 20:22:44.000000 operbot-170/operbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1130 2023-04-13 20:23:05.000000 operbot-170/operbot/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17293 2023-04-17 15:50:03.000000 operbot-170/operbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      894 2023-04-13 20:23:30.000000 operbot-170/operbot/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7720 2023-04-13 20:24:16.000000 operbot-170/operbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-13 20:24:29.000000 operbot-170/operbot/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      997 2023-04-13 20:24:42.000000 operbot-170/operbot/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-16 21:53:04.000000 operbot-170/operbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-13 20:25:19.000000 operbot-170/operbot/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2632 2023-04-13 20:25:32.000000 operbot-170/operbot/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-17 14:44:06.000000 operbot-170/operbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3462 2023-04-17 14:05:02.000000 operbot-170/operbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-14 16:23:57.000000 operbot-170/operbot/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-16 21:54:33.000000 operbot-170/operbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-13 20:14:50.000000 operbot-170/operbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/operbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      801 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-17 15:53:45.140474 operbot-170/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-17 12:23:48.000000 operbot-170/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-13 20:09:14.000000 operbot-170/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-13 20:09:14.000000 operbot-170/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-13 20:09:14.000000 operbot-170/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-13 20:09:14.000000 operbot-170/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-13 20:09:14.000000 operbot-170/test/test_storage.py
```

### Comparing `operbot-168/PKG-INFO` & `operbot-170/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 168
+Version: 170
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-168/README.rst` & `operbot-170/README.rst`

 * *Files identical despite different names*

### Comparing `operbot-168/bin/operbot` & `operbot-170/bin/operbot`

 * *Files 16% similar despite different names*

```diff
@@ -16,26 +16,38 @@
 sys.path.insert(0, os.getcwd())
 
 
 import operbot.modules
 
 
 from operbot.handler import Client, Error, command, parse
+from operbot.loggers import Logging
 from operbot.persist import Persist
 from operbot.scanner import importer, scandir, scanpkg, starter
 from operbot.threads import launch
 
 
-MOD = "cmd,err,irc,rss,sts,thr"
+MOD = "cmd,err,irc,log,rss,sts,thr"
 NAME = "operbot"
 
 
+date = time.ctime(time.time()).replace('  ', ' ')
+
+
 Persist.workdir = os.path.expanduser("~/.%s" % NAME)
 
 
+def cprint(txt):
+    print(txt)
+    sys.stdout.flush()
+
+
+Logging.debug = cprint
+
+
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
     def raw(self, txt):
         print(txt)
@@ -101,22 +113,22 @@
     if cfg.txt:
         cli = CLI()
         command(cli, cfg.otxt)
     elif 'd' in cfg.opts:
         daemon()
         dowait = True
     elif 'c' in cfg.opts:
-        date = time.ctime(time.time()).replace('  ', ' ')
         print(f'{NAME.upper()} started {date}')
-        csl = Console()
-        launch(csl.loop)
         dowait = True
     if dowait:
         scanpkg(operbot.modules, starter, cfg.mod or MOD)
         scandir("modules", starter, cfg.mod or MOD)
+        if "c" in cfg.opts:
+            csl = Console()
+            launch(csl.loop)
         while 1:
             time.sleep(1.0)
             waiter()
 
 
 wrap(main)
 waiter()
```

### Comparing `operbot-168/bin/operbotcmd` & `operbot-170/bin/operbotcmd`

 * *Files identical despite different names*

### Comparing `operbot-168/bin/operbotd` & `operbot-170/bin/operbotd`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/clocked.py` & `operbot-170/operbot/clocked.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/handler.py` & `operbot-170/operbot/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,21 @@
     def byorig(orig):
         for obj in Listens.objs:
             if repr(obj) == orig:
                 return obj
         return None
 
     @staticmethod
+    def remove(bot):
+        try:
+            Listens.objs.remove(bot)
+        except ValueError:
+            pass
+
+    @staticmethod
     def say(orig, txt, channel=None):
         bot = Listens.byorig(orig)
         if bot:
             if channel:
                 bot.say(channel, txt)
             else:
                 bot.raw(txt)
```

### Comparing `operbot-168/operbot/modules/fnd.py` & `operbot-170/operbot/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/modules/irc.py` & `operbot-170/operbot/modules/irc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915
 # pylint: disable=E0402,E0401
 
+
 'internet relay chat'
 
 
 import base64
 import os
 import queue
 import random
@@ -13,16 +14,17 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from ..handler import Client, Command, Error, Event
-from ..objects import Default, Object, keys, prt, update
+from ..handler import Client, Command, Error, Event, Listens
+from ..loggers import Logging
+from ..objects import Default, Object, edit, keys, prt
 from ..persist import last, write
 from ..threads import launch
 
 
 from .usr import Users
 
 
@@ -42,14 +44,15 @@
 
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
+    #irc.joined.wait()
     return irc
 
 
 class Config(Default):
 
     channel = '#%s' % NAME
     control = '!'
@@ -96,14 +99,16 @@
 
     cache = Object()
 
     def __init__(self):
         Object.__init__(self)
         self.oqueue = queue.Queue()
         self.dostop = threading.Event()
+        self.state = Default()
+        self.state.starttime = time.time()
 
     def dosay(self, channel, txt):
         raise NotImplementedError
 
     def extend(self, channel, txtlist):
         if channel not in self.cache:
             setattr(self.cache, channel, [])
@@ -163,14 +168,15 @@
 class IRC(Client, Output):
 
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
+        self.authed = threading.Event()
         self.connected = threading.Event()
         self.channels = []
         self.joined = threading.Event()
         self.keeprunning = False
         self.outqueue = queue.Queue()
         self.sock = None
         self.speed = 'slow'
@@ -179,14 +185,15 @@
         self.state.errors = []
         self.state.last = 0
         self.state.lastline = ''
         self.state.nrconnect = 0
         self.state.nrerror = 0
         self.state.nrsend = 0
         self.state.pongcheck = False
+        self.state.starttime = time.time()
         self.threaded = False
         self.zelf = ''
         self.register('903', self.h903)
         self.register('904', self.h903)
         self.register('AUTHENTICATE', self.auth)
         self.register('CAP', self.cap)
         self.register('ERROR', self.error)
@@ -198,19 +205,18 @@
         self.target = 'type'
 
     def announce(self, txt):
         for channel in self.channels:
             self.say(channel, txt)
 
     def auth(self, event):
-        time.sleep(1.0)
+        assert self.cfg.password
         self.direct('AUTHENTICATE %s' % self.cfg.password)
 
     def cap(self, event):
-        time.sleep(1.0)
         if self.cfg.password and 'ACK' in event.arguments:
             self.direct('AUTHENTICATE PLAIN')
         else:
             self.direct('CAP REQ :sasl')
 
     def command(self, cmd, *args):
         with saylock:
@@ -243,38 +249,51 @@
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
             self.sock.connect((server, port))
             self.command('CAP LS 302')
         else:
             addr = socket.getaddrinfo(server, port, socket.AF_INET)[-1][-1]
             self.sock = socket.create_connection(addr)
+            self.authed.set()
         if self.sock:
             os.set_inheritable(self.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.connected.set()
             return True
         return False
 
     def direct(self, txt):
-        self.sock.send(bytes(txt+'\n', 'utf-8'))
+        Logging.debug(txt)
+        self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
-        self.sock.shutdown(2)
+        try:
+            self.sock.shutdown(2)
+        except (
+                ssl.SSLError,
+                OSError,
+                BrokenPipeError
+               ) as ex:
+            Logging.debug(str(ex))
 
     def docommand(self, evt):
         evt.orig = repr(self)
         Command.handle(evt)
 
     def doconnect(self, server, nck, port=6667):
         while 1:
             try:
                 if self.connect(server, port):
                     break
-            except (ssl.SSLError, OSError, ConnectionResetError) as ex:
+            except (
+                    ssl.SSLError,
+                    OSError,
+                    ConnectionResetError
+                   ) as ex:
                 self.state.errors = str(ex)
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def dosay(self, channel, txt):
         self.joined.wait()
         txt = str(txt).replace('\n', '')
@@ -311,20 +330,20 @@
             self.command('NICK', nck)
         return evt
 
     def fileno(self):
         return self.sock.fileno()
 
     def h903(self, event):
-        time.sleep(1.0)
         self.command('CAP END')
+        self.authed.set()
 
     def h904(self, event):
-        time.sleep(1.0)
         self.command('CAP END')
+        self.authed.set()
 
     def joinall(self):
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
         while 1:
@@ -332,18 +351,22 @@
             self.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 self.state.pongcheck = False
                 self.keeprunning = False
-                self.reconnect()
-
+                self.connected.clear()
+                self.stop()
+                start()
+                break
 
     def logon(self, server, nck):
+        self.connected.wait()
+        self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
                  'USER %s %s %s :%s' % (self.cfg.username or NAME,
                  server,
                  server,
                  self.cfg.realname or NAME)
                 )
@@ -414,28 +437,35 @@
             obj.txt = arguments[1]
         spl = obj.txt.split()
         if len(spl) > 1:
             obj.args = spl[1:]
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
+        Logging.debug(rawstr)
         return obj
 
     def poll(self):
         self.connected.wait()
         if not self.buffer:
             try:
                 self.some()
-            except (ssl.SSLError, socket.timeout, ConnectionResetError) as ex:
-                self.joined.clear()
-                time.sleep(5.0)
-                evt = Event()
-                evt.txt = str(ex)
-                evt.orig = repr(self)
-                return evt
+            except BlockingIOError as ex:
+                time.sleep(1.0)
+                return self.event(str(ex))
+            except (
+                    socket.timeout,
+                    ssl.SSLError,
+                    ssl.SSLZeroReturnError,
+                    ConnectionResetError,
+                    BrokenPipeError
+                   ) as ex:
+                Error.errors.append(ex)
+                self.stop()
+                return self.event(str(ex))
         return self.event(self.buffer.pop(0))
 
     def privmsg(self, event):
         if event.txt:
             if event.txt[0] in [self.cfg.control, '!']:
                 event.txt = event.txt[1:]
             elif event.txt.startswith('%s:' % self.cfg.nick):
@@ -451,28 +481,29 @@
 
     def quit(self, event):
         if event.orig and event.orig in self.zelf:
             self.stop()
 
     def raw(self, txt):
         txt = txt.rstrip()
+        Logging.debug(txt)
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
                     ssl.SSLError,
+                    ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                time.sleep(5.0)
                 Error.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
@@ -515,33 +546,32 @@
                self.cfg.nick or NAME,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        try:
-            self.sock.shutdown(2)
-        except(ssl.SSLError,  OSError):
-            pass
+        Logging.debug("stopping")
+        Listens.remove(self)
         Client.stop(self)
         Output.stop(self)
+        self.disconnect()
 
 
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(prt(
                         config,
                         keys(config),
                         skip='control,password,realname,sleep,username')
                        )
     else:
-        update(config, event.sets)
+        edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
```

### Comparing `operbot-168/operbot/modules/log.py` & `operbot-170/operbot/modules/log.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/modules/rss.py` & `operbot-170/operbot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/modules/tdo.py` & `operbot-170/operbot/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/modules/thr.py` & `operbot-170/operbot/modules/thr.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
             uptime = obj.sleep - int(time.time() - obj.state.latest)
+        elif getattr(obj, 'starttime', None):
+            uptime = int(time.time() - obj.starttime)
         else:
             uptime = int(time.time() - starttime)
         result.append((uptime, thread.name))
     res = []
     for uptime, txt in sorted(result, key=lambda x: x[0]):
         res.append('%s/%s' % (txt, elapsed(uptime)))
     if res:
```

### Comparing `operbot-168/operbot/modules/usr.py` & `operbot-170/operbot/modules/usr.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/objects.py` & `operbot-170/operbot/objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 def __dir__():
     return (
             'Default',
             'Object',
             'dumps',
+            'edit',
             'items',
             'keys',
             'kind',
             'loads',
             'prt',
             'search',
             'update',
@@ -62,14 +63,45 @@
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
+def edit(obj, setter, skip=False):
+    try:
+        setter = vars(setter)
+    except (TypeError, ValueError):
+        pass
+    if not setter:
+        setter = {}
+    count = 0
+    for key, val in setter.items():
+        if skip and val == "":
+            continue
+        count += 1
+        try:
+            setattr(obj, key, int(val))
+            continue
+        except ValueError:
+            pass
+        try:
+            setattr(obj, key, float(val))
+            continue
+        except ValueError:
+            pass
+        if val in ["True", "true"]:
+            setattr(obj, key, True)
+        elif val in ["False", "false"]:
+            setattr(obj, key, False)
+        else:
+            setattr(obj, key, val)
+    return count
+
+
 def ident(obj):
     return os.path.join(
                         kind(obj),
                         str(uuid.uuid4().hex),
                         os.sep.join(str(datetime.datetime.now()).split()),
                        )
```

### Comparing `operbot-168/operbot/persist.py` & `operbot-170/operbot/persist.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,19 @@
 
 
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
 
-    workdir = os.path.expanduser("~/.opr")
+    workdir = ""
+
+    @staticmethod
+    def logdir():
+        return os.path.join(Persist.workdir, "logs")
 
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
         pth = os.path.dirname(pth)
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
@@ -99,14 +103,19 @@
     Persist.workdir = pth
 
 
 def strip(pth) -> str:
     return os.sep.join(pth.split(os.sep)[-4:])
 
 
+def touch(fname):
+    fds = os.open(fname, os.O_WRONLY | os.O_CREAT)
+    os.close(fds)
+
+
 def write(obj) -> str:
     pth = path(obj.__oid__)
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
```

### Comparing `operbot-168/operbot/scanner.py` & `operbot-170/operbot/scanner.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot/threads.py` & `operbot-170/operbot/threads.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pylint: disable=C0115,C0116,W0613,E0402
 
 
 'threads'
 
 
 import queue
+import time
 import types
 
 
 from functools import wraps
 from threading import Thread as BasicThread
 
 
@@ -29,14 +30,15 @@
     def __init__(self, func, thrname, *args, daemon=True):
         super().__init__(None, self.run, thrname, (), {}, daemon=daemon)
         self._result = None
         self.name = thrname or name(func)
         self.queue = queue.Queue()
         self.queue.put_nowait((func, args))
         self.sleep = None
+        self.starttime = time.time()
 
     def __iter__(self):
         return self
 
     def __next__(self):
         for k in dir(self):
             yield k
```

### Comparing `operbot-168/operbot/utility.py` & `operbot-170/operbot/utility.py`

 * *Files identical despite different names*

### Comparing `operbot-168/operbot.egg-info/PKG-INFO` & `operbot-170/operbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 168
+Version: 170
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-168/operbot.egg-info/SOURCES.txt` & `operbot-170/operbot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 bin/operbotcmd
 bin/operbotctl
 bin/operbotd
 files/operbot.service
 operbot/__init__.py
 operbot/clocked.py
 operbot/handler.py
+operbot/loggers.py
 operbot/objects.py
 operbot/persist.py
 operbot/scanner.py
 operbot/threads.py
 operbot/utility.py
 operbot.egg-info/PKG-INFO
 operbot.egg-info/SOURCES.txt
```

### Comparing `operbot-168/setup.py` & `operbot-170/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="operbot",
-    version="168",
+    version="170",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/operbot",
     description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `operbot-168/test/test_decoder.py` & `operbot-170/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `operbot-168/test/test_inherit.py` & `operbot-170/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `operbot-168/test/test_objects.py` & `operbot-170/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `operbot-168/test/test_storage.py` & `operbot-170/test/test_storage.py`

 * *Files identical despite different names*

