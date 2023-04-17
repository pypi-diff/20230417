# Comparing `tmp/invokify-0.1.1.tar.gz` & `tmp/invokify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokify-0.1.1.tar", max compression
+gzip compressed data, was "invokify-0.1.2.tar", max compression
```

## Comparing `invokify-0.1.1.tar` & `invokify-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      232 2023-04-14 21:08:33.165762 invokify-0.1.1/invokify/__init__.py
--rw-r--r--   0        0        0     6886 2023-04-14 20:37:10.251034 invokify-0.1.1/invokify/invokify.py
--rw-r--r--   0        0        0     2208 2023-04-14 20:15:39.083725 invokify-0.1.1/invokify/parser.py
--rw-r--r--   0        0        0     1082 2023-04-14 19:28:07.595190 invokify-0.1.1/LICENSE
--rw-r--r--   0        0        0      346 2023-04-14 21:08:44.870955 invokify-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2125 2023-04-14 21:08:46.184136 invokify-0.1.1/README.md
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 invokify-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-04-17 19:23:05.551213 invokify-0.1.2/invokify/__init__.py
+-rw-r--r--   0        0        0     8179 2023-04-17 19:20:57.265858 invokify-0.1.2/invokify/invokify.py
+-rw-r--r--   0        0        0     2350 2023-04-17 19:17:05.658800 invokify-0.1.2/invokify/parser.py
+-rw-r--r--   0        0        0     1082 2023-04-14 19:28:07.595190 invokify-0.1.2/LICENSE
+-rw-r--r--   0        0        0      346 2023-04-17 19:23:07.133560 invokify-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2125 2023-04-14 21:08:46.184136 invokify-0.1.2/README.md
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 invokify-0.1.2/PKG-INFO
```

### Comparing `invokify-0.1.1/invokify/invokify.py` & `invokify-0.1.2/invokify/invokify.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Allows the creation of parsible commands using decorators.
 """
 __all__ = ["CommandAlreadyExists", "EngineRequired", "meta", "Command", "InvokeEngine"]
 
 import functools
 from dataclasses import dataclass, field
+from typing import Any, Callable, Optional, Union
 
 
 class CommandAlreadyExists(Exception):
     """
     Will be raised when attempting to name a command/alias
     the same as one that already exists.
     """
@@ -23,90 +24,105 @@
 
 
 @dataclass(slots=True)
 class meta:
     """Define requirements for a command, such as injecting itself into the function."""
 
     requires: dict[str, bool] = field(default_factory=dict)
-    injections: dict[str, any] = field(default_factory=dict)
-    func: callable = None
+    injections: dict[str, Any] = field(default_factory=dict)
+    func: Optional[Callable[..., Any]] = None
     helptext: str = ""
 
     @staticmethod
-    def require(engine: bool = False, command: bool = False, **kwargs: bool) -> "meta":
+    def require(
+        engine: bool = False, command: bool = False, **kwargs: bool
+    ) -> Callable[[Callable[..., Any] | "meta"], "meta|Command"]:
         """
         Specifies the requirements for a command.
         `engine` and `command` are considered special and will be
         injected automatically when set to true.
 
         Any other value will be available in the command's "requires" property
         and can be used for evaluation.
         """
 
-        def wrapper(func: any) -> "meta":
+        def wrapper(func: Callable[..., Any] | "meta") -> meta | Command:
             if isinstance(func, meta):
                 raise TypeError("meta.require cannot be passed a command object.")
             if not isinstance(func, Command):
                 return meta(
                     requires={"engine": engine, "command": command, **kwargs},
                     injections={},
                     func=func,
                     helptext="",
                 )
             func.requires = {"engine": engine, "command": command, **kwargs}
+            return func
 
         return wrapper
 
     @staticmethod
-    def inject(**kwargs: bool) -> "meta":
+    def inject(
+        **kwargs: Any,
+    ) -> Callable[[Callable[..., Any] | "meta"], "meta|Command"]:
         """
         Specifies objects to inject into the function.
         The function's argument must match the injection's argument.
         """
 
-        def wrapper(func: any):
+        def wrapper(func: Callable[..., Any] | "meta") -> "meta|Command":
             if isinstance(func, Command):
                 raise TypeError("meta.inject cannot be passed a command object.")
             if not isinstance(func, meta):
                 return meta(requires={}, injections=kwargs, func=func, helptext="")
             func.injections = kwargs
             return func
 
         return wrapper
 
     @staticmethod
-    def help(text: str) -> "meta":
+    def help(text: str) -> Callable[[Callable[..., Any] | "meta"], "meta|Command"]:
         """
         Creates a help text for a command.
         """
 
-        def wrapper(func: any):
+        def wrapper(func: Callable[..., Any] | "meta") -> "meta|Command":
             if isinstance(func, Command):
                 raise TypeError("meta.inject cannot be passed a command object.")
             if not isinstance(func, meta):
                 return meta(requires={}, injections={}, func=func, helptext=text)
             func.helptext = text
             return func
 
         return wrapper
 
 
 @dataclass(slots=True)
 class Command:
     """A class that defines a command"""
 
-    func: callable
+    func: Callable[
+        ..., Any
+    ]  # The function or method that was transformed into a Command.
     name: str
     aliases: list[str]
-    requires: dict[str, bool]
-    injections: dict[str, any]
-    children: dict[str, "Command"] = field(default_factory=dict)
-    helptext: str = None
-
-    def __call__(self, *args: any, engine: "InvokeEngine" = None, **kwargs: any) -> any:
+    requires: dict[
+        str, bool
+    ]  # The requirements for the command, this can be accessed for custom tests.
+    injections: dict[
+        str, Any
+    ]  # Objects that will be injected into the command as kwargs.
+    children: dict[str, "Command"] = field(
+        default_factory=dict
+    )  # Similar to engine.commands; Lists the subcommands attached to a command.
+    helptext: Optional[str] = None
+
+    def __call__(
+        self, *args: Any, engine: Optional["InvokeEngine"] = None, **kwargs: Any
+    ) -> Any:
         if self.requires.get("engine"):
             if engine is None:
                 raise EngineRequired
             self.injections["engine"] = engine
 
         if self.requires.get("command"):
             self.injections["command"] = self
@@ -116,115 +132,119 @@
     def __repr__(self) -> str:
         return f"Command(func={self.func.__name__}, aliases={self.aliases})"
 
     @property
     def __name__(self) -> str:
         return self.func.__name__
 
-    def _set_current_engine(self, engine: "InvokeEngine"):
-        self.engine = engine
-
     def subcommand(
         self,
-        func: callable = None,
-        name: str = None,
-        aliases: list[str] = None,
+        func: Optional[Union[Callable[..., Any], "Command", meta]] = None,
+        name: Optional[str] = None,
+        aliases: Optional[list[str]] = None,
     ) -> "Command":
         """A decorator that turns a function into a subcommand"""
 
         return create_command(
             func=func,
             commanddict=self.children,
             name=name,
             aliases=aliases,
         )
 
 
-def create_command(func: callable, commanddict: dict, name: str, aliases: list[str]):
+def create_command(
+    func: Optional[Callable[..., Any] | meta],
+    commanddict: dict[str, Command],
+    name: Optional[str],
+    aliases: Optional[list[str]],
+) -> Command:
     """Creates a command."""
     if aliases is None:
         aliases = []
 
-    @functools.wraps(func)
-    def wrapper(func: callable):
+    @functools.wraps(func)  # type: ignore
+    def wrapper(func: Callable[..., Any] | Command | meta) -> Command:
         nonlocal aliases
         nonlocal name
 
         requires = {}
         inject = {}
         helptext = None
         if isinstance(func, meta):
             requires = func.requires
             inject = func.injections
             helptext = func.helptext
-            func = func.func
+            func = func.func  # type: ignore
 
         if name is None:
-            name = func.__name__
+            name = func.__name__  # type: ignore
 
         command = func
         if not isinstance(func, Command):
             command = Command(
-                func=func,
-                name=name,
+                func=func,  # type: ignore
+                name=name,  # type: ignore
                 aliases=aliases,
                 requires=requires,
                 injections=inject,
                 helptext=helptext,
             )
 
-        aliases.append(name)
+        aliases.append(name)  # type: ignore
         for name in aliases:
             if commanddict.get(name):
                 raise CommandAlreadyExists
-            commanddict[name] = command
-        return command
+            # This will always be set to a command because in the above code,
+            # if command is not a Command, it will be set as one.
+            commanddict[name] = command  # type: ignore
+        return command  # type: ignore
 
     if func:
         return wrapper(func)
-    return wrapper
+    return wrapper  # type: ignore
 
 
 @dataclass(slots=True)
 class InvokeEngine:
     """A container for commands."""
 
     commands: dict[str, Command] = field(default_factory=dict)
 
     def parse(
         self,
-        command_list: list[any],
-        _command: Command = None,
-        _callstack: list[Command] = None,
-    ) -> tuple[Command, tuple[any, ...], tuple[Command, ...]]:
+        command_list: list[Any],
+        _command: Optional[Command] = None,
+        _callstack: Optional[list[Command]] = None,
+    ) -> tuple[Command, tuple[Any, ...], tuple[Command, ...]]:
         """Parses a list to find the lowest level subcommand, and passes the rest of the arguments back."""
         if _callstack is None:
             _callstack = []
         else:
-            _callstack.append(_command)
+            _callstack.append(_command)  # type: ignore
 
         if len(command_list) == 0:
-            return (_command, command_list, tuple(_callstack))
+            return (_command, command_list, tuple(_callstack))  # type: ignore
 
         if _command is None:
             command = self.commands.get(command_list[0])
         else:
             command = _command.children.get(command_list[0])
 
         if command is None:
-            return (_command, command_list, tuple(_callstack))
+            return (_command, command_list, tuple(_callstack))  # type: ignore
 
         return self.parse(
             command_list=command_list[1:], _command=command, _callstack=_callstack
         )
 
     def command(
         self,
-        func: callable | Command = None,
-        name: str = None,
-        aliases: list[str] = None,
+        func: Optional[Union[Callable[..., Any], Command, meta]] = None,
+        name: Optional[str] = None,
+        aliases: Optional[list[str]] = None,
     ) -> Command:
         """A decorator that turns a function into a command"""
 
         return create_command(
             func=func, commanddict=self.commands, name=name, aliases=aliases
         )
```

### Comparing `invokify-0.1.1/invokify/parser.py` & `invokify-0.1.2/invokify/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 from tokenstream import Token, TokenStream
 import re
 
 __all__ = ["string_to_args"]
 
 ESCAPE_REGEX = re.compile(r"\\.")
 
@@ -12,15 +13,15 @@
 }
 
 
 def unquote_string(token: Token) -> str:
     return ESCAPE_REGEX.sub(lambda match: ESCAPE_SEQUENCES[match[0]], token.value[1:-1])
 
 
-def parse_list(stream: TokenStream):
+def parse_list(stream: TokenStream) -> list[Any] | int | float | str | None:
     with stream.syntax(
         comma=r",\s*",
         decimal=r"-?\d*\.\d+|-?\d+\.\d*",
         integer=r"\d+",
         entry=r"[^\"\[\],]+",
     ), stream.ignore("comma"):
         match stream.expect_any(
@@ -32,14 +33,16 @@
                 return float(decimal.value)
             case Token(type="integer") as integer:
                 return int(integer.value)
             case Token(type="entry") as entry:
                 return entry.value
             case Token(type="string") as string:
                 return unquote_string(string)
+            case _:
+                pass
 
 
 def parse_token(token: Token, stream: TokenStream):
     print(token.value)
     match token:
         case Token(type="brace"):
             return [(parse_list(stream)) for _ in stream.peek_until(("brace", "]"))]
@@ -47,14 +50,16 @@
             return unquote_string(string)
         case Token(type="decimal") as decimal:
             return float(decimal.value)
         case Token(type="integer") as integer:
             return int(integer.value)
         case Token(type="word") as word:
             return word.value
+        case _:
+            pass
 
 
 def string_to_args(string: str):
     stream = TokenStream(string)
     with stream.syntax(
         brace=r"\[|\]",
         decimal=r"-?\d*\.\d+|-?\d+\.\d*",
```

### Comparing `invokify-0.1.1/LICENSE` & `invokify-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invokify-0.1.1/README.md` & `invokify-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `invokify-0.1.1/PKG-INFO` & `invokify-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokify
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: iRedSC
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

