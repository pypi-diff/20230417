# Comparing `tmp/pawnlib-0.1.8-py3-none-any.whl.zip` & `tmp/pawnlib-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 78612 bytes, number of entries: 44
+Zip file size: 78811 bytes, number of entries: 44
 -rw-r--r--  2.0 unx     1188 b- defN 23-Jan-31 08:49 pawnlib/__init__.py
 -rw-r--r--  2.0 unx     1224 b- defN 23-Jan-31 08:49 pawnlib/__main__.py
--rw-r--r--  2.0 unx      292 b- defN 23-Feb-08 02:53 pawnlib/__version__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Feb-08 03:20 pawnlib/__version__.py
 -rw-r--r--  2.0 unx       19 b- defN 22-Jul-21 06:00 pawnlib/asyncio/__init__.py
 -rw-r--r--  2.0 unx     2952 b- defN 23-Jan-31 06:38 pawnlib/asyncio/run.py
 -rw-r--r--  2.0 unx       36 b- defN 22-Jul-28 01:54 pawnlib/builder/__init__.py
 -rw-r--r--  2.0 unx     5382 b- defN 23-Jan-31 06:30 pawnlib/builder/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-28 04:35 pawnlib/builder/templates/__init__.py
 -rw-r--r--  2.0 unx     2195 b- defN 22-Dec-01 01:31 pawnlib/builder/templates/app_with_logging.tmpl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-28 04:34 pawnlib/cli/__init__.py
@@ -24,23 +24,23 @@
 -rw-r--r--  2.0 unx     6198 b- defN 23-Jan-31 06:29 pawnlib/output/file.py
 -rw-r--r--  2.0 unx      288 b- defN 22-Sep-13 06:52 pawnlib/resource/__init__.py
 -rw-r--r--  2.0 unx     6568 b- defN 23-Jan-31 04:59 pawnlib/resource/net.py
 -rw-r--r--  2.0 unx    11387 b- defN 22-Nov-22 01:36 pawnlib/resource/server.py
 -rw-r--r--  2.0 unx     1653 b- defN 23-Jan-31 08:53 pawnlib/typing/__init__.py
 -rw-r--r--  2.0 unx     4402 b- defN 23-Jan-31 09:06 pawnlib/typing/check.py
 -rw-r--r--  2.0 unx      689 b- defN 23-Jan-31 06:03 pawnlib/typing/constants.py
--rw-r--r--  2.0 unx    53503 b- defN 23-Feb-08 02:48 pawnlib/typing/converter.py
+-rw-r--r--  2.0 unx    54524 b- defN 23-Feb-08 03:20 pawnlib/typing/converter.py
 -rw-r--r--  2.0 unx     7137 b- defN 23-Jan-31 09:13 pawnlib/typing/date_utils.py
 -rw-r--r--  2.0 unx     1898 b- defN 22-Aug-17 08:57 pawnlib/typing/defines.py
 -rw-r--r--  2.0 unx    12711 b- defN 23-Jan-31 06:35 pawnlib/typing/generator.py
 -rw-r--r--  2.0 unx      349 b- defN 22-Dec-01 06:49 pawnlib/utils/__init__.py
 -rw-r--r--  2.0 unx    12506 b- defN 23-Jan-31 02:59 pawnlib/utils/http.py
 -rw-r--r--  2.0 unx    12365 b- defN 23-Jan-31 02:23 pawnlib/utils/icx_signer.py
 -rw-r--r--  2.0 unx    12172 b- defN 23-Jan-31 05:22 pawnlib/utils/log.py
 -rw-r--r--  2.0 unx     5929 b- defN 23-Jan-31 06:40 pawnlib/utils/notify.py
 -rw-r--r--  2.0 unx    22138 b- defN 23-Jan-31 06:38 pawnlib/utils/operate_handler.py
