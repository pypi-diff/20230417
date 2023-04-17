# Comparing `tmp/retentioneering-3.0.0b0.tar.gz` & `tmp/retentioneering-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retentioneering-3.0.0b0.tar", max compression
+gzip compressed data, was "retentioneering-3.0.0b1.tar", max compression
```

## Comparing `retentioneering-3.0.0b0.tar` & `retentioneering-3.0.0b1.tar`

### file list

```diff
@@ -1,124 +1,123 @@
--rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0b0/LICENSE
--rw-r--r--   0        0        0     2065 2023-03-14 09:27:23.150888 retentioneering-3.0.0b0/pyproject.toml
--rw-r--r--   0        0        0      393 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/__init__.py
--rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/backend/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/backend/callback/__init__.py
--rw-r--r--   0        0        0      487 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/backend/callback/list_dataprocessors.py
--rw-r--r--   0        0        0     5290 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/backend/callback/mock_list_dataprocessor.py
--rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/backend/jupiter_server.py
--rw-r--r--   0        0        0     5293 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/backend/server_manager.py
--rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0b0/retentioneering/constants/__init__.py
--rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0b0/retentioneering/constants/constants.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/data_processor/__init__.py
--rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0b0/retentioneering/data_processor/data_processor.py
--rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0b0/retentioneering/data_processor/registry.py
--rw-r--r--   0        0        0      841 2023-01-16 14:26:06.541078 retentioneering-3.0.0b0/retentioneering/data_processors_lib/__init__.py
--rw-r--r--   0        0        0     4717 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/collapse_loops.py
--rw-r--r--   0        0        0     3224 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/delete_users_by_path_length.py
--rw-r--r--   0        0        0     2185 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/filter_events.py
--rw-r--r--   0        0        0     3207 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/group_events.py
--rw-r--r--   0        0        0     4565 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/lost_users.py
--rw-r--r--   0        0        0     3963 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/negative_target.py
--rw-r--r--   0        0        0     3060 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/new_users.py
--rw-r--r--   0        0        0     3885 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/positive_target.py
--rw-r--r--   0        0        0     1760 2023-03-07 11:03:25.184838 retentioneering-3.0.0b0/retentioneering/data_processors_lib/rename.py
--rw-r--r--   0        0        0     8234 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/split_sessions.py
--rw-r--r--   0        0        0     2331 2023-01-16 14:26:06.544412 retentioneering-3.0.0b0/retentioneering/data_processors_lib/start_end_events.py
--rw-r--r--   0        0        0     6437 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/truncate_path.py
--rw-r--r--   0        0        0     5479 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/data_processors_lib/truncated_events.py
--rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0b0/retentioneering/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0b0/retentioneering/datasets/data/__init__.py
--rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0b0/retentioneering/datasets/data/ab_test_demo.csv
--rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0b0/retentioneering/datasets/data/simple-onlineshop.csv
--rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0b0/retentioneering/datasets/load.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/edgelist/__init__.py
--rw-r--r--   0        0        0     3689 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/edgelist/edgelist.py
--rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/eventstream/__init__.py
--rw-r--r--   0        0        0    40489 2023-03-14 09:27:23.150888 retentioneering-3.0.0b0/retentioneering/eventstream/eventstream.py
--rw-r--r--   0        0        0      719 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/__init__.py
--rw-r--r--   0        0        0     1603 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/collapse_loops_helper.py
--rw-r--r--   0        0        0     1451 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/delete_users_by_path_length_helper.py
--rw-r--r--   0        0        0     1094 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/filter_helper.py
--rw-r--r--   0        0        0     1471 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/group_helper.py
--rw-r--r--   0        0        0     1434 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/lost_users_helper.py
--rw-r--r--   0        0        0     1473 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/negative_target.py
--rw-r--r--   0        0        0     1249 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/new_users_helper.py
--rw-r--r--   0        0        0     1473 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/positive_target.py
--rw-r--r--   0        0        0      692 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/rename_helper.py
--rw-r--r--   0        0        0     1913 2023-03-14 09:18:13.137154 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/split_session_helper.py
--rw-r--r--   0        0        0     1138 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/start_end_helper.py
--rw-r--r--   0        0        0     1685 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/truncate_path_helper.py
--rw-r--r--   0        0        0     1584 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/eventstream/helpers/truncated_events_helper.py
--rw-r--r--   0        0        0     3939 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/eventstream/schema.py
--rw-r--r--   0        0        0     2351 2023-03-13 11:05:55.223966 retentioneering-3.0.0b0/retentioneering/eventstream/types.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/exceptions/__init__.py
--rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/exceptions/base.py
--rw-r--r--   0        0        0     1242 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/exceptions/server.py
--rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/exceptions/widget.py
--rw-r--r--   0        0        0       81 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/graph/__init__.py
--rw-r--r--   0        0        0     3562 2023-03-07 16:29:54.474509 retentioneering-3.0.0b0/retentioneering/graph/nodes.py
--rw-r--r--   0        0        0    13646 2023-03-07 16:29:54.477842 retentioneering-3.0.0b0/retentioneering/graph/p_graph.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/nodelist/__init__.py
--rw-r--r--   0        0        0     1107 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/nodelist/nodelist.py
--rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/params_model/__init__.py
--rw-r--r--   0        0        0     9934 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/params_model/params_model.py
--rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/params_model/registry.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/preprocessor/__init__.py
--rw-r--r--   0        0        0       41 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/__init__.py
--rw-r--r--   0        0        0       33 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/p_graph/__init__.py
--rw-r--r--   0        0        0     1704 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/templates/p_graph/p_graph.html
--rw-r--r--   0        0        0      700 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/templates/p_graph/show.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/transition_graph/__init__.py
--rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/transition_graph/body.html
--rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/transition_graph/full.html
--rw-r--r--   0        0        0      894 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/templates/transition_graph/init_template.py
--rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/transition_graph/inner_iframe.html
--rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/templates/transition_graph/show.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/__init__.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/clusters/__init__.py
--rw-r--r--   0        0        0    32768 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/clusters/clusters.py
--rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/clusters/segments.py
--rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/clusters/userlist.py
--rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/cohorts/__init__.py
--rw-r--r--   0        0        0    12664 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/cohorts/cohorts.py
--rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/constants/__init__.py
--rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/constants/constants.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/describe/__init__.py
--rw-r--r--   0        0        0     4560 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/describe/describe.py
--rw-r--r--   0        0        0       44 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/describe_events/__init__.py
--rw-r--r--   0        0        0     4828 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/describe_events/describe_events.py
--rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0b0/retentioneering/tooling/event_timestamp_hist/__init__.py
--rw-r--r--   0        0        0     5096 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
--rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/tooling/funnel/__init__.py
--rw-r--r--   0        0        0    12071 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/funnel/funnel.py
--rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/mixins/__init__.py
--rw-r--r--   0        0        0     1427 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/mixins/ended_events.py
--rw-r--r--   0        0        0       67 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/tooling/stattests/__init__.py
--rw-r--r--   0        0        0      167 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/tooling/stattests/constants.py
--rw-r--r--   0        0        0    11771 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/stattests/stattests.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/tooling/step_matrix/__init__.py
--rw-r--r--   0        0        0    21140 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/step_matrix/step_matrix.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/tooling/step_sankey/__init__.py
--rw-r--r--   0        0        0    24137 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/step_sankey/step_sankey.py
--rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/timedelta_hist/__init__.py
--rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/timedelta_hist/constants.py
--rw-r--r--   0        0        0    12499 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/timedelta_hist/timedelta_hist.py
--rw-r--r--   0        0        0       48 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/transition_matrix/__init__.py
--rw-r--r--   0        0        0     2012 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/transition_matrix/transition_matrix.py
--rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/typing/__init__.py
--rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/tooling/typing/transition_graph/__init__.py
--rw-r--r--   0        0        0     1260 2023-03-14 09:27:23.150888 retentioneering-3.0.0b0/retentioneering/tooling/typing/transition_graph/graph_types.py
--rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/tooling/user_lifetime_hist/__init__.py
--rw-r--r--   0        0        0     5913 2023-03-14 09:18:13.140487 retentioneering-3.0.0b0/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
--rw-r--r--   0        0        0       46 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/transition_graph/__init__.py
--rw-r--r--   0        0        0    28394 2023-03-14 09:27:23.150888 retentioneering-3.0.0b0/retentioneering/transition_graph/transition_graph.py
--rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/utils/__init__.py
--rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/utils/dict.py
--rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/utils/list.py
--rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/utils/pandas.py
--rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/utils/registry.py
--rw-r--r--   0        0        0      269 2023-01-16 14:26:06.561078 retentioneering-3.0.0b0/retentioneering/utils/singleton.py
--rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0b0/retentioneering/widget/__init__.py
--rw-r--r--   0        0        0     7265 2023-03-07 16:29:54.477842 retentioneering-3.0.0b0/retentioneering/widget/widgets.py
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 retentioneering-3.0.0b0/setup.py
--rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 retentioneering-3.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2065 2023-03-22 12:06:39.614862 retentioneering-3.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/__init__.py
+-rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/__init__.py
+-rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/callback/__init__.py
+-rw-r--r--   0        0        0      487 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/callback/list_dataprocessors.py
+-rw-r--r--   0        0        0     5290 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/callback/mock_list_dataprocessor.py
+-rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/jupiter_server.py
+-rw-r--r--   0        0        0     5293 2023-03-14 09:18:13.137154 retentioneering-3.0.0b1/retentioneering/backend/server_manager.py
+-rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/constants/__init__.py
+-rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/constants/constants.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/data_processor/__init__.py
+-rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/data_processor/data_processor.py
+-rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/data_processor/registry.py
+-rw-r--r--   0        0        0      841 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/data_processors_lib/__init__.py
+-rw-r--r--   0        0        0     4892 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/collapse_loops.py
+-rw-r--r--   0        0        0     3546 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/delete_users_by_path_length.py
+-rw-r--r--   0        0        0     2342 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/filter_events.py
+-rw-r--r--   0        0        0     3332 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/group_events.py
+-rw-r--r--   0        0        0     4696 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/lost_users.py
+-rw-r--r--   0        0        0     4055 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/negative_target.py
+-rw-r--r--   0        0        0     3173 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/new_users.py
+-rw-r--r--   0        0        0     3962 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/positive_target.py
+-rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0b1/retentioneering/data_processors_lib/rename.py
+-rw-r--r--   0        0        0     8627 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/split_sessions.py
+-rw-r--r--   0        0        0     2437 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/start_end_events.py
+-rw-r--r--   0        0        0     6571 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncate_path.py
+-rw-r--r--   0        0        0     5760 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncated_events.py
+-rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0b1/retentioneering/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0b1/retentioneering/datasets/data/__init__.py
+-rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0b1/retentioneering/datasets/data/ab_test_demo.csv
+-rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0b1/retentioneering/datasets/data/simple-onlineshop.csv
+-rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0b1/retentioneering/datasets/load.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/edgelist/__init__.py
+-rw-r--r--   0        0        0     4222 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/edgelist/edgelist.py
+-rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/eventstream/__init__.py
+-rw-r--r--   0        0        0    41037 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/eventstream.py
+-rw-r--r--   0        0        0      719 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/__init__.py
+-rw-r--r--   0        0        0     1574 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/collapse_loops_helper.py
+-rw-r--r--   0        0        0     1434 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/delete_users_by_path_length_helper.py
+-rw-r--r--   0        0        0     1137 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/filter_helper.py
+-rw-r--r--   0        0        0     1454 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/group_helper.py
+-rw-r--r--   0        0        0     1381 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/lost_users_helper.py
+-rw-r--r--   0        0        0     1410 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/negative_target.py
+-rw-r--r--   0        0        0     1196 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/new_users_helper.py
+-rw-r--r--   0        0        0     1409 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/positive_target.py
+-rw-r--r--   0        0        0      692 2023-03-14 09:18:13.137154 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/rename_helper.py
+-rw-r--r--   0        0        0     1882 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/split_session_helper.py
+-rw-r--r--   0        0        0     1009 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/start_end_helper.py
+-rw-r--r--   0        0        0     1670 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncate_path_helper.py
+-rw-r--r--   0        0        0     1517 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncated_events_helper.py
+-rw-r--r--   0        0        0     4157 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/schema.py
+-rw-r--r--   0        0        0     2389 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/types.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/exceptions/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/exceptions/base.py
+-rw-r--r--   0        0        0     1242 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/exceptions/server.py
+-rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/exceptions/widget.py
+-rw-r--r--   0        0        0       81 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/graph/__init__.py
+-rw-r--r--   0        0        0     4073 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/graph/nodes.py
+-rw-r--r--   0        0        0    13921 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/graph/p_graph.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/nodelist/__init__.py
+-rw-r--r--   0        0        0     1071 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/nodelist/nodelist.py
+-rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/params_model/__init__.py
+-rw-r--r--   0        0        0    10064 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/params_model/params_model.py
+-rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/params_model/registry.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/preprocessor/__init__.py
+-rw-r--r--   0        0        0       41 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/__init__.py
+-rw-r--r--   0        0        0       33 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/p_graph/__init__.py
+-rw-r--r--   0        0        0     1704 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/templates/p_graph/p_graph.html
+-rw-r--r--   0        0        0      700 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/templates/p_graph/show.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/__init__.py
+-rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/body.html
+-rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/full.html
+-rw-r--r--   0        0        0      894 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/init_template.py
+-rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/inner_iframe.html
+-rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/show.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/__init__.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/clusters/__init__.py
+-rw-r--r--   0        0        0    33379 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/clusters/clusters.py
+-rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/clusters/segments.py
+-rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/clusters/userlist.py
+-rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/cohorts/__init__.py
+-rw-r--r--   0        0        0    12952 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/cohorts/cohorts.py
+-rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/constants/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/constants/constants.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/describe/__init__.py
+-rw-r--r--   0        0        0     4560 2023-03-14 09:18:13.140487 retentioneering-3.0.0b1/retentioneering/tooling/describe/describe.py
+-rw-r--r--   0        0        0       44 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/describe_events/__init__.py
+-rw-r--r--   0        0        0     4828 2023-03-14 09:18:13.140487 retentioneering-3.0.0b1/retentioneering/tooling/describe_events/describe_events.py
+-rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/event_timestamp_hist/__init__.py
+-rw-r--r--   0        0        0     5552 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
+-rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/funnel/__init__.py
+-rw-r--r--   0        0        0    12195 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/funnel/funnel.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/mixins/__init__.py
+-rw-r--r--   0        0        0     1427 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/mixins/ended_events.py
+-rw-r--r--   0        0        0       67 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/stattests/__init__.py
+-rw-r--r--   0        0        0      167 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/stattests/constants.py
+-rw-r--r--   0        0        0    11911 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/stattests/stattests.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/step_matrix/__init__.py
+-rw-r--r--   0        0        0    21475 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/step_matrix/step_matrix.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/step_sankey/__init__.py
+-rw-r--r--   0        0        0    24468 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/step_sankey/step_sankey.py
+-rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/constants.py
+-rw-r--r--   0        0        0    13335 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/timedelta_hist.py
+-rw-r--r--   0        0        0       46 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/transition_graph/__init__.py
+-rw-r--r--   0        0        0    32526 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/transition_graph/transition_graph.py
+-rw-r--r--   0        0        0       48 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/transition_matrix/__init__.py
+-rw-r--r--   0        0        0     3264 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/transition_matrix/transition_matrix.py
+-rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/typing/__init__.py
+-rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/typing/transition_graph/__init__.py
+-rw-r--r--   0        0        0     1327 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/typing/transition_graph/graph_types.py
+-rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/user_lifetime_hist/__init__.py
+-rw-r--r--   0        0        0     6525 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
+-rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/__init__.py
+-rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/utils/dict.py
+-rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/list.py
+-rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/pandas.py
+-rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/utils/registry.py
+-rw-r--r--   0        0        0      269 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/singleton.py
+-rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/widget/__init__.py
+-rw-r--r--   0        0        0     7265 2023-03-07 16:29:54.477842 retentioneering-3.0.0b1/retentioneering/widget/widgets.py
+-rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 retentioneering-3.0.0b1/PKG-INFO
```

### Comparing `retentioneering-3.0.0b0/LICENSE` & `retentioneering-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/pyproject.toml` & `retentioneering-3.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retentioneering"
-version = "3.0.0b0"
+version = "3.0.0b1"
 license = "Retentioneering Software Non-Exclusive License (License)"
 description = "Product analytics and marketing optimization framework based on deep user trajectories analysis"
 authors = ["Retentioneering User Trajectory Analysis Lab <retentioneering@gmail.com>"]
 repository = "https://github.com/retentioneering/retentioneering-tools"
 packages = [
     { include = "retentioneering"}
 ]
```

### Comparing `retentioneering-3.0.0b0/retentioneering/backend/callback/mock_list_dataprocessor.py` & `retentioneering-3.0.0b1/retentioneering/backend/callback/mock_list_dataprocessor.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/backend/jupiter_server.py` & `retentioneering-3.0.0b1/retentioneering/backend/jupiter_server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/backend/server_manager.py` & `retentioneering-3.0.0b1/retentioneering/backend/server_manager.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processor/data_processor.py` & `retentioneering-3.0.0b1/retentioneering/data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processor/registry.py` & `retentioneering-3.0.0b1/retentioneering/data_processor/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/__init__.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/collapse_loops.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/collapse_loops.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,62 +7,70 @@
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 
 
 class CollapseLoopsParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.CollapseLoops`.
+    A class with parameters for :py:class:`.CollapseLoops` class.
     """
 
     suffix: Optional[Literal["loop", "count"]] = "loop"
     timestamp_aggregation_type: Literal["max", "min", "mean"] = "max"
 
 
 class CollapseLoops(DataProcessor):
     """
-    Finds ``loops`` and creates new synthetic events in each user's path who have such sequences.
+    Find ``loops`` and create new synthetic events in the paths of all users having such sequences.
 
-    ``Loop`` - is the sequence of repetitive events in user's path.
+    A ``loop`` - is a sequence of repetitive events.
     For example *"event1 -> event1"*
 
     Parameters
     ----------
     suffix : {"loop", "count", None}, default "loop"
 
-        - If ``loop`` event_name will be event_name_loop.\n
-        For example *"event1 - event1 - event1"* --> event1_loop
+        - If ``loop``, event_name will be event_name_loop.\n
+        For example *"event1 - event1 - event1"* --> event1_loop.
 
-        - If ``count`` event_name will be event_name_loop_{number of events}.\n
-        For example *"event1 - event1 - event1"* --> event1_loop_3
+        - If ``count``, event_name will be event_name_loop_{number of events}.\n
+        For example *"event1 - event1 - event1"* --> event1_loop_3.
 
-        - If ``None`` event_name will be - event_name without any changes.\n
-        For example *"event1 - event1 - event1"* --> event1
+        - If ``None``, event_name will be event_name without any changes.\n
+        For example *"event1 - event1 - event1"* --> event1.
 
     timestamp_aggregation_type : {"max", "min", "mean"}, default "max"
-        Aggregation method to define ``timestamp`` for new group.
+        Aggregation method to calculate timestamp values for new groups.
 
     Returns
     -------
     Eventstream
-        ``Eventstream`` with:
+        Eventstream with:
 
-        - raw events: that will be soft-deleted from input ``eventstream`` marked ``_deleted=True``.
-        - new synthetic events: that can be added to the input ``eventstream`` with columns below.
+        - raw events: the returned events will be marked ``_deleted=True`` and soft-deleted from input eventstream.
+        - new synthetic events: the returned events will be added to the input eventstream with columns below.
 
         +------------------------+----------------+--------------------------------------------+
         | **event_name**         | **event_type** | **timestamp**                              |
         +------------------------+----------------+--------------------------------------------+
         | event_name_loop        | group_alias    | min/max/mean(group of repetitive events))  |
         +------------------------+----------------+--------------------------------------------+
         | event_name_loop_{count}| group_alias    | (min/max/mean(group of repetitive events)) |
         +------------------------+----------------+--------------------------------------------+
         | event_name             | group_alias    | (min/max/mean(group of repetitive events)) |
         +------------------------+----------------+--------------------------------------------+
 
+
+    See Also
+    --------
+    .StepMatrix
+
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: CollapseLoopsParams
 
     def __init__(self, params: CollapseLoopsParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/delete_users_by_path_length.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/delete_users_by_path_length.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
 
 class DeleteUsersByPathLengthParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.DeleteUsersByPathLength`
