# Comparing `tmp/chem_templates-0.0.4.tar.gz` & `tmp/chem_templates-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chem_templates-0.0.4.tar", last modified: Wed Mar 22 02:51:13 2023, max compression
+gzip compressed data, was "chem_templates-0.0.5.tar", last modified: Mon Apr 17 16:25:02 2023, max compression
```

## Comparing `chem_templates-0.0.4.tar` & `chem_templates-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.187198 chem_templates-0.0.4/
--rw-r--r--   0 karlheyer   (501) staff       (20)    11337 2023-03-11 06:40:03.000000 chem_templates-0.0.4/LICENSE
--rw-r--r--   0 karlheyer   (501) staff       (20)      201 2023-03-21 20:16:11.000000 chem_templates-0.0.4/MANIFEST.in
--rw-r--r--   0 karlheyer   (501) staff       (20)     1040 2023-03-22 02:51:13.187012 chem_templates-0.0.4/PKG-INFO
--rw-r--r--   0 karlheyer   (501) staff       (20)      239 2023-03-11 06:40:03.000000 chem_templates-0.0.4/README.md
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.163142 chem_templates-0.0.4/chem_templates/
--rw-r--r--   0 karlheyer   (501) staff       (20)       22 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/__init__.py
--rw-r--r--   0 karlheyer   (501) staff       (20)    36606 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/_modidx.py
--rw-r--r--   0 karlheyer   (501) staff       (20)    16925 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/assembly.py
--rw-r--r--   0 karlheyer   (501) staff       (20)    11202 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/building_blocks.py
--rw-r--r--   0 karlheyer   (501) staff       (20)     5388 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/chem.py
--rw-r--r--   0 karlheyer   (501) staff       (20)     7467 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/filter.py
--rw-r--r--   0 karlheyer   (501) staff       (20)     8988 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/fragments.py
--rw-r--r--   0 karlheyer   (501) staff       (20)      366 2023-03-21 06:21:43.000000 chem_templates-0.0.4/chem_templates/imports.py
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.183370 chem_templates-0.0.4/chem_templates/synt_on/
--rw-r--r--   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/synt_on/__init__.py
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.184505 chem_templates-0.0.4/chem_templates/synt_on/config/
--rw-r--r--   0 karlheyer   (501) staff       (20)    52779 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/config/BB_Marks.xml
--rw-r--r--   0 karlheyer   (501) staff       (20)   108462 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/config/SMARTSLibNew.json
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.186314 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/
--rw-r--r--   0 karlheyer   (501) staff       (20)      723 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-heterocycles.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      792 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-lactam.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      830 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Amine_alkylation_arylation.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      231 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Amine_sulphoacylation.json
--rw-r--r--   0 karlheyer   (501) staff       (20)     1065 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/C-C couplings.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      313 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Condensation_of_Y-NH2_with_carbonyl_compounds.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      508 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Metal organics C-C bong assembling.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      987 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/N-acylation.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      594 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/O-acylation.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      726 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/O-alkylation_arylation.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      483 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Olefination.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      535 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Radical_reactions.json
--rw-r--r--   0 karlheyer   (501) staff       (20)      620 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/S-alkylation_arylation.json
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.186844 chem_templates-0.0.4/chem_templates/synt_on/src/
--rw-r--r--   0 karlheyer   (501) staff       (20)    41176 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/src/SyntOn_BBs.py
--rw-r--r--   0 karlheyer   (501) staff       (20)     3848 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/src/SyntOn_Classifier.py
--rw-r--r--   0 karlheyer   (501) staff       (20)    10425 2023-03-11 06:40:03.000000 chem_templates-0.0.4/chem_templates/synt_on/src/UsefulFunctions.py
--rw-r--r--   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/synt_on/src/__init__.py
--rw-r--r--   0 karlheyer   (501) staff       (20)     1880 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/template.py
--rw-r--r--   0 karlheyer   (501) staff       (20)     2247 2023-03-22 02:49:55.000000 chem_templates-0.0.4/chem_templates/utils.py
-drwxr-xr-x   0 karlheyer   (501) staff       (20)        0 2023-03-22 02:51:13.183064 chem_templates-0.0.4/chem_templates.egg-info/
--rw-r--r--   0 karlheyer   (501) staff       (20)     1040 2023-03-22 02:51:13.000000 chem_templates-0.0.4/chem_templates.egg-info/PKG-INFO
--rw-r--r--   0 karlheyer   (501) staff       (20)     1788 2023-03-22 02:51:13.000000 chem_templates-0.0.4/chem_templates.egg-info/SOURCES.txt
--rw-r--r--   0 karlheyer   (501) staff       (20)        1 2023-03-22 02:51:13.000000 chem_templates-0.0.4/chem_templates.egg-info/dependency_links.txt
--rw-r--r--   0 karlheyer   (501) staff       (20)       50 2023-03-22 02:51:13.000000 chem_templates-0.0.4/chem_templates.egg-info/entry_points.txt
--rw-r--r--   0 karlheyer   (501) staff       (20)        1 2023-03-11 06:42:16.000000 chem_templates-0.0.4/chem_templates.egg-info/not-zip-safe
--rw-r--r--   0 karlheyer   (501) staff       (20)       20 2023-03-22 02:51:13.000000 chem_templates-0.0.4/chem_templates.egg-info/requires.txt
--rw-r--r--   0 karlheyer   (501) staff       (20)       15 2023-03-22 02:51:13.000000 chem_templates-0.0.4/chem_templates.egg-info/top_level.txt
--rw-r--r--   0 karlheyer   (501) staff       (20)      876 2023-03-22 02:49:55.000000 chem_templates-0.0.4/settings.ini
--rw-r--r--   0 karlheyer   (501) staff       (20)       38 2023-03-22 02:51:13.187245 chem_templates-0.0.4/setup.cfg
--rw-r--r--   0 karlheyer   (501) staff       (20)     2560 2023-03-11 06:40:03.000000 chem_templates-0.0.4/setup.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    11337 2023-01-20 02:50:04.000000 chem_templates-0.0.5/LICENSE
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      201 2023-04-02 22:59:46.000000 chem_templates-0.0.5/MANIFEST.in
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2632 2023-04-17 16:25:02.215520 chem_templates-0.0.5/PKG-INFO
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1831 2023-04-17 16:19:23.000000 chem_templates-0.0.5/README.md
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/chem_templates/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       22 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/__init__.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    36981 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/_modidx.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    18112 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/assembly.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    12851 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/building_blocks.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     5388 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/chem.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     9161 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/filter.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     8988 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/fragments.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      366 2023-04-02 22:59:46.000000 chem_templates-0.0.5/chem_templates/imports.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/chem_templates/synt_on/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/synt_on/__init__.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/chem_templates/synt_on/config/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    52779 2023-03-06 01:47:51.000000 chem_templates-0.0.5/chem_templates/synt_on/config/BB_Marks.xml
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)   108462 2023-03-06 01:44:44.000000 chem_templates-0.0.5/chem_templates/synt_on/config/SMARTSLibNew.json
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      723 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-heterocycles.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      792 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-lactam.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      830 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Amine_alkylation_arylation.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      231 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Amine_sulphoacylation.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1065 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/C-C couplings.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      313 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Condensation_of_Y-NH2_with_carbonyl_compounds.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      508 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Metal organics C-C bong assembling.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      987 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/N-acylation.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      594 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/O-acylation.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      726 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/O-alkylation_arylation.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      483 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Olefination.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      535 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Radical_reactions.json
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      620 2023-03-05 23:57:01.000000 chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/S-alkylation_arylation.json
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/chem_templates/synt_on/src/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    41176 2023-03-06 01:45:52.000000 chem_templates-0.0.5/chem_templates/synt_on/src/SyntOn_BBs.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3848 2023-03-06 01:45:27.000000 chem_templates-0.0.5/chem_templates/synt_on/src/SyntOn_Classifier.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    10425 2023-03-06 01:45:09.000000 chem_templates-0.0.5/chem_templates/synt_on/src/UsefulFunctions.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/synt_on/src/__init__.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2247 2023-04-17 16:21:09.000000 chem_templates-0.0.5/chem_templates/utils.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-04-17 16:25:02.215520 chem_templates-0.0.5/chem_templates.egg-info/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2632 2023-04-17 16:25:02.000000 chem_templates-0.0.5/chem_templates.egg-info/PKG-INFO
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1761 2023-04-17 16:25:02.000000 chem_templates-0.0.5/chem_templates.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-17 16:25:02.000000 chem_templates-0.0.5/chem_templates.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       50 2023-04-17 16:25:02.000000 chem_templates-0.0.5/chem_templates.egg-info/entry_points.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-02-27 00:41:03.000000 chem_templates-0.0.5/chem_templates.egg-info/not-zip-safe
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       20 2023-04-17 16:25:02.000000 chem_templates-0.0.5/chem_templates.egg-info/requires.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       15 2023-04-17 16:25:02.000000 chem_templates-0.0.5/chem_templates.egg-info/top_level.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      876 2023-04-17 16:21:09.000000 chem_templates-0.0.5/settings.ini
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       38 2023-04-17 16:25:02.215520 chem_templates-0.0.5/setup.cfg
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2560 2023-01-20 02:50:04.000000 chem_templates-0.0.5/setup.py
```

### Comparing `chem_templates-0.0.4/LICENSE` & `chem_templates-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/_modidx.py` & `chem_templates-0.0.5/chem_templates/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
                                                                                                'chem_templates/assembly.py'),
                                          'chem_templates.assembly.AssemblyPool.__init__': ( 'assembly.html#assemblypool.__init__',
                                                                                             'chem_templates/assembly.py'),
                                          'chem_templates.assembly.AssemblyPool.__len__': ( 'assembly.html#assemblypool.__len__',
                                                                                            'chem_templates/assembly.py'),
                                          'chem_templates.assembly.AssemblyPool.__repr__': ( 'assembly.html#assemblypool.__repr__',
                                                                                             'chem_templates/assembly.py'),
