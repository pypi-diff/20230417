# Comparing `tmp/markdown-exec-1.4.0.tar.gz` & `tmp/markdown_exec-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-exec-1.4.0.tar", last modified: Wed Mar 15 20:43:30 2023, max compression
+gzip compressed data, was "markdown_exec-1.4.1.tar", last modified: Sun Apr 16 18:26:45 2023, max compression
```

## Comparing `markdown-exec-1.4.0.tar` & `markdown_exec-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      754 2023-02-05 13:04:21.887252 markdown-exec-1.4.0/LICENSE
--rw-r--r--   0        0        0     3181 2023-03-07 19:40:08.710236 markdown-exec-1.4.0/README.md
--rw-r--r--   0        0        0     4226 2023-02-18 12:34:04.245221 markdown-exec-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4016 2023-03-15 20:14:16.682872 markdown-exec-1.4.0/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     5657 2023-02-18 12:34:04.251887 markdown-exec-1.4.0/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown-exec-1.4.0/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4273 2023-03-15 19:55:54.456239 markdown-exec-1.4.0/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      733 2023-01-27 11:27:12.010702 markdown-exec-1.4.0/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      766 2023-01-26 23:29:24.054562 markdown-exec-1.4.0/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      247 2023-01-26 23:02:30.685829 markdown-exec-1.4.0/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      728 2023-02-05 22:43:19.191288 markdown-exec-1.4.0/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     1486 2023-03-15 20:38:55.268625 markdown-exec-1.4.0/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      723 2023-01-27 11:27:12.014035 markdown-exec-1.4.0/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2094 2022-08-31 21:38:40.781039 markdown-exec-1.4.0/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2125 2022-05-11 20:15:37.562034 markdown-exec-1.4.0/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     2286 2023-02-18 12:34:04.251887 markdown-exec-1.4.0/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0        0 2023-02-05 13:04:21.390597 markdown-exec-1.4.0/src/markdown_exec/py.typed
--rw-r--r--   0        0        0     5675 2023-02-18 12:34:32.904786 markdown-exec-1.4.0/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2023-02-05 13:04:21.387264 markdown-exec-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0      642 2023-02-05 13:04:22.160579 markdown-exec-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1433 2023-02-18 12:42:25.607639 markdown-exec-1.4.0/tests/test_base_formatter.py
--rw-r--r--   0        0        0     2968 2023-03-15 20:36:59.550759 markdown-exec-1.4.0/tests/test_python.py
--rw-r--r--   0        0        0     1858 2023-01-27 11:29:31.950208 markdown-exec-1.4.0/tests/test_shell.py
--rw-r--r--   0        0        0      486 2022-08-31 20:38:18.561843 markdown-exec-1.4.0/tests/test_tree.py
--rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown-exec-1.4.0/tests/test_validator.py
--rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 markdown-exec-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-04-10 19:47:46.084183 markdown_exec-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3354 2023-04-10 19:47:48.247486 markdown_exec-1.4.1/README.md
+-rw-r--r--   0        0        0     3595 2023-04-16 18:26:45.518380 markdown_exec-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4053 2023-04-10 19:52:01.520574 markdown_exec-1.4.1/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     5657 2023-02-18 12:34:04.251887 markdown_exec-1.4.1/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0       51 2022-11-24 19:29:10.145475 markdown_exec-1.4.1/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-16 17:38:22.998491 markdown_exec-1.4.1/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      846 2023-04-16 17:59:46.215238 markdown_exec-1.4.1/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-03-16 19:48:00.312652 markdown_exec-1.4.1/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-03-16 19:47:25.386530 markdown_exec-1.4.1/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      778 2023-03-16 19:45:37.928204 markdown_exec-1.4.1/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2406 2023-04-16 18:25:10.659529 markdown_exec-1.4.1/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      836 2023-04-16 18:00:27.374551 markdown_exec-1.4.1/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-04-10 19:31:13.183765 markdown_exec-1.4.1/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2089 2023-03-16 19:40:46.186083 markdown_exec-1.4.1/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     2450 2023-03-16 19:51:07.785411 markdown_exec-1.4.1/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:47:45.977517 markdown_exec-1.4.1/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0     5665 2023-04-10 19:47:04.774761 markdown_exec-1.4.1/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2023-04-10 19:47:45.974184 markdown_exec-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      635 2023-04-10 19:47:48.247486 markdown_exec-1.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-04-10 19:58:25.733492 markdown_exec-1.4.1/tests/test_base_formatter.py
+-rw-r--r--   0        0        0     3896 2023-04-16 18:24:56.359699 markdown_exec-1.4.1/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-04-10 20:00:44.382565 markdown_exec-1.4.1/tests/test_shell.py
+-rw-r--r--   0        0        0      488 2023-03-16 19:34:00.679063 markdown_exec-1.4.1/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2022-02-06 15:25:17.240565 markdown_exec-1.4.1/tests/test_validator.py
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 markdown_exec-1.4.1/PKG-INFO
```

### Comparing `markdown-exec-1.4.0/LICENSE` & `markdown_exec-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-exec-1.4.0/README.md` & `markdown_exec-1.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 ```yaml
 # mkdocs.yml
 plugins:
 - search
 - markdown-exec
 ```
 
