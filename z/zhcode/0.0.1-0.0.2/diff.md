# Comparing `tmp/zhcode-0.0.1.tar.gz` & `tmp/zhcode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcode-0.0.1.tar", last modified: Sat Apr 15 04:04:51 2023, max compression
+gzip compressed data, was "zhcode-0.0.2.tar", last modified: Mon Apr 17 00:07:07 2023, max compression
```

## Comparing `zhcode-0.0.1.tar` & `zhcode-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-15 04:04:51.334435 zhcode-0.0.1/
--rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-14 00:50:18.000000 zhcode-0.0.1/LICENSE
--rw-r--r--   0 lnjng      (501) staff       (20)      129 2023-04-15 04:04:51.334109 zhcode-0.0.1/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)     1077 2023-04-14 16:58:54.000000 zhcode-0.0.1/README.md
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-15 04:04:51.332224 zhcode-0.0.1/python/
--rw-r--r--   0 lnjng      (501) staff       (20)       13 2023-04-15 04:01:55.000000 zhcode-0.0.1/python/__init__.py
--rw-r--r--   0 lnjng      (501) staff       (20)     9435 2023-04-14 20:46:17.000000 zhcode-0.0.1/python/main.py
--rw-r--r--   0 lnjng      (501) staff       (20)     3017 2023-04-15 03:51:28.000000 zhcode-0.0.1/python/stdlib.py
--rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-15 04:04:51.334564 zhcode-0.0.1/setup.cfg
--rw-r--r--   0 lnjng      (501) staff       (20)      204 2023-04-15 04:04:50.000000 zhcode-0.0.1/setup.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-15 04:04:51.333540 zhcode-0.0.1/zhcode.egg-info/
--rw-r--r--   0 lnjng      (501) staff       (20)      129 2023-04-15 04:04:51.000000 zhcode-0.0.1/zhcode.egg-info/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)      197 2023-04-15 04:04:51.000000 zhcode-0.0.1/zhcode.egg-info/SOURCES.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-15 04:04:51.000000 zhcode-0.0.1/zhcode.egg-info/dependency_links.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-15 04:04:51.000000 zhcode-0.0.1/zhcode.egg-info/top_level.txt
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.059444 zhcode-0.0.2/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.0.2/LICENSE
+-rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 00:07:07.058884 zhcode-0.0.2/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)     1127 2023-04-16 22:16:34.000000 zhcode-0.0.2/README.md
+-rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-17 00:07:07.059596 zhcode-0.0.2/setup.cfg
+-rw-r--r--   0 lnjng      (501) staff       (20)      484 2023-04-17 00:07:03.000000 zhcode-0.0.2/setup.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.056017 zhcode-0.0.2/zhcode/
+-rw-r--r--   0 lnjng      (501) staff       (20)       50 2023-04-16 23:38:02.000000 zhcode-0.0.2/zhcode/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.2/zhcode/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     1524 2023-04-16 23:39:23.000000 zhcode-0.0.2/zhcode/main.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.058513 zhcode-0.0.2/zhcode/python/
+-rw-r--r--   0 lnjng      (501) staff       (20)       24 2023-04-16 23:30:59.000000 zhcode-0.0.2/zhcode/python/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.2/zhcode/python/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     3017 2023-04-16 21:51:24.000000 zhcode-0.0.2/zhcode/python/stdlib.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     8409 2023-04-16 23:31:32.000000 zhcode-0.0.2/zhcode/python/translate.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.057335 zhcode-0.0.2/zhcode.egg-info/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)      298 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/SOURCES.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/dependency_links.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/top_level.txt
```

### Comparing `zhcode-0.0.1/LICENSE` & `zhcode-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.1/README.md` & `zhcode-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # zhcode
-`zhcode` is a Python library designed to facilitate coding in Chinese. It's main purpose is to advance certain programming languages by transforming them into esoteric forms through the Chinese language.
+`zhcode` is a Python library designed to facilitate coding in Chinese. It's main purpose is to create **esoteric forms of programming languages using the Chinese language**.
+
+You can install `zhcode` by running `pip3 install zhcode` in your environment.
 
 ## Python
 Currently, basic Python 3 functions are supported. The project is still in the process of translating library keywords, names, and functions into Chinese equivalents. In general, the syntax for coding in 
 中文Python is the same as that of normal Python, simply with variables switched. However, several syntactic additions have been made: the dot delimeter `.` in standard Python has been changed to `·`, and 
 variables should be enclosed with `「」` to facilitate easier differentiation.
 
 Furthermore, Chinese keyboard characters often have a tendency to include extra space as part of the character—-thus oftentimes reducing the need for extra whitespace after the character. In particular,
```

### Comparing `zhcode-0.0.1/python/main.py` & `zhcode-0.0.2/zhcode/python/translate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,18 @@
-# main.py
-# main functions of zhcode
+# translate.py
+# main function for translating from zhPython to Python
 
+from zhcode.python.helper import *
 from os import path
 import sys
-import stdlib
+from zhcode.python import stdlib
 
 # dictionary of new functions created by the program
 newfunc = {}
 
