# Comparing `tmp/autoflake-2.0.2.tar.gz` & `tmp/autoflake-2.1.0.tar.gz`

## Comparing `autoflake-2.0.2.tar` & `autoflake-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0    46884 2020-02-02 00:00:00.000000 autoflake-2.0.2/autoflake.py
--rwxr-xr-x   0        0        0    90488 2020-02-02 00:00:00.000000 autoflake-2.0.2/test_autoflake.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 autoflake-2.0.2/.gitignore
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 autoflake-2.0.2/AUTHORS.rst
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 autoflake-2.0.2/LICENSE
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 autoflake-2.0.2/README.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 autoflake-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 autoflake-2.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    47002 2020-02-02 00:00:00.000000 autoflake-2.1.0/autoflake.py
+-rwxr-xr-x   0        0        0    91308 2020-02-02 00:00:00.000000 autoflake-2.1.0/test_autoflake.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 autoflake-2.1.0/.gitignore
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 autoflake-2.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoflake-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 autoflake-2.1.0/README.md
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 autoflake-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 autoflake-2.1.0/PKG-INFO
```

### Comparing `autoflake-2.0.2/autoflake.py` & `autoflake-2.1.0/autoflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import tokenize
 
 import pyflakes.api
 import pyflakes.messages
 import pyflakes.reporter
 
 
-__version__ = "2.0.2"
+__version__ = "2.1.0"
 
 
 _LOGGER = logging.getLogger("autoflake")
 _LOGGER.propagate = False
 
 ATOMS = frozenset([tokenize.NAME, tokenize.NUMBER, tokenize.STRING])
 
@@ -1190,15 +1190,19 @@
         "no": False,
         "false": False,
         "off": False,
     }
 
     if "config_file" in flag_args:
         config_file = pathlib.Path(flag_args["config_file"]).resolve()
-        config = process_config_file(config_file)
+
+        if config_file.suffix == ".toml":
+            config = process_pyproject_toml(config_file)
+        else:
+            config = process_config_file(config_file)
 
         if not config:
             _LOGGER.error(
                 "can't parse config file '%s'",
                 config_file,
             )
             return flag_args, False
```

### Comparing `autoflake-2.0.2/test_autoflake.py` & `autoflake-2.1.0/test_autoflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -3381,14 +3381,40 @@
             assert success is True
             assert args == self.with_defaults(
                 files=files,
                 config_file=temp_config,
                 check=True,
             )
 
+    def test_config_option_toml(self):
+        with temporary_file(
+            suffix=".toml",
+            contents=(
+                "[tool.autoflake]\n"
+                "check = true\n"
+                'exclude = [\n  "build",\n  ".venv",\n]'
+            ),
+        ) as temp_config:
+            self.create_file("test_me.py")
+            files = [self.effective_path("test_me.py")]
+
+            args, success = autoflake.merge_configuration_file(
+                {
+                    "files": files,
+                    "config_file": temp_config,
+                },
+            )
+            assert success is True
+            assert args == self.with_defaults(
+                files=files,
+                config_file=temp_config,
+                check=True,
+                exclude="build,.venv",
+            )
+
     def test_load_false(self):
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[autoflake]\nexpand-star-imports = no\n",
         )
         files = [self.effective_path("test_me.py")]
```

### Comparing `autoflake-2.0.2/AUTHORS.rst` & `autoflake-2.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `autoflake-2.0.2/LICENSE` & `autoflake-2.1.0/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2012-2018 Steven Myint
+Copyright (C) Steven Myint
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `autoflake-2.0.2/README.md` & `autoflake-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -197,11 +197,11 @@
 
 ## Using [pre-commit](https://pre-commit.com) hooks
 
 Add the following to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.2
+    rev: v2.1.0
     hooks:
     -   id: autoflake
 ```
```

### Comparing `autoflake-2.0.2/pyproject.toml` & `autoflake-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoflake-2.0.2/PKG-INFO` & `autoflake-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoflake
-Version: 2.0.2
+Version: 2.1.0
 Summary: Removes unused imports and unused variables
 Project-URL: Homepage, https://www.github.com/PyCQA/autoflake
 License: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: automatic,clean,fix,import,unused
 Classifier: Environment :: Console
@@ -217,11 +217,11 @@
 
 ## Using [pre-commit](https://pre-commit.com) hooks
 
 Add the following to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.2
+    rev: v2.1.0
     hooks:
     -   id: autoflake
 ```
```

