# Comparing `tmp/markdown_exec-1.4.1.tar.gz` & `tmp/markdown_exec-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_exec-1.4.1.tar", last modified: Sun Apr 16 18:26:45 2023, max compression
+gzip compressed data, was "markdown_exec-1.5.0.tar", last modified: Mon Apr 17 12:42:03 2023, max compression
```

## Comparing `markdown_exec-1.4.1.tar` & `markdown_exec-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.4.1/LICENSE
--rw-r--r--   0        0        0     3354 2023-04-10 19:47:48.247486 markdown_exec-1.4.1/README.md
--rw-r--r--   0        0        0     3595 2023-04-16 18:26:45.518380 markdown_exec-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     4053 2023-04-10 19:52:01.520574 markdown_exec-1.4.1/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     5657 2023-02-18 12:34:04.251887 markdown_exec-1.4.1/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.4.1/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4379 2023-04-16 17:38:22.998491 markdown_exec-1.4.1/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      846 2023-04-16 17:59:46.215238 markdown_exec-1.4.1/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      815 2023-03-16 19:48:00.312652 markdown_exec-1.4.1/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      276 2023-03-16 19:47:25.386530 markdown_exec-1.4.1/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      778 2023-03-16 19:45:37.928204 markdown_exec-1.4.1/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     2406 2023-04-16 18:25:10.659529 markdown_exec-1.4.1/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      836 2023-04-16 18:00:27.374551 markdown_exec-1.4.1/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2046 2023-04-10 19:31:13.183765 markdown_exec-1.4.1/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2089 2023-03-16 19:40:46.186083 markdown_exec-1.4.1/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     2450 2023-03-16 19:51:07.785411 markdown_exec-1.4.1/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.4.1/src/markdown_exec/py.typed
--rw-r--r--   0        0        0     5665 2023-04-10 19:47:04.774761 markdown_exec-1.4.1/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0      635 2023-04-10 19:47:48.247486 markdown_exec-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0     1443 2023-04-10 19:58:25.733492 markdown_exec-1.4.1/tests/test_base_formatter.py
--rw-r--r--   0        0        0     3896 2023-04-16 18:24:56.359699 markdown_exec-1.4.1/tests/test_python.py
--rw-r--r--   0        0        0     2027 2023-04-10 20:00:44.382565 markdown_exec-1.4.1/tests/test_shell.py
--rw-r--r--   0        0        0      488 2023-03-16 19:34:00.679063 markdown_exec-1.4.1/tests/test_tree.py
--rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.4.1/tests/test_validator.py
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3354 2023-04-16 18:40:30.714066 markdown_exec-1.5.0/README.md
+-rw-r--r--   0        0        0     3595 2023-04-17 12:42:03.712483 markdown_exec-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4162 2023-04-17 12:40:04.204193 markdown_exec-1.5.0/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     5657 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.5.0/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0     4554 2023-04-17 12:40:04.204193 markdown_exec-1.5.0/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      846 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      778 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2406 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      836 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-04-16 18:40:30.810731 markdown_exec-1.5.0/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2089 2023-04-16 18:40:30.834064 markdown_exec-1.5.0/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     2450 2023-04-17 11:02:02.812131 markdown_exec-1.5.0/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0     4258 2023-04-17 12:40:04.207527 markdown_exec-1.5.0/src/markdown_exec/processors.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.5.0/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0     5990 2023-04-17 12:40:04.204193 markdown_exec-1.5.0/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      635 2023-04-16 18:40:30.837398 markdown_exec-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-04-16 18:40:30.854064 markdown_exec-1.5.0/tests/test_base_formatter.py
+-rw-r--r--   0        0        0     3896 2023-04-16 18:40:30.854064 markdown_exec-1.5.0/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-04-16 18:40:30.854064 markdown_exec-1.5.0/tests/test_shell.py
+-rw-r--r--   0        0        0     2335 2023-04-17 12:40:04.207527 markdown_exec-1.5.0/tests/test_toc.py
+-rw-r--r--   0        0        0      488 2023-04-16 18:40:30.854064 markdown_exec-1.5.0/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.5.0/tests/test_validator.py
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.5.0/PKG-INFO
```

### Comparing `markdown_exec-1.4.1/LICENSE` & `markdown_exec-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/README.md` & `markdown_exec-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/pyproject.toml` & `markdown_exec-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "pymdown-extensions>=9",
 ]
