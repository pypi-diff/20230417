# Comparing `tmp/cherryblossom-0.0.2.tar.gz` & `tmp/cherryblossom-0.0.3.tar.gz`

## Comparing `cherryblossom-0.0.2.tar` & `cherryblossom-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/LICSENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/.ipynb_checkpoints/README-checkpoint.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/.ipynb_checkpoints/pyproject-checkpoint.toml
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.key
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Analyzer.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Blossom.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Channels.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Chat.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/DB.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Data.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Functions.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/GPTModel.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Index.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Plots.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/Timezone.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/get_file.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/imports.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/main.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Analyzer-checkpoint.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Blossom-checkpoint.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Channels-checkpoint.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Chat-checkpoint.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/DB-checkpoint.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Data-checkpoint.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Functions-checkpoint.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/GPTModel-checkpoint.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Index-checkpoint.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Plots-checkpoint.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/Timezone-checkpoint.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/get_file-checkpoint.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/imports-checkpoint.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/main-checkpoint.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cherryblossom-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/LICSENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/.ipynb_checkpoints/README-checkpoint.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/.ipynb_checkpoints/pyproject-checkpoint.toml
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.key
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Analyzer.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Blossom.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Channels.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Chat.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/DB.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Data.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Functions.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/GPTModel.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Index.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Plots.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/Timezone.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/get_file.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/imports.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/main.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Analyzer-checkpoint.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Blossom-checkpoint.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Channels-checkpoint.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Chat-checkpoint.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/DB-checkpoint.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Data-checkpoint.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Functions-checkpoint.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/GPTModel-checkpoint.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Index-checkpoint.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Plots-checkpoint.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/Timezone-checkpoint.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/get_file-checkpoint.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/imports-checkpoint.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/main-checkpoint.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/README.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cherryblossom-0.0.3/PKG-INFO
```

### Comparing `cherryblossom-0.0.2/.ipynb_checkpoints/pyproject-checkpoint.toml` & `cherryblossom-0.0.3/.ipynb_checkpoints/pyproject-checkpoint.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #  "src/cherryblossom/*.py",
 #  "/tests",
 #  "src/cherryblossom/.key"
 #]
 
 [project]
 name = "cherryblossom"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cherryblossom-0.0.2/src/cherryblossom/.key` & `cherryblossom-0.0.3/src/cherryblossom/.key`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.2/src/cherryblossom/get_file.py` & `cherryblossom-0.0.3/src/cherryblossom/get_file.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.2/src/cherryblossom/main.py` & `cherryblossom-0.0.3/src/cherryblossom/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from get_file import TOS
+from .get_file import TOS
 
 print(TOS)
 print()
 if input("Do you agree with the Terms of Service? y/n: ") == 'y':
     print('Loading...', end = '\r')
     print()
-    from Analyzer import Analyzer
-    from Blossom import Blossom
-    from Channels import Channels
-    from Chat import Chat
-    from Data import Data
-    from Functions import Functions
-    from GPTModel import GPTModel
-    from Index import Index
-    from Plots import Plots
-    from Timezone import Timezone
+    from .Analyzer import Analyzer
+    from .Blossom import Blossom
+    from .Channels import Channels
+    from .Chat import Chat
+    from .Data import Data
+    from .Functions import Functions
+    from .GPTModel import GPTModel
+    from .Index import Index
+    from .Plots import Plots
+    from .Timezone import Timezone
 else:
     print("You must agree to the Terms of Service.")
```

### Comparing `cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/get_file-checkpoint.py` & `cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/get_file-checkpoint.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.2/src/cherryblossom/.ipynb_checkpoints/main-checkpoint.py` & `cherryblossom-0.0.3/src/cherryblossom/.ipynb_checkpoints/main-checkpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from get_file import TOS
+from .get_file import TOS
 
 print(TOS)
 print()
 if input("Do you agree with the Terms of Service? y/n: ") == 'y':
     print('Loading...', end = '\r')
     print()
-    from Analyzer import Analyzer
-    from Blossom import Blossom
-    from Channels import Channels
-    from Chat import Chat
-    from Data import Data
-    from Functions import Functions
-    from GPTModel import GPTModel
-    from Index import Index
-    from Plots import Plots
-    from Timezone import Timezone
+    from .Analyzer import Analyzer
+    from .Blossom import Blossom
+    from .Channels import Channels
+    from .Chat import Chat
+    from .Data import Data
+    from .Functions import Functions
+    from .GPTModel import GPTModel
+    from .Index import Index
+    from .Plots import Plots
+    from .Timezone import Timezone
 else:
     print("You must agree to the Terms of Service.")
```

### Comparing `cherryblossom-0.0.2/pyproject.toml` & `cherryblossom-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #  "src/cherryblossom/*.py",
 #  "/tests",
 #  "src/cherryblossom/.key"
 #]
 
 [project]
 name = "cherryblossom"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