+                                         'chem_templates.assembly.AssemblyPool.deduplicate': ( 'assembly.html#assemblypool.deduplicate',
+                                                                                               'chem_templates/assembly.py'),
                                          'chem_templates.assembly.AssemblyPool.filter': ( 'assembly.html#assemblypool.filter',
                                                                                           'chem_templates/assembly.py'),
                                          'chem_templates.assembly.FragmentLeafNode': ( 'assembly.html#fragmentleafnode',
                                                                                        'chem_templates/assembly.py'),
                                          'chem_templates.assembly.FragmentLeafNode.__init__': ( 'assembly.html#fragmentleafnode.__init__',
                                                                                                 'chem_templates/assembly.py'),
                                          'chem_templates.assembly.FragmentLeafNode.assemble': ( 'assembly.html#fragmentleafnode.assemble',
@@ -99,14 +101,16 @@
                                          'chem_templates.assembly.SynthonPool.__init__': ( 'assembly.html#synthonpool.__init__',
                                                                                            'chem_templates/assembly.py'),
                                          'chem_templates.assembly.SynthonPool.filter': ( 'assembly.html#synthonpool.filter',
                                                                                          'chem_templates/assembly.py'),
                                          'chem_templates.assembly.SynthonPool.get_matching': ( 'assembly.html#synthonpool.get_matching',
                                                                                                'chem_templates/assembly.py'),
                                          'chem_templates.assembly.add_rxn': ('assembly.html#add_rxn', 'chem_templates/assembly.py'),
+                                         'chem_templates.assembly.build_synthesis_scheme': ( 'assembly.html#build_synthesis_scheme',
+                                                                                             'chem_templates/assembly.py'),
                                          'chem_templates.assembly.make_assemblies': ( 'assembly.html#make_assemblies',
                                                                                       'chem_templates/assembly.py'),
                                          'chem_templates.assembly.make_pairs': ('assembly.html#make_pairs', 'chem_templates/assembly.py'),
                                          'chem_templates.assembly.make_pairs_chunked': ( 'assembly.html#make_pairs_chunked',
                                                                                          'chem_templates/assembly.py')},
             'chem_templates.building_blocks': { 'chem_templates.building_blocks.FusionReaction': ( 'building_blocks.html#fusionreaction',
                                                                                                    'chem_templates/building_blocks.py'),
@@ -230,14 +234,24 @@
                                        'chem_templates.filter.SmartsFilter': ('filters.html#smartsfilter', 'chem_templates/filter.py'),
                                        'chem_templates.filter.SmartsFilter.__call__': ( 'filters.html#smartsfilter.__call__',
                                                                                         'chem_templates/filter.py'),
                                        'chem_templates.filter.SmartsFilter.__init__': ( 'filters.html#smartsfilter.__init__',
                                                                                         'chem_templates/filter.py'),
                                        'chem_templates.filter.SmartsFilter.has_match': ( 'filters.html#smartsfilter.has_match',
                                                                                          'chem_templates/filter.py'),
+                                       'chem_templates.filter.Template': ('filters.html#template', 'chem_templates/filter.py'),
+                                       'chem_templates.filter.Template.__call__': ( 'filters.html#template.__call__',
+                                                                                    'chem_templates/filter.py'),
+                                       'chem_templates.filter.Template.__init__': ( 'filters.html#template.__init__',
+                                                                                    'chem_templates/filter.py'),
+                                       'chem_templates.filter.Template._empty_result': ( 'filters.html#template._empty_result',
+                                                                                         'chem_templates/filter.py'),
+                                       'chem_templates.filter.TemplateResult': ('filters.html#templateresult', 'chem_templates/filter.py'),
+                                       'chem_templates.filter.TemplateResult.__init__': ( 'filters.html#templateresult.__init__',
+                                                                                          'chem_templates/filter.py'),
                                        'chem_templates.filter.ValidityFilter': ('filters.html#validityfilter', 'chem_templates/filter.py'),
                                        'chem_templates.filter.ValidityFilter.__call__': ( 'filters.html#validityfilter.__call__',
                                                                                           'chem_templates/filter.py'),
                                        'chem_templates.filter.ValidityFilter.__init__': ( 'filters.html#validityfilter.__init__',
                                                                                           'chem_templates/filter.py')},
             'chem_templates.fragments': { 'chem_templates.fragments.add_fragment_mapping': ( 'fragments.html#add_fragment_mapping',
                                                                                              'chem_templates/fragments.py'),
@@ -264,21 +278,10 @@
                                                                                                 'chem_templates/fragments.py'),
                                           'chem_templates.fragments.shred_smiles': ( 'fragments.html#shred_smiles',
                                                                                      'chem_templates/fragments.py')},
             'chem_templates.imports': {},
             'chem_templates.synt_on.src.SyntOn_BBs': {},
             'chem_templates.synt_on.src.SyntOn_Classifier': {},
             'chem_templates.synt_on.src.UsefulFunctions': {},
