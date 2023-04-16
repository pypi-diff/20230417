# Comparing `tmp/Bevy-1.3.9.tar.gz` & `tmp/bevy-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bevy-1.3.9.tar", max compression
+gzip compressed data, was "bevy-2.0.0b1.tar", max compression
```

## Comparing `Bevy-1.3.9.tar` & `bevy-2.0.0b1.tar`

### file list

```diff
@@ -1,24 +1,14 @@
--rw-r--r--   0        0        0     1076 2022-06-19 19:43:37.391919 Bevy-1.3.9/LICENSE
--rw-r--r--   0        0        0     3201 2022-06-19 19:43:37.395919 Bevy-1.3.9/README.md
--rw-r--r--   0        0        0      162 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/__init__.py
--rw-r--r--   0        0        0       41 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/context/__init__.py
--rw-r--r--   0        0        0     1866 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/context/abstract_context.py
--rw-r--r--   0        0        0     4970 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/context/context.py
--rw-r--r--   0        0        0      906 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/context/null_context.py
--rw-r--r--   0        0        0       44 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/inject/__init__.py
--rw-r--r--   0        0        0     1388 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/inject/annotations.py
--rw-r--r--   0        0        0      673 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/inject/context_injector.py
--rw-r--r--   0        0        0     1895 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/inject/inject.py
--rw-r--r--   0        0        0     2787 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/inject/inject_strategies.py
--rw-r--r--   0        0        0      191 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/__init__.py
--rw-r--r--   0        0        0     2370 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/base.py
--rw-r--r--   0        0        0     1618 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/builder.py
--rw-r--r--   0        0        0     3016 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/function_provider.py
--rw-r--r--   0        0        0      497 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/injection_priority_helpers.py
--rw-r--r--   0        0        0     1269 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/instance_provider.py
--rw-r--r--   0        0        0     1464 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/providers/type_provider.py
--rw-r--r--   0        0        0      429 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/sentinel.py
--rw-r--r--   0        0        0      245 2022-06-19 19:43:37.395919 Bevy-1.3.9/bevy/single_return_value_cache.py
--rw-r--r--   0        0        0      889 2022-06-19 19:43:37.399920 Bevy-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     4010 2022-06-19 19:43:46.963520 Bevy-1.3.9/setup.py
--rw-r--r--   0        0        0     4033 2022-06-19 19:43:46.964111 Bevy-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-16 23:31:42.061579 bevy-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     5871 2023-04-16 23:31:42.061579 bevy-2.0.0b1/README.md
+-rw-r--r--   0        0        0      208 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/__init__.py
+-rw-r--r--   0        0        0     1463 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/contextvar.py
+-rw-r--r--   0        0        0     1692 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/injectors/classes.py
+-rw-r--r--   0        0        0     2244 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/injectors/functions.py
+-rw-r--r--   0        0        0     2717 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/options.py
+-rw-r--r--   0        0        0      164 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/__init__.py
+-rw-r--r--   0        0        0     1537 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/annotated_provider.py
+-rw-r--r--   0        0        0     3488 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/base.py
+-rw-r--r--   0        0        0     1143 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/providers/type_provider.py
+-rw-r--r--   0        0        0     5950 2023-04-16 23:31:42.061579 bevy-2.0.0b1/bevy/repository.py
+-rw-r--r--   0        0        0      866 2023-04-16 23:31:42.061579 bevy-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6710 1970-01-01 00:00:00.000000 bevy-2.0.0b1/PKG-INFO
```

### Comparing `Bevy-1.3.9/LICENSE` & `bevy-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `Bevy-1.3.9/pyproject.toml` & `bevy-2.0.0b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Bevy"
-version = "1.3.9"
+version = "2.0.0b1"
 description = "Python Dependency Inversion made simple so you can focus on creating amazing code."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Bevy"
 repository = "https://github.com/ZechCodes/Bevy"
 documentation = "https://github.com/ZechCodes/Bevy/blob/master/README.md"
@@ -14,15 +14,14 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Application Frameworks"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fast-protocol = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-asyncio = "^0.18.3"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