+    A class with parameters for :py:class:`.DeleteUsersByPathLength` class.
     """
 
     events_num: Optional[int]
     cutoff: Optional[Tuple[float, DATETIME_UNITS]]
 
     _widgets = {
         "cutoff": ReteTimeWidget(),
     }
 
 
 class DeleteUsersByPathLength(DataProcessor):
     """
-    Filters entire user's paths if they are shorter than the specified number of events or cut_off.
+    Filter user paths based on the path length, removing the paths that are shorter than the
+    specified number of events or cut_off.
 
     Parameters
     ----------
     events_num : int, optional
         Minimum user path length
 
     cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
@@ -41,14 +42,23 @@
     Eventstream
         ``Eventstream`` with events that should be deleted from input ``eventstream`` marked ``_deleted=True``.
 
     Raises
     ------
     ValueError
         If both of ``events_num`` and ``cutoff`` are empty or both are given.
+
+    See Also
+    --------
+    .TimedeltaHist : Plot the distribution of the time deltas between two events.
+    .UserLifetimeHist : Plot the distribution of user lifetimes.
+
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: DeleteUsersByPathLengthParams
 
     def __init__(self, params: DeleteUsersByPathLengthParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/filter_events.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/filter_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from retentioneering.eventstream.types import EventstreamSchemaType, EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteFunction
 
 
 class FilterEventsParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.FilterEvents`
+    A class with parameters for :py:class:`.FilterEvents` class.
 
     """
 
     func: Callable[[DataFrame, EventstreamSchema], bool]
 
     _widgets = {
         "func": ReteFunction(),
@@ -26,24 +26,27 @@
 class FilterEvents(DataProcessor):
     """
     Filters input ``eventstream`` on the basis of custom conditions.
 
     Parameters
     ----------
     func : Callable[[DataFrame, EventstreamSchema], bool]
-        Custom function which returns boolean mask the same length as input ``eventstream``.
+        Custom function that returns boolean mask the same length as input ``eventstream``.
 
-        - If ``True`` - row will be remained
-        - If ``False`` - row will be deleted
+        - If ``True`` - the row will be left in the eventstream.
+        - If ``False`` - the row will be deleted from the eeventstream.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with events that should be deleted from input ``eventstream``.
 
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
     params: FilterEventsParams
 
     def __init__(self, params: FilterEventsParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/group_events.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/group_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,42 +8,43 @@
 from retentioneering.widget.widgets import ReteFunction
 
 EventstreamFilter = Callable[[pd.DataFrame, EventstreamSchemaType], Any]
 
 
 class GroupEventsParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.GroupEvents`
+    A class with parameters for :py:class:`.GroupEvents` class.
     """
 
     event_name: str
     func: EventstreamFilter
     event_type: Optional[str] = "group_alias"
 
     _widgets = {
         "func": ReteFunction(),
     }
 
 
 class GroupEvents(DataProcessor):
     """
-    Filters specified events from input ``eventstream`` and creates on their basis
-    new synthetic events with new name.
+    Filter the specified events from the input ``eventstream`` and create
+    new synthetic events, with names based on the old events' names.
 
     Parameters
     ----------
     event_name : str
-        Name of new, grouped event
+        Name of the created event.
     func : Callable[[DataFrame, EventstreamSchema], Any]
-        Custom function which returns boolean mask the same length as input Eventstream
-        If ``True`` - events, that will be grouped
-        If ``False`` - events, that will be remained
+        Custom function that returns boolean mask with the same length as input eventstream.
+
+        - If ``True`` - events will be grouped.
+        - If ``False`` - events will be remained.
     event_type : str, default="group_alias"
-        Event_type name for the grouped events
-        If custom event_type is created - it is important to add it to the ``DEFAULT_INDEX_ORDER``
+        Event_type name for the grouped events.
+        If custom event_type is created, it should be added to the ``DEFAULT_INDEX_ORDER``.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with:
 
          - new synthetic events with ``group_alias`` or custom type
@@ -53,14 +54,17 @@
         | **event_name**  | **event_type** | **timestamp**     |  **_deleted**  |
         +-----------------+----------------+-------------------+----------------+
         | raw_event_name  | raw            | raw_event         |  True          |
         +-----------------+----------------+-------------------+----------------+
         | new_event_name  | group_alias    | raw_event         |  False         |
         +-----------------+----------------+-------------------+----------------+
 
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: GroupEventsParams
 
     def __init__(self, params: GroupEventsParams) -> None:
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/lost_users.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/lost_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfInt, ReteTimeWidget
 
 
 class LostUsersParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.LostUsersEvents`
+    A class with parameters for :py:class:`.LostUsersEvents` class.
     """
 
     lost_cutoff: Optional[Tuple[float, DATETIME_UNITS]]
     lost_users_list: Optional[Union[List[int], List[str]]]
 
     _widgets = {
         "lost_cutoff": ReteTimeWidget(),
         "lost_users_list": ListOfInt(),
     }
 
 
 class LostUsersEvents(DataProcessor):
     """
-    Creates one of synthetic events in each user's path:
+    Create one of synthetic events in each user's path:
     ``lost_user`` or ``absent_user``.
 
 
     Parameters
     ----------
     Only one of parameters could be used at the same time
     lost_cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
-        Threshold value and it's unit of measure.
-        Calculate timedelta between last event in each user's path and last event in whole Eventstream.
-        For users with timedelta more or equal than selected ``lost_cutoff``, new synthetic event - ``lost_user``
+        Threshold value and its unit of measure.
+        Calculate timedelta between the last event in each user's path and the last event in the whole eventstream.
+        For users with timedelta greater or equal to selected ``lost_cutoff``, a new synthetic event - ``lost_user``
         will be added.
-        For other user's paths will be added new synthetic event - ``absent_user``
+        For other users paths a new synthetic event - ``absent_user`` will be added.
 
     lost_users_list : list of int or list of str, optional
         If the `list of user_ids` is given new synthetic event - ``lost_user`` will be added to each user from the list.
-        For other user's paths will be added new synthetic event - ``absent_user``
+        For other user's paths will be added new synthetic event - ``absent_user``.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with new synthetic events only - one for each user:
 
         +-----------------+-----------------+------------------+
@@ -58,16 +58,19 @@
         +-----------------+-----------------+------------------+
         | absent_user     | absent_user     | last_event       |
         +-----------------+-----------------+------------------+
 
     Raises
     ------
     ValueError
-        If both of ``lost_cutoff`` and ``lost_users_list`` are empty or both are given.
+        Raised when both ``lost_cutoff`` and ``lost_users_list`` are either empty or given.
 
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: LostUsersParams
 
     def __init__(self, params: LostUsersParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/negative_target.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/negative_target.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,48 +42,53 @@
     )
 
     return df.loc[negative_events_index]  # type: ignore
 
 
 class NegativeTargetParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.NegativeTarget`
+    A class with parameters for :py:class:`.NegativeTarget` class.
     """
 
     negative_target_events: List[str]
     func: Callable = _default_func
 
     _widgets = {"func": ReteFunction(), "negative_target_events": ListOfString()}
 
 
 class NegativeTarget(DataProcessor):
     """
-    Creates new synthetic events in each user's path who have specified event(s):
-    ``negative_target_RAW_EVENT_NAME``
+    Create new synthetic events in paths of all users having the specified event(s):
+    ``negative_target_RAW_EVENT_NAME``.
 
     Parameters
     ----------
     negative_target_events : list of str
-        Each event from that list is associated with the negative user behaviour in the product.
-        If there are several target events in user path - the event with minimum timestamp is taken.
+        Define the list of events that we consider negative.
+        If there are several target events in the user path, the event with the minimum timestamp is taken.
 
     func : Callable, default _default_func_negative
         Filter rows with target events from the input eventstream.
 
     Returns
     -------
     Eventstream
-        ``Eventstream`` with new synthetic events only added to users who fit the conditions.
+        ``Eventstream`` with new synthetic events only added to the users who fit the conditions.
 
         +--------------------------------+-----------------+-----------------------------+
         | **event_name**                 | **event_type**  | **timestamp**               |
         +--------------------------------+-----------------+-----------------------------+
         | negative_target_RAW_EVENT_NAME | negative_target | min(negative_target_events) |
         +--------------------------------+-----------------+-----------------------------+
 
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
+
+
     """
 
     params: NegativeTargetParams
 
     def __init__(self, params: NegativeTargetParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/new_users.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/new_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,48 +8,51 @@
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfIntNewUsers
 
 
 class NewUsersParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.NewUsersEvents`
+    A class with parameters for :py:class:`.NewUsersEvents` class.
     """
 
     new_users_list: Union[List[int], List[str], Literal["all"]]
     _widgets = {"new_users_list": ListOfIntNewUsers()}
 
 
 class NewUsersEvents(DataProcessor):
     """
-    Creates new synthetic event for each user:
+    Create a new synthetic event for each user:
     ``new_user`` or ``existing_user``.
 
     Parameters
     ----------
     new_users_list : list of int or list of str or `all`
 
         If the `list of user_ids` is given - ``new_user`` event will be created for each user from the list.
         Event ``existing_user`` will be added to the rest of the users.
 
         If ``all`` - ``new_user`` synthetic event will be created for all users from the input ``eventstream``.
 
     Returns
     -------
     Eventstream
-        Eventstream with new synthetic events one for each user:
+        Eventstream with new synthetic events, one for each user:
 
         +-----------------+-----------------+------------------------+
         | **event_name**  | **event_type**  | **timestamp**          |
         +-----------------+-----------------+------------------------+
         | new_user        | new_user        | first_event            |
         +-----------------+-----------------+------------------------+
         | existing_user   | existing_user   | first_event            |
         +-----------------+-----------------+------------------------+
 
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
     params: NewUsersParams
 
     def __init__(self, params: NewUsersParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/positive_target.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/positive_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,33 +39,33 @@
     )
 
     return df.loc[positive_events_index]  # type: ignore
 
 
 class PositiveTargetParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.PositiveTarget`
+    A class with parameters for :py:class:`.PositiveTarget` class.
     """
 
     positive_target_events: List[str]
     func: Callable = _default_func
 
     _widgets = {"func": ReteFunction(), "positive_target_events": ListOfString()}
 
 
 class PositiveTarget(DataProcessor):
     """
-    Creates new synthetic events in each user's path who have specified event(s):
+    Create new synthetic events in paths of all users having the specified events:
     ``positive_target_RAW_EVENT_NAME``
 
     Parameters
     ----------
     positive_target_events : list of str
-        Each event from that list is associated with a conversional user behaviour in the product.
-        If there are several target events in user path - the event with minimum timestamp taken.
+        Define the list of events we consider positive.
+        If there are several target events in a user path, the event with the minimum timestamp is taken.
 
     func : Callable, default _default_func
         Filter rows with target events from the input eventstream.
 
     Returns
     -------
     Eventstream
@@ -73,14 +73,17 @@
 
         +--------------------------------+-----------------+-----------------------------+
         | **event_name**                 | **event_type**  | **timestamp**               |
         +--------------------------------+-----------------+-----------------------------+
         | positive_target_RAW_EVENT_NAME | positive_target | min(positive_target_events) |
         +--------------------------------+-----------------+-----------------------------+
 
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: PositiveTargetParams
 
     def __init__(self, params: PositiveTargetParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/rename.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/rename.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/split_sessions.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/split_sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,54 +11,55 @@
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
 
 class SplitSessionsParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.SplitSessions`
+    A class with parameters for :py:class:`.SplitSessions` class.
 
     """
 
     session_cutoff: Tuple[float, DATETIME_UNITS]
     mark_truncated: bool = False
     session_col: str = "session_id"
 
     _widgets = {"session_cutoff": ReteTimeWidget()}
 
 
 class SplitSessions(DataProcessor):
     """
-    Creates new synthetic events, which divide user's paths on sessions:
+    Create new synthetic events, that divide users' paths on sessions:
     ``session_start`` (or ``session_start_truncated``) and ``session_end`` (or ``session_end_truncated``).
-    Also creates new column which contains session number for each event in input eventstream
-    Session number will take the form: ``{user_id}_{session_number through one user path}``
+    Also create a new column that contains session number for each event in input eventstream.
+    Session number will take the form: ``{user_id}_{session_number through one user path}``.
 
     Parameters
     ----------
     session_cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`)
         Threshold value and its unit of measure.
         ``session_start`` and ``session_end`` events are always placed before the first and after the last event
         in each user's path.
-        But user can have more than one session, so that calculates timedelta between every two consecutive events in
+        Because user can have more than one session, it calculates timedelta between every two consecutive events in
         each user's path.
-        If calculated timedelta is more than selected session_cutoff,
-        new synthetic events - ``session_start`` and ``session_end`` will occur in the middle of user path.
+        If the calculated timedelta is more than selected session_cutoff,
+        new synthetic events - ``session_start`` and ``session_end`` are created inside the user path,
+        marking session starting and ending points.
 
     mark_truncated : bool, default False
         If ``True`` - calculates timedelta between:
 
-        - first event in each user's path and first event in whole ``eventstream``.
-        - last event in each user's path and last event in whole ``eventstream``.
+        - first event in each user's path and first event in the whole eventstream.
+        - last event in each user's path and last event in the whole eventstream.
 
         For users with timedelta less than selected ``session_cutoff``,
-        new synthetic event - ``session_start_truncated`` or ``session_end_truncated`` will be added.
+        a new synthetic event - ``session_start_truncated`` or ``session_end_truncated`` will be added.
 
     session_col : str, default "session_id"
-        The name of future ``session_col``
+        The name of the ``session_col``.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with new synthetic events and ``session_col``.
 
         +-----------------------------+----------------------------+-----------------+
@@ -69,32 +70,40 @@
         | session_end                 | session_end                | last_event      |
         +-----------------------------+----------------------------+-----------------+
         | session_start_truncated     | session_start_truncated    | first_event     |
         +-----------------------------+----------------------------+-----------------+
         | session_end_truncated       | session_end_truncated      | last_event      |
         +-----------------------------+----------------------------+-----------------+
 
-        The user will have more than one session if the delta between timestamps of two consecutive events
-        (raw_event_n and raw_event_n+1) is greater than the selected ``session_cutoff``:
+        If the delta between timestamps of two consecutive events
+        (raw_event_n and raw_event_n+1) is greater than the selected ``session_cutoff``
+        the user will have more than one session:
 
         +--------------+-------------------+------------------+-------------------+------------------+
         |  **user_id** | **event_name**    | **event_type**   | **timestamp**     | **session_col**  |
         +--------------+-------------------+------------------+-------------------+------------------+
         |     1        | session_start     | session_start    | first_event       |     1_0          |
         +--------------+-------------------+------------------+-------------------+------------------+
         |     1        | session_end       | session_end      | raw_event_n       |     1_0          |
         +--------------+-------------------+------------------+-------------------+------------------+
         |     1        | session_start     | session_start    | raw_event_n+1     |     1_1          |
         +--------------+-------------------+------------------+-------------------+------------------+
         |     1        | session_end       | session_end      | last_event        |     1_1          |
         +--------------+-------------------+------------------+-------------------+------------------+
 
+    See Also
+    --------
+    .TimedeltaHist : Plot the distribution of the time deltas between two events.
+    .Eventstream.describe : Show general eventstream statistics.
+    .Eventstream.describe_events : Show general eventstream events statistics.
+
+
     Notes
     -----
-    Hists
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
     params: SplitSessionsParams
 
     def __init__(self, params: SplitSessionsParams) -> None:
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/start_end_events.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/start_end_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class StartEndEventsParams(ParamsModel):
     pass
 
 
 class StartEndEvents(DataProcessor):
     """
-    Creates two synthetic events in each user's path:
+    Create two synthetic events in each user's path:
     ``path_start`` and ``path_end``.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with new synthetic events only - two for each user:
 
@@ -26,15 +26,17 @@
         | **event_name** | **event_type** | **timestamp**  |
         +----------------+----------------+----------------+
         | path_start     | path_start     | first_event    |
         +----------------+----------------+----------------+
         | path_end       | path_end       | last_event     |
         +----------------+----------------+----------------+
 
-
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: StartEndEventsParams
 
     def __init__(self, params: StartEndEventsParams) -> None:
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/truncate_path.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncate_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,61 +7,64 @@
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 
 
 class TruncatePathParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.TruncatePath`
+    A class with parameters for :py:class:`.TruncatePath` class.
     """
 
     drop_before: Optional[str]
     drop_after: Optional[str]
     occurrence_before: Literal["first", "last"] = "first"
     occurrence_after: Literal["first", "last"] = "first"
     shift_before: int = 0
     shift_after: int = 0
 
 
 class TruncatePath(DataProcessor):
     """
-    Filters events that will be deleted from each user's path
-    on the base of specified event and selected parameters.
+    Remove events that will be deleted from each user's path
+    based on the specified event and selected parameters.
 
     Parameters
     ----------
     drop_before : str, optional
-        Event name before which part of the user's path is dropped. Specified event remains in the data.
+        Event name before which part of the user's path is dropped. The specified event remains in the data.
     drop_after : str, optional
-        Event name after which part of the user's path is dropped. Specified event remains in the data.
+        Event name after which part of the user's path is dropped. The specified event remains in the data.
     occurrence_before : {"first", "last"}, default="first"
-        This parameter is necessary when specified event occurs more than once in one user's path.
-        ``first`` - before first occurrence of the specified event the user's path will be dropped.
-        ``last`` - before last occurrence of the specified event the user's path will be dropped.
+        This parameter is necessary when the specified event occurs more than once in one user's path.
+
+        - when set to ``first``, the part of the user path before the first event occurrence is dropped;
+        - when set to ``last``, the part of the user path before the last event occurrence is dropped;
+
     occurrence_after : {"first", "last"}, default="first"
         The same behavior as in the 'occurrence_before', but for the other part of the user path.
     shift_before : int,  default=0
-        Sets the number of steps by which truncate point is shifted from the selected event.
+        Sets the number of steps by which the truncate point is shifted from the selected event.
         If the value is negative, then the offset occurs to the left along the timeline.
-        If positive, then to the right.
+        If positive, then it occurs to the right.
     shift_after : int,  default=0
         The same behavior as in the ``shift_before``, but for the other part of the user path.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with events that should be deleted from input ``eventstream``.
 
 
     Notes
     -----
-    ``Step`` - is the group of events in user path with the same timestamp
-    If user path doesn't contain events from ``drop_before`` and ``drop_after`` parameters - than its
+    ``Step`` - is the group of events in the user path with the same timestamp.
+    If the user path doesn't contain events from ``drop_before`` and ``drop_after`` parameters, then its
     path does not change.
 
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: TruncatePathParams
 
     def __init__(self, params: TruncatePathParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/data_processors_lib/truncated_events.py` & `retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncated_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,66 +11,72 @@
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
 
 class TruncatedEventsParams(ParamsModel):
     """
-    Class with parameters for class :py:class:`.TruncatedEvents`
+    A class with parameters for :py:class:`.TruncatedEvents` class.
     """
 
     left_truncated_cutoff: Optional[Tuple[float, DATETIME_UNITS]]
     right_truncated_cutoff: Optional[Tuple[float, DATETIME_UNITS]]
 
     _widgets = {
         "left_truncated_cutoff": ReteTimeWidget(),
         "right_truncated_cutoff": ReteTimeWidget(),
     }
 
 
 class TruncatedEvents(DataProcessor):
     """
-    Creates new synthetic event(s) for each user on the base of timeout threshold:
-    ``truncated_left`` and ``truncated_right``
+    Create new synthetic event(s) for each user based on the timeout threshold:
+    ``truncated_left`` or ``truncated_right``
 
     Parameters
     ----------
     left_truncated_cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
-        Threshold value, and it's unit of measure.
-        Timedelta between last event in each user's path and first event in whole Eventstream is calculating.
-        For users with timedelta less than selected ``left_truncated_cutoff``, new synthetic event - ``truncated_left``
-        will be added.
+        Threshold value with its unit of measure.
+        The timedelta between the last event in each user's path and the first event in the whole eventstream
+        is calculated. For users with the timedelta less than the selected ``left_truncated_cutoff``,
+        the new ``truncated_left`` event is added.
 
     right_truncated_cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
-        Threshold value and its unit of measure.
-        Timedelta between first event in each user's path and last event in whole Eventstream is calculating.
-        For users with timedelta less than selected ``right_truncated_cutoff``,
-        new synthetic event - ``truncated_right`` will be added.
+        Threshold value with its unit of measure.
+        The timedelta between the first event in each user's path and the last event in the whole eventstream
+        is calculated. For users with timedelta less than the selected ``right_truncated_cutoff``,
+        the new ``truncated_right`` event is added.
 
     Returns
     -------
     Eventstream
-        ``Eventstream`` with new synthetic events only, for users whose paths satisfy the specified cut-offs.
+        Eventstream containing only the generated synthetic events, for users whose paths
+        satisfy the specified cut-offs.
 
         +-------------------+-------------------+------------------+
         | **event_name**    | **event_type**    |  **timestamp**   |
         +-------------------+-------------------+------------------+
         | truncated_left    | truncated_left    |  first_event     |
         +-------------------+-------------------+------------------+
         | truncated_right   | truncated_right   |  last_event      |
         +-------------------+-------------------+------------------+
 
     See Also
     --------
-    Hists
+    .TimedeltaHist : Plot the distribution of the time deltas between two events.
+    .UserLifetimeHist : Plot the distribution of user lifetimes.
 
     Raises
     ------
     ValueError
         If both of ``left_truncated_cutoff`` and ``right_truncated_cutoff`` are empty.
+
+    Notes
+    -----
+    See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: TruncatedEventsParams
 
     def __init__(self, params: TruncatedEventsParams):
         super().__init__(params=params)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/datasets/data/ab_test_demo.csv` & `retentioneering-3.0.0b1/retentioneering/datasets/data/ab_test_demo.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/datasets/data/simple-onlineshop.csv` & `retentioneering-3.0.0b1/retentioneering/datasets/data/simple-onlineshop.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/datasets/load.py` & `retentioneering-3.0.0b1/retentioneering/datasets/load.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/eventstream.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/eventstream.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 from __future__ import annotations
 
 import uuid
 from collections.abc import Collection
-from typing import Any, Callable, List, Literal, Optional, Tuple, Union
+from typing import Any, Callable, List, Literal, MutableMapping, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.eventstream.schema import EventstreamSchema, RawDataSchema
 from retentioneering.eventstream.types import (
@@ -28,18 +28,18 @@
 from retentioneering.tooling.step_matrix import StepMatrix
 from retentioneering.tooling.step_sankey import StepSankey
 from retentioneering.tooling.timedelta_hist import (
     AGGREGATION_NAMES,
     EVENTSTREAM_GLOBAL_EVENTS,
     TimedeltaHist,
 )
+from retentioneering.tooling.transition_graph import TransitionGraph
 from retentioneering.tooling.transition_matrix import TransitionMatrix
 from retentioneering.tooling.typing.transition_graph import NormType, Threshold
 from retentioneering.tooling.user_lifetime_hist import UserLifetimeHist
-from retentioneering.transition_graph import TransitionGraph
 from retentioneering.utils import get_merged_col
 from retentioneering.utils.list import find_index
 
 from .helpers import (
     CollapseLoopsHelperMixin,
     DeleteUsersByPathLengthHelperMixin,
     FilterHelperMixin,
@@ -115,39 +115,45 @@
     Parameters
     ----------
     raw_data : pd.DataFrame or pd.Series
         Raw clickstream data.
     raw_data_schema : RawDataSchema, optional
         Should be specified as an instance of class ``RawDataSchema``:
 
-        - If ``raw_data`` column names are different from default :py:class:`.RawDataSchema`.
+        - If ``raw_data`` column names are different from the default :py:class:`.RawDataSchema`.
         - If there is at least one ``custom_col`` in ``raw_data``.
 
     schema : EventstreamSchema, optional
-        Schema of created ``eventstream``.
+        Schema of the created ``eventstream``.
         See default schema :py:class:`.EventstreamSchema`.
     prepare : bool, default True
+        - If ``True``, input data will be transformed in the following way:
+
+            * ``event_timestamp`` column is converted to pandas datetime format.
+            * | ``event_type`` column is added and filled with ``raw`` value.
+              | If the column exists, it remains unchanged.
 
-        - If ``True`` input data will be transformed in the following way:
-            - Convert column ``event_timestamp`` to pandas datetime format.
-            - | Adds ``event_type`` column and fills with ``raw`` value.
-              | if that column already exists it will remain unchanged.
         - If ``False`` - ``raw_data`` will be remained as is.
 
     index_order : list of str, default DEFAULT_INDEX_ORDER
         Sorting order for ``event_type`` column.
     relations : list, optional
     user_sample_size : int of float, optional
-        Number (``int``) or share (``float``) of all users trajectories which will be randomly chosen
-        and remained in final sample.
+        Number (``int``) or share (``float``) of all users' trajectories that will be randomly chosen
+        and left in final sample (all other trajectories will be removed) .
         See :numpy_random_choice:`numpy documentation<>`.
     user_sample_seed : int, optional
-        Random seed value to generate repeated random users sample.
+        A seed value that is used to generate user samples.
         See :numpy_random_seed:`numpy documentation<>`.
 
+    Notes
+    -----
+    See :doc:`Eventstream user guide</user_guides/eventstream>` for the details.
+
+
     """
 
     schema: EventstreamSchema
     index_order: IndexOrder
     relations: List[Relation]
     __raw_data_schema: RawDataSchemaType
     __events: pd.DataFrame | pd.Series[Any]
@@ -373,18 +379,18 @@
         Convert ``eventstream`` to ``pd.Dataframe``
 
         Parameters
         ----------
         raw_cols : bool, default False
             If ``True`` - original columns of the input ``raw_data`` will be shown.
         show_deleted : bool, default False
-            If ``True`` - show all rows in ``eventstream``
+            If ``True`` - show all rows in ``eventstream``.
         copy : bool, default False
             If ``True`` - copy data from current ``eventstream``.
-            See details :pandas_copy:`pandas documentation<>`
+            See details in the :pandas_copy:`pandas documentation<>`.
 
         Returns
         -------
         pd.DataFrame
 
         """
         cols = self.schema.get_cols() + self._get_relation_cols()
@@ -432,24 +438,24 @@
         for col in cols:
             if col.startswith("ref_"):  # type: ignore
                 relation_cols.append(col)  # type: ignore
         return relation_cols
 
     def add_custom_col(self, name: str, data: pd.Series[Any] | None) -> None:
         """
-        Add custom column to existing ``eventstream``.
+        Add custom column to an existing ``eventstream``.
 
         Parameters
         ----------
         name : str
             New column name.
         data : pd.Series
 
             - If ``pd.Series`` - new column with given values will be added.
-            - If ``None`` - new column will be filled with ``np.nan``
+            - If ``None`` - new column will be filled with ``np.nan``.
 
         Returns
         -------
         Eventstream
         """
         self.__raw_data_schema.custom_cols.extend([{"custom_col": name, "raw_data_col": name}])
         self.schema.custom_cols.extend([name])
@@ -594,15 +600,20 @@
         segments: Collection[Collection[int]] | None = None,
         segment_names: list[str] | None = None,
         show_plot: bool = True,
     ) -> Funnel:
         """
         Show a visualization of the user sequential events represented as a funnel.
 
-        See parameters description :py:class:`.Funnel`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, a funnel visualization is shown.
+        See other parameters' description
+            :py:class:`.Funnel`
 
         Returns
         -------
         Funnel
             A ``Funnel`` class instance fitted to the given parameters.
 
         """
@@ -619,20 +630,23 @@
             figure = self.__funnel.plot()
             figure.show()
         return self.__funnel
 
     @property
     def clusters(self) -> Clusters:
         """
-        Return a blank (not fitted) instance of ``Clusters`` class to be used for cluster analysis.
-        See :py:class:`.Clusters`
 
         Returns
         -------
         Clusters
+            A blank (not fitted) instance of ``Clusters`` class to be used for cluster analysis.
+
+        See Also
+        --------
+        .Clusters
         """
         if self.__clusters is None:
             self.__clusters = Clusters(eventstream=self)
         return self.__clusters
 
     def step_matrix(
         self,
@@ -646,15 +660,20 @@
         centered: Optional[dict] = None,
         groups: Optional[Tuple[list, list]] = None,
         show_plot: bool = True,
     ) -> StepMatrix:
         """
         Show a heatmap visualization of the step matrix.
 
-        See parameters description :py:class:`.StepMatrix`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, a step matrix heatmap is shown.
+        See other parameters' description
+            :py:class:`.StepMatrix`
 
         Returns
         -------
         StepMatrix
             A ``StepMatrix`` class instance fitted to the given parameters.
 
         """
@@ -685,17 +704,22 @@
         target: Union[list[str], str] | None = None,
         autosize: bool = True,
         width: int | None = None,
         height: int | None = None,
         show_plot: bool = True,
     ) -> StepSankey:
         """
-        Show a Sankey diagram visualizing the user paths in step-wise manner.
+        Show a Sankey diagram visualizing the user paths in stepwise manner.
 
-        See parameters description :py:class:`.StepSankey`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, a sankey diagram is shown.
+        See other parameters' description
+            :py:class:`.StepSankey`
 
         Returns
         -------
         StepSankey
             A ``StepSankey`` class instance fitted to the given parameters.
 
         """
@@ -726,15 +750,20 @@
         cut_diagonal: int = 0,
         figsize: Tuple[float, float] = (10, 10),
         show_plot: bool = True,
     ) -> Cohorts:
         """
         Show a heatmap visualization of the user appearance grouped by cohorts.
 
-        See parameters description :py:class:`.Cohorts`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, a cohort matrix heatmap is shown.
+        See other parameters' description
+            :py:class:`.Cohorts`
 
         Returns
         -------
         Cohorts
             A ``Cohorts`` class instance fitted to the given parameters.
         """
 
@@ -760,15 +789,18 @@
         func: Callable,
         group_names: Tuple[str, str] = ("group_1", "group_2"),
         alpha: float = 0.05,
     ) -> StatTests:
         """
         Determine the statistical difference between the metric values in two user groups.
 
-        See parameters description :py:class:`.Stattests`
+        Parameters
+        ----------
+        See parameters' description
+            :py:class:`.Stattests`
 
         Returns
         -------
         StatTests
             A ``StatTest`` class instance fitted to the given parameters.
         """
         self.__stattests = StatTests(
@@ -794,15 +826,20 @@
         show_plot: bool = True,
     ) -> TimedeltaHist:
         """
         Plot the distribution of the time deltas between two events. Support various
         distribution types, such as distribution of time for adjacent consecutive events, or
         for a pair of pre-defined events, or median transition time from event to event per user/session.
 
-        See parameters description :py:class:`.TimedeltaHist`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, histogram is shown.
+        See other parameters' description
+            :py:class:`.TimedeltaHist`
 
         Returns
         -------
         TimedeltaHist
             A ``TimedeltaHist`` class instance fitted with given parameters.
 
         """
@@ -834,24 +871,30 @@
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
         figsize: tuple[float, float] = (12.0, 7.0),
         show_plot: bool = True,
     ) -> UserLifetimeHist:
         """
-        Plot the distribution of user lifetimes. A ``users' lifetime`` is the timedelta between the first and the last
-        events of the user. Can be useful for finding suitable parameters of various data processors, such as
-        :py:class:`.DeleteUsersByPathLength>` or :py:class:`.TruncatedEvents>`.
+        Plot the distribution of user lifetimes. A ``users lifetime`` is the timedelta between the first and the last
+        events of the user.
 
-        See parameters description :py:class:`.UserLifetimeHist`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, histogram is shown.
+        See other parameters' description
+            :py:class:`.UserLifetimeHist`
 
         Returns
         -------
         UserLifetimeHist
             A ``UserLifetimeHist`` class instance with given parameters.
+
+
         """
         self.__user_lifetime_hist = UserLifetimeHist(
             eventstream=self,
             timedelta_unit=timedelta_unit,
             log_scale=log_scale,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
@@ -870,18 +913,24 @@
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
         figsize: tuple[float, float] = (12.0, 7.0),
         show_plot: bool = True,
     ) -> EventTimestampHist:
         """
-        Plot the distribution of events over time. Can be useful for detecting time-based anomalies, and visualising
+        Plot distribution of events over time. Can be useful for detecting time-based anomalies, and visualising
         general timespan of the eventstream.
 
-        See parameters description :py:class:`.EventTimestampHist`
+        Parameters
+        ----------
+        show_plot : bool, default True
+            If ``True``, histogram is shown.
+        See other parameters' description
+            :py:class:`.EventTimestampHist`
+
 
         Returns
         -------
         EventTimestampHist
             A ``EventTimestampHist`` class instance with given parameters.
         """
         self.__event_timestamp_hist = EventTimestampHist(
@@ -897,194 +946,191 @@
         self.__event_timestamp_hist.fit()
         if show_plot:
             self.__event_timestamp_hist.plot()
         return self.__event_timestamp_hist
 
     def describe(self, session_col: str = "session_id", raw_events_only: bool = False) -> pd.DataFrame:
         """
-        Display general eventstream information. If ``session_col`` is presented in eventstream, also
+        Display general eventstream information. If ``session_col`` is present in eventstream, also
         output session statistics.
 
         Parameters
         ----------
         session_col : str, default 'session_id'
-            Specify name of the session column. If the column is presented in the eventstream,
+            Specify name of the session column. If the column is present in the eventstream,
             session statistics will be added to the output.
 
         raw_events_only : bool, default False
-            If ``True`` - statistics will be shown only for raw events.
-            If ``False`` - for all events presented in your data.
+            If ``True`` - statistics will only be shown for raw events.
+            If ``False`` - statistics will be shown for all events presented in your data.
+
+        Returns
+        -------
+        pd.DataFrame
+            A dataframe containing descriptive statistics for the eventstream.
+
+
+        See Also
+        --------
+        .EventTimestampHist : Plot the distribution of events over time.
+        .TimedeltaHist : Plot the distribution of the time deltas between two events.
+        .UserLifetimeHist : Plot the distribution of user lifetimes.
+        .Eventstream.describe_events : Show general eventstream events statistics.
+
 
         Notes
         -----
         - All ``float`` values are rounded to 2.
         - All ``datetime`` values are rounded to seconds.
 
-        Returns
-        -------
-        pd.DataFrame
-            A dataframe containing descriptive statistics on the eventstream.
+        See :ref:`Eventstream user guide<eventstream_describe>` for the details.
+
 
         """
         describer = Describe(eventstream=self, session_col=session_col, raw_events_only=raw_events_only)
         return describer._describe()
 
     def describe_events(
         self, session_col: str = "session_id", raw_events_only: bool = False, event_list: list[str] | None = None
     ) -> pd.DataFrame:
         """
-        Display general information on the eventstream events. If ``session_col`` is presented in eventstream, also
+        Display general information on eventstream events. If ``session_col`` is present in eventstream, also
         output session statistics.
 
         Parameters
         ----------
         session_col : str, default 'session_id'
-            Specify name of the session column. If the column is presented in the eventstream,
+            Specify name of the session column. If the column is present in the eventstream,
             output session statistics.
 
         raw_events_only : bool, default False
-            If ``True`` - statistics will be shown only for raw events.
-            If ``False`` - for all events presented in your data.
+            If ``True`` - statistics will only be shown for raw events.
+            If ``False`` - statistics will be shown for all events presented in your data.
 
         event_list : list of str, optional
-            Specify the events to be displayed.
+            Specify events to be displayed.
 
         Returns
         -------
         pd.DataFrame
             **Eventstream statistics**:
 
-            - | The following metrics are calculated for each event represented in the eventstream
-              | (or the narrowed eventstream if parameters ``event_list`` or ``raw_events_only`` are used).
-              | Let all_events, all_users, all_sessions be the number of all events, users,
-              | and sessions represented in the eventstream. Then:
-
-                - *number_of_occurrences* - the number of occurrences of a particular event in the eventstream
-                - *unique_users* - the number of unique users who experienced a particular event
-                - *unique_sessions* - the number of unique sessions with each event
-                - *number_of_occurrences_shared* - number_of_occurrences / all_events (raw_events_only, if this parameter = ``True``)
-                - *unique_users_shared* - unique_users / all_users
-                - *unique_sessions_shared* - unique_sessions / all_sessions
-
-            - | **time_to_FO_user_wise** category - timedelta between ``path_start``
-              | and the first occurrence (FO) of a specified event in each user path.
-            - | **steps_to_FO_user_wise** category - the number of steps (events) from
-              | ``path_start`` to the first occurrence (FO) of a specified event in each user path.
-              | If ``raw_events_only=True`` only raw events will be counted.
-            - | **time_to_FO_session_wise** category - timedelta  between ``session_start``
-              | and the first occurrence (FO) of a specified event in each session.
-            - | **steps_to_FO_session_wise** category - the number of steps (events) from
-              | ``session_start`` to the first occurrence (FO) of a specified event in each session.
-              | If ``raw_events_only=True`` only raw events will be counted.
-
-            Agg functions for each ``first_occurrence*`` category are: mean, std, median, min, max
+            - The following metrics are calculated for each event present in the eventstream
+              (or the narrowed eventstream if parameters ``event_list`` or ``raw_events_only`` are used).
+              Let all_events, all_users, all_sessions be the numbers of all events, users,
+              and sessions present in the eventstream. Then:
+
+                - *number_of_occurrences* - the number of occurrences of a particular event in the eventstream;
+                - *unique_users* - the number of unique users who experienced a particular event;
+                - *unique_sessions* - the number of unique sessions with each event;
+                - *number_of_occurrences_shared* - number_of_occurrences / all_events (raw_events_only,
+                  if this parameter = ``True``);
+                - *unique_users_shared* - unique_users / all_users;
+                - *unique_sessions_shared* - unique_sessions / all_sessions;
+
+            - **time_to_FO_user_wise** category - timedelta between ``path_start``
+              and the first occurrence (FO) of a specified event in each user path.
+            - **steps_to_FO_user_wise** category - the number of steps (events) from
+              ``path_start`` to the first occurrence (FO) of a specified event in each user path.
+              If ``raw_events_only=True`` only raw events will be counted.
+            - **time_to_FO_session_wise** category - timedelta  between ``session_start``
+              and the first occurrence (FO) of a specified event in each session.
+            - **steps_to_FO_session_wise** category - the number of steps (events) from
+              ``session_start`` to the first occurrence (FO) of a specified event in each session.
+              If ``raw_events_only=True`` only raw events will be counted.
+
+            Agg functions for each ``first_occurrence*`` category are: mean, std, median, min, max.
+
+        See Also
+        --------
+        .EventTimestampHist : Plot the distribution of events over time.
+        .TimedeltaHist : Plot the distribution of the time deltas between two events.
+        .UserLifetimeHist : Plot the distribution of user lifetimes.
+        .Eventstream.describe : Show general eventstream statistics.
 
         Notes
         -----
-        - All ``float`` values rounded to 2.
+        - All ``float`` values are rounded to 2.
         - All ``datetime`` values are rounded to seconds.
 
+        See :ref:`Eventstream user guide<eventstream_describe_events>` for the details.
+
         """
         describer = DescribeEvents(
             eventstream=self, session_col=session_col, event_list=event_list, raw_events_only=raw_events_only
         )
         return describer._describe()
 
     def transition_graph(
         self,
-        thresholds: dict[str, Threshold] | None = None,
-        norm_type: NormType = None,
-        weights: dict[str, str] | None = None,
-        targets: dict[str, str | None] | None = None,
+        graph_settings: dict[str, Any] | None = None,
+        edges_norm_type: NormType = None,
+        targets: MutableMapping[str, str | None] | None = None,
+        nodes_threshold: Threshold | None = None,
+        edges_threshold: Threshold | None = None,
+        nodes_weight_col: str | None = None,
+        edges_weight_col: str | None = None,
+        custom_weight_cols: list[str] | None = None,
         width: int = 960,
         height: int = 900,
     ) -> TransitionGraph:
         """
-        Create interactive transition graph visualization with callback to sourcing eventstream.
 
         Parameters
         ----------
-        norm_type: {"full", "node", None}, default None
-            Type of normalization that is used to calculate weights for graph nodes and edges. See
-            :ref:`Transition graph user guide <transition_graph_weights>` for the details.
-
-        weights: dict, optional
-            Weighting columns for nodes and edges. See :ref:`Transition graph user guide <transition_graph_weights>`
-            for the details.
-
-            - Possible keys: "nodes", "edges".
-            - Possible values: "event_id", user column (typically "user_id") or custom columns.
-
-            If None, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
-
-        thresholds: dict, optional
-            Threshold values for hiding nodes and edges from the canvas.
-
-            - Possible keys: "nodes", "edges".
-            - Possible values: dict with weighting columns as dict keys and threshold values as dict values.
-
-            Example: {'nodes': {'event_id': 0.03}, 'edges': {'event_id': 0.03, user_id: 0.05}}
-
-            If None, all the threshold values are set to 0.
-
-        targets: dict, optional
-            Events mapping that defines which nodes and edges should be colored for better visualization.
-
-            - Possible keys: "positive" (green), "negative" (red), "source" (orange).
-            - Possible values: list of events of a given type.
-
-        width: int, default 960
-            Width of the plot in pixels.
-        height: int, default 960
-            Height of the plot in pixels.
+        See parameters' description
+            :py:class:`.TransitionGraph`
 
         Returns
         -------
         TransitionGraph
-            A ``TransitionGraph`` class instance fitted to the given parameters.
+            Rendered IFrame graph.
+
         """
         self.__transition_graph = TransitionGraph(
             eventstream=self,
-            graph_settings={},  # type: ignore
-            norm_type=norm_type,
-            weights=weights,
-            thresholds=thresholds,
+            graph_settings=graph_settings,
+            edges_norm_type=edges_norm_type,
             targets=targets,
+            nodes_threshold=nodes_threshold,
+            edges_threshold=edges_threshold,
+            nodes_weight_col=nodes_weight_col,
+            edges_weight_col=edges_weight_col,
+            custom_weight_cols=custom_weight_cols,
         )
         self.__transition_graph.plot_graph(
-            thresholds=thresholds, targets=targets, weights=weights, width=width, height=height, norm_type=norm_type
+            targets=targets,
+            width=width,
+            height=height,
+            edges_norm_type=edges_norm_type,
         )
         return self.__transition_graph
 
     def processing_graph(self) -> PGraph:
         if self.__p_graph is None:
             self.__p_graph = PGraph(source_stream=self)
         self.__p_graph.display()
         return self.__p_graph
 
-    def transition_matrix(self, weights: list[str] | None = None, norm_type: NormType = None) -> TransitionMatrix:
+    def transition_matrix(self, weight_col: str | None = None, norm_type: NormType = None) -> TransitionMatrix:
         """
-        Get transition weights as a matrix for each unique pair of events. The calculation logic is the same
-        that is used for edge weights calculation of transition graph.
+        Display transition weights as a matrix for each unique pair of events.
+        The calculation logic is the same that is used for edge weights calculation of transition graph.
 
         Parameters
         ----------
+        See parameters' description
+            :py:meth:`.TransitionMatrix.values`
 
-        weights : str, default None
-            Weighting column for the transition weights calculation.
-            See :ref:`transition graph user guide <transition_graph_weights>` for the details.
-
-        norm_type : {"full", "node", None}, default None
-            Normalization type. See :ref:`transition graph user guide <transition_graph_weights>` for the details.
 
         Returns
         -------
-        pd.DataFrame
-            ``(i, j)``-th matrix value relates to the weight of i → j transition.
+        TransitionMatrix
+            Display ``(i, j)``-th matrix value relates to the weight of i → j transition.
 
         """
         if self.__transition_matrix is None:
             self.__transition_matrix = TransitionMatrix(
                 eventstream=self,
             )
-        self.__transition_matrix.display(weights=weights, norm_type=norm_type)
+        self.__transition_matrix.display(weight_col=weight_col, norm_type=norm_type)
         return self.__transition_matrix
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/__init__.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/collapse_loops_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/collapse_loops_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 class CollapseLoopsHelperMixin:
     def collapse_loops(
         self,
         suffix: Union[Literal["loop", "count"], None] = "loop",
         timestamp_aggregation_type: Literal["max", "min", "mean"] = "max",
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which finds ``loops`` and creates new synthetic events
-        in each user's path who have such sequences.
+        A method of ``Eventstream`` class that finds ``loops`` and creates new synthetic events
+        in paths of all users having such sequences.
 
-        ``Loop`` - is the sequence of repetitive events in user's path.
+        A ``loop`` - is a sequence of repetitive events.
         For example *"event1 -> event1"*
 
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.CollapseLoops`
+
         Returns
         -------
         Eventstream
              Input ``eventstream`` with ``loops`` replaced by new synthetic events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.CollapseLoops`
+
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             CollapseLoops,
             CollapseLoopsParams,
         )
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/delete_users_by_path_length_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/delete_users_by_path_length_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
 
 class DeleteUsersByPathLengthHelperMixin:
     def delete_users(
         self, events_num: int | None = None, cutoff: Tuple[float, DATETIME_UNITS] | None = None
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which deletes entire user's paths if they are shorter than the specified
+        A method of ``Eventstream`` class that deletes users' paths that are shorter than the specified
         number of events or cut_off.
 
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.DeleteUsersByPathLength`
+
         Returns
         -------
         Eventstream
-             Input ``eventstream`` with deleted short user's paths.
+             Input ``eventstream`` without the deleted short users' paths.
+
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.DeleteUsersByPathLength`
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             DeleteUsersByPathLength,
             DeleteUsersByPathLengthParams,
         )
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/filter_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/filter_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 from ..types import EventstreamSchemaType, EventstreamType
 
 
 class FilterHelperMixin:
     def filter(self, func: Callable[[DataFrame, EventstreamSchemaType], Any]) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which filters input ``eventstream`` on the basis of custom conditions.
+        A method of ``Eventstream`` class that filters input ``eventstream`` based on custom conditions.
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.FilterEvents`
 
         Returns
         -------
         Eventstream
-            Filtered ``eventstream``.
+            The filtered ``eventstream``.
+
 
-        See Also
-        --------
-        :py:class:`.FilterEvents`
         """
         # avoid circular import
         from retentioneering.data_processors_lib import FilterEvents, FilterEventsParams
         from retentioneering.graph.nodes import EventsNode
         from retentioneering.graph.p_graph import PGraph
 
         p = PGraph(source_stream=self)  # type: ignore
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/group_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/group_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,28 @@
     def group(
         self,
         event_name: str,
         func: EventstreamFilter,
         event_type: str | None = "group_alias",
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which filters and replaces raw events with new synthetic events.
-        Where ``timestamp``, ``user_id`` are the same, but ``event_name`` is new.
+        A method of ``Eventstream`` class that filters and replaces raw events with new synthetic events,
+        having the same ``timestamp`` and ``user_id``, but new ``event_name``.
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.GroupEvents`
 
         Returns
         -------
         Eventstream
              Input ``eventstream`` with replaced events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.GroupEvents`
+
 
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import GroupEvents, GroupEventsParams
         from retentioneering.graph.nodes import EventsNode
         from retentioneering.graph.p_graph import PGraph
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/lost_users_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/lost_users_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
 
 class LostUsersHelperMixin:
     def lost_users(
         self, lost_cutoff: Optional[Tuple[float, DATETIME_UNITS]] = None, lost_users_list: Optional[List[int]] = None
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates one of synthetic events in each user's path:
-        ``lost_user`` or ``absent_user``. And adds them to the input ``eventstream``.
+        A method of ``Eventstream`` class that creates one
+        of the synthetic events in each user's path: ``lost_user`` or ``absent_user`` .
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.LostUsersEvents`
 
         Returns
         -------
         Eventstream
              Input ``eventstream`` with new synthetic events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.LostUsersEvents`
+
 
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import LostUsersEvents, LostUsersParams
         from retentioneering.graph.nodes import EventsNode
         from retentioneering.graph.p_graph import PGraph
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/negative_target.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/negative_target.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 
 from ..types import EventstreamType
 
 
 class NegativeTargetHelperMixin:
     def negative_target(self, negative_target_events: List[str], func: Optional[Callable] = None) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates new synthetic events in each user's path
-        who have specified event(s) - ``negative_target_RAW_EVENT_NAME``.
-        And adds them to the input ``eventstream``.
+        A method of ``Eventstream`` class that creates new synthetic
+        events in paths of all users having the specified events - ``negative_target_RAW_EVENT_NAME``.
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.NegativeTarget`
+
 
         Returns
         -------
         Eventstream
             Input ``eventstream`` with new synthetic events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.NegativeTarget`
+
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             NegativeTarget,
             NegativeTargetParams,
         )
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/new_users_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/new_users_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 
 from ..types import EventstreamType
 
 
 class NewUsersHelperMixin:
     def add_new_users(self, new_users_list: Union[List[int], Literal["all"]]) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates one of synthetic events in each user's path:
-        ``new_user`` or ``existing_user``. And adds them to the input ``eventstream``.
+        A method of ``Eventstream`` class that creates one
+        of the synthetic events in each user's path: ``new_user`` or ``existing_user`` .
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.NewUsersEvents`
 
         Returns
         -------
         Eventstream
              Input ``eventstream`` with new synthetic events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.NewUsersEvents`
+
         """
         # avoid circular import
         from retentioneering.data_processors_lib import NewUsersEvents, NewUsersParams
         from retentioneering.graph.nodes import EventsNode
         from retentioneering.graph.p_graph import PGraph
 
         p = PGraph(source_stream=self)  # type: ignore
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/positive_target.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/positive_target.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 
 from ..types import EventstreamType
 
 
 class PositiveTargetHelperMixin:
     def positive_target(self, positive_target_events: List[str], func: Optional[Callable] = None) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates new synthetic events in each user's path
-        who have specified event(s) - ``positive_target_RAW_EVENT_NAME``.
-        And adds them to the input ``eventstream``.
+        A method of ``Eventstream`` class that creates new synthetic
+        events in paths of all users having the specified events - ``positive_target_RAW_EVENT_NAME``.
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.PositiveTarget`
 
         Returns
         -------
         Eventstream
             Input ``eventstream`` with new synthetic events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.PositiveTarget`
+
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             PositiveTarget,
             PositiveTargetParams,
         )
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/rename_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/rename_helper.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/split_session_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/split_session_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,30 +11,31 @@
     def split_sessions(
         self,
         session_cutoff: Tuple[float, DATETIME_UNITS],
         session_col: str = "session_id",
         mark_truncated: Optional[bool] = False,
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates new synthetic events in each user's path:
+        A method of ``Eventstream`` class that creates new synthetic events in each user's path:
         ``session_start`` (or ``session_start_truncated``) and ``session_end`` (or ``session_end_truncated``).
-        Those events divide user's paths on sessions.
-        Also creates new column which contains session number for each event in input eventstream
-        Session number will take the form: ``{user_id}_{session_number through one user path}``
-        And adds those events and the new column to the input ``eventstream``.
+        The created events divide users' paths on sessions.
+        Also creates a new column that contains session number for each event in the input eventstream
+        Session number will take the form: ``{user_id}_{session_number through one user path}``.
+        The created events and column are added to the input eventstream.
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.SplitSessions`
 
         Returns
         -------
         Eventstream
              Input ``eventstream`` with new synthetic events and ``session_col``.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        Parameters and details :py:class:`.SplitSessions`
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             SplitSessions,
             SplitSessionsParams,
         )
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/start_end_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/start_end_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 
 from ..types import EventstreamType
 
 
 class StartEndHelperMixin:
     def add_start_end(self) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates two synthetic events in each user's path:
-        ``path_start`` and ``path_end``. And adds them to the input ``eventstream``.
+        A method of ``Eventstream`` class that creates
+        two synthetic events in each user's path: ``path_start`` and ``path_end``.
 
         Returns
         -------
         Eventstream
-            Input ``eventstream`` with new synthetic events.
+            Input ``eventstream`` with added synthetic events. See details :py:class:`.StartEndEvents`.
+
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.StartEndEvents`
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             StartEndEvents,
             StartEndEventsParams,
         )
         from retentioneering.graph.nodes import EventsNode
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/truncate_path_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncate_path_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,26 +12,29 @@
         drop_after: Optional[str] = None,
         occurrence_before: Literal["first", "last"] = "first",
         occurrence_after: Literal["first", "last"] = "first",
         shift_before: int = 0,
         shift_after: int = 0,
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which truncates each user's path on the base of
+        A method of ``Eventstream`` class that truncates each user's path based on the
         specified event(s) and selected parameters.
 
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.TruncatePath`
+
         Returns
         -------
         Eventstream
              Input ``eventstream`` with truncated paths.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.TruncatePath`