-version = "1.4.1"
+version = "1.5.0"
 
 [project.license]
 text = "ISC"
 
 [project.optional-dependencies]
 ansi = [
     "pygments-ansi-color",
```

### Comparing `markdown_exec-1.4.1/src/markdown_exec/__init__.py` & `markdown_exec-1.5.0/src/markdown_exec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,24 @@
         return False
     id_value = inputs.pop("id", "")
     html_value = _to_bool(inputs.pop("html", "no"))
     source_value = inputs.pop("source", "")
     result_value = inputs.pop("result", "")
     returncode_value = int(inputs.pop("returncode", "0"))
     session_value = inputs.pop("session", "")
+    update_toc_value = _to_bool(inputs.pop("updatetoc", "yes"))
     tabs_value = inputs.pop("tabs", "|".join(default_tabs))
     tabs = tuple(_tabs_re.split(tabs_value, maxsplit=1))
     options["id"] = id_value
     options["html"] = html_value
     options["source"] = source_value
     options["result"] = result_value
     options["returncode"] = returncode_value
     options["session"] = session_value
+    options["update_toc"] = update_toc_value
     options["tabs"] = tabs
     options["extra"] = inputs
     return True
 
 
 def formatter(
     source: str,
```

### Comparing `markdown_exec-1.4.1/src/markdown_exec/ansi.css` & `markdown_exec-1.5.0/src/markdown_exec/ansi.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/base.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     source: str = "",
     result: str = "",
     tabs: tuple[str, str] = default_tabs,
     id: str = "",  # noqa: A002
     returncode: int = 0,
     transform_source: Callable[[str], tuple[str, str]] | None = None,
     session: str | None = None,
+    update_toc: bool = True,
     **options: Any,
 ) -> Markup:
     """Execute code and return HTML.
 
     Parameters:
         language: The code language.
         run: Function that runs code and returns output.
@@ -68,20 +69,22 @@
         tabs: Titles of tabs (if used).
         id: An optional ID for the code block (useful when warning about errors).
         returncode: The expected exit code.
         transform_source: An optional callable that returns transformed versions of the source.
             The input source is the one that is ran, the output source is the one that is
             rendered (when the source option is enabled).
         session: A session name, to persist state between executed code blocks.
+        update_toc: Whether to include generated headings
+            into the Markdown table of contents (toc extension).
         **options: Additional options passed from the formatter.
 
     Returns:
         HTML contents.
     """
-    markdown = MarkdownConverter(md)
+    markdown = MarkdownConverter(md, update_toc=update_toc)
     extra = options.get("extra", {})
 
     if transform_source:
         source_input, source_output = transform_source(code)
     else:
         source_input = code
         source_output = code
```

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/bash.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/console.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/console.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/pycon.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/pycon.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/python.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/sh.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/sh.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.5.0/src/markdown_exec/formatters/tree.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/logger.py` & `markdown_exec-1.5.0/src/markdown_exec/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.5.0/src/markdown_exec/mkdocs_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/src/markdown_exec/rendering.py` & `markdown_exec-1.5.0/src/markdown_exec/rendering.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 """Markdown extensions and helpers."""
 
 from __future__ import annotations
 
+from functools import lru_cache
 from itertools import chain
 from textwrap import indent
 from typing import TYPE_CHECKING
 
 from markdown import Markdown
-from markdown.treeprocessors import Treeprocessor
 from markupsafe import Markup
 
+from markdown_exec.processors import (
+    HeadingReportingTreeprocessor,
+    IdPrependingTreeprocessor,
+    InsertHeadings,
+    RemoveHeadings,
+)
+
 if TYPE_CHECKING:
     from xml.etree.ElementTree import Element
 
 
 def code_block(language: str, code: str, **options: str) -> str:
     """Format code as a code block.
 
@@ -95,87 +102,92 @@
         return tabbed((source_tab_title, source_block), (result_tab_title, output))
     if location == "tabbed-right":
         return tabbed((result_tab_title, output), (source_tab_title, source_block))
 
     raise ValueError(f"unsupported location for sources: {location}")
 
 
-# code taken from mkdocstrings, credits to @oprypin
-class _IdPrependingTreeprocessor(Treeprocessor):
-    """Prepend the configured prefix to IDs of all HTML elements."""
-
-    name = "markdown_exec_ids"
-
-    def __init__(self, md: Markdown, id_prefix: str) -> None:
-        super().__init__(md)
-        self.id_prefix = id_prefix
-
-    def run(self, root: Element) -> None:
-        if not self.id_prefix:
-            return
-        for el in root.iter():
-            id_attr = el.get("id")
-            if id_attr:
-                el.set("id", self.id_prefix + id_attr)
-
-            href_attr = el.get("href")
-            if href_attr and href_attr.startswith("#"):
-                el.set("href", "#" + self.id_prefix + href_attr[1:])
-
-            name_attr = el.get("name")
-            if name_attr:
-                el.set("name", self.id_prefix + name_attr)
-
-            if el.tag == "label":
-                for_attr = el.get("for")
-                if for_attr:
-                    el.set("for", self.id_prefix + for_attr)
+@lru_cache(maxsize=None)
+def _register_headings_processors(md: Markdown) -> None:
+    md.treeprocessors.register(
+        InsertHeadings(md),
+        InsertHeadings.name,
+        priority=75,  # right before markdown.blockprocessors.HashHeaderProcessor
+    )
+    md.treeprocessors.register(
+        RemoveHeadings(md),
+        RemoveHeadings.name,
+        priority=4,  # right after toc
+    )
 
 
-def _mimic(md: Markdown) -> Markdown:
+def _mimic(md: Markdown, headings: list[Element], *, update_toc: bool = True) -> Markdown:
     md = getattr(md, "_original_md", md)
     new_md = Markdown()
     extensions = list(chain(md.registeredExtensions, ["tables", "md_in_html"]))
     new_md.registerExtensions(extensions, {})
     new_md.treeprocessors.register(
-        _IdPrependingTreeprocessor(md, ""),
-        _IdPrependingTreeprocessor.name,
-        priority=4,  # right after 'toc' (needed because that extension adds ids to headers)
+        IdPrependingTreeprocessor(md, ""),
+        IdPrependingTreeprocessor.name,
+        priority=4,  # right after 'toc' (needed because that extension adds ids to headings)
     )
     new_md._original_md = md  # type: ignore[attr-defined]
+
+    if update_toc:
+        _register_headings_processors(md)
+        new_md.treeprocessors.register(
+            HeadingReportingTreeprocessor(md, headings),
+            HeadingReportingTreeprocessor.name,
+            priority=1,  # Close to the end.
+        )
+
     return new_md
 
 
 class MarkdownConverter:
     """Helper class to avoid breaking the original Markdown instance state."""
 
     counter: int = 0
 
-    def __init__(self, md: Markdown) -> None:  # noqa: D107
+    def __init__(self, md: Markdown, *, update_toc: bool = True) -> None:  # noqa: D107
         self._md_ref: Markdown = md
+        self._headings: list[Element] = []
+        self._update_toc = update_toc
 
     def convert(self, text: str, stash: dict[str, str] | None = None) -> Markup:
         """Convert Markdown text to safe HTML.
 
         Parameters:
             text: Markdown text.
             stash: An HTML stash.
 
         Returns:
             Safe HTML.
         """
-        md = _mimic(self._md_ref)
+        md = _mimic(self._md_ref, self._headings, update_toc=self._update_toc)
 
         # prepare for conversion
-        md.treeprocessors[_IdPrependingTreeprocessor.name].id_prefix = f"exec-{MarkdownConverter.counter}--"
+        md.treeprocessors[IdPrependingTreeprocessor.name].id_prefix = f"exec-{MarkdownConverter.counter}--"
         MarkdownConverter.counter += 1
 
         try:
             converted = md.convert(text)
         finally:
-            md.treeprocessors[_IdPrependingTreeprocessor.name].id_prefix = ""
+            md.treeprocessors[IdPrependingTreeprocessor.name].id_prefix = ""
 
         # restore html from stash
         for placeholder, stashed in (stash or {}).items():
             converted = converted.replace(placeholder, stashed)
 
-        return Markup(converted)
+        markup = Markup(converted)
+
+        # pass headings to upstream conversion layer
+        if self._update_toc:
+            self._md_ref.treeprocessors[InsertHeadings.name].headings[markup] = self.headings
+
+        return markup
+
+    @property
+    def headings(self) -> list[Element]:  # noqa: D102
+        headings = self._headings
+        self._headings = []
+        return headings
```

### Comparing `markdown_exec-1.4.1/tests/conftest.py` & `markdown_exec-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/tests/test_base_formatter.py` & `markdown_exec-1.5.0/tests/test_base_formatter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/tests/test_python.py` & `markdown_exec-1.5.0/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/tests/test_shell.py` & `markdown_exec-1.5.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/tests/test_validator.py` & `markdown_exec-1.5.0/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.4.1/PKG-INFO` & `markdown_exec-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.4.1
+Version: 1.5.0
 Summary: Utilities to execute code blocks in Markdown files.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

