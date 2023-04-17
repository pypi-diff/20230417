# Comparing `tmp/pddl-plus-parser-3.2.2.tar.gz` & `tmp/pddl-plus-parser-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl-plus-parser-3.2.2.tar", last modified: Tue Mar 14 09:35:58 2023, max compression
+gzip compressed data, was "pddl-plus-parser-3.3.0.tar", last modified: Mon Apr 17 12:20:48 2023, max compression
```

## Comparing `pddl-plus-parser-3.2.2.tar` & `pddl-plus-parser-3.3.0.tar`

### file list

```diff
@@ -1,85 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.687265 pddl-plus-parser-3.2.2/
--rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.2.2/LICENSE
--rw-rw-rw-   0        0        0     1425 2023-03-14 09:35:58.687265 pddl-plus-parser-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1156 2022-12-26 16:00:35.000000 pddl-plus-parser-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.264944 pddl-plus-parser-3.2.2/pddl_plus_parser/
--rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.313051 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/
--rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/__init__.py
--rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/domain_exporter.py
--rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/enhsp_output_parser.py
--rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/ff_output_parser.py
--rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
--rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/problem_exporter.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.365881 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/
--rw-rw-rw-   0        0        0      278 2022-03-13 11:19:35.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/__init__.py
--rw-rw-rw-   0        0        0    32015 2023-01-25 08:20:05.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/domain_parser.py
--rw-rw-rw-   0        0        0      814 2023-02-01 12:22:20.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/parsing_utils.py
--rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
--rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
--rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/problem_parser.py
--rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/trajectory_parser.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.470950 pddl-plus-parser-3.2.2/pddl_plus_parser/models/
--rw-rw-rw-   0        0        0      822 2023-01-25 08:20:05.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/action_call.py
--rw-rw-rw-   0        0        0     1883 2022-12-05 10:27:33.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/conditional_effect.py
--rw-rw-rw-   0        0        0     6618 2022-12-05 08:50:16.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/numerical_expression.py
--rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/observation.py
--rw-rw-rw-   0        0        0     1992 2023-01-25 08:20:05.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_action.py
--rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_domain.py
--rw-rw-rw-   0        0        0     3702 2022-12-05 08:50:44.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_function.py
--rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_object.py
--rw-rw-rw-   0        0        0    32583 2023-01-25 08:26:37.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_operator.py
--rw-rw-rw-   0        0        0     4365 2023-01-31 14:29:25.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_predicate.py
--rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_problem.py
--rw-rw-rw-   0        0        0     2361 2022-11-18 11:18:07.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_state.py
--rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_type.py
--rw-rw-rw-   0        0        0     2236 2022-12-26 16:36:19.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/models/universal_quantifier.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.514479 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/
--rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     3443 2022-12-05 15:56:44.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/common.py
--rw-rw-rw-   0        0        0     3162 2023-02-21 12:40:06.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
--rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
--rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
--rw-rw-rw-   0        0        0    10132 2022-11-03 09:33:36.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.578379 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/
--rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/__init__.py
--rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/common.py
--rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/counters_generator.py
--rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/depots_generator.py
--rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/farmland_generator.py
--rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/plant_watering_generator.py
--rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/sailing_generator.py
--rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/settlers_problem_generator.py
--rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/zenotravel_generator.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.278975 pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/
--rw-rw-rw-   0        0        0     1425 2023-03-14 09:35:58.000000 pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-03-14 09:35:58.000000 pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 09:35:58.000000 pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-03-14 09:35:58.000000 pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 09:35:58.688272 pddl-plus-parser-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-03-14 09:35:41.000000 pddl-plus-parser-3.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.255943 pddl-plus-parser-3.2.2/tests/
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.580364 pddl-plus-parser-3.2.2/tests/exporters_tests/
--rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.2.2/tests/exporters_tests/__init__.py
--rw-rw-rw-   0        0        0     9626 2023-03-14 09:34:14.000000 pddl-plus-parser-3.2.2/tests/exporters_tests/numeric_trajectory_exporter_test.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.617113 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/
--rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/__init__.py
--rw-rw-rw-   0        0        0     3235 2023-02-21 15:21:04.000000 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/consts.py
--rw-rw-rw-   0        0        0    34466 2023-01-25 08:21:39.000000 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/domain_parser_test.py
--rw-rw-rw-   0        0        0     2219 2022-03-13 12:12:23.000000 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/pddl_tokenizer_test.py
--rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/problem_parser_test.py
--rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/trajectory_parser_test.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.647083 pddl-plus-parser-3.2.2/tests/models_tests/
--rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.2.2/tests/models_tests/__init__.py
--rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.2.2/tests/models_tests/consts.py
--rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.2.2/tests/models_tests/numerical_expression_test.py
--rw-rw-rw-   0        0        0    28898 2022-12-05 14:51:13.000000 pddl-plus-parser-3.2.2/tests/models_tests/operator_test.py
--rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.2.2/tests/models_tests/pddl_function_test.py
-drwxrwxrwx   0        0        0        0 2023-03-14 09:35:58.684286 pddl-plus-parser-3.2.2/tests/multi_agent_tests/
--rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.2.2/tests/multi_agent_tests/__init__.py
--rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.2.2/tests/multi_agent_tests/consts.py
--rw-rw-rw-   0        0        0     2069 2022-11-13 14:51:03.000000 pddl-plus-parser-3.2.2/tests/multi_agent_tests/multi_agent_domain_converter_test.py
--rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.2.2/tests/multi_agent_tests/multi_agent_problem_converter_test.py
--rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.2.2/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
--rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.2.2/tests/multi_agent_tests/single_agent_plan_converter_test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.203707 pddl-plus-parser-3.3.0/
+-rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1519 2023-04-17 12:20:48.203707 pddl-plus-parser-3.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:47.912536 pddl-plus-parser-3.3.0/pddl_plus_parser/
+-rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:47.970354 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/
+-rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/__init__.py
+-rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/domain_exporter.py
+-rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/enhsp_output_parser.py
+-rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/ff_output_parser.py
+-rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
+-rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/problem_exporter.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.004009 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/
+-rw-rw-rw-   0        0        0      374 2023-04-09 14:37:04.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/__init__.py
+-rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/domain_parser.py
+-rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/effects_parser.py
+-rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/parsing_utils.py
+-rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
+-rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
+-rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/preconditions_parser.py
+-rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/problem_parser.py
+-rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/trajectory_parser.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.084313 pddl-plus-parser-3.3.0/pddl_plus_parser/models/
+-rw-rw-rw-   0        0        0      929 2023-04-09 14:33:10.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/action_call.py
+-rw-rw-rw-   0        0        0     1853 2023-04-13 11:59:48.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/conditional_effect.py
+-rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/grounded_effect.py
+-rw-rw-rw-   0        0        0    12934 2023-04-17 09:01:49.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/grounded_precondition.py
+-rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/grounding_utils.py
+-rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/numerical_expression.py
+-rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/observation.py
+-rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_action.py
+-rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_domain.py
+-rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_function.py
+-rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_object.py
+-rw-rw-rw-   0        0        0     8519 2023-04-17 10:10:02.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_operator.py
+-rw-rw-rw-   0        0        0     3826 2023-04-16 15:06:32.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_precondition.py
+-rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_predicate.py
+-rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_problem.py
+-rw-rw-rw-   0        0        0     2845 2023-04-16 13:40:45.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_state.py
+-rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_type.py
+-rw-rw-rw-   0        0        0     1865 2023-04-09 08:35:12.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/models/universal_quantifier.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.089857 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/
+-rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/common.py
+-rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
+-rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
+-rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
+-rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.153034 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/
+-rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/__init__.py
+-rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/common.py
+-rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/counters_generator.py
+-rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/depots_generator.py
+-rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/farmland_generator.py
+-rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/plant_watering_generator.py
+-rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/sailing_generator.py
+-rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/settlers_problem_generator.py
+-rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/zenotravel_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:47.932594 pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/
+-rw-rw-rw-   0        0        0     1519 2023-04-17 12:20:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3522 2023-04-17 12:20:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 12:20:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-17 12:20:47.000000 pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 12:20:48.203707 pddl-plus-parser-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-04-17 12:03:25.000000 pddl-plus-parser-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:47.902947 pddl-plus-parser-3.3.0/tests/
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.154040 pddl-plus-parser-3.3.0/tests/exporters_tests/
+-rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.3.0/tests/exporters_tests/__init__.py
+-rw-rw-rw-   0        0        0     9454 2023-04-17 10:52:47.000000 pddl-plus-parser-3.3.0/tests/exporters_tests/numeric_trajectory_exporter_test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.179614 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/__init__.py
+-rw-rw-rw-   0        0        0     3288 2023-04-17 12:07:14.000000 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/consts.py
+-rw-rw-rw-   0        0        0    39905 2023-04-17 12:16:07.000000 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/domain_parser_test.py
+-rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/pddl_tokenizer_test.py
+-rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/problem_parser_test.py
+-rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/trajectory_parser_test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.190183 pddl-plus-parser-3.3.0/tests/models_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.3.0/tests/models_tests/__init__.py
+-rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.3.0/tests/models_tests/consts.py
+-rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.3.0/tests/models_tests/grounded_effect_test.py
+-rw-rw-rw-   0        0        0    25195 2023-04-17 09:16:34.000000 pddl-plus-parser-3.3.0/tests/models_tests/grounded_precondition_test.py
+-rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.3.0/tests/models_tests/numerical_expression_test.py
+-rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.3.0/tests/models_tests/operator_test.py
+-rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.3.0/tests/models_tests/pddl_function_test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:20:48.201718 pddl-plus-parser-3.3.0/tests/multi_agent_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.3.0/tests/multi_agent_tests/__init__.py
+-rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.3.0/tests/multi_agent_tests/consts.py
+-rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.3.0/tests/multi_agent_tests/multi_agent_domain_converter_test.py
+-rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.3.0/tests/multi_agent_tests/multi_agent_problem_converter_test.py
+-rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.3.0/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
+-rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.3.0/tests/multi_agent_tests/single_agent_plan_converter_test.py
```

### Comparing `pddl-plus-parser-3.2.2/LICENSE` & `pddl-plus-parser-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/PKG-INFO` & `pddl-plus-parser-3.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.2.2
+Version: 3.3.0
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
@@ -24,8 +24,9 @@
 * version 1.4.0 - Added negative preconditions for actions.
 * version 2.0.0 - Added support for multi-agent PDDL domains and problems.
 * version 2.1.0 - Added support for more complex type of multi-agent trajectories to support non-trivial interactions. 
 * version 2.2.0 - Added support for domains with disjunctive numeric preconditions.
 * version 3.0.0 - Added support for conditional effect without existential quantification and only conjunctive conditions.
 * version 3.1.0 - Added support for universal effects containing only conjunctive conditions.
 * version 3.1.4 - Added support for inapplicable actions and fixed a minor logical bug in the universal effects.