+
         """
         # avoid circular import
         from retentioneering.data_processors_lib import TruncatePath, TruncatePathParams
         from retentioneering.graph.nodes import EventsNode
         from retentioneering.graph.p_graph import PGraph
 
         p = PGraph(source_stream=self)  # type: ignore
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/helpers/truncated_events_helper.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncated_events_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 class TruncatedEventsHelperMixin:
     def truncated_events(
         self,
         left_truncated_cutoff: Optional[Tuple[float, DATETIME_UNITS]],
         right_truncated_cutoff: Optional[Tuple[float, DATETIME_UNITS]],
     ) -> EventstreamType:
         """
-        Method of ``Eventstream Class`` which creates new synthetic event(s) for each user on the
-        base of timeout threshold: ``truncated_left`` and ``truncated_right``.
-        And adds them to the input ``eventstream``.
+        A method of ``Eventstream`` class that creates new synthetic event(s) for each user based
+        on the timeout threshold: ``truncated_left`` and ``truncated_right``.
+
+
+        Parameters
+        ----------
+        See parameters description
+            :py:class:`.TruncatedEvents`
 
         Returns
         -------
         Eventstream
             Input ``eventstream`` with new synthetic events.
 
-        Notes
-        -----
-        See parameters and details of dataprocessor functionality
-        :py:class:`.TruncatedEvents`
+
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             TruncatedEvents,
             TruncatedEventsParams,
         )
         from retentioneering.graph.nodes import EventsNode
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/schema.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,31 @@
     RawDataSchemaType,
 )
 
 
 @dataclass
 class EventstreamSchema(EventstreamSchemaType):
     """
-    Create schema for ``eventstream`` columns names.
-    If names of the columns are different from default names they should be
+    Define a schema for ``eventstream`` columns names.
+    If names of the columns are different from default names, they need to be
     specified.
 
     Parameters
     ----------
     event_id : str, default "event_id"
     event_type : str, default "event_type"
     event_index : str, default "event_index"
     event_name : str, default "event"
     event_timestamp : str, default "timestamp"
     user_id : str, default "user_id"
-    custom_cols : list, optional
+    custom_cols : list of str, optional
+
+    Notes
+    -----
+    See :ref:`Eventstream user guide<eventstream_field_names>` for the details.
 
     """
 
     event_id: str = "event_id"
     event_type: str = "event_type"
     event_index: str = "event_index"
     event_name: str = "event"
