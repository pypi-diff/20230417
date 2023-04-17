# Comparing `tmp/font-CLI-0.9.7.tar.gz` & `tmp/font-CLI-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "font-CLI-0.9.7.tar", last modified: Wed Apr 12 10:52:25 2023, max compression
+gzip compressed data, was "font-CLI-0.9.8.tar", last modified: Mon Apr 17 05:18:12 2023, max compression
```

## Comparing `font-CLI-0.9.7.tar` & `font-CLI-0.9.8.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 10:52:15.000000 font-CLI-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-12 10:52:25.212588 font-CLI-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    86796 2023-04-12 10:52:15.000000 font-CLI-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/font_CLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/ftCLI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/ftCLI/Lib/
--rw-r--r--   0 runner    (1001) docker     (123)    28621 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/Font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/VFont.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/ftCLI/Lib/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/assistant/fonts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/assistant/styles_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/converter/otf_to_ttf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/converter/ttf_to_otf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/cui/
--rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/cui/CUI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/cui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/tables/
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/OS_2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/head.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/click_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/glyphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_cff.py
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_os2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_print.py
--rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/ftCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:52:25.212588 font-CLI-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-12 10:52:15.000000 font-CLI-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 05:17:58.000000 font-CLI-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-17 05:18:12.533495 font-CLI-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    86796 2023-04-17 05:17:58.000000 font-CLI-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/font_CLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    28606 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/Font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/VFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/assistant/fonts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/assistant/styles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/otf_to_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/sfnt_to_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/ttf_to_otf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/variable_to_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/web_to_sfnt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/cui/
+-rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/cui/CUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/cui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/ftCLI/Lib/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/OS_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/ftCLI/Lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/click_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/glyphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/ftCLI/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_cff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_os2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/ftCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:18:12.533495 font-CLI-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-17 05:17:58.000000 font-CLI-0.9.8/setup.py
```

### Comparing `font-CLI-0.9.7/LICENSE` & `font-CLI-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/PKG-INFO` & `font-CLI-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-CLI
-Version: 0.9.7
+Version: 0.9.8
 Summary: A set of command line tools to edit fonts with FontTools
 Home-page: https://github.com/ftCLI/ftCLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.11
```

### Comparing `font-CLI-0.9.7/README.md` & `font-CLI-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/font_CLI.egg-info/PKG-INFO` & `font-CLI-0.9.8/font_CLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-CLI
-Version: 0.9.7
+Version: 0.9.8
 Summary: A set of command line tools to edit fonts with FontTools
 Home-page: https://github.com/ftCLI/ftCLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.11
```

### Comparing `font-CLI-0.9.7/font_CLI.egg-info/SOURCES.txt` & `font-CLI-0.9.8/font_CLI.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 ftCLI/Lib/Font.py
 ftCLI/Lib/VFont.py
 ftCLI/Lib/__init__.py
 ftCLI/Lib/constants.py
 ftCLI/Lib/assistant/__init__.py
 ftCLI/Lib/assistant/fonts_data.py
 ftCLI/Lib/assistant/styles_mapping.py
-ftCLI/Lib/converter/__init__.py
-ftCLI/Lib/converter/otf_to_ttf.py
-ftCLI/Lib/converter/ttf_to_otf.py
+ftCLI/Lib/converters/__init__.py
+ftCLI/Lib/converters/otf_to_ttf.py
+ftCLI/Lib/converters/sfnt_to_web.py
+ftCLI/Lib/converters/ttf_to_otf.py
+ftCLI/Lib/converters/variable_to_static.py
+ftCLI/Lib/converters/web_to_sfnt.py
 ftCLI/Lib/cui/CUI.py
 ftCLI/Lib/cui/__init__.py
 ftCLI/Lib/tables/OS_2.py
 ftCLI/Lib/tables/__init__.py
 ftCLI/Lib/tables/head.py
 ftCLI/Lib/tables/hhea.py
 ftCLI/Lib/tables/name.py
```

### Comparing `font-CLI-0.9.7/ftCLI/Lib/Font.py` & `font-CLI-0.9.8/ftCLI/Lib/Font.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,20 +655,20 @@
 
     def get_ui_name_ids(self) -> list:
         """
         Returns a list of all the UI name IDs in the font's GSUB table
 
         :return: A list of integers.
         """
