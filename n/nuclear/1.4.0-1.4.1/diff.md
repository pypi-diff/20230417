# Comparing `tmp/nuclear-1.4.0.tar.gz` & `tmp/nuclear-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclear-1.4.0.tar", last modified: Thu Apr  6 12:14:09 2023, max compression
+gzip compressed data, was "nuclear-1.4.1.tar", last modified: Mon Apr 17 13:48:22 2023, max compression
```

## Comparing `nuclear-1.4.0.tar` & `nuclear-1.4.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.963242 nuclear-1.4.0/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2020-07-28 11:14:52.000000 nuclear-1.4.0/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18604 2023-04-06 12:14:09.963242 nuclear-1.4.0/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18152 2023-04-06 12:14:09.000000 nuclear-1.4.0/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      571 2023-04-06 10:36:33.000000 nuclear-1.4.0/nuclear/__init__.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/args/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/args/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1399 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/args/args_que.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      504 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/args/container.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/autocomplete/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/autocomplete/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     4445 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/autocomplete/autocomplete.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     2175 2022-04-12 16:38:36.000000 nuclear-1.4.0/nuclear/autocomplete/install.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/builder/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/builder/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     9263 2022-04-13 09:01:27.000000 nuclear-1.4.0/nuclear/builder/builder.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3752 2022-04-13 09:02:59.000000 nuclear-1.4.0/nuclear/builder/decorator_builder.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2974 2021-12-11 21:16:15.000000 nuclear-1.4.0/nuclear/builder/rule.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11321 2022-04-13 09:13:28.000000 nuclear-1.4.0/nuclear/builder/rule_factory.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      227 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/builder/typedef.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/completers/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       33 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/completers/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      739 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/completers/file.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/help/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/help/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11775 2023-03-13 13:40:47.000000 nuclear-1.4.0/nuclear/help/help.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/inspection/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-03 14:03:48.000000 nuclear-1.4.0/nuclear/inspection/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    10314 2023-04-06 12:05:54.000000 nuclear-1.4.0/nuclear/inspection/inspection.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/parser/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      442 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/context.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      449 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/error.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1843 2021-12-11 21:16:15.000000 nuclear-1.4.0/nuclear/parser/inject.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      326 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/internal_vars.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      666 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/keyword.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1378 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/matcher.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    12607 2022-05-12 13:06:55.000000 nuclear-1.4.0/nuclear/parser/parser.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      409 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/parser/transform.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3826 2021-12-11 21:16:15.000000 nuclear-1.4.0/nuclear/parser/validate.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1886 2022-05-13 09:22:45.000000 nuclear-1.4.0/nuclear/parser/value.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/shell/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      123 2022-05-16 13:47:34.000000 nuclear-1.4.0/nuclear/shell/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4734 2022-08-16 13:22:26.000000 nuclear-1.4.0/nuclear/shell/background_cmd.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     3676 2022-05-16 13:53:00.000000 nuclear-1.4.0/nuclear/shell/shell_utils.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/sublog/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      309 2022-06-08 11:51:00.000000 nuclear-1.4.0/nuclear/sublog/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3546 2022-06-08 12:00:57.000000 nuclear-1.4.0/nuclear/sublog/catch.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4039 2022-04-13 09:02:02.000000 nuclear-1.4.0/nuclear/sublog/context_logger.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      843 2022-06-08 12:04:08.000000 nuclear-1.4.0/nuclear/sublog/wrap_error.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear/types/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/types/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       94 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/types/boolean.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      358 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/types/filesystem.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1189 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/types/time.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.963242 nuclear-1.4.0/nuclear/utils/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-04-12 16:16:19.000000 nuclear-1.4.0/nuclear/utils/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      116 2022-08-24 14:04:56.000000 nuclear-1.4.0/nuclear/utils/files.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      138 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/utils/input.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1301 2022-08-24 13:59:25.000000 nuclear-1.4.0/nuclear/utils/regex.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      112 2022-04-12 16:39:09.000000 nuclear-1.4.0/nuclear/utils/shell.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      688 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/utils/strings.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      362 2020-07-28 11:14:52.000000 nuclear-1.4.0/nuclear/utils/time.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2023-04-06 12:07:16.000000 nuclear-1.4.0/nuclear/version.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-06 12:14:09.959242 nuclear-1.4.0/nuclear.egg-info/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18604 2023-04-06 12:14:09.000000 nuclear-1.4.0/nuclear.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1496 2023-04-06 12:14:09.000000 nuclear-1.4.0/nuclear.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-04-06 12:14:09.000000 nuclear-1.4.0/nuclear.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-04-06 12:14:09.000000 nuclear-1.4.0/nuclear.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        8 2023-04-06 12:14:09.000000 nuclear-1.4.0/nuclear.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-04-06 12:14:09.963242 nuclear-1.4.0/setup.cfg
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      866 2022-04-13 08:25:38.000000 nuclear-1.4.0/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.939554 nuclear-1.4.1/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2020-07-28 11:14:52.000000 nuclear-1.4.1/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-04-17 13:48:22.939554 nuclear-1.4.1/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18082 2023-04-17 13:48:22.000000 nuclear-1.4.1/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      564 2023-04-07 09:00:07.000000 nuclear-1.4.1/nuclear/__init__.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/args/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/args/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1399 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/args/args_que.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      504 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/args/container.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/autocomplete/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/autocomplete/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     4445 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/autocomplete/autocomplete.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     2175 2022-04-12 16:38:36.000000 nuclear-1.4.1/nuclear/autocomplete/install.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/builder/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/builder/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     9263 2022-04-13 09:01:27.000000 nuclear-1.4.1/nuclear/builder/builder.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3752 2022-04-13 09:02:59.000000 nuclear-1.4.1/nuclear/builder/decorator_builder.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2974 2021-12-11 21:16:15.000000 nuclear-1.4.1/nuclear/builder/rule.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11321 2022-04-13 09:13:28.000000 nuclear-1.4.1/nuclear/builder/rule_factory.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      227 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/builder/typedef.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/completers/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       33 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/completers/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      739 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/completers/file.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/help/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/help/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11775 2023-03-13 13:40:47.000000 nuclear-1.4.1/nuclear/help/help.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/inspection/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-03 14:03:48.000000 nuclear-1.4.1/nuclear/inspection/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    11910 2023-04-12 16:51:53.000000 nuclear-1.4.1/nuclear/inspection/inspection.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/parser/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      442 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/context.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      449 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/error.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1843 2021-12-11 21:16:15.000000 nuclear-1.4.1/nuclear/parser/inject.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      326 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/internal_vars.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      666 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/keyword.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1378 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/matcher.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    12607 2022-05-12 13:06:55.000000 nuclear-1.4.1/nuclear/parser/parser.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      409 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/transform.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3826 2021-12-11 21:16:15.000000 nuclear-1.4.1/nuclear/parser/validate.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1886 2022-05-13 09:22:45.000000 nuclear-1.4.1/nuclear/parser/value.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/shell/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      123 2022-05-16 13:47:34.000000 nuclear-1.4.1/nuclear/shell/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4734 2022-08-16 13:22:26.000000 nuclear-1.4.1/nuclear/shell/background_cmd.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     3676 2022-05-16 13:53:00.000000 nuclear-1.4.1/nuclear/shell/shell_utils.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/sublog/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      309 2022-06-08 11:51:00.000000 nuclear-1.4.1/nuclear/sublog/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3546 2022-06-08 12:00:57.000000 nuclear-1.4.1/nuclear/sublog/catch.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4039 2022-04-13 09:02:02.000000 nuclear-1.4.1/nuclear/sublog/context_logger.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      843 2022-06-08 12:04:08.000000 nuclear-1.4.1/nuclear/sublog/wrap_error.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/types/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       94 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/boolean.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      358 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/filesystem.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1189 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/time.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.939554 nuclear-1.4.1/nuclear/utils/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-04-12 16:16:19.000000 nuclear-1.4.1/nuclear/utils/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      116 2022-08-24 14:04:56.000000 nuclear-1.4.1/nuclear/utils/files.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      138 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/utils/input.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1301 2022-08-24 13:59:25.000000 nuclear-1.4.1/nuclear/utils/regex.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      112 2022-04-12 16:39:09.000000 nuclear-1.4.1/nuclear/utils/shell.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      688 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/utils/strings.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      362 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/utils/time.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2023-04-17 13:46:38.000000 nuclear-1.4.1/nuclear/version.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear.egg-info/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1496 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        8 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-04-17 13:48:22.939554 nuclear-1.4.1/setup.cfg
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      866 2022-04-13 08:25:38.000000 nuclear-1.4.1/setup.py
```

### Comparing `nuclear-1.4.0/LICENSE` & `nuclear-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/PKG-INFO` & `nuclear-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclear
-Version: 1.4.0
+Version: 1.4.1
 Summary: Declarative parser for command line interfaces
 Home-page: https://github.com/igrek51/nuclear
 Author: igrek51
 Author-email: igrek51.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,18 +12,18 @@
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nuclear - binding glue for CLI
 [![GitHub version](https://badge.fury.io/gh/igrek51%2Fnuclear.svg)](https://github.com/igrek51/nuclear)
 [![PyPI version](https://badge.fury.io/py/nuclear.svg)](https://pypi.org/project/nuclear)
+[![Github Pages](https://img.shields.io/badge/docs-github.io-blue)](https://igrek51.github.io/nuclear)
 [![Documentation Status](https://readthedocs.org/projects/nuclear-py/badge/?version=latest)](https://nuclear-py.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://app.travis-ci.com/igrek51/nuclear.svg?branch=master)](https://app.travis-ci.com/igrek51/nuclear)
 [![codecov](https://codecov.io/gh/igrek51/nuclear/branch/master/graph/badge.svg)](https://codecov.io/gh/igrek51/nuclear)
-[![Github Pages](https://img.shields.io/badge/github.io-ok-brightgreen)](https://igrek51.github.io/nuclear)
 
 
 `nuclear` is a declarative parser for command line interfaces in Python.
 It's a binding glue between CLI shell arguments and functions being invoked.
 It mostly focuses on building multi level command trees.
 
 `nuclear` parses and validates the command line arguments provided by the user when starting a console application.
@@ -61,15 +61,15 @@
 
 ![sublog demo](https://github.com/igrek51/nuclear/blob/master/docs/demo/demo-live.gif?raw=true)
 
 See [demo.py](https://github.com/igrek51/nuclear/blob/master/docs/demo/demo-decorator.py) for a complete example.
 
 ## Get it now
 ```bash
-pip install nuclear
+python3 -m pip install --upgrade nuclear
 ```
 
 ## CLI Tree builder
 Apart from decorator syntax style, you can also do the same using tree-builder syntax,
 which is useful in more complex cases:
 
 ```python
@@ -388,24 +388,22 @@
             argument('z'),
         ),
     ),
 ).run()
 ```
 
 ## Installation
-### Step 1. Prerequisites
-- Python 3.6 or newer (`sudo apt install python3` on Debian/Ubuntu)
-- pip
 
-### Step 2. Install package using pip
 Install package from [PyPI repository](https://pypi.org/project/nuclear) using pip:
-```bash
-pip3 install nuclear
+```shell
+python3 -m pip install --upgrade nuclear
 ```
 
+You need Python 3.6 or newer.
+
 ### Install package in develop mode
 You can install package in develop mode in order to make any changes for your own:
 ```bash
 pip3 install -r requirements.txt
 python3 setup.py develop
 ```
```

### Comparing `nuclear-1.4.0/README.md` & `nuclear-1.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Nuclear - binding glue for CLI
 [![GitHub version](https://badge.fury.io/gh/igrek51%2Fnuclear.svg)](https://github.com/igrek51/nuclear)
 [![PyPI version](https://badge.fury.io/py/nuclear.svg)](https://pypi.org/project/nuclear)
+[![Github Pages](https://img.shields.io/badge/docs-github.io-blue)](https://igrek51.github.io/nuclear)
 [![Documentation Status](https://readthedocs.org/projects/nuclear-py/badge/?version=latest)](https://nuclear-py.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://app.travis-ci.com/igrek51/nuclear.svg?branch=master)](https://app.travis-ci.com/igrek51/nuclear)
 [![codecov](https://codecov.io/gh/igrek51/nuclear/branch/master/graph/badge.svg)](https://codecov.io/gh/igrek51/nuclear)
-[![Github Pages](https://img.shields.io/badge/github.io-ok-brightgreen)](https://igrek51.github.io/nuclear)
 
 
 `nuclear` is a declarative parser for command line interfaces in Python.
 It's a binding glue between CLI shell arguments and functions being invoked.
 It mostly focuses on building multi level command trees.
 
 `nuclear` parses and validates the command line arguments provided by the user when starting a console application.
@@ -46,15 +46,15 @@
 
 ![sublog demo](https://github.com/igrek51/nuclear/blob/master/docs/demo/demo-live.gif?raw=true)
 
 See [demo.py](https://github.com/igrek51/nuclear/blob/master/docs/demo/demo-decorator.py) for a complete example.
 
 ## Get it now
 ```bash
-pip install nuclear
+python3 -m pip install --upgrade nuclear
 ```
 
 ## CLI Tree builder
 Apart from decorator syntax style, you can also do the same using tree-builder syntax,
 which is useful in more complex cases:
 
 ```python
@@ -373,24 +373,22 @@
             argument('z'),
         ),
     ),
 ).run()
 ```
 
 ## Installation
-### Step 1. Prerequisites
-- Python 3.6 or newer (`sudo apt install python3` on Debian/Ubuntu)
-- pip
 
-### Step 2. Install package using pip
 Install package from [PyPI repository](https://pypi.org/project/nuclear) using pip:
-```bash
-pip3 install nuclear
+```shell
+python3 -m pip install --upgrade nuclear
 ```
 
+You need Python 3.6 or newer.
+
 ### Install package in develop mode
 You can install package in develop mode in order to make any changes for your own:
 ```bash
 pip3 install -r requirements.txt
 python3 setup.py develop
 ```
```

### Comparing `nuclear-1.4.0/nuclear/__init__.py` & `nuclear-1.4.1/nuclear/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from .builder.rule_factory import subcommand, flag, dictionary, parameter, primary_option, argument, arguments, \
     default_action
 from .shell.shell_utils import shell, shell_error_code, shell_output, CommandError
 from .shell.background_cmd import BackgroundCommand
 from .sublog.catch import logerr, ContextError, log_exception
 from .sublog.context_logger import log
 from .sublog.wrap_error import wrap_context
-from .inspection.inspection import inspect, ins, insp, insl, insa
+from .inspection.inspection import inspect, wat, ins, insp
 
 from .version import __version__
 
 name = "nuclear"
```

### Comparing `nuclear-1.4.0/nuclear/args/args_que.py` & `nuclear-1.4.1/nuclear/args/args_que.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/autocomplete/autocomplete.py` & `nuclear-1.4.1/nuclear/autocomplete/autocomplete.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/autocomplete/install.py` & `nuclear-1.4.1/nuclear/autocomplete/install.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/builder/builder.py` & `nuclear-1.4.1/nuclear/builder/builder.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/builder/decorator_builder.py` & `nuclear-1.4.1/nuclear/builder/decorator_builder.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/builder/rule.py` & `nuclear-1.4.1/nuclear/builder/rule.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/builder/rule_factory.py` & `nuclear-1.4.1/nuclear/builder/rule_factory.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/completers/file.py` & `nuclear-1.4.1/nuclear/completers/file.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/help/help.py` & `nuclear-1.4.1/nuclear/help/help.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/inspection/inspection.py` & `nuclear-1.4.1/nuclear/inspection/inspection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from dataclasses import dataclass
 import inspect as std_inspect
 import os
 import re
 import sys
-from typing import Any, Dict, List, Optional, Type, Iterable
+from typing import Any, Dict, List, Optional, Type, Iterable, Union
 
 
 @dataclass
 class InspectConfig:
-    attrs: bool
+    attr: bool
     dunder: bool
     docs: bool
     long: bool
-    long_docs: bool
     code: bool
 
 
 @dataclass
 class InspectAttribute:
     name: str
     value: Any
@@ -27,92 +26,83 @@
     signature: Optional[str]
     doc: Optional[str]
 
 
 def inspect(
     obj: Any,
     *,
-    attrs: bool = True,
+    attr: bool = True,
     dunder: bool = False,
     docs: bool = True,
     long: bool = False,
-    long_docs: bool = False,
     code: bool = False,
     all: bool = False,
 ):
     """
     Examine the object's information, such as its type, formatted value, variables, methods,
     documentation or source code.
     :param obj: object to inspect
-    :param attrs: whether to print attributes (variables and methods)
+    :param attr: whether to print attributes (variables and methods)
     :param dunder: whether to print dunder attributes
-    :param docs: whether to print documentation
-    :param long: whether to print non-abbreviated values
-    :param long_docs: whether to print non-abbreviated documentation
+    :param docs: whether to print documentation for functions and classes
+    :param long: whether to print non-abbreviated values and documentation
     :param code: whether to print source code of a function, method or class
     :param all: whether to include all information
     """
     print(inspect_format(
-        obj, attrs=attrs or all, dunder=dunder or all, long=long or all, docs=docs or all,
-        long_docs=long_docs or all, code=code or all))
+        obj, attr=attr or all, dunder=dunder or all, long=long or all, docs=docs or all,
+        code=code or all))
 
 
 def insp(obj: Any, **kwargs):
-    """Examine object's attributes (variables and methods)"""
+    """Inspect object's attributes (variables and methods)"""
     inspect(obj, **kwargs)
 
 
 def ins(obj: Any, **kwargs):
-    """Examine object's elementary data"""
-    inspect(obj, attrs=False, **kwargs)
-
-
-def insl(obj: Any, **kwargs):
-    """Examine object's attributes, long (non-abbreviated) values and docs"""
-    inspect(obj, long=True, long_docs=True, **kwargs)
-
-
-def insa(obj: Any, **kwargs):
-    """Examine all object's information"""
-    inspect(obj, all=True, **kwargs)
+    """Inspect object's short, elementary data: value, type, signature"""
+    inspect(obj, attr=False, **kwargs)
 
 
 def inspect_format(
     obj: Any,
     *,
-    attrs: bool = True,
+    attr: bool = True,
     dunder: bool = False,
     docs: bool = True,
     long: bool = False,
-    long_docs: bool = False,
     code: bool = False,
 ) -> str:
-    config = InspectConfig(attrs=attrs, dunder=dunder, docs=docs, long=long, long_docs=long_docs, code=code)
+    config = InspectConfig(attr=attr, dunder=dunder, docs=docs, long=long, code=code)
 
     str_value = _format_value(obj)
     str_type = _format_type(type(obj))
     output: List[str] = [
         f'{STYLE_BRIGHT_BLUE}value:{RESET} {str_value}',
-        f'{STYLE_BRIGHT_BLUE}type:{RESET} {STYLE_YELLOW}{str_type}{RESET}',
+        f'{STYLE_BRIGHT_BLUE}type:{RESET} {STYLE_BRIGHT_YELLOW}{str_type}{RESET}',
     ]
  
     if callable(obj):
-        signature = _get_callable_signature(obj.__name__, obj)
+        name = getattr(obj, '__name__', '…')
+        signature = _get_callable_signature(name, obj)
         output.append(f'{STYLE_BRIGHT_BLUE}signature:{RESET} {signature}')
 
     doc = _get_doc(obj, long=True)
-    if doc and config.docs:
-        output.append(f'{STYLE_GRAY}"""\n{doc}\n"""{RESET}')
+    if doc and config.docs and callable(obj):
+        if doc.count('\n') == 0:
+            output.append(f'{STYLE_GRAY}"""{doc}"""{RESET}')
+        else:
+            output.extend([f'{STYLE_GRAY}"""', doc, f'"""{RESET}'])
 
     if config.code and (std_inspect.isclass(obj) or callable(obj)):
         source = _get_source_code(obj)
         if source:
             output.append(f'{STYLE_BRIGHT_BLUE}source code:{RESET}\n{source}')
 
-    if config.attrs:
+    if config.attr:
         attributes = sorted(_iter_attributes(obj, config), key=lambda attr: attr.name)
         output.extend(_render_attrs_section(attributes, config))
 
     if sys.stdout.isatty():  # horizontal bar
         terminal_width = os.get_terminal_size().columns
         output.insert(0, STYLE_BLUE + '─' * terminal_width + RESET)
         output.append(STYLE_BLUE + '─' * terminal_width + RESET)
@@ -127,15 +117,15 @@
     keys = dir(obj)
     for key in keys:
         value = getattr(obj, key)
         callable_ = callable(value)
         dunder = key.startswith('__') and key.endswith('__')
         private = key.startswith('_') and not dunder
         signature = _get_callable_signature(key, value) if callable_ else None
-        doc = _get_doc(value, long=config.long_docs) if callable_ else None
+        doc = _get_doc(value, long=config.long) if callable_ else None
         yield InspectAttribute(
             name=key,
             value=value,
             type=type(value),
             callable=callable_,
             dunder=dunder,
             private=private,
@@ -147,21 +137,29 @@
 def _get_callable_signature(name: str, obj: Any) -> Optional[str]:
     try:
         _signature = str(std_inspect.signature(obj))
     except (ValueError, TypeError):
         _signature = "(…)"
     
     if std_inspect.isclass(obj):
-        prefix = "class"
+        prefix = "class "
     elif std_inspect.iscoroutinefunction(obj):
-        prefix = "async def"
+        prefix = "async def "
+    elif std_inspect.isfunction(obj):
+        prefix = "def "
+    elif std_inspect.ismethod(obj):
+        prefix = "def "
+    elif std_inspect.isbuiltin(obj):
+        prefix = "def "
+    elif hasattr(obj, '__name__'):
+        prefix = "def "
     else:
-        prefix = "def"
+        prefix = ""
 
-    return f'{STYLE_BLUE}{prefix} {STYLE_BRIGHT_GREEN}{name}{STYLE_GREEN}{_signature}{RESET}'
+    return f'{STYLE_BLUE}{prefix}{STYLE_BRIGHT_GREEN}{name}{STYLE_GREEN}{_signature}{RESET}'
 
 
 def _get_source_code(obj: Any) -> Optional[str]:
     try:
         return std_inspect.getsource(obj)
     except (OSError, TypeError, IndentationError):
         return None
@@ -184,15 +182,18 @@
     return f'  {STYLE_BRIGHT_YELLOW}{attr.name}{STYLE_YELLOW}: {type_str} = {value_str}'
 
 
 def _render_attr_method(attr: InspectAttribute) -> str:
     if not attr.signature:
         return f'  {attr.name}(…)'
     if attr.doc:
-        return f'  {attr.signature}: {STYLE_GRAY}# {attr.doc}{RESET}'
+        if attr.doc.count('\n') == 0:
+            return f'  {attr.signature} {STYLE_GRAY}# {attr.doc}{RESET}'
+        else:
+            return f'  {attr.signature}:\n{STYLE_GRAY}"""\n{attr.doc}\n"""{RESET}'
     else:
         return f'  {attr.signature}'
 
 
 def _format_short_value(value: Any, long: bool) -> str:
     value_str = _format_value(value)
     if long:
@@ -301,14 +302,56 @@
             yield _render_attr_variable(attr, config)
         if dunder_vars and dunder_methods:
             yield ""
         for attr in dunder_methods:
             yield _render_attr_method(attr)
 
 
+class Wat:
+    """Reactive Inspector instance to examine unknown objects"""
+    def __init__(self, **kwargs):
+        self._params = kwargs
+
+    def __repr__(self) -> str:
+        self._print_help()
+        return ''
+        
+    def __str__(self) -> str:
+        return '<nuclear Wat Inspector object>'
+    
+    def _print_help(self):
+        print("""
+Try `wat / object`, `wat(**options) / object` or `wat(object, **options)` to inspect an object.
+options are:
+  attr=False to hide attributes (variables and methods)
+  dunder=True to print dunder attributes
+  docs=False to hide documentation for functions and classes
+  long=True to print non-abbreviated values and documentation
+  code=True to print source code of a function, method or class
+  all=True to include all information
+""".strip())
+
+    def _react_with(self, other: Any) -> None:
+        inspect(other, **self._params)
+    
+    def __call__(self, *args: Any, **kwargs: Any) -> Union['Wat', None]:
+        if args:
+            inspect(*args, **kwargs)
+        else:
+            return Wat(**kwargs)
+
+    def __truediv__(self, other: Any): return self._react_with(other) # /
+    def __lshift__(self, other: Any): return self._react_with(other)  # <<
+    def __rshift__(self, other: Any): return self._react_with(other)  # >>
+    def __or__(self, other: Any): return self._react_with(other)  # |
+    def __lt__(self, other: Any): return self._react_with(other)  # <
+
+wat = Wat()
+
+
 def _strip_color(text: str) -> str:
     return re.sub(r'\x1b\[\d+(;\d+)?m', '', text)
 
 
 RESET ='\033[0m'
 STYLE_BRIGHT = '\033[1m'
 STYLE_DIM = '\033[2m'
```

### Comparing `nuclear-1.4.0/nuclear/parser/inject.py` & `nuclear-1.4.1/nuclear/parser/inject.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/parser/keyword.py` & `nuclear-1.4.1/nuclear/parser/keyword.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/parser/matcher.py` & `nuclear-1.4.1/nuclear/parser/matcher.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/parser/parser.py` & `nuclear-1.4.1/nuclear/parser/parser.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/parser/validate.py` & `nuclear-1.4.1/nuclear/parser/validate.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/parser/value.py` & `nuclear-1.4.1/nuclear/parser/value.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/shell/background_cmd.py` & `nuclear-1.4.1/nuclear/shell/background_cmd.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/shell/shell_utils.py` & `nuclear-1.4.1/nuclear/shell/shell_utils.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/sublog/catch.py` & `nuclear-1.4.1/nuclear/sublog/catch.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/sublog/context_logger.py` & `nuclear-1.4.1/nuclear/sublog/context_logger.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/sublog/wrap_error.py` & `nuclear-1.4.1/nuclear/sublog/wrap_error.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/types/time.py` & `nuclear-1.4.1/nuclear/types/time.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/utils/regex.py` & `nuclear-1.4.1/nuclear/utils/regex.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear/utils/strings.py` & `nuclear-1.4.1/nuclear/utils/strings.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/nuclear.egg-info/PKG-INFO` & `nuclear-1.4.1/nuclear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclear
-Version: 1.4.0
+Version: 1.4.1
 Summary: Declarative parser for command line interfaces
 Home-page: https://github.com/igrek51/nuclear
 Author: igrek51
 Author-email: igrek51.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,18 +12,18 @@
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nuclear - binding glue for CLI
 [![GitHub version](https://badge.fury.io/gh/igrek51%2Fnuclear.svg)](https://github.com/igrek51/nuclear)
 [![PyPI version](https://badge.fury.io/py/nuclear.svg)](https://pypi.org/project/nuclear)
+[![Github Pages](https://img.shields.io/badge/docs-github.io-blue)](https://igrek51.github.io/nuclear)
 [![Documentation Status](https://readthedocs.org/projects/nuclear-py/badge/?version=latest)](https://nuclear-py.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://app.travis-ci.com/igrek51/nuclear.svg?branch=master)](https://app.travis-ci.com/igrek51/nuclear)
 [![codecov](https://codecov.io/gh/igrek51/nuclear/branch/master/graph/badge.svg)](https://codecov.io/gh/igrek51/nuclear)
-[![Github Pages](https://img.shields.io/badge/github.io-ok-brightgreen)](https://igrek51.github.io/nuclear)
 
 
 `nuclear` is a declarative parser for command line interfaces in Python.
 It's a binding glue between CLI shell arguments and functions being invoked.
 It mostly focuses on building multi level command trees.
 
 `nuclear` parses and validates the command line arguments provided by the user when starting a console application.
@@ -61,15 +61,15 @@
 
 ![sublog demo](https://github.com/igrek51/nuclear/blob/master/docs/demo/demo-live.gif?raw=true)
 
 See [demo.py](https://github.com/igrek51/nuclear/blob/master/docs/demo/demo-decorator.py) for a complete example.
 
 ## Get it now
 ```bash
-pip install nuclear
+python3 -m pip install --upgrade nuclear
 ```
 
 ## CLI Tree builder
 Apart from decorator syntax style, you can also do the same using tree-builder syntax,
 which is useful in more complex cases:
 
 ```python
@@ -388,24 +388,22 @@
             argument('z'),
         ),
     ),
 ).run()
 ```
 
 ## Installation
-### Step 1. Prerequisites
-- Python 3.6 or newer (`sudo apt install python3` on Debian/Ubuntu)
-- pip
 
-### Step 2. Install package using pip
 Install package from [PyPI repository](https://pypi.org/project/nuclear) using pip:
-```bash
-pip3 install nuclear
+```shell
+python3 -m pip install --upgrade nuclear
 ```
 
+You need Python 3.6 or newer.
+
 ### Install package in develop mode
 You can install package in develop mode in order to make any changes for your own:
 ```bash
 pip3 install -r requirements.txt
 python3 setup.py develop
 ```
```

### Comparing `nuclear-1.4.0/nuclear.egg-info/SOURCES.txt` & `nuclear-1.4.1/nuclear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.0/setup.py` & `nuclear-1.4.1/setup.py`

 * *Files identical despite different names*