+* version 3.3.0 - Added support for nested action schemas including universal preconditions.
```

### Comparing `pddl-plus-parser-3.2.2/README.md` & `pddl-plus-parser-3.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 * version 1.4.0 - Added negative preconditions for actions.
 * version 2.0.0 - Added support for multi-agent PDDL domains and problems.
 * version 2.1.0 - Added support for more complex type of multi-agent trajectories to support non-trivial interactions. 
 * version 2.2.0 - Added support for domains with disjunctive numeric preconditions.
 * version 3.0.0 - Added support for conditional effect without existential quantification and only conjunctive conditions.
 * version 3.1.0 - Added support for universal effects containing only conjunctive conditions.
 * version 3.1.4 - Added support for inapplicable actions and fixed a minor logical bug in the universal effects.
+* version 3.3.0 - Added support for nested action schemas including universal preconditions.
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/domain_exporter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/domain_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/enhsp_output_parser.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/enhsp_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/ff_output_parser.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/ff_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/numeric_trajectory_exporter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/numeric_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/exporters/problem_exporter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/exporters/problem_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/problem_parser.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/problem_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/lisp_parsers/trajectory_parser.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/lisp_parsers/trajectory_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/__init__.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .action_call import ActionCall, JointActionCall, NOP_ACTION
-from .conditional_effect import ConditionalEffect
+from .conditional_effect import ConditionalEffect, UniversalEffect
 from .numerical_expression import construct_expression_tree, calculate, evaluate_expression, NumericalExpressionTree
 from .observation import ActionCall, Observation, ObservedComponent, MultiAgentObservation, MultiAgentComponent
 from .pddl_action import Action
 from .pddl_domain import Domain
 from .pddl_function import PDDLFunction
 from .pddl_object import PDDLObject, PDDLConstant
 from .pddl_operator import Operator, NOPOperator
+from .pddl_precondition import Precondition, CompoundPrecondition, UniversalPrecondition
 from .pddl_predicate import SignatureType, Predicate, GroundedPredicate
 from .pddl_problem import Problem
 from .pddl_state import State
 from .pddl_type import PDDLType
 from .universal_quantifier import UniversalQuantifiedPrecondition, UniversalQuantifiedEffect
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/action_call.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/action_call.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/conditional_effect.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/conditional_effect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 """Module to handle the functionality of conditional effects."""
 from typing import Union, Set
 
+from .pddl_precondition import CompoundPrecondition
+from .pddl_type import PDDLType
 from .pddl_predicate import Predicate, GroundedPredicate
 from .numerical_expression import NumericalExpressionTree
 
 
 class ConditionalEffect:
     """Class representing a conditional effect in a PDDL+ action."""
 
-    positive_conditions: Set[Union[Predicate, GroundedPredicate]]
-    negative_conditions: Set[Union[Predicate, GroundedPredicate]]
-    numeric_conditions: Set[NumericalExpressionTree]
-    add_effects: Set[Union[Predicate, GroundedPredicate]]
-    delete_effects: Set[Union[Predicate, GroundedPredicate]]
+    antecedents: CompoundPrecondition
+    discrete_effects: Set[Union[Predicate, GroundedPredicate]]
     numeric_effects: Set[NumericalExpressionTree]
 
     def __init__(self):
-        self.positive_conditions = set()
-        self.negative_conditions = set()
-        self.numeric_conditions = set()
-        self.add_effects = set()
-        self.delete_effects = set()
+        self.antecedents = CompoundPrecondition()
+        self.discrete_effects = set()
         self.numeric_effects = set()
 
     def __str__(self):
-        positive_antecedents = "\n\t".join([cond.untyped_representation for cond in self.positive_conditions])
-        negative_antecedents = "\n\t".join(
-            [f"(not {negative_cond.untyped_representation})" for negative_cond in self.negative_conditions])
-        numeric_antecedents = "\n\t".join([cond.to_pddl() for cond in self.numeric_conditions])
-        add_effect = "\n\t".join([effect.untyped_representation for effect in self.add_effects])
-        delete_effect = "\n\t".join(
-            [f"(not {negative_effect.untyped_representation})" for negative_effect in self.delete_effects])
-        discrete_effect = add_effect + delete_effect
+        discrete_effect = "\n\t".join([effect.untyped_representation for effect in self.discrete_effects])
         numeric_effect = "\n\t".join([effect.to_pddl() for effect in self.numeric_effects])
 
-        return f"(when (and {positive_antecedents}{negative_antecedents}{numeric_antecedents}) " \
+        return f"(when {str(self.antecedents)} " \
                f"(and {discrete_effect}{numeric_effect}))"
+
+
+class UniversalEffect:
+    """Class representing a universal quantifier in a PDDL+ action."""
+
+    quantified_parameter: str
+    quantified_type: PDDLType
+    conditional_effects: Set[ConditionalEffect]
+
+    def __init__(self, quantified_parameter: str, quantified_type: PDDLType):
+        self.quantified_parameter = quantified_parameter
+        self.quantified_type = quantified_type
+        self.conditional_effects = set()
+
+    def __str__(self):
+        if len(self.conditional_effects) == 0:
+            return ""
+
+        conditional_effects = "\n\t".join([str(conditional_effect) for conditional_effect in self.conditional_effects])
+        return f"(forall ({self.quantified_parameter} - {self.quantified_type.name})" \
+               f"\n\t\t{conditional_effects})"
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/numerical_expression.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/numerical_expression.py`

 * *Files 10% similar despite different names*

```diff
@@ -131,14 +131,37 @@
         return assigned_variable
 
     compared_operator = calculate(expression_tree.children[0])
     evaluated_operand = calculate(expression_tree.children[1])
     return COMPARISON_OPERATORS[expression_tree.value](compared_operator, evaluated_operand)
 
 