@@ -89,25 +93,30 @@
             custom_cols=custom_cols,
         )
 
 
 @dataclass
 class RawDataSchema(RawDataSchemaType):
     """
-    Create schema for ``raw_data`` columns names.
-    If names of the columns are different from default names they should be
+    Define schema for ``raw_data`` columns names.
+    If names of the columns are different from default names, they need to be
     specified.
 
     Parameters
     ----------
     event_name : str, default "event"
     event_timestamp : str, default "timestamp"
     user_id : str, default "user_id"
     event_type : str, optional
     custom_cols : list, optional
+
+    Notes
+    -----
+    See :ref:`Eventstream user guide<eventstream_custom_fields>` for the details.
+
     """
 
     event_name: str = "event"
     event_timestamp: str = "timestamp"
     user_id: str = "user_id"
     event_type: Optional[str] = None
     custom_cols: List[RawDataCustomColSchema] = field(default_factory=list)
```

### Comparing `retentioneering-3.0.0b0/retentioneering/eventstream/types.py` & `retentioneering-3.0.0b1/retentioneering/eventstream/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from dataclasses import field
-from typing import Any, List, Optional, Protocol, TypedDict
+from typing import Any, List, Optional, Protocol, TypedDict, runtime_checkable
 
 import pandas as pd
 
 IndexOrder = List[Optional[str]]
 
 
 class Relation(TypedDict):
     eventstream: "EventstreamType"
     raw_col: Optional[str]
 
 
+@runtime_checkable
 class EventstreamType(Protocol):
     schema: EventstreamSchemaType
     index_order: IndexOrder
     relations: List[Relation]
     __raw_data_schema: RawDataSchemaType
     __events: pd.DataFrame | pd.Series[Any]
```

### Comparing `retentioneering-3.0.0b0/retentioneering/exceptions/server.py` & `retentioneering-3.0.0b1/retentioneering/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/graph/nodes.py` & `retentioneering-3.0.0b1/retentioneering/graph/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,26 @@
         super().__init__()
         self.events = source
         self.description = description
 
 
 class EventsNode(BaseNode):
     """
-    A class for a regular node of a preprocessing graph
+    Class for regular nodes of a preprocessing graph.
+
+    Notes
+    -----
+    See :doc:`Preprocessing user guide</user_guides/preprocessing>` for the details.
+
+    See Also
+    --------
+    .PGraph.add_node : Add a node to Pgraph.
+    .PGraph.combine : Run calculations of Preprocessing Graph.
+    .MergeNode
+
     """
 
     processor: DataProcessor
     events: Optional[EventstreamType]
     description: Optional[str]
 
     def __init__(self, processor: DataProcessor, description: Optional[str] = None) -> None:
@@ -61,15 +72,26 @@
 
     def calc_events(self, parent: EventstreamType) -> None:
         self.events = self.processor.apply(parent)
 
 
 class MergeNode(BaseNode):
     """
-    A class for a merging node of a preprocessing graph
+    Class for merging nodes of a preprocessing graph.
+
+    Notes
+    -----
+    See :doc:`Preprocessing user guide</user_guides/preprocessing>` for the details.
+
+    See Also
+    --------
+    .PGraph.add_node : Add a node to Pgraph.
+    .PGraph.combine : Run calculations of Preprocessing Graph.
+    .EventsNode
+
     """
 
     events: Optional[EventstreamType]
     description: Optional[str]
 
     def __init__(self, description: Optional[str] = None) -> None:
         super().__init__()
