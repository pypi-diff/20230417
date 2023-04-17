# Comparing `tmp/dnadb-0.2.6.tar.gz` & `tmp/dnadb-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.2.6.tar", last modified: Fri Apr 14 19:33:06 2023, max compression
+gzip compressed data, was "dnadb-0.2.7.tar", last modified: Mon Apr 17 03:05:38 2023, max compression
```

## Comparing `dnadb-0.2.6.tar` & `dnadb-0.2.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.6/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 19:33:06.681676 dnadb-0.2.6/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.6/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-14 19:32:15.000000 dnadb-0.2.6/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-14 19:33:06.681676 dnadb-0.2.6/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-14 19:32:23.000000 dnadb-0.2.6/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.6/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.6/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.6/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.6/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.6/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.6/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.6/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.6/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.6/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    14308 2023-04-14 19:31:56.000000 dnadb-0.2.6/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.6/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.366622 dnadb-0.2.7/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.7/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-17 03:05:38.366622 dnadb-0.2.7/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.7/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-17 03:04:57.000000 dnadb-0.2.7/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-17 03:05:38.366622 dnadb-0.2.7/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.362621 dnadb-0.2.7/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.362621 dnadb-0.2.7/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-17 03:05:03.000000 dnadb-0.2.7/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.366622 dnadb-0.2.7/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.7/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.7/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.7/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.366622 dnadb-0.2.7/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.7/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.7/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.7/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.7/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.7/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.7/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    15111 2023-04-17 02:55:42.000000 dnadb-0.2.7/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.7/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.362621 dnadb-0.2.7/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.2.6/LICENSE` & `dnadb-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/PKG-INFO` & `dnadb-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.2.6/pyproject.toml` & `dnadb-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.2.6/src/dnadb/datasets/dataset.py` & `dnadb-0.2.7/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/datasets/greengenes.py` & `dnadb-0.2.7/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.2.7/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.2.7/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/db.py` & `dnadb-0.2.7/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/dna.py` & `dnadb-0.2.7/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/fasta.py` & `dnadb-0.2.7/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/fastq.py` & `dnadb-0.2.7/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb/taxonomy.py` & `dnadb-0.2.7/src/dnadb/taxonomy.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .db import DbFactory
 from .utils import open_file
 
 TAXON_LEVEL_NAMES = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 TAXON_PREFIXES = ''.join(name[0] for name in TAXON_LEVEL_NAMES).lower()
 
 class TaxonHierarchyJson(TypedDict):
+    max_depth: int
     parent_map: List[Dict[str, str]]
 
 # Utility Functions --------------------------------------------------------------------------------
 
 def split_taxonomy(taxonomy: str, max_depth: int = 7) -> Tuple[str, ...]:
     """
     Split taxonomy label into a tuple
@@ -150,16 +151,20 @@
         """
         return self.encode(taxonomy_entry.taxons(len(self.taxon_identifiers)))
 
 
 class TaxonomyHierarchy:
     @classmethod
     def deserialize(cls, taxonomy_hierarchy: bytes) -> "TaxonomyHierarchy":
-        hierarchy_json: TaxonHierarchyJson = json.loads(taxonomy_hierarchy.decode())
-        hierarchy = TaxonomyHierarchy(len(hierarchy_json["parent_map"]))
+        return cls.from_json(json.loads(taxonomy_hierarchy.decode()))
+
+    @classmethod
+    def from_json(cls, hierarchy_json: TaxonHierarchyJson) -> "TaxonomyHierarchy":
+        hierarchy = TaxonomyHierarchy(hierarchy_json["max_depth"])
+        hierarchy.depth = len(hierarchy_json["parent_map"])
         for i in range(len(hierarchy.taxon_maps)):
             taxon_map = hierarchy.taxon_maps[i]
             parent_map = hierarchy_json["parent_map"][i]
             for child, parent_name in parent_map.items():
                 parent = hierarchy.taxon_maps[i-1][parent_name] if i > 0 else None
                 taxon_map[child] = Taxon(child, parent)
         return hierarchy
@@ -177,44 +182,52 @@
         for label in set(labels):
             hierarchy.add_taxons(split_taxonomy(label))
         return hierarchy
 
     @classmethod
     def merge(cls, hierarchies: Iterable["TaxonomyHierarchy"]) -> "TaxonomyHierarchy":
         hierarchy_list = list(hierarchies)
-        depth = min(hierarchy.depth for hierarchy in hierarchy_list)
-        if any(hierarchy.depth > depth for hierarchy in hierarchy_list):
+        max_depth = min(hierarchy.max_depth for hierarchy in hierarchy_list)
+        if any(hierarchy.depth > max_depth for hierarchy in hierarchy_list):
             print(
-                "Warning: Merging taxonomy hierarchies with different depths.",
-                f"Using depth: {depth}."
+                "Warning: Merging taxonomy hierarchies with different maximum depths.",
+                f"Using depth: {max_depth}."
             )