-        ui_name_ids = []
-        if "GSUB" not in self.keys():
+        if "GSUB" not in self:
             return []
         else:
+            ui_name_ids = []
             for record in self["GSUB"].table.FeatureList.FeatureRecord:
-                if record.Feature.FeatureParams is not None:
+                if record.Feature.FeatureParams:
                     ui_name_ids.append(record.Feature.FeatureParams.UINameID)
         return sorted(set(ui_name_ids))
 
     def reorder_ui_name_ids(self):
         """
         Takes the IDs of the UI names in the name table and reorders them to start at 256
         """
```

### Comparing `font-CLI-0.9.7/ftCLI/Lib/VFont.py` & `font-CLI-0.9.8/ftCLI/Lib/VFont.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                     name_ids_to_delete.append(axis.ValueNameID)
 
         name_ids_to_delete = [n for n in name_ids_to_delete if n > 24]
         name_ids_to_delete = sorted(list(set(name_ids_to_delete)))
 
         return name_ids_to_delete
 
-    def get_static_instance_file_name(self, instance: NamedInstance) -> str:
+    def get_instance_file_name(self, instance: NamedInstance) -> str:
         if hasattr(instance, "postscriptNameID") and instance.postscriptNameID < 65535:
             instance_file_name = self.name_table.getDebugName(instance.postscriptNameID)
 
         else:
             if hasattr(instance, "subfamilyNameID") and instance.subfamilyNameID > 0:
                 subfamily_name = self.name_table.getDebugName(instance.subfamilyNameID)
             else:
```

### Comparing `font-CLI-0.9.7/ftCLI/Lib/assistant/fonts_data.py` & `font-CLI-0.9.8/ftCLI/Lib/assistant/fonts_data.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/assistant/styles_mapping.py` & `font-CLI-0.9.8/ftCLI/Lib/assistant/styles_mapping.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/constants.py` & `font-CLI-0.9.8/ftCLI/Lib/constants.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/converter/otf_to_ttf.py` & `font-CLI-0.9.8/ftCLI/Lib/converters/otf_to_ttf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,80 @@
-import logging
-
-from fontTools import configLogger
 from fontTools.pens.cu2quPen import Cu2QuPen
 from fontTools.pens.ttGlyphPen import TTGlyphPen
 from fontTools.ttLib import TTLibError, newTable
 
 from ftCLI.Lib.Font import Font
+from ftCLI.Lib.utils.click_tools import generic_warning_message
 
-log = logging.getLogger()
-configLogger(logger=log)
-
-# default approximation error, measured in UPEM
-MAX_ERR = 1.0
-
-# default 'post' table format
-POST_FORMAT = 2.0
 
