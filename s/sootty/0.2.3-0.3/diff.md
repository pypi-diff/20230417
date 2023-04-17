# Comparing `tmp/sootty-0.2.3.tar.gz` & `tmp/sootty-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sootty-0.2.3.tar", last modified: Mon Jan 17 06:56:59 2022, max compression
+gzip compressed data, was "dist/sootty-0.3.tar", last modified: Mon Apr 17 01:13:50 2023, max compression
```

## Comparing `sootty-0.2.3.tar` & `sootty-0.3.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-01-17 06:56:59.000000 sootty-0.2.3/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-21 07:58:08.000000 sootty-0.2.3/MANIFEST.in
--rw-r--r--   0 benjamin   (501) staff       (20)     2103 2022-01-17 06:56:59.000000 sootty-0.2.3/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)     1468 2021-12-06 07:38:40.000000 sootty-0.2.3/README.md
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2022-01-17 06:56:59.000000 sootty-0.2.3/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      851 2022-01-17 06:54:43.000000 sootty-0.2.3/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty/
--rw-r--r--   0 benjamin   (501) staff       (20)      206 2022-01-17 06:44:06.000000 sootty-0.2.3/sootty/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     2982 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/__main__.py
--rw-r--r--   0 benjamin   (501) staff       (20)      789 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/display.py
--rw-r--r--   0 benjamin   (501) staff       (20)      197 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/exceptions.py
--rw-r--r--   0 benjamin   (501) staff       (20)     2017 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/limits.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty/static/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-01 21:29:54.000000 sootty-0.2.3/sootty/static/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)      900 2021-10-01 21:29:54.000000 sootty-0.2.3/sootty/static/grammar.lark
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty/storage/
--rw-r--r--   0 benjamin   (501) staff       (20)      126 2022-01-17 06:48:58.000000 sootty-0.2.3/sootty/storage/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     5489 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/storage/valuechange.py
--rw-r--r--   0 benjamin   (501) staff       (20)     5157 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/storage/wire.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1355 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/storage/wiregroup.py
--rw-r--r--   0 benjamin   (501) staff       (20)    10278 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/storage/wiretrace.py
--rw-r--r--   0 benjamin   (501) staff       (20)    38183 2022-01-17 06:54:19.000000 sootty-0.2.3/sootty/visualizer.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)     2103 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      516 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       49 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/entry_points.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       41 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        7 2022-01-17 06:56:59.000000 sootty-0.2.3/sootty.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-21 07:58:08.000000 sootty-0.3/MANIFEST.in
+-rw-r--r--   0 benjamin   (501) staff       (20)     5785 2023-04-17 01:13:50.000000 sootty-0.3/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)     4480 2023-04-17 00:26:55.000000 sootty-0.3/README.md
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-04-17 01:13:50.000000 sootty-0.3/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      865 2023-04-17 01:12:47.000000 sootty-0.3/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty/
+-rw-r--r--   0 benjamin   (501) staff       (20)      206 2022-01-17 06:44:06.000000 sootty-0.3/sootty/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     5045 2022-11-11 21:06:02.000000 sootty-0.3/sootty/__main__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      789 2022-01-17 06:54:19.000000 sootty-0.3/sootty/display.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      197 2022-01-17 06:54:19.000000 sootty-0.3/sootty/exceptions.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2566 2022-09-20 06:13:12.000000 sootty-0.3/sootty/parser.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2192 2022-09-20 06:13:12.000000 sootty-0.3/sootty/save.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty/static/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-01 21:29:54.000000 sootty-0.3/sootty/static/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1103 2022-11-11 21:06:02.000000 sootty-0.3/sootty/static/grammar.lark
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty/storage/
+-rw-r--r--   0 benjamin   (501) staff       (20)      126 2022-01-17 06:48:58.000000 sootty-0.3/sootty/storage/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     6243 2022-11-11 20:12:51.000000 sootty-0.3/sootty/storage/valuechange.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     5693 2022-11-11 20:12:51.000000 sootty-0.3/sootty/storage/wire.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1771 2022-11-11 21:06:02.000000 sootty-0.3/sootty/storage/wiregroup.py
+-rw-r--r--   0 benjamin   (501) staff       (20)    13157 2022-11-11 21:06:02.000000 sootty-0.3/sootty/storage/wiretrace.py
+-rw-r--r--   0 benjamin   (501) staff       (20)    15024 2022-09-20 06:13:12.000000 sootty-0.3/sootty/utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)    40240 2022-11-11 21:33:17.000000 sootty-0.3/sootty/visualizer.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)     5785 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      679 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       49 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       41 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       12 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/test/
+-rw-r--r--   0 benjamin   (501) staff       (20)      216 2022-11-11 21:40:39.000000 sootty-0.3/test/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      215 2022-11-11 21:21:24.000000 sootty-0.3/test/test_all.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1241 2022-11-11 21:40:49.000000 sootty-0.3/test/test_general.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      988 2022-11-11 21:28:20.000000 sootty-0.3/test/test_limits.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2840 2022-11-11 21:35:18.000000 sootty-0.3/test/test_pyrtl.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      647 2022-11-11 21:37:11.000000 sootty-0.3/test/test_style.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      303 2022-11-11 21:32:01.000000 sootty-0.3/test/test_wires.py
```

### Comparing `sootty-0.2.3/setup.py` & `sootty-0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pathlib
 import setuptools 
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-README = (HERE / "README.md").read_text()
+README = (HERE / "README.md").read_text(encoding='utf-8')
 
 
 setuptools.setup( 
     name='sootty',
-    version='0.2.3',
+    version='0.3',
     description='Displays vcd files to the command line.', 
     long_description=README,
     packages=setuptools.find_packages(exclude=("tests",)), 
     long_description_content_type="text/markdown",
     url="https://github.com/Ben1152000/sootty",
     author="Ben Darnell",
     author_email="ben@bdarnell.com",
```

### Comparing `sootty-0.2.3/sootty/display.py` & `sootty-0.3/sootty/display.py`

 * *Files identical despite different names*

### Comparing `sootty-0.2.3/sootty/static/grammar.lark` & `sootty-0.3/sootty/static/grammar.lark`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 %import common.WS
 %ignore WS
 %import common.LETTER -> LETTER
 %import common.DIGIT -> DIGIT
 %import common.NUMBER -> NUM
 
-start : lexp
-NAME: ("_"|LETTER) ("_"|LETTER|DIGIT)* ("." ("_"|LETTER|DIGIT)+)*
+NAME : ("_"|LETTER) ("_"|LETTER|DIGIT)* ("." ("_"|LETTER|DIGIT)+)*
 
 AND : "&"
 OR : "|"
+INV : "~"
 XOR : "^"
+LAND : "&&"
+LOR : "||"
+NOT : "!"
 EQ : "=="
 NEQ : "!="
 GT : ">"
 GEQ : ">="
 LT : "<"
 LEQ : "<="
 SL : "<<"
 SR : ">>"
 ADD : "+"
 SUB : "-"
+NEG : "-"
 MOD : "%"
 CONST : "const"
 TIME : "time"
-NOT : "!"
-NEG : "-"
 FROM : "from"
 AFTER : "after"
 UNTIL : "until"
 BEFORE : "before"
 NEXT : "next"
 PREV : "prev"
 ACC : "acc"
 
-lop : AND | OR | XOR
+lop : LAND | LOR
 lexp : rexp | lexp lop rexp
 
 rop : EQ | NEQ | GT | GEQ | LT | LEQ
-rexp : sexp | rexp rop sexp
+rexp : bexp | rexp rop bexp
+
+bop : AND | OR | XOR
+bexp : sexp | bexp bop sexp
 
 sop : SL | SR
 sexp : aexp | sexp sop aexp
 
-aop : ADD | SUB | MOD
-aexp : wire | aexp aop wire
+aop : ADD | SUB
+aexp : mexp | aexp aop mexp
 
-uop : NOT | NEG
+mop : MOD
+mexp : wire | mexp mop wire
+
+uop : INV | NEG | NOT
 type : CONST | TIME
 top : FROM | AFTER | UNTIL | BEFORE
 tsop : NEXT | PREV
-wire : NAME | "(" lexp ")" | uop wire | type NUM 
-    | top wire | tsop wire | NUM tsop wire | ACC wire
+
+call : NAME "(" args ")"
+args : wire ("," wire)*
+
+wire : NAME | "(" lexp ")" | uop wire | type NUM | top wire | tsop wire 
+    | NUM tsop wire | ACC wire | call
+
+expr : lexp
+exprs : expr ("," expr)*
```

### Comparing `sootty-0.2.3/sootty/storage/valuechange.py` & `sootty-0.3/sootty/storage/valuechange.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from vcd.reader import *
 from itertools import islice
 from sortedcontainers import SortedDict, SortedList, SortedSet
 
 from ..exceptions import *
 
 
@@ -39,54 +38,75 @@
                 prev = i
             else:
                 prev = None
         if prev is not None and end is not None and end > prev:
             indices.extend(range(prev + 1, end))
         return indices
 
+    def _to_bool(self):
+        data = ValueChange(width=1)
+        for key in self:
+            data[key] = None if self[key] == None else (int(bool(self[key])))
+        return data
+
     def __invert__(self):
         data = ValueChange(width=self.width)
         for key in self:
             data[key] = (
                 None if self[key] == None else (~self[key] & (2 << self.width - 1) - 1)
             )
         return data
 
     def __neg__(self):
         data = ValueChange(width=self.width)
         for key in self:
             data[key] = None if self[key] == None else (-self[key])
         return data
 
-    def _binop(self, other, binop, width):
+    def __not__(self):
+        return not (self.width)
+
+    def _binop(self, other, binop, width, xz_flag=0):
         data = ValueChange(width=width)
         keys = SortedSet()
         keys.update(self.keys())
         keys.update(other.keys())
         values = [None, None, None]
         for key in keys:
+            reduced = None
             if key in self:
                 values[0] = self[key]
             if key in other:
                 values[1] = other[key]
-            reduced = (
-                None
-                if (values[0] is None or values[1] is None)
-                else binop(values[0], values[1])
-            )
+            if xz_flag == 1:
+                if values[0] == 0 or values[1] == 0:  # xz = 1 is logical and
+                    reduced = 0
+            if xz_flag == 2:  # xz = 2 is logical or
+                if values[0] == 1 or values[1] == 1:
+                    reduced = 1
+            if reduced is None:
+                reduced = (
+                    None
+                    if (
+                        (values[0] is None or values[1] is None)
+                        or (type(values[0]) == str)
+                        or (type(values[1]) == str)
+                    )
+                    else binop(values[0], values[1])
+                )
             if reduced != values[2]:
                 values[2] = reduced
                 data[key] = reduced
         return data
 
     def __and__(self, other):
-        return self._binop(other, lambda x, y: x & y, max(self.width, other.width))
+        return self._binop(other, lambda x, y: x & y, max(self.width, other.width), 1)
 
     def __or__(self, other):
-        return self._binop(other, lambda x, y: x | y, max(self.width, other.width))
+        return self._binop(other, lambda x, y: x | y, max(self.width, other.width), 2)
 
     def __xor__(self, other):
         return self._binop(other, lambda x, y: x ^ y, max(self.width, other.width))
 
     def __eq__(self, other):
         return self._binop(other, lambda x, y: int(x == y), 1)
```

### Comparing `sootty-0.2.3/sootty/storage/wire.py` & `sootty-0.3/sootty/storage/wire.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from itertools import compress, chain
 
 from ..exceptions import *
 from .valuechange import ValueChange
 
 
 class Wire:
@@ -79,14 +78,29 @@
         return wire
 
     def __xor__(self, other):
         wire = Wire(name="(" + self.name + " ^ " + other.name + ")")
         wire._data = self._data.__xor__(other._data)
         return wire
 
+    def _logical_not(self):
+        wire = Wire(name="!" + self.name)
+        wire._data = self._data._to_bool().__invert__()
+        return wire
+
+    def _logical_and(self, other):
+        wire = Wire(name="(" + self.name + " && " + other.name + ")")
+        wire._data = self._data._to_bool().__and__(other._data._to_bool())
+        return wire
+
+    def _logical_or(self, other):
+        wire = Wire(name="(" + self.name + " || " + other.name + ")")
+        wire._data = self._data._to_bool().__or__(other._data._to_bool())
+        return wire
+
     def __eq__(self, other):
         wire = Wire(name="(" + self.name + " == " + other.name + ")")
         wire._data = self._data.__eq__(other._data)
         return wire
 
     def __ne__(self, other):
         wire = Wire(name="(" + self.name + " != " + other.name + ")")
```

### Comparing `sootty-0.2.3/sootty/storage/wiregroup.py` & `sootty-0.3/sootty/storage/wiregroup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-
 from ..exceptions import *
 from .wire import Wire
 
 
 class WireGroup:
     def __init__(self, name: str):
         self.name = name
@@ -42,7 +40,19 @@
         """Returns list of all wire names."""
         names = set()
         for wire in self.wires:
             names.add(wire.name)
         for group in self.groups:
             names.update(group.get_names())
         return names
+    
+    def get_wires(self):
+        """Returns a dictionary of all wires of this wiregroup or a list if this wiregroup is the innermost one."""
+        if self.groups:
+            wires = dict()
+            if self.wires:
+                wires[self.name] = self.wires
+            for group in self.groups:
+                wires[group.name] = group.get_wires()
+        else:
+            wires = self.wires
+        return wires
```

### Comparing `sootty-0.2.3/sootty/storage/wiretrace.py` & `sootty-0.3/sootty/storage/wiretrace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,92 @@
-import json, sys
+import sys
 from vcd.reader import *
 
 from ..exceptions import *
-from ..limits import LimitExpression
+from ..parser import parser
 from .wiregroup import WireGroup
 from .wire import Wire
+from ..utils import evcd2vcd
 
 
 class WireTrace:
     def __init__(self):
         self.root = WireGroup("__root__")
 
     @classmethod
     def from_vcd(cls, filename):
         """
         Construct a WireTrace object from a parsed vcd file, using the pyvcd library.
 
-        Syntax of four-state VCD file (IEEE 1364-2005 §18.2.1):
+        Syntax of 4-state VCD file (IEEE 1800-2017 §21.7.2):
 
         value_change_dump_definitions ::=
-            { declaration_command }{ simulation_command }
+             { declaration_command }{ simulation_command }
         declaration_command ::=
-            declaration_keyword
-            [ command_text ]
-            $end
+             $comment [ comment_text ] $end
+           | $date [ date_text ] $end
+           | $enddefinitions $end
+           | $scope [ scope_type scope_identifier ] $end
+           | $timescale [ time_number time_unit ] $end
+           | $upscope $end
+           | $var [ var_type size identifier_code reference ] $end
+           | $version [ version_text system_task ] $end
         simulation_command ::=
-            simulation_keyword { value_change } $end
-            | $comment [ comment_text ] $end
-            | simulation_time
-            | value_change
-        declaration_keyword ::=
-            $comment | $date | $enddefinitions | $scope | $timescale | $upscope
-            | $var | $version
-        simulation_keyword ::=
-            $dumpall | $dumpoff | $dumpon | $dumpvars
-        simulation_time ::=
-            # decimal_number
+             $dumpall { value_change } $end
+           | $dumpoff { value_change } $end
+           | $dumpon { value_change } $end
+           | $dumpvars { value_change } $end
+           | $comment [ comment_text ] $end
+           | simulation_time
+           | value_change
+        scope_type ::=
+             begin
+           | fork
+           | function
+           | module
+           | task
+        time_number ::= 1 | 10 | 100
+        time_unit ::= s | ms | us | ns | ps | fs
+        var_type ::=
+            event | integer | parameter | real | realtime | reg | supply0 | supply1 | time
+           | tri | triand | trior | trireg | tri0 | tri1 | wand | wire | wor
+        simulation_time ::= # decimal_number
         value_change ::=
-            scalar_value_change
-            | vector_value_change
-        scalar_value_change ::=
-            value identifier_code
-        value ::=
-            0 | 1 | x | X | z | Z
+             scalar_value_change
+           | vector_value_change
+        scalar_value_change ::= value identifier_code
+        value ::= 0 | 1 | x | X | z | Z
         vector_value_change ::=
-            b binary_number identifier_code
-            | B binary_number identifier_code
-            | r real_number identifier_code
-            | R real_number identifier_code
-        identifier_code ::=
-            { ASCII character }
+             b binary_number identifier_code
+           | B binary_number identifier_code
+           | r real_number identifier_code
+           | R real_number identifier_code
+        identifier_code ::= { ASCII character }
+        size ::= decimal_number
+        reference ::=
+             identifier
+           | identifier [ bit_select_index ]
+           | identifier [ msb_index : lsb_index ]
+        index ::= decimal_number
+        scope_identifier ::= { ASCII character }
+        comment_text ::= { ASCII character }
+        date_text ::= { ASCII character }
+        version_text ::= { ASCII character }
+        system_task ::= ${ASCII character}
         """
 
         this = cls()
         this.metadata = dict()  # dictionary of vcd metadata
         wires = dict()  # map from id_code to wire object
         stack = [this.root]  # store stack of current group for scoping
 
         with open(filename, "rb") as stream:
+            if filename.endswith(".evcd"):
+                stream = evcd2vcd(stream)
+
             tokens = tokenize(stream)
             for token in tokens:
                 if token.kind is TokenKind.COMMENT:
                     this.metadata["comment"] = token.comment
                 elif token.kind is TokenKind.DATE:
                     this.metadata["date"] = token.date
                 elif token.kind is TokenKind.ENDDEFINITIONS:
@@ -155,102 +180,143 @@
         """Returns the wire object with the given name, raises an error if not found."""
         return self.root.find(name)
 
     def get_wire_names(self):
         """Returns list of all wire names."""
         return self.root.get_names()
 
-    def evaluate(self, expr: str):
-        wire = self._compute_wire(LimitExpression(expr).tree)
-        return wire.times(self.length())
+    def _compute_wire(self, node):
+        """Evaluate a limit expression"""
+        if node.data == "wire":
+            return self.find(node.children[0])
+        elif node.data == "call":
+            name = node.children[0]
+            args = list(map(self._compute_wire, node.children[1].children))
+            if name == "AXI":
+                return args[0]  # TODO: implement axi protocol
+            raise SoottyError(f'Function "{name}" does not exist.')
+        elif node.data.type == "NEG":
+            return self._compute_wire(node.children[0]).__neg__()
+        elif node.data.type == "INV":
+            return self._compute_wire(node.children[0]).__invert__()
+        elif node.data.type == "AND":
+            return self._compute_wire(node.children[0]) & self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "OR":
+            return self._compute_wire(node.children[0]) | self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "XOR":
+            return self._compute_wire(node.children[0]) ^ self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "LNOT":
+            return self._compute_wire(node.children[0])._logical_not()
+        elif node.data.type == "LAND":
+            return self._compute_wire(node.children[0])._logical_and(
+                self._compute_wire(node.children[1])
+            )
+        elif node.data.type == "LOR":
+            return self._compute_wire(node.children[0])._logical_or(
+                self._compute_wire(node.children[1])
+            )
+        elif node.data.type == "EQ":
+            return self._compute_wire(node.children[0]) == self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "NEQ":
+            return self._compute_wire(node.children[0]) != self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "GT":
+            return self._compute_wire(node.children[0]) > self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "GEQ":
+            return self._compute_wire(node.children[0]) >= self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "LT":
+            return self._compute_wire(node.children[0]) < self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "LEQ":
+            return self._compute_wire(node.children[0]) <= self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "SL":
+            return self._compute_wire(node.children[0]) << self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "SR":
+            return self._compute_wire(node.children[0]) >> self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "ADD":
+            return self._compute_wire(node.children[0]) + self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "SUB":
+            return self._compute_wire(node.children[0]) - self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "MOD":
+            return self._compute_wire(node.children[0]) % self._compute_wire(
+                node.children[1]
+            )
+        elif node.data.type == "FROM":
+            return self._compute_wire(node.children[0])._from()
+        elif node.data.type == "AFTER":
+            return self._compute_wire(node.children[0])._after()
+        elif node.data.type == "UNTIL":
+            return self._compute_wire(node.children[0])._until()
+        elif node.data.type == "BEFORE":
+            return self._compute_wire(node.children[0])._before()
+        elif node.data.type == "NEXT":
+            return self._compute_wire(node.children[0])._next()
+        elif node.data.type == "PREV":
+            return self._compute_wire(node.children[0])._prev()
+        elif node.data.type == "ACC":
+            return self._compute_wire(node.children[0])._acc()
+        elif node.data.type == "CONST":
+            return Wire.const(int(node.children[0]))
+        elif node.data.type == "TIME":
+            return Wire.time(int(node.children[0]))
+
+    def compute_wire(self, expr: str):
+        """Evaluate a limit expression to a wire."""
+        return self._compute_wire(parser.parse(expr))
+
+    def compute_wires(self, exprs: str):
+        """Evaluate comma-separated limit expressions as a list of wires."""
+        return list(map(self._compute_wire, parser.parse_list(exprs)))
 
-    def _compute_wire(self, expr):
-        """
-        Evaluate a limit expression
-        """
-        if expr.data == "wire":
-            return self.find(expr.children[0])
-        elif expr.data.type == "NOT":
-            return ~self._compute_wire(expr.children[0])
-        elif expr.data.type == "NEG":
-            return -self._compute_wire(expr.children[0])
-        elif expr.data.type == "AND":
-            return self._compute_wire(expr.children[0]) & self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "OR":
-            return self._compute_wire(expr.children[0]) | self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "XOR":
-            return self._compute_wire(expr.children[0]) ^ self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "EQ":
-            return self._compute_wire(expr.children[0]) == self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "NEQ":
-            return self._compute_wire(expr.children[0]) != self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "GT":
-            return self._compute_wire(expr.children[0]) > self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "GEQ":
-            return self._compute_wire(expr.children[0]) >= self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "LT":
-            return self._compute_wire(expr.children[0]) < self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "LEQ":
-            return self._compute_wire(expr.children[0]) <= self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "SL":
-            return self._compute_wire(expr.children[0]) << self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "SR":
-            return self._compute_wire(expr.children[0]) >> self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "ADD":
-            return self._compute_wire(expr.children[0]) + self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "SUB":
-            return self._compute_wire(expr.children[0]) - self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "MOD":
-            return self._compute_wire(expr.children[0]) % self._compute_wire(
-                expr.children[1]
-            )
-        elif expr.data.type == "FROM":
-            return self._compute_wire(expr.children[0])._from()
-        elif expr.data.type == "AFTER":
-            return self._compute_wire(expr.children[0])._after()
-        elif expr.data.type == "UNTIL":
-            return self._compute_wire(expr.children[0])._until()
-        elif expr.data.type == "BEFORE":
-            return self._compute_wire(expr.children[0])._before()
-        elif expr.data.type == "NEXT":
-            return self._compute_wire(expr.children[0])._next()
-        elif expr.data.type == "PREV":
-            return self._compute_wire(expr.children[0])._prev()
-        elif expr.data.type == "ACC":
-            return self._compute_wire(expr.children[0])._acc()
-        elif expr.data.type == "CONST":
-            return Wire.const(int(expr.children[0]))
-        elif expr.data.type == "TIME":
-            return Wire.time(int(expr.children[0]))
+    def evaluate(self, expr: str):
+        return self.compute_wire(expr).times(self.length())
 
     def compute_limits(self, start_expr: str, end_expr: str):
         starts = self.evaluate(start_expr)
         start = starts[0] if len(starts) > 0 else 0
         ends = list(filter(lambda time: time > start, self.evaluate(end_expr)))
         end = ends[0] if len(ends) else self.length()
         return (start, end)
+    
+    def print_breakpoints(self, breakpoints: list):
+        """
+        Print a table of wires and their values.
+        """
+        def rec_print(wires):
+            for scope, sub in wires.items():
+                if type(sub) is dict:
+                    print("scope\t" + scope)
+                    rec_print(sub)
+                else:  # is list
+                    print("scope\t" + scope)
+                    for wire in sub:
+                        print(wire.name, end="\t")
+                        for breakpoint in breakpoints:
+                            print(str(wire._data.get(breakpoint)), end="\t")
+                        print()
+        
+        print("time", *breakpoints, sep="\t")
+        rec_print(self.root.get_wires())
```

### Comparing `sootty-0.2.3/sootty/visualizer.py` & `sootty-0.3/sootty/visualizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-import sys
+import html
 from enum import Enum
 
 from .display import VectorImage
 from .exceptions import SoottyInternalError
+from .utils import dec2anybase
 
 
 class Style:
     """Container class for visualizer style settings."""
 
     class Default:
         TOP_MARGIN = 15
         LEFT_MARGIN = 15
         CHAR_WIDTH = 7
-        LABEL_WIDTH = 12
-        TEXT_WIDTH = CHAR_WIDTH * LABEL_WIDTH
+        LABEL_WIDTH = 10
+        TEXT_WIDTH = CHAR_WIDTH * (LABEL_WIDTH + 2)
         FULL_WIDTH = 800
         WIRE_HEIGHT = 20
         WIRE_MARGIN = 10
         TRANS_START = 5
         TRANS_WIDTH = 5
         BLOCK_TRANS = False
         LINE_COLOR = "#FFFFFF"  # line color now needs to be its own class (?) depending on wires and variables
         LINE_COLOR_HIGH = "#00FF00"
         LINE_COLOR_LOW = "#3DB8B8"
         LINE_COLOR_Z = "#FFFF00"
         LINE_COLOR_X = "#FF0000"
         LINE_COLOR_DATA = "#3DB8B8"
-        BREAKPOINT_COLOR = "#FFFF00"
+        BREAKPOINT_COLOR_LIST = ["#FFFF00"]
         TEXT_COLOR = "#FFFFFF"
         BKGD_COLOR = "#000000"
         # wires going from 0 and 1 are two different colors, x variable is red rectangle, z variable is yellow
+        # breakpoints: Han Purple, Orange, Erin, Electric Purple, Aqua, Tart Orange, Gainsboro, Slimy Green, Yellow Pantone
 
     class Dark(Default):
         pass
 
     class Light(Default):
         LINE_COLOR = "#000000"
         LINE_COLOR_HIGH = "#2e9947"
@@ -50,39 +52,67 @@
         LINE_COLOR_Z = "#7a5b1b"
         LINE_COLOR_X = "#faf6bb"
         # TEXT_COLOR = "#30FF30"
         TEXT_COLOR = "#FFFFFF"
         # BKGD_COLOR = "#003000"
         BKGD_COLOR = "#2b5e2b"
 
+    class Colorful(Default):
+        BREAKPOINT_COLOR_LIST = ["#2829FF", "#FF8314", "#48FF45", "#C200DD", "#26F0F6", "#FF3D3B", "#E1E1E1", "#1A9D1F", "#FDE12D"]
+
     class Debug(Default):
         pass
 
 
 class Visualizer:
     """Converter for wiretrace objects to a svg vector image format."""
 
     def __init__(self, style=Style.Default):
         """Optionally pass in a style class to control how the visualizer looks."""
         self.style = style
 
-    def to_svg(self, wiretrace, start=0, length=None, wires=None, breakpoints=None):
+    def to_svg(
+        self,
+        wiretrace,
+        start=0,
+        length=None,
+        wires="",
+        breakpoints=None,
+        vector_radix=10,
+    ):
+        """
+        Converts the provided wiretrace object to a VectorImage object (svg).
+
+        :param wires: comma-seperated list of wires to include
+        """
         if length is None:
             length = wiretrace.length()
-        """Converts the provided wiretrace object to a VectorImage object (svg)."""
+
+        if wires is not None:  # include all wires if empty list provided
+            wires = (
+                None
+                if len(wires) == 0
+                else set(
+                    map(lambda wire: wire.name, wiretrace.compute_wires(wires.strip()))
+                )
+            )
+
         return VectorImage(
-            self._wiretrace_to_svg(wiretrace, start, length, wires, breakpoints)
+            self._wiretrace_to_svg(
+                wiretrace, start, length, wires, breakpoints, vector_radix
+            )
         )
 
-    def _wiretrace_to_svg(self, wiretrace, start, length, wires=None, breakpoints=None):
-        if wires and len(wires) == 0:  # include all wires if empty list provided
-            wires = None
+    def _wiretrace_to_svg(
+        self, wiretrace, start, length, wires=None, breakpoints=None, vector_radix=10
+    ):
         width = (
             2 * self.style.LEFT_MARGIN + self.style.TEXT_WIDTH + self.style.FULL_WIDTH
         )
+
         height = (
             2 * self.style.TOP_MARGIN
             - self.style.WIRE_MARGIN
             + (self.style.WIRE_HEIGHT + self.style.WIRE_MARGIN)
             * (1 + (len(wires) if wires else wiretrace.num_wires()))
         )
 
@@ -105,24 +135,42 @@
             left=self.style.LEFT_MARGIN + self.style.TEXT_WIDTH,
             top=self.style.TOP_MARGIN,
             start=start,
             length=length,
             height=height - 2 * self.style.TOP_MARGIN + self.style.WIRE_MARGIN,
         )
 
