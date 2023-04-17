# Comparing `tmp/friendly-id-0.2.2.tar.gz` & `tmp/friendly-id-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendly-id-0.2.2.tar", last modified: Wed Dec 14 06:17:35 2022, max compression
+gzip compressed data, was "friendly-id-0.3.0.tar", last modified: Mon Apr 17 08:31:47 2023, max compression
```

## Comparing `friendly-id-0.2.2.tar` & `friendly-id-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 06:17:35.104429 friendly-id-0.2.2/
--rw-rw-rw-   0        0        0     1051 2022-11-04 02:20:16.000000 friendly-id-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     3917 2022-12-14 06:17:35.104429 friendly-id-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2192 2022-12-14 06:17:00.000000 friendly-id-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-14 06:17:35.088748 friendly-id-0.2.2/friendly_id/
--rw-rw-rw-   0        0        0      120 2022-12-14 06:17:00.000000 friendly-id-0.2.2/friendly_id/__init__.py
--rw-rw-rw-   0        0        0      751 2022-11-03 07:23:05.000000 friendly-id-0.2.2/friendly_id/friendly_id.py
-drwxrwxrwx   0        0        0        0 2022-12-14 06:17:35.103428 friendly-id-0.2.2/friendly_id.egg-info/
--rw-rw-rw-   0        0        0     3917 2022-12-14 06:17:35.000000 friendly-id-0.2.2/friendly_id.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2022-12-14 06:17:35.000000 friendly-id-0.2.2/friendly_id.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 06:17:35.000000 friendly-id-0.2.2/friendly_id.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2022-12-14 06:17:35.000000 friendly-id-0.2.2/friendly_id.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-14 06:17:35.000000 friendly-id-0.2.2/friendly_id.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1264 2022-12-14 06:17:00.000000 friendly-id-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-14 06:17:35.105428 friendly-id-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-04 02:46:16.000000 friendly-id-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:47.222158 friendly-id-0.3.0/
+-rw-rw-rw-   0        0        0     1051 2023-04-17 07:47:50.000000 friendly-id-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3917 2023-04-17 08:31:47.221156 friendly-id-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2130 2023-04-17 08:28:55.000000 friendly-id-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:47.200157 friendly-id-0.3.0/friendly_id/
+-rw-rw-rw-   0        0        0      115 2023-04-17 08:28:55.000000 friendly-id-0.3.0/friendly_id/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-04-17 08:21:14.000000 friendly-id-0.3.0/friendly_id/friendly_id.py
+-rw-rw-rw-   0        0        0      436 2023-04-17 08:20:38.000000 friendly-id-0.3.0/friendly_id/test_friendly_id.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:47.219149 friendly-id-0.3.0/friendly_id.egg-info/
+-rw-rw-rw-   0        0        0     3917 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 08:31:47.000000 friendly-id-0.3.0/friendly_id.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1220 2023-04-17 08:28:55.000000 friendly-id-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:31:47.222158 friendly-id-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-04-17 07:47:50.000000 friendly-id-0.3.0/setup.py
```

### Comparing `friendly-id-0.2.2/LICENSE` & `friendly-id-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `friendly-id-0.2.2/PKG-INFO` & `friendly-id-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendly-id
-Version: 0.2.2
+Version: 0.3.0
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
 
-> version 0.2.2
+> version 0.3.0
 
 Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
 
 What is the FriendlyId library?
 --
 The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
```

