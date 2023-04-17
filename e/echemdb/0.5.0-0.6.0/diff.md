# Comparing `tmp/echemdb-0.5.0.tar.gz` & `tmp/echemdb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echemdb-0.5.0.tar", last modified: Fri Mar 31 20:23:32 2023, max compression
+gzip compressed data, was "echemdb-0.6.0.tar", last modified: Mon Apr 17 06:17:25 2023, max compression
```

## Comparing `echemdb-0.5.0.tar` & `echemdb-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 20:23:32.040058 echemdb-0.5.0/
--rw-rw-rw-   0        0        0    35823 2022-06-29 12:45:45.000000 echemdb-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     3755 2023-03-31 20:23:32.038787 echemdb-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3529 2023-03-31 20:23:15.000000 echemdb-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 20:23:32.022422 echemdb-0.5.0/echemdb/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:45:45.000000 echemdb-0.5.0/echemdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 20:23:32.036278 echemdb-0.5.0/echemdb/cv/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:45:45.000000 echemdb-0.5.0/echemdb/cv/__init__.py
--rw-rw-rw-   0        0        0     3349 2023-03-31 19:55:03.000000 echemdb-0.5.0/echemdb/cv/cv_database.py
--rw-rw-rw-   0        0        0     8312 2023-03-31 19:55:03.000000 echemdb-0.5.0/echemdb/cv/cv_entry.py
--rw-rw-rw-   0        0        0     8382 2023-03-31 19:55:03.000000 echemdb-0.5.0/echemdb/database.py
--rw-rw-rw-   0        0        0     7366 2023-03-31 19:55:03.000000 echemdb-0.5.0/echemdb/descriptor.py
--rw-rw-rw-   0        0        0    17058 2023-03-31 19:55:03.000000 echemdb-0.5.0/echemdb/entry.py
--rw-rw-rw-   0        0        0     3214 2023-03-31 19:55:03.000000 echemdb-0.5.0/echemdb/local.py
--rw-rw-rw-   0        0        0     3474 2023-03-31 19:54:11.000000 echemdb-0.5.0/echemdb/remote.py
-drwxrwxrwx   0        0        0        0 2023-03-31 20:23:32.030323 echemdb-0.5.0/echemdb.egg-info/
--rw-rw-rw-   0        0        0     3755 2023-03-31 20:23:31.000000 echemdb-0.5.0/echemdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-03-31 20:23:31.000000 echemdb-0.5.0/echemdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 20:23:31.000000 echemdb-0.5.0/echemdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-03-31 20:23:31.000000 echemdb-0.5.0/echemdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-31 20:23:31.000000 echemdb-0.5.0/echemdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 20:23:32.040058 echemdb-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1694 2023-03-31 20:23:15.000000 echemdb-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:17:25.443063 echemdb-0.6.0/
+-rw-rw-rw-   0        0        0    35823 2022-06-29 12:45:45.000000 echemdb-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3755 2023-04-17 06:17:25.442023 echemdb-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2023-04-17 06:17:17.000000 echemdb-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 06:17:25.417041 echemdb-0.6.0/echemdb/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:45:45.000000 echemdb-0.6.0/echemdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:17:25.438044 echemdb-0.6.0/echemdb/cv/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:45:45.000000 echemdb-0.6.0/echemdb/cv/__init__.py
+-rw-rw-rw-   0        0        0     3259 2023-04-17 06:15:57.000000 echemdb-0.6.0/echemdb/cv/cv_database.py
+-rw-rw-rw-   0        0        0     9471 2023-04-17 06:15:57.000000 echemdb-0.6.0/echemdb/cv/cv_entry.py
+-rw-rw-rw-   0        0        0     7956 2023-04-17 06:15:57.000000 echemdb-0.6.0/echemdb/database.py
+-rw-rw-rw-   0        0        0     7366 2023-03-31 20:34:39.000000 echemdb-0.6.0/echemdb/descriptor.py
+-rw-rw-rw-   0        0        0    18438 2023-04-17 06:15:57.000000 echemdb-0.6.0/echemdb/entry.py
+-rw-rw-rw-   0        0        0     2547 2023-04-17 06:15:57.000000 echemdb-0.6.0/echemdb/local.py
+-rw-rw-rw-   0        0        0     2596 2023-04-17 06:15:57.000000 echemdb-0.6.0/echemdb/remote.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:17:25.430046 echemdb-0.6.0/echemdb.egg-info/
+-rw-rw-rw-   0        0        0     3755 2023-04-17 06:17:24.000000 echemdb-0.6.0/echemdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-04-17 06:17:25.000000 echemdb-0.6.0/echemdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:17:24.000000 echemdb-0.6.0/echemdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2023-04-17 06:17:24.000000 echemdb-0.6.0/echemdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 06:17:24.000000 echemdb-0.6.0/echemdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 06:17:25.444015 echemdb-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-04-17 06:17:17.000000 echemdb-0.6.0/setup.py
```

### Comparing `echemdb-0.5.0/LICENSE` & `echemdb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echemdb-0.5.0/PKG-INFO` & `echemdb-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: echemdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: a Python library to work with the echemdb repository
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/echemdb/0.5.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/echemdb/0.6.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6502901.svg)](https://doi.org/10.5281/zenodo.6502901)
 
 The echemdb Python package can interact with a database of
 [frictionless datapackages](https://frictionlessdata.io/)
 containing electrochemical data following [echemdb's metadata schema](https://github.com/echemdb/metadata-schema).
 Such a database can be generated from the data on [echemdb.org](https://www.echemdb.org)
 or from local files.
```

### Comparing `echemdb-0.5.0/README.md` & `echemdb-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/echemdb/0.5.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/echemdb/0.6.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6502901.svg)](https://doi.org/10.5281/zenodo.6502901)
 
 The echemdb Python package can interact with a database of
 [frictionless datapackages](https://frictionlessdata.io/)
 containing electrochemical data following [echemdb's metadata schema](https://github.com/echemdb/metadata-schema).
 Such a database can be generated from the data on [echemdb.org](https://www.echemdb.org)
 or from local files.
```

### Comparing `echemdb-0.5.0/echemdb/cv/cv_database.py` & `echemdb-0.6.0/echemdb/cv/cv_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,36 +76,31 @@
             >>> database.materials() == {'Cu', 'Ru'}
             True
 
         """
         import pandas as pd
 
         return set(
-            pd.unique(
-                pd.Series(
-                    [
-                        entry.system.electrodes.working_electrode.material
-                        for entry in self
-                    ]
-                )
-            )
+            pd.unique(pd.Series([entry.get_electrode("WE").material for entry in self]))
         )
 
     def describe(self):
         r"""
         Return some statistics about the database.
 
         EXAMPLES::
 
             >>> database = CVDatabase.create_example()
             >>> database.describe() == \
             ... {'number of references': 2,
-            ... 'number of entries': 2,
+            ... 'number of entries': 3,
             ... 'materials': {'Cu', 'Ru'}}
             True
 
         """
         return {
-            "number of references": len(self.bibliography.entries),
+            "number of references": 0
+            if isinstance(self.bibliography, str)
+            else len(self.bibliography.entries),
             "number of entries": len(self),
             "materials": self.materials(),
         }
```

### Comparing `echemdb-0.5.0/echemdb/cv/cv_entry.py` & `echemdb-0.6.0/echemdb/cv/cv_entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         ('abstract', 'We investigated ...')],
       persons=OrderedCaseInsensitiveDict([('author', [Person('Alves, Otavio B'), Person('Hoster, Harry E'), Person('Behm, Rolf J{\\"u}rgen')])]))
 
 """
 # ********************************************************************
 #  This file is part of echemdb.
 #
-#        Copyright (C) 2021-2022 Albert Engstfeld
+#        Copyright (C) 2021-2023 Albert Engstfeld
 #        Copyright (C)      2021 Johannes Hermann
 #        Copyright (C) 2021-2022 Julian Rüth
 #        Copyright (C)      2021 Nicolas Hörmann
 #
 #  echemdb is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
@@ -79,14 +79,43 @@
             >>> entry = CVEntry.create_examples()[0]
             >>> entry
             CVEntry('alves_2011_electrochemistry_6010_f1a_solid')
 
         """
         return f"CVEntry({self.identifier!r})"
 
+    def get_electrode(self, name):
+        r"""
+        Returns an electrode with the specified name.
+
+        EXAMPLES::
+
+            >>> entry = CVEntry.create_examples()[0]
+            >>> entry.get_electrode('WE') # doctest: +NORMALIZE_WHITESPACE
+            {'name': 'WE', 'function': 'working electrode', 'type': 'single crystal',
+            'crystallographic orientation': '0001', 'material': 'Ru',
+            'preparation procedure': 'Sputtering and flash annealing under UHV
+            conditions with repeated cycles of oxygen adsorption and desorption.',
+            'shape': {'height': {'unit': 'mm', 'value': 2}, 'type': 'hat shaped'},
+            'source': {'supplier': 'Mateck'}}
+
+        TESTS::
+
+            >>> entry.get_electrode('foo') # doctest: +NORMALIZE_WHITESPACE
+            Traceback (most recent call last):
+            ...
+            KeyError: "Electrode with name 'foo' does not exist"
+
+        """
+        for electrode in self.system.electrodes:
+            if electrode["name"] == name:
+                return electrode
+
+        raise KeyError(f"Electrode with name '{name}' does not exist")
+
     def rescale(self, units):
         r"""
         Return a rescaled :class:`CVEntry` with axes in the specified ``units``.
 
         Usage is essentially the same as for :meth:`echemdb.entry.Entry.rescale', i.e.,
         new units are expected as dict, where the key is the axis name and the value
         the new unit, such as `{'j': 'uA / cm2', 't': 'h'}`.
```

### Comparing `echemdb-0.5.0/echemdb/database.py` & `echemdb-0.6.0/echemdb/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     >>> database.filter(lambda entry: entry.source.url == 'https://doi.org/10.1039/C0CP01001D')  # doctest: +REMOTE_DATA
     [Entry('alves_2011_electrochemistry_6010_f1a_solid'), ...
 
 """
 # ********************************************************************
 #  This file is part of echemdb.
 #
-#        Copyright (C) 2021-2022 Albert Engstfeld
+#        Copyright (C) 2021-2023 Albert Engstfeld
 #        Copyright (C) 2021      Johannes Hermann
 #        Copyright (C) 2021-2022 Julian Rüth
 #        Copyright (C) 2021      Nicolas Hörmann
 #
 #  echemdb is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
@@ -61,63 +61,48 @@
 
     """
     from echemdb.entry import Entry
 
     # Entries of this database are created from this type. Subclasses can replace this with a specialized entry type.
     Entry = Entry
 
-    def __init__(self, data_packages=None, bibliography=None):
+    def __init__(self, data_packages=None):
         if data_packages is None:
             import os.path
 
             import echemdb.remote
 
             data_packages = echemdb.remote.collect_datapackages(
                 os.path.join("website-gh-pages", "data", "generated", "svgdigitizer")
             )
 
-            if bibliography is None:
-                bibliography = echemdb.remote.collect_bibliography(
-                    os.path.join("website-gh-pages", "data", "generated")
-                )
-
-        if bibliography is None:
-            bibliography = []
-
-        from collections.abc import Iterable
-
-        if isinstance(bibliography, Iterable):
-            from pybtex.database import BibliographyData
-
-            bibliography = BibliographyData(
-                entries={entry.key: entry for entry in bibliography}
-            )
-
         self._packages = data_packages
-        self._bibliography = bibliography
 
     @classmethod
     def create_example(cls):
         r"""
         Return a sample database for use in automated tests.
 
         EXAMPLES::
 
-            >>> Database.create_example()
-            [Entry('alves_2011_electrochemistry_6010_f1a_solid'), Entry('engstfeld_2018_polycrystalline_17743_f4b_1')]
+            >>> Database.create_example()  # doctest: +NORMALIZE_WHITESPACE
+            [Entry('alves_2011_electrochemistry_6010_f1a_solid'),
+            Entry('engstfeld_2018_polycrystalline_17743_f4b_1'),
+            Entry('no_bibliography')]
 
         """
 
-        entries = cls.Entry.create_examples(
-            "alves_2011_electrochemistry_6010"
-        ) + cls.Entry.create_examples("engstfeld_2018_polycrystalline_17743")
+        entries = (
+            cls.Entry.create_examples("alves_2011_electrochemistry_6010")
+            + cls.Entry.create_examples("engstfeld_2018_polycrystalline_17743")
+            + cls.Entry.create_examples("no_bibliography")
+        )
 
         return cls(
             [entry.package for entry in entries],
-            [entry.bibliography for entry in entries],
         )
 
     @property
     def bibliography(self):
         r"""
         Return a pybtex database of all bibtex bibliography files.
 
@@ -128,25 +113,43 @@
             BibliographyData(
               entries=OrderedCaseInsensitiveDict([
                 ('alves_2011_electrochemistry_6010', Entry('article',
                 ...
                 ('engstfeld_2018_polycrystalline_17743', Entry('article',
                 ...
 
+        A database with entries without bibliography.
+
+            >>> database = Database.create_example()["no_bibliography"]
+            >>> database.bibliography
+            ''
+
         """
         from pybtex.database import BibliographyData
 
-        return BibliographyData(
+        bib_data = BibliographyData(
             {
                 entry.bibliography.key: entry.bibliography
                 for entry in self
                 if entry.bibliography
             }
         )
 
+        if isinstance(bib_data, str):
+            return bib_data
+
+        # Remove duplicates from the bibliography
+        bib_data_ = BibliographyData()
+
+        for key, entry in bib_data.entries.items():
+            if key not in bib_data_.entries:
+                bib_data_.add_entry(key, entry)
+
+        return bib_data_
+
     def filter(self, predicate):
         r"""
         Return the subset of the database that satisfies predicate.
 
         EXAMPLES::
 
             >>> database = Database.create_example()
@@ -170,59 +173,47 @@
                 logger.debug(f"Filter removed entry {entry} due to error: {e}")
                 return False
 
         return type(self)(
             data_packages=[
                 entry.package for entry in self if catching_predicate(entry)
             ],
-            bibliography=self._bibliography,
         )
 
     def __iter__(self):
         r"""
         Return an iterator over the entries in this database.
 
         EXAMPLES::
 
             >>> database = Database.create_example()
             >>> next(iter(database))
             Entry('alves_2011_electrochemistry_6010_f1a_solid')
 
         """
-
-        def get_bibliography(package):
-            if len(self._bibliography.entries) == 0:
-                return None
-            try:
-                bib = self.Entry(package, bibliography=None).source.citation_key
-            except AttributeError:
-                return None
-
-            return self._bibliography.entries.get(bib, None)
-
         # Return the entries sorted by their identifier. There's a small cost
         # associated with the sorting but we do not expect to be managing
         # millions of identifiers and having them show in sorted order is very
         # convenient, e.g., when doctesting.
         return iter(
             [
-                self.Entry(package, bibliography=get_bibliography(package))
+                self.Entry(package)
                 for package in sorted(self._packages, key=lambda p: p.resources[0].name)
             ]
         )
 
     def __len__(self):
         r"""
         Return the number of entries in this database.
 
         EXAMPLES::
 
             >>> database = Database.create_example()
             >>> len(database)
-            2
+            3
 
         """
         return len(self._packages)
 
     def __repr__(self):
         r"""
         Return a printable representation of this database.
```

### Comparing `echemdb-0.5.0/echemdb/descriptor.py` & `echemdb-0.6.0/echemdb/descriptor.py`

 * *Files identical despite different names*

### Comparing `echemdb-0.5.0/echemdb/entry.py` & `echemdb-0.6.0/echemdb/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ('abstract', 'We investigated ...')],
       persons=OrderedCaseInsensitiveDict([('author', [Person('Alves, Otavio B'), Person('Hoster, Harry E'), Person('Behm, Rolf J{\\"u}rgen')])]))
 
 """
 # ********************************************************************
 #  This file is part of echemdb.
 #
-#        Copyright (C) 2021-2022 Albert Engstfeld
+#        Copyright (C) 2021-2023 Albert Engstfeld
 #        Copyright (C)      2021 Johannes Hermann
 #        Copyright (C) 2021-2022 Julian Rüth
 #        Copyright (C)      2021 Nicolas Hörmann
 #
 #  echemdb is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
@@ -67,17 +67,16 @@
 
         >>> from echemdb.database import Database
         >>> database = Database.create_example()
         >>> entry = next(iter(database))
 
     """
 
-    def __init__(self, package, bibliography):
+    def __init__(self, package):
         self.package = package
-        self.bibliography = bibliography
 
     @property
     def identifier(self):
         r"""
         Return a unique identifier for this entry, i.e., its filename.
 
         EXAMPLES::
@@ -97,32 +96,33 @@
 
         EXAMPLES::
 
             >>> entry = Entry.create_examples()[0]
             >>> dir(entry) # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             [... 'bibliography', 'citation', 'create_examples', 'curation',
             'data_description', 'df', 'experimental', 'field_unit', 'figure_description',
-            'identifier', 'package',  'plot', 'rescale', 'resources', 'source',
-            'system', 'version', 'yaml']
-
+            'identifier', 'package',  'plot', 'rescale', 'source',
+            'system', 'yaml']
 
         """
         return list(set(dir(self._descriptor) + object.__dir__(self)))
 
     def __getattr__(self, name):
         r"""
         Return a property of the data package's descriptor.
 
         EXAMPLES::
 
             >>> entry = Entry.create_examples()[0]
-            >>> entry.source # doctest: +NORMALIZE_WHITESPACE
+            >>> entry.source # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             {'citation key': 'alves_2011_electrochemistry_6010',
             'url': 'https://doi.org/10.1039/C0CP01001D',
-            'version': 1, 'figure': '1a', 'curve': 'solid'}
+            'figure': '1a',
+            'curve': 'solid',
+            'bibdata': '@article{alves_2011_electrochemistry_6010,...}
 
         The returned descriptor can again be accessed in the same way::
 
             >>> entry.system.electrolyte.components[0].name
             'H2O'
 
         """
@@ -134,22 +134,69 @@
 
         EXAMPLES::
 
             >>> entry = Entry.create_examples()[0]
             >>> entry["source"] # doctest: +NORMALIZE_WHITESPACE
             {'citation key': 'alves_2011_electrochemistry_6010',
             'url': 'https://doi.org/10.1039/C0CP01001D',
-            'version': 1, 'figure': '1a', 'curve': 'solid'}
+            'figure': '1a',
+            'curve': 'solid',
+            'bibdata': '@article{alves_2011_electrochemistry_6010,...}
 
         """
         return self._descriptor[name]
 
     @property
     def _descriptor(self):
-        return Descriptor(self.package.to_dict())
+        return Descriptor(self.package.resources[0].custom["metadata"]["echemdb"])
+
+    @property
+    def _metadata(self):
+        r"""
+        Returns the metadata of the resource named "echemdb".
+
+        EXAMPLES::
+
+            >>> entry = Entry.create_examples()[0]
+            >>> entry._metadata # doctest: +NORMALIZE_WHITESPACE
+            {...'source': {'citation key': 'alves_2011_electrochemistry_6010',...}
+
+        """
+        return self.package.resources[0].custom["metadata"]["echemdb"]
+
+    @property
+    def bibliography(self):
+        r"""
+        Return a pybtex bibliography object.
+
+        EXAMPLES::
+
+            >>> entry = Entry.create_examples()[0]
+            >>> entry.bibliography # doctest: +NORMALIZE_WHITESPACE
+            Entry('article',
+            fields=[
+                ('title', ...
+                ...
+
+            >>> entry_no_bib = Entry.create_examples(name="no_bibliography")[0]
+            >>> entry_no_bib.bibliography
+            ''
+
+        """
+        metadata = self._metadata.setdefault("source", {})
+        citation = metadata.setdefault("bibdata", "")
+
+        if not citation:
+            logger.warning(f"Entry with name {self.identifier} has no bibliography.")
+            return citation
+
+        from pybtex.database import parse_string
+
+        bibliography = parse_string(citation, "bibtex")
+        return bibliography.entries[self.source.citation_key]
 
     def citation(self, backend="text"):
         r"""
         Return a formatted reference for the entry's bibliography such as:
 
         J. Doe, et al., Journal Name, volume (YEAR) page, "Title"
 
@@ -295,15 +342,15 @@
                 )
 
         df_resource = Resource(df)
         df_resource.infer()
 
         package.get_resource("echemdb").data = df_resource.data
 
-        return type(self)(package=package, bibliography=self.bibliography)
+        return type(self)(package=package)
 
     @property
     def df(self):
         r"""
         Return the data of this entry as a data frame.
 
         EXAMPLES::
@@ -346,14 +393,19 @@
         The examples are built on-demand from data in echemdb's examples directory.
 
         EXAMPLES::
 
             >>> Entry.create_examples()
             [Entry('alves_2011_electrochemistry_6010_f1a_solid')]
 
+        An entry without associated BIB file.
+
+            >>> Entry.create_examples(name="no_bibliography")
+            [Entry('no_bibliography')]
+
         """
         source = os.path.join(os.path.dirname(__file__), "..", "examples", name)
 
         if not os.path.exists(source):
             raise ValueError(
                 f"No subdirectory in examples/ for {name}, i.e., could not find {source}."
             )
@@ -365,30 +417,27 @@
             "generated",
             "svgdigitizer",
             name,
         )
 
         cls._digitize_example(source=source, outdir=outdir)
 
-        from echemdb.local import collect_bibliography, collect_datapackages
+        from echemdb.local import collect_datapackages
 
         packages = collect_datapackages(outdir)
-        bibliography = collect_bibliography(source)
-        assert len(bibliography) == 1, f"No bibliography found for {name}."
-        bibliography = next(iter(bibliography))
 
         if len(packages) == 0:
             from glob import glob
 
             raise ValueError(
                 f"No literature data found for {name}. The directory for this data {outdir} exists. But we could not find any datapackages in there. "
                 f"There is probably some outdated data in {outdir}. The contents of that directory are: { glob(os.path.join(outdir,'**')) }"
             )
 
-        return [cls(package=package, bibliography=bibliography) for package in packages]
+        return [cls(package=package) for package in packages]
 
     @classmethod
     def _digitize_example(cls, source, outdir):
         r"""
         Digitize ``source`` and write the output to ``outdir``.
 
         When running tests in parallel, this introduces a race condition that
@@ -412,20 +461,20 @@
                     from svgdigitizer.entrypoint import digitize_cv
                     from svgdigitizer.test.cli import invoke
 
                     invoke(
                         digitize_cv,
                         "--sampling-interval",
                         ".001",
-                        "--package",
                         "--metadata",
                         yaml,
                         svg,
                         "--outdir",
                         outdir,
+                        "--bibliography",
                         "--si-units",
                     )
 
                 assert os.path.exists(
                     outdir
                 ), f"Ran digitizer to generate {outdir}. But directory is still missing after invoking digitizer."
                 assert any(
```

### Comparing `echemdb-0.5.0/echemdb/local.py` & `echemdb-0.6.0/echemdb/local.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
 Utilities to work with local data packages.
 """
 # ********************************************************************
 #  This file is part of echemdb.
 #
-#        Copyright (C) 2021-2022 Albert Engstfeld
+#        Copyright (C) 2021-2023 Albert Engstfeld
 #        Copyright (C)      2021 Johannes Hermann
 #        Copyright (C)      2021 Julian Rüth
 #        Copyright (C)      2021 Nicolas Hörmann
 #
 #  echemdb is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
@@ -29,17 +29,15 @@
     Return a list of data packages defined in the directory `data` and its
     subdirectories.
 
     EXAMPLES::
 
         >>> packages = collect_datapackages("./examples")
         >>> packages[0] # doctest: +NORMALIZE_WHITESPACE
-        {'$frictionless': 'package/v2',
-        'version': '1',
-        'resources': [{'name': 'alves_2011_electrochemistry_6010_f1a_solid',
+        {'resources': [{'name':
         ...
 
     """
     # Collect all datapackage descriptors, see
     # https://specs.frictionlessdata.io/data-package/#metadata
     import os.path
     from glob import glob
@@ -69,29 +67,7 @@
         package.get_resource("echemdb").schema = Schema.from_descriptor(
             package.resources[0].schema.to_dict()
         )
 
         packages.append(package)
 
     return packages
-
-
-def collect_bibliography(bibfiles):
-    r"""
-    Return a list of bibliography data (pybtex) parsed from the bibtex files
-    in the directory `bibfiles` and its subdirectories.
-
-    EXAMPLES::
-
-        >>> bibfiles = collect_bibliography(".")
-
-    """
-    import os.path
-    from glob import glob
-
-    from pybtex.database import parse_file
-
-    return [
-        entry
-        for file in glob(os.path.join(bibfiles, "**", "*.bib"), recursive=True)
-        for entry in parse_file(file, bib_format="bibtex").entries.values()
-    ]
```

### Comparing `echemdb-0.5.0/echemdb/remote.py` & `echemdb-0.6.0/echemdb/remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
 Utilities to work with remote data packages.
 """
 # ********************************************************************
 #  This file is part of echemdb.
 #
-#        Copyright (C)      2021 Albert Engstfeld
+#        Copyright (C) 2021-2023 Albert Engstfeld
 #        Copyright (C)      2021 Johannes Hermann
 #        Copyright (C) 2021-2022 Julian Rüth
 #        Copyright (C)      2021 Nicolas Hörmann
 #
 #  echemdb is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
@@ -79,40 +79,7 @@
             if name.endswith(".json") or name.endswith(".csv")
         ],
     )
 
     import echemdb.local
 
     return echemdb.local.collect_datapackages(os.path.join(outdir, data))
-
-
-@cache
-def collect_bibliography(data=".", url=ECHEMDB_DATABASE_URL, outdir=None):
-    r"""
-    Return a list of bibliography files (bibtex) in a remote location.
-
-    The default is to download the bibliography currently available on echemdb and
-    extract them to a temporary directory.
-
-    EXAMPLES::
-
-        >>> packages = collect_bibliography()  # doctest: +REMOTE_DATA
-
-    """
-    if outdir is None:
-        import atexit
-        import shutil
-        import tempfile
-
-        outdir = tempfile.mkdtemp()
-        atexit.register(shutil.rmtree, outdir)
-
-    compressed = collect_zipfile_from_url(url)
-
-    compressed.extractall(
-        outdir,
-        members=[name for name in compressed.namelist() if name.endswith(".bib")],
-    )
-
-    import echemdb.local
-
-    return echemdb.local.collect_bibliography(os.path.join(outdir, data))
```

### Comparing `echemdb-0.5.0/echemdb.egg-info/PKG-INFO` & `echemdb-0.6.0/echemdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: echemdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: a Python library to work with the echemdb repository
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/echemdb/0.5.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/echemdb/0.6.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6502901.svg)](https://doi.org/10.5281/zenodo.6502901)
 
 The echemdb Python package can interact with a database of
 [frictionless datapackages](https://frictionlessdata.io/)
 containing electrochemical data following [echemdb's metadata schema](https://github.com/echemdb/metadata-schema).
 Such a database can be generated from the data on [echemdb.org](https://www.echemdb.org)
 or from local files.
```

### Comparing `echemdb-0.5.0/setup.py` & `echemdb-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ********************************************************************
 #  This file is part of echemdb.
 #
-#        Copyright (C)      2021 Albert Engstfeld
+#        Copyright (C) 2021-2023 Albert Engstfeld
 #        Copyright (C)      2021 Johannes Hermann
 #        Copyright (C) 2021-2022 Julian Rüth
 #        Copyright (C)      2021 Nicolas Hörmann
 #
 #  echemdb is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
@@ -20,26 +20,26 @@
 #  along with echemdb. If not, see <https://www.gnu.org/licenses/>.
 # ********************************************************************
 
 from distutils.core import setup
 
 setup(
     name='echemdb',
-    version="0.5.0",
+    version="0.6.0",
     packages=['echemdb', 'echemdb.cv'],
     license='GPL 3.0+',
     description="a Python library to work with the echemdb repository",
     long_description=open('README.md', encoding="UTF-8").read(),
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[
       "astropy>=5,<6",
       "filelock>=3,<4",
       "frictionless>=5.10.1,<6",
       "matplotlib>=3.5.0,<4",
       "pandas>=1,<2",
       "plotly>=5,<6",
       "pybtex>=0.24,<0.25",
-      "svgdigitizer>=0.8.0,<0.9.0",
+      "svgdigitizer>=0.10.0,<0.11.0",
     ],
     python_requires=">=3.9",
 )
```