```

### Comparing `retentioneering-3.0.0b0/retentioneering/graph/p_graph.py` & `retentioneering-3.0.0b1/retentioneering/graph/p_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,24 @@
     msg: Optional[str]
     fields_errors: List[FieldErrorDesc]
 
 
 class PGraph:
     """
     Collection of methods for preprocessing graph construction and calculation.
+
+    Parameters
+    ----------
+    source_stream : EventstreamType
+        Source eventstream.
+
+    Notes
+    -----
+    See :doc:`Preprocessing user guide</user_guides/preprocessing>` for the details.
+
     """
 
     root: SourceNode
     combine_result: EventstreamType | None
     _ngraph: networkx.DiGraph
     __server_manager: ServerManager | None = None
     __server: JupyterServer | None = None
@@ -76,28 +86,29 @@
     def add_node(self, node: Node, parents: List[Node]) -> None:
         """
         Add node to ``PGraph`` instance.
 
         Parameters
         ----------
         node : Node
-            Instance of class ``EventsNode`` or ``MergeNode``.
-        parents : list of Node
+            An instance of either ``EventsNode`` or ``MergeNode``.
+        parents : list of Nodes
 
-            - If ``node`` is ``EventsNode`` - it should be only 1 parent
-            - If ``node`` is ``MergeNode`` - it should be at least 2 parents
+            - If ``node`` is ``EventsNode`` - only 1 parent must be defined.
+            - If ``node`` is ``MergeNode`` - at least 2 parents have to be defined.
 
         Returns
         -------
         None
 
-        Notes
-        -----
-        Adding node doesn't run calculations.
-        See :py:func:`combine`.
+        See Also
+        --------
+        PGraph.combine : Adding a node doesn't cause graph recalculation.
+        .EventsNode
+        .MergeNode
 
         """
         self.__valiate_already_exists(node)
         self.__validate_not_found(parents)
 
         if node.events is not None:
             self.__validate_schema(node.events)
@@ -108,25 +119,25 @@
         self._ngraph.add_node(node)
 
         for parent in parents:
             self._ngraph.add_edge(parent, node)
 
     def combine(self, node: Node) -> EventstreamType:
         """
-        Run calculation from the ``SourceNode`` up to specified ``node``.
+        Run calculations from the ``SourceNode`` up to the specified ``node``.
 
         Parameters
         ----------
         node : Node
-            Instance of the class ``SourceNode``, ``EventsNode`` or ``MergeNode``
+            Instance of either ``SourceNode``, ``EventsNode`` or ``MergeNode``.
 
         Returns
         -------
         EventstreamType
-            ``Eventstream`` with all changes after data processors apply.
+            ``Eventstream`` with all changes applied by data processors.
         """
         self.__validate_not_found([node])
 
         if isinstance(node, SourceNode):
             return node.events.copy()
 
         if isinstance(node, EventsNode):
@@ -154,20 +165,20 @@
 
         node.events = curr_eventstream
 
         return cast(EventstreamType, curr_eventstream)
 
     def get_parents(self, node: Node) -> List[Node]:
         """
-        Show parents of specified ``node``.
+        Show parents of the specified ``node``.
 
         Parameters
         ----------
         node : Node
-            Instance of the class SourceNode, EventsNode or MergeNode
+            Instance of one of the classes SourceNode, EventsNode or MergeNode.
 
         """
         self.__validate_not_found([node])
         parents: List[Node] = []
 
         for parent in self._ngraph.predecessors(node):
             parents.append(parent)
@@ -222,15 +233,15 @@
                     server_id=self.__server.pk, env=self.__server_manager.check_env(), width=width, height=height
                 )
             )
         )
 
     def export(self, payload: dict[str, Any]) -> dict:
         """
-        Show ``PGraph`` as config.
+        Show ``PGraph`` as a dict.
 
         Parameters
         ----------
         payload : dict
 
         Returns
         -------
```

### Comparing `retentioneering-3.0.0b0/retentioneering/nodelist/nodelist.py` & `retentioneering-3.0.0b1/retentioneering/nodelist/nodelist.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import pandas as pd
 
 
 class Nodelist:
     nodelist_df: pd.DataFrame
 
-    def __init__(self, event_col: str, time_col: str, nodelist_default_col: str, custom_cols: list[str]) -> None:
+    def __init__(self, event_col: str, time_col: str, weight_cols: list[str]) -> None:
         self.event_col = event_col
         self.time_col = time_col
-        self.nodelist_default_col = nodelist_default_col
-        self.custom_cols = custom_cols
+        self.weight_cols = weight_cols
 
     def calculate_nodelist(self, data: pd.DataFrame) -> pd.DataFrame:
         res: pd.DataFrame = data.groupby([self.event_col])[self.time_col].count().reset_index()
-        if self.custom_cols is not None:
-            for weight_col in self.custom_cols:
+        if self.weight_cols is not None:
+            for weight_col in self.weight_cols:
+                if weight_col == self.event_col:
+                    continue
                 by_col = data.groupby([self.event_col])[weight_col].nunique().reset_index()
                 res = res.join(by_col[weight_col])
 
         res = res.sort_values(by=self.time_col, ascending=False)
-        res.rename(columns={self.time_col: self.nodelist_default_col}, inplace=True)
-
+        res = res.drop(columns=[self.time_col], axis=1)
         res["active"] = True
         res["alias"] = False
         res["parent"] = None
         res["changed_name"] = None
 
         self.nodelist_df = res
         return res
```

### Comparing `retentioneering-3.0.0b0/retentioneering/params_model/params_model.py` & `retentioneering-3.0.0b1/retentioneering/params_model/params_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
+import warnings
 from collections.abc import Iterable
 from dataclasses import asdict
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Type, Union
 
 from pydantic import BaseModel, ValidationError, validator
 from typing_extensions import TypedDict
 
 from retentioneering.exceptions.widget import WidgetParseError
 from retentioneering.params_model.registry import register_params_model
 from retentioneering.utils.dict import clear_dict
 from retentioneering.widget import WIDGET_MAPPING
 
+# disable warning for pydantic schema Callable type
+warnings.simplefilter(action="ignore", category=UserWarning)
+
 if TYPE_CHECKING:
     from pydantic.typing import AbstractSetIntStr, MappingIntStrAny
 
 
 class CustomWidgetProperties(TypedDict):
     widget: str
     serialize: Callable
```

### Comparing `retentioneering-3.0.0b0/retentioneering/params_model/registry.py` & `retentioneering-3.0.0b1/retentioneering/params_model/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/templates/p_graph/p_graph.html` & `retentioneering-3.0.0b1/retentioneering/templates/p_graph/p_graph.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/templates/p_graph/show.py` & `retentioneering-3.0.0b1/retentioneering/templates/p_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/templates/transition_graph/full.html` & `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/full.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/templates/transition_graph/init_template.py` & `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/init_template.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/templates/transition_graph/inner_iframe.html` & `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/inner_iframe.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/templates/transition_graph/show.py` & `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/clusters/clusters.py` & `retentioneering-3.0.0b1/retentioneering/tooling/clusters/clusters.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 Method = Literal["kmeans", "gmm"]
 PlotType = Literal["cluster_bar"]
 PlotProjectionMethod = Literal["tsne", "umap"]
 
 
 class Clusters:
     """
-    A class that holds the methods for cluster analysis.
+    A class that holds methods for the cluster analysis.
 
     Parameters
     ----------
     eventstream : EventstreamType
 
     See Also
     --------
-    :py:meth:`.Eventstream.clusters`
+    .Eventstream.clusters : Call Clusters tool as an eventstream method.
+
+    Notes
+    -----
+    See :doc:`Clusters user guide</user_guides/clusters>` for the details.
     """
 
     def __init__(self, eventstream: EventstreamType):
         self.__eventstream: EventstreamType = eventstream
         self.user_col = eventstream.schema.user_id
         self.event_col = eventstream.schema.event_name
         self.time_col = eventstream.schema.event_timestamp
@@ -66,36 +70,39 @@
         method: Method,
         n_clusters: int,
         feature_type: FeatureType | None = None,
         ngram_range: NgramRange | None = None,
         vector: pd.DataFrame | None = None,
     ) -> Clusters:
         """
-        Fits clusters to the eventstream data.
+        Prepare features and compute clusters for the input eventstream data.
 
         Parameters
         ----------
         method : {"kmeans", "gmm"}
-            - ``kmeans`` stands for classic K-means algorithm. See details in :sklearn_kmeans:`sklearn documentation<>`
-            - ``gmm`` stands for Gaussian mixture model. See details in :sklearn_gmm:`sklearn documentation<>`
+            - ``kmeans`` stands for the classic K-means algorithm.
+              See details in :sklearn_kmeans:`sklearn documentation<>`.
+            - ``gmm`` stands for Gaussian mixture model. See details in :sklearn_gmm:`sklearn documentation<>`.
 
         n_clusters : int
             The expected number of clusters to be passed to a clustering algorithm.
         feature_type : {"tfidf", "count", "frequency", "binary", "markov", "time", "time_fraction"}, default None
-            See :py:func:`extract_features`
+            See :py:func:`extract_features`.
         ngram_range : Tuple(int, int), optional
-            See :py:func:`extract_features`
+            See :py:func:`extract_features`.
         vector : pd.DataFrame, optional
-            ``pd.DataFrame`` representing custom vectorization of the user paths. The index corresponds to user_ids,
+            ``pd.DataFrame`` representing a custom vectorization of the user paths. The index corresponds to user_ids,
             the columns are vectorized values of the path.
 
         Returns
         -------
         Clusters
             A fitted ``Clusters`` instance.
+
+
         """
 
         self._method, self._n_clusters, self._feature_type, self._ngram_range, self._vector = self.__validate_input(
             method, n_clusters, feature_type, ngram_range, vector
         )
 
         self.__features, self.__cluster_result = self._prepare_clusters()
@@ -116,38 +123,43 @@
         cluster_id2: int | None = None,
         top_n: int = 8,
         weight_col: str | None = None,
         targets: list[str] | None = None,
     ) -> go.Figure:
         """
         Plots a bar plot illustrating the distribution of ``top_n`` events in cluster ``cluster_id1``
-        compared vs the entire dataset or vs cluster ``cluster_id2``.
+        compared with the entire dataset or the cluster ``cluster_id2`` if specified.
+        Should be used after :py:func:`fit` or :py:func:`set_clusters`.
+
 
         Parameters
         ----------
         cluster_id1 : int
             ID of the cluster to compare.
         cluster_id2 : int, optional
-            ID of the second cluster to compare with top events from first
-            cluster. If None, then compares with entire dataset.
+            ID of the second cluster to compare with the first
+            cluster. If ``None``, then compares with the entire dataset.
         top_n : int, default 8
             Number of top events.
         weight_col : str, optional
-            If None distribution will be compared based on events occurrences in
+            If ``None``, distribution will be compared based on event occurrences in
             datasets. If ``weight_col`` is specified, percentages of users
             (column name specified by parameter ``weight_col``) who have particular
             events will be plotted.
         targets : list of str, optional
-            List of event names always to include for comparison regardless
+            List of event names always to include for comparison, regardless
             of the parameter top_n value. Target events will appear in the same
             order as specified.
 
+
+
         Returns
         -------
-        Plots the distribution barchart.
+        matplotlib.axes.Axes
+            Plots the distribution barchart.
         """
         if not self.__is_fitted:
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
         cluster1 = self.filter_cluster(cluster_id1).to_dataframe()
 
         if targets is None:
@@ -210,16 +222,16 @@
             cl2=cluster_id2,
         )
 
         return figure
 
     def plot(self, targets: list[str] | list[list[str]] | None = None) -> go.Figure:
         """
-        Plots a bar plot illustrating the clusters sizes and the conversion rates of
-        the ``targets`` events within the clusters.
+        Plot a bar plot illustrating the cluster sizes and the conversion rates of
+        the ``target`` events within the clusters. Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
         targets : list of str (optional, default None)
             Represents the list of the target events
 
         """
@@ -232,53 +244,53 @@
             target=cast(List[List[bool]], targets_bool),  # @TODO: fix types. Vladimir Makhanov
             target_names=target_names,
         )
 
     @property
     def user_clusters(self) -> pd.Series | None:
         """
-        Returns ``user_id -> cluster_id`` mapping representing as ``pd.Series``. The index corresponds to
-        user_ids, the values relate to the corresponding cluster_ids.
 
         Returns
         -------
         pd.Series
+            ``user_id -> cluster_id`` mapping representing as ``pd.Series``. The index corresponds to
+            user_ids, the values relate to the corresponding cluster_ids.
         """
         if not self.__is_fitted:
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
         return self.__cluster_result
 
     @property
     def cluster_mapping(self) -> dict:
         """
-        Returns ``cluster_id -> list[user_ids]`` mapping.
+        Return calculated before ``cluster_id -> list[user_ids]`` mapping.
 
         Returns
         -------
         dict
-            The keys are cluster_ids, the values are the lists of the user_ids related to the corresponding cluster.
+            The keys are cluster_ids, and the values are the lists of the user_ids related to the corresponding cluster.
         """
         if not self.__is_fitted or self.__cluster_result is None:
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
         df = self.__cluster_result.to_frame("cluster_id").reset_index()
         user_col, cluster_col = df.columns
         cluster_map = df.groupby(cluster_col)[user_col].apply(list)  # type: ignore
         return cluster_map.to_dict()
 
     @property
     def features(self) -> pd.DataFrame | None:
         """
-        Returns the calculated features if the clusters are fitted. The index corresponds to user_ids,
-        the columns are values of the vectorized user's trajectory.
 
         Returns
         -------
         pd.DataFrame
+            The calculated features if the clusters are fitted. The index corresponds to user_ids,
+            the columns are values of the vectorized user's trajectory.
         """
         if self.__features is None:
             raise RuntimeError("The features are not calculated. Consider to run 'extract_features()` method.")
 
         return self.__features
 
     @property
@@ -292,15 +304,15 @@
             "n_clusters": self._n_clusters,
             "ngram_range": self._ngram_range,
             "feature_type": self._feature_type,
         }
 
     def set_clusters(self, user_clusters: pd.Series) -> Clusters:
         """
-        Sets custom user-cluster mapping.
+        Set custom user-cluster mapping.
 
         Parameters
         ----------
         user_clusters : pd.Series
             Series index corresponds to user_ids. Values are cluster_ids.
 
         Returns
@@ -316,15 +328,16 @@
         self._method = None
         self._ngram_range = None
         self.__is_fitted = True
         return self
 
     def filter_cluster(self, cluster_id: int | str) -> EventstreamType:
         """
-        Truncate the eventstream and leave the trajectories of the users who belong to the selected cluster.
+        Truncate the eventstream, leaving the trajectories of the users who belong to the selected cluster.
+        Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
         cluster_id : int or str
             Cluster identifier to be selected.
 
             If :py:func:`create_clusters` was used for cluster generation, then
@@ -358,28 +371,30 @@
     def extract_features(self, feature_type: FeatureType, ngram_range: NgramRange | None = None) -> pd.DataFrame:
         """
         Calculate vectorized user paths.
 
         Parameters
         ----------
         feature_type : {"tfidf", "count", "frequency", "binary", "markov", "time", "time_fraction"}
+            Algorithms for converting text sequences to numerical vectors:
 
             - ``tfidf`` see details in :sklearn_tfidf:`sklearn documentation<>`
             - ``count`` see details in :sklearn_countvec:`sklearn documentation<>`
-            - | ``frequency`` the same as count but normalized to the total number of the events
-              | in the user's trajectory.
-            - ``binary`` 1 if a user had given n-gram at least once and 0 otherwise.
-            - | ``markov`` available for bigrams only. For a given bigram ``(A, B)`` the vectorized values
-              | are the user's transition probabilities from ``A`` to ``B``.
-            - | ``time`` Associated with unigrams only. The total number of the seconds spent from the
-              | beginning of a user's path until a given event.
-            - | ``time_fraction`` the same as ``time`` but divided by the total length of the user's trajectory
-              | (in seconds).
+            - ``frequency`` is similar to count, but normalized to the total number of the events
+              in the user's trajectory.
+            - ``binary`` 1 if a user had the given n-gram at least once and 0 otherwise.
+            - ``markov`` available for bigrams only. For a given bigram ``(A, B)`` the vectorized values
+              are the user's transition probabilities from ``A`` to ``B``.
+            - ``time`` associated with unigrams only. The total number of the seconds spent
+              from the beginning of a user's path until the given event.
+            - ``time_fraction`` the same as ``time`` but divided by the total length of the user's trajectory
+              (in seconds).
+
         ngram_range : Tuple(int, int)
-            The lower and upper boundary of the range of n-values for different word n-grams or char n-grams to be
+            The lower and upper boundary of the range of n-values for different word n-grams to be
             extracted. For example, ngram_range=(1, 1) means only single events, (1, 2) means single events
             and bigrams. Ignored for ``markov``, ``time``, ``time_fraction`` feature types.
 
         Returns
         -------
         pd.DataFrame
             A DataFrame with the vectorized values. Index contains user_ids, columns contain n-grams.
