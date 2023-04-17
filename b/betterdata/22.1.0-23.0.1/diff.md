# Comparing `tmp/betterdata-22.1.0.tar.gz` & `tmp/betterdata-23.0.1.tar.gz`

## Comparing `betterdata-22.1.0.tar` & `betterdata-23.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 betterdata-22.1.0/build.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 betterdata-22.1.0/changelog.md
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 betterdata-22.1.0/start.sh
--rwxr-xr-x   0        0        0     4517 2020-02-02 00:00:00.000000 betterdata-22.1.0/betterdata/__init__.py
--rw-r--r--   0        0        0   153907 2020-02-02 00:00:00.000000 betterdata-22.1.0/img/filled.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 betterdata-22.1.0/img/filled.svg
--rw-r--r--   0        0        0    59577 2020-02-02 00:00:00.000000 betterdata-22.1.0/img/transparent.png
--rwxr-xr-x   0        0        0     3969 2020-02-02 00:00:00.000000 betterdata-22.1.0/img/transparent.svg
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 betterdata-22.1.0/.gitignore
--rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 betterdata-22.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     3760 2020-02-02 00:00:00.000000 betterdata-22.1.0/readme.md
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 betterdata-22.1.0/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 betterdata-23.0.1/build.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 betterdata-23.0.1/changelog.md
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 betterdata-23.0.1/start.sh
+-rwxr-xr-x   0        0        0     4409 2020-02-02 00:00:00.000000 betterdata-23.0.1/betterdata/__init__.py
+-rw-r--r--   0        0        0   153907 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/filled.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/filled.svg
+-rw-r--r--   0        0        0    59577 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/transparent.png
+-rwxr-xr-x   0        0        0     3969 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/transparent.svg
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 betterdata-23.0.1/.gitignore
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 betterdata-23.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0     3760 2020-02-02 00:00:00.000000 betterdata-23.0.1/readme.md
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 betterdata-23.0.1/PKG-INFO
```

### Comparing `betterdata-22.1.0/betterdata/__init__.py` & `betterdata-23.0.1/betterdata/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,52 +28,52 @@
 
 pretty.install()
 traceback.install(
     show_locals=True
 )
 c = rich.console.Console()
 print = c.print
-version = '22.1.0'
+version = '23.0.0'
 
 
 class Data:
     # pylint: disable=no-member
     '''
     @DynamicAttrs
     '''
     def __init__(
         self,
         data: dict = {},
-        file_path: str | Path = None,
+        path: str | Path | None = None,
     ) -> None:
         self.data = {}
-        self.file_path = None
+        self.path = None
         self.set_data(
             data = data,
-            file_path = file_path,
+            path = path,
         )
         if (
             not self.data
         ) and (
-            self.file_path
+            self.path
         ) and (
-            self.file_path.exists()
+            self.path.exists()
         ):
             self.read_file()
 
     def __repr__(self) -> dict:
         return self.data
 
     def __str__(self) -> str:
         return str(self.data)
 
     def __getitem__(
         self,
         item,
-    ) -> any:
+    ):
         if item in self.data:
             return self.data[item]
         else:
             return None
 
     def __setitem__(
         self,
@@ -94,29 +94,29 @@
         self,
         item,
     ) -> bool:
         return item in self.data
 
     def set_data(
         self,
-        data: dict = None,
-        file_path = None
+        data: dict | None = None,
+        path = None
     ):
         if not data:
             data = {}
         if not isinstance(
             data,
             dict,
         ):
             raise TypeError(
                 f'expected dict but {type(data)} got'
             )
 
-        if file_path:
-            self.file_path = Path(file_path)
+        if path:
+            self.path = Path(path)
         if data:
             self.data = data
             for key, val in data.items():
                 vars(self)[key] = val
             self.to_file()
 
     def to_str(
@@ -124,36 +124,36 @@
     ):
         return yml.to_str(
             data = self.data
         )
 
     def read_file(
         self,
-        file_path = None,
+        path = None,
     ):
         self.set_data(
-            file_path = file_path,
+            path = path,
         )
         self.set_data(
             data = yml.read_file(
-                file_path = self.file_path
+                path = self.path
             )
         )
 
     def to_file(
         self,
-        file_path = None
+        path = None
     ):
         self.set_data(
-            file_path = file_path
+            path = path
         )
-        if self.file_path and self.data:
+        if self.path and self.data:
             yml.to_file(
                 data = self.data,
-                file_path = self.file_path,
+                path = self.path,
             )
 
     def interactive_input(
         self,
         item: str,
         digits_to_int: bool = True,
         skip_if_exist: bool = True,
@@ -189,17 +189,17 @@
                         else:
                             return
                     case 'yes':
                         pass
             if digits_to_int and val.isdigit():
                 val = int(val)
             self[item] = val
-            if self.file_path:
+            if self.path:
                 self.to_file()
-                print(f'[green]{item} saved to config:\n[deep_sky_blue1]{self.file_path}')
+                print(f'[green]{item} saved to config:\n[deep_sky_blue1]{self.path}')
             return
 
     def print(
         self
     ):
         c.print(
             self.data
```

### Comparing `betterdata-22.1.0/img/filled.png` & `betterdata-23.0.1/img/filled.png`

 * *Files identical despite different names*

### Comparing `betterdata-22.1.0/img/filled.svg` & `betterdata-23.0.1/img/filled.svg`

 * *Files identical despite different names*

### Comparing `betterdata-22.1.0/img/transparent.png` & `betterdata-23.0.1/img/transparent.png`

 * *Files identical despite different names*

### Comparing `betterdata-22.1.0/img/transparent.svg` & `betterdata-23.0.1/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `betterdata-22.1.0/readme.md` & `betterdata-23.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `betterdata-22.1.0/PKG-INFO` & `betterdata-23.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: betterdata
-Version: 22.1.0
+Version: 23.0.1
 Summary: a lib for working with data
 Project-URL: Homepage, https://github.com/gmankab/betterdata
 Project-URL: Documentation, https://github.com/gmankab/betterdata
 Project-URL: Bug Tracker, https://github.com/gmankab/betterdata/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: easyselect
-Requires-Dist: gmanka-yml
+Requires-Dist: easyselect==23.0.0
+Requires-Dist: gmanka-yml==23.0.0
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # betterdata by gmanka
 
 <img src="https://github.com/gmankab/betterdata/raw/main/img/transparent.png">
```

