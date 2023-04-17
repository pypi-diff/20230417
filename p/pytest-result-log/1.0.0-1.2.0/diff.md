# Comparing `tmp/pytest_result_log-1.0.0-py3-none-any.whl.zip` & `tmp/pytest_result_log-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3467 bytes, number of entries: 6
+Zip file size: 4090 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pytest_result_log/__init__.py
--rw-r--r--  2.0 unx     3653 b- defN 16-Jan-01 00:00 pytest_result_log/plugin.py
-?rw-------  2.0 unx       48 b- defN 16-Jan-01 00:00 pytest_result_log-1.0.0.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_result_log-1.0.0.dist-info/WHEEL
-?rw-------  2.0 unx     1520 b- defN 16-Jan-01 00:00 pytest_result_log-1.0.0.dist-info/METADATA
-?rw-------  2.0 unx      508 b- defN 16-Jan-01 00:00 pytest_result_log-1.0.0.dist-info/RECORD
-6 files, 5816 bytes uncompressed, 2535 bytes compressed:  56.4%
+-rw-r--r--  2.0 unx      148 b- defN 16-Jan-01 00:00 pytest_result_log/hooks.py
+-rw-r--r--  2.0 unx     4791 b- defN 16-Jan-01 00:00 pytest_result_log/plugin.py
+?rw-------  2.0 unx       48 b- defN 16-Jan-01 00:00 pytest_result_log-1.2.0.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_result_log-1.2.0.dist-info/WHEEL
+?rw-------  2.0 unx     1520 b- defN 16-Jan-01 00:00 pytest_result_log-1.2.0.dist-info/METADATA
+?rw-------  2.0 unx      590 b- defN 16-Jan-01 00:00 pytest_result_log-1.2.0.dist-info/RECORD
+7 files, 7184 bytes uncompressed, 3030 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: pytest_result_log/__init__.py
 Comment: 
 
+Filename: pytest_result_log/hooks.py
+Comment: 
+
 Filename: pytest_result_log/plugin.py
 Comment: 
 
-Filename: pytest_result_log-1.0.0.dist-info/entry_points.txt
+Filename: pytest_result_log-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_result_log-1.0.0.dist-info/WHEEL
+Filename: pytest_result_log-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_result_log-1.0.0.dist-info/METADATA
+Filename: pytest_result_log-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pytest_result_log-1.0.0.dist-info/RECORD
+Filename: pytest_result_log-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_result_log/plugin.py