+def set_expression_value(expression_node: AnyNode, state_fluents: Dict[str, PDDLFunction]) -> None:
+    """Set the value of the expression according to the fluents present in the state.
+
+    :param expression_node: the node that is currently being observed.
+    :param state_fluents: the grounded numeric fluents present in the state.
+    """
+    if expression_node.is_leaf:
+        if not isinstance(expression_node.value, PDDLFunction):
+            return
+
+        grounded_fluent: PDDLFunction = expression_node.value
+        try:
+            grounded_fluent.set_value(state_fluents[grounded_fluent.untyped_representation].value)
+
+        except KeyError:
+            grounded_fluent.set_value(0.0)
+
+        return
+
+    set_expression_value(expression_node.children[0], state_fluents)
+    set_expression_value(expression_node.children[1], state_fluents)
+
+
 class NumericalExpressionTree:
     root: AnyNode
 
     def __init__(self, expression_tree: AnyNode):
         self.root = expression_tree
 
     def __str__(self):
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/observation.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/observation.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_action.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 """Module that represents a PDDL+ action."""
-from typing import Set, List, Tuple
+from typing import Set, List
 
-from .universal_quantifier import UniversalQuantifiedEffect
-from .conditional_effect import ConditionalEffect
+from .conditional_effect import ConditionalEffect, UniversalEffect
 from .numerical_expression import NumericalExpressionTree
+from .pddl_precondition import CompoundPrecondition
 from .pddl_predicate import SignatureType, Predicate
 
 
 class Action:
     """Class representing an instantaneous action in a PDDL+ problems."""
 
     name: str
     signature: SignatureType
-    positive_preconditions: Set[Predicate]
-    negative_preconditions: Set[Predicate]
-    numeric_preconditions: Set[NumericalExpressionTree]
-    equality_preconditions: Set[Tuple[str, str]]
-    inequality_preconditions: Set[Tuple[str, str]]
-    add_effects: Set[Predicate]
-    delete_effects: Set[Predicate]
+    preconditions: CompoundPrecondition
+
+    discrete_effects: Set[Predicate]
     conditional_effects: Set[ConditionalEffect]
-    universal_effects: Set[UniversalQuantifiedEffect]
+    universal_effects: Set[UniversalEffect]
     numeric_effects: Set[NumericalExpressionTree]
-    # currently only supporting disjunction of numeric preconditions
-    disjunctive_numeric_preconditions: List[Set[NumericalExpressionTree]]
 
     def __init__(self):
-        self.positive_preconditions = set()
-        self.negative_preconditions = set()
-        self.numeric_preconditions = set()
-        self.equality_preconditions = set()
-        self.inequality_preconditions = set()
-        self.add_effects = set()
-        self.delete_effects = set()
+        self.discrete_effects = set()
         self.numeric_effects = set()
-        self.disjunctive_numeric_preconditions = []
         self.conditional_effects = set()
         self.universal_effects = set()
 
     def __str__(self):
         signature_str_items = []
         for parameter_name, parameter_type in self.signature.items():
             signature_str_items.append(f"{parameter_name} - {str(parameter_type)}")
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_domain.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_domain.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_function.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
             other_param_type = other.signature[parameter_name]
             if not parameter_type.is_sub_type(other_param_type):
                 return False
 
         return True
 
+    def copy(self) -> "PDDLFunction":
+        """Creates a copy of the function."""
+        copied_function = PDDLFunction(self.name, self.signature, self.repeating_variables)
+        copied_function.stored_value = self.stored_value
+        return copied_function
+
     @property
     def value(self) -> float:
         return self.stored_value
 
     def set_value(self, value: float) -> None:
         """Set the value of a function to be the input value.
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_predicate.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_predicate.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
             other_param_type = other.signature[parameter_name]
             if not parameter_type == other_param_type and not parameter_type.is_sub_type(other_param_type):
                 return False
 
         return True
 
+    def copy(self) -> "Predicate":
+        """Creates a copy of the predicate."""
+        return Predicate(self.name, self.signature, is_positive=self.is_positive)
+
     @property
     def untyped_representation(self) -> str:
         untyped_signature_str = " ".join(self.signature.keys())
         if self.is_positive:
             return f"({self.name} {untyped_signature_str})"
         return f"(not ({self.name} {untyped_signature_str}))"
 
@@ -85,14 +89,18 @@
             return False
 
         return self.object_mapping == other.object_mapping
 
     def __ne__(self, other: "GroundedPredicate") -> bool:
         return not self.__eq__(other)
 
+    def copy(self) -> "GroundedPredicate":
+        """Creates a copy of the grounded predicate."""
+        return GroundedPredicate(self.name, self.signature, self.object_mapping, self.is_positive)
+
     @property
     def untyped_representation(self) -> str:
         untyped_grounded_signature_str = " ".join(self.object_mapping.values())
         if self.is_positive:
             return f"({self.name} {untyped_grounded_signature_str})"
         return f"(not ({self.name} {untyped_grounded_signature_str}))"
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_problem.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_problem.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_state.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,7 +52,15 @@
         return f"({' '.join(fluent.state_typed_representation for fluent in self.state_fluents.values())}" \
                f"{typed_predicates_str})\n"
 
     def serialize(self) -> str:
         return f"({':init' if self.is_init else ':state'}" \
                f" {self._serialize_numeric_fluents()}" \
                f"{self._serialize_predicates()})\n"
+
+    def copy(self) -> "State":
+        """Creates a copy of the state."""
+        copied_predicates = {predicate_name: {predicate.copy() for predicate in predicates} for
+                             predicate_name, predicates
+                             in self.state_predicates.items()}
+        copied_fluents = {fluent_name: fluent.copy() for fluent_name, fluent in self.state_fluents.items()}
+        return State(copied_predicates, copied_fluents, is_init=self.is_init)
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/pddl_type.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/pddl_type.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/models/universal_quantifier.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/models/universal_quantifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,30 +7,26 @@
 
 
 class UniversalQuantifiedPrecondition:
     """Class representing a universally quantified precondition."""
 
     quantified_parameter: str
     quantified_type: PDDLType
-    positive_conditions: Set[Predicate]
-    negative_conditions: Set[Predicate]
+    discrete_conditions: Set[Predicate]
+    # TODO: Add numeric conditions
 
-    def __init__(self, quantified_parameter: str, quantified_type: PDDLType, positive_conditions: Set[Predicate],
-                 negative_conditions: Set[Predicate]):
+    def __init__(self, quantified_parameter: str, quantified_type: PDDLType, conditions: Set[Predicate]):
         self.quantified_parameter = quantified_parameter
         self.quantified_type = quantified_type
-        self.positive_conditions = positive_conditions
-        self.negative_conditions = negative_conditions
+        self.discrete_conditions = conditions
 
     def __str__(self):
-        positive_conditionals = "\n\t".join([cond.untyped_representation for cond in self.positive_conditions])
-        negative_conditionals = "\n\t".join([f"(not {negative_cond.untyped_representation})" for
-                                             negative_cond in self.negative_conditions])
+        conditions = "\n\t".join([cond.untyped_representation for cond in self.discrete_conditions])
         return f"(forall ({self.quantified_parameter} - {self.quantified_type.name})" \
-               f"\n\t{positive_conditionals}\n\t{negative_conditionals})"
+               f"\n\t{conditions})"
 
 
 class UniversalQuantifiedEffect:
     """Class representing a universal quantifier in a PDDL+ action."""
 
     quantified_parameter: str
     quantified_type: PDDLType
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/common.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,45 +22,26 @@
 
     :param domain: the domain with the action scheme.
     :param current_state: the current state that the action is being applied on.
     :param joint_action: the executable actions of the agents.
     :param allow_inapplicable_actions: whether to allow inapplicable actions.
     :return: The state resulting from applying the actions.
     """
-    operators = []
     if len(joint_action) == 1:
         action_call = joint_action[0]
         action = domain.actions[action_call.name]
         return Operator(action=action, domain=domain, grounded_action_call=action_call.parameters).apply(
             previous_state=current_state, allow_inapplicable_actions=allow_inapplicable_actions)
 
-    accumulative_discrete_effects = defaultdict(set)
-    accumulative_numeric_effects = current_state.state_fluents.copy()
-    for lifted_name, grounded_predicates in current_state.state_predicates.items():
-        for predicate in grounded_predicates:
-            accumulative_discrete_effects[lifted_name].add(GroundedPredicate(predicate.name, predicate.signature,
-                                                                             predicate.object_mapping))
-
+    accumulative_changed_state = current_state.copy()
     for action_call in joint_action:
         if action_call.name == NOP_ACTION:
             continue
 
         action = domain.actions[action_call.name]
         operator = Operator(action=action, domain=domain, grounded_action_call=action_call.parameters)