@@ -422,33 +437,34 @@
         self,
         method: PlotProjectionMethod = "tsne",
         targets: list[str] | None = None,
         plot_type: Literal["targets", "clusters"] = "clusters",
         **kwargs: Any,
     ) -> go.Figure:
         """
-        Shows the clusters projection on a plane applying dimension reduction techniques.
+        Show the clusters' projection on a plane, applying dimension reduction techniques.
+        Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
         method : {'umap', 'tsne'}, default 'tsne'
             Type of manifold transformation.
         plot_type : {'targets', 'clusters'}, default 'clusters'
             Type of color-coding used for projection visualization:
 
             - ``clusters`` colors trajectories with different colors depending on cluster number.
-            - | ``targets`` colors trajectories based on reach to any event provided in 'targets' parameter.
-              | Must provide ``targets`` parameter in this case.
+            - ``targets`` colors trajectories based on reach to any event provided in 'targets' parameter.
+              Must provide ``targets`` parameter in this case.
 
         targets : list or tuple of str, optional
-            Vector of event_names as str. If user reach any of the specified events, the dot corresponding
+            Vector of event_names as str. If user reaches any of the specified events, the dot corresponding
             to this user will be highlighted as converted on the resulting projection plot.
 
         **kwargs : optional
-            Parameters for ``sklearn.manifold.TSNE()`` and ``umap.UMAP()``
+            Parameters for :sklearn_tsne:`sklearn.manifold.TSNE()<>` and :umap:`umap.UMAP()<>`.
 
         Returns
         -------
         sns.scatterplot
             Plot in the low-dimensional space for user trajectories indexed by user IDs.
         """
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/clusters/segments.py` & `retentioneering-3.0.0b1/retentioneering/tooling/clusters/segments.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/clusters/userlist.py` & `retentioneering-3.0.0b1/retentioneering/tooling/clusters/userlist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/cohorts/cohorts.py` & `retentioneering-3.0.0b1/retentioneering/tooling/cohorts/cohorts.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from retentioneering.eventstream.types import EventstreamType
 
 # @TODO Подумать над сокращением списка поддерживаемых типов для когорт? dpanina
 
 
 class Cohorts:
     """
-    A class which provides methods for cohort analysis. The users are split into groups
-    depending on the time of their first appearance in the eventstream so each user is
-    associated with some ``cohort_group``. The retention rate of the active users
-    belonging to each ``cohort_group`` is  calculated within each ``cohort_period``.
+    A class that provides methods for cohort analysis. The users are split into groups
+    depending on the time of their first appearance in the eventstream; thus each user is
+    associated with some ``cohort_group``. Retention rates of the active users
+    belonging to each ``cohort_group`` are  calculated within each ``cohort_period``.
 
     Parameters
     ----------
     eventstream : EventstreamType
     cohort_start_unit : :numpy_link:`DATETIME_UNITS<>`
-        The way of rounding and format of the moment from which the cohort count begins.
-        Minimum timestamp rounding down to the selected datetime unit.
+        The way of rounding and formatting of the moment from which the cohort count begins.
+        The minimum timestamp is rounded down to the selected datetime unit.
 
         For example:
-        We have eventstream with minimum timestamp - "2021-12-28 09:08:34.432456"
-        The result of roundings with different ``DATETIME_UNITS`` is in the table below:
+        assume we have an eventstream with the following minimum timestamp - "2021-12-28 09:08:34.432456".
+        The result of roundings with different ``DATETIME_UNITS`` is shown in the table below:
 
         +------------------------+-------------------------+
         | **cohort_start_unit**  | **cohort_start_moment** |
         +------------------------+-------------------------+
         | Y                      |  2021-01-01 00:00:00    |
         +------------------------+-------------------------+
         | M                      |  2021-12-01 00:00:00    |
@@ -42,42 +42,46 @@
         +------------------------+-------------------------+
         | D                      |  2021-08-28 00:00:00    |
         +------------------------+-------------------------+
 
     cohort_period : Tuple(int, :numpy_link:`DATETIME_UNITS<>`)
         The cohort_period size and its ``DATETIME_UNIT``. This parameter is used in calculating:
 
-        - Start moments for each cohort from the moment defined with the ``cohort_start_unit`` parameter
-        - Cohort periods for each cohort from ifs start moment.
+        - Start moments for each cohort from the moment specified with the ``cohort_start_unit`` parameter
+        - Cohort periods for each cohort from its start moment.
     average : bool, default True
         - If ``True`` - calculating average for each cohort period.
-        - If ``False`` - averaged values don't calculated.
+        - If ``False`` - averaged values aren't calculated.
     cut_bottom : int, default 0
         Drop 'n' rows from the bottom of the cohort matrix.
         Average is recalculated.
     cut_right : int, default 0
         Drop 'n' columns from the right side of the cohort matrix.
         Average is recalculated.
     cut_diagonal : int, default 0
         Replace values in 'n' diagonals (last period-group cells) with ``np.nan``.
         Average is recalculated.
 
+    See Also
+    --------
+    .Eventstream.cohorts : Call Cohorts tool as an eventstream method.
+    .EventTimestampHist : Plot the distribution of events over time.
+    .UserLifetimeHist : Plot the distribution of user lifetimes.
+
     Notes
     -----
     Parameters ``cohort_start_unit`` and ``cohort_period`` should be consistent.
-    Due to "Y" and "M" are non-fixed types it can be used only with each other
+    Due to "Y" and "M" being non-fixed types, it can be used only with each other
     or if ``cohort_period_unit`` is more detailed than ``cohort_start_unit``.
     More information - :numpy_timedelta_link:`about numpy timedelta<>`
 
+    Only cohorts with at least 1 user in some period are shown.
 
-    Only cohorts with at least 1 user in any period - are shown.
+    See :doc:`Cohorts user guide</user_guides/cohorts>` for the details.
 
-    See Also
-    --------
-    :py:meth:`.Eventstream.cohorts`
     """
 
     __eventstream: EventstreamType
     cohort_period: int
     cohort_period_unit: DATETIME_UNITS
     cohort_start_unit: DATETIME_UNITS
 
