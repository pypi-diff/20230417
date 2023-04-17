# Comparing `tmp/interlinking-0.0.3.tar.gz` & `tmp/interlinking-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interlinking-0.0.3.tar", last modified: Sat Apr 15 11:14:09 2023, max compression
+gzip compressed data, was "interlinking-0.0.4.tar", last modified: Mon Apr 17 18:13:04 2023, max compression
```

## Comparing `interlinking-0.0.3.tar` & `interlinking-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:14:09.640031 interlinking-0.0.3/
--rw-rw-rw-   0        0        0      706 2023-04-15 11:14:09.639019 interlinking-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 11:14:09.622018 interlinking-0.0.3/interlinking/
--rw-rw-rw-   0        0        0       66 2023-04-15 11:10:19.000000 interlinking-0.0.3/interlinking/__init__.py
--rw-rw-rw-   0        0        0     7964 2023-04-15 10:20:31.000000 interlinking-0.0.3/interlinking/interlinking.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:14:09.635865 interlinking-0.0.3/interlinking.egg-info/
--rw-rw-rw-   0        0        0      706 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 11:14:09.641033 interlinking-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-04-15 11:13:02.000000 interlinking-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:13:04.307530 interlinking-0.0.4/
+-rw-rw-rw-   0        0        0     1805 2023-04-17 18:13:04.306019 interlinking-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-04-17 18:10:06.000000 interlinking-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 18:13:04.289945 interlinking-0.0.4/interlinking/
+-rw-rw-rw-   0        0        0       66 2023-04-15 11:10:19.000000 interlinking-0.0.4/interlinking/__init__.py
+-rw-rw-rw-   0        0        0     9812 2023-04-17 18:12:42.000000 interlinking-0.0.4/interlinking/interlinking.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:13:04.303024 interlinking-0.0.4/interlinking.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-04-17 18:13:04.000000 interlinking-0.0.4/interlinking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-17 18:13:04.000000 interlinking-0.0.4/interlinking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:13:04.000000 interlinking-0.0.4/interlinking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-17 18:13:04.000000 interlinking-0.0.4/interlinking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 18:13:04.000000 interlinking-0.0.4/interlinking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 18:13:04.307530 interlinking-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-04-17 18:12:01.000000 interlinking-0.0.4/setup.py
```

### Comparing `interlinking-0.0.3/interlinking/interlinking.py` & `interlinking-0.0.4/interlinking/interlinking.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,159 +5,178 @@
 import time
 import threading
 
 class Server:
     def __init__(self,output=True, port=5000,format="ascii",host=socket.gethostbyname(socket.gethostname())):
         super(Server, self).__init__()
         self.connections = []
+        self.check = []
         self.format = format
         self.host = host
         self.port = port
         self.output = output
-        self.running = True
+        self.recived = False
+        self.recived_data = False
+        self.threads = []
         self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.server.bind((self.host, self.port))
         self.conn,self.addr = None, None
+        self.data = None
+        self.using = False
+        self.shutdown = False
         def check():
             while True:
-                for x in self.connections:
-                    data = x[0].recv(1024)
-                    if data == b"":
-                        self.connections.remove(list([x[0],x[1],x[2]]))
-                time.sleep(1)
-    
-        def x():
+                try:
+                    if self.shutdown:
+                        break
+                    if not self.using:
+                        for x in self.connections:
+                            data = x[0].recv(1024)
+                            if data == b"":
+                                self.connections.remove(list([x[0],x[1],x[2]]))
+                        time.sleep(1)
+                except:
+                    break
+        
+        def connect():
             while True:
-                self.server.listen()
-                self.conn, self.addr = self.server.accept()
-                message = ""
-                while not message.startswith("$"):
-                    message = self.conn.recv(1024).decode(self.format)
-                if message.split("$")[2] != "!AUTHORIZE":
-                    self.conn.shutdown(socket.SHUT_RDWR)
-                    self.conn.close()
-                    continue
-                self.connections.append(list([self.conn, self.addr, message.split("$")[1]]))
+                if self.shutdown:
+                    break
+                try:
+                    self.server.listen()
+                    self.conn, self.addr = self.server.accept()
+                    message = ""
+                    while not message.startswith("$"):
+                        message = self.conn.recv(1024).decode(self.format)
+                    if message.split("$")[2] != "!AUTHORIZE":
+                        self.conn.shutdown(socket.SHUT_RDWR)
+                        self.conn.close()
+                        continue
+                    self.connections.append(list([self.conn, self.addr, message.split("$")[1]]))
+                except:
+                    break
                 
-        t = threading.Thread(target=x)
+        t = threading.Thread(target=connect)
         t.start()
         t2 = threading.Thread(target=check)
         t2.start()
