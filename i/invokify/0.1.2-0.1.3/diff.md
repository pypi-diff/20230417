# Comparing `tmp/invokify-0.1.2.tar.gz` & `tmp/invokify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokify-0.1.2.tar", max compression
+gzip compressed data, was "invokify-0.1.3.tar", max compression
```

## Comparing `invokify-0.1.2.tar` & `invokify-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      232 2023-04-17 19:23:05.551213 invokify-0.1.2/invokify/__init__.py
--rw-r--r--   0        0        0     8179 2023-04-17 19:20:57.265858 invokify-0.1.2/invokify/invokify.py
--rw-r--r--   0        0        0     2350 2023-04-17 19:17:05.658800 invokify-0.1.2/invokify/parser.py
--rw-r--r--   0        0        0     1082 2023-04-14 19:28:07.595190 invokify-0.1.2/LICENSE
--rw-r--r--   0        0        0      346 2023-04-17 19:23:07.133560 invokify-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2125 2023-04-14 21:08:46.184136 invokify-0.1.2/README.md
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 invokify-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-04-17 19:47:26.825940 invokify-0.1.3/invokify/__init__.py
+-rw-r--r--   0        0        0     8205 2023-04-17 19:41:03.407150 invokify-0.1.3/invokify/invokify.py
+-rw-r--r--   0        0        0     2364 2023-04-17 19:45:39.652323 invokify-0.1.3/invokify/parser.py
+-rw-r--r--   0        0        0     1082 2023-04-14 19:28:07.595190 invokify-0.1.3/LICENSE
+-rw-r--r--   0        0        0      346 2023-04-17 19:47:16.144198 invokify-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2163 2023-04-17 19:24:41.617183 invokify-0.1.3/README.md
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 invokify-0.1.3/PKG-INFO
```

### Comparing `invokify-0.1.2/invokify/invokify.py` & `invokify-0.1.3/invokify/invokify.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 class Command:
     """A class that defines a command"""
 
     func: Callable[
         ..., Any
     ]  # The function or method that was transformed into a Command.
     name: str
-    aliases: list[str]
+    aliases: Optional[list[str]]
     requires: dict[
         str, bool
     ]  # The requirements for the command, this can be accessed for custom tests.
     injections: dict[
         str, Any
     ]  # Objects that will be injected into the command as kwargs.
     children: dict[str, "Command"] = field(
@@ -187,15 +187,15 @@
                 aliases=aliases,
                 requires=requires,
                 injections=inject,
                 helptext=helptext,
             )
 
         aliases.append(name)  # type: ignore
-        for name in aliases:
+        for name in aliases:  # type: ignore
             if commanddict.get(name):
                 raise CommandAlreadyExists
             # This will always be set to a command because in the above code,
             # if command is not a Command, it will be set as one.
             commanddict[name] = command  # type: ignore
         return command  # type: ignore
```

### Comparing `invokify-0.1.2/invokify/parser.py` & `invokify-0.1.3/invokify/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             case Token(type="integer") as integer:
                 return int(integer.value)
             case Token(type="entry") as entry:
                 return entry.value
             case Token(type="string") as string:
                 return unquote_string(string)
             case _:
-                pass
+                return None
 
 
 def parse_token(token: Token, stream: TokenStream):
     print(token.value)
     match token:
         case Token(type="brace"):
             return [(parse_list(stream)) for _ in stream.peek_until(("brace", "]"))]
@@ -51,15 +51,15 @@
         case Token(type="decimal") as decimal:
             return float(decimal.value)
         case Token(type="integer") as integer:
             return int(integer.value)
         case Token(type="word") as word:
             return word.value
         case _:
-            pass
+            return None
 
 
 def string_to_args(string: str):
     stream = TokenStream(string)
     with stream.syntax(
         brace=r"\[|\]",
         decimal=r"-?\d*\.\d+|-?\d+\.\d*",
```

### Comparing `invokify-0.1.2/LICENSE` & `invokify-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invokify-0.1.2/README.md` & `invokify-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 Invokify is published on PyPI so you can easily install it with either `pip` or `poetry`.
 ```shell
 pip install invokify
 ```
 ```shell
 poetry add invokify
 ```
+This package is for python 3.10+
+
 ---
 ## Getting started
 
 Let's create a simple command-line command.
 
 We can start by importing the `InvokeEngine` from invokify:
 
@@ -64,8 +66,8 @@
 
     cmd, args, cs = engine.parse(cleaned)
 
     if cmd:
         cmd(*args)
     else:
         print("No command was found.")
-```
+```
```

### Comparing `invokify-0.1.2/PKG-INFO` & `invokify-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokify
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: iRedSC
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -23,14 +23,16 @@
 Invokify is published on PyPI so you can easily install it with either `pip` or `poetry`.
 ```shell
 pip install invokify
 ```
 ```shell
 poetry add invokify
 ```
+This package is for python 3.10+
+
 ---
 ## Getting started
 
 Let's create a simple command-line command.
 
 We can start by importing the `InvokeEngine` from invokify:
 
@@ -79,7 +81,8 @@
     cmd, args, cs = engine.parse(cleaned)
 
     if cmd:
         cmd(*args)
     else:
         print("No command was found.")
 ```
+
```

