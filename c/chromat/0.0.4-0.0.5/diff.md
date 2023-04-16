# Comparing `tmp/chromat-0.0.4.tar.gz` & `tmp/chromat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromat-0.0.4.tar", max compression
+gzip compressed data, was "chromat-0.0.5.tar", max compression
```

## Comparing `chromat-0.0.4.tar` & `chromat-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       60 2023-04-14 16:30:12.300399 chromat-0.0.4/chromat/__init__.py
--rw-r--r--   0        0        0     2405 2023-04-16 01:32:09.534293 chromat-0.0.4/chromat/console.py
--rw-r--r--   0        0        0      146 2023-04-13 19:57:48.808921 chromat-0.0.4/chromat/palettes.py
--rw-r--r--   0        0        0    10281 2023-04-16 01:30:18.308501 chromat-0.0.4/chromat/swatches.py
--rw-r--r--   0        0        0     3004 2023-04-16 01:29:19.967497 chromat-0.0.4/chromat/utils.py
--rw-r--r--   0        0        0     1239 2023-04-16 01:37:00.848418 chromat-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.4/README.md
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 chromat-0.0.4/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 chromat-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-14 16:30:12.300399 chromat-0.0.5/chromat/__init__.py
+-rw-r--r--   0        0        0     2405 2023-04-16 01:32:09.534293 chromat-0.0.5/chromat/console.py
+-rw-r--r--   0        0        0      146 2023-04-13 19:57:48.808921 chromat-0.0.5/chromat/palettes.py
+-rw-r--r--   0        0        0    10612 2023-04-16 21:59:38.809938 chromat-0.0.5/chromat/swatches.py
+-rw-r--r--   0        0        0     3004 2023-04-16 01:29:19.967497 chromat-0.0.5/chromat/utils.py
+-rw-r--r--   0        0        0     1239 2023-04-16 22:00:54.627267 chromat-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.5/README.md
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 chromat-0.0.5/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 chromat-0.0.5/PKG-INFO
```

### Comparing `chromat-0.0.4/chromat/console.py` & `chromat-0.0.5/chromat/console.py`

 * *Files identical despite different names*

### Comparing `chromat-0.0.4/chromat/swatches.py` & `chromat-0.0.5/chromat/swatches.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def __init__(
         self,
         color: Union[str, tuple[int, int, int]] = "#ffffff",
         mode: Literal["hex", "rgb", "hsv"] = "hex",
         name: Optional[str] = None,
     ):
-        self._mode = mode
+        self._mode = mode.lower()
 
         if self._mode == "hex" and isinstance(color, str):
             self._color = hex_to_rgb(color)
             self._mode = "rgb"
         elif isinstance(color, tuple):
             if mode == "hex":
                 raise ValueError("Cannot use hex mode with tuple input.")
@@ -161,30 +161,29 @@
     def v(self):
         return self.value
 
     @property
     def rel_lum(self):
         return self.relative_luminance
 
-    @property
-    def summary_panel(self):
-        return SwatchPanel(self, "summary")
-
-    @property
-    def thumb_panel(self):
-        return SwatchPanel(self, "thumb")
+    def panel(self, mode: Literal["large", "medium", "small"] = "medium"):
+        return SwatchPanel(self, mode)
 
 
 class SwatchPanel(Panel):
-    def __init__(self, swatch: Swatch, mode: Literal["summary", "thumb"]):
-        self.mode = mode
+    def __init__(
+        self,
+        swatch: Swatch,
+        mode: Literal["large", "medium", "small"],
+    ):
+        self.mode = mode.lower()
 
         _style = make_swatch_style(swatch.hex)
 
-        if self.mode == "summary":
+        if self.mode == "large":
             title = Text(
                 swatch.name,
                 style=_style + Style(bold=True),
                 overflow="ellipsis",
             )
             title.truncate(13)
 
@@ -201,27 +200,39 @@
                 ),
                 "subtitle_align": "left",
                 "style": _style,
                 "border_style": _style,
                 "padding": (0, 0),
                 "expand": False,
             }
-        elif self.mode == "thumb":
+
+        elif self.mode == "medium":
             args = {
-                "renderable": " " * 12,
+                "renderable": f"{' ' * 12}\n{' ' * 12}",
                 "subtitle": Text(
                     swatch.name,
                     style=_style + Style(bold=True),
                 ),
                 "subtitle_align": "center",
                 "style": _style,
                 "border_style": _style,
                 "padding": (0, 1),
                 "expand": False,
             }
+
+        elif self.mode == "small":
+            args = {
+                "renderable": f"{' ' * 3}#\n{' ' * 4}",
+                # "renderable": "",
+                "style": _style,
+                "border_style": _style,
+                "padding": (0, 0),
+                "expand": False,
+            }
+
         else:
             raise ValueError(f"Invalid mode: {self.mode}")
 
         super().__init__(**args)
 
 
 class SwatchSummaryTable(Table):
```

### Comparing `chromat-0.0.4/chromat/utils.py` & `chromat-0.0.5/chromat/utils.py`

 * *Files identical despite different names*

### Comparing `chromat-0.0.4/pyproject.toml` & `chromat-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromat"
-version = "0.0.4"
+version = "0.0.5"
 description = "color palettes! under heavy construction!"
 license = "GPL-3.0-or-later"
 authors = ["hex benjamin <hex@hexbenjam.in>"]
 readme = "README.md"
 repository = "https://github.com/hexbenjamin/chromat"
 keywords = ["color", "palette"]
 classifiers = [
```

### Comparing `chromat-0.0.4/setup.py` & `chromat-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['rich>=13.3.4,<14.0.0']
 
 setup_kwargs = {
     'name': 'chromat',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'color palettes! under heavy construction!',
     'long_description': '\ufeff# chromat: algorithmic color palettes\ncoming soon!\n\nhttps://github.com/hexbenjamin/chromat',
     'author': 'hex benjamin',
     'author_email': 'hex@hexbenjam.in',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hexbenjamin/chromat',
```

### Comparing `chromat-0.0.4/PKG-INFO` & `chromat-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromat
-Version: 0.0.4
+Version: 0.0.5
 Summary: color palettes! under heavy construction!
 Home-page: https://github.com/hexbenjamin/chromat
 License: GPL-3.0-or-later
 Keywords: color,palette
 Author: hex benjamin
 Author-email: hex@hexbenjam.in
 Requires-Python: >=3.10,<4.0
```

