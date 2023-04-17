# Comparing `tmp/ib110hw-0.1.1.tar.gz` & `tmp/ib110hw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib110hw-0.1.1.tar", last modified: Sun Apr 16 21:36:31 2023, max compression
+gzip compressed data, was "ib110hw-0.1.2.tar", last modified: Mon Apr 17 08:44:02 2023, max compression
```

## Comparing `ib110hw-0.1.1.tar` & `ib110hw-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.507216 ib110hw-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    26595 2023-04-16 21:36:31.507216 ib110hw-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    26213 2023-04-16 21:05:41.000000 ib110hw-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 21:36:31.508216 ib110hw-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-04-16 21:36:12.000000 ib110hw-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.466218 ib110hw-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.472217 ib110hw-0.1.1/src/ib110hw/
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.1/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.493217 ib110hw-0.1.1/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.1/src/ib110hw/automaton/__init__.py
--rw-rw-rw-   0        0        0     2304 2023-04-16 00:59:04.000000 ib110hw-0.1.1/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8262 2023-04-16 19:56:06.000000 ib110hw-0.1.1/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8539 2023-04-16 19:56:24.000000 ib110hw-0.1.1/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1439 2023-02-10 23:11:04.000000 ib110hw-0.1.1/src/ib110hw/automaton/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.501217 ib110hw-0.1.1/src/ib110hw/turing/
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.1/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0     4911 2023-04-11 20:33:53.000000 ib110hw-0.1.1/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.1/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.1/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.1/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.1/src/ib110hw/turing/tape.py
--rw-rw-rw-   0        0        0     1186 2023-04-16 21:34:51.000000 ib110hw-0.1.1/src/ib110hw/turing/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.488215 ib110hw-0.1.1/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0    26595 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.505216 ib110hw-0.1.1/tests/
--rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.1/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.1/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.1/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.1/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.309251 ib110hw-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    26675 2023-04-17 08:44:02.309251 ib110hw-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    26293 2023-04-17 08:42:12.000000 ib110hw-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:44:02.309251 ib110hw-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-04-17 08:42:50.000000 ib110hw-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.261225 ib110hw-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.269228 ib110hw-0.1.2/src/ib110hw/
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.2/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.301249 ib110hw-0.1.2/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.2/src/ib110hw/automaton/__init__.py
+-rw-rw-rw-   0        0        0     2304 2023-04-16 00:59:04.000000 ib110hw-0.1.2/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8286 2023-04-17 08:04:31.000000 ib110hw-0.1.2/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8539 2023-04-16 19:56:24.000000 ib110hw-0.1.2/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.2/src/ib110hw/automaton/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.309251 ib110hw-0.1.2/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.2/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0     5031 2023-04-17 08:11:17.000000 ib110hw-0.1.2/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.2/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.2/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.2/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.2/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     1246 2023-04-17 08:14:21.000000 ib110hw-0.1.2/src/ib110hw/turing/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.293254 ib110hw-0.1.2/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0    26675 2023-04-17 08:44:02.000000 ib110hw-0.1.2/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-04-17 08:44:02.000000 ib110hw-0.1.2/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:44:02.000000 ib110hw-0.1.2/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 08:44:02.000000 ib110hw-0.1.2/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 08:44:02.309251 ib110hw-0.1.2/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.2/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.2/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.2/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.2/tests/test_nfa.py
```

### Comparing `ib110hw-0.1.1/LICENSE` & `ib110hw-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/PKG-INFO` & `ib110hw-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: ib110hw
-Version: 0.1.1
-Home-page: https://github.com/pilatmartin/ib110hw
-Author: Martin Pilát
-Author-email: 8pilatmartin8@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 This library was created for the course **IB110 - Introduction to Informatics** at [MUNI FI](https://www.fi.muni.cz/).
 
 # INSTALLATION
 
-Using virtual environment is of course optional, but recommended.
+Python version >=3.6 is required in order to use the library.
+Using virtual environment for installation is of course optional, but recommended.
 
 ```sh
 # Bash
 $ python3 -m venv <name> 
 $ source <name>/bin/activate
 $ pip install ib110hw
 ```
```

### Comparing `ib110hw-0.1.1/README.md` & `ib110hw-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,25 @@
+Metadata-Version: 2.1
+Name: ib110hw
+Version: 0.1.2
+Home-page: https://github.com/pilatmartin/ib110hw
+Author: Martin Pilát
+Author-email: 8pilatmartin8@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 This library was created for the course **IB110 - Introduction to Informatics** at [MUNI FI](https://www.fi.muni.cz/).
 
 # INSTALLATION
 
-Using virtual environment is of course optional, but recommended.
+Python version >=3.6 is required in order to use the library.
+Using virtual environment for installation is of course optional, but recommended.
 
 ```sh
 # Bash
 $ python3 -m venv <name> 
 $ source <name>/bin/activate
 $ pip install ib110hw
 ```
```

### Comparing `ib110hw-0.1.1/setup.py` & `ib110hw-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.1.1",
+    version="0.1.2",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ib110hw-0.1.1/src/ib110hw/automaton/base.py` & `ib110hw-0.1.2/src/ib110hw/automaton/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.2/src/ib110hw/automaton/dfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,16 @@
             bool: True if word is accepted, False otherwise.
         """
         assert self.is_valid(), "DFA needs to be valid."
 
         current_state = self.initial_state
 
         for symbol in input_string:
-            if not (current_state := self.get_transition(current_state, symbol)):
+            current_state = self.get_transition(current_state, symbol)
+            if not current_state:
                 return False
 
         return current_state in self.final_states
 
     def is_valid(self) -> bool:
         """
         Checks whether the DFA is valid:
```

### Comparing `ib110hw-0.1.1/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.2/src/ib110hw/automaton/nfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.2/src/ib110hw/automaton/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         for s_from in automaton.states:
             for s_to in automaton.states:
                 label_symbols = automaton.get_symbols_between_states(s_from, s_to)
                 if "" in label_symbols:
                     label_symbols.discard("")
                     label_symbols.add("ε")
 
-                if label := ",".join(label_symbols):
+                label = ",".join(label_symbols)
+                if label:
                     file.write(f'\t{s_from} -> {s_to}[label="{label}"]\n')
 
         for non_fin_state in automaton.states.difference(automaton.final_states):
             file.write(f"\t{non_fin_state} [shape=circle]\n")
 
         for fin_state in automaton.final_states:
             file.write(f"\t{fin_state} [shape=doublecircle]\n")
```

### Comparing `ib110hw-0.1.1/src/ib110hw/turing/_helpers.py` & `ib110hw-0.1.2/src/ib110hw/turing/_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,16 +102,17 @@
         return "The divider is missing."
 
     config = list(takewhile(lambda l: l != "---", definition))[:-1]
 
     if not any((l.startswith("init") for l in config)):
         return "Specifying the initial state is mandatory."
 
-    if l := next((l for l in config if l.startswith("init")), None):
-        if len(l.split()) != 2:
+    init_line = next((l for l in config if l.startswith("init")), None)
+    if init_line:
+        if len(init_line.split()) != 2:
             return "Invalid initial state"
 
 
 def validate_dtm_transitions(definition: List[str]) -> Optional[str]:
     lines = list(dropwhile(lambda l: l != "---", definition))[1:]
     get_part = lambda l, i: l.split("->")[i]
     # checks the length of arguments on the left side
@@ -121,28 +122,34 @@
     # checks the length of arguments on the right side
     valid_next = lambda l: len(get_part(l, 1).split()) == 3
     # checks the length of the write symbol
     valid_write = lambda l: len(get_part(l, 1).split()[1]) == 1
     # checks the direction
     valid_dir = lambda l: get_part(l, 1).split()[-1] in ["L", "R", "S"]
 
-    if l := next((l for l in lines if "->" not in l), None):
-        return f"Missing arrow in rule:\n{l}."
-
-    if l := next((l for l in lines if not valid_current(l)), None):
-        return f"Invalid combination of state and read symbol in rule:\n{l}"
-
-    if l := next((l for l in lines if not valid_read(l)), None):
-        return f"Invalid read symbol length (> 1) in rule\n{l}"
-
-    if l := next((l for l in lines if not valid_next(l)), None):
-        return f"The next state, write symbol or direction is missing in rule:\n{l}"
-
-    if l := next((l for l in lines if not valid_write(l)), None):
-        return f"Invalid write symbol length (> 1) in rule\n{l}"
-
-    if l := next((l for l in lines if not valid_dir(l)), None):
-        return f"Invalid direction in rule:\n{l}"
+    rule = next((l for l in lines if "->" not in l), None)
+    if rule:
+        return f"Missing arrow in rule:\n{rule}."
+
+    rule = next((l for l in lines if not valid_current(l)), None)
+    if rule:
+        return f"Invalid combination of state and read symbol in rule:\n{rule}"
+
+    rule = next((l for l in lines if not valid_read(l)), None)
+    if rule:
+        return f"Invalid read symbol length (> 1) in rule\n{rule}"
+
+    rule = next((l for l in lines if not valid_next(l)), None)
+    if rule:
+        return f"The next state, write symbol or direction is missing in rule:\n{rule}"
+
+    rule = next((l for l in lines if not valid_write(l)), None)
+    if rule:
+        return f"Invalid write symbol length (> 1) in rule\n{rule}"
+
+    rule = next((l for l in lines if not valid_dir(l)), None)
+    if rule:
+        return f"Invalid direction in rule:\n{rule}"
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `ib110hw-0.1.1/src/ib110hw/turing/base.py` & `ib110hw-0.1.2/src/ib110hw/turing/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/src/ib110hw/turing/dtm.py` & `ib110hw-0.1.2/src/ib110hw/turing/dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/src/ib110hw/turing/mtm.py` & `ib110hw-0.1.2/src/ib110hw/turing/mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/src/ib110hw/turing/tape.py` & `ib110hw-0.1.2/src/ib110hw/turing/tape.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/src/ib110hw.egg-info/PKG-INFO` & `ib110hw-0.1.2/src/ib110hw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This library was created for the course **IB110 - Introduction to Informatics** at [MUNI FI](https://www.fi.muni.cz/).
 
 # INSTALLATION
 
-Using virtual environment is of course optional, but recommended.
+Python version >=3.6 is required in order to use the library.
+Using virtual environment for installation is of course optional, but recommended.
 
 ```sh
 # Bash
 $ python3 -m venv <name> 
 $ source <name>/bin/activate
 $ pip install ib110hw
 ```
```

### Comparing `ib110hw-0.1.1/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.2/src/ib110hw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/tests/test_dfa.py` & `ib110hw-0.1.2/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/tests/test_dtm.py` & `ib110hw-0.1.2/tests/test_dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/tests/test_mtm.py` & `ib110hw-0.1.2/tests/test_mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.1/tests/test_nfa.py` & `ib110hw-0.1.2/tests/test_nfa.py`

 * *Files identical despite different names*

