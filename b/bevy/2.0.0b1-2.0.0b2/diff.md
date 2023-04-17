# Comparing `tmp/bevy-2.0.0b1.tar.gz` & `tmp/bevy-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bevy-2.0.0b1.tar", max compression
+gzip compressed data, was "bevy-2.0.0b2.tar", max compression
```

## Comparing `bevy-2.0.0b1.tar` & `bevy-2.0.0b2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1076 2023-04-16 23:31:42.061579 bevy-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     5871 2023-04-16 23:31:42.061579 bevy-2.0.0b1/README.md
--rw-r--r--   0        0        0      208 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/__init__.py
--rw-r--r--   0        0        0     1463 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/contextvar.py
--rw-r--r--   0        0        0     1692 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/injectors/classes.py
--rw-r--r--   0        0        0     2244 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/injectors/functions.py
--rw-r--r--   0        0        0     2717 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/options.py
--rw-r--r--   0        0        0      164 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/annotated_provider.py
--rw-r--r--   0        0        0     3488 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/base.py
--rw-r--r--   0        0        0     1143 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/type_provider.py
--rw-r--r--   0        0        0     5950 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/repository.py
--rw-r--r--   0        0        0      866 2023-04-16 23:31:42.061579 bevy-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     6710 1970-01-01 00:00:00.000000 bevy-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-17 00:09:47.133909 bevy-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0     5859 2023-04-17 00:09:47.133909 bevy-2.0.0b2/README.md
+-rw-r--r--   0        0        0      208 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/__init__.py
+-rw-r--r--   0        0        0     1463 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/contextvar.py
+-rw-r--r--   0        0        0     1692 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/injectors/classes.py
+-rw-r--r--   0        0        0     2244 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/injectors/functions.py
+-rw-r--r--   0        0        0     2717 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/options.py
+-rw-r--r--   0        0        0      164 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/__init__.py
+-rw-r--r--   0        0        0     1537 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/annotated_provider.py
+-rw-r--r--   0        0        0     3488 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/base.py
+-rw-r--r--   0        0        0     1143 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/type_provider.py
+-rw-r--r--   0        0        0     5950 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/repository.py
+-rw-r--r--   0        0        0      866 2023-04-17 00:09:47.133909 bevy-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b2/PKG-INFO
```

### Comparing `bevy-2.0.0b1/LICENSE` & `bevy-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/README.md` & `bevy-2.0.0b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,12 +80,12 @@
 
 **Dependency Providers**
 
 To make Bevy as flexible as possible, it has dependency providers. These are classes that can be registered with the repository to cache value instances, look up cached instances using a key type, and create new instances for a key type.
 
 The default repository type has two dependency providers: an annotated provider and a type provider.
 - The **Type Provider** handles key types that are class types. So when a dependency annotation is `Thing`, for example, the type provider will handle looking through its cache for an instance of `Thing` and creating an instance if it is not found.
-- The **Annotated Provider** handles key types that are instances of `typing.Annotated`. It works very similarly to the type provider except it allows you to provide an annotation. This is helpful if you have multiple instances of the same type that need to exist together. You could have `Annotated[Thing, {"test": "A"}]` and `Annotated[Thing, {"test": "B"}]`, both of them would be able to point to distinct instances of `Thing` in the same repository cache.
+- The **Annotated Provider** handles key types that are instances of `typing.Annotated`. It works very similarly to the type provider except it allows you to provide an annotation. This is helpful if you have multiple instances of the same type that need to exist together. You could have `Annotated[Thing, "testA"]` and `Annotated[Thing, "testB"]`, both of them would be able to point to distinct instances of `Thing` in the same repository cache.
 
 It is possible to add new providers to the repository using it's `add_providers` method which takes any number of provider types.
 
 It is also possible to subclass `bevy.Repository`, provide a custom `factory` class method that returns an instance of `Repository` with whatever default providers you want set. Just call `Repository.set_repository` with an instance of the new repository type.
```

### Comparing `bevy-2.0.0b1/bevy/contextvar.py` & `bevy-2.0.0b2/bevy/contextvar.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/injectors/classes.py` & `bevy-2.0.0b2/bevy/injectors/classes.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/injectors/functions.py` & `bevy-2.0.0b2/bevy/injectors/functions.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/options.py` & `bevy-2.0.0b2/bevy/options.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/providers/annotated_provider.py` & `bevy-2.0.0b2/bevy/providers/annotated_provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/providers/base.py` & `bevy-2.0.0b2/bevy/providers/base.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/providers/type_provider.py` & `bevy-2.0.0b2/bevy/providers/type_provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/bevy/repository.py` & `bevy-2.0.0b2/bevy/repository.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b1/pyproject.toml` & `bevy-2.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Bevy"
-version = "2.0.0b1"
+version = "2.0.0b2"
 description = "Python Dependency Inversion made simple so you can focus on creating amazing code."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Bevy"
 repository = "https://github.com/ZechCodes/Bevy"
 documentation = "https://github.com/ZechCodes/Bevy/blob/master/README.md"
```

### Comparing `bevy-2.0.0b1/PKG-INFO` & `bevy-2.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bevy
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Python Dependency Inversion made simple so you can focus on creating amazing code.
 Home-page: https://github.com/ZechCodes/Bevy
 License: MIT
 Keywords: dependency,injection,annotations,types
 Author: Zech Zimmerman
 Author-email: hi@zech.codes
 Requires-Python: >=3.10,<4.0
@@ -100,12 +100,12 @@
 
 **Dependency Providers**
 
 To make Bevy as flexible as possible, it has dependency providers. These are classes that can be registered with the repository to cache value instances, look up cached instances using a key type, and create new instances for a key type.
 
 The default repository type has two dependency providers: an annotated provider and a type provider.
 - The **Type Provider** handles key types that are class types. So when a dependency annotation is `Thing`, for example, the type provider will handle looking through its cache for an instance of `Thing` and creating an instance if it is not found.
-- The **Annotated Provider** handles key types that are instances of `typing.Annotated`. It works very similarly to the type provider except it allows you to provide an annotation. This is helpful if you have multiple instances of the same type that need to exist together. You could have `Annotated[Thing, {"test": "A"}]` and `Annotated[Thing, {"test": "B"}]`, both of them would be able to point to distinct instances of `Thing` in the same repository cache.
+- The **Annotated Provider** handles key types that are instances of `typing.Annotated`. It works very similarly to the type provider except it allows you to provide an annotation. This is helpful if you have multiple instances of the same type that need to exist together. You could have `Annotated[Thing, "testA"]` and `Annotated[Thing, "testB"]`, both of them would be able to point to distinct instances of `Thing` in the same repository cache.
 
 It is possible to add new providers to the repository using it's `add_providers` method which takes any number of provider types.
 
 It is also possible to subclass `bevy.Repository`, provide a custom `factory` class method that returns an instance of `Repository` with whatever default providers you want set. Just call `Repository.set_repository` with an instance of the new repository type.
```