### Comparing `friendly-id-0.2.2/README.md` & `friendly-id-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# Friendly Id
-
-> version 0.2.2
-
-Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
-
-What is the FriendlyId library?
---
-The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
-
-
-    UUID                                        Friendly ID
-
-    c3587ec5-0976-497f-8374-61e0c2ea3da5   ->   5wbwf6yUxVBcr48AMbz9cb
-    |                                           |                              
-    36 characters                               22 characters or less
-
-In addition, this library allows to:
-
-
-* convert from a FriendlyId back to the original UUID; and
-* create a new, random FriendlyId
-
-Why use a FriendlyId?
---
-Universal Unique IDs (UUIDs) provide a non-sequential and unique identifier that can be generated separately from the source database. As a result, it is not possible to guess either the previous or next identifier. That's great, but, to achieve this level of security, a UUID is long (128 bits long) and looks ugly (36 alphanumeric characters including four hyphens which are added to make it easier to read the UUID), as in this example: `123e4567-e89b-12d3-a456-426655440000`.
-
-Such a format is:
-
-* difficult to read (especially if it is part of a URL)
-* difficult to remember
-* cannot be copied with just two mouse-clicks (you have to select manually the start and end positions)
-* can easily become broken across lines when it is copied, pasted, edited, or sent.
-
-FriendlyId library solves these problems by converting a given UUID using Base62 with alphanumeric characters in the range [0-9A-Za-z] into a FriendlyId which consists of a maximum of 22 characters (but in fact often contains fewer characters).
-
-Usage
----
-
-Python Package
-----
-FriendlyId can be installed through PyPI:
-
-```bash
-python -m pip install friendly-id
-```
-
-Generate a FriendlyId
-```python
-from friendly_id import friendly_id
-
-id: str = friendly_id(),
-```
-
-Convert UUID to FriendlyId
-```python
-import uuid
-from friendly_id import encode
-
-uid = uuid.uuid4()
-id: str = encode(uid),
-```
+# Friendly Id
+
+> version 0.3.0
+
+Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
+
+What is the FriendlyId library?
+--
+The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
+
+
+    UUID                                        Friendly ID
+
+    c3587ec5-0976-497f-8374-61e0c2ea3da5   ->   5wbwf6yUxVBcr48AMbz9cb
+    |                                           |                              
+    36 characters                               22 characters or less
+
+In addition, this library allows to:
+
+
+* convert from a FriendlyId back to the original UUID; and
+* create a new, random FriendlyId
+
+Why use a FriendlyId?
+--
+Universal Unique IDs (UUIDs) provide a non-sequential and unique identifier that can be generated separately from the source database. As a result, it is not possible to guess either the previous or next identifier. That's great, but, to achieve this level of security, a UUID is long (128 bits long) and looks ugly (36 alphanumeric characters including four hyphens which are added to make it easier to read the UUID), as in this example: `123e4567-e89b-12d3-a456-426655440000`.
+
+Such a format is:
+
+* difficult to read (especially if it is part of a URL)
+* difficult to remember
+* cannot be copied with just two mouse-clicks (you have to select manually the start and end positions)
+* can easily become broken across lines when it is copied, pasted, edited, or sent.
+
+FriendlyId library solves these problems by converting a given UUID using Base62 with alphanumeric characters in the range [0-9A-Za-z] into a FriendlyId which consists of a maximum of 22 characters (but in fact often contains fewer characters).
+
+Usage
+---
+
+Python Package
+----
+FriendlyId can be installed through PyPI:
+
+```bash
+python -m pip install friendly-id
+```
+
+Generate a FriendlyId
+```python
+from friendly_id import friendly_id
+
+id: str = friendly_id(),
+```
+
+Convert UUID to FriendlyId
+```python
+import uuid
+from friendly_id import encode
+
+uid = uuid.uuid4()
+id: str = encode(uid),
+```
```

### Comparing `friendly-id-0.2.2/friendly_id/friendly_id.py` & `friendly-id-0.3.0/friendly_id/friendly_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 
 
 # https://en.wikipedia.org/wiki/Base62
 base62alphabet: str = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'
-
+base: int = len(base62alphabet) # base62
 
 def friendly_id() -> str:
     id = uuid.uuid4()
     return encode(id)
 
 def encode(raw: uuid.UUID) -> str:
     """
@@ -18,14 +18,23 @@
         raw (str): _description_
         mask (str): _description_
 
     Returns:
         str: _description_
     """
     
-    base = len(base62alphabet) # base62
     input = raw.int
     res = ''
     while input != 0:
         res += base62alphabet[input % base]
         input = input // base
     return res[::-1]
