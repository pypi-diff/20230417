# Comparing `tmp/pygtkspellcheck-5.0.1.tar.gz` & `tmp/pygtkspellcheck-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygtkspellcheck-5.0.1.tar", max compression
+gzip compressed data, was "pygtkspellcheck-5.0.2.tar", max compression
```

## Comparing `pygtkspellcheck-5.0.1.tar` & `pygtkspellcheck-5.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35147 2022-04-24 09:18:24.907288 pygtkspellcheck-5.0.1/LICENSE
--rw-r--r--   0        0        0     3903 2022-06-28 06:42:54.380798 pygtkspellcheck-5.0.1/README.md
--rw-r--r--   0        0        0     1404 2022-09-17 09:06:20.528103 pygtkspellcheck-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     2332 2022-06-13 12:41:01.173448 pygtkspellcheck-5.0.1/src/gtkspellcheck/__init__.py
--rw-r--r--   0        0        0    13052 2022-04-25 07:14:56.982200 pygtkspellcheck-5.0.1/src/gtkspellcheck/_oxt_extract.py
--rw-r--r--   0        0        0     2143 2022-06-13 13:04:22.195392 pygtkspellcheck-5.0.1/src/gtkspellcheck/_pylocales/__init__.py
--rw-r--r--   0        0        0    29696 2022-04-24 09:18:24.914202 pygtkspellcheck-5.0.1/src/gtkspellcheck/_pylocales/locales.db
--rw-r--r--   0        0        0     5411 2022-06-13 13:04:38.314761 pygtkspellcheck-5.0.1/src/gtkspellcheck/_pylocales/locales.py
--rw-r--r--   0        0        0    34019 2022-09-17 09:08:02.893986 pygtkspellcheck-5.0.1/src/gtkspellcheck/spellcheck.py
--rw-r--r--   0        0        0     4929 2022-09-17 09:08:10.430173 pygtkspellcheck-5.0.1/setup.py
--rw-r--r--   0        0        0     5278 2022-09-17 09:08:10.430458 pygtkspellcheck-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-04-24 09:18:24.907288 pygtkspellcheck-5.0.2/LICENSE
+-rw-r--r--   0        0        0     3903 2022-06-28 06:42:54.380798 pygtkspellcheck-5.0.2/README.md
+-rw-r--r--   0        0        0     1404 2023-04-17 18:14:24.876029 pygtkspellcheck-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2332 2022-06-13 12:41:01.173448 pygtkspellcheck-5.0.2/src/gtkspellcheck/__init__.py
+-rw-r--r--   0        0        0    13096 2023-04-17 18:13:57.254396 pygtkspellcheck-5.0.2/src/gtkspellcheck/_oxt_extract.py
+-rw-r--r--   0        0        0     2143 2022-06-13 13:04:22.195392 pygtkspellcheck-5.0.2/src/gtkspellcheck/_pylocales/__init__.py
+-rw-r--r--   0        0        0    29696 2022-04-24 09:18:24.914202 pygtkspellcheck-5.0.2/src/gtkspellcheck/_pylocales/locales.db
+-rw-r--r--   0        0        0     5411 2022-06-13 13:04:38.314761 pygtkspellcheck-5.0.2/src/gtkspellcheck/_pylocales/locales.py
+-rw-r--r--   0        0        0    34341 2023-04-17 18:11:52.980080 pygtkspellcheck-5.0.2/src/gtkspellcheck/spellcheck.py
+-rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 pygtkspellcheck-5.0.2/PKG-INFO
```

### Comparing `pygtkspellcheck-5.0.1/LICENSE` & `pygtkspellcheck-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygtkspellcheck-5.0.1/README.md` & `pygtkspellcheck-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pygtkspellcheck-5.0.1/pyproject.toml` & `pygtkspellcheck-5.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygtkspellcheck"
-version = "5.0.1"
+version = "5.0.2"
 description = "A simple but quite powerful spellchecking library for GTK written in pure Python."
 authors = ["Maximilian Köhl <mail@koehlma.de>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/koehlma/pygtkspellcheck.git"
 homepage = "https://github.com/koehlma/pygtkspellcheck"
 classifiers = [
```

### Comparing `pygtkspellcheck-5.0.1/src/gtkspellcheck/__init__.py` & `pygtkspellcheck-5.0.2/src/gtkspellcheck/__init__.py`

 * *Files identical despite different names*

### Comparing `pygtkspellcheck-5.0.1/src/gtkspellcheck/_oxt_extract.py` & `pygtkspellcheck-5.0.2/src/gtkspellcheck/_oxt_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     # TODO 5.0: remove this function
     warnings.warn(
         (
             'call to deprecated function "{}", '
             'moved to separate package "oxt_extract", '
             "will be removed in pygtkspellcheck 5.0"
         ).format(extract.__name__),
+        stacklevel=2,
         category=DeprecationWarning,
     )
     try:
         with zipfile.ZipFile(filename, "r") as extension:
             files = extension.namelist()
 
             registry = "dictionaries.xcu"
@@ -248,14 +249,15 @@
     # TODO 5.0: remove this function
     warnings.warn(
         (
             'call to deprecated function "{}", '
             'moved to separate package "oxt_extract", '
             "will be removed in pygtkspellcheck 5.0"
         ).format(extract.__name__),
+        stacklevel=2,
         category=DeprecationWarning,
     )
 
     # get the real, absolute and normalized path
     oxt_path = os.path.normpath(os.path.abspath(os.path.realpath(oxt_path)))
 
     # check that the input directory exists
```

### Comparing `pygtkspellcheck-5.0.1/src/gtkspellcheck/_pylocales/__init__.py` & `pygtkspellcheck-5.0.2/src/gtkspellcheck/_pylocales/__init__.py`

 * *Files identical despite different names*

### Comparing `pygtkspellcheck-5.0.1/src/gtkspellcheck/_pylocales/locales.db` & `pygtkspellcheck-5.0.2/src/gtkspellcheck/_pylocales/locales.db`

 * *Files identical despite different names*

### Comparing `pygtkspellcheck-5.0.1/src/gtkspellcheck/_pylocales/locales.py` & `pygtkspellcheck-5.0.2/src/gtkspellcheck/_pylocales/locales.py`

 * *Files identical despite different names*

### Comparing `pygtkspellcheck-5.0.1/src/gtkspellcheck/spellcheck.py` & `pygtkspellcheck-5.0.2/src/gtkspellcheck/spellcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     ):
         super().__init__()
         self._view = view
         self.collapse = collapse
         # GTK 3-only signals. GTK 4 uses actions, below.
         if _IS_GTK3:
             self._view.connect(
-                "populate-popup", lambda entry, menu: self._extend_menu(menu)
+                "populate-popup", lambda entry, menu: self.populate_menu(menu)
             )
             self._view.connect("popup-menu", self._click_move_popup)
             self._view.connect("button-press-event", self._click_move_button)
         self._prefix = prefix
         self._broker = enchant.Broker()
         if params is not None:
             for param, value in params.items():
@@ -622,14 +622,79 @@
                 self._deferred_check = False
             self._iter_worker.forward_word_end(word_end)
             self._iter_worker.backward_word_start(word_end)
             if word_start.equal(word_end):
                 break
             word_start = word_end.copy()
 
+    def populate_menu(self, menu):
+        """
+        Populate the provided menu with spelling items.
+
+        :param menu: The menu to populate.
+        """
+        # In GTK 4 our existing menu needs to be cleared, providing for disabling
+        if not _IS_GTK3:
+            menu.remove_all()
+
+        if not self._enabled:
+            return
+
+        if _IS_GTK3:
+            separator = Gtk.SeparatorMenuItem.new()
+            separator.show()
+            menu.prepend(separator)
+            languages = Gtk.MenuItem.new_with_label(_("Languages"))
+            languages.set_submenu(self._get_languages_menu())
+            languages.show_all()
+            menu.prepend(languages)
+        else:
+            menu.append_item(self._get_languages_menu())
+
+        if self._marks["click"].inside_word:
+            start, end = self._marks["click"].word
+            if start.has_tag(self._misspelled):
+                word = self._buffer.get_text(start, end, False)
+                items = self._suggestion_menu(word)
+                if self.collapse:
+                    menu_label = _("Suggestions")
+                    if _IS_GTK3:
+                        suggestions = Gtk.MenuItem.new_with_label(menu_label)
+                        submenu = Gtk.Menu.new()
+                    else:
+                        suggestions = Gio.MenuItem.new(menu_label, None)
+                        submenu = Gio.Menu.new()
+                    for item in items:
+                        if _IS_GTK3:
+                            submenu.append(item)
+                        else:
+                            submenu.append_item(item)
+                    suggestions.set_submenu(submenu)
+                    if _IS_GTK3:
+                        suggestions.show_all()
+                        menu.prepend(suggestions)
+                    else:
+                        menu.prepend_item(suggestions)
+                else:
+                    items.reverse()
+                    for item in items:
+                        if _IS_GTK3:
+                            menu.prepend(item)
+                            menu.show_all()
+                        else:
+                            menu.prepend_item(item)
+
+    def move_click_mark(self, iter):
+        """
+        Move the "click" mark, used to determine the word being checked.
+
+        :param iter: TextIter for the new location
+        """
+        self._marks["click"].move(iter)
+
     def _gtk4_setup_actions(self) -> None:
         action_group = Gio.SimpleActionGroup.new()
 
         action = Gio.SimpleAction.new("ignore-all", GLib.VariantType("s"))
         action.connect(
             "activate", lambda _action, word: self.ignore_all(word.get_string())
         )
@@ -749,92 +814,38 @@
         else:
             item = Gio.MenuItem.new(
                 ignore_menu_label, f"spelling.ignore-all('{word_escaped}')"
             )
         menu.append(item)
         return menu
 
-    def _extend_menu(self, menu):
-        # In GTK 4 our existing menu needs to be cleared, providing for disabling
-        if not _IS_GTK3:
-            menu.remove_all()
-
-        if not self._enabled:
-            return
-
-        if _IS_GTK3:
-            separator = Gtk.SeparatorMenuItem.new()
-            separator.show()
-            menu.prepend(separator)
-            languages = Gtk.MenuItem.new_with_label(_("Languages"))
-            languages.set_submenu(self._get_languages_menu())
-            languages.show_all()
-            menu.prepend(languages)
-        else:
-            menu.append_item(self._get_languages_menu())
-
-        if self._marks["click"].inside_word:
-            start, end = self._marks["click"].word
-            if start.has_tag(self._misspelled):
-                word = self._buffer.get_text(start, end, False)
-                items = self._suggestion_menu(word)
-                if self.collapse:
-                    menu_label = _("Suggestions")
-                    if _IS_GTK3:
-                        suggestions = Gtk.MenuItem.new_with_label(menu_label)
-                        submenu = Gtk.Menu.new()
-                    else:
-                        suggestions = Gio.MenuItem.new(menu_label, None)
-                        submenu = Gio.Menu.new()
-                    for item in items:
-                        if _IS_GTK3:
-                            submenu.append(item)
-                        else:
-                            submenu.append_item(item)
-                    suggestions.set_submenu(submenu)
-                    if _IS_GTK3:
-                        suggestions.show_all()
-                        menu.prepend(suggestions)
-                    else:
-                        menu.prepend_item(suggestions)
-                else:
-                    items.reverse()
-                    for item in items:
-                        if _IS_GTK3:
-                            menu.prepend(item)
-                            menu.show_all()
-                        else:
-                            menu.prepend_item(item)
-
     def _click_move_popup(self, *args):
-        self._marks["click"].move(
-            self._buffer.get_iter_at_mark(self._buffer.get_insert())
-        )
+        self.move_click_mark(self._buffer.get_iter_at_mark(self._buffer.get_insert()))
         return False
 
     def _click_move_button(self, widget, event):
         if event.button == 3:
             self._move_mark_for_input(event.x, event.y)
         return False
 
     def _move_mark_for_input(self, input_x, input_y):
         if self._deferred_check:
             self._check_deferred_range(True)
         x, y = self._view.window_to_buffer_coords(2, int(input_x), int(input_y))
         iter = self._view.get_iter_at_location(x, y)
         if isinstance(iter, tuple):
             iter = iter[1]
-        self._marks["click"].move(iter)
+        self.move_click_mark(iter)
 
     def _gtk4_on_textview_click(self, click, n_press, x, y) -> None:
         if n_press != 1 or click.get_current_button() != 3:
             return
 
         self._move_mark_for_input(x, y)
-        self._extend_menu(self._spelling_menu)
+        self.populate_menu(self._spelling_menu)
 
     def _before_text_insert(self, textbuffer, location, text, length):
         self._marks["insert-start"].move(location)
 
     def _after_text_insert(self, textbuffer, location, text, length):
         start = self._marks["insert-start"].iter
         self.check_range(start, location)
```

### Comparing `pygtkspellcheck-5.0.1/setup.py` & `pygtkspellcheck-5.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,102 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pygtkspellcheck
+Version: 5.0.2
+Summary: A simple but quite powerful spellchecking library for GTK written in pure Python.
+Home-page: https://github.com/koehlma/pygtkspellcheck
+License: GPL-3.0-or-later
+Author: Maximilian Köhl
+Author-email: mail@koehlma.de
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: X11 Applications :: GTK
+Classifier: Environment :: X11 Applications :: Gnome
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Localization
+Provides-Extra: docs
+Requires-Dist: PyGObject (>=3.42.1,<4.0.0)
+Requires-Dist: myst-parser (>=0.18.0,<0.19.0) ; extra == "docs"
+Requires-Dist: pyenchant (>=3.0,<4.0)
+Requires-Dist: sphinx (>=4.5.0,<5.0.0) ; extra == "docs"
+Project-URL: Repository, https://github.com/koehlma/pygtkspellcheck.git
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Python GTK Spellcheck
 
-packages = \
-['gtkspellcheck', 'gtkspellcheck._pylocales']
+[![PyPi Project Page](https://img.shields.io/pypi/v/pygtkspellcheck.svg?&label=latest%20version)](https://pypi.python.org/pypi/pygtkspellcheck)
+[![Documentation](https://readthedocs.org/projects/pygtkspellcheck/badge/?version=latest)](https://pygtkspellcheck.readthedocs.org/en/latest/)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyGObject>=3.42.1,<4.0.0', 'pyenchant>=3.0,<4.0']
-
-extras_require = \
-{'docs': ['sphinx>=4.5.0,<5.0.0', 'myst-parser>=0.18.0,<0.19.0']}
-
-setup_kwargs = {
-    'name': 'pygtkspellcheck',
-    'version': '5.0.1',
-    'description': 'A simple but quite powerful spellchecking library for GTK written in pure Python.',
-    'long_description': '# Python GTK Spellcheck\n\n[![PyPi Project Page](https://img.shields.io/pypi/v/pygtkspellcheck.svg?&label=latest%20version)](https://pypi.python.org/pypi/pygtkspellcheck)\n[![Documentation](https://readthedocs.org/projects/pygtkspellcheck/badge/?version=latest)](https://pygtkspellcheck.readthedocs.org/en/latest/)\n\nPython GTK Spellcheck is a simple but quite powerful spellchecking library for GTK written in pure Python. It\'s spellchecking component is based on [Enchant](http://www.abisource.com/projects/enchant/) and it supports both GTK 3 and 4 via [PyGObject](https://live.gnome.org/PyGObject/).\n\n**⚡️ News:** Thanks to [@cheywood](https://github.com/cheywood), Python GTK Spellcheck now supports GTK 4! 🎉\n\n**🟢 Status:** This project is mature, actively maintained, and open to contributions and co-maintainership.\n\n\n## ✨ Features\n\n- **spellchecking** based on [Enchant](http://www.abisource.com/projects/enchant/) for `GtkTextView`\n- support for word, line, and multiline **ignore regular expressions**\n- support for both **GTK 3 and 4** via [PyGObject](https://live.gnome.org/PyGObject/) for Python 3\n- configurable extra word characters such as `\'`\n- localized names of the available languages based on [ISO-Codes](http://pkg-isocodes.alioth.debian.org/)\n- support for custom ignore tags and hot swap of `GtkTextBuffer`\n- support for Hunspell (LibreOffice) and Aspell (GNU) dictionaries\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/koehlma/pygtkspellcheck/master/docs/screenshots/screenshot.png" alt="Screenshot" />\n</p>\n\n\n## 🚀 Getting Started\n\nPython GTK Spellcheck is available from the [Python Package Index](https://pypi.python.org/pypi/pygtkspellcheck):\n```sh\npip install pygtkspellcheck\n```\nDepending on your distribution, you may also find Python GTK Spellcheck in your package manager.\nFor instance, on Debian you may want to install the [`python3-gtkspellcheck`](https://packages.debian.org/bullseye/python3-gtkspellcheck) package.\n\n\n## 🥳 Showcase\n\nOver time, several projects have used Python GTK Spellcheck or are still using it. Among those are:\n\n- [Nested Editor](http://nestededitor.sourceforge.net/about.html): “Specialized editor for structured documents.”\n- [Cherry Tree](http://www.giuspen.com/cherrytree/): “A hierarchical note taking application, […].”\n- [Zim](http://zim-wiki.org/): “Zim is a graphical text editor used to maintain a collection of wiki pages.”\n- [REMARKABLE](http://remarkableapp.github.io/): “The best markdown editor for Linux and Windows.”\n- [RedNotebook](http://rednotebook.sourceforge.net/): “RedNotebook is a modern journal.”\n- [Reportbug](https://packages.debian.org/stretch/reportbug): “Reports bugs in the Debian distribution.”\n- [UberWriter](http://uberwriter.wolfvollprecht.de/): “UberWriter is a writing application for markdown.”\n- [Gourmet](https://github.com/thinkle/gourmet): “Gourmet Recipe Manager is a manager, editor, and organizer for recipes.“\n\n\n## 🔖 Versions\n\nVersion numbers follow [Semantic Versioning](http://semver.org/). However, the update from 3 to 4 pertains only API incompatible changes in `oxt_extract` and not the spellchecking component. The update from 4 to 5 removed support for Python 2, GTK 2, `pylocales`, and the `oxt_extract` API. Otherwise, the API is still compatible with version 3.\n\n\n## 📚 Documentation\n\nThe documentation is available at [Read the Docs](http://pygtkspellcheck.readthedocs.org/).\n\n\n## 🏗 Contributing\n\nWe welcome all kinds of contributions! ❤️\n\nFor minor changes and bug fixes feel free to simply open a pull request. For major changes impacting the overall design of Python GTK Spellcheck, please first [start a discussion](https://github.com/koehlma/pygtkspellcheck/discussions/new?category=ideas) outlining your idea.\n\nBy submitting a PR, you agree to license your contributions under “GPLv3 or later”.\n',
-    'author': 'Maximilian Köhl',
-    'author_email': 'mail@koehlma.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/koehlma/pygtkspellcheck',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+Python GTK Spellcheck is a simple but quite powerful spellchecking library for GTK written in pure Python. It's spellchecking component is based on [Enchant](http://www.abisource.com/projects/enchant/) and it supports both GTK 3 and 4 via [PyGObject](https://live.gnome.org/PyGObject/).
 
+**⚡️ News:** Thanks to [@cheywood](https://github.com/cheywood), Python GTK Spellcheck now supports GTK 4! 🎉
+
+**🟢 Status:** This project is mature, actively maintained, and open to contributions and co-maintainership.
+
+
+## ✨ Features
+
+- **spellchecking** based on [Enchant](http://www.abisource.com/projects/enchant/) for `GtkTextView`
+- support for word, line, and multiline **ignore regular expressions**
+- support for both **GTK 3 and 4** via [PyGObject](https://live.gnome.org/PyGObject/) for Python 3
+- configurable extra word characters such as `'`
+- localized names of the available languages based on [ISO-Codes](http://pkg-isocodes.alioth.debian.org/)
+- support for custom ignore tags and hot swap of `GtkTextBuffer`
+- support for Hunspell (LibreOffice) and Aspell (GNU) dictionaries
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/koehlma/pygtkspellcheck/master/docs/screenshots/screenshot.png" alt="Screenshot" />
+</p>
+
+
+## 🚀 Getting Started
+
+Python GTK Spellcheck is available from the [Python Package Index](https://pypi.python.org/pypi/pygtkspellcheck):
+```sh
+pip install pygtkspellcheck
+```
+Depending on your distribution, you may also find Python GTK Spellcheck in your package manager.
+For instance, on Debian you may want to install the [`python3-gtkspellcheck`](https://packages.debian.org/bullseye/python3-gtkspellcheck) package.
+
+
+## 🥳 Showcase
+
+Over time, several projects have used Python GTK Spellcheck or are still using it. Among those are:
+
+- [Nested Editor](http://nestededitor.sourceforge.net/about.html): “Specialized editor for structured documents.”
+- [Cherry Tree](http://www.giuspen.com/cherrytree/): “A hierarchical note taking application, […].”
+- [Zim](http://zim-wiki.org/): “Zim is a graphical text editor used to maintain a collection of wiki pages.”
+- [REMARKABLE](http://remarkableapp.github.io/): “The best markdown editor for Linux and Windows.”
+- [RedNotebook](http://rednotebook.sourceforge.net/): “RedNotebook is a modern journal.”
+- [Reportbug](https://packages.debian.org/stretch/reportbug): “Reports bugs in the Debian distribution.”
+- [UberWriter](http://uberwriter.wolfvollprecht.de/): “UberWriter is a writing application for markdown.”
+- [Gourmet](https://github.com/thinkle/gourmet): “Gourmet Recipe Manager is a manager, editor, and organizer for recipes.“
+
+
+## 🔖 Versions
+
+Version numbers follow [Semantic Versioning](http://semver.org/). However, the update from 3 to 4 pertains only API incompatible changes in `oxt_extract` and not the spellchecking component. The update from 4 to 5 removed support for Python 2, GTK 2, `pylocales`, and the `oxt_extract` API. Otherwise, the API is still compatible with version 3.
+
+
+## 📚 Documentation
+
+The documentation is available at [Read the Docs](http://pygtkspellcheck.readthedocs.org/).
+
+
+## 🏗 Contributing
+
+We welcome all kinds of contributions! ❤️
+
+For minor changes and bug fixes feel free to simply open a pull request. For major changes impacting the overall design of Python GTK Spellcheck, please first [start a discussion](https://github.com/koehlma/pygtkspellcheck/discussions/new?category=ideas) outlining your idea.
+
+By submitting a PR, you agree to license your contributions under “GPLv3 or later”.
 
-setup(**setup_kwargs)
```

