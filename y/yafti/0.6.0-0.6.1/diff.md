# Comparing `tmp/yafti-0.6.0.tar.gz` & `tmp/yafti-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafti-0.6.0.tar", max compression
+gzip compressed data, was "yafti-0.6.1.tar", max compression
```

## Comparing `yafti-0.6.0.tar` & `yafti-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-04-12 22:19:04.769860 yafti-0.6.0/LICENSE
--rw-r--r--   0        0        0    10052 2023-04-12 22:19:04.769860 yafti-0.6.0/README.md
--rw-r--r--   0        0        0     1528 2023-04-12 22:19:04.769860 yafti-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      560 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/__main__.py
--rw-r--r--   0        0        0     2081 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/abc.py
--rw-r--r--   0        0        0     1901 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/app.py
--rw-r--r--   0        0        0     1813 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/events.py
--rw-r--r--   0        0        0      532 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/log.py
--rw-r--r--   0        0        0     1571 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/parser.py
--rw-r--r--   0        0        0     6823 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/plugin/flatpak.py
--rw-r--r--   0        0        0     2760 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/plugin/run.py
--rw-r--r--   0        0        0      302 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/registry.py
--rw-r--r--   0        0        0     3278 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/consent.py
--rw-r--r--   0        0        0     2227 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/console.py
--rw-r--r--   0        0        0     1817 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/dialog.py
--rw-r--r--   0        0        0       50 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/__init__.py
--rw-r--r--   0        0        0      317 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/models.py
--rw-r--r--   0        0        0       98 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/__init__.py
--rw-r--r--   0        0        0     5151 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/install.py
--rw-r--r--   0        0        0     4002 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/package.py
--rw-r--r--   0        0        0     5522 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/picker.py
--rw-r--r--   0        0        0     1368 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/state.py
--rw-r--r--   0        0        0      509 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/utils.py
--rw-r--r--   0        0        0     3104 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/title.py
--rw-r--r--   0        0        0     1214 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/utils.py
--rw-r--r--   0        0        0     5216 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/window.py
--rw-r--r--   0        0        0      448 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/setup.py
--rw-r--r--   0        0        0       32 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/share.py
--rw-r--r--   0        0        0    10952 1970-01-01 00:00:00.000000 yafti-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-17 01:36:39.158258 yafti-0.6.1/LICENSE
+-rw-r--r--   0        0        0    10052 2023-04-17 01:36:39.158258 yafti-0.6.1/README.md
+-rw-r--r--   0        0        0     1528 2023-04-17 01:36:39.158258 yafti-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-04-17 01:36:39.158258 yafti-0.6.1/yafti/__init__.py
+-rw-r--r--   0        0        0     1087 2023-04-17 01:36:39.158258 yafti-0.6.1/yafti/__main__.py
+-rw-r--r--   0        0        0     2081 2023-04-17 01:36:39.158258 yafti-0.6.1/yafti/abc.py
+-rw-r--r--   0        0        0     1901 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/app.py
+-rw-r--r--   0        0        0     1813 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/events.py
+-rw-r--r--   0        0        0      532 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/log.py
+-rw-r--r--   0        0        0     1571 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/parser.py
+-rw-r--r--   0        0        0     6823 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/plugin/flatpak.py
+-rw-r--r--   0        0        0     2760 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/plugin/run.py
+-rw-r--r--   0        0        0      302 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/registry.py
+-rw-r--r--   0        0        0     3278 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/consent.py
+-rw-r--r--   0        0        0     2227 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/console.py
+-rw-r--r--   0        0        0     1817 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/dialog.py
+-rw-r--r--   0        0        0       50 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/__init__.py
+-rw-r--r--   0        0        0      317 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/models.py
+-rw-r--r--   0        0        0       98 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/__init__.py
+-rw-r--r--   0        0        0     5232 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/install.py
+-rw-r--r--   0        0        0     4021 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/package.py
+-rw-r--r--   0        0        0     5522 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/picker.py
+-rw-r--r--   0        0        0     1368 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/state.py
+-rw-r--r--   0        0        0      509 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/utils.py
+-rw-r--r--   0        0        0     3413 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/title.py
+-rw-r--r--   0        0        0     1214 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/utils.py
+-rw-r--r--   0        0        0     5216 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/window.py
+-rw-r--r--   0        0        0      448 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/setup.py
+-rw-r--r--   0        0        0       32 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/share.py
+-rw-r--r--   0        0        0    10952 1970-01-01 00:00:00.000000 yafti-0.6.1/PKG-INFO
```

### Comparing `yafti-0.6.0/LICENSE` & `yafti-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/README.md` & `yafti-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/pyproject.toml` & `yafti-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yafti"
-version = "0.6.0"
+version = "0.6.1"
 description = "Yet another first time installer"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/ublue-os/yafti"
 repository = "https://github.com/ublue-os/yafti"
 classifiers = [
```

### Comparing `yafti-0.6.0/yafti/__init__.py` & `yafti-0.6.1/yafti/__init__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/__main__.py` & `yafti-0.6.1/yafti/__main__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/abc.py` & `yafti-0.6.1/yafti/abc.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/app.py` & `yafti-0.6.1/yafti/app.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/events.py` & `yafti-0.6.1/yafti/events.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/log.py` & `yafti-0.6.1/yafti/log.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/parser.py` & `yafti-0.6.1/yafti/parser.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/plugin/flatpak.py` & `yafti-0.6.1/yafti/plugin/flatpak.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/plugin/run.py` & `yafti-0.6.1/yafti/plugin/run.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/consent.py` & `yafti-0.6.1/yafti/screen/consent.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/console.py` & `yafti-0.6.1/yafti/screen/console.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/dialog.py` & `yafti-0.6.1/yafti/screen/dialog.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/package/screen/install.py` & `yafti-0.6.1/yafti/screen/package/screen/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 """
 
 
 @Gtk.Template(string=_xml)
 class PackageInstallScreen(YaftiScreen, Gtk.Box):
     __gtype_name__ = "YaftiPackageInstallScreen"
 
+    status_page = Gtk.Template.Child()
     pkg_progress = Gtk.Template.Child()
     btn_console = Gtk.Template.Child()
     started = False
     already_run = False
     pulse = True
 
     def __init__(
@@ -80,14 +81,15 @@
         package_manager: str = "yafti.plugin.flatpak",
         package_manager_defaults: Optional[dict] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         from yafti.registry import PLUGINS
 
+        self.status_page.set_title(title)
         self.package_manager = PLUGINS.get(package_manager)
         self.package_manager_defaults = package_manager_defaults or {}
         self.btn_console.connect("clicked", self.toggle_console)
 
     async def on_activate(self):
         if self.started or self.already_run:
             return
```

### Comparing `yafti-0.6.0/yafti/screen/package/screen/package.py` & `yafti-0.6.1/yafti/screen/package/screen/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 @Gtk.Template(string=_xml)
 class PackageScreen(YaftiScreen, Adw.Bin):
     __gtype_name__ = "YaftiPackageScreen"
 
     pkg_carousel = Gtk.Template.Child()
 
     class Config(YaftiScreenConfig):
+        title: str
         show_terminal: bool = True
         package_manager: str
         groups: Optional[PackageGroupConfig] = None
         packages: Optional[list[PackageConfig]] = None
         package_manager_defaults: Optional[dict] = None
 
     def __init__(
```

### Comparing `yafti-0.6.0/yafti/screen/package/screen/picker.py` & `yafti-0.6.1/yafti/screen/package/screen/picker.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/package/state.py` & `yafti-0.6.1/yafti/screen/package/state.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/title.py` & `yafti-0.6.1/yafti/screen/title.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import hashlib
 from functools import partial
 from typing import List, Optional
 
 from gi.repository import Adw, Gtk
 
 from yafti import events
 from yafti.abc import YaftiScreen, YaftiScreenConfig
@@ -45,15 +46,15 @@
 
     def __init__(
         self,
         title: str = None,
         description: str = None,
         icon: str = None,
         links: List[dict[str, str]] = None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.status_page.set_title(title)
         self.status_page.set_description(description)
 
         if links:
             links_list_box = self.render_links_list_box()
@@ -66,32 +67,40 @@
         self.status_page.set_child(links_list_box)
         return links_list_box
 
     def append_action_rows(self, links, links_list_box):
         for link in links:
             title, action = list(link.items())[0]
             plugin, config = list(action.items())[0]
-            events.register("on_action_row_open")
-
-            events.on(
-                "on_action_row_open", lambda _: self.on_action_row_open(plugin, config)
+            hash_title = hashlib.md5(
+                title.encode("utf-8"), usedforsecurity=False
+            ).hexdigest()
+            event_name = f"on_action_row_open_{hash_title}"
+            event_fn = partial(
+                TitleScreen.on_action_row_open, plugin=plugin, config=config
             )
 
+            events.register(event_name)
+            events.on(event_name, event_fn)
+
             def do_emit(*args, **kwargs):
                 asyncio.create_task(events.emit(*args, **kwargs))
 
-            _on_clicked = partial(do_emit, "on_action_row_open")
+            _on_clicked = partial(do_emit, event_name)
 
             link_action_row = Adw.ActionRow()
 
             action_btn = Gtk.Button()
             action_btn.set_label("Open")
             action_btn.set_valign(Gtk.Align.CENTER)
             action_btn.connect("clicked", _on_clicked)
 
             link_action_row.set_title(title)
             link_action_row.add_suffix(action_btn)
 
             links_list_box.append(link_action_row)
 
-    async def on_action_row_open(self, plugin, config):
+    @staticmethod
+    async def on_action_row_open(*args, plugin=None, config=None):
+        if not plugin and not config:
+            return
         await PLUGINS.get(plugin)(config)
```

### Comparing `yafti-0.6.0/yafti/screen/utils.py` & `yafti-0.6.1/yafti/screen/utils.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/yafti/screen/window.py` & `yafti-0.6.1/yafti/screen/window.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.0/PKG-INFO` & `yafti-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafti
-Version: 0.6.0
+Version: 0.6.1
 Summary: Yet another first time installer
 Home-page: https://github.com/ublue-os/yafti
 License: Apache 2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: X11 Applications :: GTK
```