+We do recommend enabling Markdown Exec with the MkDocs plugin
+if you are using MkDocs: it will take care of adding relevant
+assets (CSS/JS) to the final site when needed. 
+
 ## Usage
 
 You are now able to execute code blocks instead of displaying them:
 
 ````md
 ```python exec="on"
 print("Hello Markdown!")
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/__init__.py` & `markdown_exec-1.4.1/src/markdown_exec/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-Markdown Exec package.
+"""Markdown Exec package.
 
 Utilities to execute code blocks in Markdown files.
 """
 
 # https://facelessuser.github.io/pymdown-extensions/extensions/superfences/#custom-fences
 # https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#snippets
 
 from __future__ import annotations
 
 import re
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from markdown import Markdown
+if TYPE_CHECKING:
+    from markdown import Markdown
 
 from markdown_exec.formatters.base import default_tabs
-from markdown_exec.formatters.bash import _format_bash  # noqa: WPS450
-from markdown_exec.formatters.console import _format_console  # noqa: WPS450
-from markdown_exec.formatters.markdown import _format_markdown  # noqa: WPS450
-from markdown_exec.formatters.pycon import _format_pycon  # noqa: WPS450
-from markdown_exec.formatters.python import _format_python  # noqa: WPS450
-from markdown_exec.formatters.sh import _format_sh  # noqa: WPS450
-from markdown_exec.formatters.tree import _format_tree  # noqa: WPS450
+from markdown_exec.formatters.bash import _format_bash
+from markdown_exec.formatters.console import _format_console
+from markdown_exec.formatters.markdown import _format_markdown
+from markdown_exec.formatters.pycon import _format_pycon
+from markdown_exec.formatters.python import _format_python
+from markdown_exec.formatters.sh import _format_sh
+from markdown_exec.formatters.tree import _format_tree
 
-__all__: list[str] = ["formatter", "validator"]  # noqa: WPS410
+__all__: list[str] = ["formatter", "validator"]
 
 
 formatters = {
     "bash": _format_bash,
     "console": _format_console,
     "md": _format_markdown,
     "markdown": _format_markdown,
@@ -39,15 +39,19 @@
 }
 
 # negative look behind: matches only if | (pipe) if not preceded by \ (backslash)
 _tabs_re = re.compile(r"(?<!\\)\|")
 
 
 def validator(
-    language: str, inputs: dict[str, str], options: dict[str, Any], attrs: dict[str, Any], md: Markdown
+    language: str,
+    inputs: dict[str, str],
+    options: dict[str, Any],
+    attrs: dict[str, Any],  # noqa: ARG001
+    md: Markdown,  # noqa: ARG001
 ) -> bool:
     """Validate code blocks inputs.
 
     Parameters:
         language: The code language, like python or bash.
         inputs: The code block inputs, to be sorted into options and attrs.
         options: The container for options.
@@ -78,21 +82,21 @@
     options["extra"] = inputs
     return True
 
 
 def formatter(
     source: str,
     language: str,
-    css_class: str,
+    css_class: str,  # noqa: ARG001
     options: dict[str, Any],
     md: Markdown,
-    classes: list[str] | None = None,
-    id_value: str = "",
-    attrs: dict[str, Any] | None = None,
-    **kwargs: Any,
+    classes: list[str] | None = None,  # noqa: ARG001
+    id_value: str = "",  # noqa: ARG001
+    attrs: dict[str, Any] | None = None,  # noqa: ARG001
+    **kwargs: Any,  # noqa: ARG001
 ) -> str:
     """Execute code and return HTML.
 
     Parameters:
         source: The code to execute.
         language: The code language, like python or bash.
         css_class: The CSS class to add to the HTML element.
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/ansi.css` & `markdown_exec-1.4.1/src/markdown_exec/ansi.css`

 * *Files identical despite different names*

### Comparing `markdown-exec-1.4.0/src/markdown_exec/formatters/base.py` & `markdown_exec-1.4.1/src/markdown_exec/formatters/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Generic formatter for executing code."""
 
 from __future__ import annotations
 
 from textwrap import indent
