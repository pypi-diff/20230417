# Comparing `tmp/kenu-1.3.4.tar.gz` & `tmp/kenu-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.3.4.tar", last modified: Sun Apr 16 16:25:55 2023, max compression
+gzip compressed data, was "kenu-1.3.5.tar", last modified: Mon Apr 17 08:19:04 2023, max compression
```

## Comparing `kenu-1.3.4.tar` & `kenu-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:25:55.805057 kenu-1.3.4/
--rw-rw-rw-   0        0        0      122 2023-04-16 16:25:55.803063 kenu-1.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:25:55.761208 kenu-1.3.4/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.3.4/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.3.4/kenu/__main__.py
--rw-rw-rw-   0        0        0     3798 2023-04-16 16:25:44.000000 kenu-1.3.4/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:25:55.799073 kenu-1.3.4/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 16:25:55.806055 kenu-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-04-16 16:25:51.000000 kenu-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:19:04.251349 kenu-1.3.5/
+-rw-rw-rw-   0        0        0      122 2023-04-17 08:19:04.249357 kenu-1.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 08:19:04.183532 kenu-1.3.5/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.3.5/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.3.5/kenu/__main__.py
+-rw-rw-rw-   0        0        0     4138 2023-04-17 08:18:28.000000 kenu-1.3.5/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:19:04.245372 kenu-1.3.5/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-17 08:19:03.000000 kenu-1.3.5/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-17 08:19:03.000000 kenu-1.3.5/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:19:03.000000 kenu-1.3.5/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-17 08:19:03.000000 kenu-1.3.5/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-17 08:19:03.000000 kenu-1.3.5/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-17 08:19:03.000000 kenu-1.3.5/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:19:04.251349 kenu-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-04-17 08:11:44.000000 kenu-1.3.5/setup.py
```

### Comparing `kenu-1.3.4/kenu/__init__.py` & `kenu-1.3.5/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.3.4/kenu/__main__.py` & `kenu-1.3.5/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.3.4/kenu/connect.py` & `kenu-1.3.5/kenu/connect.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 def main():
     arg = sys.argv[1]
     global PORT
     PORT = 5050
     if(arg == "kenu-1"):
         HOST = "20.238.119.193"
         connectserver(arg, HOST)
+    elif(arg == "kenu-2"):
+        HOST = "20.250.2.200"
+        connectserver(arg, HOST)
     else:
         print("This server is invalid.")
         exit()
     
-    
     try:
         client_id = '1085214791771111485'
         global RPC
         RPC = pypresence.Presence(client_id)
         RPC.connect()
     except Exception as e:
         pass
@@ -103,15 +105,21 @@
         signin()
         if login() == False:
             print("Try again. \n")
             signin()
         receive_thread = threading.Thread(target=handle_receive)
         receive_thread.start()
     except Exception as e:
-        print("The server did not respond.",e)
+        HOST = "20.250.2.200"
+        if(server != HOST):
+            print("The kenu-1 server is offline due to an unknown reason. We are transferring you to the kenu-2 server.")
+            connectserver(HOST)
+        else:
+            print("The server did not respond.")
+        
         time.sleep(2)
         sys.exit()
 
     while True:
         try:
             message = input()
             client.send(message.encode())
@@ -121,15 +129,15 @@
             sys.exit()
         except:
             client.close()
             sys.exit()
 
     
 
-def connectserver(servername, server):
+def connectserver(server, servername ="kenu-1"):
     print("Connecting to the server. - " + servername)
     connectserverld()
     start_client(server)
 
 @loadwave.process
 def connectserverld():
     time.sleep(3.5)
```

