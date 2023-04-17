# Comparing `tmp/vpp_papi-2.0.0.tar.gz` & `tmp/vpp-papi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "vpp-papi-2.0.1.tar", last modified: Mon Apr 17 11:52:50 2023, max compression
```

## Comparing `vpp_papi-2.0.0.tar` & `vpp-papi-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/CMakeLists.txt
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/setup.cfg
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/setup.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/tox.ini
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/__init__.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/macaddress.py
--rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/vpp_format.py
--rw-r--r--   0        0        0    33249 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/vpp_papi.py
--rw-r--r--   0        0        0    21818 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/vpp_serializer.py
--rwxr-xr-x   0        0        0    18576 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/vpp_stats.py
--rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/vpp_transport_socket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/tests/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/tests/test_macaddress.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/tests/test_vpp_format.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/tests/test_vpp_papi.py
--rwxr-xr-x   0        0        0    23137 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/vpp_papi/tests/test_vpp_serializer.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 vpp_papi-2.0.0/PKG-INFO
+drwxrwxr-x   0 otroan    (1000) otroan    (1000)        0 2023-04-17 11:52:50.674452 vpp-papi-2.0.1/
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)    11358 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/LICENSE.txt
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      238 2023-04-17 11:52:50.674452 vpp-papi-2.0.1/PKG-INFO
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      548 2023-04-17 11:52:46.000000 vpp-papi-2.0.1/pyproject.toml
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)       38 2023-04-17 11:52:50.674452 vpp-papi-2.0.1/setup.cfg
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      169 2023-04-17 11:48:39.000000 vpp-papi-2.0.1/setup.py
+drwxrwxr-x   0 otroan    (1000) otroan    (1000)        0 2023-04-17 11:52:50.674452 vpp-papi-2.0.1/vpp_papi/
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      827 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/__init__.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)     2144 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/macaddress.py
+drwxrwxr-x   0 otroan    (1000) otroan    (1000)        0 2023-04-17 11:52:50.674452 vpp-papi-2.0.1/vpp_papi/tests/
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)        0 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/tests/__init__.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      207 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/tests/test_macaddress.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)     4510 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/tests/test_vpp_format.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)     6352 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/tests/test_vpp_papi.py
+-rwxrwxr-x   0 otroan    (1000) otroan    (1000)    24145 2023-03-29 14:15:30.000000 vpp-papi-2.0.1/vpp_papi/tests/test_vpp_serializer.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)     7692 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/vpp_format.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)    33249 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/vpp_papi.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)    21872 2023-03-29 14:15:30.000000 vpp-papi-2.0.1/vpp_papi/vpp_serializer.py
+-rwxrwxr-x   0 otroan    (1000) otroan    (1000)    18576 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/vpp_stats.py
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)     7976 2023-02-22 15:06:34.000000 vpp-papi-2.0.1/vpp_papi/vpp_transport_socket.py
+drwxrwxr-x   0 otroan    (1000) otroan    (1000)        0 2023-04-17 11:52:50.674452 vpp-papi-2.0.1/vpp_papi.egg-info/
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      238 2023-04-17 11:52:50.000000 vpp-papi-2.0.1/vpp_papi.egg-info/PKG-INFO
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)      498 2023-04-17 11:52:50.000000 vpp-papi-2.0.1/vpp_papi.egg-info/SOURCES.txt
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)        1 2023-04-17 11:52:50.000000 vpp-papi-2.0.1/vpp_papi.egg-info/dependency_links.txt
+-rw-rw-r--   0 otroan    (1000) otroan    (1000)        9 2023-04-17 11:52:50.000000 vpp-papi-2.0.1/vpp_papi.egg-info/top_level.txt
```

### Comparing `vpp_papi-2.0.0/vpp_papi/__init__.py` & `vpp-papi-2.0.1/vpp_papi/__init__.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/macaddress.py` & `vpp-papi-2.0.1/vpp_papi/macaddress.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/vpp_format.py` & `vpp-papi-2.0.1/vpp_papi/vpp_format.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/vpp_papi.py` & `vpp-papi-2.0.1/vpp_papi/vpp_papi.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/vpp_serializer.py` & `vpp-papi-2.0.1/vpp_papi/vpp_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,32 +300,31 @@
             return b""
         if len(lst) != kwargs[self.length_field]:
             raise VPPSerializerValueError(
                 "Variable length error, got: {} expected: {}".format(
                     len(lst), kwargs[self.length_field]
                 )
             )