-        svg += self._wiregroup_to_svg(
+        # Add the root wiregroup to the image.
+        result = self._wiregroup_to_svg(
             wiregroup=wiretrace.root,
             left=self.style.LEFT_MARGIN,
             top=self.style.TOP_MARGIN + self.style.WIRE_HEIGHT + self.style.WIRE_MARGIN,
             start=start,
             length=length,
             wires=wires,
-        )[
-            0
-        ]  # the first element is the svg data
+            vector_radix=vector_radix,
+        )
+        svg += result[0]
+        index = result[1]
+
+        # Add each composite wire to the image.
+        if wires is not None:
+            for wire in wires:
+                svg += self._wire_to_svg(
+                    wiretrace.compute_wire(wire),
+                    left=self.style.LEFT_MARGIN,
+                    top=self.style.TOP_MARGIN
+                    + self.style.WIRE_HEIGHT
+                    + self.style.WIRE_MARGIN
+                    + (index * (self.style.WIRE_HEIGHT + self.style.WIRE_MARGIN)),
+                    start=start,
+                    length=length,
+                )
+                index += 1
+            wires.clear()  # TODO: fix temporary solution for catching exceptions
 
         svg += "</svg>"
         return svg
 
     def _timestamps_to_svg(self, left, top, start, length):
         svg = ""
         for index in range(start, start + length, ((length - 1) // 32) + 1):
@@ -140,84 +188,93 @@
                 }
             )
         return svg
 
     def _breakpoints_to_svg(self, breakpoints, left, top, start, length, height):
         """Convert a list of breakpoint times to highlights on the svg."""
         svg = ""