-            'chem_templates.template': { 'chem_templates.template.Template': ('template.html#template', 'chem_templates/template.py'),
-                                         'chem_templates.template.Template.__call__': ( 'template.html#template.__call__',
-                                                                                        'chem_templates/template.py'),
-                                         'chem_templates.template.Template.__init__': ( 'template.html#template.__init__',
-                                                                                        'chem_templates/template.py'),
-                                         'chem_templates.template.Template._empty_result': ( 'template.html#template._empty_result',
-                                                                                             'chem_templates/template.py'),
-                                         'chem_templates.template.TemplateResult': ( 'template.html#templateresult',
-                                                                                     'chem_templates/template.py'),
-                                         'chem_templates.template.TemplateResult.__init__': ( 'template.html#templateresult.__init__',
-                                                                                              'chem_templates/template.py')},
             'chem_templates.utils': { 'chem_templates.utils.deduplicate_list': ('utils.html#deduplicate_list', 'chem_templates/utils.py'),
                                       'chem_templates.utils.flatten_list': ('utils.html#flatten_list', 'chem_templates/utils.py'),
                                       'chem_templates.utils.validate_range': ('utils.html#validate_range', 'chem_templates/utils.py')}}}
```

### Comparing `chem_templates-0.0.4/chem_templates/assembly.py` & `chem_templates-0.0.5/chem_templates/assembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_assembly.ipynb.
 
 # %% ../nbs/06_assembly.ipynb 3
 from __future__ import annotations
 from .imports import *
 from .utils import *
 from .chem import Molecule, to_smile