--rw-r--r--  2.0 unx     5042 b- defN 23-Feb-08 02:53 pawnlib-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-08 02:53 pawnlib-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Feb-08 02:53 pawnlib-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Feb-08 02:53 pawnlib-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3601 b- defN 23-Feb-08 02:53 pawnlib-0.1.8.dist-info/RECORD
-44 files, 267563 bytes uncompressed, 72924 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx     5042 b- defN 23-Feb-08 03:22 pawnlib-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-08 03:22 pawnlib-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Feb-08 03:22 pawnlib-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Feb-08 03:22 pawnlib-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3601 b- defN 23-Feb-08 03:22 pawnlib-0.1.9.dist-info/RECORD
+44 files, 268584 bytes uncompressed, 73123 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -111,23 +111,23 @@
 
 Filename: pawnlib/utils/notify.py
 Comment: 
 
 Filename: pawnlib/utils/operate_handler.py
 Comment: 
 
-Filename: pawnlib-0.1.8.dist-info/METADATA
+Filename: pawnlib-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: pawnlib-0.1.8.dist-info/WHEEL
+Filename: pawnlib-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: pawnlib-0.1.8.dist-info/entry_points.txt
+Filename: pawnlib-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: pawnlib-0.1.8.dist-info/top_level.txt
+Filename: pawnlib-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pawnlib-0.1.8.dist-info/RECORD
+Filename: pawnlib-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pawnlib/__version__.py

```diff
@@ -1,9 +1,9 @@
 ####
 __title__ = 'pawnlib'
 __description__ = 'pawnlib is a collection of libraries for IaC.'
 __url__ = 'https://github.com/jinwoo-j/pawnlib'
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 __author__ = 'Jinwoo Jeong'
 __author_email__ = 'jinwoo@iconloop.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022 JINWOO'
```

## pawnlib/typing/converter.py

```diff
@@ -1595,14 +1595,56 @@
         value = value.replace(" ", "_").strip()
         result += f"{key}{operator}{value}"
         if count < len(key_values):
             result += sep
     return result
 
 
+def extract_values_in_list(key: Any, list_of_dicts: list = []):
+    """
+    Extract the values from a list of dictionaries.
+
+    :param key:
+    :param list_of_dicts:
+    :return:
+
+    Example:
+
+        .. code-block:: python
+
+            from pawnlib.typing import converter
+            sample_list = [
+                {
+                    "name": "John Doe",
+                    "age": 30,
+                    "height": 1.75,
+                    "weight": 70,
+                },{
+                    "name": "John",
+                    "age": 32,
+                    "height": 1.71,
+                    "weight": 71,
+                }
+            ]
+
+            print(extract_values_in_list("age", sample_list))
+            # [30, 32]
+
+            print(extract_values_in_list("none_key", sample_list))
+            # []
+
+    """
+    result = []
+    if isinstance(list_of_dicts, list):
+        for _dict in list_of_dicts:
+            if _dict.get(key):
+                result.append(_dict.get(key))
+    return result
+
+
 def split_every_n(data, n):
     return [data[i:i + n] for i in range(0, len(data), n)]
 
 
 def class_extract_attr_list(obj, attr_name="name"):
     if isinstance(obj, list):
         return_list = []
```