-# assuming the input contours' direction is correctly set (counter-clockwise),
-# we just flip it to clockwise
-REVERSE_DIRECTION = True
-
-
-def glyphs_to_quadratic(glyphs, max_err=MAX_ERR, reverse_direction=REVERSE_DIRECTION):
-    quadGlyphs = {}
-    for gname in glyphs.keys():
-        glyph = glyphs[gname]
-        ttPen = TTGlyphPen(glyphs)
-        cu2quPen = Cu2QuPen(ttPen, max_err, reverse_direction=reverse_direction)
-        glyph.draw(cu2quPen)
-        quadGlyphs[gname] = ttPen.glyph()
-    return quadGlyphs
-
-
-def update_hmtx(ttFont, glyf):
-    hmtx = ttFont["hmtx"]
-    for glyphName, glyph in glyf.glyphs.items():
-        if hasattr(glyph, "xMin"):
-            hmtx[glyphName] = (hmtx[glyphName][0], glyph.xMin)
-
-
-def convert_font(ttFont: Font, post_format=POST_FORMAT, **kwargs):
-    if ttFont.sfntVersion != "OTTO":
-        raise TTLibError("Not a OpenType font (bad sfntVersion)")
-    assert "CFF " in ttFont
-
-    glyphOrder = ttFont.getGlyphOrder()
-
-    ttFont["loca"] = newTable("loca")
-    ttFont["glyf"] = glyf = newTable("glyf")
-    glyf.glyphOrder = glyphOrder
-    glyf.glyphs = glyphs_to_quadratic(ttFont.getGlyphSet(), **kwargs)
-    del ttFont["CFF "]
-    if "VORG" in ttFont:
-        del ttFont["VORG"]
-    glyf.compile(ttFont)
-    update_hmtx(ttFont, glyf)
-
-    ttFont["maxp"] = maxp = newTable("maxp")
-    maxp.tableVersion = 0x00010000
-    maxp.maxZones = 1
-    maxp.maxTwilightPoints = 0
-    maxp.maxStorage = 0
-    maxp.maxFunctionDefs = 0
-    maxp.maxInstructionDefs = 0
-    maxp.maxStackElements = 0
-    maxp.maxSizeOfInstructions = 0
-    maxp.maxComponentElements = max(len(g.components if hasattr(g, "components") else []) for g in glyf.glyphs.values())
-    maxp.compile(ttFont)
-
-    post = ttFont["post"]
-    post.formatType = post_format
-    post.extraNames = []
-    post.mapping = {}
-    post.glyphOrder = glyphOrder
-    try:
-        post.compile(ttFont)
-    except OverflowError:
-        post.formatType = 3
-        log.warning("Dropping glyph names, they do not fit in 'post' table.")
-
-    ttFont.sfntVersion = "\000\001\000\000"
-
-
-def run(input_file, output_file, recalc_timestamp=False):
-    font = Font(input_file, recalcTimestamp=recalc_timestamp)
-    convert_font(font, post_format=2.0, max_err=1.0, reverse_direction=True)
-    font.save(output_file)
+class Options(object):
+    def __init__(self):
+        self.max_err = 1.0
+        self.reverse_direction = True
+        self.post_format = 2.0
+
+
+class CFFToTrueType(object):
+    def __init__(self, font: Font):
+        self.font = font
+        self.options = Options()
+
+    def run(self):
+        if self.font.sfntVersion != "OTTO":
+            raise TTLibError("Not a OpenType font (bad sfntVersion)")
+        assert "CFF " in self.font
+
+        glyphOrder = self.font.getGlyphOrder()
+
+        self.font["loca"] = newTable("loca")
+        self.font["glyf"] = glyf = newTable("glyf")
+        glyf.glyphOrder = glyphOrder
+        glyf.glyphs = self.glyphs_to_quadratic(glyphs=self.font.getGlyphSet())
+        del self.font["CFF "]
+        if "VORG" in self.font:
+            del self.font["VORG"]
+        glyf.compile(self.font)
+        self.update_hmtx(glyf)
+
+        self.font["maxp"] = maxp = newTable("maxp")
+        maxp.tableVersion = 0x00010000
+        maxp.maxZones = 1
+        maxp.maxTwilightPoints = 0
+        maxp.maxStorage = 0
+        maxp.maxFunctionDefs = 0
+        maxp.maxInstructionDefs = 0
+        maxp.maxStackElements = 0
+        maxp.maxSizeOfInstructions = 0
+        maxp.maxComponentElements = max(
+            len(g.components if hasattr(g, "components") else []) for g in glyf.glyphs.values()
+        )
+        maxp.compile(self.font)
+
+        post = self.font["post"]
+        post.formatType = self.options.post_format
+        post.extraNames = []
+        post.mapping = {}
+        post.glyphOrder = glyphOrder
+        try:
+            post.compile(self.font)
+        except OverflowError:
+            post.formatType = 3
+            generic_warning_message("Dropping glyph names, they do not fit in 'post' table.")
+
+        self.font.sfntVersion = "\000\001\000\000"
+        return self.font
+
+    def update_hmtx(self, glyf):
+        hmtx = self.font["hmtx"]
+        for glyphName, glyph in glyf.glyphs.items():
+            if hasattr(glyph, "xMin"):
+                hmtx[glyphName] = (hmtx[glyphName][0], glyph.xMin)
+
+    def glyphs_to_quadratic(self, glyphs):
+        quadGlyphs = {}
+        for gname in glyphs.keys():
+            glyph = glyphs[gname]
+            ttPen = TTGlyphPen(glyphs)
+            cu2quPen = Cu2QuPen(ttPen, max_err=self.options.max_err, reverse_direction=self.options.reverse_direction)
+            glyph.draw(cu2quPen)
+            quadGlyphs[gname] = ttPen.glyph()
+        return quadGlyphs
```

### Comparing `font-CLI-0.9.7/ftCLI/Lib/converter/ttf_to_otf.py` & `font-CLI-0.9.8/ftCLI/Lib/converters/ttf_to_otf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,46 @@
 from fontTools.pens.t2CharStringPen import T2CharStringPen
 from fontTools.subset import Subsetter
 
 from ftCLI.Lib.Font import Font
 from ftCLI.Lib.utils.click_tools import generic_error_message, generic_warning_message
 
 