-        partial_numeric_state = State(predicates=current_state.state_predicates, fluents=accumulative_numeric_effects)
-        partial_next_state = operator.apply(partial_numeric_state)
-        accumulative_numeric_effects.update(partial_next_state.state_fluents)
-        # since there are multiple actions being executed at once, we need to take the difference between the
-        # current state and the next state and accumulate it.
-        for delete_effect in operator.grounded_delete_effects:
-            for grounded_predicate in accumulative_discrete_effects[delete_effect.lifted_untyped_representation]:
-                if grounded_predicate.untyped_representation == delete_effect.untyped_representation:
-                    accumulative_discrete_effects[delete_effect.lifted_untyped_representation].remove(
-                        grounded_predicate)
-                    break
-
-        for add_effect in operator.grounded_add_effects:
-            accumulative_discrete_effects[add_effect.lifted_untyped_representation].add(add_effect)
-
-        operators.append(operator)
+        if operator.is_applicable(current_state) or allow_inapplicable_actions:
+            accumulative_changed_state = operator.apply(accumulative_changed_state, allow_inapplicable_actions=True)
+        else:
+            raise ValueError("Cannot apply an action when it is not applicable!")
 
-    return State(predicates=accumulative_discrete_effects, fluents=accumulative_numeric_effects)
+    return accumulative_changed_state
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 
 from pddl_plus_parser.exporters import DomainExporter
 from pddl_plus_parser.lisp_parsers import DomainParser
 from pddl_plus_parser.models import Domain, Predicate, Action
 
 DUMMY_PREDICATE_NAME = "dummy-additional-predicate"
-DUMMY_PREDICATE = Predicate(name=DUMMY_PREDICATE_NAME, signature={}, is_positive=True)
+DUMMY_ADD_PREDICATE = Predicate(name=DUMMY_PREDICATE_NAME, signature={}, is_positive=True)
+DUMMY_DEL_PREDICATE = Predicate(name=DUMMY_PREDICATE_NAME, signature={}, is_positive=False)
 
 
 class MultiAgentDomainsConverter:
     """Converts multiple MA domains to single agent domain containing all the agents' data."""
 
     logger: logging.Logger
     domains_directory_path: Path
@@ -25,21 +26,21 @@
 
         :param domain: the domain to add the dummy action to.
         """
         self.logger.debug("Adding the dummy actions to the domain.")
         add_action = Action()
         add_action.name = "dummy-add-predicate-action"
         add_action.signature = {"?agent": domain.types["object"]}
-        add_action.add_effects = {DUMMY_PREDICATE}
+        add_action.discrete_effects = {DUMMY_ADD_PREDICATE}
         domain.actions[add_action.name] = add_action
 
         delete_action = Action()
         delete_action.name = "dummy-del-predicate-action"
         delete_action.signature = {"?agent": domain.types["object"]}
-        delete_action.delete_effects = {DUMMY_PREDICATE}
+        delete_action.discrete_effects = {DUMMY_DEL_PREDICATE}
         domain.actions[delete_action.name] = delete_action
 
     def locate_domains(self) -> Domain:
         """Locate only the domains when there is no need to also parse the problems."""
         combined_domain = Domain()
         for domain_path in self.domains_directory_path.glob("domain-*.pddl"):
             self.logger.debug(f"Working on the domain - {domain_path.stem}")
@@ -53,15 +54,15 @@
             combined_domain.predicates.update(agent_domain.predicates)
             combined_domain.constants.update(agent_domain.constants)
             combined_domain.actions.update(agent_domain.actions)
             combined_domain.functions.update(agent_domain.functions)
 
             self.logger.debug(f"extracted the domain - {domain_file_name}")
 
-        combined_domain.predicates[DUMMY_PREDICATE.name] = DUMMY_PREDICATE
+        combined_domain.predicates[DUMMY_ADD_PREDICATE.name] = DUMMY_ADD_PREDICATE
         self._add_dummy_actions(combined_domain)
         return combined_domain
 
     def export_combined_domain(self) -> None:
         """Export the multi-agent domains to a single PDDL domain file."""
         combined_domain = self.locate_domains()
         DomainExporter().export_domain(combined_domain, self.domains_directory_path / f"combined_domain.pddl")
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/multi_agent/single_agent_plan_converter.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/multi_agent/single_agent_plan_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module to convert single agent plans to multi-agent plans with joint actions."""
 import logging
 import re
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, Tuple, Set
 
 from pddl_plus_parser.models import Domain, ActionCall, Operator, JointActionCall, NOP_ACTION, Problem, State
 from pddl_plus_parser.multi_agent.common import create_initial_state, apply_actions
 
 PLAN_COMPONENT_REGEX = r"[\d+ : ]?\(([\w+\s?-]+)\)"
 
 
@@ -38,14 +38,32 @@
             action_parameters = action_components[1:]
             # assuming that only one agent executes an action
             executing_agent = [param for param in action_parameters if param in agent_names][0]
             plan_seq.append((ActionCall(action_name, action_parameters), executing_agent))
 
         return plan_seq
 