@@ -175,15 +179,15 @@
             df.loc[row, max(0, df.loc[row].notna()[::-1].idxmax() + 1 - cut_diagonal) :] = None  # type: ignore
 
         return df.iloc[: len(df) - cut_bottom, : len(df.columns) - cut_right]
 
     def fit(self) -> None:
         """
         Calculates the cohort internal values with the defined parameters.
-        Applying ``fit`` method is mandatory for the following usage
+        Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``Cohorts`` methods.
 
         """
 
         df = self._add_min_date(
             data=self.data,
             cohort_start_unit=self.cohort_start_unit,
@@ -236,15 +240,15 @@
 
     def lineplot(
         self,
         show_plot: Literal["cohorts", "average", "all"] = "cohorts",
         figsize: Tuple[float, float] = (10, 10),
     ) -> sns.lineplot:
         """
-        Creates a chart representing each cohort dynamics over time.
+        Create a chart representing each cohort dynamics over time.
         Should be used after :py:func:`fit`.
 
         Parameters
         ----------
         show_plot: 'cohorts', 'average' or 'all'
             - if ``cohorts`` - shows a lineplot for each cohort,
             - if ``average`` - shows a lineplot only for the average values over all the cohorts,
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/describe/describe.py` & `retentioneering-3.0.0b1/retentioneering/tooling/describe/describe.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/describe_events/describe_events.py` & `retentioneering-3.0.0b1/retentioneering/tooling/describe_events/describe_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py` & `retentioneering-3.0.0b1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,33 +11,45 @@
 
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.constants import BINS_ESTIMATORS
 
 
 class EventTimestampHist:
     """
-    A class for visualize the distribution of events over time.
+    Plot the distribution of events over time. Can be useful for detecting
+    time-based anomalies, and visualising general timespan of the eventstream.
 
     Parameters
     ----------
     raw_events_only : bool, default False
-        If ``True`` - statistics will be shown only for raw events.
-        If ``False`` - for all events presented in your data.
+        If ``True`` - statistics will only be shown for raw events.
+        If ``False`` - statistics will be shown for all events presented in your data.
     event_list : list of str, optional
-        Specify the events to be displayed.
+        Specify events to be displayed.
     lower_cutoff_quantile : float, optional
-        Specify the time distance quantile as the lower boundary. The values below the boundary are truncated.
+        Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
     upper_cutoff_quantile : float, optional
-        Specify the time distance quantile as the upper boundary. The values above the boundary are truncated.
+        Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
     bins : int or str, default 20
         Generic bin parameter that can be the name of a reference rule or
-        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`
+        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
     figsize : tuple of float, default (12.0, 7.0)
         Width, height in inches.
 
+
+    See Also
+    --------
+    .TimedeltaHist : Plot the distribution of the time deltas between two events.
+    .UserLifetimeHist : Plot the distribution of user lifetimes.
+    .Eventstream.describe : Show general eventstream statistics.
+    .Eventstream.describe_events : Show general eventstream events statistics.
+
+    Notes
+    -----
+    See :ref:`Eventstream user guide<eventstream_events_timestamp>` for the details.
     """
 
     def __init__(
         self,
         eventstream: EventstreamType,
         raw_events_only: bool = False,
         event_list: list[str] | None = None,
@@ -80,16 +92,17 @@
             idx &= series >= series.quantile(self.lower_cutoff_quantile)
         return series[idx]
 
     def fit(self) -> None:
         """
         Calculate values for the histplot.
 
-            1. The first array contains the values for histogram
-            2. The first array contains the bin edges
+        Returns
+        -------
+        None
 
         """
         data = self.__eventstream.to_dataframe()
 
         if self.raw_events_only:
             data = data[data["event_type"].isin(["raw"])]
         if self.event_list:
@@ -111,16 +124,16 @@
     def values(self) -> tuple[np.ndarray, np.ndarray]:
         """
 
         Returns
         -------
         tuple(np.ndarray, np.ndarray)
 
-            1. The first array contains the values for histogram
-            2. The first array contains the bin edges
+            1. The first array contains the values for histogram.
+            2. The first array contains the bin edges.
 
         """
         return self.values_to_plot, self.bins_to_show
 
     def plot(self) -> matplotlib.axes.Axesne:
         """
         Create a sns.histplot based on the calculated values.
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/funnel/funnel.py` & `retentioneering-3.0.0b1/retentioneering/tooling/funnel/funnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,41 @@
 
     Parameters
     ----------
     eventstream : EventstreamType
     stages: list of str
         List of events used as stages for the funnel. Absolute and relative
         number of users who reached specified events at least once will be
-        plotted. Multiple events can be grouped together as individual state
-        by combining them as sub list.
+        plotted. Multiple events can be grouped together as an individual state
+        by combining them as a sub list.
     stage_names: list of str, optional
-        List of stage names, this is especially necessary for stages that include several events.
+        List of stage names, this is necessary for stages that include several events.
     funnel_type: 'open', 'closed' or 'hybrid', default 'closed'
         - if ``open`` - all users will be counted on each stage;
-        - if ``closed`` - each stage will include only users, who was on all previous stages;
-        - | if ``hybrid`` - combination of 2 previous types. The first stage is required for
-          | to go further. And for the second and subsequent stages it is important have
-          | all previous stages in their path, but the order of these events is not taken
-          | into account.
+        - if ``closed`` - each stage will include only users, that were present on all previous stages;
+        - if ``hybrid`` - combination of 2 previous types. The first stage is required
+          to go further. And for the second and subsequent stages it is important to have
+          all previous stages in their path, but the order of these events is not taken
+          into account.
 
     segments: Collection[Collection[int]], optional
         List of user_ids collections. Funnel for each user_id collection will be plotted.
-        If ``None`` - all users from dataset will be plotted. A user can only belong to one segment at a time.
+        If ``None`` - all users from the dataset will be plotted. A user can only belong to one segment at a time.
     segment_names: list of str, optional
         Names of segments. Should be a list from unique values of the ``segment_col``.
         If ``None`` and ``segment_col`` is given - all values from ``segment_col`` will be used.
 
+
     See Also
     --------
-    :py:meth:`.Eventstream.funnel`
+    .Eventstream.funnel : Call Funnel tool as an eventstream method.
+
+    Notes
+    -----
+    See :doc:`Funnel user guide</user_guides/funnel>` for the details.
 
     """
 
     __eventstream: EventstreamType
     __default_layout = dict(
         margin={"l": 180, "r": 0, "t": 30, "b": 0, "pad": 0},
         funnelmode="stack",
@@ -211,16 +216,16 @@
             else:
                 df = df.drop(df[~df[self.user_col].isin(user_stage)].index.tolist())
 
         return vals, df
 
     def fit(self) -> None:
         """
-        Calculates the funnel internal values with the defined parameters.
-        Applying ``fit`` method is mandatory for the following usage
+        Calculate the funnel internal values with the defined parameters.
+        Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``Funnel`` methods.
 
         """
 
         if self.funnel_type in ["closed", "hybrid"]:
             self.res_dict = self._prepare_data_for_closed_and_hybrid_funnel(
                 data=self.data,
@@ -240,15 +245,15 @@
             )
 
         del self.data
         self.data = pd.DataFrame()
 
     def plot(self) -> go.Figure:
         """
-        Creates a funnel plot based on the calculated funnel values.
+        Create a funnel plot based on the calculated funnel values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         go.Figure
 
         """
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/mixins/ended_events.py` & `retentioneering-3.0.0b1/retentioneering/tooling/mixins/ended_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/stattests/stattests.py` & `retentioneering-3.0.0b1/retentioneering/tooling/stattests/stattests.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,44 +27,49 @@
 def _cohenh(d1: list, d2: list) -> float:
     u1, u2 = np.mean(d1), np.mean(d2)
     return 2 * (math.asin(math.sqrt(u1)) - math.asin(math.sqrt(u2)))
 
 
 class StatTests:
     """
-    A class for the determining statistical difference between two groups of users.
+    A class for determining statistical difference between two groups of users.
 
     Parameters
     ----------
     eventstream : EventstreamType
     test : {'mannwhitneyu', 'ttest', 'ztest', 'ks_2samp', 'chi2_contingency', 'fisher_exact'}
         Test the null hypothesis that 2 independent samples are drawn from the same
         distribution. Supported tests are:
 
-        - ``mannwhitneyu`` see :mannwhitneyu:`scipy documentation<>`
-        - ``ttest`` see :statsmodel_ttest:`statsmodels documentation<>`
-        - ``ztest`` see :statsmodel_ztest:`statsmodels documentation<>`
-        - ``ks_2samp`` see :scipy_ks:`scipy documentation<>`
-        - ``chi2_contingency`` see :scipy_chi2:`scipy documentation<>`
-        - ``fisher_exact`` see :scipy_fisher:`scipy documentation<>`
+        - ``mannwhitneyu`` see :mannwhitneyu:`scipy documentation<>`.
+        - ``ttest`` see :statsmodel_ttest:`statsmodels documentation<>`.
+        - ``ztest`` see :statsmodel_ztest:`statsmodels documentation<>`.
+        - ``ks_2samp`` see :scipy_ks:`scipy documentation<>`.
+        - ``chi2_contingency`` see :scipy_chi2:`scipy documentation<>`.
+        - ``fisher_exact`` see :scipy_fisher:`scipy documentation<>`.
 
     groups : tuple of list
-        Must contain tuple of two elements (g_1, g_2): where g_1 and g_2 are collections
+        Must contain a tuple of two elements (g_1, g_2): g_1 and g_2 are collections
         of user_id`s.
     func : Callable
-        Selected metrics. Must contain a function which takes as an argument dataset for
-        single user trajectory and returns a single numerical value.
+        Selected metrics. Must contain a function that takes a dataset as an argument for
+        a single user trajectory and returns a single numerical value.
     group_names : tuple, default ('group_1', 'group_2')
         Names for selected groups g_1 and g_2.
     alpha : float, default 0.05
         Selected level of significance.
 
+
     See Also
     --------
-    :py:meth:`.Eventstream.stattests`
+    .Eventstream.stattests : Call StatTests tool as an eventstream method.
+
+    Notes
+    -----
+    See :doc:`StatTests user guide</user_guides/stattests>` for the details.
 
     """
 
     def __init__(
         self,
         eventstream: EventstreamType,
         test: TEST_NAMES,
@@ -163,16 +168,16 @@
             power = power_rev
             label_max = self.group_names[1]
             label_min = self.group_names[0]
         return p_val, power, label_max, label_min
 
     def fit(self) -> None:
         """
-        Calculates the cohort internal values with the defined parameters.
-        Applying ``fit`` method is mandatory for the following usage
+        Calculates the stattests internal values with the defined parameters.
+        Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StatTests`` methods.
 
         """
         self.g1_data, self.g2_data = self._get_group_values()
         self.p_val, self.power, self.label_min, self.label_max = self._get_sorted_test_results()
         self.is_fitted = True
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/step_matrix/step_matrix.py` & `retentioneering-3.0.0b1/retentioneering/tooling/step_matrix/step_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
             raise ValueError("Occurrence in 'centered' dictionary must be >=1")
         if self.left_gap < 1:
             raise ValueError("left_gap in 'centered' dictionary must be >=1")
 
 
 class StepMatrix(EndedEventsMixin):
     """
-    Step matrix is a matrix where its ``(i, j)`` element means the frequency
-    of event ``i`` occurred as ``j``-th step in user trajectories. This class
-    provides methods for a step matrix calculation and visualization.
+    Step matrix is a matrix where its ``(i, j)`` element shows the frequency
+    of event ``i`` occurring as ``j``-th step in user trajectories. This class
+    provides methods for step matrix calculation and visualization.
 
     Parameters
     ----------
     eventstream : EventstreamType
     max_steps : int, default=20
         Maximum number of steps in ``user path`` to include.
     weight_col : str, optional
@@ -44,66 +44,69 @@
     precision : int, default=2
         Number of decimal digits after 0 to show as fractions in the ``heatmap``.
     targets : list of str or str, optional
         List of event names to include in the bottom of ``step_matrix`` as individual rows.
         Each specified target will have separate color-coding space for clear visualization.
         `Example: ['product_page', 'cart', 'payment']`
 
-        If multiple targets need to be compared and plotted using same color-coding scale,
-        such targets must be combined in sub-list.
-        `Examples: ['product_page', ['cart', 'payment']]`
+        If multiple targets need to be compared and plotted using the same color-coding scale,
+        such targets must be combined in a sub-list.
+        `Example: ['product_page', ['cart', 'payment']]`
     accumulated : {"both", "only"}, optional
         Option to include accumulated values for targets.
 
-        - If ``None`` accumulated tartes  do not show.
-        - If ``both`` show step values and accumulated values.
-        - If ``only`` show targets only as accumulated.
+        - If ``None``, accumulated tartes are not shown.
+        - If ``both``, show step values and accumulated values.
+        - If ``only``, show targets only as accumulated.
     sorting : list of str, optional
-        - | If list of event names specified - lines in the heatmap will be shown in
-          | passed order.
-        - | If ``None`` - rows will be ordered according to i`th value (first row,
-          | where 1st element is max, second row, where second element is max, etc)
+        - If list of event names specified - lines in the heatmap will be shown in
+          the passed order.
+        - If ``None`` - rows will be ordered according to i`th value (first row,
+          where 1st element is max; second row, where second element is max; etc)
     thresh : float, default=0
         Used to remove rare events. Aggregates all rows where all values are
-        less than specified threshold.
+        less than the specified threshold.
     centered : dict, optional
-        Parameter used to align user paths at specific event at specific step.
+        Parameter used to align user paths at a specific event at a specific step.
         Has to contain three keys:
-        - ``event``: str, name of event to align
-        - ``left_gap``: int, number of events to include before specified event
-        - ``occurrence`` : int which occurrence of event to align (typical 1)
+        - ``event``: str, name of event to align.
+        - ``left_gap``: int, number of events to include before specified event.
+        - ``occurrence`` : int which occurrence of event to align (typical 1).
 
-        If not ``None`` - only users who have selected events with specified
+        If not ``None`` - only users who have selected events with the specified
         ``occurrence`` in their paths will be included.
         ``Fraction`` of such remaining users is specified in the title of centered
         step_matrix.
         `Example: {'event': 'cart', 'left_gap': 8, 'occurrence': 1}`
     groups : tuple[list, list], optional
         Can be specified to plot differential step_matrix. Must contain
-        tuple of two elements (g_1, g_2): where g_1 and g_2 are collections
+        a tuple of two elements (g_1, g_2): where g_1 and g_2 are collections
         of user_id`s. Two separate step_matrices M1 and M2 will be calculated
         for users from g_1 and g_2, respectively. Resulting matrix will be the matrix
         M = M1-M2.
 
     Notes
     -----
     During step matrix calculation an artificial ``ENDED`` event is created. If a path already
     contains ``path_end`` event (See :py:class:`.StartEndEvents`), it
     will be temporarily replaced with ``ENDED`` (within step matrix only). Otherwise, ``ENDED``
     event will be explicitly added to the end of each path.
 
     Event ``ENDED`` is cumulated so that the values in its row are summed up from
     the first step to the last. ``ENDED`` row is always placed at the last line of step matrix.
-
-    Also, such a cumulative design guarantees that the sum of any step matrix's column is 1
+    This design guarantees that the sum of any step matrix's column is 1
     (0 for a differential step matrix).
 
+    See :doc:`StepMatrix user guide</user_guides/step_matrix>` for the details.
+
     See Also
     --------
-    :py:meth:`.Eventstream.step_matrix`
+    .Eventstream.step_matrix : Call StepMatrix tool as an eventstream method.
+    .StepSankey : A class for the visualization of user paths in stepwise manner using Sankey diagram.
+    .CollapseLoops : Find loops and create new synthetic events in the paths of all users having such sequences.
     """
 
     __eventstream: EventstreamType
 
     def __init__(
         self,
         eventstream: EventstreamType,
@@ -388,15 +391,15 @@
                     [centered_position - 0.02, centered_position + 0.98], *axs.get_ylim(), colors="Black", linewidth=0.7
                 )
         return figure
 
     def fit(self) -> None:
         """
         Calculates the step matrix internal values with the defined parameters.
-        Applying ``fit`` method is mandatory for the following usage
+        Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StepMatrix`` methods.
 
         """
         weight_col = self.weight_col or self.user_col
         data = self.__eventstream.to_dataframe()
         data = self._add_ended_events(data, self.__eventstream.schema)
         data["event_rank"] = data.groupby(weight_col).cumcount() + 1
@@ -463,15 +466,15 @@
         self.result_data = piv
         self.result_targets = piv_targets
         self.fraction_title = fraction_title
         self.targets_list = targets_plot
 
     def plot(self) -> sns.heatmap:
         """
-        Creates a heatmap plot based on the calculated step matrix values.
+        Create a heatmap plot based on the calculated step matrix values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         sns.heatmap
 
         """
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/step_sankey/step_sankey.py` & `retentioneering-3.0.0b1/retentioneering/tooling/step_sankey/step_sankey.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,50 +9,56 @@
 
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.mixins.ended_events import EndedEventsMixin
 
 
 class StepSankey(EndedEventsMixin):
     """
-    A class for the visualization of user paths in step-wise manner using Sankey diagram.
+    A class for the visualization of user paths in stepwise manner using Sankey diagram.
 
     Parameters
     ----------
     eventstream : EventstreamType
     max_steps : int, default 10
         Maximum number of steps in trajectories to include. Should be > 1.
     thresh : float | int, default 0.05
         Used to remove rare events from the plot. An event is collapsed to ``thresholded_N`` artificial event if
-        its maximum frequency across all the steps is less than or equal to ``thresh``. The frequency is considered
+        its maximum frequency across all the steps is less than or equal to ``thresh``. The frequency is set
         with respect to ``thresh`` type:
 
         - If ``int`` - the frequency is the number of unique users who had given event at given step.
-        - | If ``float`` - percentage of users: the same as for ``int``, but divided by the number of unique users.
+        - If ``float`` - percentage of users: the same as for ``int``, but divided by the number of unique users.
 
         The events which are prohibited for collapsing could be enlisted in ``target`` parameter.
     sorting : list of str, optional
-        Tunes the order of the events visualized at each step. The events which are not represented in the list
+        Define the order of the events visualized at each step. The events that are not represented in the list
         will follow after the events from the list.
     target : list of str, optional
-        Contains the events which are prohibited for collapsing with ``thresh`` parameter.
+        Contain events that are prohibited for collapsing with ``thresh`` parameter.
     autosize : bool, default True
-        Plotly autosize parameter. See :plotly_autosize:`plotly documentation<>`
+        Plotly autosize parameter. See :plotly_autosize:`plotly documentation<>`.
     width : int, optional
-        Plot's width (in px). See :plotly_width:`plotly documentation<>`
+        Plot's width (in px). See :plotly_width:`plotly documentation<>`.
     height : int, optional
-        Plot's height (in px). See :plotly_height:`plotly documentation<>`
+        Plot's height (in px). See :plotly_height:`plotly documentation<>`.
+
     Raises
     ------
     ValueError
         If ``max_steps`` parameter is <= 1.
 
-
     See Also
     --------
-    :py:meth:`.Eventstream.step_sankey`
+    .Eventstream.step_sankey : Call StepSankey tool as an eventstream method.
+    .CollapseLoops : Find loops and create new synthetic events in the paths of all users having such sequences.
+    .StepMatrix : This class provides methods for step matrix calculation and visualization.
+
+    Notes
+    -----
+    See :doc:`StepSankey user guide</user_guides/step_sankey>` for the details.
 
     """
 
     def __init__(
         self,
         eventstream: EventstreamType,
         max_steps: int = 10,
@@ -527,29 +533,29 @@
         data["next_timestamp"] = grouped[self.time_col].shift(-1)
         data["time_to_next"] = data["next_timestamp"] - data[self.time_col]
         data = data.drop("next_timestamp", axis=1)
         return data
 
     def fit(self) -> None:
         """
-        Calculates the sankey diagram internal values with the defined parameters.
-        Applying ``fit`` method is mandatory for the following usage
+        Calculate the sankey diagram internal values with the defined parameters.
+        Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StepSankey`` methods.
 
         """
         data = self.__eventstream.to_dataframe().copy()[
             [self.user_col, self.event_col, self.time_col, self.event_index_col]
         ]
         self.data = self._prepare_data(data)
         data_for_plot, self.data_grp_nodes = self._get_nodes(self.data)
         self.data_for_plot, self.data_grp_links = self._get_links(self.data, data_for_plot, self.data_grp_nodes)
 
     def plot(self) -> go.Figure:
         """
-        Creates a Sankey interactive plot base on the calculated values.
+        Create a Sankey interactive plot based on the calculated values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         plotly.graph_objects.Figure
 
         """
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/timedelta_hist/timedelta_hist.py` & `retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/timedelta_hist.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     distribution types, such as distribution of time for adjacent consecutive events, or
     for a pair of pre-defined events, or median transition time from event to event per user/session.
 
     Parameters
     ----------
     raw_events_only : bool, default True
         If ``True`` - statistics will be shown only for raw events.
-        If ``False`` - for all events presented in your data.
+        If ``False`` - statistics will be shown for all events presented in your data.
     event_pair : tuple of str, optional
         Specify an event pair to plot the time distance between. The first
         item corresponds to chronologically first event, the second item corresponds to the second event. If
         ``event_pair=None``, plot distribution of timedelta for all adjacent events.
 
         Examples: ('login', 'purchase'); ['start', 'cabinet']
 
@@ -43,15 +43,15 @@
 
     only_adjacent_event_pairs : bool, default True
         Is used only when ``event_pair`` is not ``None``; specifies whether events need to be
         adjacent to be included.
 
         For example, if ``event_pair=("login", "purchase")`` and ``only_adjacent_event_pairs=False``,
         then the sequence ("login", "main", "trading", "purchase") will contain a valid pair
-        (which is not the case with only_adjacent_event_pairs=True)
+        (which is not the case with only_adjacent_event_pairs=True).
 
     weight_col : str, default 'user_id'
         Specify a unit of observation, inside which time differences will be computed.
         For example:
 
         - If ``user_id`` - time deltas will be computed only for events inside each user path.
         - If ``session_id`` - the same, but inside each session.
@@ -61,30 +61,47 @@
 
         - If ``None`` - no aggregation;
         - ``mean`` and ``median`` plot distributions of ``weight_col`` unit mean or unit ``median`` timedeltas.
 
         For example, if session id is specified in ``weight_col``, one observation per
         session (for example, session median) will be provided for the histogram.
     timedelta_unit : :numpy_link:`DATETIME_UNITS<>`, default 's'
-        Specify the units of the time differences the histogram should use. Use "s" for seconds, "m" for minutes,
+        Specify units of time differences the histogram should use. Use "s" for seconds, "m" for minutes,
         "h" for hours and "D" for days.
-    log_scale: bool | tuple of bool | None = None,
+    log_scale: bool | tuple of bool | None, optional
 
          - If ``True`` - apply log scaling to the ``x`` axis.
          - If tuple of bool - apply log scaling to the (``x``,``y``) axes correspondingly.
 
     lower_cutoff_quantile : float, optional
-        Specify the time distance quantile as the lower boundary. The values below the boundary are truncated.
+        Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
     upper_cutoff_quantile : float, optional
-        Specify the time distance quantile as the upper boundary. The values above the boundary are truncated.
+        Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
     bins : int or {"auto", "fd", "doane", "scott", "stone", "rice", "sturges", "sqrt"}, default 20
         Generic bin parameter that can be the name of a reference rule or
-        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`
+        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
     figsize : tuple of float, default (6.0, 4.5)
         Width, height in inches.
+
+    See Also
+    --------
+    .UserLifetimeHist : Plot the distribution of user lifetimes.
+    .EventTimestampHist : Plot the distribution of events over time.
+    .Eventstream.describe : Show general eventstream statistics.
+    .Eventstream.describe_events : Show general eventstream events statistics.
+    .StartEndEvents : Create new synthetic events ``path_start`` and ``path_end`` to each user trajectory.
+    .SplitSessions : Create new synthetic events, that divide users’ paths on sessions.
+    .TruncatedEvents : Create new synthetic event(s) for each user based on the timeout threshold.
+    .DeleteUsersByPathLength : Filter user paths based on the path length, removing the paths that are shorter than the
+                                specified number of events or cut_off.
+
+
+    Notes
+    -----
+    See :ref:`Eventstream user guide<eventstream_timedelta_hist>` for the details.
     """
 
     EVENTSTREAM_START = "eventstream_start"
     EVENTSTREAM_END = "eventstream_end"
 
     def __init__(
         self,
@@ -202,17 +219,17 @@
         data = pd.concat([data, global_events]).sort_values([self.weight_col, self.time_col]).reset_index(drop=True)
         return data
 
     def fit(self) -> None:
         """
         Calculate values and bins for the histplot.
 
-            1. The first array contains the values for histogram
-            2. The first array contains the bin edges
-
+        Returns
+        -------
+        None
         """
         data = self.data.sort_values([self.weight_col, self.time_col])
 
         if self.event_pair is not None and set([self.EVENTSTREAM_START, self.EVENTSTREAM_END]).intersection(
             self.event_pair
         ):
             data = self._prepare_global_events_diff(data)
@@ -238,22 +255,22 @@
     def values(self) -> tuple[np.ndarray, np.ndarray]:
         """
 
         Returns
         -------
         tuple(np.ndarray, np.ndarray)
 
-            1. The first array contains the values for histogram
-            2. The first array contains the bin edges
+            1. The first array contains the values for histogram.
+            2. The first array contains the bin edges.
         """
         return self.values_to_plot, self.bins_to_show
 
     def plot(self) -> matplotlib.axes.Axes:
         """
-        Creates a sns.histplot based on the calculated values.
+        Create a sns.histplot based on the calculated values.
 
         Returns
         -------
         :matplotlib_axes:`matplotlib.axes.Axes<>`
             The matplotlib axes containing the plot.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/typing/transition_graph/graph_types.py` & `retentioneering-3.0.0b1/retentioneering/tooling/typing/transition_graph/graph_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,27 +23,26 @@
 
 class PlotParamsType(TypedDict):
     pass
 
 
 AllowedColors = Literal["red", "green", "yellow", "blue", "magenta", "cyan"]
 
-Threshold = MutableMapping[str, float]
+# @FIXME: idk why import annotation not fixed this cause, and I need to use Union. Vladimir Makhanov
+Threshold = MutableMapping[str, Union[float, int]]  # type: ignore
 NodeParams = MutableMapping[str, Optional[str]]
 Position = MutableMapping[str, Sequence[float]]
 
 
 class GraphSettings(PlotParamsType):
     show_weights: bool
     show_percents: bool
     show_nodes_names: bool
     show_all_edges_for_targets: bool
     show_nodes_without_links: bool
-    nodes_threshold: Threshold
-    links_threshold: Threshold
 
 
 class Weight(TypedDict):
     weight_norm: float
     weight: float
```

### Comparing `retentioneering-3.0.0b0/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py` & `retentioneering-3.0.0b1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,35 +12,52 @@
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.constants import BINS_ESTIMATORS
 
 
 class UserLifetimeHist:
     """
-    A class for visualize a ``users' lifetime``.
+
+    Plot the distribution of user lifetimes. A ``users lifetime`` is the timedelta between
+    the first and the last events of the user.
 
     Parameters
     ----------
     timedelta_unit : :numpy_link:`DATETIME_UNITS<>`, default 's'
-        Specifies the units of the time differences the histogram should use. Use "s" for seconds, "m" for minutes,
+        Specify units of time differences the histogram should use. Use "s" for seconds, "m" for minutes,
         "h" for hours and "D" for days.
     log_scale : bool or tuple of bool, optional
 
         - If ``True`` - apply log scaling to the ``x`` axis.
         - If tuple of bool - apply log scaling to the (``x``,``y``) axes correspondingly.
     lower_cutoff_quantile : float, optional
-        Specifies the time distance quantile as the lower boundary. The values below the boundary are truncated.
+        Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
     upper_cutoff_quantile : float, optional
-        Specifies the time distance quantile as the upper boundary. The values above the boundary are truncated.
+        Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
     bins : int or str, default 20
         Generic bin parameter that can be the name of a reference rule or
-        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`
+        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
     figsize : tuple of float, default (12.0, 7.0)
         Width, height in inches.
 
+
+
+    See Also
+    --------
+    .EventTimestampHist : Plot the distribution of events over time.
+    .TimedeltaHist : Plot the distribution of the time deltas between two events.
+    .Eventstream.describe : Show general eventstream statistics.
+    .Eventstream.describe_events : Show general eventstream events statistics.
+    .DeleteUsersByPathLength : Filter user paths based on the path length, removing the paths that are shorter than the
+                               specified number of events or cut_off.
+
+    Notes
+    -----
+    See :ref:`Eventstream user guide<eventstream_user_lifetime>` for the details.
+
     """
 
     def __init__(
         self,
         eventstream: EventstreamType,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
@@ -87,17 +104,17 @@
             idx &= series >= series.quantile(self.lower_cutoff_quantile)
         return series[idx]
 
     def fit(self) -> None:
         """
         Calculate values for the histplot.
 
-            1. The first array contains the values for histogram
-            2. The first array contains the bin edges
-
+        Returns
+        -------
+        None
         """
         data = self.__eventstream.to_dataframe().groupby(self.user_col)[self.time_col].agg(["min", "max"])
         data["time_passed"] = data["max"] - data["min"]
         values_to_plot = (data["time_passed"] / np.timedelta64(1, self.timedelta_unit)).reset_index(  # type: ignore
             drop=True
         )
 
@@ -118,17 +135,16 @@
     @property
     def values(self) -> tuple[np.ndarray, np.ndarray]:
         """
 
         Returns
         -------
         tuple(np.ndarray, np.ndarray)
-
-            1. The first array contains the values for histogram
-            2. The first array contains the bin edges
+            1. The first array contains the values for histogram.
+            2. The first array contains the bin edges.
 
         """
         return self.values_to_plot, self.bins_to_show
 
     def plot(self) -> matplotlib.axes.Axes:
         """
         Create a sns.histplot based on the calculated values.
```

### Comparing `retentioneering-3.0.0b0/retentioneering/transition_graph/transition_graph.py` & `retentioneering-3.0.0b1/retentioneering/tooling/transition_graph/transition_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import copy
 import json
 import random
 import string
 from typing import Any, Dict, List, MutableMapping, MutableSequence, Union, cast
 
 import networkx as nx
 import pandas as pd
@@ -24,47 +25,48 @@
     PreparedNode,
     Threshold,
     Weight,
 )
 from retentioneering.utils.dict import clear_dict
 
 RenameRule = Dict[str, Union[List[str], str]]
+SESSION_ID_COL = "session_id"
 
 
 class TransitionGraph:
     """
     A class that holds methods for transition graph visualization.
 
     Parameters
     ----------
     eventstream: EventstreamType
-        Sourcing eventstream.
+        Source eventstream.
 
-    norm_type: {"full", "node", None}, default None
+    edges_norm_type: {"full", "node", None}, default None
         Type of normalization that is used to calculate weights for graph nodes and edges. See
         :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
     weights: dict, optional
         Weighting columns for nodes and edges. See :ref:`Transition graph user guide <transition_graph_weights>`
         for the details.
 
         - Possible keys: "nodes", "edges".
         - Possible values: "event_id", user column (typically "user_id") or custom columns.
 
-        If None, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
+        If ``None``, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
 
     thresholds: dict, optional
         Threshold values for hiding nodes and edges from the canvas.
 
         - Possible keys: "nodes", "edges".
         - Possible values: dict with weighting columns as dict keys and threshold values as dict values.
 
         Example: {'nodes': {'event_id': 0.03}, 'edges': {'event_id': 0.03, user_id: 0.05}}
 
-        If None, all the threshold values are set to 0.
+        If ``None``, all the threshold values are set to 0.
 
     targets: dict, optional
         Events mapping that defines which nodes and edges should be colored for better visualization.
 
         - Possible keys: "positive" (green), "negative" (red), "source" (orange).
         - Possible values: list of events of a given type.
 
@@ -75,35 +77,89 @@
         Possible keys:
         - show_weights,
         - show_percents,
         - show_nodes_names,
         - show_all_edges_for_targets,
         - show_nodes_without_links.
 
+    See Also
+    --------
+    .Eventstream.transition_graph : Call TransitionGraph tool as an eventstream method.
+
+    Notes
+    -----
+    See :doc:`transition graph user guide</user_guides/transition_graph>` for the details.
+
     """
 
     _weights: MutableMapping[str, str] | None = None
-    _norm_type: NormType = None
+    _edges_norm_type: NormType = None
+    _nodes_threshold: Threshold
+    _edges_threshold: Threshold
+
+    @property
+    def nodes_thresholds(self) -> Threshold:
+        return self._nodes_threshold
+
+    @nodes_thresholds.setter
+    def nodes_thresholds(self, value: Threshold) -> None:
+        if self._check_thresholds_for_norm_type(value):
+            self._nodes_threshold = value
+
+    @property
+    def edges_thresholds(self) -> Threshold:
+        return self._edges_threshold
+
+    @edges_thresholds.setter
+    def edges_thresholds(self, value: Threshold) -> None:
+        if self._check_thresholds_for_norm_type(value):
+            self._edges_threshold = value
+
+    def _check_thresholds_for_norm_type(self, value: Threshold) -> bool:
+        if self.edges_norm_type is None:
+            if not all(map(lambda x: x is None or x >= 0, value.values())):
+                raise ValueError(
+                    f"For normalization type {self.edges_norm_type} all thresholds must be positive or None"
+                )
+        else:
+            if not all(map(lambda x: x is None or 0 <= x <= 1, value.values())):
+                raise ValueError(
+                    f"For normalization type {self.edges_norm_type} all thresholds must be between 0 and 1 or None"
+                )
+
+        return True
 
     def __init__(
         self,
         eventstream: EventstreamType,  # graph: dict,  # preprocessed graph
-        graph_settings: GraphSettings,
-        norm_type: NormType = None,
-        weights: MutableMapping[str, str] | None = None,
+        graph_settings: GraphSettings | dict[str, Any] | None = None,
+        edges_norm_type: NormType = None,
         targets: MutableMapping[str, str | None] | None = None,
-        thresholds: dict[str, Threshold] | None = None,
+        nodes_threshold: Threshold | None = None,
+        edges_threshold: Threshold | None = None,
+        nodes_weight_col: str | None = None,
+        edges_weight_col: str | None = None,
+        custom_weight_cols: list[str] | None = None,
     ) -> None:
         from retentioneering.eventstream.eventstream import Eventstream
 
-        self.nodelist_default_col = "events"
-        self.edgelist_default_col = "events"
+        if graph_settings is None:
+            graph_settings = {}  # type: ignore
+        if nodes_threshold is None:
+            nodes_threshold = {"user_id": 0.0, "event_id": 0.0}
+        self.nodes_thresholds = nodes_threshold
+
+        if edges_threshold is None:
+            edges_threshold = {"user_id": 0.0, "event_id": 0.0}
+        self.edges_thresholds = edges_threshold
+
+        self.nodelist_default_col = eventstream.schema.event_id
+        self.edgelist_default_col = eventstream.schema.event_id
 
         self.targets = targets if targets else {"positive": None, "negative": None, "source": None}
-        self.thresholds = thresholds if thresholds else {"edges": {"events": 0.03}, "nodes": {"events": 0.03}}
         sm = ServerManager()
         self.env = sm.check_env()
         self.server = sm.create_server()
 
         self.server.register_action("save-nodelist", lambda n: self._on_nodelist_updated(n))
         self.server.register_action("save-layout", lambda n: self._on_layout_request(n))
         self.server.register_action("save-graph-settings", lambda n: self._on_graph_settings_request(n))
@@ -111,47 +167,57 @@
 
         self.eventstream: Eventstream = eventstream  # type: ignore
 
         self.event_col = self.eventstream.schema.event_name
         self.event_time_col = self.eventstream.schema.event_timestamp
         self.user_col = self.eventstream.schema.user_id
         self.id_col = self.eventstream.schema.event_id
-        self.custom_cols = [self.eventstream.schema.user_id] + self.eventstream.schema.custom_cols
+        self.weight_cols = self._define_weight_cols(custom_weight_cols)
 
-        self.weights = weights if weights else {"edges": "events", "nodes": "events"}
+        self.nodes_weight_col = nodes_weight_col if nodes_weight_col else eventstream.schema.event_id
+        self.edges_weight_col = edges_weight_col if edges_weight_col else eventstream.schema.event_id
 
         self.spring_layout_config = {"k": 0.1, "iterations": 300, "nx_threshold": 1e-4}
 
         self.layout: pd.DataFrame | None = None
         self.graph_settings = graph_settings
 
-        self.norm_type: NormType | None = norm_type
+        self.edges_norm_type: NormType | None = edges_norm_type
 
         self.nodelist: Nodelist = Nodelist(
-            nodelist_default_col=self.nodelist_default_col,
-            custom_cols=self.custom_cols,
+            weight_cols=self.weight_cols,
             time_col=self.event_time_col,
             event_col=self.event_col,
         )
 
         self.nodelist.calculate_nodelist(data=self.eventstream.to_dataframe())
-
-        self.edgelist: Edgelist = Edgelist(
-            event_col=self.event_col,
-            time_col=self.event_time_col,
-            default_weight_col=self.edgelist_default_col,
-            nodelist=self.nodelist.nodelist_df,
-            index_col=self.user_col,
-        )
+        self.edgelist: Edgelist = Edgelist(eventstream=self.eventstream)
         self.edgelist.calculate_edgelist(
-            norm_type=self.norm_type, custom_cols=self.custom_cols, data=self.eventstream.to_dataframe()
+            weight_cols=self.weight_cols,
+            norm_type=self.edges_norm_type,
         )
 
         self.render: TransitionGraphRenderer = TransitionGraphRenderer()
 
+    def _define_weight_cols(self, custom_weight_cols: list[str] | None) -> list[str]:
+        weight_cols = [
+            self.eventstream.schema.event_id,
+            self.eventstream.schema.user_id,
+        ]
+        if SESSION_ID_COL in self.eventstream.schema.custom_cols:
+            weight_cols.append(SESSION_ID_COL)
+        if isinstance(custom_weight_cols, list):
+            for col in custom_weight_cols:
+                if col not in weight_cols:
+                    if col not in self.eventstream.schema.custom_cols:
+                        raise ValueError(f"Custom weights column {col} not found in eventstream schema")
+                    else:
+                        weight_cols.append(col)
+        return weight_cols
+
     @property
     def weights(self) -> MutableMapping[str, str] | None:
         return self._weights
 
     @weights.setter
     def weights(self, value: MutableMapping[str, str] | None) -> None:
         available_cols = self.__get_nodelist_cols()
@@ -161,55 +227,59 @@
 
         if value and (value["edges"] not in available_cols or value["nodes"] not in available_cols):
             raise ValueError("Allowed only: %s" % {"edges": "col_name", "nodes": "col_name"})
 
         self._weights = value
 
     @property
-    def norm_type(self) -> NormType:  # type: ignore
-        return self._norm_type
+    def edges_norm_type(self) -> NormType:  # type: ignore
+        return self._edges_norm_type
 
-    @norm_type.setter
-    def norm_type(self, norm_type: NormType) -> None:  # type: ignore
-        allowed_norm_types: list[str | None] = [None, "full", "node"]
-        if norm_type in allowed_norm_types:
-            self._norm_type = norm_type
+    @edges_norm_type.setter
+    def edges_norm_type(self, edges_norm_type: NormType) -> None:  # type: ignore
+        allowed_edges_norm_types: list[str | None] = [None, "full", "node"]
+        if edges_norm_type in allowed_edges_norm_types:
+            self._edges_norm_type = edges_norm_type
         else:
-            raise ValueError("Norm type should be one of: %s" % allowed_norm_types)
+            raise ValueError("Norm type should be one of: %s" % allowed_edges_norm_types)
 
     def _on_recalc_request(
         self, rename_rules: list[RenameRule]
     ) -> dict[str, MutableSequence[PreparedNode] | MutableSequence[PreparedLink] | list]:
         try:
             self._recalculate(rename_rules=rename_rules)
 
             nodes, nodes_set = self._prepare_nodes(
                 nodelist=self.nodelist.nodelist_df,
             )
             self._on_nodelist_updated(nodes)
-
-            self.edgelist.edgelist_df["type"] = "suit"
-            links = self._prepare_edges(edgelist=self.edgelist.edgelist_df, nodes_set=nodes_set)
+            edgelist = self.edgelist.edgelist_df
+            edgelist["type"] = "suit"
+            links = self._prepare_edges(edgelist=edgelist, nodes_set=nodes_set)
             result: dict[str, MutableSequence[PreparedNode] | MutableSequence[PreparedLink] | list] = {
                 "nodes": nodes,
                 "links": links,
             }
 
             return result
         except Exception as err:
             raise ValueError("error! %s" % err)
 
     def _recalculate(self, rename_rules: list[RenameRule]) -> None:
         eventstream = self.eventstream.copy()
-        renamed_df = eventstream.rename(rules=rename_rules).to_dataframe()
+        # frontend can ask recalculate without grouping or renaming
+        if len(rename_rules) > 0:
+            eventstream = eventstream.rename(rules=rename_rules)  # type: ignore
+        renamed_df = eventstream.to_dataframe()
 
         # save norm type
         recalculated_nodelist = self.nodelist.calculate_nodelist(data=renamed_df)
+        self.edgelist.eventstream = eventstream
         recalculated_edgelist = self.edgelist.calculate_edgelist(
-            norm_type=self.norm_type, custom_cols=self.custom_cols, data=renamed_df
+            weight_cols=self.weight_cols, norm_type=self.edges_norm_type
         )
 
         curr_nodelist = self.nodelist.nodelist_df
 
         self.nodelist.nodelist_df = curr_nodelist.apply(
             lambda x: self._update_node_after_recalc(recalculated_nodelist, x), axis=1
         )
@@ -270,17 +340,17 @@
         self.nodelist.nodelist_df.set_index("index")
         self.nodelist.nodelist_df = self.nodelist.nodelist_df.drop(columns=["index"])
 
     def _make_node_params(
         self, targets: MutableMapping[str, str | None] | None = None
     ) -> MutableMapping[str, str | None] | dict[str, str | None]:
         if targets is not None:
-            return targets
+            return self._map_targets(targets)  # type: ignore
         else:
-            return self.targets  # type: ignore
+            return self._map_targets(self.targets)  # type: ignore
 
     def _get_norm_link_threshold(self, links_threshold: Threshold | None = None) -> dict[str, float] | None:
         nodelist_default_col = self.nodelist_default_col
         edgelist_default_col = self.edgelist_default_col
         scale = float(cast(float, self.edgelist.edgelist_df[edgelist_default_col].abs().max()))
         norm_links_threshold = None
 
@@ -339,17 +409,24 @@
             ]
             for i, j in pos.items()
         }
         return pos_new
 
     def __get_nodelist_cols(self) -> list[str]:
         default_col = self.nodelist_default_col
-        custom_cols = self.custom_cols
+        custom_cols = self.weight_cols
         return list([default_col]) + list(custom_cols)
 
+    def __round_value(self, value: float) -> float:
+        if self.edges_norm_type in ["full", "node"]:
+            # @TODO: make this magical number as constant or variable from config dict. Vladimir Makhanov
+            return round(value, 5)
+        else:
+            return value
+
     def _prepare_nodes(
         self, nodelist: pd.DataFrame, node_params: NodeParams | None = None, pos: Position | None = None
     ) -> tuple[list, MutableMapping]:
         node_names = set(nodelist[self.event_col])
 
         cols = self.__get_nodelist_cols()
 
@@ -359,16 +436,16 @@
             degree = {}
             for weight_col in cols:
                 max_degree = cast(float, nodelist[weight_col].max())
                 r = row[weight_col]
                 r = r.tolist()
                 value = r[0]
                 curr_degree = {}
-                curr_degree["degree"] = (abs(value)) / abs(max_degree) * 30 + 4
-                curr_degree["source"] = value
+                curr_degree["degree"] = self.__round_value((abs(value)) / abs(max_degree) * 30 + 4)
+                curr_degree["source"] = self.__round_value(value)
                 degree[weight_col] = curr_degree
 
             node_pos = pos.get(node_name) if pos is not None else None
             active = cast(bool, row["active"].tolist()[0])
             alias = cast(str, row["alias"].to_list()[0])
             parent = cast(str, row["parent"].to_list()[0])
 
@@ -398,34 +475,33 @@
     def _prepare_edges(
         self, edgelist: pd.DataFrame, nodes_set: MutableMapping[str, PreparedNode]
     ) -> MutableSequence[PreparedLink]:
         default_col = self.nodelist_default_col
         source_col = edgelist.columns[0]
         target_col = edgelist.columns[1]
         weight_col = edgelist.columns[2]
-        custom_cols: list[str] = self.custom_cols
+        custom_cols: list[str] = self.weight_cols
         edges: MutableSequence[PreparedLink] = []
 
         edgelist["weight_norm"] = edgelist[weight_col] / edgelist[weight_col].abs().max()
-
         for _, row in edgelist.iterrows():
             default_col_weight: Weight = {
-                "weight_norm": row.weight_norm,
-                "weight": cast(float, row[weight_col]),  # type: ignore
+                "weight_norm": self.__round_value(row.weight_norm),
+                "weight": self.__round_value(cast(float, row[weight_col])),  # type: ignore
             }
             weights = {
                 default_col: default_col_weight,
             }
             for custom_weight_col in custom_cols:
-                weight = cast(float, row[custom_weight_col])
+                weight = self.__round_value(cast(float, row[custom_weight_col]))
                 max_weight = cast(float, edgelist[custom_weight_col].abs().max())
-                weight_norm = weight / max_weight
+                weight_norm = self.__round_value(weight / max_weight)
                 col_weight: Weight = {
                     "weight_norm": weight_norm,
-                    "weight": cast(float, row[custom_weight_col]),
+                    "weight": weight,
                 }
                 weights[custom_weight_col] = col_weight
 
             source_node_name = str(row[source_col])  # type: ignore
             target_node_name = str(row[target_col])  # type: ignore
 
             source_node = nodes_set.get(source_node_name)
@@ -442,15 +518,15 @@
                         }
                     )
 
         return edges
 
     def _make_template_data(
         self, node_params: NodeParams, width: int, height: int
-    ) -> tuple[MutableSequence, MutableSequence]:
+    ) -> tuple[MutableSequence, MutableSequence[PreparedLink]]:
         edgelist = self.edgelist.edgelist_df.copy()
         nodelist = self.nodelist.nodelist_df.copy()
 
         source_col = edgelist.columns[0]
         target_col = edgelist.columns[1]
 
         # calc edge type
@@ -478,14 +554,25 @@
                 position[node_name] = [x, y]
 
         return position
 
     def _to_json(self, data: Any) -> str:
         return json.dumps(data).encode("latin1").decode("utf-8")
 
+    def _to_json_links(self, data: MutableSequence[PreparedLink]) -> str:
+        # We need to remove links with zero weight
+        cleaned_data = []
+        for link in data:
+            cleaned_link = copy.deepcopy(link)
+            cleaned_link["weights"] = {
+                weight_col: weight for weight_col, weight in link["weights"].items() if weight["weight"] > 0
+            }
+            cleaned_data.append(cleaned_link)
+        return self._to_json(cleaned_data)
+
     def _apply_settings(
         self,
         show_weights: bool | None = None,
         show_percents: bool | None = None,
         show_nodes_names: bool | None = None,
         show_all_edges_for_targets: bool | None = None,
         show_nodes_without_links: bool | None = None,
@@ -493,70 +580,88 @@
         settings = {
             "show_weights": show_weights,
             "show_percents": show_percents,
             "show_nodes_names": show_nodes_names,
             "show_all_edges_for_targets": show_all_edges_for_targets,
             "show_nodes_without_links": show_nodes_without_links,
         }
-        merged = {**self.graph_settings, **clear_dict(settings)}
+        # @FIXME: idk why pyright doesn't like this. Vladimir Makhanov
+        merged = {**self.graph_settings, **clear_dict(settings)}  # type: ignore
 
         return clear_dict(merged)
 
+    def _map_targets(self, targets: dict[str, str | list[str]]) -> dict[str, str]:
+        targets_mapping = {
+            "positive": "nice",
+            "negative": "bad",
+            "source": "source",
+        }
+        mapped_targets = {}
+
+        for target, nodes in targets.items():
+            if nodes is None:
+                pass
+            if isinstance(nodes, list):
+                for node in nodes:
+                    mapped_targets[node] = targets_mapping[target]
+            else:
+                mapped_targets[nodes] = targets_mapping[target]
+
+        return mapped_targets
+
     def _to_js_val(self, val: Any = None) -> str:
         return self._to_json(val) if val is not None else "undefined"
 
     @staticmethod
     def generateId(size: int = 6, chars: str = string.ascii_uppercase + string.digits) -> str:
         return "el" + "".join(random.choice(chars) for _ in range(size))
 
-    def _norm_type_to_json_value(self, norm_type: NormType) -> str:
-        return "none" if norm_type is None else str(norm_type).lower()
+    def _edges_norm_type_to_json_value(self, edges_norm_type: NormType) -> str:
+        return "none" if edges_norm_type is None else str(edges_norm_type).lower()
 
     def plot_graph(
         self,
-        thresholds: dict[str, Threshold] | None = None,
         targets: MutableMapping[str, str | None] | None = None,
-        weights: MutableMapping[str, str] | None = None,
-        norm_type: NormType | None = None,
+        edges_norm_type: NormType | None = None,
         width: int = 960,
         height: int = 900,
         weight_template: str | None = None,
         show_weights: bool | None = None,
         show_percents: bool | None = None,
         show_nodes_names: bool | None = None,
         show_all_edges_for_targets: bool | None = None,
         show_nodes_without_links: bool | None = None,
     ) -> None:
         """
         Create interactive transition graph visualization with callback to sourcing eventstream.
 
         Parameters
         ----------
-        norm_type: {"full", "node", None}, default None
+        edges_norm_type: {"full", "node", None}, default None
             Type of normalization that is used to calculate weights for graph nodes and edges. See
             :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
         weights: dict, optional
             Weighting columns for nodes and edges. See :ref:`Transition graph user guide <transition_graph_weights>`
             for the details.
 
             - Possible keys: "nodes", "edges".
             - Possible values: "event_id", user column (typically "user_id") or custom columns.
 
-            If None, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
+            If ``None``, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
 
         thresholds: dict, optional
             Threshold values for hiding nodes and edges from the canvas.
 
             - Possible keys: "nodes", "edges".
             - Possible values: dict with weighting columns as dict keys and threshold values as dict values.
 
             Example: {'nodes': {'event_id': 0.03}, 'edges': {'event_id': 0.03, user_id: 0.05}}
 
-            If None, all the threshold values are set to 0.
+            If ``None``, all the threshold values are set to 0.
 
         targets: dict, optional
             Events mapping that defines which nodes and edges should be colored for better visualization.
 
             - Possible keys: "positive" (green), "negative" (red), "source" (orange).
             - Possible values: list of events of a given type.
 
@@ -569,64 +674,62 @@
         show_percents : bool, optional
         show_nodes_names : bool, optional
         show_all_edges_for_targets : bool, optional
         show_nodes_without_links : bool, optional
 
         Returns
         -------
-            Rendered IFrame graph
+            Rendered IFrame graph.
 
         Notes
         -----
         To get the definition of ``show_*`` visual parameters see
         :ref:`Settings block <transition_graph_visual_settings>` in the control of transition graph interface.
 
         """
         if targets:
             self.targets = targets
-        if weights:
-            self.weights = weights
-        self.norm_type = norm_type
+        self.edges_norm_type = edges_norm_type
 
         settings = self._apply_settings(
             show_weights=show_weights,
             show_percents=show_percents,
             show_nodes_names=show_nodes_names,
             show_all_edges_for_targets=show_all_edges_for_targets,
             show_nodes_without_links=show_nodes_without_links,
         )
 
-        nodes_threshold = thresholds.get("nodes", self.thresholds.get("nodes", None)) if thresholds else None
-        links_threshold = thresholds.get("edges", self.thresholds.get("edges", None)) if thresholds else None
-        norm_nodes_threshold = nodes_threshold if nodes_threshold else self._get_norm_node_threshold(nodes_threshold)
-        norm_links_threshold = links_threshold if links_threshold else self._get_norm_link_threshold(links_threshold)
-
-        self.edgelist.calculate_edgelist(
-            norm_type=self.norm_type, custom_cols=self.custom_cols, data=self.eventstream.to_dataframe()
+        norm_nodes_threshold = (
+            self.nodes_thresholds if self.nodes_thresholds else self._get_norm_node_threshold(self.nodes_thresholds)
+        )
+        norm_links_threshold = (
+            self.edges_thresholds if self.edges_thresholds else self._get_norm_link_threshold(self.edges_thresholds)
         )
+
+        self.edgelist.calculate_edgelist(weight_cols=self.weight_cols, norm_type=self.edges_norm_type)
         node_params = self._make_node_params(targets)
         cols = self.__get_nodelist_cols()
 
         nodes, links = self._make_template_data(
             node_params=node_params,
             width=width,
             height=height,
         )
 
-        shown_nodes_col = self.weights["nodes"] if self.weights else "events"
-        shown_links_weight = self.weights["edges"] if self.weights else "events"
+        shown_nodes_col = self.nodes_weight_col
+        shown_links_weight = self.edges_weight_col
         selected_nodes_col_for_thresholds = shown_nodes_col
         selected_links_weight_for_thresholds = shown_links_weight
 
         init_graph_js = self.render.init(
             **dict(
                 server_id=self.server.pk,
                 env=self.env,
-                norm_type=self._norm_type_to_json_value(self.norm_type),
-                links=self._to_json(links),
+                norm_type=self._edges_norm_type_to_json_value(self.edges_norm_type),
+                links=self._to_json_links(links),
                 nodes=self._to_json(nodes),
                 node_params=self._to_json(node_params),
                 layout_dump=1 if self.layout is not None else 0,
                 links_weights_names=cols,
                 node_cols_names=cols,
                 shown_nodes_col=shown_nodes_col,
                 shown_links_weight=shown_links_weight,
@@ -650,15 +753,15 @@
             + self.generateId()
         )
 
         init_graph_template = self.render.init(
             **dict(
                 server_id=self.server.pk,
                 env=self.env,
-                norm_type=self._norm_type_to_json_value(self.norm_type),
+                norm_type=self._edges_norm_type_to_json_value(self.edges_norm_type),
                 node_params=self._to_json(node_params),
                 links="<%= links %>",
                 nodes="<%= nodes %>",
                 layout_dump=1,
                 links_weights_names=cols,
                 node_cols_names=cols,
                 shown_nodes_col="<%= shown_nodes_col %>",
```

### Comparing `retentioneering-3.0.0b0/retentioneering/utils/registry.py` & `retentioneering-3.0.0b1/retentioneering/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/retentioneering/widget/widgets.py` & `retentioneering-3.0.0b1/retentioneering/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b0/PKG-INFO` & `retentioneering-3.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retentioneering
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: Product analytics and marketing optimization framework based on deep user trajectories analysis
 Home-page: https://github.com/retentioneering/retentioneering-tools
 License: Retentioneering Software Non-Exclusive License (License)
 Author: Retentioneering User Trajectory Analysis Lab
 Author-email: retentioneering@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