-        for index in breakpoints:
+        for i, index in enumerate(breakpoints):
             if index >= start and index < start + length:
                 svg += self._shape_to_svg(
                     {
                         "name": "rect",
                         "x": left
                         + (index - start) * (self.style.FULL_WIDTH / length)
                         + self.style.TRANS_START,
                         "y": top,
                         "width": (self.style.FULL_WIDTH / length),
                         "height": height,
-                        "fill": self.style.BREAKPOINT_COLOR,
+                        "fill": self.style.BREAKPOINT_COLOR_LIST[i % len(self.style.BREAKPOINT_COLOR_LIST)],
                         "fill-opacity": 0.4,
                     }
                 )
         return svg
 
-    def _wiregroup_to_svg(self, wiregroup, left, top, start, length, wires=None):
+    def _wiregroup_to_svg(
+        self, wiregroup, left, top, start, length, wires=None, vector_radix=10
+    ):
         svg = ""
         index = 0
         for wire in wiregroup.wires:
             if wires == None or wire.name in wires:
                 if wires:  # ensure only one copy of the wire is included
                     wires.remove(wire.name)
                 svg += self._wire_to_svg(
                     wire,
                     left=left,
                     top=top
                     + (index * (self.style.WIRE_HEIGHT + self.style.WIRE_MARGIN)),
                     start=start,
                     length=length,
+                    vector_radix=vector_radix,
                 )
                 index += 1
         # recursively call function on nested wiregroups
         for group in wiregroup.groups:
             result = self._wiregroup_to_svg(
                 group,
                 left=left,
                 top=top + (index * (self.style.WIRE_HEIGHT + self.style.WIRE_MARGIN)),
                 start=start,
                 length=length,
                 wires=wires,
+                vector_radix=vector_radix,
             )
             svg += result[0]
             index += result[1]
         return svg, index
 