-from .template import Template, TemplateResult
+from .filter import Template, TemplateResult
 from .fragments import combine_dummies, get_dummy_mol, generate_mapping_permutations,\
 match_mapping, fuse_smile_on_atom_mapping
-from .building_blocks import Synthon, ReactionUniverse, REACTION_GROUPS
+from .building_blocks import Synthon, ReactionUniverse, REACTION_GROUPS, molecule_to_synthon
 
 # %% auto 0
 __all__ = ['AssemblyPool', 'AssemblyInputs', 'Node', 'FragmentNode', 'FragmentLeafNode', 'SynthonPool', 'make_pairs',
-           'make_pairs_chunked', 'add_rxn', 'make_assemblies', 'SynthonNode', 'SynthonLeafNode']
+           'make_pairs_chunked', 'add_rxn', 'make_assemblies', 'SynthonNode', 'SynthonLeafNode',
+           'build_synthesis_scheme']
 
 # %% ../nbs/06_assembly.ipynb 4
 class AssemblyPool():
     def __init__(self, items: list[Molecule]):
         self.items = items
         
     def __len__(self) -> int:
@@ -30,14 +31,21 @@
             bools = worker_pool.map(filter_func, self.items)
             
         else:
             bools = [filter_func(i) for i in self.items]
             
         return AssemblyPool([self.items[i] for i in range(len(self.items)) if bools[i]])
     
+    def deduplicate(self, key_func: Callable) -> AssemblyPool:
+        item_dict = {}
+        for item in self.items:
+            item_dict[key_func(item)] = item
+        
+        return AssemblyPool(list(item_dict.values()))
+    
     def __repr__(self) -> str:
         return f'AssemblyPool: {len(self.items)} items'
 
 # %% ../nbs/06_assembly.ipynb 6
 class AssemblyInputs():
     def __init__(self, 
                  pool_dict: dict[str, AssemblyPool], 
@@ -180,17 +188,20 @@
             'source' : self.name,
             'source_molecules' : fusion_inputs,
             'input_smiles' : fusion_string
         }
         molecule = Molecule(fused_smile, data=fusion_data)
         return molecule
     
-    def assemble(self, assembly_inputs: AssemblyInputs) -> AssemblyPool:
-        child_pools = [child.assemble(assembly_inputs) for child in self.children]
-        print(self.name)
+    def assemble(self, assembly_inputs: AssemblyInputs, verbose:bool=False) -> AssemblyPool:
+        child_pools = [child.assemble(assembly_inputs, verbose=verbose) for child in self.children]
+        
+        if verbose:
+            print(self.name)
+            
         outputs = []
         assembly_iterator = self.assembly_iterator(child_pools, assembly_inputs.assembly_chunksize)
         
         for fusion_inputs in assembly_iterator:
             fused_pool = self.fuse(fusion_inputs, assembly_inputs.worker_pool)
             fused_pool = fused_pool.filter(self.template_screen, worker_pool=assembly_inputs.worker_pool)
             outputs += fused_pool.items
@@ -230,16 +241,17 @@
         self.mapping_idxs = sorted(mapping_idxs)
         super().__init__(name, [], template)
         
     def build_dummy(self):
         self.dummy = get_dummy_mol(self.name, self.mapping_idxs, id=self.id)
         self.dummy_smile = to_smile(self.dummy)
         
-    def assemble(self, assembly_inputs: AssemblyInputs) -> AssemblyPool:
-        print(self.name)
+    def assemble(self, assembly_inputs: AssemblyInputs, verbose:bool=False) -> AssemblyPool:
+        if verbose:
+            print(self.name)
         pool = assembly_inputs.pool_dict[self.name]
         pool = pool.filter(self.template_screen, worker_pool=assembly_inputs.worker_pool)
         return pool
 
 # %% ../nbs/06_assembly.ipynb 10
 class SynthonPool(AssemblyPool):
     def __init__(self, items: list[Synthon]):