+class Options(object):
+    def __init__(self):
+        self.tolerance: float = 1.0
+        self.charstring_source = "qu2cu"
+        self.purge_glyphs = True
+        self.subroutinize = True
+
+
 class TrueTypeToCFF(object):
-    def __init__(self, font: Font, output_file):
+    def __init__(self, font: Font):
         self.font = font
-        self.output_file = output_file
+        self.options = Options()
 
-    def run(
-        self,
-        charstrings_source="qu2cu",
-        tolerance=1,
-        purge_glyphs=True,
-        subroutinize=True,
-    ):
-        if purge_glyphs:
+    def run(self):
+        if self.options.purge_glyphs:
             self.purge_glyphs()
 
         charstrings = {}
 
-        if charstrings_source == "qu2cu":
+        if self.options.charstring_source == "qu2cu":
             self.font.decomponentize()
             try:
-                charstrings = self.get_qu2cu_charstrings(tolerance=tolerance, all_cubic=True)
+                charstrings = self.get_qu2cu_charstrings(tolerance=self.options.tolerance, all_cubic=True)
             except NotImplementedError:
                 generic_warning_message("all_cubic set to False")
                 try:
-                    charstrings = self.get_qu2cu_charstrings(tolerance=tolerance, all_cubic=False)
+                    charstrings = self.get_qu2cu_charstrings(tolerance=self.options.tolerance, all_cubic=False)
                 except Exception as e:
                     generic_error_message(f"Failed to get charstring with Qu2CuPen ({e})")
                     return
 
-        if charstrings_source == "t2":
+        if self.options.charstring_source == "t2":
             try:
                 charstrings = self.get_t2_charstrings()
             except Exception as e:
                 generic_error_message(f"Failed to get charstrings with T2CharStringPen ({e})")
                 return
 
         cff_font_info = self.get_cff_font_info()
@@ -60,23 +62,23 @@
             fontInfo=cff_font_info,
             privateDict={},
         )
         fb.setupDummyDSIG()
         fb.setupMaxp()
         fb.setupPost(**post_values)
 
-        if subroutinize:
+        if self.options.subroutinize:
             # cffsubr doesn't work with woff/woff2 fonts
             flavor = fb.font.flavor
             if flavor is not None:
                 fb.font.flavor = None
             cffsubr.subroutinize(fb.font)
             fb.font.flavor = flavor
 
-        fb.save(self.output_file)
+        return fb.font
 
     def get_cff_font_info(self) -> dict:
         """
         Setup CFF topDict
 
         :return: A dictionary of the font info.
         """
```

### Comparing `font-CLI-0.9.7/ftCLI/Lib/cui/CUI.py` & `font-CLI-0.9.8/ftCLI/Lib/cui/CUI.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/tables/OS_2.py` & `font-CLI-0.9.8/ftCLI/Lib/tables/OS_2.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/tables/head.py` & `font-CLI-0.9.8/ftCLI/Lib/tables/head.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/tables/hhea.py` & `font-CLI-0.9.8/ftCLI/Lib/tables/hhea.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/tables/name.py` & `font-CLI-0.9.8/ftCLI/Lib/tables/name.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/utils/cli_tools.py` & `font-CLI-0.9.8/ftCLI/Lib/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/utils/click_tools.py` & `font-CLI-0.9.8/ftCLI/Lib/utils/click_tools.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/utils/glyphs.py` & `font-CLI-0.9.8/ftCLI/Lib/utils/glyphs.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/Lib/utils/misc.py` & `font-CLI-0.9.8/ftCLI/Lib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_assistant.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_assistant.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_cff.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_cff.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_converter.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 import os
 import time
-from io import BytesIO
 
 import click
 import fontTools.ttLib
-from afdko import checkoutlinesufo
 from fontTools.misc.cliTools import makeOutputFileName
-from fontTools.ttLib import TTCollection
-from fontTools.ttLib.tables._f_v_a_r import NamedInstance
-from fontTools.varLib.instancer import instantiateVariableFont, OverlapMode
-from pathvalidate import sanitize_filename
 
 from ftCLI.Lib.Font import Font
