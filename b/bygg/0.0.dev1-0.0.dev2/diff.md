# Comparing `tmp/bygg-0.0.dev1.tar.gz` & `tmp/bygg-0.0.dev2.tar.gz`

## Comparing `bygg-0.0.dev1.tar` & `bygg-0.0.dev2.tar`

### file list

```diff
@@ -1,5 +1,41 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev1/src/bygg/__init__.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.0.dev1/LICENSE
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bygg-0.0.dev1/README.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bygg-0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 bygg-0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bygg-0.0.dev2/.tool-versions
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bygg-0.0.dev2/Byggfile.yml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 bygg-0.0.dev2/_version.py
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 bygg-0.0.dev2/bootstrap.sh
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 bygg-0.0.dev2/mypy.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bygg-0.0.dev2/noxfile.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bygg-0.0.dev2/requirements-dev.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 bygg-0.0.dev2/requirements.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/.gitignore
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/Byggfile.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/Byggfile.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/README.md
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/taskrunner/Byggfile.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/Byggfile.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/Byggfile.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/input1.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/more_things/MoreActions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/more_things/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/__init__.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/action.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/cache.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/configuration.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/dag.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/digest.py
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/py.typed
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/runner.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/scaffolding.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/scheduler.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/status_display.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/types.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/util.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_action.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_cache.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_scheduler.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_utils.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bygg-0.0.dev2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.0.dev2/LICENSE
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 bygg-0.0.dev2/README.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 bygg-0.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 bygg-0.0.dev2/PKG-INFO
```

### Comparing `bygg-0.0.dev1/LICENSE` & `bygg-0.0.dev2/LICENSE`

 * *Files identical despite different names*