## Comparing `pawnlib-0.1.8.dist-info/METADATA` & `pawnlib-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawnlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: pawnlib is a collection of libraries for IaC.
 Home-page: https://github.com/jinwoo-j/pawnlib
 Author: Jinwoo Jeong
 Author-email: jinwoo@iconloop.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `pawnlib-0.1.8.dist-info/RECORD` & `pawnlib-0.1.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pawnlib/__init__.py,sha256=FXDHsJ3zZkGKwHLxXvy0z-DLH9UwQvGh7SoLiigPptw,1188
 pawnlib/__main__.py,sha256=wmMMh9f5l39HY6p_IfARRZwRDcK1rnfENZdCb9tzJYg,1224
-pawnlib/__version__.py,sha256=WHy4Niw1jGg8OUM1ESy8V2bq6EtQgUOyaxHepoz8CVQ,292
+pawnlib/__version__.py,sha256=WRpOMFQni8aLTOUrOqiQDzuk2SSwfYK9tlQyzwwF-hM,292
 pawnlib/asyncio/__init__.py,sha256=ToWEND0eBP0YeJw4xZaBPLgQ-BGSeIvIApyysQMCsgo,19
 pawnlib/asyncio/run.py,sha256=S5WG6HuT_JF2FqaxYbEDvzTzwxdFS3thPs8eF19cRQA,2952
 pawnlib/builder/__init__.py,sha256=2uuVV8xTTPsD8SCN1PDLhAcKOKISEZLQCQgOeritMrE,36
 pawnlib/builder/generator.py,sha256=4nsaQvZpzaLpIYLovIqmofBmyItj6nApae9zFdmvIuQ,5382
 pawnlib/builder/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pawnlib/builder/templates/app_with_logging.tmpl,sha256=1x2OfxuzVzuKV0dSCGj9gpCR3WEoQtd5TudEktNAlRE,2195
 pawnlib/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -23,22 +23,22 @@
 pawnlib/output/file.py,sha256=V2_kYLQo5EG-PTeQa-HtYFhWagCGoV5PTkPUh8K0vUI,6198
 pawnlib/resource/__init__.py,sha256=0ijpoXW4ZYN3IaQWExMHtukZZWn5DUPu5bWYz4gx5Hk,288
 pawnlib/resource/net.py,sha256=W8TwyXkXzhiTEqgZi-0l_alljzOw7bo4OC7iNkvb5wE,6568
 pawnlib/resource/server.py,sha256=T3_qcSL3TCxJ5AT9d3kBw_EQARYTpooxVjDdF-5Lo7w,11387
 pawnlib/typing/__init__.py,sha256=MHmQz-2kVsBTIvfghHOOHQYBE4Ztx9dfdtsjkQbZpxM,1653
 pawnlib/typing/check.py,sha256=O0R_jVATbv-bkQpreayhZZgUVG-eMGW8gU2zjBNOJ30,4402
 pawnlib/typing/constants.py,sha256=Rzm92LOI55JT2-nmR1BtZRNFzDEvHa4qDUxecB9MClo,689
-pawnlib/typing/converter.py,sha256=218t4D0VW4kKxZdz2tdgJlkFeHQ38OcMen3YNe_Xdm4,53503
+pawnlib/typing/converter.py,sha256=YlGmg9yv4Hnyw6CwTVpJUoPT_hhAZRLlssSA2cIWnd0,54524
 pawnlib/typing/date_utils.py,sha256=nNpliOVgREsQiBlynoqI26jWIc8NdZ7QaXjNmXGCj0U,7137
 pawnlib/typing/defines.py,sha256=rub1puD3M_WHUcwR0hG59lu9df_jQA0LzrT1HxYpyYQ,1898
 pawnlib/typing/generator.py,sha256=tAzkL5hJt0le958oYkVjTMbRGmlOwP3gE7mZaD-yXJY,12711
 pawnlib/utils/__init__.py,sha256=NqR4yzkjOYz1rMI2EIe0nti2URz8PFWUNbjkHSMDdek,349
 pawnlib/utils/http.py,sha256=PV0R-N3-3tHdsThpglnSP8EdATFCvW1etA3ujYjMaVo,12506
 pawnlib/utils/icx_signer.py,sha256=-NJIKOv6BR9Uc8LVK6R9G7VQmJb1Em-AXlUDppX4VbM,12365
 pawnlib/utils/log.py,sha256=zYClSlvFJt9ZxZpApWvFZ7EcFRFtwUIyCyrtmUdfiLI,12172
 pawnlib/utils/notify.py,sha256=UlQyJSfH7_NYxIcec84SDFDV3lBhbQE1CbTsxOHPvQ8,5929
 pawnlib/utils/operate_handler.py,sha256=603oZfZhDB3yWyxeJoZZ-y_HPTu6inP74Q0g9LPWzFo,22138
-pawnlib-0.1.8.dist-info/METADATA,sha256=UYRkSvKkuPn1PER0IagvYSg5Vb9AEUMiRMzo_Xc6Hz0,5042
-pawnlib-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pawnlib-0.1.8.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
-pawnlib-0.1.8.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
-pawnlib-0.1.8.dist-info/RECORD,,
+pawnlib-0.1.9.dist-info/METADATA,sha256=Tsl2vnNvtXveq1s3vG0jLnktIsm0buQv5SEiE1vG-T8,5042
+pawnlib-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pawnlib-0.1.9.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
+pawnlib-0.1.9.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
+pawnlib-0.1.9.dist-info/RECORD,,
```