-from ftCLI.Lib.converter import otf_to_ttf
-from ftCLI.Lib.converter.ttf_to_otf import TrueTypeToCFF
 from ftCLI.Lib.utils.cli_tools import check_output_dir, check_input_path
 from ftCLI.Lib.utils.click_tools import (
     add_file_or_path_argument,
     add_common_options,
     generic_error_message,
-    generic_warning_message,
     generic_info_message,
     file_saved_message,
     select_instance_coordinates,
 )
 
 
 @click.group()
@@ -76,28 +67,30 @@
     is_flag=True,
     help="""
               Performs optional outline quality checks and removes overlaps with afdko.checkoutlinesufo
               """,
 )
 @add_common_options()
 def ttf2otf(
-    input_path,
-    tolerance=1,
-    safe=False,
-    purge_glyphs=False,
-    subroutinize=True,
-    check_outlines=False,
-    outputDir=None,
-    recalcTimestamp=False,
-    overWrite=True,
+        input_path,
+        tolerance=1,
+        safe=False,
+        purge_glyphs=False,
+        subroutinize=True,
+        check_outlines=False,
+        outputDir=None,
+        recalcTimestamp=False,
+        overWrite=True,
 ):
     """
     Converts TTF fonts (or TrueType flavored woff/woff2 web fonts) to OTF fonts (or CFF flavored woff/woff2 web fonts).
     """
 
+    from ftCLI.Lib.converters.ttf_to_otf import TrueTypeToCFF
+
     files = check_input_path(input_path, allow_variable=False, allow_cff=False)
     output_dir = check_output_dir(input_path=input_path, output_path=outputDir)
 
     start_time = time.time()
     converted_files_counter = 0
     counter = 0
 
@@ -118,38 +111,46 @@
             suffix = "" if source_font.flavor is None else ".otf"
             output_file = makeOutputFileName(
                 file, suffix=suffix, extension=ext, outputDir=output_dir, overWrite=overWrite
             )
 
             if safe:
                 # Create a temporary OTF file with T2CharStringPen...
-                buf = BytesIO()
-                ttf2otf_converter_temp = TrueTypeToCFF(source_font, output_file=buf)
-                ttf2otf_converter_temp.run(charstrings_source="t2", purge_glyphs=purge_glyphs, subroutinize=False)
+                from ftCLI.Lib.converters.otf_to_ttf import CFFToTrueType
+                ttf2otf_converter_temp = TrueTypeToCFF(source_font)
+                ttf2otf_converter_temp.options.charstring_source = "t2"
+                ttf2otf_converter_temp.options.subroutinize = False
+                ttf2otf_converter_temp.options.purge_glyphs = purge_glyphs
+                temp_cff_font = ttf2otf_converter_temp.run()
 
                 # ... and convert it back to a temporary TTF file that will be used for conversion
-                data = buf.getvalue()
-                temp_otf = Font(BytesIO(data), recalcTimestamp=recalcTimestamp)
-                otf_to_ttf.convert_font(temp_otf, post_format=2.0, max_err=1.0, reverse_direction=True)
-                input_font = Font(BytesIO(buf.getvalue()), recalcTimestamp=recalcTimestamp)
+                otf_to_ttf_converter = CFFToTrueType(temp_cff_font)
+                # since the temp CFF font has many more points than needed, increase max_err from 1.0 to 2.0
+                otf_to_ttf_converter.options.max_err = 2.0
+                input_font = otf_to_ttf_converter.run()
+
             else:
                 input_font = source_font
 
-            ttf2otf_converter = TrueTypeToCFF(font=input_font, output_file=output_file)
-            ttf2otf_converter.run(
-                charstrings_source="qu2cu", tolerance=tolerance, subroutinize=subroutinize, purge_glyphs=purge_glyphs
-            )
+            ttf2otf_converter = TrueTypeToCFF(font=input_font)
+            ttf2otf_converter.options.charstring_source = "qu2cu"
+            ttf2otf_converter.options.tolerance = tolerance
+            ttf2otf_converter.options.subroutinize = subroutinize
+            ttf2otf_converter.options.purge_glyphs = purge_glyphs
+            cff_font = ttf2otf_converter.run()
+            cff_font.save(output_file)
 
             if check_outlines:
