# Comparing `tmp/phenospy-0.12.tar.gz` & `tmp/phenospy-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenospy-0.12.tar", last modified: Mon Apr  3 19:30:08 2023, max compression
+gzip compressed data, was "phenospy-0.13.tar", last modified: Mon Apr 17 16:05:41 2023, max compression
```

## Comparing `phenospy-0.12.tar` & `phenospy-0.13.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 taravser (1128288419) 984178727        0 2023-04-03 19:30:08.787028 phenospy-0.12/
--rw-r--r--   0 taravser (1128288419) 984178727     1080 2023-03-13 19:55:04.000000 phenospy-0.12/LICENSE.txt
--rw-r--r--   0 taravser (1128288419) 984178727       31 2023-03-13 20:40:28.000000 phenospy-0.12/MANIFEST.in
--rw-r--r--   0 taravser (1128288419) 984178727     4126 2023-04-03 19:30:08.786651 phenospy-0.12/PKG-INFO
--rw-r--r--   0 taravser (1128288419) 984178727     3281 2023-04-03 19:28:48.000000 phenospy-0.12/README.md
-drwxr-xr-x   0 taravser (1128288419) 984178727        0 2023-04-03 19:30:08.762610 phenospy-0.12/phenospy/
--rw-r--r--   0 taravser (1128288419) 984178727      370 2023-04-03 16:35:02.000000 phenospy-0.12/phenospy/__init__.py
--rw-r--r--   0 taravser (1128288419) 984178727    18762 2023-04-03 16:08:26.000000 phenospy-0.12/phenospy/nl_fun.py
--rw-r--r--   0 taravser (1128288419) 984178727     1109 2023-04-03 16:31:49.000000 phenospy-0.12/phenospy/nl_owlToMd.py
--rw-r--r--   0 taravser (1128288419) 984178727     2258 2023-04-03 16:50:14.000000 phenospy-0.12/phenospy/nl_owlToMd_fun.py
--rw-r--r--   0 taravser (1128288419) 984178727     2403 2023-03-28 14:23:07.000000 phenospy-0.12/phenospy/owl_make_phsOntology.py
--rw-r--r--   0 taravser (1128288419) 984178727      631 2023-03-28 17:14:38.000000 phenospy-0.12/phenospy/owl_owlready_config.py
--rw-r--r--   0 taravser (1128288419) 984178727     4013 2023-03-28 18:24:24.000000 phenospy-0.12/phenospy/owl_xml2owl_fun.py
--rw-r--r--   0 taravser (1128288419) 984178727    16670 2023-03-31 12:43:13.000000 phenospy-0.12/phenospy/owl_xmlToOwl.py
-drwxr-xr-x   0 taravser (1128288419) 984178727        0 2023-04-03 19:30:08.785447 phenospy-0.12/phenospy/package-data/
--rw-r--r--   0 taravser (1128288419) 984178727     6148 2023-03-28 19:11:16.000000 phenospy-0.12/phenospy/package-data/.DS_Store
--rw-r--r--   0 taravser (1128288419) 984178727      591 2023-03-27 19:35:46.000000 phenospy-0.12/phenospy/package-data/phenoscript.obda
--rw-r--r--   0 taravser (1128288419) 984178727    18495 2023-03-27 19:35:46.000000 phenospy-0.12/phenospy/package-data/phenoscript.owl
--rw-r--r--   0 taravser (1128288419) 984178727      127 2023-03-27 19:35:46.000000 phenospy-0.12/phenospy/package-data/phenoscript.properties
--rw-r--r--   0 taravser (1128288419) 984178727     2691 2023-03-24 22:15:59.000000 phenospy-0.12/phenospy/package-data/phs-config.yaml
--rw-r--r--   0 taravser (1128288419) 984178727     7502 2023-03-27 17:52:38.000000 phenospy-0.12/phenospy/package-data/snippets-default.json
--rw-r--r--   0 taravser (1128288419) 984178727     1065 2023-03-15 14:43:16.000000 phenospy-0.12/phenospy/phs_addXmlMeta.py
--rw-r--r--   0 taravser (1128288419) 984178727     5390 2023-03-28 18:02:16.000000 phenospy-0.12/phenospy/phs_grammar.py
--rw-r--r--   0 taravser (1128288419) 984178727     2232 2023-03-28 18:15:48.000000 phenospy-0.12/phenospy/phs_mainConvert.py
--rw-r--r--   0 taravser (1128288419) 984178727     3898 2023-03-28 18:28:37.000000 phenospy-0.12/phenospy/phs_parser_fun.py
--rw-r--r--   0 taravser (1128288419) 984178727     3153 2023-03-28 18:28:31.000000 phenospy-0.12/phenospy/phs_various_fun.py
--rw-r--r--   0 taravser (1128288419) 984178727    14872 2023-03-28 18:12:47.000000 phenospy-0.12/phenospy/phs_xml.py
--rw-r--r--   0 taravser (1128288419) 984178727     6508 2023-03-28 18:13:03.000000 phenospy-0.12/phenospy/phs_xmlTranslateTerms.py
--rw-r--r--   0 taravser (1128288419) 984178727     7009 2023-03-28 17:14:38.000000 phenospy-0.12/phenospy/snips_fun.py
--rw-r--r--   0 taravser (1128288419) 984178727    10935 2023-03-28 18:13:20.000000 phenospy-0.12/phenospy/snips_makeFromYaml.py
--rw-r--r--   0 taravser (1128288419) 984178727     5201 2023-03-28 18:13:28.000000 phenospy-0.12/phenospy/snips_readFromJSON.py
--rw-r--r--   0 taravser (1128288419) 984178727     2224 2023-03-28 18:13:34.000000 phenospy-0.12/phenospy/xml_recodeThis.py
-drwxr-xr-x   0 taravser (1128288419) 984178727        0 2023-04-03 19:30:08.772986 phenospy-0.12/phenospy.egg-info/
--rw-r--r--   0 taravser (1128288419) 984178727     4126 2023-04-03 19:30:08.000000 phenospy-0.12/phenospy.egg-info/PKG-INFO
--rw-r--r--   0 taravser (1128288419) 984178727      944 2023-04-03 19:30:08.000000 phenospy-0.12/phenospy.egg-info/SOURCES.txt
--rw-r--r--   0 taravser (1128288419) 984178727        1 2023-04-03 19:30:08.000000 phenospy-0.12/phenospy.egg-info/dependency_links.txt
--rw-r--r--   0 taravser (1128288419) 984178727       43 2023-04-03 19:30:08.000000 phenospy-0.12/phenospy.egg-info/requires.txt
--rw-r--r--   0 taravser (1128288419) 984178727        9 2023-04-03 19:30:08.000000 phenospy-0.12/phenospy.egg-info/top_level.txt
--rw-r--r--   0 taravser (1128288419) 984178727       38 2023-04-03 19:30:08.787137 phenospy-0.12/setup.cfg
--rw-r--r--   0 taravser (1128288419) 984178727     1238 2023-04-03 16:40:32.000000 phenospy-0.12/setup.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:05:41.547907 phenospy-0.13/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.13/LICENSE.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.13/MANIFEST.in
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3666 2023-04-17 16:05:41.547721 phenospy-0.13/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2821 2023-04-17 14:30:21.000000 phenospy-0.13/README.md
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:05:41.544723 phenospy-0.13/phenospy/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.13/phenospy/__init__.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18762 2023-04-03 16:08:26.000000 phenospy-0.13/phenospy/nl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.13/phenospy/nl_owlToMd.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.13/phenospy/nl_owlToMd_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.13/phenospy/owl_make_phsOntology.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.13/phenospy/owl_owlready_config.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.13/phenospy/owl_xml2owl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16700 2023-04-17 06:49:33.000000 phenospy-0.13/phenospy/owl_xmlToOwl.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:05:41.547471 phenospy-0.13/phenospy/package-data/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.13/phenospy/package-data/.DS_Store
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.13/phenospy/package-data/phenoscript.obda
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.13/phenospy/package-data/phenoscript.owl
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.13/phenospy/package-data/phenoscript.properties
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2690 2023-04-17 08:10:21.000000 phenospy-0.13/phenospy/package-data/phs-config.yaml
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.13/phenospy/package-data/snippets-default.json
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.13/phenospy/phs_addXmlMeta.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.13/phenospy/phs_grammar.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.13/phenospy/phs_mainConvert.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.13/phenospy/phs_parser_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.13/phenospy/phs_various_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.13/phenospy/phs_xml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.13/phenospy/phs_xmlTranslateTerms.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.13/phenospy/snips_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10935 2023-03-28 18:13:20.000000 phenospy-0.13/phenospy/snips_makeFromYaml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5201 2023-03-28 18:13:28.000000 phenospy-0.13/phenospy/snips_readFromJSON.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.13/phenospy/xml_recodeThis.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:05:41.545995 phenospy-0.13/phenospy.egg-info/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3666 2023-04-17 16:05:41.000000 phenospy-0.13/phenospy.egg-info/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-04-17 16:05:41.000000 phenospy-0.13/phenospy.egg-info/SOURCES.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-04-17 16:05:41.000000 phenospy-0.13/phenospy.egg-info/dependency_links.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-04-17 16:05:41.000000 phenospy-0.13/phenospy.egg-info/requires.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-04-17 16:05:41.000000 phenospy-0.13/phenospy.egg-info/top_level.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-04-17 16:05:41.547962 phenospy-0.13/setup.cfg
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-04-17 16:05:32.000000 phenospy-0.13/setup.py
```

### Comparing `phenospy-0.12/LICENSE.txt` & `phenospy-0.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/PKG-INFO` & `phenospy-0.13/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.12
+Version: 0.13
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,15 @@
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/phenospy?color=blue&label=PyPI%20Downloads)
 
 # Phenospy (= Phenoscript Python tools)
 
  <p align="left">
   <img src="https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/phenospy.png" width="300" title="Phenospy logo">
