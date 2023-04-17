# Comparing `tmp/tkblock-1.1.0.tar.gz` & `tmp/tkblock-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkblock-1.1.0.tar", last modified: Mon Apr 17 10:49:37 2023, max compression
+gzip compressed data, was "tkblock-1.1.1.tar", last modified: Mon Apr 17 10:54:53 2023, max compression
```

## Comparing `tkblock-1.1.0.tar` & `tkblock-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:49:37.648985 tkblock-1.1.0/
--rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    14133 2023-04-17 10:49:37.647988 tkblock-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    13433 2023-04-17 09:10:12.000000 tkblock-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 10:49:37.649983 tkblock-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-04-17 10:49:30.000000 tkblock-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:49:37.618079 tkblock-1.1.0/tkblock/
--rw-rw-rw-   0        0        0      225 2023-03-14 16:09:02.000000 tkblock-1.1.0/tkblock/__init__.py
--rw-rw-rw-   0        0        0      488 2023-03-17 02:44:56.000000 tkblock-1.1.0/tkblock/block_framebase.py
--rw-rw-rw-   0        0        0    21260 2023-04-17 10:11:19.000000 tkblock-1.1.0/tkblock/block_framework.py
--rw-rw-rw-   0        0        0     6263 2023-04-17 10:43:14.000000 tkblock-1.1.0/tkblock/block_service.py
--rw-rw-rw-   0        0        0      426 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/block_util.py
--rw-rw-rw-   0        0        0     1418 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/canvas.py
--rw-rw-rw-   0        0        0      494 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/layout.py
--rw-rw-rw-   0        0        0      368 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/scrollbar.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:49:37.644995 tkblock-1.1.0/tkblock.egg-info/
--rw-rw-rw-   0        0        0    14133 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:53.379711 tkblock-1.1.1/
+-rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    13947 2023-04-17 10:54:53.378713 tkblock-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13251 2023-04-17 10:53:59.000000 tkblock-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:54:53.380709 tkblock-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-04-17 10:54:50.000000 tkblock-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:53.349791 tkblock-1.1.1/tkblock/
+-rw-rw-rw-   0        0        0      225 2023-03-14 16:09:02.000000 tkblock-1.1.1/tkblock/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-03-17 02:44:56.000000 tkblock-1.1.1/tkblock/block_framebase.py
+-rw-rw-rw-   0        0        0    21260 2023-04-17 10:11:19.000000 tkblock-1.1.1/tkblock/block_framework.py
+-rw-rw-rw-   0        0        0     6263 2023-04-17 10:43:14.000000 tkblock-1.1.1/tkblock/block_service.py
+-rw-rw-rw-   0        0        0      426 2023-03-16 16:16:54.000000 tkblock-1.1.1/tkblock/block_util.py
+-rw-rw-rw-   0        0        0     1418 2023-03-16 16:16:54.000000 tkblock-1.1.1/tkblock/canvas.py
+-rw-rw-rw-   0        0        0      494 2023-03-16 16:16:54.000000 tkblock-1.1.1/tkblock/layout.py
+-rw-rw-rw-   0        0        0      368 2023-03-16 16:16:54.000000 tkblock-1.1.1/tkblock/scrollbar.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:53.375724 tkblock-1.1.1/tkblock.egg-info/
+-rw-rw-rw-   0        0        0    13947 2023-04-17 10:54:53.000000 tkblock-1.1.1/tkblock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-17 10:54:53.000000 tkblock-1.1.1/tkblock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:54:53.000000 tkblock-1.1.1/tkblock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:54:53.000000 tkblock-1.1.1/tkblock.egg-info/top_level.txt
```

### Comparing `tkblock-1.1.0/LICENSE` & `tkblock-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkblock-1.1.0/PKG-INFO` & `tkblock-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 1.1.0
+Version: 1.1.1
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -286,18 +286,14 @@
 frame = BlockService.create_frame("test_scrollbar")
 listbox_list = tuple([str(x) for x in range(0, 100)] + ["aabfsdgadfsgasdfkj;adsfadsj;kjfeijof"])
 listbox_var = tk.StringVar(value=listbox_list)
 listbox = tk.Listbox(frame, listvariable=listbox_var)
 listbox.layout = BlockService.layout(1, 2, 1, 4)
 scrollbar_y = tk.Scrollbar(frame, orient=tk.VERTICAL)
 scrollbar_x = tk.Scrollbar(frame, orient=tk.HORIZONTAL)