+                from afdko import checkoutlinesufo
                 generic_info_message("Checking outlines...")
                 checkoutlinesufo.run(args=[output_file, "--error-correction-mode", "--quiet-mode"])
 
             converted_files_counter += 1
             generic_info_message(f"Done in {round(time.time() - t, 3)} seconds")
-            file_saved_message(ttf2otf_converter.output_file)
+            file_saved_message(output_file)
 
         except Exception as e:
             generic_error_message(e)
 
     print()
     generic_info_message(f"Total files       : {len(files)}")
     generic_info_message(f"Converted files   : {converted_files_counter}")
@@ -159,39 +160,49 @@
 @click.group()
 def otf_2_ttf():
     pass
 
 
 @otf_2_ttf.command()
 @add_file_or_path_argument()
+@click.option(
+    "--max-err",
+    type=click.FloatRange(0.0, 3.0),
+    default=1.0,
+    help="""Approximation error, measured in UPEM"""
+)
 @add_common_options()
-def otf2ttf(input_path, outputDir=None, recalcTimestamp=False, overWrite=True):
+def otf2ttf(input_path, max_err, outputDir=None, recalcTimestamp=False, overWrite=True):
     """
     Converts fonts from OTF to TTF format.
     """
+    from ftCLI.Lib.converters.otf_to_ttf import CFFToTrueType
 
     files = check_input_path(input_path, allow_variable=False, allow_ttf=False)
     output_dir = check_output_dir(input_path=input_path, output_path=outputDir)
 
     start_time = time.time()
     counter = 0
     converted_files = 0
 
     for file in files:
         t = time.time()
         counter += 1
         generic_info_message(f"Converting file {counter} of {len(files)}")
         try:
+            font = Font(file, recalcTimestamp=recalcTimestamp)
+
+            converter = CFFToTrueType(font=font)
+            converter.options.max_err = max_err
+            ttf_font = converter.run()
+
             output_file = makeOutputFileName(file, outputDir=output_dir, overWrite=overWrite, extension=".ttf")
-            otf_to_ttf.run(
-                input_file=file,
-                output_file=output_file,
-                recalc_timestamp=recalcTimestamp,
-            )
+            ttf_font.save(output_file)
             converted_files += 1
+
             generic_info_message(f"Done in {round(time.time() - t, 3)}")
             file_saved_message(output_file)
         except Exception as e:
             generic_error_message(e)
 
     print()
     generic_info_message(f"Total files       : {len(files)}")
@@ -221,50 +232,54 @@
     is_flag=True,
     help="""
               Deletes the source files after conversion.
               """,
 )
 @add_common_options()
 def wf2ft(
-    input_path,
-    flavor=None,
-    delete_source_file=False,
-    outputDir=None,
-    recalcTimestamp=False,
-    overWrite=True,
+        input_path,
+        flavor=None,
+        delete_source_file=False,
+        outputDir=None,
+        recalcTimestamp=False,
+        overWrite=True,
 ):
     """
     Converts web fonts (WOFF and WOFF2) to SFNT fonts (TTF or OTF)
     """
+    from ftCLI.Lib.converters.web_to_sfnt import WebToSFNT
+
+    if not flavor:
+        allowed_extensions = [".woff", ".woff2"]
+    else:
+        allowed_extensions = [f".{flavor}"]
 
-    files = check_input_path(input_path, allow_extensions=[".woff", ".woff2"])
+    files = check_input_path(input_path, allow_extensions=allowed_extensions)
     output_dir = check_output_dir(input_path=input_path, output_path=outputDir)
 
     for file in files:
         try:
             web_font = Font(file, recalcTimestamp=recalcTimestamp)