```diff
@@ -2,37 +2,42 @@
 from string import Template
 
 import pytest
 from _pytest.reports import BaseReport
 
 logger = logging.getLogger("pytest_result_log")
 
-__test_set = set()
-
 template = ""
 level_map = {}
 enable_plugin = True
+enable_separator = True
 
 
 def pytest_cmdline_parse():
     global __test_set
 
     __test_set = set()
 
 
 def pytest_addoption(parser):
     parser.addini(
         "result_log",
         type="bool",
         default=True,
-        help="用例执行结果的日志格式",
+        help="是否在日志中【记录】用例结果",
+    )
+    parser.addini(
+        "result_log_separator",
+        type="bool",
+        default=True,
+        help="是否在日志中【划线分隔】用例结果",
     )
     parser.addini(
         "result_log_format",
-        default="test status is ${result} (${case_id}): ${reason}",
+        default="test status is ${result_word} (${case_id}): ${reason}",
         help="用例执行结果的日志格式",
     )
     parser.addini(
         "result_log_passed",
         default="info",
         help="用例执行通过的的日志等级",
     )
@@ -55,68 +60,79 @@
         "result_log_xpass",
         default="warning",
         help="用例意外通过的的日志等级",
     )
     parser.addini(
         "result_log_xfail",
         default="warning",
-        help="用例逾期失败的的日志等级",
+        help="用例预期失败的的日志等级",
+    )
+    parser.addini(
+        "result_log_verbose",
+        default="debug",
+        help="失败详情的日志等级",
     )
 
 
+def pytest_addhooks(pluginmanager):
+    from . import hooks
+
+    pluginmanager.add_hookspecs(hooks)
+
+
 def pytest_configure(config):
-    global template, level_map, enable_plugin
+    global template, level_map, enable_plugin, enable_separator
     enable_plugin = config.getini("result_log")
+    enable_separator = config.getini("result_log_separator")
 
     template = config.getini("result_log_format")
     level_map = {
         "PASSED": config.getini("result_log_passed"),
         "FAILED": config.getini("result_log_failed"),
         "ERROR": config.getini("result_log_error"),
         "SKIPPED": config.getini("result_log_skipped"),
         "XPASS": config.getini("result_log_xpass"),
         "XFAIL": config.getini("result_log_xfail"),
+        "VERBOSE": config.getini("result_log_verbose"),
     }
 
+    config.pluginmanager.register(Logger())
+
+
+def pytest_runtest_setup(item):
+    if enable_plugin and enable_separator:
+        logger.info(f"Start: {item.nodeid}".center(60, "-"))
+
+
+def pytest_runtest_teardown(item):
+    if enable_plugin and enable_separator:
+        logger.info(f"End: {item.nodeid}".center(60, "-"))
+
 
 @pytest.hookimpl(hookwrapper=True, trylast=True)
-def pytest_report_teststatus(report: BaseReport):
+def pytest_report_teststatus(report: BaseReport, config: pytest.Config):
     outcome = yield
 
     if not enable_plugin:
         return
 
     result = outcome.get_result()
 
-    if report.nodeid in __test_set:
-        return
+    if report.when == "setup" and result[1] in ["s", "E"]:
+        config.hook.pytest_result_log(report=report, config=config, result=result)
 
-    if report.when == "setup":
-        match result[1]:
-            case "s":
-                log(report.nodeid, result[2], *get_reason(report, "s"))
-            case "E":
-                log(report.nodeid, result[2], *get_reason(report, "E"))
-
-    if report.when == "call":
-
-        match result[1]:
-            case ".":
-                log(report.nodeid, result[2])
-            case "F" | "x":
-                log(report.nodeid, result[2], *get_reason(report, "F"))
-            case "X":
-                log(report.nodeid, result[2])
+    if report.when == "call" and result[1] in [".", "F", "x", "X"]:
+        config.hook.pytest_result_log(report=report, config=config, result=result)
 
 
 def get_reason(report: BaseReport, result="F"):
     reason = "unknown"
 
     match result:
-        case "F":
+        case "F" | "x":
             try:
                 reason = report.longrepr.reprtraceback.reprentries[
                     -1
                 ].reprfileloc.message
             except Exception:
                 ...
         case "E":
@@ -125,20 +141,37 @@
             except Exception:
                 ...
         case "s":
             try:
                 reason = report.longrepr[2]
             except Exception:
                 ...
+        case _:
+            reason = ""
 
     return reason, report.longreprtext
 
 
-def log(case_id, result, reason=None, detail=None):
-    level = level_map.get(result, "warning").lower()
-    f = getattr(logger, level)
-    f(Template(template).safe_substitute(**locals()))
-
-    if detail:
-        logger.debug(f"{case_id} -> {detail}")
+class Logger:
+    def __init__(self):
+        self.test_set = set()
+
+    def pytest_result_log(
+        self, report: BaseReport, config: pytest.Config, result: tuple
+    ):
+        if report.nodeid in self.test_set:
+            return
+        case_id = report.nodeid
+        result_char = result[1]
+        result_word = result[2]
+        reason, detail = get_reason(report, result_char)
+
+        level = level_map.get(result_word, "warning").lower()
+        f = getattr(logger, level)
+        f(Template(template).safe_substitute(**locals()))
+
+        if detail:
+            verbose_level = level_map.get("VERBOSE", "debug").lower()
+            f = getattr(logger, verbose_level)(f"{case_id} -> {detail}")
 
-    __test_set.add(case_id)
+        self.test_set.add(case_id)
+        return case_id, result_word
```

## Comparing `pytest_result_log-1.0.0.dist-info/METADATA` & `pytest_result_log-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-result-log
-Version: 1.0.0
+Version: 1.2.0
 Summary: Write the execution result of the case to the log
 License: Apache-2.0
 Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
 Requires-Python: >=3.10
 Requires-Dist: pytest>=7.2.0
 Project-URL: Homepage, https://github.com/dongfangtianyu/pytest_result_log
 Description-Content-Type: text/markdown
```