-
         # u8 array
-        if self.packer.size == 1:
+        if self.packer.size == 1 and self.field_type == "u8":
             if isinstance(lst, list):
                 return b"".join(lst)
             return bytes(lst)
 
         b = bytearray()
         for e in lst:
             b += self.packer.pack(e)
         return bytes(b)
 
     def unpack(self, data, offset=0, result=None, ntc=False):
         # Return a list of arguments
         total = 0
 
         # u8 array
-        if self.packer.size == 1:
+        if self.packer.size == 1 and self.field_type == "u8":
             if result[self.index] == 0:
                 return b"", 0
             p = BaseTypes("u8", result[self.index])
             return p.unpack(data, offset, ntc=ntc)
 
         r = []
         for e in range(result[self.index]):
@@ -614,15 +613,14 @@
                 if "default" in self.options:
                     p = self.get_packer_with_options(f_type, self.options)
                 else:
                     p = types[f_type]
 
                 self.packers.append(p)
                 size += p.size
-
         self.size = size
         self.tuple = collections.namedtuple(name, self.fields, rename=True)
         types[name] = self
         self.toplevelconversion = False
 
     def pack(self, data, kwargs=None):
         if not kwargs:
```

### Comparing `vpp_papi-2.0.0/vpp_papi/vpp_stats.py` & `vpp-papi-2.0.1/vpp_papi/vpp_stats.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/vpp_transport_socket.py` & `vpp-papi-2.0.1/vpp_papi/vpp_transport_socket.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/tests/test_vpp_format.py` & `vpp-papi-2.0.1/vpp_papi/tests/test_vpp_format.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/tests/test_vpp_papi.py` & `vpp-papi-2.0.1/vpp_papi/tests/test_vpp_papi.py`

 * *Files identical despite different names*

### Comparing `vpp_papi-2.0.0/vpp_papi/tests/test_vpp_serializer.py` & `vpp-papi-2.0.1/vpp_papi/tests/test_vpp_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,14 +422,40 @@
         s = VPPType("str", [["u32", "length"], ["u8", "string", 0, "length"]])
 
         string = ""
         b = s.pack({"length": len(string), "string": string.encode("utf-8")})
         nt, size = s.unpack(b)
         self.assertEqual(len(b), size)
 
+        # Try same with VLA u8
+        byte_array = [b"\0"] * (10)
+        vla_u8 = VPPType("vla_u8", [["u8", "length"], ["u8", "data", 0, "length"]])
+        b = vla_u8.pack({"length": len(byte_array), "data": byte_array})
+        nt, size = vla_u8.unpack(b)
+
+        # VLA Array of fixed length strings
+        fixed_string = VPPType("fixed_string", [["string", "data", 32]])
+        s = VPPType(
+            "string_vla", [["u32", "length"], ["fixed_string", "services", 0, "length"]]
+        )
+
+        string_list = [{"data": "foobar1"}, {"data": "foobar2"}]
+        b = s.pack({"length": 2, "services": string_list})
+        nt, size = s.unpack(b)
+
+        # Try same with u8
+        fixed_u8 = VPPType("fixed_u8", [["u8", "data", 32]])
+        s = VPPType(
+            "u8_vla", [["u32", "length"], ["fixed_string", "services", 0, "length"]]
+        )
+
+        u8_list = [{"data": "foobar1"}, {"data": "foobar2"}]
+        b = s.pack({"length": 2, "services": u8_list})
+        nt, size = s.unpack(b)
+
     def test_message(self):
         foo = VPPMessage(
             "foo",
             [
                 ["u16", "_vl_msg_id"],
                 ["u8", "client_index"],
                 ["u8", "something"],
```

### Comparing `vpp_papi-2.0.0/LICENSE.txt` & `vpp-papi-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