+
+def decode(raw: str) -> uuid.UUID:
+    res = 0
+    for c in raw:
+        try:
+            i = base62alphabet.index(c)
+        except ValueError:
+            raise ValueError('Invalid character in base62 string')
+        res = res * base + i
+    return uuid.UUID(int=res)
```

### Comparing `friendly-id-0.2.2/friendly_id.egg-info/PKG-INFO` & `friendly-id-0.3.0/friendly_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendly-id
-Version: 0.2.2
+Version: 0.3.0
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
 
-> version 0.2.2
+> version 0.3.0
 
 Inspired by [FriendlyID](https://github.com/Devskiller/friendly-id)
 
 What is the FriendlyId library?
 --
 The FriendlyId library converts a given UUID (with 36 characters) to a URL-friendly ID (a "FriendlyId") which is based on Base62 (with a maximum of 22 characters), as in the example below:
```

### Comparing `friendly-id-0.2.2/pyproject.toml` & `friendly-id-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,77 @@
-00000000: 0d0a 5b62 7569 6c64 2d73 7973 7465 6d5d  ..[build-system]
-00000010: 0d0a 7265 7175 6972 6573 203d 205b 2273  ..requires = ["s
-00000020: 6574 7570 746f 6f6c 733e 3d36 312e 302e  etuptools>=61.0.
-00000030: 3022 2c20 2277 6865 656c 225d 0d0a 6275  0", "wheel"]..bu
-00000040: 696c 642d 6261 636b 656e 6420 3d20 2273  ild-backend = "s
-00000050: 6574 7570 746f 6f6c 732e 6275 696c 645f  etuptools.build_
-00000060: 6d65 7461 220d 0a0d 0a5b 7072 6f6a 6563  meta"....[projec
-00000070: 745d 0d0a 6e61 6d65 203d 2022 6672 6965  t]..name = "frie
-00000080: 6e64 6c79 2d69 6422 0d0a 7665 7273 696f  ndly-id"..versio
-00000090: 6e20 3d20 2230 2e32 2e32 220d 0a64 6573  n = "0.2.2"..des
-000000a0: 6372 6970 7469 6f6e 203d 2022 5265 6164  cription = "Read
-000000b0: 2074 6865 206c 6174 6573 7420 5265 616c   the latest Real
-000000c0: 2050 7974 686f 6e20 7475 746f 7269 616c   Python tutorial
-000000d0: 7322 0d0a 7265 6164 6d65 203d 2022 5245  s"..readme = "RE
-000000e0: 4144 4d45 2e6d 6422 0d0a 6175 7468 6f72  ADME.md"..author
-000000f0: 7320 3d20 5b7b 206e 616d 6520 3d20 224a  s = [{ name = "J
-00000100: 756e 6c69 6e20 5a68 6f75 222c 2065 6d61  unlin Zhou", ema
-00000110: 696c 203d 2022 6a61 6d65 737a 686f 7532  il = "jameszhou2
-00000120: 3130 3840 686f 746d 6169 6c2e 636f 6d22  108@hotmail.com"
-00000130: 207d 5d0d 0a6c 6963 656e 7365 203d 207b   }]..license = {
-00000140: 2066 696c 6520 3d20 224c 4943 454e 5345   file = "LICENSE
-00000150: 2220 7d0d 0a63 6c61 7373 6966 6965 7273  " }..classifiers
-00000160: 203d 205b 0d0a 2020 2020 224c 6963 656e   = [..    "Licen
-00000170: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000180: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000190: 6522 2c0d 0a20 2020 2022 5072 6f67 7261  e",..    "Progra
-000001a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001b0: 3a20 5079 7468 6f6e 222c 0d0a 2020 2020  : Python",..    
-000001c0: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001e0: 3a3a 2033 222c 0d0a 5d0d 0a6b 6579 776f  :: 3",..]..keywo
-000001f0: 7264 7320 3d20 5b22 7575 6964 222c 2022  rds = ["uuid", "
-00000200: 6672 6965 6e64 6c79 2d69 6422 5d0d 0a64  friendly-id"]..d
-00000210: 6570 656e 6465 6e63 6965 7320 3d20 5b5d  ependencies = []
-00000220: 0d0a 7265 7175 6972 6573 2d70 7974 686f  ..requires-pytho
-00000230: 6e20 3d20 223e 3d33 2e35 220d 0a0d 0a20  n = ">=3.5".... 
-00000240: 2020 205b 7072 6f6a 6563 742e 6f70 7469     [project.opti
-00000250: 6f6e 616c 2d64 6570 656e 6465 6e63 6965  onal-dependencie
-00000260: 735d 0d0a 2020 2020 6275 696c 6420 3d20  s]..    build = 
-00000270: 5b22 6275 696c 6422 2c20 2274 7769 6e65  ["build", "twine
-00000280: 225d 0d0a 2020 2020 6465 7620 3d20 5b22  "]..    dev = ["
-00000290: 626c 6163 6b22 2c20 2262 756d 7076 6572  black", "bumpver
-000002a0: 222c 2022 6973 6f72 7422 2c20 2270 6970  ", "isort", "pip
-000002b0: 2d74 6f6f 6c73 222c 2022 7079 7465 7374  -tools", "pytest
-000002c0: 225d 0d0a 0d0a 2020 2020 5b70 726f 6a65  "]....    [proje
-000002d0: 6374 2e75 726c 735d 0d0a 2020 2020 686f  ct.urls]..    ho
-000002e0: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
-000002f0: 2f2f 6769 7468 7562 2e63 6f6d 2f65 6477  //github.com/edw
-00000300: 6172 647a 6a6c 2f66 7269 656e 646c 792d  ardzjl/friendly-
-00000310: 6964 220d 0a20 2020 2072 6570 6f73 6974  id"..    reposit
-00000320: 6f72 7920 3d20 2268 7474 7073 3a2f 2f67  ory = "https://g
-00000330: 6974 6875 622e 636f 6d2f 6564 7761 7264  ithub.com/edward
-00000340: 7a6a 6c2f 6672 6965 6e64 6c79 2d69 6422  zjl/friendly-id"
-00000350: 0d0a 0d0a 5b74 6f6f 6c2e 6275 6d70 7665  ....[tool.bumpve
-00000360: 725d 0d0a 6375 7272 656e 745f 7665 7273  r]..current_vers
-00000370: 696f 6e20 3d20 2230 2e32 2e32 220d 0a76  ion = "0.2.2"..v
-00000380: 6572 7369 6f6e 5f70 6174 7465 726e 203d  ersion_pattern =
-00000390: 2022 4d41 4a4f 522e 4d49 4e4f 522e 5041   "MAJOR.MINOR.PA
-000003a0: 5443 4822 0d0a 636f 6d6d 6974 5f6d 6573  TCH"..commit_mes
-000003b0: 7361 6765 203d 2022 6275 6d70 2076 6572  sage = "bump ver
-000003c0: 7369 6f6e 207b 6f6c 645f 7665 7273 696f  sion {old_versio
-000003d0: 6e7d 202d 3e20 7b6e 6577 5f76 6572 7369  n} -> {new_versi
-000003e0: 6f6e 7d22 0d0a 636f 6d6d 6974 203d 2074  on}"..commit = t
-000003f0: 7275 650d 0a74 6167 203d 2074 7275 650d  rue..tag = true.
-00000400: 0a70 7573 6820 3d20 6661 6c73 650d 0a0d  .push = false...
-00000410: 0a20 2020 205b 746f 6f6c 2e62 756d 7076  .    [tool.bumpv
-00000420: 6572 2e66 696c 655f 7061 7474 6572 6e73  er.file_patterns
-00000430: 5d0d 0a20 2020 2022 7079 7072 6f6a 6563  ]..    "pyprojec
-00000440: 742e 746f 6d6c 2220 3d20 5b0d 0a20 2020  t.toml" = [..   
-00000450: 2020 2020 2027 6375 7272 656e 745f 7665       'current_ve
-00000460: 7273 696f 6e20 3d20 227b 7665 7273 696f  rsion = "{versio
-00000470: 6e7d 2227 2c0d 0a20 2020 2020 2020 2027  n}"',..        '
-00000480: 7665 7273 696f 6e20 3d20 227b 7665 7273  version = "{vers
-00000490: 696f 6e7d 2227 2c0d 0a20 2020 205d 0d0a  ion}"',..    ]..
-000004a0: 2020 2020 2266 7269 656e 646c 795f 6964      "friendly_id
-000004b0: 2f5f 5f69 6e69 745f 5f2e 7079 2220 3d20  /__init__.py" = 
-000004c0: 5b22 7b76 6572 7369 6f6e 7d22 5d0d 0a20  ["{version}"].. 
-000004d0: 2020 2022 5245 4144 4d45 2e6d 6422 203d     "README.md" =
-000004e0: 205b 227b 7665 7273 696f 6e7d 225d 0d0a   ["{version}"]..
+00000000: 0a5b 6275 696c 642d 7379 7374 656d 5d0a  .[build-system].
+00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
+00000020: 7570 746f 6f6c 733e 3d36 312e 302e 3022  uptools>=61.0.0"
+00000030: 2c20 2277 6865 656c 225d 0a62 7569 6c64  , "wheel"].build
+00000040: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
+00000050: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
+00000060: 6122 0a0a 5b70 726f 6a65 6374 5d0a 6e61  a"..[project].na
+00000070: 6d65 203d 2022 6672 6965 6e64 6c79 2d69  me = "friendly-i
+00000080: 6422 0a76 6572 7369 6f6e 203d 2022 302e  d".version = "0.
+00000090: 332e 3022 0a64 6573 6372 6970 7469 6f6e  3.0".description
+000000a0: 203d 2022 5265 6164 2074 6865 206c 6174   = "Read the lat
+000000b0: 6573 7420 5265 616c 2050 7974 686f 6e20  est Real Python 
+000000c0: 7475 746f 7269 616c 7322 0a72 6561 646d  tutorials".readm
+000000d0: 6520 3d20 2252 4541 444d 452e 6d64 220a  e = "README.md".
+000000e0: 6175 7468 6f72 7320 3d20 5b7b 206e 616d  authors = [{ nam
+000000f0: 6520 3d20 224a 756e 6c69 6e20 5a68 6f75  e = "Junlin Zhou
+00000100: 222c 2065 6d61 696c 203d 2022 6a61 6d65  ", email = "jame
+00000110: 737a 686f 7532 3130 3840 686f 746d 6169  szhou2108@hotmai
+00000120: 6c2e 636f 6d22 207d 5d0a 6c69 6365 6e73  l.com" }].licens
+00000130: 6520 3d20 7b20 6669 6c65 203d 2022 4c49  e = { file = "LI
+00000140: 4345 4e53 4522 207d 0a63 6c61 7373 6966  CENSE" }.classif
+00000150: 6965 7273 203d 205b 0a20 2020 2022 4c69  iers = [.    "Li
+00000160: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000170: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000180: 656e 7365 222c 0a20 2020 2022 5072 6f67  ense",.    "Prog
+00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001a0: 203a 3a20 5079 7468 6f6e 222c 0a20 2020   :: Python",.   
+000001b0: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
+000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001d0: 203a 3a20 3322 2c0a 5d0a 6b65 7977 6f72   :: 3",.].keywor
+000001e0: 6473 203d 205b 2275 7569 6422 2c20 2266  ds = ["uuid", "f
+000001f0: 7269 656e 646c 792d 6964 225d 0a64 6570  riendly-id"].dep
+00000200: 656e 6465 6e63 6965 7320 3d20 5b5d 0a72  endencies = [].r
+00000210: 6571 7569 7265 732d 7079 7468 6f6e 203d  equires-python =
+00000220: 2022 3e3d 332e 3522 0a0a 2020 2020 5b70   ">=3.5"..    [p
+00000230: 726f 6a65 6374 2e6f 7074 696f 6e61 6c2d  roject.optional-
+00000240: 6465 7065 6e64 656e 6369 6573 5d0a 2020  dependencies].  
+00000250: 2020 6275 696c 6420 3d20 5b22 6275 696c    build = ["buil
+00000260: 6422 2c20 2274 7769 6e65 225d 0a20 2020  d", "twine"].   
+00000270: 2064 6576 203d 205b 2262 6c61 636b 222c   dev = ["black",
+00000280: 2022 6275 6d70 7665 7222 2c20 2269 736f   "bumpver", "iso
+00000290: 7274 222c 2022 7069 702d 746f 6f6c 7322  rt", "pip-tools"
+000002a0: 2c20 2270 7974 6573 7422 5d0a 0a20 2020  , "pytest"]..   
+000002b0: 205b 7072 6f6a 6563 742e 7572 6c73 5d0a   [project.urls].
+000002c0: 2020 2020 686f 6d65 7061 6765 203d 2022      homepage = "
+000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002e0: 6f6d 2f65 6477 6172 647a 6a6c 2f66 7269  om/edwardzjl/fri
+000002f0: 656e 646c 792d 6964 220a 2020 2020 7265  endly-id".    re
+00000300: 706f 7369 746f 7279 203d 2022 6874 7470  pository = "http
+00000310: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00000320: 6477 6172 647a 6a6c 2f66 7269 656e 646c  dwardzjl/friendl
+00000330: 792d 6964 220a 0a5b 746f 6f6c 2e62 756d  y-id"..[tool.bum
+00000340: 7076 6572 5d0a 6375 7272 656e 745f 7665  pver].current_ve
+00000350: 7273 696f 6e20 3d20 2230 2e33 2e30 220a  rsion = "0.3.0".
+00000360: 7665 7273 696f 6e5f 7061 7474 6572 6e20  version_pattern 
+00000370: 3d20 224d 414a 4f52 2e4d 494e 4f52 2e50  = "MAJOR.MINOR.P
+00000380: 4154 4348 220a 636f 6d6d 6974 5f6d 6573  ATCH".commit_mes
+00000390: 7361 6765 203d 2022 6275 6d70 2076 6572  sage = "bump ver
+000003a0: 7369 6f6e 207b 6f6c 645f 7665 7273 696f  sion {old_versio
+000003b0: 6e7d 202d 3e20 7b6e 6577 5f76 6572 7369  n} -> {new_versi
+000003c0: 6f6e 7d22 0a63 6f6d 6d69 7420 3d20 7472  on}".commit = tr
+000003d0: 7565 0a74 6167 203d 2074 7275 650a 7075  ue.tag = true.pu
+000003e0: 7368 203d 2066 616c 7365 0a0a 2020 2020  sh = false..    
+000003f0: 5b74 6f6f 6c2e 6275 6d70 7665 722e 6669  [tool.bumpver.fi
+00000400: 6c65 5f70 6174 7465 726e 735d 0a20 2020  le_patterns].   
+00000410: 2022 7079 7072 6f6a 6563 742e 746f 6d6c   "pyproject.toml
+00000420: 2220 3d20 5b0a 2020 2020 2020 2020 2763  " = [.        'c
+00000430: 7572 7265 6e74 5f76 6572 7369 6f6e 203d  urrent_version =
+00000440: 2022 7b76 6572 7369 6f6e 7d22 272c 0a20   "{version}"',. 
+00000450: 2020 2020 2020 2027 7665 7273 696f 6e20         'version 
+00000460: 3d20 227b 7665 7273 696f 6e7d 2227 2c0a  = "{version}"',.
+00000470: 2020 2020 5d0a 2020 2020 2266 7269 656e      ].    "frien
+00000480: 646c 795f 6964 2f5f 5f69 6e69 745f 5f2e  dly_id/__init__.
+00000490: 7079 2220 3d20 5b22 7b76 6572 7369 6f6e  py" = ["{version
+000004a0: 7d22 5d0a 2020 2020 2252 4541 444d 452e  }"].    "README.
+000004b0: 6d64 2220 3d20 5b22 7b76 6572 7369 6f6e  md" = ["{version
+000004c0: 7d22 5d0a                                }"].
```

