# Comparing `tmp/gmanka_yml-23.0.2.tar.gz` & `tmp/gmanka_yml-23.0.3.tar.gz`

## Comparing `gmanka_yml-23.0.2.tar` & `gmanka_yml-23.0.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/changelog.md
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/start.sh
--rwxr-xr-x   0        0        0     1981 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/gmanka_yml/__init__.py
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/.gitignore
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/pyproject.toml
--rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/readme.md
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/changelog.md
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/gmanka_yml/__init__.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/.gitignore
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/readme.md
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/PKG-INFO
```

### Comparing `gmanka_yml-23.0.2/gmanka_yml/__init__.py` & `gmanka_yml-23.0.3/gmanka_yml/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,68 +36,61 @@
         file = path,
         mode = 'w',
         encoding = 'utf-8',
     ) as file:
         file.write(
             to_str(
                 data,
-            )
+            ),
         )
 
 
-def read_str(
+def from_str(
     data: str | TextIOWrapper,
     default = _sential,
     expected_type = None,
 ):
     try:
-        loaded = yaml.load(
-            data,
-            Loader = yaml.CLoader,
-        )
-    except AttributeError:
-        return yaml.load(
-            data,
-            Loader = yaml.Loader,
+        parsed = yaml.safe_load(
+            stream = data,
         )
     except Exception as error:
         if default == _sential:
             raise error
         else:
             return default
     if expected_type == None:
-        return data
+        return parsed
     elif isinstance(
-        data,
+        parsed,
         expected_type,
     ):
-        return data
+        return parsed
     elif default == _sential:
         raise TypeError(
             f'{expected_type} expected, but got type(data)'
         )
     else:
         return default
 
 
-def read_file(
+def from_file(
     path: str | Path,
     default = _sential,
     expected_type = None,
 ):
     try:
         with open(
             file = path,
             mode = 'r',
-            encoding = 'utf-8',
         ) as file:
-            return read_str(
-                file,
-                default = default,
-                expected_type = expected_type,
+            return from_str( 
+                data = file, 
+                default = default, 
+                expected_type = expected_type, 
             )
     except Exception as error:
         if default == _sential:
             raise error
         else:
             return default
```

### Comparing `gmanka_yml-23.0.2/pyproject.toml` & `gmanka_yml-23.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "pyyaml",
 ]
 name = "gmanka_yml"
-version = "23.0.2"
+version = "23.0.3"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "some useful shortcuts for pyyaml"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gmanka_yml-23.0.2/readme.md` & `gmanka_yml-23.0.3/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 pip install gmanka_yml
 ```
 
 ## functions
 
 - [to_str](#to_str)  
 - [to_file](#to_file)  
-- [read_str](#read_str)  
-- [read_file](#read_file)  
+- [from_str](#read_str)  
+- [from_file](#read_file)  
 
 ## to_str[^](#functions)
 
 converts any data to yml string and returns it
 
 ```py
 import gmanka_yml as yml
@@ -51,66 +51,66 @@
 ```py
 yml.to_file(
     data = my_dict,
     path = 'file.yml',
 )
 ```
 
-## read_str[^](#functions)
+## from_str[^](#functions)
 
 ```py
 import gmanka_yml as yml
 
 my_str = '''
 element_1: 1
 2: element_2
 3:
 - list_element_1
 - list_element_2
 '''
 
-my_dict = yml.read_str(my_str)
+my_dict = yml.from_str(my_str)
 
 print(my_dict)
 
 print(type(my_dict))
 ```
 
 output:
 
 ```py
 {'element_1': 1, 2: 'element_2', 3: ['list_element_1', 'list_element_2']}
 
 <class 'dict'>
 ```
 
-## read_file[^](#functions)
+## from_file[^](#functions)
 
-same as [read_str](#read_str), but reads data from file
+same as [from_str](#read_str), but reads data from file
 
 ```py
-yml.read_file('file.yml')
+yml.from_file('file.yml')
 ```
 
 ## default values
 
 ```py
-yml.read_str(1) # raises TypeError
+yml.from_str(1) # raises TypeError
 
-yml.read_str(1, default = None) # returns None
+yml.from_str(1, default = None) # returns None
 ```
 
 ## expected_type
 
 ```py
-yml.read_str(
+yml.from_str(
     data = '{}',
     expected_type = list,
 ) # raises TypeError
 
-yml.read_str(
+yml.from_str(
     data = '{}',
     default = None,
     expected_type = list,
 ) # returns None
 ```
```

### Comparing `gmanka_yml-23.0.2/PKG-INFO` & `gmanka_yml-23.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmanka_yml
-Version: 23.0.2
+Version: 23.0.3
 Summary: some useful shortcuts for pyyaml
 Project-URL: Homepage, https://github.com/gmankab/yml
 Project-URL: Documentation, https://github.com/gmankab/yml
 Project-URL: Bug Tracker, https://github.com/gmankab/yml/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,16 +23,16 @@
 pip install gmanka_yml
 ```
 
 ## functions
 
 - [to_str](#to_str)  
 - [to_file](#to_file)  
-- [read_str](#read_str)  
-- [read_file](#read_file)  
+- [from_str](#read_str)  
+- [from_file](#read_file)  
 
 ## to_str[^](#functions)
 
 converts any data to yml string and returns it
 
 ```py
 import gmanka_yml as yml
@@ -66,66 +66,66 @@
 ```py
 yml.to_file(
     data = my_dict,
     path = 'file.yml',
 )
 ```
 
-## read_str[^](#functions)
+## from_str[^](#functions)
 
 ```py
 import gmanka_yml as yml
 
 my_str = '''
 element_1: 1
 2: element_2
 3:
 - list_element_1
 - list_element_2
 '''
 
-my_dict = yml.read_str(my_str)
+my_dict = yml.from_str(my_str)
 
 print(my_dict)
 
 print(type(my_dict))
 ```
 
 output:
 
 ```py
 {'element_1': 1, 2: 'element_2', 3: ['list_element_1', 'list_element_2']}
 
 <class 'dict'>
 ```
 
-## read_file[^](#functions)
+## from_file[^](#functions)
 
-same as [read_str](#read_str), but reads data from file
+same as [from_str](#read_str), but reads data from file
 
 ```py
-yml.read_file('file.yml')
+yml.from_file('file.yml')
 ```
 
 ## default values
 
 ```py
-yml.read_str(1) # raises TypeError
+yml.from_str(1) # raises TypeError
 
-yml.read_str(1, default = None) # returns None
+yml.from_str(1, default = None) # returns None
 ```
 
 ## expected_type
 
 ```py
-yml.read_str(
+yml.from_str(
     data = '{}',
     expected_type = list,
 ) # raises TypeError
 
-yml.read_str(
+yml.from_str(
     data = '{}',
     default = None,
     expected_type = list,
 ) # returns None
 ```
```

