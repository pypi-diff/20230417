# Comparing `tmp/dmtpy-0.3.2.tar.gz` & `tmp/dmtpy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtpy-0.3.2.tar", last modified: Wed Mar  1 11:30:52 2023, max compression
+gzip compressed data, was "dmtpy-0.3.3.tar", last modified: Mon Apr 17 08:55:33 2023, max compression
```

## Comparing `dmtpy-0.3.2.tar` & `dmtpy-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:52.469224 dmtpy-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-01 11:30:37.000000 dmtpy-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-01 11:30:52.469224 dmtpy-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-01 11:30:37.000000 dmtpy-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 11:30:52.469224 dmtpy-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-01 11:30:37.000000 dmtpy-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:52.469224 dmtpy-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:52.469224 dmtpy-0.3.2/src/dmt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/blueprint_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:52.469224 dmtpy-0.3.2/src/dmt/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/blueprints/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/blueprints/namedentity.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/dmt_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/dmt_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/enum_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:52.469224 dmtpy-0.3.2/src/dmt/h5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/h5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/h5/h5_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/h5/h5_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-01 11:30:37.000000 dmtpy-0.3.2/src/dmt/namedentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:30:52.469224 dmtpy-0.3.2/src/dmtpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-01 11:30:52.000000 dmtpy-0.3.2/src/dmtpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-01 11:30:52.000000 dmtpy-0.3.2/src/dmtpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 11:30:52.000000 dmtpy-0.3.2/src/dmtpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-01 11:30:52.000000 dmtpy-0.3.2/src/dmtpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-01 11:30:52.000000 dmtpy-0.3.2/src/dmtpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-17 08:55:12.000000 dmtpy-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 08:55:33.717674 dmtpy-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 08:55:12.000000 dmtpy-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:55:33.717674 dmtpy-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 08:55:12.000000 dmtpy-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.713674 dmtpy-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprint_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmt/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprints/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprints/namedentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/dmt_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/dmt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/enum_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmt/h5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/h5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/h5/h5_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/h5/h5_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/namedentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmtpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/top_level.txt
```

### Comparing `dmtpy-0.3.2/LICENSE` & `dmtpy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/PKG-INFO` & `dmtpy-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtpy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python runtime library for SIMOS based DMT models
 Home-page: https://github.com/SINTEF/dmtpy
 Author: SINTEF Ocean
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dmtpy-0.3.2/setup.py` & `dmtpy-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Remove build and dist folders
 shutil.rmtree(Path("build"), ignore_errors=True)
 shutil.rmtree(Path("dist"), ignore_errors=True)
 
 setup(
     name="dmtpy",
-    version="0.3.2",
+    version="0.3.3",
     author="SINTEF Ocean",
     description="Python runtime library for SIMOS based DMT models",
     url="https://github.com/SINTEF/dmtpy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages(where="src", exclude=["tests"]),
```

### Comparing `dmtpy-0.3.2/src/dmt/attribute.py` & `dmtpy-0.3.3/src/dmt/attribute.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmt/blueprint.py` & `dmtpy-0.3.3/src/dmt/blueprint.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmt/blueprint_attribute.py` & `dmtpy-0.3.3/src/dmt/blueprint_attribute.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmt/dmt_reader.py` & `dmtpy-0.3.3/src/dmt/dmt_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,23 +59,23 @@
         entities = [self.__from_dict(e) for e in ent_dicts]
         self.__resolve_all()
         return entities
 
     def __resolve_all(self):
         for ref in self.unresolved:
             if not self.__resolve(ref):
-                raise Exception(f"Unresolved reference: {ref}")
+                raise ValueError(f"Unresolved reference: {ref}")
 
 
     def __from_dict(self,ent_dict: Dict) -> Entity:
         """ Read entities from Dict """
         entity_type: str=ent_dict["type"]
         constructor = self._resolve_type(entity_type)
         if not constructor:
-            raise Exception(f"Unkown entity type {entity_type}")
+            raise ValueError(f"Unkown entity type {entity_type}")
         entity_instance: Entity = constructor()
         blueprint = entity_instance.blueprint
         for key, value in ent_dict.items():
             if key == "_id":
                 uid = value
                 self.entities[uid] = entity_instance
                 continue
@@ -104,15 +104,15 @@
         ename = parts.pop()
         package_path = ".".join(parts)
         if self.root_package:
             package_path = self.root_package + "." + package_path
         try:
             pkg = import_module(package_path)
         except ModuleNotFoundError as error:
-            raise Exception(f"Unable to load package {package_path}") from error
+            raise ModuleNotFoundError(f"Unable to load package {package_path}") from error
 
         constructor = pkg.__dict__.get(ename)
         return constructor
 
     def __set_blueprint_value(self,entity_instance: Entity, attribute: EnumAttribute,value):
         if attribute.contained:
             self.__set_value(entity_instance,attribute,value)
@@ -147,10 +147,10 @@
         return False
 
     def __set_enum_value(self,entity: Entity, attribute: EnumAttribute,value: str):
         """ Convert from string to Enum"""
 
         constructor = self._resolve_type(attribute.type)
         if not constructor:
-            raise Exception(f"Unkown Enum type {attribute.type}")
+            raise ValueError(f"Unkown Enum type {attribute.type}")
         evalue = constructor[value]
         setattr(entity,attribute.name, evalue)
```

### Comparing `dmtpy-0.3.2/src/dmt/dmt_writer.py` & `dmtpy-0.3.3/src/dmt/dmt_writer.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmt/entity.py` & `dmtpy-0.3.3/src/dmt/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from typing import Iterator, Sequence, TypeVar,Dict
 
 from dmt.blueprint import Blueprint
 from dmt.dimension import Dimension
 from dmt.attribute import Attribute
 
+
 E = TypeVar("E")
 
 class Entity():
     """ A basic Entity Istance"""
 
     def __init__(self, description="", **kwargs):
         self.description = description
@@ -47,14 +48,22 @@
         if prop.is_string():
             if isinstance(value,Enum):
                 return True
             return len(value) > 0
         if prop.has_dimensions():
             return len(value)>0
         return True
+    
+    def set(self, prop: Attribute, value: any):
+        """Set the attribute"""
+        setattr(self,prop.name,value)
+    
+    def get(self, prop: Attribute) -> any:
+        """Get the attribute"""
+        return getattr(self,prop.name,None)
 
     def content(self) -> Iterator[Entity]:
         """Get direct children contained in this entity"""
         for p in self.blueprint.blueprint_attributes():
             if p.contained and self.is_set(p):
                 value = getattr(self, p.name, None)
                 if p.has_dimensions():
@@ -76,17 +85,11 @@
                         yield child
                         yield from child.all_content()
                 else:
                     child: Entity = value
                     yield child
                     yield from child.all_content()
 
-    def copy(self: E) -> E:
+    def copy(self: E,keep_uncontained_references=False) -> E:
         """"Copy the entity"""
-        from dmt.dmt_reader import DMTReader
-        from dmt.dmt_writer import DMTWriter
-        writer = DMTWriter(use_external_refs=True)
-        entity_dict = writer.to_dict(self)
-        refs = dict(writer.external_refs)
-        for entity, uuid in writer.uuids.items():
-            refs[uuid]=entity
-        return DMTReader(refs).from_dict(entity_dict)
+        from .copier import Copier
+        return Copier(keep_uncontained_references).copy(self)
```

### Comparing `dmtpy-0.3.2/src/dmt/enum_attribute.py` & `dmtpy-0.3.3/src/dmt/enum_attribute.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmt/h5/h5_reader.py` & `dmtpy-0.3.3/src/dmt/h5/h5_reader.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmt/h5/h5_writer.py` & `dmtpy-0.3.3/src/dmt/h5/h5_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         with h5.File(filename, "w") as root:
             for idx, entity in enumerate(entities):
                 self.__write_root(root, idx, entity)
 
     def __write_root(self, group: h5.Group, idx, entity: Entity) -> str:
         try:
             name = entity.name
+            if not name:
+                name = str(idx)
         except AttributeError:
             name = str(idx)
         grp = group.create_group(name)
         self.__write_group(grp, entity)
         return name
 
     def __write_group(self, group: h5.Group, entity: Entity):
```

### Comparing `dmtpy-0.3.2/src/dmt/namedentity.py` & `dmtpy-0.3.3/src/dmt/namedentity.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.2/src/dmtpy.egg-info/PKG-INFO` & `dmtpy-0.3.3/src/dmtpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtpy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python runtime library for SIMOS based DMT models
 Home-page: https://github.com/SINTEF/dmtpy
 Author: SINTEF Ocean
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dmtpy-0.3.2/src/dmtpy.egg-info/SOURCES.txt` & `dmtpy-0.3.3/src/dmtpy.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 src/dmt/__init__.py
 src/dmt/attribute.py
 src/dmt/blueprint.py
 src/dmt/blueprint_attribute.py
+src/dmt/copier.py
 src/dmt/dimension.py
 src/dmt/dmt_reader.py
 src/dmt/dmt_writer.py
 src/dmt/entity.py
 src/dmt/enum_attribute.py
 src/dmt/namedentity.py
 src/dmt/blueprints/__init__.py
```