-        self.messages = []
+        self.threads.append(t)
+        self.threads.append(t2)
         return
-    def recive_msg(self):
-        def recive(conn, addr):
-            message = ""
-            while message == "":
-                try:
-                    message = conn.recv(1024).decode(self.format)
-                except ConnectionResetError:
-                    for x in self.connections:
-                        try:
-                            x.find(conn)
-                            self.connections.remove(list([conn, addr, x[2]]))
-                            break 
-                        except:
-                            continue
-            final_msg = message
-            message = message.split("$")
-            check_message = message
-            message = message[2]
-            if "!USER" in message:
-                message, user = message.split("!USER")
-                for clients in self.connections:
-                    if clients[2] == user.strip():
-                        try:
-                            clients[0].sendall(final_msg.encode(self.format))
-                            break
-                        except:
+    def start_server(self):
+        def reciving(conn, addr):
+            while True:
+                if self.shutdown:
+                    break
+                message = ""
+                while message == "":
+                    try:
+                        message = conn.recv(1024).decode(self.format)
+                    except ConnectionResetError:
+                        for x in self.connections:
                             try:
-                                self.connections.remove(list([conn, addr, check_message[1]])) 
-                                continue
+                                x.find(conn)
+                                self.connections.remove(list([conn, addr, x[2]]))
+                                break 
                             except:
                                 continue
-                return
-            if self.output == True:
-                print(f"[CLIENT] {addr[0]} -- {message}")
-            self.messages.append(message)
-        self.check = []
-        while True:
-            if len(self.connections) > 0:
-                for i in range(len(self.connections)):
+                    except:
+                        break
+                if message == "!FILE":
+                    self.using = True
+                    self.recived = False
+                    file_name = conn.recv(1024).decode(self.format)
+                    file_size = conn.recv(1024).decode(self.format)
+                    file = open(file_name, "wb")
+                    file_bytes = b""
+                    done = False
+                    progress = tqdm.tqdm(unit="B", unit_scale=True, unit_divisor=1000,total=int(file_size))
+                    while not done:
+                        data = conn.recv(1024)
+                        if data[-5:] == b"<END>":
+                            file_bytes += data
+                            done = True
+                        else:
+                            file_bytes += data
+                        progress.update(1024)
+                    file.write(file_bytes.split(b"<END>")[0])
+                    file.close()
+                    self.recived = True
+                    conn.sendall("!RECIVED".encode(self.format))
+                elif message == "!DATA":
+                    self.recived_data = False
+                    data = conn.recv(1024)
                     try:
-                        if list([self.connections[i][0], self.connections[i][1]]) not in self.check:
-                            t = threading.Thread(target=recive, args=(self.connections[i][0], self.connections[i][1],))
-                            t.start()
-                            self.check.append(list([self.connections[i][0], self.connections[i][1]]))
-                    except IndexError:
-                        continue
+                        self.data = pickle.loads(data)
+                        self.recived_data = True
+                    except AttributeError:
+                        print("[ERROR] -- bad data --")
+                else:
+                    try:
+                        final_msg = message
+                        message = message.split("$")
+                        check_message = message
+                        message = message[2]
+                        cont = True
+                    except:
+                        break
+                    if "!USER" in message:
+                        cont = False
+                        message, user = message.split("!USER")
+                        for clients in self.connections:
+                            if clients[2] == user.strip():
+                                try:
+                                    clients[0].sendall(final_msg.encode(self.format))
+                                    break
+                                except:
+                                    try:
+                                        self.connections.remove(list([conn, addr, check_message[1]])) 
+                                        continue
+                                    except:
+                                        continue
+                    if self.output == True and cont == True:
+                        print(f"[CLIENT] {addr[0]} -- {message}")
+        def checking():
+            while True:
+                if self.shutdown:
+                    break
+                if len(self.connections) > 0:
+                    for i in range(len(self.connections)):
+                        try:
+                            if list([self.connections[i][0], self.connections[i][1]]) not in self.check:
+                                t = threading.Thread(target=reciving, args=(self.connections[i][0], self.connections[i][1],))
+                                t.start()
+                                self.threads.append(t)
+                                self.check.append(list([self.connections[i][0], self.connections[i][1]]))
+                        except IndexError:
+                            continue
+        t3 = threading.Thread(target=checking)
+        t3.start()
+        self.threads.append(t3)
     def stop_server(self):
-        self.running == False
-        self.server.shutdown(socket.SHUT_RDWR)
+        self.shutdown = True
         self.server.close()