@@ -400,22 +412,23 @@
              worker_pool: Optional[Pool]=None) -> SynthonPool:
         if worker_pool:
             outputs = worker_pool.map(self._fuse, fusion_inputs)
         else:
             outputs = [self._fuse(i) for i in fusion_inputs]
         return SynthonPool(flatten_list(outputs))
     
-    def assemble(self, assembly_inputs: AssemblyInputs) -> SynthonPool:
-        incoming_pool = self.incoming_node.assemble(assembly_inputs)
+    def assemble(self, assembly_inputs: AssemblyInputs, verbose:bool=False) -> SynthonPool:
+        incoming_pool = self.incoming_node.assemble(assembly_inputs, verbose=verbose)
         incoming_pool = incoming_pool.filter(self.reaction_screen, assembly_inputs.worker_pool)
         
-        next_pool = self.next_node.assemble(assembly_inputs)
+        next_pool = self.next_node.assemble(assembly_inputs, verbose=verbose)
         next_pool = next_pool.filter(self.reaction_screen, assembly_inputs.worker_pool)
         
-        print(self.name)
+        if verbose:
+            print(self.name)
         
         outputs = []
         
         assembly_generator = make_assemblies(incoming_pool, next_pool, self.rxn_universe,
                                             assembly_inputs.assembly_chunksize, assembly_inputs.worker_pool)
         
         for assemblies in assembly_generator:
@@ -440,15 +453,34 @@
 class SynthonLeafNode(SynthonNode):
     def __init__(self, 
                  name: str, 
                  n_func: set[int], 
                  template: Optional[Template]=None):
         super().__init__(name, None, None, None, n_func, template)
         
-    def assemble(self, assembly_inputs: AssemblyInputs) -> SynthonPool:
-        print(self.name)
+    def assemble(self, assembly_inputs: AssemblyInputs, verbose:bool=False) -> SynthonPool:
+        if verbose:
+            print(self.name)
         pool = assembly_inputs.pool_dict[self.name]
         pool = pool.filter(self.template_screen, worker_pool=assembly_inputs.worker_pool)
         return pool
     
     def __repr__(self) -> str:
         return f'Synthon Leaf: {self.name}'
+
+# %% ../nbs/06_assembly.ipynb 14
+def build_synthesis_scheme(synthon: Synthon) -> dict:
+    output = {}
+    
+    if 'parents' in synthon.data:
+        if isinstance(synthon.data['parents'][0], Synthon):
+            for i, parent in enumerate(synthon.data['parents']):
+                output['smile'] = synthon.smile
+                output['reaction_tags'] = synthon.data['reaction_tags']
+                output[f'reactant_{i}'] = build_synthesis_scheme(parent)
+            
+        else:
+            parent = synthon.data['parents'][0]
+            output['smile'] = parent.smile
+            output['data'] = parent.data
+            
+    return output
```

### Comparing `chem_templates-0.0.4/chem_templates/building_blocks.py` & `chem_templates-0.0.5/chem_templates/building_blocks.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,35 @@
 
 # %% auto 0
 __all__ = ['SYNTHON_VALID_COMBINATIONS', 'REACTION_GROUP_NAMES', 'FUSION_REACTION_PATH', 'REACTION_GROUPS', 'REACTION_GROUP_DICT',
            'smile_to_synthon', 'get_synthon_marks', 'add_reconstruction_atoms', 'remove_reconstruction_atoms',
            'Synthon', 'molecule_to_synthon', 'FusionReaction', 'ReactionGroup', 'ReactionUniverse']
 
 # %% ../nbs/05_building_blocks.ipynb 4
-def smile_to_synthon(smile: str, 
-                     keep_pg: bool=False) -> Tuple[list[str], list[list[str]]]:
+def smile_to_synthon(smile: str, # smiles string to convert
+                     keep_pg: bool=False # if True, results include synthons with un-removed protecting groups
+            ) -> Tuple[list[str], list[list[str]]]: # Returns paired list of SMILES and reaction classes
+
     classes = BBClassifier(mol=to_mol(smile))
     
     azoles,fSynt = mainSynthonsGenerator(smile, keep_pg, classes, returnBoolAndDict=True)
 
     smiles = list(fSynt.keys())
     rxns = list(fSynt.values())
     rxns = [list(i) for i in rxns]
     return smiles, rxns
 
 # %% ../nbs/05_building_blocks.ipynb 6
-def get_synthon_marks(smile: str) -> list[str]:
+def get_synthon_marks(smile: str # input synthon smiles string
+                     ) -> list[str]: # list of marks
+    '''
+    extracts reaction tag marks from synthon
+    
+    ie `'CC1(C)CC(N[CH:10]=O)CC(C)(CNC(=O)NCc2cc([CH:10]=O)ccn2)C1' -> ['C:10']`
+    '''
     pat = re.compile("\[\w*:\w*\]")
     current_marks = [smile[m.start() + 1] + ":" + smile[m.end() - 3:m.end() - 1]
                     for m in re.finditer(pat, smile)]
     return deduplicate_list(current_marks)
 
 # %% ../nbs/05_building_blocks.ipynb 8
 SYNTHON_VALID_COMBINATIONS = {'C:10': ['N:20', 'O:20', 'C:20', 'c:20', 'n:20', 'S:20'],
@@ -55,16 +63,18 @@
                               'C:50': ['C:50'], 
                               'C:70': ['C:60', 'c:60'],
                               'c:60':['C:70'], 
                               'C:60': ['C:70'], 
                               'N:40': ['C:30'] }
 
 # %% ../nbs/05_building_blocks.ipynb 9
