# Comparing `tmp/yeagerai-agent-0.0.40.tar.gz` & `tmp/yeagerai-agent-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeagerai-agent-0.0.40.tar", last modified: Mon Apr 17 03:51:04 2023, max compression
+gzip compressed data, was "yeagerai-agent-0.0.41.tar", last modified: Mon Apr 17 03:53:32 2023, max compression
```

## Comparing `yeagerai-agent-0.0.40.tar` & `yeagerai-agent-0.0.41.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/LICENSE
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3083 2023-04-16 23:42:11.000000 yeagerai-agent-0.0.40/README.md
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/setup.cfg
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1207 2023-04-17 03:45:48.000000 yeagerai-agent-0.0.40/setup.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/agent/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/agent/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1270 2023-04-16 23:42:12.000000 yeagerai-agent-0.0.40/yeagerai/agent/master_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-16 23:42:12.000000 yeagerai-agent-0.0.40/yeagerai/agent/output_parser.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/agent/prompt_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2815 2023-04-17 03:32:24.000000 yeagerai-agent-0.0.40/yeagerai/agent/yeagerai_agent.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/interfaces/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/interfaces/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/interfaces/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/interfaces/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/interfaces/callbacks/local_file_system_n_git.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5719 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/interfaces/cli.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     8533 2023-04-17 03:45:58.000000 yeagerai-agent-0.0.40/yeagerai/interfaces/gradio_chat.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/memory/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/memory/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/memory/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/memory/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/memory/callbacks/session_memory_handler.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-16 23:42:12.000000 yeagerai-agent-0.0.40/yeagerai/memory/yeagerai_context.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/toolkit/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      670 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_mocked_tests/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_mocked_tests/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4065 2023-04-17 03:22:11.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5114 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_source/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_source/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2574 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4855 2023-04-17 03:22:32.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_source/create_tool_source.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/toolkit/design_solution_sketch/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/design_solution_sketch/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2781 2023-04-17 03:21:49.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3508 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai/toolkit/load_n_fix_new_tool/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/load_n_fix_new_tool/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5728 2023-04-17 03:23:06.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3221 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/yeagerai_tool.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      617 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.40/yeagerai/toolkit/yeagerai_toolkit.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:51:04.050529 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-17 03:51:04.000000 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1644 2023-04-17 03:51:04.000000 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-17 03:51:04.000000 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       72 2023-04-17 03:51:04.000000 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/entry_points.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-17 03:51:04.000000 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/requires.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-17 03:51:04.000000 yeagerai-agent-0.0.40/yeagerai_agent.egg-info/top_level.txt
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.552174 yeagerai-agent-0.0.41/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/LICENSE
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-17 03:53:32.552174 yeagerai-agent-0.0.41/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3083 2023-04-16 23:42:11.000000 yeagerai-agent-0.0.41/README.md
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-17 03:53:32.552174 yeagerai-agent-0.0.41/setup.cfg
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1225 2023-04-17 03:52:52.000000 yeagerai-agent-0.0.41/setup.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/agent/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/agent/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1270 2023-04-16 23:42:12.000000 yeagerai-agent-0.0.41/yeagerai/agent/master_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-16 23:42:12.000000 yeagerai-agent-0.0.41/yeagerai/agent/output_parser.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/agent/prompt_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2815 2023-04-17 03:32:24.000000 yeagerai-agent-0.0.41/yeagerai/agent/yeagerai_agent.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/interfaces/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/interfaces/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/interfaces/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/interfaces/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/interfaces/callbacks/local_file_system_n_git.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5719 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/interfaces/cli.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     8533 2023-04-17 03:45:58.000000 yeagerai-agent-0.0.41/yeagerai/interfaces/gradio_chat.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/memory/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/memory/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/memory/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/memory/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/memory/callbacks/session_memory_handler.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-16 23:42:12.000000 yeagerai-agent-0.0.41/yeagerai/memory/yeagerai_context.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/toolkit/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      670 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_mocked_tests/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_mocked_tests/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4065 2023-04-17 03:22:11.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5114 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_source/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_source/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2574 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4855 2023-04-17 03:22:32.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_source/create_tool_source.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/toolkit/design_solution_sketch/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/design_solution_sketch/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2781 2023-04-17 03:21:49.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3508 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.548174 yeagerai-agent-0.0.41/yeagerai/toolkit/load_n_fix_new_tool/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/load_n_fix_new_tool/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5728 2023-04-17 03:23:06.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3221 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/yeagerai_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      617 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.41/yeagerai/toolkit/yeagerai_toolkit.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-17 03:53:32.552174 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-17 03:53:32.000000 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1644 2023-04-17 03:53:32.000000 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-17 03:53:32.000000 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       72 2023-04-17 03:53:32.000000 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       54 2023-04-17 03:53:32.000000 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/requires.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-17 03:53:32.000000 yeagerai-agent-0.0.41/yeagerai_agent.egg-info/top_level.txt
```

### Comparing `yeagerai-agent-0.0.40/LICENSE` & `yeagerai-agent-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/PKG-INFO` & `yeagerai-agent-0.0.41/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.40
+Version: 0.0.41
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.40/README.md` & `yeagerai-agent-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/setup.py` & `yeagerai-agent-0.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="yeagerai-agent",
-    version="0.0.40",
+    version="0.0.41",
     description="The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.",
     author="YeagerAI LLC",
     author_email="jm@yeager.ai",
     packages=find_packages(),
     install_requires=[
         "langchain",
         "openai",
         "GitPython",
         "click",
+        "gradio",
         "python-dotenv",
     ],
     entry_points={
         "console_scripts": [
             "yeagerai-agent = yeagerai.interfaces.gradio_chat:main",
         ],
     },
```

### Comparing `yeagerai-agent-0.0.40/yeagerai/agent/master_template.py` & `yeagerai-agent-0.0.41/yeagerai/agent/master_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/agent/output_parser.py` & `yeagerai-agent-0.0.41/yeagerai/agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/agent/prompt_template.py` & `yeagerai-agent-0.0.41/yeagerai/agent/prompt_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/agent/yeagerai_agent.py` & `yeagerai-agent-0.0.41/yeagerai/agent/yeagerai_agent.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/interfaces/callbacks/local_file_system_n_git.py` & `yeagerai-agent-0.0.41/yeagerai/interfaces/callbacks/local_file_system_n_git.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/interfaces/cli.py` & `yeagerai-agent-0.0.41/yeagerai/interfaces/cli.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/interfaces/gradio_chat.py` & `yeagerai-agent-0.0.41/yeagerai/interfaces/gradio_chat.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/memory/callbacks/session_memory_handler.py` & `yeagerai-agent-0.0.41/yeagerai/memory/callbacks/session_memory_handler.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/memory/yeagerai_context.py` & `yeagerai-agent-0.0.41/yeagerai/memory/yeagerai_context.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/__init__.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/create_tool_source/create_tool_source.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/create_tool_source/create_tool_source.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool_master_prompt.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai/toolkit/yeagerai_toolkit.py` & `yeagerai-agent-0.0.41/yeagerai/toolkit/yeagerai_toolkit.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.40/yeagerai_agent.egg-info/PKG-INFO` & `yeagerai-agent-0.0.41/yeagerai_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.40
+Version: 0.0.41
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.40/yeagerai_agent.egg-info/SOURCES.txt` & `yeagerai-agent-0.0.41/yeagerai_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