-scrollbar_y.config(command=listbox.yview)
-scrollbar_x.config(command=listbox.xview)
-listbox.config(yscrollcommand=scrollbar_y.set)
-listbox.config(xscrollcommand=scrollbar_x.set)
 listbox.scrollbar = BlockService.scrollbar(y=scrollbar_y, x=scrollbar_x, size=30)
 BlockService.place_frame_widget()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.
```

### Comparing `tkblock-1.1.0/README.md` & `tkblock-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -272,18 +272,14 @@
 frame = BlockService.create_frame("test_scrollbar")
 listbox_list = tuple([str(x) for x in range(0, 100)] + ["aabfsdgadfsgasdfkj;adsfadsj;kjfeijof"])
 listbox_var = tk.StringVar(value=listbox_list)
 listbox = tk.Listbox(frame, listvariable=listbox_var)
 listbox.layout = BlockService.layout(1, 2, 1, 4)
 scrollbar_y = tk.Scrollbar(frame, orient=tk.VERTICAL)
 scrollbar_x = tk.Scrollbar(frame, orient=tk.HORIZONTAL)
-scrollbar_y.config(command=listbox.yview)
-scrollbar_x.config(command=listbox.xview)
-listbox.config(yscrollcommand=scrollbar_y.set)
-listbox.config(xscrollcommand=scrollbar_x.set)
 listbox.scrollbar = BlockService.scrollbar(y=scrollbar_y, x=scrollbar_x, size=30)
 BlockService.place_frame_widget()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.
```

### Comparing `tkblock-1.1.0/setup.py` & `tkblock-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 # README.mdをlong_discriptionにするために読み込む
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version="1.1.0",
+    version="1.1.1",
     description="tkinter block framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kuri-pome/tkblock",
     author="kuri_pome",
     license="MIT",
     keywords="tkinter place widget easy",
```

### Comparing `tkblock-1.1.0/tkblock/block_framework.py` & `tkblock-1.1.1/tkblock/block_framework.py`

 * *Files identical despite different names*

### Comparing `tkblock-1.1.0/tkblock/block_service.py` & `tkblock-1.1.1/tkblock/block_service.py`

 * *Files identical despite different names*

### Comparing `tkblock-1.1.0/tkblock/canvas.py` & `tkblock-1.1.1/tkblock/canvas.py`

 * *Files identical despite different names*

### Comparing `tkblock-1.1.0/tkblock.egg-info/PKG-INFO` & `tkblock-1.1.1/tkblock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 1.1.0
+Version: 1.1.1
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -286,18 +286,14 @@
 frame = BlockService.create_frame("test_scrollbar")
 listbox_list = tuple([str(x) for x in range(0, 100)] + ["aabfsdgadfsgasdfkj;adsfadsj;kjfeijof"])
 listbox_var = tk.StringVar(value=listbox_list)
 listbox = tk.Listbox(frame, listvariable=listbox_var)
 listbox.layout = BlockService.layout(1, 2, 1, 4)
 scrollbar_y = tk.Scrollbar(frame, orient=tk.VERTICAL)
 scrollbar_x = tk.Scrollbar(frame, orient=tk.HORIZONTAL)
-scrollbar_y.config(command=listbox.yview)
-scrollbar_x.config(command=listbox.xview)
-listbox.config(yscrollcommand=scrollbar_y.set)
-listbox.config(xscrollcommand=scrollbar_x.set)
 listbox.scrollbar = BlockService.scrollbar(y=scrollbar_y, x=scrollbar_x, size=30)
 BlockService.place_frame_widget()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.
```