-# determine if string is in any part of a dictionary key and if so return the index of the key, otherwise return -1
-def inkey(x, keys):
-    length = len(keys)
-    for k in range(length):
-        if x in keys[k]:
-            return k
-        else:
-            pass
-    return -1
-
-# find if entire string matches the key and if so return the length of the key, otherwise return 0
-def matchkey(x, i, key):
-    length = len(key)
-    if length == 1:
-        return 1
-    else:
-        for j in range(length):
-            try:
-                if x[i + j] == key[j]:
-                    pass
-                else:
-                    return 0
-            except:
-                return 0
-        return length
-
-# General print of filename and line for error handling
-def errprint(name, line, x):
-    print(f"File {name}, line {line}")
-    print(f"    {x}")
-
 # translatepy: Given the path of a txt file containing zhPython code, translate it to Python code and write to new file
 def translatepy(filename):
     file = path.splitext(filename)[0]  # Get file name without extension
     zh = open(filename, "r")
     py = open(f"{file}.py", "a+")
     lines = zh.readlines()  # Read the file line by line into a list
     state = 0  # Use a state variable to preserve continuity
@@ -60,14 +30,27 @@
         for i in range(length):
             if state == 0 or state == 1:
                 # Check if character is within any of the keys of translation dictionaries
                 innames = inkey(x[i], name_keys)
                 infunc = inkey(x[i], func_keys)
                 innewfunc = inkey(x[i], newfunc_keys)
                 indunder = inkey(x[i], dunder_keys)
+                # For each, if in dictionary, check for compelete match
+                matchnames = 0
+                matchfunc = 0
+                matchnewfunc = 0
+                matchdunder = 0
+                if innames != -1:
+                    matchnames = matchkey(x, i, name_keys[innames])
+                if infunc != -1:
+                    matchfunc = matchkey(x, i, func_keys[infunc])
+                if innewfunc != -1:
+                    matchnewfunc = matchkey(x, i, newfunc_keys[innewfunc])
+                if indunder != -1:
+                    matchdunder = matchkey(x, i, dunder_keys[indunder])
                 # Check for strings
                 if x[i] == '"':
                     if sstate == 1:  # State to ignore strings
                         py.write('"')
                         sstate = 2
                     elif sstate == 2:  # State to end the ignoring period
                         py.write('"')
@@ -106,59 +89,41 @@
                             else:
                                 py.write("'")
                                 state = 4
                         except:
                             py.write("'")
                             state = 4
                 # Check for dunder methods
-                elif x[i] == "—":
-                    if indunder != -1:
-                        dunderkey = dunder_keys[indunder]
-                        matchindex = matchkey(x, i, dunderkey)
-                        if matchindex != 0:
-                            py.write(stdlib.dunder.get(dunderkey))
-                            state = -1 * (matchindex - 1)
-                        else:
-                            errprint(filename, linenum, x)
-                            print("TranslateError: dunder method not found")
-                            sys.exit()
-                    else:
-                        errprint(filename, linenum, x)
-                        print("TranslateError: dunder method not found")
-                        sys.exit()
+                elif matchdunder != 0:
+                    dunderkey = dunder_keys[indunder]
+                    py.write(stdlib.dunder.get(dunderkey))
+                    state = -1 * (matchdunder - 1)
                 # Check for names
-                elif innames != -1:
+                elif matchnames != 0:
                     nameskey = name_keys[innames]
-                    matchindex = matchkey(x, i, nameskey)
-                    if matchindex != 0:
-                        py.write(stdlib.names.get(nameskey))
-                        state = -1 * (matchindex - 1)
+                    py.write(stdlib.names.get(nameskey))
+                    state = -1 * (matchnames - 1)
                 # Check for functions
-                elif infunc != -1:
+                elif matchfunc != 0:
                     funckey = func_keys[infunc]
-                    matchindex = matchkey(x, i, funckey)
-                    if matchindex != 0:
-                        if stdlib.func.get(funckey) == "format":  # Check for string format exception
-                            if state == 1:
-                                pass
-                            elif x[i + 2] == '"' or x[i + 2] == "'":
-                                py.write("f")
-                                sstate = 1
-                            else:
-                                pass
+                    if stdlib.func.get(funckey) == "format":  # Check for string format exception
+                        if x[i + 2] == '"' or x[i + 2] == "'":
+                            py.write("f")
+                            sstate = 1  # Use string state to ignore string
+                            state = -1  # Use negative state to ignore next iteration
                         else:
-                            py.write(stdlib.func.get(funckey))
-                            state = -1 * (matchindex - 1)
+                            pass
+                    else:
+                        py.write(stdlib.func.get(funckey))
+                        state = -1 * (matchfunc - 1)
                 # Check for program-created functions
-                elif innewfunc != -1:
+                elif matchnewfunc != 0:
                     newfunckey = newfunc_keys[innewfunc]
-                    matchindex = matchkey(x, i, newfunckey)
-                    if matchindex != 0:
-                        py.write(newfunc.get(newfunckey))
-                        state = -1 * (matchindex - 1)
+                    py.write(newfunc.get(newfunckey))
+                    state = -1 * (matchnewfunc - 1)
                 # Check for keywords
                 elif x[i] in stdlib.keywords:
                     py.write(stdlib.keywords.get(x[i]) + " ")
                     if stdlib.keywords.get(x[i]) == "def":
                         state = 3
                 # Check for variable delimiter
                 elif x[i] == "「":
@@ -224,9 +189,7 @@
                 if x[i] == '"' or x[i] == "'":
                     py.write(x[i])
                     state = 0
                 else:
                     py.write(x[i])
             else:
                 pass
-
-translatepy("test.txt")
```

### Comparing `zhcode-0.0.1/python/stdlib.py` & `zhcode-0.0.2/zhcode/python/stdlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # stdlib.py
 # translations for the Python Standard Library
 
-# keywords not to exceed one charcater
+# keywords not to exceed one character
 keywords = {
         "用" : "import",
         "定" : "def",
         "为" : "for",
         "在" : "in",
         "是" : "if",
         "还" : "elif",
```