-from typing import Any, Callable
+from typing import TYPE_CHECKING, Any, Callable
 from uuid import uuid4
 
-from markdown.core import Markdown
 from markupsafe import Markup
 
 from markdown_exec.logger import get_logger
 from markdown_exec.rendering import MarkdownConverter, add_source, code_block
 
+if TYPE_CHECKING:
+    from markdown.core import Markdown
+
 logger = get_logger(__name__)
 default_tabs = ("Source", "Result")
 
 
 class ExecutionError(Exception):
     """Exception raised for errors during execution of a code block.
 
@@ -25,33 +27,33 @@
     """
 
     def __init__(self, message: str, returncode: int | None = None) -> None:  # noqa: D107
         super().__init__(message)
         self.returncode = returncode
 
 
-def _format_log_details(details: str, strip_fences: bool = False) -> str:
+def _format_log_details(details: str, *, strip_fences: bool = False) -> str:
     if strip_fences:
         lines = details.split("\n")
         if lines[0].startswith("```") and lines[-1].startswith("```"):
             details = "\n".join(lines[1:-1])
     return indent(details, " " * 2)
 
 
-def base_format(  # noqa: WPS231
+def base_format(
     *,
     language: str,
     run: Callable,
     code: str,
     md: Markdown,
     html: bool = False,
     source: str = "",
     result: str = "",
     tabs: tuple[str, str] = default_tabs,
-    id: str = "",  # noqa: A002,VNE003
+    id: str = "",  # noqa: A002
     returncode: int = 0,
     transform_source: Callable[[str], tuple[str, str]] | None = None,
     session: str | None = None,
     **options: Any,
 ) -> Markup:
     """Execute code and return HTML.
 
@@ -81,15 +83,15 @@
     if transform_source:
         source_input, source_output = transform_source(code)
     else:
         source_input = code
         source_output = code
 
     try:
-        output = run(source_input, returncode=returncode, session=session, **extra)
+        output = run(source_input, returncode=returncode, session=session, id=id, **extra)
     except ExecutionError as error:
         identifier = id or extra.get("title", "")
         identifier = identifier and f"'{identifier}' "
         exit_message = "errors" if error.returncode is None else f"unexpected code {error.returncode}"
         log_message = (
             f"Execution of {language} code block {identifier}exited with {exit_message}\n\n"
             f"Code block is:\n\n{_format_log_details(source_input)}\n\n"
@@ -98,15 +100,20 @@
         logger.warning(log_message)
         return markdown.convert(str(error))
 
     if html:
         if source:
             placeholder = str(uuid4())
             wrapped_output = add_source(
-                source=source_output, location=source, output=placeholder, language=language, tabs=tabs, **extra
+                source=source_output,
+                location=source,
+                output=placeholder,
+                language=language,
+                tabs=tabs,
+                **extra,
             )
             return markdown.convert(wrapped_output, stash={placeholder: output})
         return Markup(output)
 
     wrapped_output = output
     if result and source != "console":
         wrapped_output = code_block(result, output)
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.4.1/src/markdown_exec/formatters/bash.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """Formatter for executing shell code."""
 
 from __future__ import annotations
 
-import subprocess  # noqa: S404
+import subprocess
+from typing import Any
 
 from markdown_exec.formatters.base import ExecutionError, base_format
 from markdown_exec.rendering import code_block
 
 
-def _run_bash(code: str, *, returncode: int = 0, **extra: str) -> str:
-    process = subprocess.run(  # noqa: S603,S607
+def _run_bash(
+    code: str,
+    returncode: int | None = None,
+    session: str | None = None,  # noqa: ARG001
+    id: str | None = None,  # noqa: A002,ARG001
+    **extra: str,
+) -> str:
+    process = subprocess.run(
         ["bash", "-c", code],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         text=True,
     )
     if process.returncode != returncode:
         raise ExecutionError(code_block("sh", process.stdout, **extra), process.returncode)
     return process.stdout
 
 
-def _format_bash(**kwargs) -> str:
+def _format_bash(**kwargs: Any) -> str:
     return base_format(language="bash", run=_run_bash, **kwargs)
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/formatters/console.py` & `markdown_exec-1.4.1/src/markdown_exec/formatters/pycon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""Formatter for executing shell console code."""
+"""Formatter for executing `pycon` code."""
 
 from __future__ import annotations
 
-import textwrap
-
-from markupsafe import Markup
+from typing import TYPE_CHECKING, Any
 
 from markdown_exec.formatters.base import base_format
-from markdown_exec.formatters.sh import _run_sh  # noqa: WPS450
+from markdown_exec.formatters.python import _run_python
 from markdown_exec.logger import get_logger
 
+if TYPE_CHECKING:
+    from markupsafe import Markup
+
 logger = get_logger(__name__)
 
 
 def _transform_source(code: str) -> tuple[str, str]:
-    sh_lines = []
+    python_lines = []
     for line in code.split("\n"):
-        prompt = line[:2]
-        if prompt in {"$ ", "% "}:
-            sh_lines.append(line[2:])
-    sh_code = "\n".join(sh_lines)
-    return sh_code, textwrap.indent(sh_code, prompt)
+        if line.startswith((">>> ", "... ")):
+            python_lines.append(line[4:])
+    python_code = "\n".join(python_lines)
+    return python_code, code
 
 
-def _format_console(**kwargs) -> Markup:
-    return base_format(language="console", run=_run_sh, transform_source=_transform_source, **kwargs)
+def _format_pycon(**kwargs: Any) -> Markup:
+    return base_format(language="pycon", run=_run_python, transform_source=_transform_source, **kwargs)
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/formatters/python.py` & `markdown_exec-1.4.1/src/markdown_exec/formatters/python.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,70 @@
 """Formatter for executing Python code."""
 
 from __future__ import annotations
 
 import traceback
+from collections import defaultdict
 from functools import partial
 from io import StringIO
 from typing import Any
 
 from markdown_exec.formatters.base import ExecutionError, base_format
 from markdown_exec.rendering import code_block
 
-_sessions: dict[str, dict] = {}
+_sessions_globals: dict[str, dict] = defaultdict(dict)
+_sessions_counter: dict[str | None, int] = defaultdict(int)
+_code_blocks: dict[str, list[str]] = {}
 
 
-def _buffer_print(buffer: StringIO, *texts: str, end: str = "\n", **kwargs: Any) -> None:
+def _buffer_print(buffer: StringIO, *texts: str, end: str = "\n", **kwargs: Any) -> None:  # noqa: ARG001
     buffer.write(" ".join(str(text) for text in texts) + end)
 
 
-def _run_python(code: str, session: str | None = None, **extra: str) -> str:
-    if session:
-        if session in _sessions:
-            exec_globals = _sessions[session]
-        else:
-            exec_globals = _sessions[session] = {}  # noqa: WPS429
+def _code_block_id(
+    id: str | None = None,  # noqa: A002
+    session: str | None = None,
+    title: str | None = None,
+) -> str:
+    _sessions_counter[session] += 1
+    if id:
+        code_block_id = f"id {id}"
+    elif session:
+        code_block_id = f"session {session}; n{_sessions_counter[session]}"
+        if title:
+            code_block_id = f"{code_block_id}; title {title}"
     else:
-        exec_globals = {}
+        code_block_id = f"n{_sessions_counter[session]}"
+        if title:
+            code_block_id = f"{code_block_id}; title {title}"
+    return f"<code block: {code_block_id}>"
+
+
+def _run_python(
+    code: str,
+    returncode: int | None = None,  # noqa: ARG001
+    session: str | None = None,
+    id: str | None = None,  # noqa: A002
+    **extra: str,
+) -> str:
+    title = extra.get("title", None)
+    code_block_id = _code_block_id(id, session, title)
+    _code_blocks[code_block_id] = code.split("\n")
+    exec_globals = _sessions_globals[session] if session else {}
+
     buffer = StringIO()
     exec_globals["print"] = partial(_buffer_print, buffer)
 
     try:
-        exec(code, exec_globals)  # noqa: S102
-    except Exception as error:
+        compiled = compile(code, filename=code_block_id, mode="exec")
+        exec(compiled, exec_globals)  # noqa: S102
+    except Exception as error:  # noqa: BLE001
         trace = traceback.TracebackException.from_exception(error)
         for frame in trace.stack:
-            if frame.filename == "<string>":
-                frame.filename = "<executed code block>"
-                frame._line = code.split("\n")[frame.lineno - 1]  # type: ignore[attr-defined,operator]  # noqa: WPS437
-        raise ExecutionError(code_block("python", "".join(trace.format()), **extra))
+            if frame.filename.startswith("<code block: "):
+                frame._line = _code_blocks[frame.filename][frame.lineno - 1]  # type: ignore[attr-defined,operator]
+        raise ExecutionError(code_block("python", "".join(trace.format()), **extra)) from error
     return buffer.getvalue()
 
 
-def _format_python(**kwargs) -> str:
+def _format_python(**kwargs: Any) -> str:
     return base_format(language="python", run=_run_python, **kwargs)
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.4.1/src/markdown_exec/formatters/tree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Formatter for file-system trees."""
 
 from __future__ import annotations
 
 from textwrap import dedent
-from typing import Any
-
-from markdown import Markdown
+from typing import TYPE_CHECKING, Any
 
 from markdown_exec.rendering import MarkdownConverter, code_block
 
+if TYPE_CHECKING:
+    from markdown import Markdown
+
 
-def _rec_build_tree(lines: list[str], parent: list, offset: int, base_indent: int):
+def _rec_build_tree(lines: list[str], parent: list, offset: int, base_indent: int) -> int:
     while offset < len(lines):
         line = lines[offset]
         lstripped = line.lstrip()
         indent = len(line) - len(lstripped)
         if indent == base_indent:
             parent.append((lstripped, []))
             offset += 1
@@ -28,20 +29,20 @@
 def _build_tree(code: str) -> list[tuple[str, list]]:
     lines = dedent(code.strip()).split("\n")
     root_layer: list[tuple[str, list]] = []
     _rec_build_tree(lines, root_layer, 0, 0)
     return root_layer
 
 
-def _rec_format_tree(tree, root=True) -> list[str]:  # noqa: WPS231
+def _rec_format_tree(tree: list[tuple[str, list]], *, root: bool = True) -> list[str]:
     lines = []
     n_items = len(tree)
     for index, node in enumerate(tree):
         last = index == n_items - 1
-        prefix = "" if root else f"{'└' if last else '├'}── "  # noqa: WPS509
+        prefix = "" if root else f"{'└' if last else '├'}── "
         if node[1]:
             lines.append(f"{prefix}📁 {node[0]}")
             sublines = _rec_format_tree(node[1], root=False)
             if root:
                 lines.extend(sublines)
             else:
                 indent_char = " " if last else "│"
@@ -49,19 +50,11 @@
         else:
             name = node[0].split()[0]
             icon = "📁" if name.endswith("/") else "📄"
             lines.append(f"{prefix}{icon} {node[0]}")
     return lines
 
 
-def _format_tree(  # noqa: WPS231
-    code: str,
-    md: Markdown,
-    html: bool,
-    source: str,
-    result: str,
-    tabs: tuple[str, str],
-    **options: Any,
-) -> str:
+def _format_tree(code: str, md: Markdown, result: str, **options: Any) -> str:
     markdown = MarkdownConverter(md)
     output = "\n".join(_rec_format_tree(_build_tree(code)))
     return markdown.convert(code_block(result or "bash", output, **options.get("extra", {})))
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/logger.py` & `markdown_exec-1.4.1/src/markdown_exec/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,41 +23,41 @@
 def get_logger(name):
     logger = logging.getLogger(f"mkdocs.plugins.{name}")
     return LoggerAdapter(name.split(".", 1)[0], logger)
 
 
 patch_loggers(get_logger)
 ```
-"""  # noqa: P102
+"""
 
 from __future__ import annotations
 
 import logging
 from typing import Any, Callable
 
 
 class _Logger:
     _default_logger: Any = logging.getLogger
     _instances: dict[str, _Logger] = {}
 
-    def __init__(self, name: str):
+    def __init__(self, name: str) -> None:
         # default logger that can be patched by third-party
-        self._logger = self.__class__._default_logger(name)  # noqa: WPS437
+        self._logger = self.__class__._default_logger(name)
         # register instance
         self._instances[name] = self
 
     def __getattr__(self, name: str) -> Any:
         # forward everything to the logger
         return getattr(self._logger, name)
 
     @classmethod
-    def _patch_loggers(cls, get_logger_func):
+    def _patch_loggers(cls, get_logger_func: Callable) -> None:
         # patch current instances
         for name, instance in cls._instances.items():
-            instance._logger = get_logger_func(name)  # noqa: WPS437
+            instance._logger = get_logger_func(name)
         # future instances will be patched as well
         cls._default_logger = get_logger_func
 
 
 def get_logger(name: str) -> _Logger:
     """Create and return a new logger instance.
 
@@ -72,8 +72,8 @@
 
 def patch_loggers(get_logger_func: Callable[[str], Any]) -> None:
     """Patch loggers.
 
     Parameters:
         get_logger_func: A function accepting a name as parameter and returning a logger.
     """
-    _Logger._patch_loggers(get_logger_func)  # noqa: WPS437
+    _Logger._patch_loggers(get_logger_func)
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.4.1/src/markdown_exec/mkdocs_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module contains an optional plugin for MkDocs."""
 
 from __future__ import annotations
 
 import logging
 import os
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, MutableMapping
 
 from mkdocs.config import Config, config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.utils import write_file
 
 from markdown_exec import formatter, formatters, validator
 from markdown_exec.logger import patch_loggers
@@ -23,50 +23,50 @@
 except ImportError:
     ansi_ok = False
 else:
     ansi_ok = True
 
 
 class _LoggerAdapter(logging.LoggerAdapter):
-    def __init__(self, prefix, logger):
+    def __init__(self, prefix: str, logger: logging.Logger) -> None:
         super().__init__(logger, {})
         self.prefix = prefix
 
-    def process(self, msg, kwargs):
+    def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> tuple[str, MutableMapping[str, Any]]:
         return f"{self.prefix}: {msg}", kwargs
 
 
-def _get_logger(name):
+def _get_logger(name: str) -> _LoggerAdapter:
     logger = logging.getLogger(f"mkdocs.plugins.{name}")
     return _LoggerAdapter(name.split(".", 1)[0], logger)
 
 
 patch_loggers(_get_logger)
 
 
 class MarkdownExecPlugin(BasePlugin):
     """MkDocs plugin to easily enable custom fences for code blocks execution."""
 
     config_scheme = (("languages", config_options.Type(list, default=list(formatters.keys()))),)
 
-    def on_config(self, config: Config, **kwargs) -> Config:  # noqa: D102
+    def on_config(self, config: Config, **kwargs: Any) -> Config:  # noqa: ARG002,D102
         self.languages = self.config["languages"]
         mdx_configs = config.setdefault("mdx_configs", {})
         superfences = mdx_configs.setdefault("pymdownx.superfences", {})
         custom_fences = superfences.setdefault("custom_fences", [])
         for language in self.languages:
             custom_fences.append(
                 {
                     "name": language,
                     "class": language,
                     "validator": validator,
                     "format": formatter,
-                }
+                },
             )
         return config
 
-    def on_env(self, env: Environment, *, config: Config, files: Files) -> Environment | None:  # noqa: D102
+    def on_env(self, env: Environment, *, config: Config, files: Files) -> Environment | None:  # noqa: ARG002,D102
         css_filename = "assets/_markdown_exec_ansi.css"
         css_content = Path(__file__).parent.joinpath("ansi.css").read_text()
         write_file(css_content.encode("utf-8"), os.path.join(config["site_dir"], css_filename))
         config["extra_css"].insert(0, css_filename)
         return env
```

### Comparing `markdown-exec-1.4.0/src/markdown_exec/rendering.py` & `markdown_exec-1.4.1/src/markdown_exec/rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Markdown extensions and helpers."""
 
 from __future__ import annotations
 
 from itertools import chain
 from textwrap import indent
-from xml.etree.ElementTree import Element
+from typing import TYPE_CHECKING
 
 from markdown import Markdown
 from markdown.treeprocessors import Treeprocessor
 from markupsafe import Markup
 
+if TYPE_CHECKING:
+    from xml.etree.ElementTree import Element
+
 
 def code_block(language: str, code: str, **options: str) -> str:
     """Format code as a code block.
 
     Parameters:
         language: The code block language.
         code: The source code to format.
@@ -33,26 +36,26 @@
         *tabs: Tuples of strings: title and text.
 
     Returns:
         The formatted tabs.
     """
     parts = []
     for title, text in tabs:
-        title = title.replace(r"\|", "|").strip()
+        title = title.replace(r"\|", "|").strip()  # noqa: PLW2901
         parts.append(f'=== "{title}"')
         parts.append(indent(text, prefix=" " * 4))
         parts.append("")
     return "\n".join(parts)
 
 
 def _hide_lines(source: str) -> str:
     return "\n".join(line for line in source.split("\n") if "markdown-exec: hide" not in line).strip()
 
 
-def add_source(  # noqa: WPS212
+def add_source(
     *,
     source: str,
     location: str,
     output: str,
     language: str,
     tabs: tuple[str, str],
     result: str = "",
@@ -98,19 +101,19 @@
 
 # code taken from mkdocstrings, credits to @oprypin
 class _IdPrependingTreeprocessor(Treeprocessor):
     """Prepend the configured prefix to IDs of all HTML elements."""
 
     name = "markdown_exec_ids"
 
-    def __init__(self, md: Markdown, id_prefix: str):  # noqa: D107
+    def __init__(self, md: Markdown, id_prefix: str) -> None:
         super().__init__(md)
         self.id_prefix = id_prefix
 
-    def run(self, root: Element):  # noqa: D102,WPS231
+    def run(self, root: Element) -> None:
         if not self.id_prefix:
             return
         for el in root.iter():
             id_attr = el.get("id")
             if id_attr:
                 el.set("id", self.id_prefix + id_attr)
 
@@ -126,23 +129,23 @@
                 for_attr = el.get("for")
                 if for_attr:
                     el.set("for", self.id_prefix + for_attr)
 
 
 def _mimic(md: Markdown) -> Markdown:
     md = getattr(md, "_original_md", md)
-    new_md = Markdown()  # noqa: WPS442
+    new_md = Markdown()
     extensions = list(chain(md.registeredExtensions, ["tables", "md_in_html"]))
     new_md.registerExtensions(extensions, {})
     new_md.treeprocessors.register(
         _IdPrependingTreeprocessor(md, ""),
         _IdPrependingTreeprocessor.name,
         priority=4,  # right after 'toc' (needed because that extension adds ids to headers)
     )
-    new_md._original_md = md  # type: ignore[attr-defined]  # noqa: WPS437
+    new_md._original_md = md  # type: ignore[attr-defined]
     return new_md
 
 
 class MarkdownConverter:
     """Helper class to avoid breaking the original Markdown instance state."""
 
     counter: int = 0
@@ -162,15 +165,15 @@
         """
         md = _mimic(self._md_ref)
 
         # prepare for conversion
         md.treeprocessors[_IdPrependingTreeprocessor.name].id_prefix = f"exec-{MarkdownConverter.counter}--"
         MarkdownConverter.counter += 1
 
-        try:  # noqa: WPS501
+        try:
             converted = md.convert(text)
         finally:
             md.treeprocessors[_IdPrependingTreeprocessor.name].id_prefix = ""
 
         # restore html from stash
         for placeholder, stashed in (stash or {}).items():
             converted = converted.replace(placeholder, stashed)
```

### Comparing `markdown-exec-1.4.0/tests/conftest.py` & `markdown_exec-1.4.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     fences = [
         {
             "name": language,
             "class": language,
             "validator": validator,
             "format": formatter,
         }
-        for language in formatters.keys()
+        for language in formatters
     ]
     return Markdown(
         extensions=["pymdownx.superfences"],
         extension_configs={"pymdownx.superfences": {"custom_fences": fences}},
     )
```

### Comparing `markdown-exec-1.4.0/tests/test_base_formatter.py` & `markdown_exec-1.4.1/tests/test_base_formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         md=md,
         html=html,
         source="tabbed-left",
     )
     assert "Source" in markup
 
 
-def test_render_console_plus_ansi_result(md) -> None:
+def test_render_console_plus_ansi_result(md: Markdown) -> None:
     """Assert we can render source as console style with `ansi` highlight.
 
     Parameters:
         md: A Markdown instance (fixture).
     """
     markup = base_format(
         language="bash",
```

### Comparing `markdown-exec-1.4.0/tests/test_python.py` & `markdown_exec-1.4.1/tests/test_shell.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,87 @@
-"""Tests for the Python formatters."""
+"""Tests for the shell formatters."""
+
+from __future__ import annotations
 
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
-from markdown import Markdown
+if TYPE_CHECKING:
+    import pytest
+    from markdown import Markdown
 
 
 def test_output_markdown(md: Markdown) -> None:
     """Assert Markdown is converted to HTML.
 
     Parameters:
         md: A Markdown instance (fixture).
     """
     html = md.convert(
         dedent(
             """
-            ```python exec="yes"
-            print("**Bold!**")
+            ```sh exec="yes"
+            echo "**Bold!**"
             ```
-            """
-        )
+            """,
+        ),
     )
     assert html == "<p><strong>Bold!</strong></p>"
 
 
 def test_output_html(md: Markdown) -> None:
     """Assert HTML is injected as is.
 
     Parameters:
         md: A Markdown instance (fixture).
     """
     html = md.convert(
         dedent(
             """
-            ```python exec="yes" html="yes"
-            print("**Bold!**")
+            ```sh exec="yes" html="yes"
+            echo "**Bold!**"
             ```
-            """
-        )
+            """,
+        ),
     )
     assert html == "<p>**Bold!**\n</p>"
 
 
-def test_error_raised(md: Markdown, caplog) -> None:
+def test_error_raised(md: Markdown, caplog: pytest.LogCaptureFixture) -> None:
     """Assert errors properly log a warning and return a formatted traceback.
 
     Parameters:
         md: A Markdown instance (fixture).
         caplog: Pytest fixture to capture logs.
     """
     html = md.convert(
         dedent(
             """
-            ```python exec="yes"
-            raise ValueError("oh no!")
+            ```sh exec="yes"
+            echo("wrong syntax")
             ```
-            """
-        )
+            """,
+        ),
     )
-    assert "Traceback" in html
-    assert "ValueError" in html
-    assert "oh no!" in html
-    assert "Execution of python code block exited with errors" in caplog.text
+    assert "error" in html
+    assert "Execution of sh code block exited with unexpected code 2" in caplog.text
 
 
-def test_can_print_non_string_objects(md: Markdown) -> None:
-    """Assert we can print non-string objects.
-
-    Parameters:
-        md: A Markdown instance (fixture).
-    """
-    html = md.convert(
-        dedent(
-            """
-            ```python exec="yes"
-            class NonString:
-                def __str__(self):
-                    return "string"
-
-            nonstring = NonString()
-            print(nonstring, nonstring)
-            ```
-            """
-        )
-    )
-    assert "Traceback" not in html
-
-
-def test_sessions(md: Markdown) -> None:
-    """Assert sessions can be reused.
+def test_return_code(md: Markdown, caplog: pytest.LogCaptureFixture) -> None:
+    """Assert return code is used correctly.
 
     Parameters:
         md: A Markdown instance (fixture).
+        caplog: Pytest fixture to capture logs.
     """
     html = md.convert(
         dedent(
             """
-            ```python exec="1" session="a"
-            a = 1
-            ```
-
-            ```pycon exec="1" session="b"
-            >>> b = 2
-            ```
-
-            ```pycon exec="1" session="a"
-            >>> print(f"a = {a}")
-            >>> try:
-            ...     print(b)
-            ... except NameError:
-            ...     print("ok")
-            ... else:
-            ...     print("ko")
+            ```sh exec="yes" returncode="1"
+            echo Not in the mood
+            exit 1
             ```
-
-            ```python exec="1" session="b"
-            print(f"b = {b}")
-            try:
-                print(a)
-            except NameError:
-                print("ok")
-            else:
-                print("ko")
-            ```
-            """
-        )
+            """,
+        ),
     )
-    assert "a = 1" in html
-    assert "b = 2" in html
-    assert "ok" in html
-    assert "ko" not in html
+    assert "Not in the mood" in html
+    assert "exited with" not in caplog.text
```

### Comparing `markdown-exec-1.4.0/tests/test_validator.py` & `markdown_exec-1.4.1/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown-exec-1.4.0/PKG-INFO` & `markdown_exec-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.4.0
+Version: 1.4.1
 Summary: Utilities to execute code blocks in Markdown files.
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Provides-Extra: ansi
+Project-URL: Homepage, https://pawamoy.github.io/markdown-exec
+Project-URL: Documentation, https://pawamoy.github.io/markdown-exec
 Project-URL: Changelog, https://pawamoy.github.io/markdown-exec/changelog
+Project-URL: Repository, https://github.com/pawamoy/markdown-exec
+Project-URL: Issues, https://github.com/pawamoy/markdown-exec/issues
 Project-URL: Discussions, https://github.com/pawamoy/markdown-exec/discussions
-Project-URL: Documentation, https://pawamoy.github.io/markdown-exec
-Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/markdown-exec/community
-Project-URL: Homepage, https://pawamoy.github.io/markdown-exec
-Project-URL: Issues, https://github.com/pawamoy/markdown-exec/issues
-Project-URL: Repository, https://github.com/pawamoy/markdown-exec
+Project-URL: Funding, https://github.com/sponsors/pawamoy
+Requires-Python: >=3.7
+Requires-Dist: pymdown-extensions>=9
+Requires-Dist: pygments-ansi-color; extra == "ansi"
+Provides-Extra: ansi
 Description-Content-Type: text/markdown
 
 # Markdown Exec
 
 [![ci](https://github.com/pawamoy/markdown-exec/workflows/ci/badge.svg)](https://github.com/pawamoy/markdown-exec/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/markdown-exec/)
 [![pypi version](https://img.shields.io/pypi/v/markdown-exec.svg)](https://pypi.org/project/markdown-exec/)
@@ -108,14 +109,18 @@
 ```yaml
 # mkdocs.yml
 plugins:
 - search
 - markdown-exec
 ```
 
+We do recommend enabling Markdown Exec with the MkDocs plugin
+if you are using MkDocs: it will take care of adding relevant
+assets (CSS/JS) to the final site when needed. 
+
 ## Usage
 
 You are now able to execute code blocks instead of displaying them:
 
 ````md
 ```python exec="on"
 print("Hello Markdown!")
@@ -131,8 +136,7 @@
 ```bash exec="1" source="tabbed-left" returncode="2"
 grep extra_css README.md && exit 2
 ```
 ````
 
 See [usage](https://pawamoy.github.io/markdown-exec/usage/) for more details,
 and the [gallery](https://pawamoy.github.io/markdown-exec/gallery/) for more examples!
-
```