-            if web_font.flavor is None:
-                continue
-            if flavor is not None:
-                if web_font.flavor != flavor:
-                    continue
-            old_extension=web_font.get_real_extension()
-            web_font.flavor = None
-            new_extension = web_font.get_real_extension()
-            desktop_font_file = makeOutputFileName(
+            suffix = web_font.get_real_extension()
+
+            converter = WebToSFNT(font=web_font)
+            desktop_font = converter.run()
+
+            new_extension = desktop_font.get_real_extension()
+            output_file = makeOutputFileName(
                 file,
                 extension=new_extension,
-                suffix=old_extension,
+                suffix=suffix,
                 outputDir=output_dir,
                 overWrite=overWrite
             )
-            web_font.save(desktop_font_file, reorderTables=False)
+            desktop_font.save(output_file, reorderTables=False)
             if delete_source_file:
                 os.remove(file)
-            file_saved_message(desktop_font_file)
+            file_saved_message(output_file)
         except Exception as e:
             generic_error_message(e)
 
 
 @click.group()
 def sfnt_to_web():
     pass
@@ -282,14 +297,15 @@
               """,
 )
 @add_common_options()
 def ft2wf(input_path, flavor=None, outputDir=None, recalcTimestamp=False, overWrite=True):
     """
     Converts SFNT fonts (TTF or OTF) to web fonts (WOFF and/or WOFF2)
     """
+    from ftCLI.Lib.converters.sfnt_to_web import SFNTToWeb
 
     files = check_input_path(input_path, allow_extensions=[".otf", ".ttf"])
     output_dir = check_output_dir(input_path=input_path, output_path=outputDir)
 
     output_flavors = ["woff", "woff2"]
     if flavor is not None:
         output_flavors = [flavor]
@@ -297,18 +313,20 @@
     for file in files:
         try:
             font = Font(file, recalcTimestamp=recalcTimestamp)
             if font.flavor is not None:
                 continue
             for flavor in output_flavors:
                 font.flavor = flavor
-                extension = font.get_real_extension()
-                web_font_file = makeOutputFileName(file, extension=extension, outputDir=output_dir, overWrite=overWrite)
-                font.save(web_font_file, reorderTables=False)
-                file_saved_message(web_font_file)
+                converter = SFNTToWeb(font=font, flavor=flavor)
+                web_font = converter.run()
+                extension = web_font.get_real_extension()
+                output_file = makeOutputFileName(file, extension=extension, outputDir=output_dir, overWrite=overWrite)
+                web_font.save(output_file, reorderTables=False)
+                file_saved_message(output_file)
         except Exception as e:
             generic_error_message(e)
 
 
 @click.group()
 def ttc_to_sfnt():
     pass
@@ -317,14 +335,15 @@
 @ttc_to_sfnt.command()
 @add_file_or_path_argument()
 @add_common_options()
 def ttc2sfnt(input_path, outputDir=None, recalcTimestamp=False, overWrite=True):
     """
     Extracts each font from a TTC file, and saves it as a TTF or OTF file.
     """
+    from fontTools.ttLib import TTCollection
 
     if os.path.isfile(input_path):
         files = [input_path]
     elif os.path.isdir(input_path):
         files = [os.path.join(input_path, file) for file in os.listdir(input_path)]
     else:
         generic_error_message(f"Invalid path: {input_path}")
@@ -396,124 +415,76 @@
     default=False,
     help="""
               Update the instantiated font's `name` table. Input font must have a STAT table with Axis Value Tables
               """,
 )
 @add_common_options()
 def var2static(
-    input_path,
-    select_instance=False,
-    cleanup=True,
-    update_name_table=False,
-    outputDir=None,
-    recalcTimestamp=False,
-    overWrite=True,
+        input_path,
+        select_instance=False,
+        cleanup=True,
+        update_name_table=False,
+        outputDir=None,
+        recalcTimestamp=False,
+        overWrite=True,
 ):
     """
     Exports static instances from variable fonts.
     """
 
     from ftCLI.Lib.VFont import VariableFont
+    from ftCLI.Lib.converters.variable_to_static import VariableToStatic
+    from fontTools.ttLib.tables._f_v_a_r import NamedInstance
 
     files = check_input_path(input_path, allow_static=False, allow_cff=False)
     output_dir = check_output_dir(input_path=input_path, output_path=outputDir)
 
     start_time = time.time()
     for file in files:
         print()
         generic_info_message(f"Converting file {os.path.basename(file)}")
         try:
             variable_font = VariableFont(file, recalcTimestamp=recalcTimestamp)
-            axes = variable_font.get_axes()
-            instances = variable_font.get_instances()
 
-            update_this_font_name_table = update_name_table
+            converter = VariableToStatic()
+            converter.options.cleanup = cleanup
+            converter.options.update_name_table = update_name_table
+            converter.options.output_dir = output_dir
+            converter.options.overwrite = overWrite
 
+            instances = variable_font.get_instances()
             if select_instance:
+                axes = variable_font.get_axes()
                 selected_coordinates = select_instance_coordinates(axes)
                 is_named_instance = selected_coordinates in [i.coordinates for i in instances]
                 if not is_named_instance:
                     # Set update_name_table value to False because we won't find this Axis Value in the STAT table.
-                    update_this_font_name_table = False
+                    converter.options.update_name_table = False
                     selected_instance = NamedInstance()
                     selected_instance.coordinates = selected_coordinates
                 else:
                     # In case there are several instances with the same coordinates, return only the first one.
                     #
                     # From https://learn.microsoft.com/en-us/typography/opentype/spec/fvar#instancerecord:
                     #
                     # All the instance records in a font should have distinct coordinates and distinct
                     # subfamilyNameID and postScriptName ID values. If two or more records share the same coordinates,
                     # the same nameID values or the same postScriptNameID values, then all but the first can be ignored.
                     selected_instance = [i for i in instances if i.coordinates == selected_coordinates][0]
 
                 instances = [selected_instance]
 
-            if len(instances) == 0:
-                generic_error_message("No instances found")
-                return
-
-            name_ids_to_delete = []
-            if cleanup:
-                name_ids_to_delete = variable_font.get_var_name_ids_to_delete()
-
-            instance_count = 0
-
-            # Cannot update name table if there is no STAT table.
-            if "STAT" not in variable_font:
-                update_this_font_name_table = False
-                generic_warning_message("Cannot update name table if there is no STAT table.")
-
-            # Cannot update name table if there are no STAT Axis Values.
-            if update_this_font_name_table:
-                if not hasattr(variable_font["STAT"], "AxisValueArray"):
-                    update_this_font_name_table = False
-                    generic_warning_message("Cannot update name table if there are no STAT Axis Values.")
-
-            for instance in instances:
-                t = time.time()
-                instance_count += 1
-
-                print()
-                generic_info_message(f"Exporting instance {instance_count} of {len(instances)}")
-                static_font: Font = instantiateVariableFont(
-                    varfont=variable_font,
-                    axisLimits=instance.coordinates,
-                    inplace=False,
-                    optimize=True,
-                    overlap=OverlapMode.REMOVE_AND_IGNORE_ERRORS,
-                    updateFontNames=update_this_font_name_table,
-                )
-
-                if cleanup:
-                    static_font.name_table.del_names(name_ids=name_ids_to_delete)
-                    if "STAT" in static_font:
-                        del static_font["STAT"]
-                    static_font.reorder_ui_name_ids()
-
-                static_font_file_name = sanitize_filename(variable_font.get_static_instance_file_name(instance))
-                static_font_ext = static_font.get_real_extension()
-                output_file = makeOutputFileName(
-                    static_font_file_name,
-                    outputDir=output_dir,
-                    extension=static_font_ext,
-                    overWrite=overWrite,
-                )
-
-                static_font.save(output_file)
-                generic_info_message(f"Done in {round(time.time() - t, 3)} seconds")
-                file_saved_message(output_file)
-
-            print()
-            generic_info_message(f"Total instances : {len(instances)}")
-            generic_info_message(f"Elapsed time    : {round(time.time() - start_time)} seconds")
+            converter.run(variable_font=variable_font, instances=instances)
 
         except Exception as e:
             generic_error_message(e)
 
+        generic_info_message(f"Total files : {len(files)}")
+        generic_info_message(f"Elapsed time    : {round(time.time() - start_time)} seconds")
+
 
 cli = click.CommandCollection(
     sources=[
         otf_2_ttf,
         ttf_to_otf,
         web_to_sfnt,
         sfnt_to_web,
```

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_fix.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_fix.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_hhea.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_hhea.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_metrics.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_metrics.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_name.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_name.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_os2.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_os2.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_post.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_post.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_print.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_print.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/commands/ftcli_utils.py` & `font-CLI-0.9.8/ftCLI/commands/ftcli_utils.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/ftCLI/ftCLI.py` & `font-CLI-0.9.8/ftCLI/ftCLI.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.7/setup.py` & `font-CLI-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="font-CLI",
-    version="0.9.7",
+    version="0.9.8",
     description="A set of command line tools to edit fonts with FontTools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ftCLI",
     author_email="ftcli@proton.me",
     url="https://github.com/ftCLI/ftCLI",
     packages=setuptools.find_packages(),
```