+  <img src="https://raw.githubusercontent.com/sergeitarasov/vscode-phenoscript/main/icon.png" width="300" title="Phenoscript logo">
 </p> 
 
 
 [Phenospy](https://pypi.org/project/phenospy/) is a Python package that facilitates the automatic analysis and comparison of ontology-based (= semantic) descriptions of species and phenotypes. Phenospy works with descriptions written in [Phenoscript](https://github.com/sergeitarasov/vscode-phenoscript), a computer language designed for describing species (support for other semantic approaches is under development). 
 
 The Phenoscript language allows rapid coding of morphological and ecological traits using an individual-based approach (ontology's A-box). You can efficiently code Phenoscript by using the [VS Code Phenoscript extension](https://marketplace.visualstudio.com/items?itemName=Tarasov-Lab.phenoscript) that provides syntax highlighting and snippet support. It can be installed from the Marketplace from within the VS Code. Its GitHub repository can be accessed [here](https://github.com/sergeitarasov/vscode-phenoscript). Afterward, Phenospy can be used to analyze and process the semantic descriptions.
 
@@ -49,51 +50,18 @@
 
 ## Install
 Phenospy can be installed directly from the [PyPI repository](https://pypi.org/project/phenospy/) by running the following command in your terminal (macOS) or a command prompt (Windows):
 
 ```{bash}
 pip install phenospy
 ```
-### Troubleshooting
-Pip is usually pre-installed with Python on macOS and Windows. However, if pip is not installed or you want to upgrade it to the latest version, you can follow these steps:
-
-**For macOS:**
-1. In your terminal type the following command to download the get-pip.py script:
-```{bash}
-curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
-```
-2. Type the following command to run the get-pip.py script and install pip:
-
-```{bash}
-sudo python get-pip.py
-````
-3. Verify that pip is installed by typing the following command:
-```{bash}
-pip --version
-```
-
-**For Windows:**
-
-Open a command prompt by clicking on the "Start" menu, typing "cmd" into the search box, and selecting "Command Prompt" from the search results.
-
-1. Type the following command to install pip:
-```
-py -m ensurepip --default-pip
-```
-
-2. Type the following command to upgrade pip to the latest version:
-```
-py -m pip install --upgrade pip
-```
-
-
-
-
 
+## Issues
 
+-  Phenospy is dependent on [Owlready2](https://github.com/pwin/owlready2), which uses the sqlite library. The latest versions of sqlite library (e.g., 3.40.0) are known to be very slow. If Phenospy package is slow, for example, when you make your snippets, downgrade your sqlite library version. In my case, 3.39.0 worked fine.
 
 ## Quick start guide
 
 Coming soon.
 
 ### Let's create snippets
```

### Comparing `phenospy-0.12/README.md` & `phenospy-0.13/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/phenospy?color=blue&label=PyPI%20Downloads)
 
 # Phenospy (= Phenoscript Python tools)
 
  <p align="left">
   <img src="https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/phenospy.png" width="300" title="Phenospy logo">
+  <img src="https://raw.githubusercontent.com/sergeitarasov/vscode-phenoscript/main/icon.png" width="300" title="Phenoscript logo">
 </p> 
 
 
 [Phenospy](https://pypi.org/project/phenospy/) is a Python package that facilitates the automatic analysis and comparison of ontology-based (= semantic) descriptions of species and phenotypes. Phenospy works with descriptions written in [Phenoscript](https://github.com/sergeitarasov/vscode-phenoscript), a computer language designed for describing species (support for other semantic approaches is under development). 
 
 The Phenoscript language allows rapid coding of morphological and ecological traits using an individual-based approach (ontology's A-box). You can efficiently code Phenoscript by using the [VS Code Phenoscript extension](https://marketplace.visualstudio.com/items?itemName=Tarasov-Lab.phenoscript) that provides syntax highlighting and snippet support. It can be installed from the Marketplace from within the VS Code. Its GitHub repository can be accessed [here](https://github.com/sergeitarasov/vscode-phenoscript). Afterward, Phenospy can be used to analyze and process the semantic descriptions.
 
@@ -29,51 +30,18 @@
 
 ## Install
 Phenospy can be installed directly from the [PyPI repository](https://pypi.org/project/phenospy/) by running the following command in your terminal (macOS) or a command prompt (Windows):
 
 ```{bash}
 pip install phenospy
 ```
-### Troubleshooting
-Pip is usually pre-installed with Python on macOS and Windows. However, if pip is not installed or you want to upgrade it to the latest version, you can follow these steps:
-
-**For macOS:**
-1. In your terminal type the following command to download the get-pip.py script:
-```{bash}
-curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
-```
-2. Type the following command to run the get-pip.py script and install pip:
-
-```{bash}
-sudo python get-pip.py
-````
-3. Verify that pip is installed by typing the following command:
-```{bash}
-pip --version
-```
-
-**For Windows:**
-
-Open a command prompt by clicking on the "Start" menu, typing "cmd" into the search box, and selecting "Command Prompt" from the search results.
-
-1. Type the following command to install pip:
-```
-py -m ensurepip --default-pip
-```
-
-2. Type the following command to upgrade pip to the latest version:
-```
-py -m pip install --upgrade pip
-```
-
-
-
-
 
+## Issues
 
+-  Phenospy is dependent on [Owlready2](https://github.com/pwin/owlready2), which uses the sqlite library. The latest versions of sqlite library (e.g., 3.40.0) are known to be very slow. If Phenospy package is slow, for example, when you make your snippets, downgrade your sqlite library version. In my case, 3.39.0 worked fine.
 
 ## Quick start guide
 
 Coming soon.
 
 ### Let's create snippets
```

### Comparing `phenospy-0.12/phenospy/nl_fun.py` & `phenospy-0.13/phenospy/nl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/nl_owlToMd.py` & `phenospy-0.13/phenospy/nl_owlToMd.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/nl_owlToMd_fun.py` & `phenospy-0.13/phenospy/nl_owlToMd_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/owl_make_phsOntology.py` & `phenospy-0.13/phenospy/owl_make_phsOntology.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/owl_owlready_config.py` & `phenospy-0.13/phenospy/owl_owlready_config.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/owl_xml2owl_fun.py` & `phenospy-0.13/phenospy/owl_xml2owl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/owl_xmlToOwl.py` & `phenospy-0.13/phenospy/owl_xmlToOwl.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import os
 import tempfile
 import xml.etree.ElementTree as ET
 from datetime import date
 
 from phenospy.owl_xml2owl_fun import *
 from phenospy.xml_recodeThis import *
+#from xml_recodeThis import *
 
 # -----------------------------------------
 # Config: imported from owl_xml2owl_fun
 # -----------------------------------------
 # from owl_owlready_config import *
 
 # -----------------------------------------
```

### Comparing `phenospy-0.12/phenospy/package-data/.DS_Store` & `phenospy-0.13/phenospy/package-data/.DS_Store`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/package-data/phenoscript.obda` & `phenospy-0.13/phenospy/package-data/phenoscript.obda`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/package-data/phenoscript.owl` & `phenospy-0.13/phenospy/package-data/phenoscript.owl`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/package-data/phs-config.yaml` & `phenospy-0.13/phenospy/package-data/phs-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #   Win: `%USERPROFILE%\.vscode\extensions`
 #   Mac:`$HOME/.vscode/extensions`
 #   Linux: `$HOME/.vscode/extensions`
-snippet-dir: /Users/taravser/.vscode/extensions/tarasov-lab.phenoscript-0.0.11/snippets/
+snippet-dir: /Users/taravser/.vscode/extensions/tarasov-lab.phenoscript-0.0.12/snippets/
 authors:
   'First1 Last1': https://orcid.org/0000-0001-xxxx-xxxx
   'First2 Last2': https://orcid.org/0000-0001-xxxx-xxxx
 importOntologies:
   - https://raw.githubusercontent.com/insect-morphology/colao/master/colao.owl
   - https://raw.githubusercontent.com/hymao/hao/master/hao.owl
   - https://raw.githubusercontent.com/insect-morphology/aism/master/aism.owl
@@ -23,15 +23,15 @@
   default:    http://www.w3.org/2002/07/owl#
   others:
     rdfs:     http://www.w3.org/2000/01/rdf-schema#
     formats:  http://www.geneontology.org/formats/oboInOwl#
     dc:       http://purl.org/dc/
     hao:      http://purl.obolibrary.org/obo/HAO_
     aism:     http://purl.obolibrary.org/obo/AISM_
-    clao:     http://purl.obolibrary.org/obo/COLAO_
+    colao:     http://purl.obolibrary.org/obo/COLAO_
     bfo:      http://purl.obolibrary.org/obo/BFO_
     ro:       http://purl.obolibrary.org/obo/RO_
     obi:      http://purl.obolibrary.org/obo/OBI_
     ncbi:     http://purl.obolibrary.org/obo/NCBITaxon_
     iao:      http://purl.obolibrary.org/obo/IAO_
     bspo:     http://purl.obolibrary.org/obo/BSPO_
     pato:     http://purl.obolibrary.org/obo/PATO_
@@ -40,9 +40,9 @@
     cdao:     http://purl.obolibrary.org/obo/CDAO_
     unit:     http://purl.obolibrary.org/obo/UO_
     dsw:      http://purl.org/dsw/
     dwc:      http://rs.tdwg.org/dwc/terms/
     zoo:      http://zoobank.org/
     gbif:     https://www.gbif.org/species/
     phs:      https://github.com/sergeitarasov/PhenoScript/PHS_
-    # uberon: http://purl.obolibrary.org/obo/UBERON_
+    uberon: http://purl.obolibrary.org/obo/UBERON_
     # obo: http://purl.obolibrary.org/obo/
```

### Comparing `phenospy-0.12/phenospy/package-data/snippets-default.json` & `phenospy-0.13/phenospy/package-data/snippets-default.json`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_addXmlMeta.py` & `phenospy-0.13/phenospy/phs_addXmlMeta.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_grammar.py` & `phenospy-0.13/phenospy/phs_grammar.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_mainConvert.py` & `phenospy-0.13/phenospy/phs_mainConvert.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_parser_fun.py` & `phenospy-0.13/phenospy/phs_parser_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_various_fun.py` & `phenospy-0.13/phenospy/phs_various_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_xml.py` & `phenospy-0.13/phenospy/phs_xml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/phs_xmlTranslateTerms.py` & `phenospy-0.13/phenospy/phs_xmlTranslateTerms.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/snips_fun.py` & `phenospy-0.13/phenospy/snips_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/snips_makeFromYaml.py` & `phenospy-0.13/phenospy/snips_makeFromYaml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/snips_readFromJSON.py` & `phenospy-0.13/phenospy/snips_readFromJSON.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/phenospy/xml_recodeThis.py` & `phenospy-0.13/phenospy/xml_recodeThis.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 def xmlRecodeThis(root, ns):
     phs = '{https://github.com/sergeitarasov/PhenoScript}'
     # make mapping to extract parents quickly
     parent_map = {c:p for p in root.iter() for c in p}
     OTUs=root.findall(".//phs:otu_object", ns)
     for otu in OTUs:
         this_node=otu.find(".//phs:otu_properties//phs:node_property[@phs:var-iri='KeyWord:this'][@phs:value-iri='KeyWord:True']", ns)
-        this_parent = parent_map[this_node]
-        # <phs:node phs:node_id="https://urn:uuid:8f7fbcbc-ccbb-11ed-beb4-acde48001122/id-4e3742" phs:triple_pos="3" phs:node_name="hao-female_organism" 
-        # phs:fromNegativeEdge="False" phs:iri="http://purl.obolibrary.org/obo/HAO_0000028" phs:label_original="female organism" phs:type_onto="C">
-        p_node_id         = this_parent.get(phs+'node_id')
-        p_node_name       = this_parent.get(phs+'node_name')
-        p_iri             = this_parent.get(phs+'iri')
-        p_label_original  = this_parent.get(phs+'label_original')
-        p_type_onto       = this_parent.get(phs+'type_onto')
-        #
-        ophuList = otu.find(".//phs:ophu_list", ns)
-        this_ophuNodes = ophuList.findall(".//phs:node[@phs:iri='KeyWord:this']", ns)
-        for this in this_ophuNodes:
-            this.set('{https://github.com/sergeitarasov/PhenoScript}node_id', p_node_id)
-            this.set('{https://github.com/sergeitarasov/PhenoScript}node_name', p_node_name)
-            this.set('{https://github.com/sergeitarasov/PhenoScript}iri', p_iri)
-            this.set('{https://github.com/sergeitarasov/PhenoScript}label_original', p_label_original)
-            this.set('{https://github.com/sergeitarasov/PhenoScript}type_onto', p_type_onto)
-            # this.text 
+        # print('THIS:', this_node)
+        if this_node is not None:
+            this_parent = parent_map[this_node]
+            # <phs:node phs:node_id="https://urn:uuid:8f7fbcbc-ccbb-11ed-beb4-acde48001122/id-4e3742" phs:triple_pos="3" phs:node_name="hao-female_organism" 
+            # phs:fromNegativeEdge="False" phs:iri="http://purl.obolibrary.org/obo/HAO_0000028" phs:label_original="female organism" phs:type_onto="C">
+            p_node_id         = this_parent.get(phs+'node_id')
+            p_node_name       = this_parent.get(phs+'node_name')
+            p_iri             = this_parent.get(phs+'iri')
+            p_label_original  = this_parent.get(phs+'label_original')
+            p_type_onto       = this_parent.get(phs+'type_onto')
+            #
+            ophuList = otu.find(".//phs:ophu_list", ns)
+            this_ophuNodes = ophuList.findall(".//phs:node[@phs:iri='KeyWord:this']", ns)
+            for this in this_ophuNodes:
+                this.set('{https://github.com/sergeitarasov/PhenoScript}node_id', p_node_id)
+                this.set('{https://github.com/sergeitarasov/PhenoScript}node_name', p_node_name)
+                this.set('{https://github.com/sergeitarasov/PhenoScript}iri', p_iri)
+                this.set('{https://github.com/sergeitarasov/PhenoScript}label_original', p_label_original)
+                this.set('{https://github.com/sergeitarasov/PhenoScript}type_onto', p_type_onto)
+                # this.text 
 
 # Save
 # Create an ElementTree object from the root element
 # tree_save = ET.ElementTree(root)
 # # Save the XML tree to a file
 # xml_save = '/Users/taravser/Documents/My_papers/PhenoScript_main/PhenoScript/phenospy_package/phenospy/package-data' \
 #            '/phs_xml.xml'
```

### Comparing `phenospy-0.12/phenospy.egg-info/PKG-INFO` & `phenospy-0.13/phenospy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.12
+Version: 0.13
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,15 @@
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/phenospy?color=blue&label=PyPI%20Downloads)
 
 # Phenospy (= Phenoscript Python tools)
 
  <p align="left">
   <img src="https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/phenospy.png" width="300" title="Phenospy logo">
+  <img src="https://raw.githubusercontent.com/sergeitarasov/vscode-phenoscript/main/icon.png" width="300" title="Phenoscript logo">
 </p> 
 
 
 [Phenospy](https://pypi.org/project/phenospy/) is a Python package that facilitates the automatic analysis and comparison of ontology-based (= semantic) descriptions of species and phenotypes. Phenospy works with descriptions written in [Phenoscript](https://github.com/sergeitarasov/vscode-phenoscript), a computer language designed for describing species (support for other semantic approaches is under development). 
 
 The Phenoscript language allows rapid coding of morphological and ecological traits using an individual-based approach (ontology's A-box). You can efficiently code Phenoscript by using the [VS Code Phenoscript extension](https://marketplace.visualstudio.com/items?itemName=Tarasov-Lab.phenoscript) that provides syntax highlighting and snippet support. It can be installed from the Marketplace from within the VS Code. Its GitHub repository can be accessed [here](https://github.com/sergeitarasov/vscode-phenoscript). Afterward, Phenospy can be used to analyze and process the semantic descriptions.
 
@@ -49,51 +50,18 @@
 
 ## Install
 Phenospy can be installed directly from the [PyPI repository](https://pypi.org/project/phenospy/) by running the following command in your terminal (macOS) or a command prompt (Windows):
 
 ```{bash}
 pip install phenospy
 ```
-### Troubleshooting
-Pip is usually pre-installed with Python on macOS and Windows. However, if pip is not installed or you want to upgrade it to the latest version, you can follow these steps:
-
-**For macOS:**
-1. In your terminal type the following command to download the get-pip.py script:
-```{bash}
-curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
-```
-2. Type the following command to run the get-pip.py script and install pip:
-
-```{bash}
-sudo python get-pip.py
-````
-3. Verify that pip is installed by typing the following command:
-```{bash}
-pip --version
-```
-
-**For Windows:**
-
-Open a command prompt by clicking on the "Start" menu, typing "cmd" into the search box, and selecting "Command Prompt" from the search results.
-
-1. Type the following command to install pip:
-```
-py -m ensurepip --default-pip
-```
-
-2. Type the following command to upgrade pip to the latest version:
-```
-py -m pip install --upgrade pip
-```
-
-
-
-
 
+## Issues
 
+-  Phenospy is dependent on [Owlready2](https://github.com/pwin/owlready2), which uses the sqlite library. The latest versions of sqlite library (e.g., 3.40.0) are known to be very slow. If Phenospy package is slow, for example, when you make your snippets, downgrade your sqlite library version. In my case, 3.39.0 worked fine.
 
 ## Quick start guide
 
 Coming soon.
 
 ### Let's create snippets
```

### Comparing `phenospy-0.12/phenospy.egg-info/SOURCES.txt` & `phenospy-0.13/phenospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.12/setup.py` & `phenospy-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phenospy',
-    version='0.12',
+    version='0.13',
     packages=find_packages(exclude=['tests*', 'devel*', 'build*']),
     license='MIT',
     description='Tools for making and processing computable phenotype descriptions',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     install_requires=['Owlready2',
                       'PyYAML',
```