+    def _extract_grounded_effects(self, operator: Operator) -> Tuple[Set[str], Set[str]]:
+        """Extracts the grounded add and delete effects of the operator.
+
+        :param operator: the operator.
+        :return: the grounded add and delete effects.
+        """
+        self.logger.debug("Extracting the grounded add and delete effects of the operator!")
+        add_effects = set()
+        delete_effects = set()
+        for effect in operator.grounded_effects:
+            for discrete_effect in effect.grounded_discrete_effects:
+                if discrete_effect.is_positive:
+                    add_effects.add(discrete_effect.untyped_representation)
+                else:
+                    delete_effects.add(discrete_effect.untyped_representation)
+
+        return add_effects, delete_effects
+
     def _validate_well_defined_action_literals(self, combined_actions: List[ActionCall], next_action: Operator) -> bool:
         """Validates whether the actions' grounded literals are well-defined.
 
         We define a contradiction as the following:
             If a fluent and its negation exist in the same time, than it is considered a contradiction.
 
         Note: extending to numeric actions is easy when considering that two actions cannot change the same function at
@@ -61,19 +79,19 @@
 
         for action_call in combined_actions:
             if action_call.name == NOP_ACTION:
                 continue
 
             op = Operator(self.ma_domain.actions[action_call.name], self.ma_domain, action_call.parameters)
             op.ground()
-            accumulated_add_effects.update([p.untyped_representation for p in op.grounded_add_effects])
-            accumulated_delete_effects.update([p.untyped_representation for p in op.grounded_delete_effects])
+            action_add_effect, action_del_effect = self._extract_grounded_effects(op)
+            accumulated_add_effects.update(action_add_effect)
+            accumulated_delete_effects.update(action_del_effect)
 
-        next_action_add_effects = [p.untyped_representation for p in next_action.grounded_add_effects]
-        next_action_del_effects = [p.untyped_representation for p in next_action.grounded_delete_effects]
+        next_action_add_effects, next_action_del_effects = self._extract_grounded_effects(next_action)
 
         return not (len(accumulated_add_effects.intersection(next_action_del_effects)) > 0 or
                     len(accumulated_delete_effects.intersection(next_action_add_effects)) > 0)
 
     def _validate_well_defined_joint_action(self, current_state: State,
                                             combined_actions: List[ActionCall], next_action: ActionCall,
                                             next_executing_agent: str, agent_names: List[str],
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/counters_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/counters_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/depots_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/depots_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/farmland_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/farmland_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/plant_watering_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/plant_watering_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/sailing_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/sailing_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/settlers_problem_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/settlers_problem_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser/problem_generators/zenotravel_generator.py` & `pddl-plus-parser-3.3.0/pddl_plus_parser/problem_generators/zenotravel_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/PKG-INFO` & `pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.2.2
+Version: 3.3.0
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
@@ -24,8 +24,9 @@
 * version 1.4.0 - Added negative preconditions for actions.
 * version 2.0.0 - Added support for multi-agent PDDL domains and problems.
 * version 2.1.0 - Added support for more complex type of multi-agent trajectories to support non-trivial interactions. 
 * version 2.2.0 - Added support for domains with disjunctive numeric preconditions.
 * version 3.0.0 - Added support for conditional effect without existential quantification and only conjunctive conditions.
 * version 3.1.0 - Added support for universal effects containing only conjunctive conditions.
 * version 3.1.4 - Added support for inapplicable actions and fixed a minor logical bug in the universal effects.
+* version 3.3.0 - Added support for nested action schemas including universal preconditions.
```

### Comparing `pddl-plus-parser-3.2.2/pddl_plus_parser.egg-info/SOURCES.txt` & `pddl-plus-parser-3.3.0/pddl_plus_parser.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,35 @@
 pddl_plus_parser/exporters/domain_exporter.py
 pddl_plus_parser/exporters/enhsp_output_parser.py
 pddl_plus_parser/exporters/ff_output_parser.py
 pddl_plus_parser/exporters/numeric_trajectory_exporter.py
 pddl_plus_parser/exporters/problem_exporter.py
 pddl_plus_parser/lisp_parsers/__init__.py
 pddl_plus_parser/lisp_parsers/domain_parser.py
+pddl_plus_parser/lisp_parsers/effects_parser.py
 pddl_plus_parser/lisp_parsers/parsing_utils.py
 pddl_plus_parser/lisp_parsers/pddl_parser_types.py
 pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
+pddl_plus_parser/lisp_parsers/preconditions_parser.py
 pddl_plus_parser/lisp_parsers/problem_parser.py
 pddl_plus_parser/lisp_parsers/trajectory_parser.py
 pddl_plus_parser/models/__init__.py
 pddl_plus_parser/models/action_call.py
 pddl_plus_parser/models/conditional_effect.py
+pddl_plus_parser/models/grounded_effect.py
+pddl_plus_parser/models/grounded_precondition.py
+pddl_plus_parser/models/grounding_utils.py
 pddl_plus_parser/models/numerical_expression.py
 pddl_plus_parser/models/observation.py
 pddl_plus_parser/models/pddl_action.py
 pddl_plus_parser/models/pddl_domain.py
 pddl_plus_parser/models/pddl_function.py
 pddl_plus_parser/models/pddl_object.py
 pddl_plus_parser/models/pddl_operator.py
+pddl_plus_parser/models/pddl_precondition.py
 pddl_plus_parser/models/pddl_predicate.py
 pddl_plus_parser/models/pddl_problem.py
 pddl_plus_parser/models/pddl_state.py
 pddl_plus_parser/models/pddl_type.py
 pddl_plus_parser/models/universal_quantifier.py
 pddl_plus_parser/multi_agent/__init__.py
 pddl_plus_parser/multi_agent/common.py
@@ -55,14 +61,16 @@
 tests/lisp_parsers_tests/consts.py
 tests/lisp_parsers_tests/domain_parser_test.py
 tests/lisp_parsers_tests/pddl_tokenizer_test.py
 tests/lisp_parsers_tests/problem_parser_test.py
 tests/lisp_parsers_tests/trajectory_parser_test.py
 tests/models_tests/__init__.py
 tests/models_tests/consts.py
+tests/models_tests/grounded_effect_test.py
+tests/models_tests/grounded_precondition_test.py
 tests/models_tests/numerical_expression_test.py
 tests/models_tests/operator_test.py
 tests/models_tests/pddl_function_test.py
 tests/multi_agent_tests/__init__.py
 tests/multi_agent_tests/consts.py
 tests/multi_agent_tests/multi_agent_domain_converter_test.py
 tests/multi_agent_tests/multi_agent_problem_converter_test.py
```

### Comparing `pddl-plus-parser-3.2.2/tests/exporters_tests/numeric_trajectory_exporter_test.py` & `pddl-plus-parser-3.3.0/tests/exporters_tests/numeric_trajectory_exporter_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,25 +184,20 @@
     assert "(lift hoist1 crate3 pallet1 distributor0)" in exportable_triplets[5]
 
 
 def test_export_numeric_trajectory_with_faulty_action_creates_but_does_not_duplicate_the_initial_state_multiple_times(
         minecraft_trajectory_exporter: TrajectoryExporter, minecraft_problem: Problem):
     triplets = minecraft_trajectory_exporter.parse_plan(minecraft_problem, TEST_MINECRAFT_PLAN_PATH)
     exportable_triplets = minecraft_trajectory_exporter.export(triplets)
-    for triplet in exportable_triplets:
-        print(triplet)
+    assert len([triplet for triplet in exportable_triplets if triplet.startswith("((:init")]) == 1
 
 
-    # pre_state = exportable_triplets[4]
-    # post_state = exportable_triplets[6]
-    # assert pre_state == post_state
-    # assert "(lift hoist1 crate3 pallet1 distributor0)" in exportable_triplets[5]
-
 def test_export_trajectory_with_conditional_effects(
         conditional_trajectory_exporter: TrajectoryExporter, conditional_problem: Problem):
     triplets = conditional_trajectory_exporter.parse_plan(conditional_problem, TEST_CONDITIONAL_PLAN_PATH)
     try:
         exportable_triplets = conditional_trajectory_exporter.export(triplets)
         for triplet in exportable_triplets:
             print(triplet)
+
     except Exception as e:
         pytest.fail("Exporting a trajectory with conditional effects failed with the following error: " + str(e))
```

### Comparing `pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/consts.py` & `pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 PLANT_WATERING_DOMAIN = Path(CWD, "plant_watering_domain.pddl")
 
 WOODWORKING_COMBINED_DOMAIN_PATH = Path(CWD) / "woodworking_combined_domain.pddl"
 WOODWORKING_COMBINED_PROBLEM_PATH = Path(CWD) / "woodworking_combined_problem.pddl"
 WOODWORKING_COMBINED_TRAJECTORY_PATH = Path(CWD) / "ma_woodworking_trajectory.trajectory"
 
+UMT2_DOMAIN_PATH = Path(CWD) / "UMT2_domain.pddl"
+
 
 TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN = """((on ?c1 - card ?c2 - cardposition)
     (clear ?c - cardposition)
     (in-play ?c - card)
     (current-deal ?d - deal)
     (CAN-CONTINUE-GROUP ?c1 - card ?c2 - cardposition)
     (CAN-BE-PLACED-ON ?c1 - card ?c2 - card)
```

### Comparing `pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/domain_parser_test.py` & `pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/domain_parser_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from pytest import fixture, raises
+from pytest import fixture, raises, fail
 
 from pddl_plus_parser.lisp_parsers import DomainParser, PDDLTokenizer
-from pddl_plus_parser.models import PDDLType, Predicate, Action
+from pddl_plus_parser.models import PDDLType, Predicate, Action, CompoundPrecondition
 from tests.lisp_parsers_tests.consts import TEST_PARSING_FILE_PATH, TEST_WOODWORKING_DOMAIN_PATH, \
     TEST_NUMERIC_DEPOT_DOMAIN_PATH, PLANT_WATERING_DOMAIN, TEST_CONSTANTS_FOR_CONDITIONAL_DOMAIN, \
     TEST_TYPES_FOR_CONDITIONAL_DOMAIN, TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN, SPIDER_DOMAIN_PATH, \
-    TYPES_FOR_UNIVERSAL_CONDITIONAL_DOMAIN, TEST_PREDICATES_FOR_UNIVERSAL_QUANTIFIER_DOMAIN
+    TYPES_FOR_UNIVERSAL_CONDITIONAL_DOMAIN, TEST_PREDICATES_FOR_UNIVERSAL_QUANTIFIER_DOMAIN, UMT2_DOMAIN_PATH
 
 test_types_with_no_parent = ['acolour', 'awood', 'woodobj', 'machine', 'surface', 'treatmentstatus', 'aboardsize',
                              'apartsize']
 
 nested_types = ['acolour', 'awood', 'woodobj', 'machine', 'surface', 'treatmentstatus', 'aboardsize', 'apartsize',
                 '-', 'object', 'highspeed-saw', 'saw', 'glazer', 'grinder', 'immersion-varnisher', 'planer',
                 'spray-varnisher', '-', 'machine', 'board', 'part', '-', 'woodobj']
@@ -109,31 +109,31 @@
     assert list(domain_consts.keys()) == ['small', 'medium', 'large', 'highspeed-saw', 'varnished', 'glazed',
                                           'untreated', 'colourfragments', 'natural', 'verysmooth', 'smooth', 'rough']
 
 
 def test_parse_predicate_with_legal_predicate_data_is_successful(domain_parser: DomainParser):
     domain_types = domain_parser.parse_types(nested_types)
     test_predicate = ['available', '?obj', '-', 'woodobj']
-    predicate = domain_parser.parse_predicate(test_predicate, domain_types)
+    predicate = domain_parser._parse_predicate(test_predicate, domain_types)
     assert predicate.name == "available"
     assert "?obj" in predicate.signature
 
 
 def test_parse_predicate_with_illegal_predicate_data_raises_error(domain_parser: DomainParser):
     domain_types = domain_parser.parse_types(nested_types)
     with raises(SyntaxError):
         test_predicate = ['available', '?obj', 'woodobj']
-        domain_parser.parse_predicate(test_predicate, domain_types)
+        domain_parser._parse_predicate(test_predicate, domain_types)
 
 
 def test_parse_predicate_with_no_parameters_returns_predicate_object_with_only_name_and_empty_signature(
         domain_parser: DomainParser):
     domain_types = domain_parser.parse_types(nested_types)
     test_predicate_no_params_ast = ["ok"]
-    predicate = domain_parser.parse_predicate(test_predicate_no_params_ast, domain_types)
+    predicate = domain_parser._parse_predicate(test_predicate_no_params_ast, domain_types)
     assert predicate is not None
     assert predicate.name == "ok"
     assert len(predicate.signature) == 0
 
 
 def test_parse_predicates_with_single_predicate_returns_predicates_dictionary_correctly(domain_parser: DomainParser):
     domain_types = domain_parser.parse_types(nested_types)
@@ -204,15 +204,15 @@
     domain_types = domain_parser.parse_types(nested_types)
     domain_consts = domain_parser.parse_constants(test_constants, domain_types)
     domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
     domain_functions = {}  # Functions are irrelevant for this case.
     action = domain_parser.parse_action(action_tokens, domain_types, domain_functions, domain_predicates, domain_consts)
 
     assert action.name == "cut-board-medium"
-    assert action.inequality_preconditions == {("?size_before", "?size_after")}
+    assert action.preconditions.root.inequality_preconditions == {("?size_before", "?size_after")}
 
 
 def test_parse_action_with_equality_precondition_adds_the_lifted_objects_correctly(domain_parser: DomainParser):
     test_action_str = """(cut-board-medium
 	:parameters   (?m - highspeed-saw ?b - board ?p - part ?w - awood ?surface - surface ?size_before - aboardsize ?s1 - aboardsize ?size_after - aboardsize)
 	:precondition (and (unused ?p) (= ?size_before ?size_after) (goalsize ?p medium) (in-highspeed-saw ?b ?m) (wood ?b ?w) (surface-condition ?b ?surface) (boardsize ?b ?size_before) (boardsize-successor ?size_after ?s1) (boardsize-successor ?s1 ?size_before))
 	:effect       (and (boardsize ?b ?size_after) (available ?p) (surface-condition ?p ?surface) (treatment ?p untreated) (wood ?p ?w) (colour ?p natural) (not (unused ?p))))"""
@@ -221,15 +221,15 @@
     domain_types = domain_parser.parse_types(nested_types)
     domain_consts = domain_parser.parse_constants(test_constants, domain_types)
     domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
     domain_functions = {}  # Functions are irrelevant for this case.
     action = domain_parser.parse_action(action_tokens, domain_types, domain_functions, domain_predicates, domain_consts)
 
     assert action.name == "cut-board-medium"
-    assert action.equality_preconditions == {("?size_before", "?size_after")}
+    assert action.preconditions.root.equality_preconditions == {("?size_before", "?size_after")}
 
 
 def test_parse_action_with_boolean_action_type_returns_action_data_correctly(domain_parser: DomainParser):
     test_action_str = """(do-spray-varnish
 	:parameters   (?m - spray-varnisher ?x - part ?newcolour - acolour ?surface - surface)
 	:precondition (and (available ?x) (has-colour ?m ?newcolour) (surface-condition ?x ?surface) (is-smooth ?surface) (treatment ?x untreated))
 	:effect       (and (treatment ?x varnished) (colour ?x ?newcolour) (not (treatment ?x untreated)) (not (colour ?x natural))))"""
@@ -244,15 +244,14 @@
     assert action.name == "do-spray-varnish"
     assert action.signature == {
         "?m": PDDLType("spray-varnisher"),
         "?x": PDDLType("part"),
         "?newcolour": PDDLType("acolour"),
         "?surface": PDDLType("surface"),
     }
-    assert action.negative_preconditions == set()
     expected_preconditions = {
         Predicate(name="available", signature={"?x": PDDLType("part")}),
         Predicate(name="has-colour", signature={
             "?m": PDDLType("spray-varnisher"),
             "?newcolour": PDDLType("acolour")
         }),
         Predicate(name="surface-condition", signature={
@@ -264,49 +263,21 @@
         }),
         Predicate(name="treatment", signature={
             "?x": PDDLType("part"),
             "untreated": PDDLType("treatmentstatus")
         }),
 
     }
-    assert len(action.positive_preconditions) == len(expected_preconditions)
-    for precondition in expected_preconditions:
-        assert precondition in action.positive_preconditions
-
-    expected_add_effects = {
-        Predicate(name="colour", signature={
-            "?x": PDDLType("part"),
-            "?newcolour": PDDLType("acolour")
-        }),
-        Predicate(name="treatment", signature={
-            "?x": PDDLType("part"),
-            "varnished": PDDLType("treatmentstatus")
-        })
-    }
-    assert len(action.add_effects) == len(expected_add_effects)
-    for effect in expected_add_effects:
-        assert effect in action.add_effects
-
-    expected_delete_effects = {
-        Predicate(name="treatment", signature={
-            "?x": PDDLType("part"),
-            "untreated": PDDLType("treatmentstatus")
-        }),
-        Predicate(name="colour", signature={
-            "?x": PDDLType("part"),
-            "natural": PDDLType("acolour")
-        })
-    }
-
-    assert len(action.add_effects) == len(expected_delete_effects)
-    for effect in expected_delete_effects:
-        assert effect in action.delete_effects
+    assert expected_preconditions.issubset(action.preconditions.root.operands)
+    assert action.preconditions.root.operands.issubset(expected_preconditions)
+    print()
+    print(str(action.preconditions))
 
 
-def test_parse_effects_with_conditional_effects_with_one_condition_and_one_effect_parse_correctly(
+def test_parse_action_with_conditional_effects_with_one_condition_and_one_effect_parse_correctly(
         domain_parser: DomainParser):
     conditional_effects = """(and (when
             (not (CAN-CONTINUE-GROUP ?c ?to))
             (make-unmovable ?to)
     ))"""
     types_tokens = PDDLTokenizer(pddl_str=TEST_TYPES_FOR_CONDITIONAL_DOMAIN).parse()
     predicate_tokens = PDDLTokenizer(pddl_str=TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN).parse()
@@ -330,15 +301,15 @@
     conditional_effect = new_action.conditional_effects.pop()
     assert conditional_effect is not None
     print(str(conditional_effect))
     assert str(
         conditional_effect) == "(when (and (not (CAN-CONTINUE-GROUP ?c ?to))) (and (make-unmovable ?to)))".lower()
 
 
-def test_parse_effects_with_conditional_effects_with_one_condition_and_two_effects_parse_correctly(
+def test_parse_action_with_conditional_effects_with_one_condition_and_two_effects_parse_correctly(
         domain_parser: DomainParser):
     conditional_effects = """(and (when
             (not (can-continue-group ?c ?to))
             (and
                 (currently-updating-unmovable)
                 (make-unmovable ?to)
             )
@@ -360,24 +331,24 @@
                                 new_action=new_action,
                                 domain_types=domain_types,
                                 domain_functions=domain_functions,
                                 domain_predicates=domain_predicates,
                                 domain_constants=domain_consts)
     conditional_effect = new_action.conditional_effects.pop()
     assert conditional_effect is not None
-    negative_condition = conditional_effect.negative_conditions.pop()
-    add_effects = conditional_effect.add_effects
-    assert negative_condition.untyped_representation == "(can-continue-group ?c ?to)"
+    negative_condition = str(conditional_effect.antecedents)
+    add_effects = conditional_effect.discrete_effects
+    assert negative_condition == "(and (not (can-continue-group ?c ?to)))"
     print([eff.untyped_representation for eff in add_effects])
     assert len(add_effects) == 2
     effects_str = {effect.untyped_representation for effect in add_effects}
     assert effects_str == {"(currently-updating-unmovable )", "(make-unmovable ?to)"}
 
 
-def test_parse_effects_with_conditional_effects_with_two_conditions_and_two_effects_parse_correctly(
+def test_parse_action_with_conditional_effects_with_two_conditions_and_two_effects_parse_correctly(
         domain_parser: DomainParser):
     conditional_effects = """(and (when
             (and (can-continue-group ?c ?to) (not (can-continue-group ?c ?from)))
             (and (currently-updating-unmovable) (make-unmovable ?to))))"""
     types_tokens = PDDLTokenizer(pddl_str=TEST_TYPES_FOR_CONDITIONAL_DOMAIN).parse()
     predicate_tokens = PDDLTokenizer(pddl_str=TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN).parse()
     constants_tokens = PDDLTokenizer(pddl_str=TEST_CONSTANTS_FOR_CONDITIONAL_DOMAIN).parse()
@@ -395,22 +366,22 @@
                                 new_action=new_action,
                                 domain_types=domain_types,
                                 domain_functions=domain_functions,
                                 domain_predicates=domain_predicates,
                                 domain_constants=domain_consts)
     conditional_effect = new_action.conditional_effects.pop()
     assert conditional_effect is not None
-    negative_condition = conditional_effect.negative_conditions.pop()
-    positive_condition = conditional_effect.positive_conditions.pop()
-    add_effects = conditional_effect.add_effects
-    assert negative_condition.untyped_representation == "(can-continue-group ?c ?from)"
-    assert positive_condition.untyped_representation == "(can-continue-group ?c ?to)"
+    antecedents = str(conditional_effect.antecedents)
+    add_effects = conditional_effect.discrete_effects
+    assert "(not (can-continue-group ?c ?from))" in antecedents
+    assert "(can-continue-group ?c ?to)" in antecedents
     assert len(add_effects) == 2
     effects_str = {effect.untyped_representation for effect in add_effects}
     assert effects_str == {"(currently-updating-unmovable )", "(make-unmovable ?to)"}
+    print(conditional_effect)
 
 
 def test_parse_action_with_conditional_effects_succeeds_in_parsing_action_and_returns_correct_fields(
         domain_parser: DomainParser):
     test_action_with_conditional_effects = """(deal-card
     :parameters (?c - card ?from - cardposition ?fromdeal - deal ?to - card ?totableau - tableau)
     :precondition
@@ -455,28 +426,82 @@
     domain_functions = {}  # Functions are irrelevant for this case.
     action = domain_parser.parse_action(action_tokens, domain_types, domain_functions, domain_predicates, domain_consts)
     assert action is not None
     assert action.name == "deal-card"
     assert action.conditional_effects is not None
 
 
-def test_parse_conditional_effect_raises_error_if_conditional_effect_not_in_correct_format(
+def test_parse_action_with_conditional_effect_raises_error_if_conditional_effect_not_in_correct_format(
         domain_parser: DomainParser):
-    conditional_effects_str = """
-    (when (and (currently-updating-unmovable) (make-unmovable ?to)))"""
+    conditional_effects_str = """(and 
+    (when (and (currently-updating-unmovable) (make-unmovable ?to))))"""
     types_tokens = PDDLTokenizer(pddl_str=TEST_TYPES_FOR_CONDITIONAL_DOMAIN).parse()
     constants_tokens = PDDLTokenizer(pddl_str=TEST_CONSTANTS_FOR_CONDITIONAL_DOMAIN).parse()
+    predicate_tokens = PDDLTokenizer(pddl_str=TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN).parse()
     conditional_effect_tokens = PDDLTokenizer(pddl_str=conditional_effects_str).parse()
     domain_types = domain_parser.parse_types(types_tokens)
     domain_consts = domain_parser.parse_constants(constants_tokens, domain_types)
+    domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
     domain_functions = {}  # Functions are irrelevant for this case.
     action = Action()
     action.name = "deal-card"
+    action.signature = {"?c": domain_types["card"], "?from": domain_types["cardposition"],
+                        "?fromdeal": domain_types["deal"], "?to": domain_types["card"],
+                        "?totableau": domain_types["tableau"]}
     with raises(SyntaxError):
-        domain_parser.parse_conditional_effect(conditional_effect_tokens, action, domain_functions, domain_consts)
+        domain_parser.parse_effects(conditional_effect_tokens, action, domain_types, domain_functions,
+                                    domain_predicates, domain_consts)
+
+
+def test_parse_action_with_universal_quantifier_in_preconditions_returns_correct_universal_precondition(
+        domain_parser: DomainParser):
+    test_action_with_universal_precondition = """
+    (stop
+      :parameters (?f - floor)
+      :precondition (and (forall (?p - passenger) (and (lift-at ?f) (not (boarded ?p)))))
+      :effect (and (not (lift-at ?f)))
+    ))"""
+    types_tokens = PDDLTokenizer(pddl_str=TYPES_FOR_UNIVERSAL_CONDITIONAL_DOMAIN).parse()
+    predicate_tokens = PDDLTokenizer(pddl_str=TEST_PREDICATES_FOR_UNIVERSAL_QUANTIFIER_DOMAIN).parse()
+    action_tokens = PDDLTokenizer(pddl_str=test_action_with_universal_precondition).parse()
+    domain_types = domain_parser.parse_types(types_tokens)
+    domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
+    domain_functions = {}
+    action = domain_parser.parse_action(action_ast=action_tokens, domain_types=domain_types,
+                                        domain_functions=domain_functions, domain_predicates=domain_predicates)
+    assert action is not None
+    universal_precondition = action.preconditions.root.operands.pop()
+    assert universal_precondition is not None
+    assert len(universal_precondition.operands) == 2
+    assert universal_precondition.quantified_parameter == "?p"
+    assert universal_precondition.quantified_type == domain_types["passenger"]
+
+
+def test_parse_action_with_both_universal_preconditions_and_regular_ones_creates_correct_preconditions(
+        domain_parser: DomainParser):
+    test_action_with_universal_precondition = """
+    (stop
+      :parameters (?f1 - floor ?f2 - floor)
+      :precondition (and (above ?f1 ?f2) (forall (?p - passenger) (and (lift-at ?f1) (not (boarded ?p)))))
+      :effect (and (not (lift-at ?f1)))
+    ))"""
+    types_tokens = PDDLTokenizer(pddl_str=TYPES_FOR_UNIVERSAL_CONDITIONAL_DOMAIN).parse()
+    predicate_tokens = PDDLTokenizer(pddl_str=TEST_PREDICATES_FOR_UNIVERSAL_QUANTIFIER_DOMAIN).parse()
+    action_tokens = PDDLTokenizer(pddl_str=test_action_with_universal_precondition).parse()
+    domain_types = domain_parser.parse_types(types_tokens)
+    domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
+    domain_functions = {}
+    action = domain_parser.parse_action(action_ast=action_tokens, domain_types=domain_types,
+                                        domain_functions=domain_functions, domain_predicates=domain_predicates)
+    assert action is not None
+    preconditions = action.preconditions.root.operands
+    assert preconditions is not None
+    assert len(preconditions) == 2
+    for op, cond in action.preconditions:
+        print(str(cond))
 
 
 def test_parse_action_with_universal_quantifier_in_conditional_effect_returns_correct_universal_quantifier_data(
         domain_parser: DomainParser):
     test_action_with_universal_quantifier = """
     (stop
       :parameters (?f - floor)
@@ -499,18 +524,17 @@
     assert action is not None
     universal_effects = action.universal_effects
     assert len(universal_effects) == 1
     universal_effect = universal_effects.pop()
     assert universal_effect.quantified_parameter == "?p"
     assert universal_effect.quantified_type.name == "passenger"
     conditional_effect = universal_effect.conditional_effects.pop()
-    assert len(conditional_effect.add_effects) == 1
-    assert len(conditional_effect.delete_effects) == 1
-    assert len(conditional_effect.positive_conditions) == 2
-    print(str(universal_effect))
+    assert len(conditional_effect.discrete_effects) == 2
+    antecedents = conditional_effect.antecedents.root.operands
+    assert len(antecedents) == 2
 
 
 def test_parse_action_with_two_universal_quantifiers_in_effect_extract_all_universal_effects(
         domain_parser: DomainParser):
     test_action_with_universal_quantifier = """
     (stop
       :parameters (?f - floor)
@@ -533,14 +557,52 @@
     action = domain_parser.parse_action(action_ast=action_tokens, domain_types=domain_types,
                                         domain_functions=domain_functions, domain_predicates=domain_predicates)
     assert action is not None
     universal_effects = action.universal_effects
     assert len(universal_effects) == 2
 
 
+def test_parse_simple_action_with_only_numeric_preconditions_and_effects_extracts_the_correct_preconditions_tree(
+        domain_parser: DomainParser):
+    test_simple_types = """(place locatable - object
+	    depot distributor - place
+        truck hoist surface - locatable
+        pallet crate - surface)"""
+    test_simple_predicates = """((at ?x - locatable ?y - place) 
+             (on ?x - crate ?y - surface)
+             (in ?x - crate ?y - truck)
+             (lifting ?x - hoist ?y - crate)
+             (available ?x - hoist)
+             (clear ?x - surface))"""
+    test_domain_simple_functions = """((load_limit ?t - truck) 
+	(current_load ?t - truck) 
+	(weight ?c - crate)
+	(fuel-cost))
+    """
+    test_simple_numeric_action = """(Load
+        :parameters (?x - hoist ?y - crate ?z - truck ?p - place)
+        :precondition (and (<= (+ (current_load ?z) (weight ?y)) (load_limit ?z)))
+        :effect (and (not (lifting ?x ?y)) (in ?y ?z) (available ?x)
+                (increase (current_load ?z) (weight ?x))))"""
+    types_tokens = PDDLTokenizer(pddl_str=test_simple_types).parse()
+    functions_tokens = PDDLTokenizer(pddl_str=test_domain_simple_functions).parse()
+    predicate_tokens = PDDLTokenizer(pddl_str=test_simple_predicates).parse()
+    action_tokens = PDDLTokenizer(pddl_str=test_simple_numeric_action).parse()
+
+    domain_types = domain_parser.parse_types(types_tokens)
+    domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
+    domain_functions = domain_parser.parse_functions(functions_tokens, domain_types)
+
+    action = domain_parser.parse_action(action_tokens, domain_types, domain_functions, domain_predicates)
+    assert len(action.preconditions.root.operands) == 1
+    precond_expression = action.preconditions.root.operands.pop()
+    assert precond_expression.root.id == "<="
+    assert precond_expression.root.height == 2
+
+
 def test_parse_simple_action_with_numeric_preconditions_and_effects_extracts_the_calculation_tree_correctly(
         domain_parser: DomainParser):
     test_simple_types = """(place locatable - object
 	    depot distributor - place
         truck hoist surface - locatable
         pallet crate - surface)"""
     test_simple_predicates = """((at ?x - locatable ?y - place) 
@@ -566,18 +628,15 @@
     action_tokens = PDDLTokenizer(pddl_str=test_simple_numeric_action).parse()
 
     domain_types = domain_parser.parse_types(types_tokens)
     domain_predicates = domain_parser.parse_predicates(predicate_tokens, domain_types)
     domain_functions = domain_parser.parse_functions(functions_tokens, domain_types)
 
     action = domain_parser.parse_action(action_tokens, domain_types, domain_functions, domain_predicates)
-    assert len(action.numeric_preconditions) == 1
-    precond_expression = action.numeric_preconditions.pop()
-    assert precond_expression.root.id == "<="
-    assert precond_expression.root.height == 2
+    assert len(action.preconditions.root.operands) == 4
 
     assert len(action.numeric_effects) == 1
     effect_expression = action.numeric_effects.pop()
     assert effect_expression.root.id == "increase"
     assert effect_expression.root.height == 1
 
 
@@ -614,19 +673,18 @@
 
 
 def test_parse_action_with_function_equality_precondition_sets_a_new_numeric_precondition():
     domain_parser = DomainParser(PLANT_WATERING_DOMAIN)
     domain = domain_parser.parse_domain()
     assert domain is not None
     assert len(domain.actions) == 10
-    assert len(domain.actions["pour"].numeric_preconditions) == 5
+    assert len(domain.actions["pour"].preconditions.root.operands) == 5
     for action in domain.actions.values():
         print(action.name)
-        for numeric_precond in action.numeric_preconditions:
-            print(str(numeric_precond))
+        print(action.preconditions)
 
 
 def test_parse_preconditions_with_action_with_disjunctive_preconditions_extracts_different_set_of_preconditions():
     test_action_str = """(lift
 	:parameters (?x - hoist ?y - crate ?z - surface ?p - place)
 	:precondition (and (on ?y ?z) (at ?y ?p) (clear ?y) (at ?x ?p) (available ?x)
 				(or (and		
@@ -642,18 +700,53 @@
             (increase (fuel-cost ) 1.0)
     ))"""
     domain_parser = DomainParser(TEST_NUMERIC_DEPOT_DOMAIN_PATH)
     domain = domain_parser.parse_domain()
     action_tokens = PDDLTokenizer(pddl_str=test_action_str).parse()
     action = domain_parser.parse_action(action_tokens, domain.types, domain.functions, domain.predicates,
                                         domain.constants)
-    disjunctive_preconditions = action.disjunctive_numeric_preconditions
-    assert len(disjunctive_preconditions) == 2
-    assert len(disjunctive_preconditions[0]) == 2
-    assert len(disjunctive_preconditions[1]) == 3
-    print(str(action))
+    preconditions = action.preconditions.root
+    assert "(>= (+ (* (fuel-cost ) -0.01) 0.78) 0.0)" in str(preconditions)
+    assert "(>= (+ (* (fuel-cost ) -0.02) 1.01) 0.0)" in str(preconditions)
+    assert "(>= (+ (* (fuel-cost ) 0.01) -1.79) 0.0)" in str(preconditions)
+    assert "(>= (+ (+ (* (weight ?y) 0.01) (* (fuel-cost ) 0.01)) -2.05) 0.0)" in str(preconditions)
+    assert "(>= (+ (* (fuel-cost ) -0.01) 0.78) 0.0)" in str(preconditions)
+    assert "or" in str(preconditions)
+    print(str(preconditions))
+
+
+def test_parse_preconditions_with_action_with_universal_preconditions_works():
+    test_action_str = """(lift
+	:parameters (?x - hoist ?y - crate ?z - surface ?p - place)
+	:precondition (and  (at ?y ?p)
+					    (not (lifting ?x ?y))
+					    (forall (?y1 - crate) (and (at ?y1 ?p)))
+				        (clear ?z))
+        :effect (and (clear ?z) (lifting ?x ?y) (not (available ?x)) (not (on ?y ?z)) (not (at ?y ?p))
+            (increase (fuel-cost ) 1.0)
+    ))"""
+    domain_parser = DomainParser(TEST_NUMERIC_DEPOT_DOMAIN_PATH)
+    domain = domain_parser.parse_domain()
+    action_tokens = PDDLTokenizer(pddl_str=test_action_str).parse()
+    action = domain_parser.parse_action(action_tokens, domain.types, domain.functions, domain.predicates,
+                                        domain.constants)
+    preconditions = action.preconditions.root
+    print(str(preconditions))
 
 
 def test_parse_domain_with_domain_with_conditional_effects_not_fail():
     domain_parser = DomainParser(SPIDER_DOMAIN_PATH)
     domain = domain_parser.parse_domain()
     print(str(domain))
+
+
+def test_parse_domain_nested_action_schema_does_not_fail():
+    domain_parser = DomainParser(UMT2_DOMAIN_PATH)
+    try:
+        domain = domain_parser.parse_domain()
+        for action in domain.actions.values():
+            print(action.name)
+            print(action.preconditions)
+            print()
+    except Exception:
+        fail("Parsing domain with nested action schema failed.")
+
```

### Comparing `pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/problem_parser_test.py` & `pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/problem_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/lisp_parsers_tests/trajectory_parser_test.py` & `pddl-plus-parser-3.3.0/tests/lisp_parsers_tests/trajectory_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/models_tests/numerical_expression_test.py` & `pddl-plus-parser-3.3.0/tests/models_tests/numerical_expression_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/models_tests/pddl_function_test.py` & `pddl-plus-parser-3.3.0/tests/models_tests/pddl_function_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/multi_agent_tests/consts.py` & `pddl-plus-parser-3.3.0/tests/multi_agent_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/multi_agent_tests/multi_agent_domain_converter_test.py` & `pddl-plus-parser-3.3.0/tests/multi_agent_tests/multi_agent_domain_converter_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 def test_locate_domains_returns_all_private_and_public_predicates(domain_converter: MultiAgentDomainsConverter):
     """Test that the locate_domains method returns a domain with all private and public predicates."""
     domain = domain_converter.locate_domains()
     assert "grind-treatment-change" in domain.predicates
     assert "boardsize-successor" in domain.predicates
-    assert len(domain.predicates) == 14
+    assert len(domain.predicates) == 14 + 1 # 14 original predicates + 1 dummy predicate
 
 
 def test_locate_domains_returns_agents_actions(domain_converter: MultiAgentDomainsConverter):
     """Test that the locate_domains method returns a domain with all agents' actions."""
     domain = domain_converter.locate_domains()
     assert "do-grind" in domain.actions
     assert "do-saw-small" in domain.actions
@@ -38,8 +38,8 @@
     assert "do-saw-large" in domain.actions
 
 
 def test_locate_domains_returns_actions_with_correct_information(blocks_domain_converter: MultiAgentDomainsConverter):
     """Test that the locate_domains method returns a domain with all agents' actions."""
     domain = blocks_domain_converter.locate_domains()
     assert "put-down" in domain.actions
-    assert len(domain.actions["put-down"].positive_preconditions) > 0
+    assert len(domain.actions["put-down"].preconditions.root.operands) > 0
```

### Comparing `pddl-plus-parser-3.2.2/tests/multi_agent_tests/multi_agent_problem_converter_test.py` & `pddl-plus-parser-3.3.0/tests/multi_agent_tests/multi_agent_problem_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py` & `pddl-plus-parser-3.3.0/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.2.2/tests/multi_agent_tests/single_agent_plan_converter_test.py` & `pddl-plus-parser-3.3.0/tests/multi_agent_tests/single_agent_plan_converter_test.py`

 * *Files identical despite different names*