-def add_reconstruction_atoms(smile: str) -> str:
-    # augments synthon annotations (ie c:10) with dummy atoms for fusion
+def add_reconstruction_atoms(smile: str # synthon smiles string
+                            ) -> str: # synthon reconstruction string
+    
+    'augments synthon annotations (ie c:10) with dummy atoms for fusion'
     labels = [10, 20, 30, 40, 50, 60, 70, 21, 11] # annotation numbers
     atomsForMarking = [23, 74, 72, 104, 105, 106, 107, 108, 109] # dummy atoms
     atomsForMarkingForDoubleBonds = [72, 104, 105]
     
     mol = to_mol(smile)
     mol = Chem.AddHs(mol)
     
@@ -80,16 +90,17 @@
                         break
                     elif replCount == 2:
                         break
                         
     mol = Chem.RemoveHs(mol)
     return to_smile(mol)
 
-def remove_reconstruction_atoms(smile: str) -> str:
-    # removes dummy atoms for fusion
+def remove_reconstruction_atoms(smile: str # synthon reconstruction string
+                               ) -> str: # synthon smiles string
+    'removes dummy atoms for fusion'
     atomsForMarking = set([23, 74, 72, 104, 105, 106, 107, 108, 109])
     mol = to_mol(smile)
     
     for atom in mol.GetAtoms():
         if atom.GetAtomicNum() in atomsForMarking:
             atom.SetAtomicNum(1)
             
@@ -97,57 +108,61 @@
     mol = Chem.RemoveHs(mol)
             
     return to_smile(mol)
 
 # %% ../nbs/05_building_blocks.ipynb 11
 class Synthon(Molecule):
     def __init__(self,
-                 synthon_smile: str,
-                 reaction_tags: list[str]=None,
-                 parents: Optional[list[Molecule]]=None,
-                 data: Optional[dict]=None
+                 synthon_smile: str, # synthon smiles string
+                 reaction_tags: list[str]=None, # reaction class tags
+                 parents: Optional[list[Molecule]]=None, # parent molecule
+                 data: Optional[dict]=None # data
                 ):
         super().__init__(synthon_smile, data)
         
         if parents:
             self.add_data({'parents' : parents})
             
         if reaction_tags:
             self.add_data({'reaction_tags' : reaction_tags})
             
         self.recon_smile = add_reconstruction_atoms(synthon_smile)
         self.recon_mol = to_mol(self.recon_smile)
         self.marks = set(get_synthon_marks(self.recon_smile))
-        self.compatible_marks = set(flatten_list([SYNTHON_VALID_COMBINATIONS[i] for i in self.marks]))
+        self.compatible_marks = set(flatten_list([SYNTHON_VALID_COMBINATIONS.get(i, []) for i in self.marks]))
         
     def is_compatible(self, synthon: Synthon) -> bool:
         overlaps = self.compatible_marks.intersection(synthon.marks)
         return bool(overlaps)
 
 # %% ../nbs/05_building_blocks.ipynb 12
-def molecule_to_synthon(molecule: Molecule) -> list[Synthon]:
+def molecule_to_synthon(molecule: Molecule # input Molecule
+                       ) -> list[Synthon]: # output list of synthons
+    'Converts `molecule` into a list of corresponding synthons'
     synthon_smiles, rxn_tags = smile_to_synthon(molecule.smile)
     outputs = []
     for i in range(len(synthon_smiles)):
         outputs.append(Synthon(synthon_smiles[i], rxn_tags[i], [molecule]))
     return outputs
 
 # %% ../nbs/05_building_blocks.ipynb 14
 class FusionReaction():
     def __init__(self, 
-                 name: str, 
-                 rxn_smarts: str):
+                 name: str, # reaction name
+                 rxn_smarts: str # reaction smarts
+                ):
         self.name = name
         self.rxn_smarts = rxn_smarts
         self.rxn = Reactions.ReactionFromSmarts(rxn_smarts)
         self.rxn.Initialize()
         
     def is_reactant(self, 
-                    synthon1: Synthon, 
-                    synthon2: Optional[Synthon]=None) -> bool:
+                    synthon1: Synthon, # first reactant
+                    synthon2: Optional[Synthon]=None # second reactant
+                   ) -> bool: # bool, True if synthons match reaction pattern
         
         if synthon2 is None:
             output = self.rxn.IsMoleculeReactant(synthon1.recon_mol)
         else:
             reactants = self.rxn.GetReactants()
             try:
                 order1 = [synthon1.recon_mol.HasSubstructMatch(reactants[0]),
@@ -159,16 +174,17 @@
                 output = all(order1) or all(order2)
             except:
                 output = False
             
         return output
     
     def _react(self, 
-               synthon1: Synthon, 
-               synthon2: Synthon) -> list[str]:
+               synthon1: Synthon, # first reactant
+               synthon2: Synthon # second reactant
+              ) -> list[str]: # list of product SMILES strings
         products = self.rxn.RunReactants((synthon1.recon_mol, 
                                           synthon2.recon_mol))
         if not products:
             products = self.rxn.RunReactants((synthon2.recon_mol, 
                                           synthon1.recon_mol))
 
         if products:
