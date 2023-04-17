# Comparing `tmp/structio-1.1.5.tar.gz` & `tmp/structio-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.1.5.tar", last modified: Sat Apr 15 22:29:42 2023, max compression
+gzip compressed data, was "structio-1.1.6.tar", last modified: Mon Apr 17 14:27:28 2023, max compression
```

## Comparing `structio-1.1.5.tar` & `structio-1.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:29:42.965475 structio-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-15 22:29:42.965475 structio-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-04-15 22:29:23.000000 structio-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-15 22:29:23.000000 structio-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 22:29:42.965475 structio-1.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:29:42.965475 structio-1.1.5/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-15 22:29:23.000000 structio-1.1.5/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:27:28.688793 structio-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-17 14:27:28.688793 structio-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-17 14:27:11.000000 structio-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-17 14:27:11.000000 structio-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:27:28.688793 structio-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:27:28.688793 structio-1.1.6/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-17 14:27:11.000000 structio-1.1.6/structio.py
```

### Comparing `structio-1.1.5/PKG-INFO` & `structio-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -344,22 +344,18 @@
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
-        string, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_len=True)
-        self.seek(length, 1)
-        return string
+        return self._read(self._struct.unpack_7bstr, ())
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
-        start = self.tell()
-        length = self._struct._get_7bstr_len(self.getvalue(), start)
-        return self.overwrite(start, start + length, self._struct.pack_7bstr(string))
+        return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
 ```
```

### Comparing `structio-1.1.5/README.md` & `structio-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -336,22 +336,18 @@
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
-        string, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_len=True)
-        self.seek(length, 1)
-        return string
+        return self._read(self._struct.unpack_7bstr, ())
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
-        start = self.tell()
-        length = self._struct._get_7bstr_len(self.getvalue(), start)
-        return self.overwrite(start, start + length, self._struct.pack_7bstr(string))
+        return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
 ```
```

### Comparing `structio-1.1.5/structio.egg-info/PKG-INFO` & `structio-1.1.6/structio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -344,22 +344,18 @@
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
-        string, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_len=True)
-        self.seek(length, 1)
-        return string
+        return self._read(self._struct.unpack_7bstr, ())
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
-        start = self.tell()
-        length = self._struct._get_7bstr_len(self.getvalue(), start)
-        return self.overwrite(start, start + length, self._struct.pack_7bstr(string))
+        return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
 ```
```

### Comparing `structio-1.1.5/structio.py` & `structio-1.1.6/structio.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         
     def unpack_float(self, b, numbytes, endian=None):
         return struct.unpack(self._get_format(numbytes, self._get_endian(endian)), b)[0]
         
     def pack_float(self, number, numbytes, endian=None):
         return struct.pack(self._get_format(numbytes, self._get_endian(endian)), number)
         
+    def _get_str_len(self, b, length, start=0):
+        return length
+        
     def unpack_str(self, b):
         return b.decode(self.encoding, errors=self.errors)
         
     def pack_str(self, string):
         return string.encode(self.encoding, errors=self.errors)
         
     def _get_cstr_len(self, b, start=0):
@@ -243,14 +246,24 @@
         end = self.find(bytes_sequence, n)
         
         if end == -1:
             raise ValueError('{} not found'.format(bytes_sequence))
             
         return end
         
+    def _read(self, unpack_func, unpack_args):
+        value, length = unpack_func(self.getvalue(), *unpack_args, start=self.tell(), ret_len=True)
+        self.seek(length, 1)
+        return value
+        
+    def _overwrite(self, len_func, len_args, pack_func, pack_args):
+        start = self.tell()
+        length = len_func(self.getvalue(), *len_args, start=start)
+        return self.overwrite(start, start + length, pack_func(*pack_args))
+        
     def read_bool(self):
         return self._struct.unpack_bool(self.read(1))
         
     def write_bool(self, boolean):
         return self.write(self._struct.pack_bool(boolean))
         
     def append_bool(self, boolean):
@@ -289,57 +302,44 @@
     def write_str(self, string):
         return self.write(self._struct.pack_str(string))
         
     def append_str(self, string):
         return self.append(self._struct.pack_str(string))
         
     def overwrite_str(self, string, length):
-        start = self.tell()
-        return self.overwrite(start, start + length, self._struct.pack_str(string))
+        return self._overwrite(self._struct._get_str_len, (length,), self._struct.pack_str, (string,))
         
     def read_cstr(self):
-        value, length = self._struct.unpack_cstr(self.getvalue(), start=self.tell(), ret_len=True)
-        self.seek(length, 1)
-        return value
+        return self._read(self._struct.unpack_cstr, ())
         
     def write_cstr(self, string):
         return self.write(self._struct.pack_cstr(string))
         
     def append_cstr(self, string):
         return self.append(self._struct.pack_cstr(string))
         
     def overwrite_cstr(self, string):
-        start = self.tell()
-        length = self._struct._get_cstr_len(self.getvalue(), start=start)
-        return self.overwrite(start, start + length, self._struct.pack_cstr(string))
+        return self._overwrite(self._struct._get_cstr_len, (), self._struct.pack_cstr, (string,))
         
     def read_pstr(self, numbytes, endian=None):
-        value, length = self._struct.unpack_pstr(self.getvalue(), numbytes, endian, start=self.tell(), ret_len=True)
-        self.seek(length, 1)
-        return value
+        return self._read(self._struct.unpack_pstr, (numbytes, endian))
         
     def write_pstr(self, string, numbytes, endian=None):
         return self.write(self._struct.pack_pstr(string, numbytes, endian))
         
     def append_pstr(self, string, numbytes, endian=None):
         return self.append(self._struct.pack_pstr(string, numbytes, endian))
         
     def overwrite_pstr(self, string, numbytes, endian=None):
-        start = self.tell()
-        length = self._struct._get_pstr_len(self.getvalue(), numbytes, endian, start=start)
-        return self.overwrite(start, start + length, self._struct.pack_pstr(string, numbytes, endian))
+        return self._overwrite(self._struct._get_pstr_len, (numbytes, endian), self._struct.pack_pstr, (string, numbytes, endian))
         
     def read_7bint(self):
-        value, length = self._struct.unpack_7bint(self.getvalue(), start=self.tell(), ret_len=True)
-        self.seek(length, 1)
-        return value
+        return self._read(self._struct.unpack_7bint, ())
         
     def write_7bint(self, number):
         return self.write(self._struct.pack_7bint(number))
         
     def append_7bint(self, number):
         return self.append(self._struct.pack_7bint(number))
         
     def overwrite_7bint(self, number):
-        start = self.tell()
-        length = self._struct._get_7bint_len(self.getvalue(), start=start)
-        return self.overwrite(start, start + length, self._struct.pack_7bint(number))
+        return self._overwrite(self._struct._get_7bint_len, (), self._struct.pack_7bint, (number,))
```

