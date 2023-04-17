# Comparing `tmp/led_list-0.5.2.tar.gz` & `tmp/led_list-0.5.3.tar.gz`

## Comparing `led_list-0.5.2.tar` & `led_list-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 led_list-0.5.2/src/led_list/__init__.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 led_list-0.5.2/src/led_list/list.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 led_list-0.5.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 led_list-0.5.2/LICENSE
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 led_list-0.5.2/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 led_list-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 led_list-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 led_list-0.5.3/src/led_list/__init__.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 led_list-0.5.3/src/led_list/list.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 led_list-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 led_list-0.5.3/LICENSE
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 led_list-0.5.3/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 led_list-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 led_list-0.5.3/PKG-INFO
```

### Comparing `led_list-0.5.2/src/led_list/list.py` & `led_list-0.5.3/src/led_list/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 updates.append((index, values[0]))
 
         if len(new) > len(cached):
             # find lights to turn on
             new = new[overlap:]
             updates.extend(enumerate(new, overlap))
         else:
-            # find lights to turn off
+            # find lights to turn off (reverse order)
             off = [(0, 0, 0)] * (len(cached) - overlap)
             updates.extend(reversed(list(enumerate(off, overlap))))
 
         return updates
 
     # convert string color values to tuples
     @staticmethod
@@ -99,14 +99,20 @@
 
     def remove(self, item) -> None:
         super().remove(item)
         self.__light()
 
         return
 
+    def pop(self, i: int = -1):
+        ret = super().pop(i)
+        self.__light()
+
+        return ret
+
     def append(self, item) -> None:
         super().append(item)
         self.__light()
 
         return
     
     def extend(self, other):
```

### Comparing `led_list-0.5.2/LICENSE` & `led_list-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `led_list-0.5.2/README.md` & `led_list-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `led_list-0.5.2/pyproject.toml` & `led_list-0.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "led-list"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Connor Fogarty", email="connorflynnfogarty@gmail.com" },
 ]
 description = "Teach Python lists with a BlinkStick LED strip."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `led_list-0.5.2/PKG-INFO` & `led_list-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: led-list
-Version: 0.5.2
+Version: 0.5.3
 Summary: Teach Python lists with a BlinkStick LED strip.
 Project-URL: Homepage, https://github.com/connorff/led-list
 Author-email: Connor Fogarty <connorflynnfogarty@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: blinkstick>=0.7.0
 Requires-Dist: pyusb==1.0.0
```

