# Comparing `tmp/raydl-0.0.8.tar.gz` & `tmp/raydl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raydl-0.0.8.tar", last modified: Mon Apr 10 17:16:36 2023, max compression
+gzip compressed data, was "raydl-0.0.9.tar", last modified: Mon Apr 17 14:53:47 2023, max compression
```

## Comparing `raydl-0.0.8.tar` & `raydl-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.692127 raydl-0.0.8/
--rw-r--r--   0 rayw       (501) staff       (20)     1069 2023-01-24 10:36:02.000000 raydl-0.0.8/LICENSE
--rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-10 17:16:36.691822 raydl-0.0.8/PKG-INFO
--rw-r--r--   0 rayw       (501) staff       (20)      227 2023-01-24 12:20:22.000000 raydl-0.0.8/README.md
--rw-r--r--   0 rayw       (501) staff       (20)     1736 2023-04-10 17:16:01.000000 raydl-0.0.8/pyproject.toml
--rw-r--r--   0 rayw       (501) staff       (20)       38 2023-04-10 17:16:36.692227 raydl-0.0.8/setup.cfg
--rw-r--r--   0 rayw       (501) staff       (20)       38 2023-01-24 12:50:45.000000 raydl-0.0.8/setup.py
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.683941 raydl-0.0.8/src/
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.690100 raydl-0.0.8/src/raydl/
--rw-r--r--   0 rayw       (501) staff       (20)      461 2023-04-10 17:16:01.000000 raydl-0.0.8/src/raydl/__init__.py
--rw-r--r--   0 rayw       (501) staff       (20)     5063 2023-04-10 17:14:21.000000 raydl-0.0.8/src/raydl/__main__.py
--rw-r--r--   0 rayw       (501) staff       (20)     1466 2023-01-31 03:35:05.000000 raydl-0.0.8/src/raydl/collect_env.py
--rw-r--r--   0 rayw       (501) staff       (20)    12896 2023-04-09 16:01:01.000000 raydl-0.0.8/src/raydl/image.py
--rw-r--r--   0 rayw       (501) staff       (20)     4339 2023-04-01 02:56:34.000000 raydl-0.0.8/src/raydl/initialization.py
--rw-r--r--   0 rayw       (501) staff       (20)    13883 2023-04-10 15:30:58.000000 raydl-0.0.8/src/raydl/sfdb.py
--rw-r--r--   0 rayw       (501) staff       (20)     5021 2023-03-29 15:02:33.000000 raydl-0.0.8/src/raydl/tensor.py
--rw-r--r--   0 rayw       (501) staff       (20)     2229 2023-02-25 16:45:04.000000 raydl-0.0.8/src/raydl/time.py
--rw-r--r--   0 rayw       (501) staff       (20)      705 2023-03-18 18:27:59.000000 raydl-0.0.8/src/raydl/utils.py
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.691449 raydl-0.0.8/src/raydl.egg-info/
--rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/PKG-INFO
--rw-r--r--   0 rayw       (501) staff       (20)      396 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/SOURCES.txt
--rw-r--r--   0 rayw       (501) staff       (20)        1 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/dependency_links.txt
--rw-r--r--   0 rayw       (501) staff       (20)       37 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/requires.txt
--rw-r--r--   0 rayw       (501) staff       (20)        6 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/top_level.txt
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-17 14:53:47.752153 raydl-0.0.9/
+-rw-r--r--   0 rayw       (501) staff       (20)     1069 2023-01-24 10:36:02.000000 raydl-0.0.9/LICENSE
+-rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-17 14:53:47.751967 raydl-0.0.9/PKG-INFO
+-rw-r--r--   0 rayw       (501) staff       (20)      227 2023-01-24 12:20:22.000000 raydl-0.0.9/README.md
+-rw-r--r--   0 rayw       (501) staff       (20)     1736 2023-04-17 14:52:50.000000 raydl-0.0.9/pyproject.toml
+-rw-r--r--   0 rayw       (501) staff       (20)       38 2023-04-17 14:53:47.752204 raydl-0.0.9/setup.cfg
+-rw-r--r--   0 rayw       (501) staff       (20)       38 2023-01-24 12:50:45.000000 raydl-0.0.9/setup.py
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-17 14:53:47.747540 raydl-0.0.9/src/
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-17 14:53:47.750969 raydl-0.0.9/src/raydl/
+-rw-r--r--   0 rayw       (501) staff       (20)      534 2023-04-17 14:52:50.000000 raydl-0.0.9/src/raydl/__init__.py
+-rw-r--r--   0 rayw       (501) staff       (20)     5063 2023-04-10 17:14:21.000000 raydl-0.0.9/src/raydl/__main__.py
+-rw-r--r--   0 rayw       (501) staff       (20)     1466 2023-01-31 03:35:05.000000 raydl-0.0.9/src/raydl/collect_env.py
+-rw-r--r--   0 rayw       (501) staff       (20)    13113 2023-04-17 14:50:11.000000 raydl-0.0.9/src/raydl/image.py
+-rw-r--r--   0 rayw       (501) staff       (20)     4339 2023-04-01 02:56:34.000000 raydl-0.0.9/src/raydl/initialization.py
+-rw-r--r--   0 rayw       (501) staff       (20)    14072 2023-04-17 14:42:55.000000 raydl-0.0.9/src/raydl/sfdb.py
+-rw-r--r--   0 rayw       (501) staff       (20)     7446 2023-04-17 14:49:52.000000 raydl-0.0.9/src/raydl/tensor.py
+-rw-r--r--   0 rayw       (501) staff       (20)     2229 2023-02-25 16:45:04.000000 raydl-0.0.9/src/raydl/time.py
+-rw-r--r--   0 rayw       (501) staff       (20)      705 2023-03-18 18:27:59.000000 raydl-0.0.9/src/raydl/utils.py
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-17 14:53:47.751764 raydl-0.0.9/src/raydl.egg-info/
+-rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-17 14:53:47.000000 raydl-0.0.9/src/raydl.egg-info/PKG-INFO
+-rw-r--r--   0 rayw       (501) staff       (20)      396 2023-04-17 14:53:47.000000 raydl-0.0.9/src/raydl.egg-info/SOURCES.txt
+-rw-r--r--   0 rayw       (501) staff       (20)        1 2023-04-17 14:53:47.000000 raydl-0.0.9/src/raydl.egg-info/dependency_links.txt
+-rw-r--r--   0 rayw       (501) staff       (20)       37 2023-04-17 14:53:47.000000 raydl-0.0.9/src/raydl.egg-info/requires.txt
+-rw-r--r--   0 rayw       (501) staff       (20)        6 2023-04-17 14:53:47.000000 raydl-0.0.9/src/raydl.egg-info/top_level.txt
```

### Comparing `raydl-0.0.8/LICENSE` & `raydl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raydl-0.0.8/PKG-INFO` & `raydl-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raydl
-Version: 0.0.8
+Version: 0.0.9
 Summary: The library of utilities to help you deal with the deep learning in PyTorch.
 Author: Ray Wang
 License: MIT License
         
         Copyright (c) [2023] [Ray Wang]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `raydl-0.0.8/pyproject.toml` & `raydl-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "raydl"
-version = "0.0.8"
+version = "0.0.9"
 description = "The library of utilities to help you deal with the deep learning in PyTorch."
 readme = "README.md"
 authors = [{ name = "Ray Wang" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -51,15 +51,15 @@
 ignore = ["UP007", "C408", "B905"]
 line-length=119
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `raydl-0.0.8/src/raydl/__main__.py` & `raydl-0.0.9/src/raydl/__main__.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.8/src/raydl/collect_env.py` & `raydl-0.0.9/src/raydl/collect_env.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.8/src/raydl/image.py` & `raydl-0.0.9/src/raydl/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     images = torch.cat(images).to(device)
     images = images * (value_range[1] - value_range[0]) + value_range[0]
     return images
 
 
 def captioning_pil_image(
     pil_image: Image.Image,
-    captions: Sequence[Union[str, tuple[str, str], None]],
-    grid_cell_size: tuple[int, int],
-    grid_cell_padding: int,
+    captions: Union[Sequence[Union[str, tuple[str, str], None]], str],
+    grid_cell_size: Optional[tuple[int, int]] = None,
+    grid_cell_padding: int = 0,
     caption_color: str = "#ff0000",
     caption_font=DEFAULT_FONT,
 ) -> Image.Image:
     """
     draw captions over grid image. use grid_cell_size to specify minimal cell size in grid.
     :param pil_image: grid image
     :param captions: a sequence of value in (None, str, tuple).
@@ -104,23 +104,32 @@
     :param grid_cell_size: tuple (height, width)
     :param grid_cell_padding: padding when make grid
     :param caption_color: the color of the captions, default is red "#ff0000"
     :param caption_font: the font of the captions, default is DejaVuSans.ttf,
         will find font as https://pillow.readthedocs.io/en/latest/reference/ImageFont.html#PIL.ImageFont.truetype
     :return:
     """