@@ -176,27 +192,29 @@
         else:
             products = []
             
         products = [to_smile(i) for i in products]
         return products
     
     def react(self, 
-              synthon1: Synthon, 
-              synthon2: Synthon) -> list[Synthon]:
+              synthon1: Synthon, # synthon reactant 1
+              synthon2: Synthon # synthon reactant 2
+             ) -> list[Synthon]: # list of product synthons
         products = self._react(synthon1, synthon2)
         outputs = []
         for recon_smile in products:
             synthon_smile = remove_reconstruction_atoms(recon_smile)
             result = Synthon(synthon_smile, reaction_tags=[self.name], parents=[synthon1, synthon2])
             outputs.append(result)
         return outputs
     
     def react_to_dict(self, 
-                      synthon1: Synthon, 
-                      synthon2: Synthon) -> list[dict]:
+                      synthon1: Synthon, # synthon reactant 1
+                      synthon2: Synthon # synthon reactant 2
+                     ) -> list[dict]: # dictionary of product synthon strings
         products = self._react(synthon1, synthon2)
         outputs = []
         for recon_smile in products:
             synthon_smile = remove_reconstruction_atoms(recon_smile)
             
             result = {
                 'synthon_smile' : synthon_smile,
@@ -207,24 +225,29 @@
         return outputs
     
     def __repr__(self) -> str:
         return f'Reaction: {self.name}'
 
 # %% ../nbs/05_building_blocks.ipynb 15
 class ReactionGroup():
-    # holds reactions beloning to the same type of transform
+    'holds reactions beloning to the same type of transform'
     def __init__(self, 
-                 name: str, 
-                 reactions: list[FusionReaction]):
+                 name: str, # group name
+                 reactions: list[FusionReaction] # list of reactions in group
+                ):
         self.name = name
         self.reactions = reactions
         
     def get_matching_reactions(self, 
-                               synthon1: Synthon, 
-                               synthon2: Optional[Synthon]=None) -> list[FusionReaction]:
+                               synthon1: Synthon, # first synthon reactant
+                               synthon2: Optional[Synthon]=None # second synthon reactant 
+                              ) -> list[FusionReaction]: # list of matching reactions
+        '''
+        checks input synthons against `self.reactions` and returns matches
+        '''
         return [i for i in self.reactions if i.is_reactant(synthon1, synthon2)]
     
     def dump(self) -> dict:
         output = {
             'name' : self.name,
             'reactions' : [
                 {'name' : i.name, 'smarts' : i.rxn_smarts} for i in self.reactions
@@ -245,27 +268,30 @@
     
     def __repr__(self):
         return f'Reaction Class: {self.name}' + '\n\t' + '\n\t'.join([i.__repr__() for i in self.reactions])
 
 # %% ../nbs/05_building_blocks.ipynb 16
 class ReactionUniverse():
     def __init__(self, 
-                 name: str, 
-                 reaction_groups: list[ReactionGroup]):
+                 name: str, # rxn universe name
+                 reaction_groups: list[ReactionGroup] # list of reaction groups
+                ):
         self.name = name
         self.reaction_groups = reaction_groups
         self.reaction_groups_dict = {i.name : i for i in self.reaction_groups}
         
-    def add_group(self, reaction_group: ReactionGroup):
+    def add_group(self, reaction_group: ReactionGroup # group to add
+                 ):
         self.reaction_groups.append(reaction_group)
         self.reaction_groups_dict[reaction_group.name] = reaction_group
         
     def get_matching_reactions(self, 
-                               synthon1: Synthon, 
-                               synthon2: Optional[Synthon]=None) -> list[FusionReaction]:
+                               synthon1: Synthon, # synthon reactant 1
+                               synthon2: Optional[Synthon]=None # synthon reactant 2
+                              ) -> list[FusionReaction]: # list of matching reactions
         outputs = []
         for group in self.reaction_groups:
             outputs += group.get_matching_reactions(synthon1, synthon2)
         return outputs
 
 # %% ../nbs/05_building_blocks.ipynb 17
 REACTION_GROUP_NAMES = ['O-acylation',
```

### Comparing `chem_templates-0.0.4/chem_templates/chem.py` & `chem_templates-0.0.5/chem_templates/chem.py`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/filter.py` & `chem_templates-0.0.5/chem_templates/filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_filters.ipynb.
 
 # %% auto 0
 __all__ = ['FilterResult', 'Filter', 'ValidityFilter', 'SingleCompoundFilter', 'AttachmentCountFilter', 'BinaryFunctionFilter',
-           'DataFunctionFilter', 'RangeFunctionFilter', 'SmartsFilter', 'CatalogFilter']
+           'DataFunctionFilter', 'RangeFunctionFilter', 'SmartsFilter', 'CatalogFilter', 'TemplateResult', 'Template']
 
 # %% ../nbs/02_filters.ipynb 3
 from .imports import *
 from .utils import *
 from .chem import Molecule, Catalog, mol_func_wrapper
 from rdkit.Chem.FilterCatalog import SmartsMatcher
+from rdkit.Chem import rdMolDescriptors, Descriptors
 
 # %% ../nbs/02_filters.ipynb 4
 class FilterResult():
     'Container for filter results'
     def __init__(self, 
                  filter_result: bool, # overall filter result (True or False)
                  filter_name:   str,  # name of filter
@@ -193,7 +194,52 @@
         
     def __call__(self, molecule: Molecule) -> FilterResult:
         has_match = self.has_match(molecule)
         result = not has_match if self.exclude else has_match
         data = {'filter_result' : has_match}
         
         return FilterResult(result, self.name, data)
+
+# %% ../nbs/02_filters.ipynb 17
+class TemplateResult():
+    'Container for template results'
+    def __init__(self, 
+                 result:         bool, # overall pass/fail result
+                 filter_results: list[bool], # pass/fail from individual filters
+                 filter_data:    list[Union[FilterResult, None]] # filter data from individual filters
+                ):
+        
+        self.result = result
+        self.filter_results = filter_results
+        self.filter_data = filter_data
+
+class Template():
+    '''
+    `Template` holds a list of filters and screens a molecule against all of them
+    '''
+    def __init__(self, filters: list[Filter] # list of filters
+                ):
+        self.filters = filters
+        
+    def _empty_result(self):
+        filter_results = [False for i in self.filters]
+        filter_data = [None for i in self.filters]
+        
+        return TemplateResult(False, filter_results, filter_data)
+        
+    def __call__(self, 
+                 molecule: Molecule, # input molecule
+                 early_exit: bool=True # if True, early exits on first failed filter
+                ) -> TemplateResult: # output template results
+        results = self._empty_result()
+        
+        for i, f in enumerate(self.filters):
+            res = f(molecule)
+            results.filter_results[i] = res.filter_result
+            results.filter_data[i] = res
+
+            if (not res.filter_result) and early_exit:
+                break
+                
+        results.result = all(results.filter_results)
+                        
+        return results
```

### Comparing `chem_templates-0.0.4/chem_templates/fragments.py` & `chem_templates-0.0.5/chem_templates/fragments.py`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/config/BB_Marks.xml` & `chem_templates-0.0.5/chem_templates/synt_on/config/BB_Marks.xml`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/config/SMARTSLibNew.json` & `chem_templates-0.0.5/chem_templates/synt_on/config/SMARTSLibNew.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-heterocycles.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-heterocycles.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-lactam.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Alkylation_arylation_of_NH-lactam.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Amine_alkylation_arylation.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Amine_alkylation_arylation.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/C-C couplings.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/C-C couplings.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/N-acylation.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/N-acylation.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/O-acylation.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/O-acylation.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/O-alkylation_arylation.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/O-alkylation_arylation.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/Radical_reactions.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/Radical_reactions.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/fusion_reactions/S-alkylation_arylation.json` & `chem_templates-0.0.5/chem_templates/synt_on/fusion_reactions/S-alkylation_arylation.json`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/src/SyntOn_BBs.py` & `chem_templates-0.0.5/chem_templates/synt_on/src/SyntOn_BBs.py`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/src/SyntOn_Classifier.py` & `chem_templates-0.0.5/chem_templates/synt_on/src/SyntOn_Classifier.py`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/synt_on/src/UsefulFunctions.py` & `chem_templates-0.0.5/chem_templates/synt_on/src/UsefulFunctions.py`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates/utils.py` & `chem_templates-0.0.5/chem_templates/utils.py`

 * *Files identical despite different names*

### Comparing `chem_templates-0.0.4/chem_templates.egg-info/SOURCES.txt` & `chem_templates-0.0.5/chem_templates.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 chem_templates/_modidx.py
 chem_templates/assembly.py
 chem_templates/building_blocks.py
 chem_templates/chem.py
 chem_templates/filter.py
 chem_templates/fragments.py
 chem_templates/imports.py
-chem_templates/template.py
 chem_templates/utils.py
 chem_templates.egg-info/PKG-INFO
 chem_templates.egg-info/SOURCES.txt
 chem_templates.egg-info/dependency_links.txt
 chem_templates.egg-info/entry_points.txt
 chem_templates.egg-info/not-zip-safe
 chem_templates.egg-info/requires.txt
```

### Comparing `chem_templates-0.0.4/settings.ini` & `chem_templates-0.0.5/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = chem_templates
 lib_name = chem_templates
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = chem_templates
 nbs_path = nbs
 recursive = True
```

### Comparing `chem_templates-0.0.4/setup.py` & `chem_templates-0.0.5/setup.py`

 * *Files identical despite different names*

