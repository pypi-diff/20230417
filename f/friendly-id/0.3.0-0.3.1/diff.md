# Comparing `tmp/friendly-id-0.3.0.tar.gz` & `tmp/friendly-id-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendly-id-0.3.0.tar", last modified: Mon Apr 17 08:31:47 2023, max compression
+gzip compressed data, was "friendly-id-0.3.1.tar", last modified: Mon Apr 17 08:41:16 2023, max compression
```

## Comparing `friendly-id-0.3.0.tar` & `friendly-id-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 08:31:47.222158 friendly-id-0.3.0/
--rw-rw-rw-   0        0        0     1051 2023-04-17 07:47:50.000000 friendly-id-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     3917 2023-04-17 08:31:47.221156 friendly-id-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2130 2023-04-17 08:28:55.000000 friendly-id-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 08:31:47.200157 friendly-id-0.3.0/friendly_id/
--rw-rw-rw-   0        0        0      115 2023-04-17 08:28:55.000000 friendly-id-0.3.0/friendly_id/__init__.py
--rw-rw-rw-   0        0        0     1023 2023-04-17 08:21:14.000000 friendly-id-0.3.0/friendly_id/friendly_id.py
--rw-rw-rw-   0        0        0      436 2023-04-17 08:20:38.000000 friendly-id-0.3.0/friendly_id/test_friendly_id.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:31:47.219149 friendly-id-0.3.0/friendly_id.egg-info/
--rw-rw-rw-   0        0        0     3917 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1220 2023-04-17 08:28:55.000000 friendly-id-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 08:31:47.222158 friendly-id-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-04-17 07:47:50.000000 friendly-id-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:41:16.596371 friendly-id-0.3.1/
+-rw-rw-rw-   0        0        0     1051 2023-04-17 07:47:50.000000 friendly-id-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3917 2023-04-17 08:41:16.593669 friendly-id-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2130 2023-04-17 08:40:37.000000 friendly-id-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 08:41:16.573340 friendly-id-0.3.1/friendly_id/
+-rw-rw-rw-   0        0        0      123 2023-04-17 08:40:37.000000 friendly-id-0.3.1/friendly_id/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-04-17 08:21:14.000000 friendly-id-0.3.1/friendly_id/friendly_id.py
+-rw-rw-rw-   0        0        0      436 2023-04-17 08:20:38.000000 friendly-id-0.3.1/friendly_id/test_friendly_id.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:41:16.593669 friendly-id-0.3.1/friendly_id.egg-info/
+-rw-rw-rw-   0        0        0     3917 2023-04-17 08:41:16.000000 friendly-id-0.3.1/friendly_id.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-17 08:41:16.000000 friendly-id-0.3.1/friendly_id.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:41:16.000000 friendly-id-0.3.1/friendly_id.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-17 08:41:16.000000 friendly-id-0.3.1/friendly_id.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 08:41:16.000000 friendly-id-0.3.1/friendly_id.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1220 2023-04-17 08:40:37.000000 friendly-id-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:41:16.596371 friendly-id-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-04-17 07:47:50.000000 friendly-id-0.3.1/setup.py
```

### Comparing `friendly-id-0.3.0/LICENSE` & `friendly-id-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `friendly-id-0.3.0/PKG-INFO` & `friendly-id-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendly-id
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read the latest Real Python tutorials
 Author-email: Junlin Zhou <jameszhou2108@hotmail.com>
 License: Copyright 2022 Junlin Zhou
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # Friendly Id
 
-> version 0.3.0
+> version 0.3.1
 
 Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
 
 What is the FriendlyId library?
 --
 The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
```

### Comparing `friendly-id-0.3.0/README.md` & `friendly-id-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Friendly Id
 
-> version 0.3.0
+> version 0.3.1
 
 Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
 
 What is the FriendlyId library?
 --
 The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
```

### Comparing `friendly-id-0.3.0/friendly_id/friendly_id.py` & `friendly-id-0.3.1/friendly_id/friendly_id.py`

 * *Files identical despite different names*

### Comparing `friendly-id-0.3.0/friendly_id.egg-info/PKG-INFO` & `friendly-id-0.3.1/friendly_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendly-id
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read the latest Real Python tutorials
 Author-email: Junlin Zhou <jameszhou2108@hotmail.com>
 License: Copyright 2022 Junlin Zhou
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # Friendly Id
 
-> version 0.3.0
+> version 0.3.1
 
 Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
 
 What is the FriendlyId library?
 --
 The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
```

### Comparing `friendly-id-0.3.0/pyproject.toml` & `friendly-id-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "friendly-id"
-version = "0.3.0"
+version = "0.3.1"
 description = "Read the latest Real Python tutorials"
 readme = "README.md"
 authors = [{ name = "Junlin Zhou", email = "jameszhou2108@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,15 +24,15 @@
     dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
     [project.urls]
     homepage = "https://github.com/edwardzjl/friendly-id"
     repository = "https://github.com/edwardzjl/friendly-id"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
     [tool.bumpver.file_patterns]
```