-        merged_hierarchy = TaxonomyHierarchy(depth)
+        merged_hierarchy = TaxonomyHierarchy(max_depth)
+        # Largest depth smaller than the maximum depth, or the maximum depth if no such depth exists
+        merged_hierarchy.depth = min(max(h.depth for h in hierarchy_list), max_depth)
         for other_hierarchy in hierarchy_list:
-            for i in range(depth):
+            for i in range(min(other_hierarchy.depth, merged_hierarchy.depth)):
                 to_map = merged_hierarchy.taxon_maps[i]
                 from_map = other_hierarchy.taxon_maps[i]
                 for taxon in from_map.values():
+                    if taxon.name in to_map:
+                        continue
                     if i > 0 and taxon.parent is not None:
                         parent = merged_hierarchy.taxon_maps[i-1][taxon.parent.name]
                     else:
                         parent = None
                     to_map[taxon.name] = Taxon(taxon.name, parent)
         return merged_hierarchy
 
-    def __init__(self, depth: int = 7):
-        self.taxon_maps: List[Dict[str, Taxon]] = [{} for _ in range(depth)] # taxon -> parent
+    def __init__(self, max_depth: int = 7):
+        self.max_depth = max_depth
+        self.taxon_maps: List[Dict[str, Taxon]] = [] # taxon -> parent
 
     def add_entry(self, entry: "TaxonomyEntry"):
-        self.add_taxons(entry.taxons(self.depth))
+        self.add_taxons(entry.taxons(self.max_depth))
 
     def add_taxonomy(self, entry: str):
         self.add_taxons(split_taxonomy(entry))
 
     def add_taxons(self, taxons: Tuple[str, ...]):
         parent: Optional[Taxon] = None
+        taxons = tuple(taxon for taxon in taxons[:self.max_depth] if taxon != "")
+        if len(taxons) > self.depth:
+            self.depth = len(taxons)
         for taxon_map, taxon_name in zip(self.taxon_maps, taxons):
             if taxon_name not in taxon_map:
                 taxon_map[taxon_name] = Taxon(taxon_name, parent)
             parent = taxon_map[taxon_name]
 
     def is_valid(self, taxons: Union[str, Tuple[str, ...]]) -> bool:
         taxon_list = split_taxonomy(taxons) if isinstance(taxons, str) else taxons
@@ -259,34 +272,38 @@
                     result.append(child)
                     continue
                 result += find_leaves(child)
             return result
         return [leaf for taxon in self.taxon_maps[0].values() for leaf in find_leaves(taxon)]
 
     def serialize(self) -> bytes:
-        json_hierarchy: TaxonHierarchyJson = {
+        json_hierarchy = self.to_json()
+        return json.dumps(json_hierarchy, separators=(',', ':')).encode()
+
+    def to_json(self) -> TaxonHierarchyJson:
+        return {
+            "max_depth": self.max_depth,
             "parent_map": [
                 {taxon.name: taxon.parent.name if taxon.parent else "" for taxon in m.values()}
                 for m in self.taxon_maps
             ]
         }
-        return json.dumps(json_hierarchy, separators=(',', ':')).encode()
 
     @property
     def depth(self):
         return len(self.taxon_maps)
 
     @depth.setter
     def depth(self, depth: int):
         assert depth >= 1
         if depth >= self.depth:
             for i in range(self.depth, depth):
                 self.taxon_maps.append({})
             return
-        for taxon in self.taxon_maps[ - 1].values():
+        for taxon in self.taxon_maps[depth - 1].values():
             taxon.children.clear()
         self.taxon_maps = self.taxon_maps[:depth]
 
     @cached_property
     def identifier_map(self) -> TaxonomyIdentifierMap:
         return TaxonomyIdentifierMap(((taxon for taxon in m) for m in self.taxon_maps))
 
@@ -322,17 +339,17 @@
         return f"{self.identifier}\t{self.label}"
 
 
 class TaxonomyDbFactory(DbFactory):
     """
     A factory for creating LMDB-backed databases of FASTA entries.
     """
-    def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
+    def __init__(self, path: Union[str, Path], max_depth: int = 7, chunk_size: int = 10000):
         super().__init__(path, chunk_size)
-        self.hierarchy = TaxonomyHierarchy()
+        self.hierarchy = TaxonomyHierarchy(max_depth)
         self.num_entries = np.int32(0)
 
     def write_entry(self, entry: TaxonomyEntry):
         """
         Create a new FASTA LMDB database from a FASTA file.
         """
         self.hierarchy.add_entry(entry)
```

### Comparing `dnadb-0.2.6/src/dnadb/utils.py` & `dnadb-0.2.7/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.6/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.2.7/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