-    h, w = grid_cell_size
-    padding = grid_cell_padding
+    if isinstance(captions, str):
+        captions = [captions]
+
+    if grid_cell_size is None:
+        h, w = pil_image.height, pil_image.width
+        padding = 0
+    else:
+        h, w = grid_cell_size
+        padding = grid_cell_padding
+
     nrow = pil_image.width // w
     im_draw = ImageDraw.Draw(pil_image)
     try:
         im_font = ImageFont.truetype(caption_font, size=max(h // 15, 12))
     except OSError:
         warnings.warn(f"can not find {caption_font}, so use the default font, better than nothing")
         im_font = ImageFont.load_default()
+
     for i, cap in enumerate(captions):
         if cap is None:
             continue
         if isinstance(cap, (tuple, list)):
             cap, fill_color = cap
         else:
             fill_color = caption_color
@@ -150,15 +159,14 @@
     value_range: Optional[tuple[int, int]] = (-1, 1),
     scale_each: bool = False,
     padding: int = 0,
     pad_value: int = 0,
     caption_color: str = "#ff0000",
     caption_font=DEFAULT_FONT,
 ) -> Union[Image.Image, list[Image.Image]]:
-
     if isinstance(captions, bool):
         captions = list(map(str, range(len(images)))) if captions else None
 
     images = images if isinstance(images, torch.Tensor) else torch.cat(images)
     images = resize_images(images, resize=resize)
     if not separately:
         if nrow is None:
```

### Comparing `raydl-0.0.8/src/raydl/initialization.py` & `raydl-0.0.9/src/raydl/initialization.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.8/src/raydl/sfdb.py` & `raydl-0.0.9/src/raydl/sfdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,20 @@
         self._commit_counter = 0
 
         self._is_close = False
 
         self.__max_commit_waiting_time = 60
         self.__max_commit_waiting_updates = 1024 * 16
 
+    def __repr__(self) -> str:
+        return f"{raydl.full_class_name(self)}(_filename={self._filename})"
+
+    def enable_wal(self):
+        self._sqlite.execute("PRAGMA journal_mode=WAL")
+
     @property
     def is_close(self):
         return self._is_close
 
     def _sanity_check(self):
         assert not self._is_close, f"SFDB[{self._filename}] Database already closed."
         assert not self._iterating, f"SFDB[{self._filename}] Database cannot be accessed inside an iterating loop."
@@ -211,17 +217,16 @@
     supported_type = {int: "INTEGER", str: "TEXT", float: "REAL", bytes: "BLOB"}
 
     def __init__(
         self,
         filename: str,
         schema_dataclass,
         type_mappers: Optional[dict[str, TypeMapper]] = None,
-        enable_mapper_guess=False,
+        enable_mapper_guess=True,
     ):
-
         assert dataclasses.is_dataclass(schema_dataclass) and isinstance(schema_dataclass, type)
 
         self.schema = schema_dataclass
 
         guessed_type_mappers = guess_type_mappers(schema_dataclass) if enable_mapper_guess else dict()
         type_mappers = dict() if type_mappers is None else type_mappers
         type_mappers.update(guessed_type_mappers)
```

### Comparing `raydl-0.0.8/src/raydl/time.py` & `raydl-0.0.9/src/raydl/time.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.8/src/raydl/utils.py` & `raydl-0.0.9/src/raydl/utils.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.8/src/raydl.egg-info/PKG-INFO` & `raydl-0.0.9/src/raydl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raydl
-Version: 0.0.8
+Version: 0.0.9
 Summary: The library of utilities to help you deal with the deep learning in PyTorch.
 Author: Ray Wang
 License: MIT License
         
         Copyright (c) [2023] [Ray Wang]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