-        return
-    def recive_file(self, name=None):
-        check = False
-        for x in self.connections:
-            if x[2] == name.strip():
-                check = True
-                conn, addr = x[0], x[1]
-            if name == None:
-                break
-        if check == False:
-            while self.conn == None and self.addr == None:
-                conn, addr = self.conn, self.addr
-        self.recived = False
-        file_name = conn.recv(1024).decode(self.format)
-        file_name = conn.recv(1024).decode(self.format)
-        file_size = conn.recv(1024).decode(self.format)
-        file = open(file_name, "wb")
-        file_bytes = b""
-        done = False
-        progress = tqdm.tqdm(unit="B", unit_scale=True, unit_divisor=1000,total=int(file_size))
-        while not done:
-            data = conn.recv(1024)
-            if file_bytes[-5:] == b"<END>":
-                done = True
-            else:
-                file_bytes += data
-            progress.update(1024)
-        file_bytes = file_bytes.split(b"<END>")[0]
-        file.write(file_bytes)
-        file.close()
-        self.recived = True
-    def recive_data(self, name=None):
-        check = False
         for x in self.connections:
-            if x[2] == name.strip():
-                check = True
-                conn, addr = x[0], x[1]
-            if name == None:
-                break
-        if check == False:
-            while self.conn == None and self.addr == None:
-                conn, addr = self.conn, self.addr
-        data = conn.recv(1024)
-        try:
-            data = pickle.loads(data)
-            return data
-        except AttributeError:
-            print("[SERVER] -- use brackets -- ")
-            return "ERROR"
+                x[0].sendall("!SHUTDOWN".encode(self.format))
+                x[0].shutdown(socket.SHUT_RDWR)
+                x[0].close()
+        for x in self.threads:
+            x.join()
 
         
 class Client:
     def __init__(self,name,output=True, recive=True,host=socket.gethostbyname(socket.gethostname()), port=5000, format="ascii"):
         super(Client, self).__init__()
         self.host = host
         self.name = name
         self.port = port
         self.format = format
         self.output = output
         self.recive = recive
+        self.recived = False
         self.client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.connected = True
         self.client.connect((self.host, self.port))
         def x():
             self.client.send(f"${self.name}$!AUTHORIZE".encode(self.format))
         t = threading.Thread(target=x)
         t.start()
@@ -169,16 +188,25 @@
             while self.recive:
                 try:
                     message = self.client.recv(1024).decode(self.format)
                 except:
                     break
                 if message == "":
                     message = self.client.recv(1024).decode(self.format)
+                if message == "!RECIVED":
+                    self.recived = True
+                    continue
+                if message == "!SHUTDOWN":
+                    self.recived = True
+                    break
                 msg = message.split("$")
-                m = msg[2].split("!USER")[0]
+                try:
+                    m = msg[2].split("!USER")[0]
+                except:
+                    break
                 if self.output:
                     print(f"{msg[1]} > {m}")
                 self.mess = f"{msg[1]} > {msg[2]}"
         
         t = threading.Thread(target=recive_msg)
         t.start()
         
@@ -186,24 +214,33 @@
         self.recive = False
         self.client.shutdown(socket.SHUT_RDWR)
         self.client.close()
     def send_msg(self, message):
         message = f"${self.name}${message}"
         self.client.send(message.encode(self.format))
     def send_file(self, filename, send_filename=None):
+        self.recived = False
         if send_filename == None:
             send_filename = filename
         try:
             file = open(filename, "rb")
             file_size = os.path.getsize(filename)
         except:
             print("[SERVER] -- filename doesnt exist -- ")
+        self.client.send("!FILE".encode(self.format))
+        time.sleep(1)
         self.client.send(send_filename.encode(self.format))
         self.client.send(str(file_size).encode (self.format))
         data = file.read()
         self.client.sendall(data)
         self.client.send(b"<END>")
         file.close()
+        while self.recived != True:
+            continue
     def send_data(self, data):
+        self.recived = False
+        self.client.send("!DATA".encode(self.format))
         data = pickle.dumps(data)
         self.client.send(data)
+        while self.recived != True:
+            continue
```

### Comparing `interlinking-0.0.3/setup.py` & `interlinking-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from setuptools import setup, find_packages
+import os
+import codecs
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Send messages, files or raw data between python codes(servers, computers, ...).'
 LONG_DESCRIPTION = 'A package that allows to build simple server with listening and handling all data.'
 
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
 # Setting up
 setup(
     name="interlinking",
     version=VERSION,
     author="AdioSs (Daniel Karlík)",
     author_email="<karlik.dan@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
+    long_description=long_description,
     packages=find_packages(),
     install_requires=['tqdm'],
     keywords=['python', 'server', 'client', 'data sending', 'servers communication', 'sockets'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