-    def _wire_to_svg(self, wire, left, top, start, length):
+    def _wire_to_svg(self, wire, left, top, start, length, vector_radix=10):
         svg = self._shape_to_svg(
             {
                 "name": "text",
                 "x": left,
                 "y": top + 15,
                 "class": "small",
                 "fill": self.style.TEXT_COLOR,
                 "font-family": "monospace",
-                "content": wire.name if len(wire.name) <= 10 else wire.name[:7] + "...",
+                "content": html.escape(
+                    wire.name
+                    if len(wire.name) <= self.style.LABEL_WIDTH
+                    else wire.name[: max(self.style.LABEL_WIDTH - 3, 0)] + "..."
+                ),
             }
         )
         for index in range(start, start + length):
             svg += self._value_to_svg(
                 prev=wire[index - 1] if index > 0 else wire[index],
                 value=wire[index],
                 width=wire.width(),
                 left=left
                 + ((index - start) * (self.style.FULL_WIDTH / length))
                 + self.style.TEXT_WIDTH,
                 top=top,
                 length=length,
                 initial=(index == start),
+                vector_radix=vector_radix,
             )
         return svg
 
     class ValueType(Enum):
         LOW = 0
         HIGH = 1
         DATA = 2
@@ -243,20 +300,25 @@
                 )
         else:
             if "x" in str(value):
                 return Visualizer.ValueType.X
             else:
                 return Visualizer.ValueType.DATA
 
-    def _value_to_svg(self, prev, value, width, left, top, length, initial=False):
+    def _value_to_svg(
+        self, prev, value, width, left, top, length, initial=False, vector_radix=10
+    ):
         # deduce types from wire width and value:
         prev_type = Visualizer.type_from_value(prev, width)
         value_type = Visualizer.type_from_value(value, width)
         is_transitioning = prev != value
 
+        if vector_radix != 10 and value_type == Visualizer.ValueType.DATA:
+            value = dec2anybase(value, vector_radix, width)
+
         # The following code builds a list of svg objects depending on the
         # current and previous value of the wire.
         shapes = []
         if (
             prev_type is Visualizer.ValueType.LOW
             and value_type is Visualizer.ValueType.LOW
         ):
```

