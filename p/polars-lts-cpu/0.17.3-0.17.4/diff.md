# Comparing `tmp/polars_lts_cpu-0.17.3.tar.gz` & `tmp/polars_lts_cpu-0.17.4.tar.gz`

## Comparing `polars_lts_cpu-0.17.3.tar` & `polars_lts_cpu-0.17.4.tar`

### file list

```diff
@@ -1,1096 +1,1098 @@
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10476 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7368 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     4143 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    21192 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    20108 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     4115 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9692 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2960 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31306 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      535 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123      320 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12466 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7059 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2008 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    23538 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20089 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24202 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123     4012 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123     9096 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/assets/SQL.sublime-syntax
--rw-r--r--   0     1001      123    21158 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/assets/theme
--rw-r--r--   0     1001      123     1450 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/cli/highlighter.rs
--rw-r--r--   0     1001      123     5052 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/cli/mod.rs
--rw-r--r--   0     1001      123     1043 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/cli/prompt.rs
--rw-r--r--   0     1001      123    14453 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    16610 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123    27444 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123      342 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/main.rs
--rw-r--r--   0     1001      123    13269 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     3386 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     6275 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13665 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     2681 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2534 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     5961 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123    10613 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2164 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20856 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23518 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     8395 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      376 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    20488 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     3277 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7771 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     4292 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/take_agg.rs
--rw-r--r--   0     1001      123     4417 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2716 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5020 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1114 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3604 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28675 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19709 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21349 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31233 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    25218 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    12866 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7580 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9218 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123     9974 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4879 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7215 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12177 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7354 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4790 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9629 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      633 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    22005 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11872 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3680 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3423 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1106 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3276 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20212 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       32 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30142 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10815 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10139 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6444 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123      552 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6768 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9288 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47120 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13439 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4184 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1211 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21864 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17409 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    18847 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5804 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     3670 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    21103 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14345 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31819 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2044 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      419 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27335 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18867 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9470 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20901 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4293 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14819 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47907 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2953 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1033 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7265 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8679 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    19782 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    13129 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5150 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7001 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19456 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    14266 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23609 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2517 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9391 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6295 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    24977 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    15089 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123    22261 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7753 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2501 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    11998 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     1592 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25934 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2701 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42068 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    11748 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5532 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7675 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36116 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6561 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     7643 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    47356 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123      218 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    12291 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14048 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39434 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10535 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    17027 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16303 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     2953 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11583 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124249 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27393 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5950 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8795 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2149 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15766 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123     8247 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    17701 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    24386 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9217 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10850 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12938 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    17994 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15242 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5718 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    15106 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14223 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6207 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18305 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5246 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7817 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11029 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9735 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4257 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    37171 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18263 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123    32703 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1181 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17253 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9424 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13169 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1327 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123     1593 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123    13227 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      810 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     1364 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123     8119 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    19145 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    13066 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    19590 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2195 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123    42498 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10196 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    64804 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2094 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    14993 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6825 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11393 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25701 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    25056 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29662 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15196 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    12019 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9752 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8148 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15287 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3260 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14494 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6715 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28281 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     2692 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27332 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13850 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19819 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10197 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15273 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4615 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13048 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11955 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/LICENSE
--rw-r--r--   0     1001      123     2414 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/Makefile
--rw-r--r--   0     1001      123    10844 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/README.md
--rw-r--r--   0     1001      123      651 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/build.rs
--rw-r--r--   0     1001      123       32 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      450 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1567 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7302 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1339 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1114 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123      968 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      339 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      722 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1118 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123      647 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6283 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/__init__.py
--rw-r--r--   0     1001      123    13396 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/api.py
--rw-r--r--   0     1001      123    24553 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/config.py
--rw-r--r--   0     1001      123    25409 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5057 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   303363 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2588 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    11189 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1541 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    12688 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/dependencies.py
--rw-r--r--   0     1001      123     2954 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/categorical.py
--rw-r--r--   0     1001      123    69359 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/datetime.py
--rw-r--r--   0     1001      123   251184 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/meta.py
--rw-r--r--   0     1001      123    44707 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/expr/struct.py
--rw-r--r--   0     1001      123     1981 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29688 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/functions/eager.py
--rw-r--r--   0     1001      123    90019 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35533 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8655 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     5309 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1271 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1299 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3611 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   166918 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24010 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/categorical.py
--rw-r--r--   0     1001      123    47287 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/list.py
--rw-r--r--   0     1001      123   162618 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/series.py
--rw-r--r--   0     1001      123    27401 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/__init__.py
--rw-r--r--   0     1001      123      929 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/_private.py
--rw-r--r--   0     1001      123     3689 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/_tempdir.py
--rw-r--r--   0     1001      123    13597 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/asserts.py
--rw-r--r--   0     1001      123     1380 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    23137 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     2811 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     5681 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/type_aliases.py
--rw-r--r--   0     1001      123     1167 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/__init__.py
--rw-r--r--   0     1001      123    50687 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/build_info.py
--rw-r--r--   0     1001      123     9483 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/convert.py
--rw-r--r--   0     1001      123     5789 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2339 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    11592 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/polars/utils/various.py
--rw-r--r--   0     1001      123     5325 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/pyproject.toml
--rw-r--r--   0     1001      123      699 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10959 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/apply/mod.rs
--rw-r--r--   0     1001      123    71436 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3906 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5214 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/batched_csv.rs
--rw-r--r--   0     1001      123    47168 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/conversion.rs
--rw-r--r--   0     1001      123    45433 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lazy/apply.rs
--rw-r--r--   0     1001      123    33479 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62595 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lazy/utils.rs
--rw-r--r--   0     1001      123    21002 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/lib.rs
--rw-r--r--   0     1001      123     7902 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/npy.rs
--rw-r--r--   0     1001      123     1029 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/py_modules.rs
--rw-r--r--   0     1001      123    54504 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/set.rs
--rw-r--r--   0     1001      123      843 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     5018 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123     3707 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     5709 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     7395 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    11514 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2766 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      280 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123    14355 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    28043 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    91453 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      218 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1937 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39029 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6360 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11067 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5919 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3391 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6849 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2881 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11849 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13315 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3259 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    13578 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12750 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23698 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    15767 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     5851 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     4390 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     7840 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3908 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123    16263 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19140 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3643 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3631 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9814 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19908 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    38697 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3497 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   120351 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1009 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    15839 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    32643 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    11301 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    32596 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    49534 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4014 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    10976 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2441 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83973 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10700 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-15 18:45:31.000000 polars_lts_cpu-0.17.3/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    64028 2023-04-15 18:46:31.000000 polars_lts_cpu-0.17.3/Cargo.lock
--rw-r--r--   0        0        0    13382 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.3/PKG-INFO
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8679 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    19782 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    13129 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5069 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7230 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19456 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    14266 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23524 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2517 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9391 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6214 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    24977 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    15089 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123    22261 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7753 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2501 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    11998 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     1592 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25934 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2701 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42410 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    12083 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5532 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7675 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36116 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33715 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6561 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4115 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7643 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    37733 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5636 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    12291 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14048 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39434 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10535 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    17027 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16352 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     2953 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11879 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124247 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27392 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5950 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8795 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2183 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15766 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123     8247 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18441 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    24323 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9217 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10850 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12938 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    17994 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15242 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5718 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    15106 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14223 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6207 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18305 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5246 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7817 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11029 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9735 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4257 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    37180 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18263 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123    32703 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1181 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17253 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9424 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13169 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1327 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123     1593 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    13227 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      810 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     1364 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123     8119 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    19145 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    13421 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    19590 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     2700 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123    42541 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10196 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    64804 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2094 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    14993 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6825 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11393 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25701 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    25056 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29662 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15196 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    12019 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9752 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8148 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15287 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3260 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14494 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6715 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28281 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26507 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2692 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27332 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13850 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19819 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10197 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15273 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4615 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13048 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11955 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6768 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9288 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47111 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13439 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4184 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1211 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21864 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17432 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    18857 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    21103 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31819 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2044 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      419 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27335 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18867 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9470 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20901 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4293 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14819 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47907 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2953 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1033 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     3030 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     6275 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    13665 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     2681 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2534 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     5961 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123    10613 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2164 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20856 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23518 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     8395 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      635 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      376 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    20488 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3275 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20212 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       32 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30142 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10815 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10139 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6444 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123      552 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7265 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1114 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3604 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28675 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19709 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21349 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31233 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25218 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    12866 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7580 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9218 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123     9974 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4879 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12177 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7354 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4790 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9629 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      633 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123     4012 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123     9096 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/assets/SQL.sublime-syntax
+-rw-r--r--   0     1001      123    21158 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/assets/theme
+-rw-r--r--   0     1001      123     1433 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/cli/highlighter.rs
+-rw-r--r--   0     1001      123     5023 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/cli/mod.rs
+-rw-r--r--   0     1001      123     1043 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/cli/prompt.rs
+-rw-r--r--   0     1001      123    14453 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    16610 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123    27444 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123      342 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/main.rs
+-rw-r--r--   0     1001      123    13269 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     3386 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10476 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7368 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     4143 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21192 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20108 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     4115 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9692 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31306 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      535 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123      320 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12466 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7059 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2008 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    23538 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20089 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24202 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    22005 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11872 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3680 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3423 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1106 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6171 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7771 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     6609 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/take_agg.rs
+-rw-r--r--   0     1001      123     4417 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2716 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5020 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/Makefile
+-rw-r--r--   0     1001      123    11845 2023-04-17 11:09:21.000000 polars_lts_cpu-0.17.4/README.md
+-rw-r--r--   0     1001      123      651 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      450 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1567 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7302 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1339 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1513 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1114 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123      968 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123      988 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      339 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      722 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1118 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123      647 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6283 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/api.py
+-rw-r--r--   0     1001      123    24553 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/config.py
+-rw-r--r--   0     1001      123    25409 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5057 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   303518 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2588 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    11189 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1541 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    12688 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/dependencies.py
+-rw-r--r--   0     1001      123     2954 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    69359 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   251184 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44707 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1981 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29688 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/functions/eager.py
+-rw-r--r--   0     1001      123    90019 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     5309 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   166918 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24010 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/categorical.py
+-rw-r--r--   0     1001      123    47287 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/list.py
+-rw-r--r--   0     1001      123   162618 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/series.py
+-rw-r--r--   0     1001      123    27401 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/__init__.py
+-rw-r--r--   0     1001      123      929 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/_private.py
+-rw-r--r--   0     1001      123     3689 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/_tempdir.py
+-rw-r--r--   0     1001      123    13597 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/asserts.py
+-rw-r--r--   0     1001      123     1380 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    23137 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     2860 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     5681 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1167 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    50687 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     9483 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2339 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/polars/utils/various.py
+-rw-r--r--   0     1001      123     5325 2023-04-17 11:09:21.000000 polars_lts_cpu-0.17.4/pyproject.toml
+-rw-r--r--   0     1001      123      699 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10959 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71436 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3906 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5214 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/batched_csv.rs
+-rw-r--r--   0     1001      123    47168 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/conversion.rs
+-rw-r--r--   0     1001      123    45433 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    33479 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62595 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    21002 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/lib.rs
+-rw-r--r--   0     1001      123     7902 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/npy.rs
+-rw-r--r--   0     1001      123     1029 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/py_modules.rs
+-rw-r--r--   0     1001      123    54504 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     5721 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123     3707 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     5709 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     7395 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    11730 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2766 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      280 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123    14355 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    29370 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    91453 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      218 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1937 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39029 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6360 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11067 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5919 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3391 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     6849 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2881 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11849 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13315 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3259 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    15436 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12750 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    15767 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     5851 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     4390 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     7840 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3908 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22696 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123    16937 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10467 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18639 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19550 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     3643 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9814 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19908 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    39286 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3497 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   120947 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1009 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    15839 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    11301 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    32596 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49534 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4014 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     6995 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    10976 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2441 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83973 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_series.py
+-rw-r--r--   0     1001      123     2561 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10700 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-17 11:09:20.000000 polars_lts_cpu-0.17.4/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    64027 2023-04-17 11:10:27.000000 polars_lts_cpu-0.17.4/Cargo.lock
+-rw-r--r--   0        0        0    14383 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.4/PKG-INFO
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 default = ["private"]
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/README.md` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/assets/SQL.sublime-syntax` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/assets/SQL.sublime-syntax`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/assets/theme` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/assets/theme`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/cli/highlighter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/cli/highlighter.rs`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 use syntect::easy::HighlightLines;
 use syntect::highlighting::{Style, Theme, ThemeSet};
 use syntect::parsing::{SyntaxDefinition, SyntaxSet, SyntaxSetBuilder};
 use syntect::util::as_24_bit_terminal_escaped;
 
 pub(crate) struct SQLHighlighter {}
 
-const SQL_SYNTAX: &'static str = include_str!("../../assets/SQL.sublime-syntax");
-const THEME: &'static [u8] = include_bytes!("../../assets/theme");
+const SQL_SYNTAX: &str = include_str!("../../assets/SQL.sublime-syntax");
+const THEME: &[u8] = include_bytes!("../../assets/theme");
 
 impl Highlighter for SQLHighlighter {
     fn highlight(&self, line: &str, cursor: usize) -> reedline::StyledText {
         let syn_def = SyntaxDefinition::load_from_str(SQL_SYNTAX, true, Some("sql")).unwrap();
         let mut ssb = SyntaxSetBuilder::new();
         ssb.add(syn_def);
         let mut ps = ssb.build();
         let mut cursor = Cursor::new(THEME);
         let ts = ThemeSet::load_from_reader(&mut cursor).unwrap();
         let syntax = ps.find_syntax_by_extension("sql").unwrap();
 
         let mut styled_text = StyledText::new();
         let mut h = HighlightLines::new(syntax, &ts);
-        let ranges: Vec<(Style, &str)> = h.highlight_line(&line, &ps).unwrap();
+        let ranges: Vec<(Style, &str)> = h.highlight_line(line, &ps).unwrap();
         for (style, text) in ranges {
             let fg = Color::Rgb(style.foreground.r, style.foreground.g, style.foreground.b);
             let s = AnsiStyle::new().fg(fg);
             styled_text.push((s, text.to_string()));
         }
         styled_text
     }
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/cli/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/cli/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,21 @@
 }
 
 fn get_extension_from_filename(filename: &str) -> Option<&str> {
     Path::new(filename).extension().and_then(OsStr::to_str)
 }
 
 fn get_home_dir() -> PathBuf {
-    let home_dir = match env::var("HOME") {
+    match env::var("HOME") {
         Ok(path) => PathBuf::from(path),
         Err(_) => match env::var("USERPROFILE") {
             Ok(path) => PathBuf::from(path),
             Err(_) => panic!("Failed to get home directory"),
         },
-    };
-    home_dir
+    }
 }
 
 fn get_history_path() -> PathBuf {
     let mut home_dir = get_home_dir();
     home_dir.push(".polars");
     home_dir.push("history.txt");
     home_dir
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/cli/prompt.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/cli/prompt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-error/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 regex = { version = "1.6", optional = true }
 thiserror= "^1"
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 timezones = ["chrono-tz", "chrono"]
 simd = []
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,85 @@
-use arrow::array::{Array, ListArray, NullArray};
-use arrow::bitmap::MutableBitmap;
-use arrow::compute::concatenate;
-use arrow::datatypes::DataType;
-use arrow::error::Result;
-use arrow::offset::Offsets;
-
-use crate::prelude::*;
-
-pub struct AnonymousBuilder<'a> {
-    arrays: Vec<&'a dyn Array>,
-    offsets: Vec<i64>,
-    validity: Option<MutableBitmap>,
-    size: i64,
-}
-
-impl<'a> AnonymousBuilder<'a> {
-    pub fn new(size: usize) -> Self {
-        let mut offsets = Vec::with_capacity(size + 1);
-        offsets.push(0i64);
-        Self {
-            arrays: Vec::with_capacity(size),
-            offsets,
-            validity: None,
-            size: 0,
-        }
-    }
-    #[inline]
-    fn last_offset(&self) -> i64 {
-        *self.offsets.last().unwrap()
-    }
+use polars_core::frame::groupby::GroupsIndicator;
 
-    pub fn is_empty(&self) -> bool {
-        self.arrays.is_empty()
-    }
+use super::*;
 
-    pub fn offsets(&self) -> &[i64] {
-        &self.offsets
-    }
+#[cfg(feature = "dtype-u8")]
+type DummyType = u8;
+#[cfg(feature = "dtype-u8")]
+type DummyCa = UInt8Chunked;
+
+#[cfg(not(feature = "dtype-u8"))]
+type DummyType = i32;
+#[cfg(not(feature = "dtype-u8"))]
+type DummyCa = Int32Chunked;
 
-    pub fn take_offsets(self) -> Offsets<i64> {
-        // safety: offsets are correct
-        unsafe { Offsets::new_unchecked(self.offsets) }
-    }
+pub trait ToDummies {
+    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame>;
+}
 
-    #[inline]
-    pub fn push(&mut self, arr: &'a dyn Array) {
-        self.size += arr.len() as i64;
-        self.offsets.push(self.size);
-        self.arrays.push(arr);
-
-        if let Some(validity) = &mut self.validity {
-            validity.push(true)
-        }
-    }
+impl ToDummies for Series {
+    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame> {
+        let sep = separator.unwrap_or("_");
+        let col_name = self.name();
+        let groups = self.group_tuples(true, false)?;
+
+        // safety: groups are in bounds
+        let columns = unsafe { self.agg_first(&groups) }
+            .iter()
+            .zip(groups.iter())
+            .map(|(av, group)| {
+                // strings are formatted with extra \" \" in polars, so we
+                // extract the string
+                let name = if let Some(s) = av.get_str() {
+                    format!("{col_name}{sep}{s}")
+                } else {
+                    // other types don't have this formatting issue
+                    format!("{col_name}{sep}{av}")
+                };
+
+                let ca = match group {
+                    GroupsIndicator::Idx((_, group)) => {
+                        dummies_helper_idx(group, self.len(), &name)
+                    }
+                    GroupsIndicator::Slice([offset, len]) => {
+                        dummies_helper_slice(offset, len, self.len(), &name)
+                    }
+                };
+                ca.into_series()
+            })
+            .collect();
 
-    pub fn push_multiple(&mut self, arrs: &'a [ArrayRef]) {
-        for arr in arrs {
-            self.size += arr.len() as i64;
-            self.arrays.push(arr.as_ref());
-        }
-        self.offsets.push(self.size);
-        self.update_validity()
+        Ok(DataFrame::new_no_checks(sort_columns(columns)))
     }
+}
 
-    pub fn push_null(&mut self) {
-        self.offsets.push(self.last_offset());
-        match &mut self.validity {
-            Some(validity) => validity.push(false),
-            None => self.init_validity(),
-        }
-    }
+fn dummies_helper_idx(groups: &[IdxSize], len: usize, name: &str) -> DummyCa {
+    let mut av = vec![0 as DummyType; len];
 
-    pub fn push_empty(&mut self) {
-        self.offsets.push(self.last_offset());
-        self.update_validity()
+    for &idx in groups {
+        let elem = unsafe { av.get_unchecked_mut(idx as usize) };
+        *elem = 1;
     }
 
-    fn init_validity(&mut self) {
-        let len = self.offsets.len() - 1;
+    ChunkedArray::from_vec(name, av)
+}
 
-        let mut validity = MutableBitmap::with_capacity(self.offsets.capacity());
-        validity.extend_constant(len, true);
-        validity.set(len - 1, false);
-        self.validity = Some(validity)
-    }
-    fn update_validity(&mut self) {
-        if let Some(validity) = &mut self.validity {
-            validity.push(true)
-        }
+fn dummies_helper_slice(
+    group_offset: IdxSize,
+    group_len: IdxSize,
+    len: usize,
+    name: &str,
+) -> DummyCa {
+    let mut av = vec![0 as DummyType; len];
+
+    for idx in group_offset..(group_offset + group_len) {
+        let elem = unsafe { av.get_unchecked_mut(idx as usize) };
+        *elem = 1;
     }
 
-    pub fn finish(self, inner_dtype: Option<&DataType>) -> Result<ListArray<i64>> {
-        // Safety:
-        // offsets are monotonically increasing
-        let offsets = unsafe { Offsets::new_unchecked(self.offsets) };
-        let (inner_dtype, values) = if self.arrays.is_empty() {
-            let len = *offsets.last() as usize;
-            let values = NullArray::new(DataType::Null, len).boxed();
-            (DataType::Null, values)
-        } else {
-            let inner_dtype = inner_dtype.unwrap_or_else(|| self.arrays[0].data_type());
-            let values = concatenate::concatenate(&self.arrays)?;
-            (inner_dtype.clone(), values)
-        };
-        let dtype = ListArray::<i64>::default_datatype(inner_dtype);
-        Ok(ListArray::<i64>::new(
-            dtype,
-            offsets.into(),
-            values,
-            self.validity.map(|validity| validity.into()),
-        ))
-    }
+    ChunkedArray::from_vec(name, av)
+}
+
+fn sort_columns(mut columns: Vec<Series>) -> Vec<Series> {
+    columns.sort_by(|a, b| a.name().partial_cmp(b.name()).unwrap());
+    columns
 }
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/null.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/take_agg.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/take_agg.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 //! kernels that combine take and aggregations.
-use arrow::array::{PrimitiveArray, Utf8Array};
+use arrow::array::{Array, BooleanArray, PrimitiveArray, Utf8Array};
 use arrow::types::NativeType;
 use num_traits::{NumCast, ToPrimitive};
 
 use crate::array::PolarsArray;
 use crate::index::IdxSize;
 
 /// Take kernel for single chunk without nulls and an iterator as index.
@@ -159,7 +159,103 @@
     f: F,
 ) -> Option<&str> {
     indices
         .into_iter()
         .map(|idx| arr.value_unchecked(idx))
         .reduce(|acc, str_val| f(acc, str_val))
 }
+
+/// Take kernel for single chunk and an iterator as index.
+/// # Safety
+/// caller must ensure iterators indexes are in bounds
+#[inline]
+pub unsafe fn take_min_bool_iter_unchecked_nulls<I: IntoIterator<Item = usize>>(
+    arr: &BooleanArray,
+    indices: I,
+    len: IdxSize,
+) -> Option<bool> {
+    let mut null_count = 0 as IdxSize;
+    let validity = arr.validity().unwrap();
+
+    for idx in indices {
+        if validity.get_bit_unchecked(idx) {
+            if !arr.value_unchecked(idx) {
+                return Some(false);
+            }
+        } else {
+            null_count += 1;
+        }
+    }
+    if null_count == len {
+        None
+    } else {
+        Some(true)
+    }
+}
+
+/// Take kernel for single chunk and an iterator as index.
+/// # Safety
+/// caller must ensure iterators indexes are in bounds
+#[inline]
+pub unsafe fn take_min_bool_iter_unchecked_no_nulls<I: IntoIterator<Item = usize>>(
+    arr: &BooleanArray,
+    indices: I,
+) -> Option<bool> {
+    if arr.is_empty() {
+        return None;
+    }
+
+    for idx in indices {
+        if !arr.value_unchecked(idx) {
+            return Some(false);
+        }
+    }
+    Some(true)
+}
+
+/// Take kernel for single chunk and an iterator as index.
+/// # Safety
+/// caller must ensure iterators indexes are in bounds
+#[inline]
+pub unsafe fn take_max_bool_iter_unchecked_nulls<I: IntoIterator<Item = usize>>(
+    arr: &BooleanArray,
+    indices: I,
+    len: IdxSize,
+) -> Option<bool> {
+    let mut null_count = 0 as IdxSize;
+    let validity = arr.validity().unwrap();
+
+    for idx in indices {
+        if validity.get_bit_unchecked(idx) {
+            if arr.value_unchecked(idx) {
+                return Some(true);
+            }
+        } else {
+            null_count += 1;
+        }
+    }
+    if null_count == len {
+        None
+    } else {
+        Some(false)
+    }
+}
+
+/// Take kernel for single chunk and an iterator as index.
+/// # Safety
+/// caller must ensure iterators indexes are in bounds
+#[inline]
+pub unsafe fn take_max_bool_iter_unchecked_no_nulls<I: IntoIterator<Item = usize>>(
+    arr: &BooleanArray,
+    indices: I,
+) -> Option<bool> {
+    if arr.is_empty() {
+        return None;
+    }
+
+    for idx in indices {
+        if arr.value_unchecked(idx) {
+            return Some(true);
+        }
+    }
+    Some(false)
+}
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/hash.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/macros.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 polars-error = { version = "0.28.0", path = "../polars-error" }
 polars-utils = { version = "0.28.0", path = "../polars-utils" }
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 tokio = { version = "1.26.0", features = ["net"], optional = true }
 url = { version = "2.3.1", optional = true }
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/json.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 semi_anti_join = ["polars-core/semi_anti_join"]
 list_take = []
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,64 @@
-use polars_core::frame::groupby::GroupsIndicator;
+use smartstring::alias::String as SmartString;
 
 use super::*;
+use crate::prelude::optimizer::predicate_pushdown::keys::{key_has_name, predicate_to_key};
 
-#[cfg(feature = "dtype-u8")]
-type DummyType = u8;
-#[cfg(feature = "dtype-u8")]
-type DummyCa = UInt8Chunked;
-
-#[cfg(not(feature = "dtype-u8"))]
-type DummyType = i32;
-#[cfg(not(feature = "dtype-u8"))]
-type DummyCa = Int32Chunked;
-
-pub trait ToDummies {
-    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame>;
-}
-
-impl ToDummies for Series {
-    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame> {
-        let sep = separator.unwrap_or("_");
-        let col_name = self.name();
-        let groups = self.group_tuples(true, false)?;
-
-        // safety: groups are in bounds
-        let columns = unsafe { self.agg_first(&groups) }
-            .iter()
-            .zip(groups.iter())
-            .map(|(av, group)| {
-                // strings are formatted with extra \" \" in polars, so we
-                // extract the string
-                let name = if let Some(s) = av.get_str() {
-                    format!("{col_name}{sep}{s}")
-                } else {
-                    // other types don't have this formatting issue
-                    format!("{col_name}{sep}{av}")
-                };
-
-                let ca = match group {
-                    GroupsIndicator::Idx((_, group)) => {
-                        dummies_helper_idx(group, self.len(), &name)
-                    }
-                    GroupsIndicator::Slice([offset, len]) => {
-                        dummies_helper_slice(offset, len, self.len(), &name)
-                    }
-                };
-                ca.into_series()
-            })
-            .collect();
-
-        Ok(DataFrame::new_no_checks(sort_columns(columns)))
+fn remove_any_key_referencing_renamed(
+    new: &str,
+    acc_predicates: &mut PlHashMap<Arc<str>, Node>,
+    local_predicates: &mut Vec<Node>,
+) {
+    let mut move_to_local = vec![];
+    for key in acc_predicates.keys() {
+        if key_has_name(key, new) {
+            move_to_local.push(key.clone())
+        }
     }
-}
-
-fn dummies_helper_idx(groups: &[IdxSize], len: usize, name: &str) -> DummyCa {
-    let mut av = vec![0 as DummyType; len];
 
-    for &idx in groups {
-        let elem = unsafe { av.get_unchecked_mut(idx as usize) };
-        *elem = 1;
+    for key in move_to_local {
+        local_predicates.push(acc_predicates.remove(&key).unwrap())
     }
-
-    ChunkedArray::from_vec(name, av)
 }
 
-fn dummies_helper_slice(
-    group_offset: IdxSize,
-    group_len: IdxSize,
-    len: usize,
-    name: &str,
-) -> DummyCa {
-    let mut av = vec![0 as DummyType; len];
-
-    for idx in group_offset..(group_offset + group_len) {
-        let elem = unsafe { av.get_unchecked_mut(idx as usize) };
-        *elem = 1;
+pub(super) fn process_rename(
+    acc_predicates: &mut PlHashMap<Arc<str>, Node>,
+    expr_arena: &mut Arena<AExpr>,
+    existing: &[SmartString],
+    new: &[SmartString],
+) -> PolarsResult<Vec<Node>> {
+    let mut local_predicates = vec![];
+    for (existing, new) in existing.iter().zip(new.iter()) {
+        let has_existing = acc_predicates.contains_key(existing.as_str());
+        let has_new = acc_predicates.contains_key(new.as_str());
+        let has_both = has_existing && has_new;
+
+        // swapping path add to local for now
+        if has_both {
+            // Search for the key and add it to local because swapping is more complicated
+            if let Some(to_local) = acc_predicates.remove(new.as_str()) {
+                local_predicates.push(to_local);
+            } else {
+                // The keys can be combined eg. `a AND b AND c` in this case replacing/finding
+                // the key that should be renamed is more complicated, so for now
+                // we just move it to local.
+                remove_any_key_referencing_renamed(new, acc_predicates, &mut local_predicates)
+            }
+            continue;
+        }
+        // simple new name path
+        else {
+            // Find the key and update the predicate as well as the key
+            // This ensure the optimization is pushed down.
+            if let Some(node) = acc_predicates.remove(new.as_str()) {
+                let new_node = rename_matching_aexpr_leaf_names(node, expr_arena, new, existing);
+                acc_predicates.insert(predicate_to_key(new_node, expr_arena), new_node);
+            } else {
+                // The keys can be combined eg. `a AND b AND c` in this case replacing/finding
+                // the key that should be renamed is more complicated, so for now
+                // we just move it to local.
+                remove_any_key_referencing_renamed(new, acc_predicates, &mut local_predicates)
+            }
+        }
     }
-
-    ChunkedArray::from_vec(name, av)
-}
-
-fn sort_columns(mut columns: Vec<Series>) -> Vec<Series> {
-    columns.sort_by(|a, b| a.name().partial_cmp(b.name()).unwrap());
-    columns
+    Ok(local_predicates)
 }
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.17.4/local_dependencies/polars/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	    -p polars-lazy \
 	    -p polars-arrow \
 	    -p polars-utils \
 	    -p polars-ops \
 	    -p polars-error \
 	    -p polars-row \
 	    -p polars-time \
-			-p polars-sql
+		-p polars-sql
 
 clippy-default:
 	cargo clippy
 
 test:  ## Run tests
 	POLARS_NO_STREAMING_GROUPBY=1 POLARS_MAX_THREADS=4 cargo t -p polars-core test_4_threads
 	cargo test --all-features \
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -542,30 +542,30 @@
         {
             #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
             state.file_cache.assert_empty();
         }
         out
     }
 
-    //// Profile a LazyFrame.
-    ////
-    //// This will run the query and return a tuple
-    //// containing the materialized DataFrame and a DataFrame that contains profiling information
-    //// of each node that is executed.
-    ////
-    //// The units of the timings are microseconds.
+    /// Profile a LazyFrame.
+    ///
+    /// This will run the query and return a tuple
+    /// containing the materialized DataFrame and a DataFrame that contains profiling information
+    /// of each node that is executed.
+    ///
+    /// The units of the timings are microseconds.
     pub fn profile(self) -> PolarsResult<(DataFrame, DataFrame)> {
         let (mut state, mut physical_plan, _) = self.prepare_collect(false)?;
         state.time_nodes();
         let out = physical_plan.execute(&mut state)?;
         let timer_df = state.finish_timer()?;
         Ok((out, timer_df))
     }
 
-    //// Stream a query result into a parquet file. This is useful if the final result doesn't fit
+    /// Stream a query result into a parquet file. This is useful if the final result doesn't fit
     /// into memory. This methods will return an error if the query cannot be completely done in a
     /// streaming fashion.
     #[cfg(feature = "parquet")]
     pub fn sink_parquet(mut self, path: PathBuf, options: ParquetWriteOptions) -> PolarsResult<()> {
         self.opt_state.streaming = true;
         self.logical_plan = LogicalPlan::FileSink {
             input: Box::new(self.logical_plan),
@@ -580,15 +580,15 @@
             ComputeError: "cannot run the whole query in a streaming order; \
             use `collect().write_parquet()` instead"
         );
         let _ = physical_plan.execute(&mut state)?;
         Ok(())
     }
 
-    //// Stream a query result into an ipc/arrow file. This is useful if the final result doesn't fit
+    /// Stream a query result into an ipc/arrow file. This is useful if the final result doesn't fit
     /// into memory. This methods will return an error if the query cannot be completely done in a
     /// streaming fashion.
     #[cfg(feature = "ipc")]
     pub fn sink_ipc(mut self, path: PathBuf, options: IpcWriterOptions) -> PolarsResult<()> {
         self.opt_state.streaming = true;
         self.logical_plan = LogicalPlan::FileSink {
             input: Box::new(self.logical_plan),
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         let schema = self.get_input_schema(df);
         let field = self.to_field(&schema)?;
 
         // aggregate representation of the aggregation contexts
         // then unpack the lists and finally create iterators from this list chunked arrays.
         let mut iters = acs
             .iter_mut()
-            .map(|ac| ac.iter_groups())
+            .map(|ac| ac.iter_groups(self.pass_name_to_apply))
             .collect::<Vec<_>>();
 
         // length of the items to iterate over
         let len = iters[0].size_hint().0;
 
         if len == 0 {
             let out = Series::full_null(field.name(), 0, &field.dtype);
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
     ) -> PolarsResult<AggregationContext<'a>> {
         if self.null_propagate(&mut ac_l, &ac_r) {
             return Ok(ac_l);
         }
 
         let name = ac_l.series().name().to_string();
         let mut ca: ListChunked = ac_l
-            .iter_groups()
-            .zip(ac_r.iter_groups())
+            .iter_groups(false)
+            .zip(ac_r.iter_groups(false))
             .map(|(l, r)| {
                 match (l, r) {
                     (Some(l), Some(r)) => {
                         let l = l.as_ref();
                         let r = r.as_ref();
                         Some(apply_operator(l, r, self.op))
                     }
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         let ac_s_f = || self.input.evaluate_on_groups(df, groups, state);
         let ac_predicate_f = || self.by.evaluate_on_groups(df, groups, state);
 
         let (ac_s, ac_predicate) = POOL.install(|| rayon::join(ac_s_f, ac_predicate_f));
         let (mut ac_s, mut ac_predicate) = (ac_s?, ac_predicate?);
 
         if ac_predicate.is_aggregated() || ac_s.is_aggregated() {
-            let preds = ac_predicate.iter_groups();
+            let preds = ac_predicate.iter_groups(false);
             let s = ac_s.aggregated();
             let ca = s.list()?;
             let mut out = ca
                 .amortized_iter()
                 .zip(preds)
                 .map(|(opt_s, opt_pred)| match (opt_s, opt_pred) {
                     (Some(s), Some(pred)) => s.as_ref().filter(pred.as_ref().bool()?).map(Some),
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files 14% similar despite different names*

```diff
@@ -3,41 +3,51 @@
 use polars_core::series::unstable::UnstableSeries;
 
 use super::*;
 
 impl<'a> AggregationContext<'a> {
     pub(super) fn iter_groups(
         &mut self,
+        keep_names: bool,
     ) -> Box<dyn Iterator<Item = Option<UnstableSeries<'_>>> + '_> {
         match self.agg_state() {
             AggState::Literal(_) => {
                 self.groups();
                 let s = self.series().rechunk();
-                Box::new(LitIter::new(s.array_ref(0).clone(), self.groups.len()))
+                let name = if keep_names { s.name() } else { "" };
+                Box::new(LitIter::new(
+                    s.array_ref(0).clone(),
+                    self.groups.len(),
+                    name,
+                ))
             }
             AggState::AggregatedFlat(_) => {
                 self.groups();
                 let s = self.series();
+                let name = if keep_names { s.name() } else { "" };
                 Box::new(FlatIter::new(
                     s.array_ref(0).clone(),
                     self.groups.len(),
                     s.dtype(),
+                    name,
                 ))
             }
             AggState::AggregatedList(_) => {
                 let s = self.series();
                 let list = s.list().unwrap();
-                Box::new(list.amortized_iter())
+                let name = if keep_names { s.name() } else { "" };
+                Box::new(list.amortized_iter_with_name(name))
             }
             AggState::NotAggregated(_) => {
                 // we don't take the owned series as we want a reference
                 let _ = self.aggregated();
                 let s = self.series();
                 let list = s.list().unwrap();
-                Box::new(list.amortized_iter())
+                let name = if keep_names { s.name() } else { "" };
+                Box::new(list.amortized_iter_with_name(name))
             }
         }
     }
 }
 
 struct LitIter<'a> {
     len: usize,
@@ -45,16 +55,16 @@
     // UnstableSeries referenced that series
     #[allow(dead_code)]
     series_container: Pin<Box<Series>>,
     item: UnstableSeries<'a>,
 }
 
 impl<'a> LitIter<'a> {
-    fn new(array: ArrayRef, len: usize) -> Self {
-        let mut series_container = Box::pin(Series::try_from(("", array.clone())).unwrap());
+    fn new(array: ArrayRef, len: usize, name: &str) -> Self {
+        let mut series_container = Box::pin(Series::try_from((name, array.clone())).unwrap());
         let ref_s = &mut *series_container as *mut Series;
         Self {
             offset: 0,
             len,
             series_container,
             // Safety: we pinned the series so the location is still valid
             item: UnstableSeries::new(unsafe { &mut *ref_s }),
@@ -86,17 +96,17 @@
     // UnstableSeries referenced that series
     #[allow(dead_code)]
     series_container: Pin<Box<Series>>,
     item: UnstableSeries<'a>,
 }
 
 impl<'a> FlatIter<'a> {
-    fn new(array: ArrayRef, len: usize, logical: &DataType) -> Self {
+    fn new(array: ArrayRef, len: usize, logical: &DataType, name: &str) -> Self {
         let mut series_container = Box::pin(
-            Series::try_from(("", array.clone()))
+            Series::try_from((name, array.clone()))
                 .unwrap()
                 .cast(logical)
                 .unwrap(),
         );
         let ref_s = &mut *series_container as *mut Series;
         Self {
             array,
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 
 fn finish_as_iters<'a>(
     mut ac_truthy: AggregationContext<'a>,
     mut ac_falsy: AggregationContext<'a>,
     mut ac_mask: AggregationContext<'a>,
 ) -> PolarsResult<AggregationContext<'a>> {
     let mut ca: ListChunked = ac_truthy
-        .iter_groups()
-        .zip(ac_falsy.iter_groups())
-        .zip(ac_mask.iter_groups())
+        .iter_groups(false)
+        .zip(ac_falsy.iter_groups(false))
+        .zip(ac_mask.iter_groups(false))
         .map(|((truthy, falsy), mask)| {
             match (truthy, falsy, mask) {
                 (Some(truthy), Some(falsy), Some(mask)) => Some(
                     truthy
                         .as_ref()
                         .zip_with(mask.as_ref().bool()?, falsy.as_ref()),
                 ),
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 url = { version = "2.3.1", optional = true }
 xxhash-rust= { version = "0.8.6", features = ["xxh3"] }
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
     match dtype {
         #[cfg(feature = "dtype-categorical")]
         // arrow dictionaries are not nested as dictionaries, but only by their keys, so we must
         // change the list-value array to the keys and store the dictionary values in the datatype.
         // if a global string cache is set, we also must modify the keys.
         DataType::List(inner) if *inner == DataType::Categorical(None) => {
-            use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
             let array = concatenate_owned_unchecked(chunks).unwrap();
             let list_arr = array.as_any().downcast_ref::<ListArray<i64>>().unwrap();
             let values_arr = list_arr.values();
             let cat = unsafe {
                 Series::try_from_arrow_unchecked(
                     "",
                     vec![values_arr.clone()],
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,32 @@
     /// # Warning
     /// Though memory safe in the sense that it will not read unowned memory, UB, or memory leaks
     /// this function still needs precautions. The returned should never be cloned or taken longer
     /// than a single iteration, as every call on `next` of the iterator will change the contents of
     /// that Series.
     #[cfg(feature = "private")]
     pub fn amortized_iter(&self) -> AmortizedListIter<impl Iterator<Item = Option<ArrayBox>> + '_> {
+        self.amortized_iter_with_name("")
+    }
+
+    #[cfg(feature = "private")]
+    pub fn amortized_iter_with_name(
+        &self,
+        name: &str,
+    ) -> AmortizedListIter<impl Iterator<Item = Option<ArrayBox>> + '_> {
         // we create the series container from the inner array
         // so that the container has the proper dtype.
         let arr = self.downcast_iter().next().unwrap();
         let inner_values = arr.values();
 
         // Safety:
         // inner types logical type fits physical type
         let series_container = unsafe {
             Box::new(Series::from_chunks_and_dtype_unchecked(
-                "",
+                name,
                 vec![inner_values.clone()],
                 &self.inner_dtype(),
             ))
         };
 
         let ptr = series_container.array_ref(0) as *const ArrayRef as *mut ArrayRef;
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 mod trusted_len;
 pub mod upstream_traits;
 
 use std::mem;
 use std::slice::Iter;
 
 use bitflags::bitflags;
+use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
 use polars_arrow::prelude::*;
 
 use crate::series::IsSorted;
 use crate::utils::{first_non_null, last_non_null, CustomIterTools};
 
 #[cfg(not(feature = "dtype-categorical"))]
 pub struct RevMapping {}
@@ -232,22 +233,15 @@
     /// no bitmap means no null values.
     pub fn has_validity(&self) -> bool {
         self.iter_validities().any(|valid| valid.is_some())
     }
 
     /// Shrink the capacity of this array to fit its length.
     pub fn shrink_to_fit(&mut self) {
-        self.chunks = vec![arrow::compute::concatenate::concatenate(
-            self.chunks
-                .iter()
-                .map(|a| &**a)
-                .collect::<Vec<_>>()
-                .as_slice(),
-        )
-        .unwrap()];
+        self.chunks = vec![concatenate_owned_unchecked(self.chunks.as_slice()).unwrap()];
     }
 
     /// Unpack a Series to the same physical type.
     ///
     /// # Safety
     ///
     /// This is unsafe as the dtype may be incorrect and
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #[cfg(feature = "object")]
 use arrow::array::Array;
-use arrow::compute::concatenate;
+use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
 
 use super::*;
 #[cfg(feature = "object")]
 use crate::chunked_array::object::builder::ObjectChunkedBuilder;
 use crate::utils::slice_offsets;
 
 #[inline]
@@ -89,18 +89,15 @@
         match self.dtype() {
             #[cfg(feature = "object")]
             DataType::Object(_) => {
                 panic!("implementation error")
             }
             _ => {
                 fn inner_rechunk(chunks: &[ArrayRef]) -> Vec<ArrayRef> {
-                    vec![concatenate::concatenate(
-                        chunks.iter().map(|a| &**a).collect::<Vec<_>>().as_slice(),
-                    )
-                    .unwrap()]
+                    vec![concatenate_owned_unchecked(chunks).unwrap()]
                 }
 
                 if self.chunks.len() == 1 {
                     self.clone()
                 } else {
                     let chunks = inner_rechunk(&self.chunks);
                     self.copy_with_chunks(chunks, true, true)
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files 1% similar despite different names*

```diff
@@ -693,14 +693,24 @@
                     unsafe { arr.deref_unchecked().value(*idx as usize) }
                 };
                 Some(s)
             }
             _ => None,
         }
     }
+
+    pub fn is_nested_null(&self) -> bool {
+        match self {
+            AnyValue::Null => true,
+            AnyValue::List(s) => s.dtype().is_nested_null(),
+            #[cfg(feature = "dtype-struct")]
+            AnyValue::Struct(_, _, _) => self._iter_struct_av().all(|av| av.is_nested_null()),
+            _ => false,
+        }
+    }
 }
 
 impl<'a> From<AnyValue<'a>> for Option<i64> {
     fn from(val: AnyValue<'a>) -> Self {
         use AnyValue::*;
         match val {
             Null => None,
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,25 @@
             Struct(fields) => {
                 let fields = fields.iter().map(|fld| fld.to_arrow()).collect();
                 ArrowDataType::Struct(fields)
             }
             Unknown => unreachable!(),
         }
     }
+
+    pub fn is_nested_null(&self) -> bool {
+        use DataType::*;
+        match self {
+            Null => true,
+            List(field) => field.is_nested_null(),
+            #[cfg(feature = "dtype-struct")]
+            Struct(fields) => fields.iter().all(|fld| fld.dtype.is_nested_null()),
+            _ => false,
+        }
+    }
 }
 
 impl PartialEq<ArrowDataType> for DataType {
     fn eq(&self, other: &ArrowDataType) -> bool {
         let dt: DataType = other.into();
         self == &dt
     }
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 mod agg_list;
+mod boolean;
 mod dispatch;
+mod utf8;
 
 pub use agg_list::*;
 use arrow::bitmap::{Bitmap, MutableBitmap};
 use arrow::types::simd::Simd;
 use arrow::types::NativeType;
 use num_traits::pow::Pow;
 use num_traits::{Bounded, Num, NumCast, ToPrimitive, Zero};
@@ -24,14 +26,18 @@
 #[cfg(feature = "object")]
 use crate::frame::groupby::GroupsIndicator;
 use crate::prelude::*;
 use crate::series::implementations::SeriesWrap;
 use crate::series::IsSorted;
 use crate::{apply_method_physical_integer, POOL};
 
+fn idx2usize(idx: &[IdxSize]) -> impl Iterator<Item = usize> + ExactSizeIterator + '_ {
+    idx.iter().map(|i| *i as usize)
+}
+
 // if the windows overlap, we can use the rolling_<agg> kernels
 // they maintain state, which saves a lot of compute by not naively traversing all elements every
 // window
 //
 // if the windows don't overlap, we should not use these kernels as they are single threaded, so
 // we miss out on easy parallelization.
 pub fn _use_rolling_kernels(groups: &GroupsSlice, chunks: &[ArrayRef]) -> bool {
@@ -151,30 +157,14 @@
     T: PolarsNumericType,
     ChunkedArray<T>: IntoSeries,
 {
     let ca: ChunkedArray<T> = POOL.install(|| groups.into_par_iter().map(f).collect());
     ca.into_series()
 }
 
-pub fn _agg_helper_idx_bool<F>(groups: &GroupsIdx, f: F) -> Series
-where
-    F: Fn((IdxSize, &Vec<IdxSize>)) -> Option<bool> + Send + Sync,
-{
-    let ca: BooleanChunked = POOL.install(|| groups.into_par_iter().map(f).collect());
-    ca.into_series()
-}
-
-pub fn _agg_helper_idx_utf8<'a, F>(groups: &'a GroupsIdx, f: F) -> Series
-where
-    F: Fn((IdxSize, &'a Vec<IdxSize>)) -> Option<&'a str> + Send + Sync,
-{
-    let ca: Utf8Chunked = POOL.install(|| groups.into_par_iter().map(f).collect());
-    ca.into_series()
-}
-
 // helper that iterates on the `all: Vec<Vec<u32>` collection
 // this doesn't have traverse the `first: Vec<u32>` memory and is therefore faster
 fn agg_helper_idx_on_all<T, F>(groups: &GroupsIdx, f: F) -> Series
 where
     F: Fn(&Vec<IdxSize>) -> Option<T::Native> + Send + Sync,
     T: PolarsNumericType,
     ChunkedArray<T>: IntoSeries,
@@ -189,243 +179,14 @@
     T: PolarsNumericType,
     ChunkedArray<T>: IntoSeries,
 {
     let ca: ChunkedArray<T> = POOL.install(|| groups.par_iter().copied().map(f).collect());
     ca.into_series()
 }
 
-pub fn _agg_helper_slice_bool<F>(groups: &[[IdxSize; 2]], f: F) -> Series
-where
-    F: Fn([IdxSize; 2]) -> Option<bool> + Send + Sync,
-{
-    let ca: BooleanChunked = POOL.install(|| groups.par_iter().copied().map(f).collect());
-    ca.into_series()
-}
-
-pub fn _agg_helper_slice_utf8<'a, F>(groups: &'a [[IdxSize; 2]], f: F) -> Series
-where
-    F: Fn([IdxSize; 2]) -> Option<&'a str> + Send + Sync,
-{
-    let ca: Utf8Chunked = POOL.install(|| groups.par_iter().copied().map(f).collect());
-    ca.into_series()
-}
-
-impl BooleanChunked {
-    pub(crate) unsafe fn agg_min(&self, groups: &GroupsProxy) -> Series {
-        // faster paths
-        match (self.is_sorted_flag2(), self.null_count()) {
-            (IsSorted::Ascending, 0) => {
-                return self.clone().into_series().agg_first(groups);
-            }
-            (IsSorted::Descending, 0) => {
-                return self.clone().into_series().agg_last(groups);
-            }
-            _ => {}
-        }
-        match groups {
-            GroupsProxy::Idx(groups) => _agg_helper_idx_bool(groups, |(first, idx)| {
-                debug_assert!(idx.len() <= self.len());
-                if idx.is_empty() {
-                    None
-                } else if idx.len() == 1 {
-                    self.get(first as usize)
-                } else {
-                    // TODO! optimize this
-                    // can just check if any is false and early stop
-                    let take = { self.take_unchecked(idx.into()) };
-                    take.min()
-                }
-            }),
-            GroupsProxy::Slice {
-                groups: groups_slice,
-                ..
-            } => _agg_helper_slice_bool(groups_slice, |[first, len]| {
-                debug_assert!(len <= self.len() as IdxSize);
-                match len {
-                    0 => None,
-                    1 => self.get(first as usize),
-                    _ => {
-                        let arr_group = _slice_from_offsets(self, first, len);
-                        arr_group.min()
-                    }
-                }
-            }),
-        }
-    }
-    pub(crate) unsafe fn agg_max(&self, groups: &GroupsProxy) -> Series {
-        // faster paths
-        match (self.is_sorted_flag2(), self.null_count()) {
-            (IsSorted::Ascending, 0) => {
-                return self.clone().into_series().agg_last(groups);
-            }
-            (IsSorted::Descending, 0) => {
-                return self.clone().into_series().agg_first(groups);
-            }
-            _ => {}
-        }
-
-        match groups {
-            GroupsProxy::Idx(groups) => _agg_helper_idx_bool(groups, |(first, idx)| {
-                debug_assert!(idx.len() <= self.len());
-                if idx.is_empty() {
-                    None
-                } else if idx.len() == 1 {
-                    self.get(first as usize)
-                } else {
-                    // TODO! optimize this
-                    // can just check if any is true and early stop
-                    let take = { self.take_unchecked(idx.into()) };
-                    take.max()
-                }
-            }),
-            GroupsProxy::Slice {
-                groups: groups_slice,
-                ..
-            } => _agg_helper_slice_bool(groups_slice, |[first, len]| {
-                debug_assert!(len <= self.len() as IdxSize);
-                match len {
-                    0 => None,
-                    1 => self.get(first as usize),
-                    _ => {
-                        let arr_group = _slice_from_offsets(self, first, len);
-                        arr_group.max()
-                    }
-                }
-            }),
-        }
-    }
-    pub(crate) unsafe fn agg_sum(&self, groups: &GroupsProxy) -> Series {
-        self.cast(&IDX_DTYPE).unwrap().agg_sum(groups)
-    }
-}
-
-impl Utf8Chunked {
-    #[allow(clippy::needless_lifetimes)]
-    pub(crate) unsafe fn agg_min<'a>(&'a self, groups: &GroupsProxy) -> Series {
-        // faster paths
-        match (&self.is_sorted_flag2(), &self.null_count()) {
-            (IsSorted::Ascending, 0) => {
-                return self.clone().into_series().agg_first(groups);
-            }
-            (IsSorted::Descending, 0) => {
-                return self.clone().into_series().agg_last(groups);
-            }
-            _ => {}
-        }
-
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let ca_self = self.rechunk();
-                let arr = ca_self.downcast_iter().next().unwrap();
-                _agg_helper_idx_utf8(groups, |(first, idx)| {
-                    debug_assert!(idx.len() <= ca_self.len());
-                    if idx.is_empty() {
-                        None
-                    } else if idx.len() == 1 {
-                        arr.get_unchecked(first as usize)
-                    } else if self.null_count() == 0 {
-                        take_agg_utf8_iter_unchecked_no_null(
-                            arr,
-                            indexes_to_usizes(idx),
-                            |acc, v| if acc < v { acc } else { v },
-                        )
-                    } else {
-                        take_agg_utf8_iter_unchecked(
-                            arr,
-                            indexes_to_usizes(idx),
-                            |acc, v| if acc < v { acc } else { v },
-                            idx.len() as IdxSize,
-                        )
-                    }
-                })
-            }
-            GroupsProxy::Slice {
-                groups: groups_slice,
-                ..
-            } => _agg_helper_slice_utf8(groups_slice, |[first, len]| {
-                debug_assert!(len <= self.len() as IdxSize);
-                match len {
-                    0 => None,
-                    1 => self.get(first as usize),
-                    _ => {
-                        let arr_group = _slice_from_offsets(self, first, len);
-                        let borrowed = arr_group.min_str();
-
-                        // Safety:
-                        // The borrowed has `arr_group`s lifetime, but it actually points to data
-                        // hold by self. Here we tell the compiler that.
-                        unsafe { std::mem::transmute::<Option<&str>, Option<&'a str>>(borrowed) }
-                    }
-                }
-            }),
-        }
-    }
-
-    #[allow(clippy::needless_lifetimes)]
-    pub(crate) unsafe fn agg_max<'a>(&'a self, groups: &GroupsProxy) -> Series {
-        // faster paths
-        match (self.is_sorted_flag2(), self.null_count()) {
-            (IsSorted::Ascending, 0) => {
-                return self.clone().into_series().agg_last(groups);
-            }
-            (IsSorted::Descending, 0) => {
-                return self.clone().into_series().agg_first(groups);
-            }
-            _ => {}
-        }
-
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let ca_self = self.rechunk();
-                let arr = ca_self.downcast_iter().next().unwrap();
-                _agg_helper_idx_utf8(groups, |(first, idx)| {
-                    debug_assert!(idx.len() <= self.len());
-                    if idx.is_empty() {
-                        None
-                    } else if idx.len() == 1 {
-                        ca_self.get(first as usize)
-                    } else if ca_self.null_count() == 0 {
-                        take_agg_utf8_iter_unchecked_no_null(
-                            arr,
-                            indexes_to_usizes(idx),
-                            |acc, v| if acc > v { acc } else { v },
-                        )
-                    } else {
-                        take_agg_utf8_iter_unchecked(
-                            arr,
-                            indexes_to_usizes(idx),
-                            |acc, v| if acc > v { acc } else { v },
-                            idx.len() as IdxSize,
-                        )
-                    }
-                })
-            }
-            GroupsProxy::Slice {
-                groups: groups_slice,
-                ..
-            } => _agg_helper_slice_utf8(groups_slice, |[first, len]| {
-                debug_assert!(len <= self.len() as IdxSize);
-                match len {
-                    0 => None,
-                    1 => self.get(first as usize),
-                    _ => {
-                        let arr_group = _slice_from_offsets(self, first, len);
-                        let borrowed = arr_group.max_str();
-
-                        // Safety:
-                        // The borrowed has `arr_group`s lifetime, but it actually points to data
-                        // hold by self. Here we tell the compiler that.
-                        unsafe { std::mem::transmute::<Option<&str>, Option<&'a str>>(borrowed) }
-                    }
-                }
-            }),
-        }
-    }
-}
-
 #[inline(always)]
 fn take_min<T: PartialOrd>(a: T, b: T) -> T {
     if a < b {
         a
     } else {
         b
     }
@@ -615,31 +376,32 @@
             }
             _ => {}
         }
         match groups {
             GroupsProxy::Idx(groups) => {
                 let ca = self.rechunk();
                 let arr = ca.downcast_iter().next().unwrap();
+                let no_nulls = arr.null_count() == 0;
                 _agg_helper_idx::<T, _>(groups, |(first, idx)| {
                     debug_assert!(idx.len() <= arr.len());
                     if idx.is_empty() {
                         None
                     } else if idx.len() == 1 {
                         arr.get(first as usize)
-                    } else if arr.null_count() == 0 {
+                    } else if no_nulls {
                         Some(take_agg_no_null_primitive_iter_unchecked(
                             arr,
-                            idx.iter().map(|i| *i as usize),
+                            idx2usize(idx),
                             take_min,
                             T::Native::max_value(),
                         ))
                     } else {
                         take_agg_primitive_iter_unchecked::<T::Native, _, _>(
                             arr,
-                            idx.iter().map(|i| *i as usize),
+                            idx2usize(idx),
                             take_min,
                             T::Native::max_value(),
                             idx.len() as IdxSize,
                         )
                     }
                 })
             }
@@ -692,33 +454,34 @@
             _ => {}
         }
 
         match groups {
             GroupsProxy::Idx(groups) => {
                 let ca = self.rechunk();
                 let arr = ca.downcast_iter().next().unwrap();
+                let no_nulls = arr.null_count() == 0;
                 _agg_helper_idx::<T, _>(groups, |(first, idx)| {
                     debug_assert!(idx.len() <= arr.len());
                     if idx.is_empty() {
                         None
                     } else if idx.len() == 1 {
                         arr.get(first as usize)
-                    } else if arr.null_count() == 0 {
+                    } else if no_nulls {
                         Some({
                             take_agg_no_null_primitive_iter_unchecked(
                                 arr,
-                                idx.iter().map(|i| *i as usize),
+                                idx2usize(idx),
                                 take_max,
                                 T::Native::min_value(),
                             )
                         })
                     } else {
                         take_agg_primitive_iter_unchecked::<T::Native, _, _>(
                             arr,
-                            idx.iter().map(|i| *i as usize),
+                            idx2usize(idx),
                             take_max,
                             T::Native::min_value(),
                             idx.len() as IdxSize,
                         )
                     }
                 })
             }
@@ -760,31 +523,32 @@
     }
 
     pub(crate) unsafe fn agg_sum(&self, groups: &GroupsProxy) -> Series {
         match groups {
             GroupsProxy::Idx(groups) => {
                 let ca = self.rechunk();
                 let arr = ca.downcast_iter().next().unwrap();
+                let no_nulls = arr.null_count() == 0;
                 _agg_helper_idx::<T, _>(groups, |(first, idx)| {
                     debug_assert!(idx.len() <= self.len());
                     if idx.is_empty() {
                         None
                     } else if idx.len() == 1 {
                         arr.get(first as usize)
-                    } else if arr.null_count() == 0 {
+                    } else if no_nulls {
                         Some(take_agg_no_null_primitive_iter_unchecked(
                             arr,
-                            idx.iter().map(|i| *i as usize),
+                            idx2usize(idx),
                             |a, b| a + b,
                             T::Native::zero(),
                         ))
                     } else {
                         take_agg_primitive_iter_unchecked::<T::Native, _, _>(
                             arr,
-                            idx.iter().map(|i| *i as usize),
+                            idx2usize(idx),
                             |a, b| a + b,
                             T::Native::zero(),
                             idx.len() as IdxSize,
                         )
                     }
                 })
             }
@@ -833,58 +597,52 @@
         + QuantileAggSeries,
     T::Native: Simd + NumericNative + Pow<T::Native, Output = T::Native>,
     <T::Native as Simd>::Simd: std::ops::Add<Output = <T::Native as Simd>::Simd>
         + arrow::compute::aggregate::Sum<T::Native>
         + arrow::compute::aggregate::SimdOrd<T::Native>,
 {
     pub(crate) unsafe fn agg_mean(&self, groups: &GroupsProxy) -> Series {
+        let ca = self.rechunk();
+        let arr = ca.downcast_iter().next().unwrap();
+        let no_nulls = arr.null_count() == 0;
         match groups {
             GroupsProxy::Idx(groups) => {
                 _agg_helper_idx::<T, _>(groups, |(first, idx)| {
                     // this can fail due to a bug in lazy code.
                     // here users can create filters in aggregations
                     // and thereby creating shorter columns than the original group tuples.
                     // the group tuples are modified, but if that's done incorrect there can be out of bounds
                     // access
                     debug_assert!(idx.len() <= self.len());
                     let out = if idx.is_empty() {
                         None
                     } else if idx.len() == 1 {
                         self.get(first as usize).map(|sum| sum.to_f64().unwrap())
+                    } else if no_nulls {
+                        take_agg_no_null_primitive_iter_unchecked(
+                            self.downcast_iter().next().unwrap(),
+                            idx2usize(idx),
+                            |a, b| a + b,
+                            T::Native::zero(),
+                        )
+                        .to_f64()
+                        .map(|sum| sum / idx.len() as f64)
                     } else {
-                        match (self.has_validity(), self.chunks.len()) {
-                            (false, 1) => {
-                                take_agg_no_null_primitive_iter_unchecked(
-                                    self.downcast_iter().next().unwrap(),
-                                    idx.iter().map(|i| *i as usize),
-                                    |a, b| a + b,
-                                    T::Native::zero(),
-                                )
-                            }
-                            .to_f64()
-                            .map(|sum| sum / idx.len() as f64),
-                            (_, 1) => {
-                                take_agg_primitive_iter_unchecked_count_nulls::<T::Native, _, _, _>(
-                                    self.downcast_iter().next().unwrap(),
-                                    idx.iter().map(|i| *i as usize),
-                                    |a, b| a + b,
-                                    T::Native::zero(),
-                                    idx.len() as IdxSize,
-                                )
-                            }
-                            .map(|(sum, null_count)| {
-                                sum.to_f64()
-                                    .map(|sum| sum / (idx.len() as f64 - null_count as f64))
-                                    .unwrap()
-                            }),
-                            _ => {
-                                let take = { self.take_unchecked(idx.into()) };
-                                take.mean()
-                            }
-                        }
+                        take_agg_primitive_iter_unchecked_count_nulls::<T::Native, _, _, _>(
+                            self.downcast_iter().next().unwrap(),
+                            idx2usize(idx),
+                            |a, b| a + b,
+                            T::Native::zero(),
+                            idx.len() as IdxSize,
+                        )
+                        .map(|(sum, null_count)| {
+                            sum.to_f64()
+                                .map(|sum| sum / (idx.len() as f64 - null_count as f64))
+                                .unwrap()
+                        })
                     };
                     out.map(|flt| NumCast::from(flt).unwrap())
                 })
             }
             GroupsProxy::Slice { groups, .. } => {
                 if _use_rolling_kernels(groups, self.chunks()) {
                     let arr = self.downcast_iter().next().unwrap();
@@ -916,15 +674,15 @@
                     })
                 }
             }
         }
     }
 
     pub(crate) unsafe fn agg_var(&self, groups: &GroupsProxy, ddof: u8) -> Series {
-        let ca = &self.0;
+        let ca = &self.0.rechunk();
         match groups {
             GroupsProxy::Idx(groups) => {
                 let ca = ca.rechunk();
                 agg_helper_idx_on_all::<T, _>(groups, |idx| {
                     debug_assert!(idx.len() <= ca.len());
                     if idx.is_empty() {
                         return None;
@@ -963,15 +721,15 @@
                         }
                     })
                 }
             }
         }
     }
     pub(crate) unsafe fn agg_std(&self, groups: &GroupsProxy, ddof: u8) -> Series {
-        let ca = &self.0;
+        let ca = &self.0.rechunk();
         match groups {
             GroupsProxy::Idx(groups) => {
                 let ca = ca.rechunk();
                 agg_helper_idx_on_all::<T, _>(groups, |idx| {
                     debug_assert!(idx.len() <= ca.len());
                     if idx.is_empty() {
                         return None;
@@ -1066,15 +824,15 @@
                     } else if idx.len() == 1 {
                         self.get(first as usize).map(|sum| sum.to_f64().unwrap())
                     } else {
                         match (self.has_validity(), self.chunks.len()) {
                             (false, 1) => {
                                 take_agg_no_null_primitive_iter_unchecked(
                                     self.downcast_iter().next().unwrap(),
-                                    idx.iter().map(|i| *i as usize),
+                                    idx2usize(idx),
                                     |a, b| a + b,
                                     0.0f64,
                                 )
                             }
                             .to_f64()
                             .map(|sum| sum / idx.len() as f64),
                             (_, 1) => {
@@ -1082,15 +840,15 @@
                                     take_agg_primitive_iter_unchecked_count_nulls::<
                                         T::Native,
                                         f64,
                                         _,
                                         _,
                                     >(
                                         self.downcast_iter().next().unwrap(),
-                                        idx.iter().map(|i| *i as usize),
+                                        idx2usize(idx),
                                         |a, b| a + b,
                                         0.0,
                                         idx.len() as IdxSize,
                                     )
                                 }
                                 .map(|(sum, null_count)| {
                                     sum / (idx.len() as f64 - null_count as f64)
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files 0% similar despite different names*

```diff
@@ -159,18 +159,20 @@
         .collect()
 }
 
 fn splitted_to_opt_vec<T>(splitted: &[ChunkedArray<T>]) -> Vec<Vec<Option<T::Native>>>
 where
     T: PolarsNumericType,
 {
-    splitted
-        .iter()
-        .map(|ca| ca.into_iter().collect_trusted::<Vec<_>>())
-        .collect()
+    POOL.install(|| {
+        splitted
+            .par_iter()
+            .map(|ca| ca.into_iter().collect_trusted::<Vec<_>>())
+            .collect()
+    })
 }
 
 // returns the join tuples and whether or not the lhs tuples are sorted
 fn num_group_join_inner<T>(
     left: &ChunkedArray<T>,
     right: &ChunkedArray<T>,
 ) -> ((Vec<IdxSize>, Vec<IdxSize>), bool)
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     let lefts = indexes.iter().map(|t| &t.0).collect::<Vec<_>>();
     let rights = indexes.iter().map(|t| &t.1).collect::<Vec<_>>();
 
     (flatten(&lefts, None), flatten(&rights, None))
 }
 
 #[cfg(feature = "performant")]
-pub(super) fn par_sorted_merge_inner(
+pub(super) fn par_sorted_merge_inner_no_nulls(
     s_left: &Series,
     s_right: &Series,
 ) -> (Vec<IdxSize>, Vec<IdxSize>) {
     // Don't use bit_repr here. It messes up sortedness.
     debug_assert_eq!(s_left.dtype(), s_right.dtype());
     let s_left = s_left.to_physical_repr();
     let s_right = s_right.to_physical_repr();
@@ -194,57 +194,63 @@
     // the `arg_sort` indices to revert the sort once the join keys are determined.
     let size_factor_rhs = s_right.len() as f32 / s_left.len() as f32;
     let size_factor_lhs = s_left.len() as f32 / s_right.len() as f32;
     let size_factor_acceptable = std::env::var("POLARS_JOIN_SORT_FACTOR")
         .map(|s| s.parse::<f32>().unwrap())
         .unwrap_or(1.0);
     let is_numeric = s_left.dtype().to_physical().is_numeric();
-    match (s_left.is_sorted_flag(), s_right.is_sorted_flag()) {
-        (IsSorted::Ascending, IsSorted::Ascending) if is_numeric => {
+
+    let no_nulls = s_left.null_count() == 0 && s_right.null_count() == 0;
+    match (s_left.is_sorted_flag(), s_right.is_sorted_flag(), no_nulls) {
+        (IsSorted::Ascending, IsSorted::Ascending, true) if is_numeric => {
             if verbose {
                 eprintln!("inner join: keys are sorted: use sorted merge join");
             }
-            (par_sorted_merge_inner(s_left, s_right), true)
+            (par_sorted_merge_inner_no_nulls(s_left, s_right), true)
         }
-        (IsSorted::Ascending, _) if is_numeric && size_factor_rhs < size_factor_acceptable => {
+        (IsSorted::Ascending, _, true)
+            if is_numeric && size_factor_rhs < size_factor_acceptable =>
+        {
             if verbose {
                 eprintln!("right key will be descending sorted in inner join operation.")
             }
 
             let sort_idx = s_right.arg_sort(SortOptions {
                 descending: false,
                 nulls_last: false,
                 multithreaded: true,
             });
             let s_right = unsafe { s_right.take_unchecked(&sort_idx).unwrap() };
-            let ids = par_sorted_merge_inner(s_left, &s_right);
+            let ids = par_sorted_merge_inner_no_nulls(s_left, &s_right);
             let reverse_idx_map = create_reverse_map_from_arg_sort(sort_idx);
 
             let (left, mut right) = ids;
 
             POOL.install(|| {
                 right.par_iter_mut().for_each(|idx| {
                     *idx = unsafe { *reverse_idx_map.get_unchecked(*idx as usize) };
                 });
             });
 
             ((left, right), true)
         }
-        (_, IsSorted::Ascending) if is_numeric && size_factor_lhs < size_factor_acceptable => {
+        (_, IsSorted::Ascending, true)
+            if is_numeric && size_factor_lhs < size_factor_acceptable =>
+        {
             if verbose {
                 eprintln!("left key will be descending sorted in inner join operation.")
             }
 
             let sort_idx = s_left.arg_sort(SortOptions {
                 descending: false,
                 nulls_last: false,
                 multithreaded: true,
             });
             let s_left = unsafe { s_left.take_unchecked(&sort_idx).unwrap() };
-            let ids = par_sorted_merge_inner(&s_left, s_right);
+            let ids = par_sorted_merge_inner_no_nulls(&s_left, s_right);
             let reverse_idx_map = create_reverse_map_from_arg_sort(sort_idx);
 
             let (mut left, right) = ids;
 
             POOL.install(|| {
                 left.par_iter_mut().for_each(|idx| {
                     *idx = unsafe { *reverse_idx_map.get_unchecked(*idx as usize) };
@@ -267,23 +273,27 @@
 pub(super) fn sort_or_hash_left(s_left: &Series, s_right: &Series, verbose: bool) -> LeftJoinIds {
     let size_factor_rhs = s_right.len() as f32 / s_left.len() as f32;
     let size_factor_acceptable = std::env::var("POLARS_JOIN_SORT_FACTOR")
         .map(|s| s.parse::<f32>().unwrap())
         .unwrap_or(1.0);
     let is_numeric = s_left.dtype().to_physical().is_numeric();
 
-    match (s_left.is_sorted_flag(), s_right.is_sorted_flag()) {
-        (IsSorted::Ascending, IsSorted::Ascending) if is_numeric => {
+    let no_nulls = s_left.null_count() == 0 && s_right.null_count() == 0;
+
+    match (s_left.is_sorted_flag(), s_right.is_sorted_flag(), no_nulls) {
+        (IsSorted::Ascending, IsSorted::Ascending, true) if is_numeric => {
             if verbose {
                 eprintln!("left join: keys are sorted: use sorted merge join");
             }
             let (left_idx, right_idx) = par_sorted_merge_left(s_left, s_right);
             to_left_join_ids(left_idx, right_idx)
         }
-        (IsSorted::Ascending, _) if is_numeric && size_factor_rhs < size_factor_acceptable => {
+        (IsSorted::Ascending, _, true)
+            if is_numeric && size_factor_rhs < size_factor_acceptable =>
+        {
             if verbose {
                 eprintln!("right key will be reverse sorted in left join operation.")
             }
 
             let sort_idx = s_right.arg_sort(SortOptions {
                 descending: false,
                 nulls_last: false,
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3157,26 +3157,26 @@
             .iter()
             .map(|s| Ok(s.dtype().clone()))
             .reduce(|acc, b| try_get_supertype(&acc?, &b.unwrap()))
     }
 
     #[cfg(feature = "chunked_ids")]
     #[doc(hidden)]
-    //// Take elements by a slice of [`ChunkId`]s.
+    /// Take elements by a slice of [`ChunkId`]s.
     /// # Safety
     /// Does not do any bound checks.
     /// `sorted` indicates if the chunks are sorted.
     #[doc(hidden)]
     pub unsafe fn _take_chunked_unchecked_seq(&self, idx: &[ChunkId], sorted: IsSorted) -> Self {
         let cols = self.apply_columns(&|s| s._take_chunked_unchecked(idx, sorted));
 
         DataFrame::new_no_checks(cols)
     }
     #[cfg(feature = "chunked_ids")]
-    //// Take elements by a slice of optional [`ChunkId`]s.
+    /// Take elements by a slice of optional [`ChunkId`]s.
     /// # Safety
     /// Does not do any bound checks.
     #[doc(hidden)]
     pub unsafe fn _take_opt_chunked_unchecked_seq(&self, idx: &[Option<ChunkId>]) -> Self {
         let cols = self.apply_columns(&|s| match s.dtype() {
             DataType::Utf8 => s._take_opt_chunked_unchecked_threaded(idx, true),
             _ => s._take_opt_chunked_unchecked(idx),
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
             Utf8 => AnyValueBuffer::Utf8(Utf8ChunkedBuilder::new("", len, len * 5)),
             // Struct and List can be recursive so use anyvalues for that
             dt => AnyValueBuffer::All(dt.clone(), Vec::with_capacity(len)),
         }
     }
 }
 
-//// An `AnyValyeBuffer` that should be used when we trust the builder
+/// An `AnyValyeBuffer` that should be used when we trust the builder
 #[derive(Clone)]
 pub enum AnyValueBufferTrusted<'a> {
     Boolean(BooleanChunkedBuilder),
     #[cfg(feature = "dtype-i8")]
     Int8(PrimitiveChunkedBuilder<Int8Type>),
     #[cfg(feature = "dtype-i16")]
     Int16(PrimitiveChunkedBuilder<Int16Type>),
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         let mut rows = arr
             .values_iter()
             .enumerate_idx()
             .map(|(idx, bytes)| CompareRow { idx, bytes })
             .collect::<Vec<_>>();
 
         let sorted = if k >= self.height() {
+            rows.sort_unstable();
             &rows
         } else {
             let (lower, _el, _upper) = rows.select_nth_unstable(k);
             lower.sort_unstable();
             &*lower
         };
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files 2% similar despite different names*

```diff
@@ -351,16 +351,35 @@
             dt => panic!("{dt:?} not supported"),
         };
         s.rename(name);
         Ok(s)
     }
 
     pub fn from_any_values(name: &str, avs: &[AnyValue], strict: bool) -> PolarsResult<Series> {
-        match avs.iter().find(|av| !matches!(av, AnyValue::Null)) {
-            None => Ok(Series::full_null(name, avs.len(), &DataType::Null)),
+        let mut all_flat_null = true;
+        match avs.iter().find(|av| {
+            if !matches!(av, AnyValue::Null) {
+                all_flat_null = false;
+            }
+            !av.is_nested_null()
+        }) {
+            None => {
+                if all_flat_null {
+                    Ok(Series::full_null(name, avs.len(), &DataType::Null))
+                } else {
+                    // second pass and check for the nested null value that toggled `all_flat_null` to false
+                    // e.g. a list<null>
+                    if let Some(av) = avs.iter().find(|av| !matches!(av, AnyValue::Null)) {
+                        let dtype: DataType = av.into();
+                        Series::from_any_values_and_dtype(name, avs, &dtype, strict)
+                    } else {
+                        unreachable!()
+                    }
+                }
+            }
             Some(av) => {
                 #[cfg(feature = "dtype-decimal")]
                 {
                     if let AnyValue::Decimal(_, _) = av {
                         let mut s = any_values_to_decimal(avs, None, None)?.into_series();
                         s.rename(name);
                         return Ok(s);
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/from.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #[cfg(any(
     feature = "dtype-date",
     feature = "dtype-datetime",
     feature = "dtype-time"
 ))]
 use arrow::temporal_conversions::*;
 use polars_arrow::compute::cast::cast;
-#[cfg(feature = "dtype-struct")]
+#[cfg(any(feature = "dtype-struct", feature = "dtype-categorical"))]
 use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
 
 use crate::chunked_array::cast::cast_chunks;
 #[cfg(feature = "object")]
 use crate::chunked_array::object::extension::polars_extension::PolarsExtension;
 #[cfg(feature = "object")]
 use crate::chunked_array::object::extension::EXTENSION_NAME;
@@ -206,16 +206,15 @@
                 panic!("activate dtype-categorical to convert dictionary arrays")
             }
             #[cfg(feature = "dtype-categorical")]
             ArrowDataType::Dictionary(key_type, value_type, _) => {
                 use arrow::datatypes::IntegerType;
                 // don't spuriously call this; triggers a read on mmapped data
                 let arr = if chunks.len() > 1 {
-                    let chunks = chunks.iter().map(|arr| &**arr).collect::<Vec<_>>();
-                    arrow::compute::concatenate::concatenate(&chunks)?
+                    concatenate_owned_unchecked(&chunks)?
                 } else {
                     chunks[0].clone()
                 };
 
                 if !matches!(
                     value_type.as_ref(),
                     ArrowDataType::Utf8 | ArrowDataType::LargeUtf8 | ArrowDataType::Null
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
     /// If the [`DataType`] is one of `{Int8, UInt8, Int16, UInt16}` the `Series` is
     /// first cast to `Int64` to prevent overflow issues.
     pub fn sum_as_series(&self) -> Series {
         use DataType::*;
         if self.is_empty()
             && (self.dtype().is_numeric() || matches!(self.dtype(), DataType::Boolean))
         {
-            return Series::new("", [0])
+            return Series::new(self.name(), [0])
                 .cast(self.dtype())
                 .unwrap()
                 .sum_as_series();
         }
         match self.dtype() {
             Int8 | UInt8 | Int16 | UInt16 => self.cast(&Int64).unwrap().sum_as_series(),
             _ => self._sum_as_series(),
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 # defines the configuration attribute `docsrs`
 rustdoc-args = ["--cfg", "docsrs"]
 
 [dependencies.arrow]
 package = "arrow2"
 # git = "https://github.com/jorgecarleitao/arrow2"
 git = "https://github.com/ritchie46/arrow2"
-rev = "11933119612e072a6eefaa65abec8c16241073c6"
+rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
 # branch = "polars_2023-04-05"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.17.4/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,21 @@
                     #[cfg(feature = "timezones")]
                     CastTimezone(tz, _use_earliest) => {
                         return mapper.map_datetime_dtype_timezone(tz.as_ref())
                     }
                     #[cfg(feature = "timezones")]
                     TzLocalize(tz) => return mapper.map_datetime_dtype_timezone(Some(tz)),
                     DateRange { .. } => return mapper.map_to_supertype(),
-                    Combine(tu) => DataType::Datetime(*tu, None),
+                    Combine(tu) => match mapper.with_same_dtype().unwrap().dtype {
+                        DataType::Datetime(_, tz) => DataType::Datetime(*tu, tz),
+                        DataType::Date => DataType::Datetime(*tu, None),
+                        dtype => {
+                            polars_bail!(ComputeError: "expected Date or Datetime, got {}", dtype)
+                        }
+                    },
                 };
                 mapper.with_dtype(dtype)
             }
 
             #[cfg(feature = "date_offset")]
             DateOffset(_) => mapper.with_same_dtype(),
             #[cfg(feature = "trigonometry")]
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files 5% similar despite different names*

```diff
@@ -50,13 +50,30 @@
     }
 }
 
 pub(super) fn combine(s: &[Series], tu: TimeUnit) -> PolarsResult<Series> {
     let date = &s[0];
     let time = &s[1];
 
+    let tz = match date.dtype() {
+        DataType::Date => None,
+        DataType::Datetime(_, tz) => tz.as_ref(),
+        _dtype => {
+            polars_bail!(ComputeError: format!("expected Date or Datetime, got {}", _dtype))
+        }
+    };
+
     let date = date.cast(&DataType::Date)?;
     let datetime = date.cast(&DataType::Datetime(tu, None)).unwrap();
 
     let duration = time.cast(&DataType::Duration(tu))?;
-    Ok(datetime + duration)
+    let result_naive = datetime + duration;
+    match tz {
+        #[cfg(feature = "timezones")]
+        Some(tz) => Ok(result_naive
+            .datetime()
+            .unwrap()
+            .replace_time_zone(Some(tz), None)?
+            .into()),
+        _ => Ok(result_naive),
+    }
 }
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1232,14 +1232,15 @@
         |s| StructChunked::new(s[0].name(), s).map(|ca| Some(ca.into_series())),
         exprs,
         GetOutput::map_fields(|fld| Field::new(fld[0].name(), DataType::Struct(fld.to_vec()))),
     )
     .with_function_options(|mut options| {
         options.input_wildcard_expansion = true;
         options.fmt_str = "as_struct";
+        options.pass_name_to_apply = true;
         options
     })
 }
 
 /// Create a column of length `n` containing `n` copies of the literal `value`. Generally you won't need this function,
 /// as `lit(value)` already represents a column containing only `value` whose length is automatically set to the correct
 /// number of rows.
```

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.17.4/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/Cargo.toml` & `polars_lts_cpu-0.17.4/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.3"
+version = "0.17.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.17.3/LICENSE` & `polars_lts_cpu-0.17.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/Makefile` & `polars_lts_cpu-0.17.4/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/README.md` & `polars_lts_cpu-0.17.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,29 +40,31 @@
   <a href="https://stackoverflow.com/questions/tagged/nodejs-polars">Node.js</a>
   |
   <a href="https://pola-rs.github.io/polars-book/">User Guide</a>
   |
   <a href="https://discord.gg/4UfP5cfBE7">Discord</a>
 </p>
 
-## Polars: Blazingly fast DataFrames in Rust, Python & Node.js
+## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL
 
-Polars is a blazingly fast DataFrames library implemented in Rust using
+Polars is a DataFrame interface on top of an OLAP Query Engine implemented in Rust using
 [Apache Arrow Columnar Format](https://arrow.apache.org/docs/format/Columnar.html) as the memory model.
 
 - Lazy | eager execution
 - Multi-threaded
 - SIMD
 - Query optimization
 - Powerful expression API
 - Hybrid Streaming (larger than RAM datasets)
 - Rust | Python | NodeJS | ...
 
 To learn more, read the [User Guide](https://pola-rs.github.io/polars-book/).
 
+## Python
+
 ```python
 >>> import polars as pl
 >>> df = pl.DataFrame(
 ...     {
 ...         "A": [1, 2, 3, 4, 5],
 ...         "fruits": ["banana", "banana", "apple", "apple", "banana"],
 ...         "B": [5, 4, 3, 2, 1],
@@ -92,14 +94,50 @@
 │ "apple"  ┆ "beetle" ┆ "fruits"     ┆ 11  ┆ 4           ┆ 7           ┆ 3           ┆ 3           │
 │ "banana" ┆ "beetle" ┆ "fruits"     ┆ 11  ┆ 4           ┆ 8           ┆ 5           ┆ 5           │
 │ "banana" ┆ "audi"   ┆ "fruits"     ┆ 11  ┆ 2           ┆ 8           ┆ 2           ┆ 2           │
 │ "banana" ┆ "beetle" ┆ "fruits"     ┆ 11  ┆ 4           ┆ 8           ┆ 1           ┆ 1           │
 └──────────┴──────────┴──────────────┴─────┴─────────────┴─────────────┴─────────────┴─────────────┘
 ```
 
+## SQL
+
+```python
+>>> # create a sql context
+>>> context = pl.SQLContext()
+>>> # register a table
+>>> table = pl.scan_ipc("file.arrow")
+>>> context.register("my_table", table)
+>>> # the query we want to run
+>>> query = """
+... SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM my_table
+... WHERE id1 = 'id016'
+... LIMIT 10
+... """
+>>> ## OPTION 1
+>>> # run query to materialization
+>>> context.query(query)
+ shape: (1, 2)
+ ┌────────┬────────┐
+ │ sum_v1 ┆ min_v2 │
+ │ ---    ┆ ---    │
+ │ i64    ┆ i64    │
+ ╞════════╪════════╡
+ │ 298268 ┆ 1      │
+ └────────┴────────┘
+>>> ## OPTION 2
+>>> # Don't materialize the query, but return as LazyFrame
+>>> # and continue in python
+>>> lf = context.execute(query)
+>>> (lf.join(other_table)
+...      .groupby("foo")
+...      .agg(
+...     pl.col("sum_v1").count()
+... ).collect())
+```
+
 ## Performance 🚀🚀
 
 ### Blazingly fast
 
 Polars is very fast. In fact, it is one of the best performing solutions available.
 See the results in [h2oai's db-benchmark](https://h2oai.github.io/db-benchmark/).
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
            Latest_Release] [NPM_Latest_Release] [DOI_Latest_Release]
 Documentation: Python - Rust - Node.js | StackOverflow: Python - Rust - Node.js
                             | User_Guide | Discord
-## Polars: Blazingly fast DataFrames in Rust, Python & Node.js Polars is a
-blazingly fast DataFrames library implemented in Rust using [Apache Arrow
-Columnar Format](https://arrow.apache.org/docs/format/Columnar.html) as the
-memory model. - Lazy | eager execution - Multi-threaded - SIMD - Query
-optimization - Powerful expression API - Hybrid Streaming (larger than RAM
-datasets) - Rust | Python | NodeJS | ... To learn more, read the [User Guide]
-(https://pola-rs.github.io/polars-book/). ```python >>> import polars as pl >>>
-df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ... "fruits": ["banana",
-"banana", "apple", "apple", "banana"], ... "B": [5, 4, 3, 2, 1], ... "cars":
-["beetle", "audi", "beetle", "beetle", "beetle"], ... } ... ) # embarrassingly
-parallel execution & very expressive query language >>> df.sort
-("fruits").select( ... "fruits", ... "cars", ... pl.lit("fruits").alias
+## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL Polars
+is a DataFrame interface on top of an OLAP Query Engine implemented in Rust
+using [Apache Arrow Columnar Format](https://arrow.apache.org/docs/format/
+Columnar.html) as the memory model. - Lazy | eager execution - Multi-threaded -
+SIMD - Query optimization - Powerful expression API - Hybrid Streaming (larger
+than RAM datasets) - Rust | Python | NodeJS | ... To learn more, read the [User
+Guide](https://pola-rs.github.io/polars-book/). ## Python ```python >>> import
+polars as pl >>> df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ...
+"fruits": ["banana", "banana", "apple", "apple", "banana"], ... "B": [5, 4, 3,
+2, 1], ... "cars": ["beetle", "audi", "beetle", "beetle", "beetle"], ... } ...
+) # embarrassingly parallel execution & very expressive query language >>>
+df.sort("fruits").select( ... "fruits", ... "cars", ... pl.lit("fruits").alias
 ("literal_string_fruits"), ... pl.col("B").filter(pl.col("cars") ==
 "beetle").sum(), ... pl.col("A").filter(pl.col("B") > 2).sum().over
 ("cars").alias("sum_A_by_cars"), ... pl.col("A").sum().over("fruits").alias
 ("sum_A_by_fruits"), ... pl.col("A").reverse().over("fruits").alias
 ("rev_A_by_fruits"), ... pl.col("A").sort_by("B").over("fruits").alias
 ("sort_A_by_B_by_fruits"), ... ) shape: (5, 8)
 ââââââââââââ¬âââââââââââ¬âââââââââââââââ¬ââââââ¬ââââââââââââââ¬ââââââââââââââ¬ââââââââââââââ¬ââââââââââââââ
@@ -32,17 +32,30 @@
 ââââââââââââªâââââââââââªâââââââââââââââªââââââªââââââââââââââªââââââââââââââªââââââââââââââªââââââââââââââ¡
 â "apple" â "beetle" â "fruits" â 11 â 4 â 7 â 4 â 4 â â
 "apple" â "beetle" â "fruits" â 11 â 4 â 7 â 3 â 3 â â
 "banana" â "beetle" â "fruits" â 11 â 4 â 8 â 5 â 5 â â
 "banana" â "audi" â "fruits" â 11 â 2 â 8 â 2 â 2 â â
 "banana" â "beetle" â "fruits" â 11 â 4 â 8 â 1 â 1 â
 ââââââââââââ´âââââââââââ´âââââââââââââââ´ââââââ´ââââââââââââââ´ââââââââââââââ´ââââââââââââââ´ââââââââââââââ
-``` ## Performance ðð ### Blazingly fast Polars is very fast. In fact, it
-is one of the best performing solutions available. See the results in [h2oai's
-db-benchmark](https://h2oai.github.io/db-benchmark/). In the [TPCH benchmarks]
+``` ## SQL ```python >>> # create a sql context >>> context = pl.SQLContext()
+>>> # register a table >>> table = pl.scan_ipc("file.arrow") >>>
+context.register("my_table", table) >>> # the query we want to run >>> query =
+""" ... SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM my_table ... WHERE id1
+= 'id016' ... LIMIT 10 ... """ >>> ## OPTION 1 >>> # run query to
+materialization >>> context.query(query) shape: (1, 2)
+ââââââââââ¬âââââââââ â sum_v1 â min_v2
+â â --- â --- â â i64 â i64 â
+ââââââââââªâââââââââ¡ â 298268 â 1 â
+ââââââââââ´âââââââââ >>> ## OPTION 2 >>> #
+Don't materialize the query, but return as LazyFrame >>> # and continue in
+python >>> lf = context.execute(query) >>> (lf.join(other_table) ... .groupby
+("foo") ... .agg( ... pl.col("sum_v1").count() ... ).collect()) ``` ##
+Performance ðð ### Blazingly fast Polars is very fast. In fact, it is one
+of the best performing solutions available. See the results in [h2oai's db-
+benchmark](https://h2oai.github.io/db-benchmark/). In the [TPCH benchmarks]
 (https://www.pola.rs/benchmarks.html) polars is orders of magnitudes faster
 than pandas, dask, modin and vaex on full queries (including IO). ###
 Lightweight Polars is also very lightweight. It comes with zero required
 dependencies, and this shows in the import times: - polars: 70ms - numpy: 104ms
 - pandas: 520ms ### Handles larger than RAM data If you have data that does not
 fit into memory, polars lazy is able to process your query (or parts of your
 query) in a streaming fashion, this drastically reduces memory requirements so
```

### Comparing `polars_lts_cpu-0.17.3/build.rs` & `polars_lts_cpu-0.17.4/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/Makefile` & `polars_lts_cpu-0.17.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.17.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.17.4/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/conf.py` & `polars_lts_cpu-0.17.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/api.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/config.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/functions.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/io.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/docs/source/reference/testing.rst` & `polars_lts_cpu-0.17.4/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/__init__.py` & `polars_lts_cpu-0.17.4/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/api.py` & `polars_lts_cpu-0.17.4/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/config.py` & `polars_lts_cpu-0.17.4/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/convert.py` & `polars_lts_cpu-0.17.4/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/dataframe/_html.py` & `polars_lts_cpu-0.17.4/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/dataframe/frame.py` & `polars_lts_cpu-0.17.4/polars/dataframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -3540,23 +3540,26 @@
         $ e  <str> usd, eur, None
         $ f <date> 2020-01-01, 2021-01-02, 2022-01-01
 
         """
         # always print at most this number of values, mainly used to ensure
         # we do not cast long arrays to strings which would be very slow
         max_num_values = min(10, self.height)
+        max_col_name_trunc = 50
 
         def _parse_column(col_name: str, dtype: PolarsDataType) -> tuple[str, str, str]:
             dtype_str = (
                 f"<{DataTypeClass._string_repr(dtype)}>"
                 if isinstance(dtype, DataTypeClass)
                 else f"<{dtype._string_repr()}>"
             )
             val = self[:max_num_values][col_name].to_list()
             val_str = ", ".join(map(str, val))
+            if len(col_name) > max_col_name_trunc:
+                col_name = col_name[: (max_col_name_trunc - 3)] + "..."
             return col_name, dtype_str, val_str
 
         data = [_parse_column(s, dtype) for s, dtype in self.schema.items()]
 
         # we make the first column as small as possible by taking the longest
         # column name
         max_col_name = max((len(col_name) for col_name, _, _ in data))
```

### Comparing `polars_lts_cpu-0.17.3/polars/dataframe/groupby.py` & `polars_lts_cpu-0.17.4/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/datatypes/__init__.py` & `polars_lts_cpu-0.17.4/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/datatypes/classes.py` & `polars_lts_cpu-0.17.4/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/datatypes/constants.py` & `polars_lts_cpu-0.17.4/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/datatypes/constructor.py` & `polars_lts_cpu-0.17.4/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/datatypes/convert.py` & `polars_lts_cpu-0.17.4/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/dependencies.py` & `polars_lts_cpu-0.17.4/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/exceptions.py` & `polars_lts_cpu-0.17.4/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/binary.py` & `polars_lts_cpu-0.17.4/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/categorical.py` & `polars_lts_cpu-0.17.4/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/datetime.py` & `polars_lts_cpu-0.17.4/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/expr.py` & `polars_lts_cpu-0.17.4/polars/expr/expr.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/list.py` & `polars_lts_cpu-0.17.4/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/meta.py` & `polars_lts_cpu-0.17.4/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/string.py` & `polars_lts_cpu-0.17.4/polars/expr/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/expr/struct.py` & `polars_lts_cpu-0.17.4/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/functions/__init__.py` & `polars_lts_cpu-0.17.4/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/functions/eager.py` & `polars_lts_cpu-0.17.4/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/functions/lazy.py` & `polars_lts_cpu-0.17.4/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/functions/whenthen.py` & `polars_lts_cpu-0.17.4/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/__init__.py` & `polars_lts_cpu-0.17.4/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/_utils.py` & `polars_lts_cpu-0.17.4/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/avro.py` & `polars_lts_cpu-0.17.4/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/csv/_utils.py` & `polars_lts_cpu-0.17.4/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.17.4/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/csv/functions.py` & `polars_lts_cpu-0.17.4/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/database.py` & `polars_lts_cpu-0.17.4/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/delta.py` & `polars_lts_cpu-0.17.4/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.17.4/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/excel/functions.py` & `polars_lts_cpu-0.17.4/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.17.4/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/ipc/functions.py` & `polars_lts_cpu-0.17.4/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/json.py` & `polars_lts_cpu-0.17.4/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/ndjson.py` & `polars_lts_cpu-0.17.4/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.17.4/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/parquet/functions.py` & `polars_lts_cpu-0.17.4/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.17.4/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.17.4/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/lazyframe/frame.py` & `polars_lts_cpu-0.17.4/polars/lazyframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.17.4/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/_numpy.py` & `polars_lts_cpu-0.17.4/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/binary.py` & `polars_lts_cpu-0.17.4/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/categorical.py` & `polars_lts_cpu-0.17.4/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/datetime.py` & `polars_lts_cpu-0.17.4/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/list.py` & `polars_lts_cpu-0.17.4/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/series.py` & `polars_lts_cpu-0.17.4/polars/series/series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/string.py` & `polars_lts_cpu-0.17.4/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/struct.py` & `polars_lts_cpu-0.17.4/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/series/utils.py` & `polars_lts_cpu-0.17.4/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/slice.py` & `polars_lts_cpu-0.17.4/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/sql/context.py` & `polars_lts_cpu-0.17.4/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/string_cache.py` & `polars_lts_cpu-0.17.4/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/testing/_private.py` & `polars_lts_cpu-0.17.4/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/testing/_tempdir.py` & `polars_lts_cpu-0.17.4/polars/testing/_tempdir.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/testing/asserts.py` & `polars_lts_cpu-0.17.4/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/testing/parametric/__init__.py` & `polars_lts_cpu-0.17.4/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/testing/parametric/primitives.py` & `polars_lts_cpu-0.17.4/polars/testing/parametric/primitives.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/testing/parametric/strategies.py` & `polars_lts_cpu-0.17.4/polars/testing/parametric/strategies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
-from string import ascii_letters, digits, punctuation
+from string import ascii_letters, ascii_uppercase, digits, punctuation
 from typing import TYPE_CHECKING, Any
 
 from hypothesis.strategies import (
     booleans,
+    characters,
     dates,
     datetimes,
     floats,
     from_type,
     integers,
     text,
     timedeltas,
@@ -58,19 +59,20 @@
 strategy_i32 = integers(min_value=-(2**31), max_value=(2**31) - 1)
 strategy_i64 = integers(min_value=-(2**63), max_value=(2**63) - 1)
 strategy_u8 = integers(min_value=0, max_value=(2**8) - 1)
 strategy_u16 = integers(min_value=0, max_value=(2**16) - 1)
 strategy_u32 = integers(min_value=0, max_value=(2**32) - 1)
 strategy_u64 = integers(min_value=0, max_value=(2**64) - 1)
 
-# TODO: when generating text for categorical, ensure
-#  there are repeats; don't want all to be unique.
-strategy_ascii = text(max_size=10, alphabet=ascii_letters + digits + punctuation + " ")
-strategy_utf8 = text(max_size=10)
-strategy_cat = text(max_size=10)
+strategy_ascii = text(max_size=8, alphabet=ascii_letters + digits + punctuation)
+strategy_categorical = text(max_size=2, alphabet=ascii_uppercase)
+strategy_utf8 = text(
+    max_size=8,
+    alphabet=characters(max_codepoint=1000, blacklist_categories=("Cs", "Cc")),
+)
 
 # TODO: confirm datetime min/max limits with different timeunit
 #  granularity. support datetime/duration time_units (ms, us, ns).
 strategy_datetime = datetimes(min_value=datetime(1970, 1, 1))
 strategy_time = times()
 strategy_date = dates()
 strategy_duration = timedeltas(
@@ -86,14 +88,14 @@
     Int16: strategy_i16,
     Int32: strategy_i32,
     Int64: strategy_i64,
     UInt8: strategy_u8,
     UInt16: strategy_u16,
     UInt32: strategy_u32,
     UInt64: strategy_u64,
-    Categorical: strategy_cat,
+    Categorical: strategy_categorical,
     Utf8: strategy_utf8,
     Time: strategy_time,
     Date: strategy_date,
     Duration: strategy_duration,
     Datetime: strategy_datetime,
 }
```

### Comparing `polars_lts_cpu-0.17.3/polars/type_aliases.py` & `polars_lts_cpu-0.17.4/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/__init__.py` & `polars_lts_cpu-0.17.4/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/_construction.py` & `polars_lts_cpu-0.17.4/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.17.4/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/_scan.py` & `polars_lts_cpu-0.17.4/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/_wrap.py` & `polars_lts_cpu-0.17.4/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/build_info.py` & `polars_lts_cpu-0.17.4/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/convert.py` & `polars_lts_cpu-0.17.4/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/decorators.py` & `polars_lts_cpu-0.17.4/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/meta.py` & `polars_lts_cpu-0.17.4/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/polars_version.py` & `polars_lts_cpu-0.17.4/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/show_versions.py` & `polars_lts_cpu-0.17.4/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/polars/utils/various.py` & `polars_lts_cpu-0.17.4/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/pyproject.toml` & `polars_lts_cpu-0.17.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/requirements-dev.txt` & `polars_lts_cpu-0.17.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/scripts/check_stacklevels.py` & `polars_lts_cpu-0.17.4/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/apply/dataframe.rs` & `polars_lts_cpu-0.17.4/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/apply/mod.rs` & `polars_lts_cpu-0.17.4/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/apply/series.rs` & `polars_lts_cpu-0.17.4/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.17.4/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.17.4/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/batched_csv.rs` & `polars_lts_cpu-0.17.4/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/conversion.rs` & `polars_lts_cpu-0.17.4/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/dataframe.rs` & `polars_lts_cpu-0.17.4/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/datatypes.rs` & `polars_lts_cpu-0.17.4/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/error.rs` & `polars_lts_cpu-0.17.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/file.rs` & `polars_lts_cpu-0.17.4/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/lazy/apply.rs` & `polars_lts_cpu-0.17.4/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/lazy/dataframe.rs` & `polars_lts_cpu-0.17.4/src/lazy/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/lazy/dsl.rs` & `polars_lts_cpu-0.17.4/src/lazy/dsl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/lazy/meta.rs` & `polars_lts_cpu-0.17.4/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/lazy/mod.rs` & `polars_lts_cpu-0.17.4/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/lib.rs` & `polars_lts_cpu-0.17.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/npy.rs` & `polars_lts_cpu-0.17.4/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/object.rs` & `polars_lts_cpu-0.17.4/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/series.rs` & `polars_lts_cpu-0.17.4/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/set.rs` & `polars_lts_cpu-0.17.4/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/sql.rs` & `polars_lts_cpu-0.17.4/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/src/utils.rs` & `polars_lts_cpu-0.17.4/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/README.md` & `polars_lts_cpu-0.17.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.17.4/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.17.4/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/benchmark/test_release.py` & `polars_lts_cpu-0.17.4/tests/benchmark/test_release.py`

 * *Files 16% similar despite different names*

```diff
@@ -158,7 +158,30 @@
     # int64 is important to hit the page size
     df = pl.arange(0, n, eager=True, dtype=pl.Int64).to_frame()
     f = "/tmp/tmp.parquet"
     df.write_parquet(f, statistics=True, use_pyarrow=False, row_group_size=n)
     result = pl.scan_parquet(f).filter(pl.col("arange") > n - 3).collect()
     expected = pl.DataFrame({"arange": [149998, 149999]})
     assert_frame_equal(result, expected)
+
+
+def test_boolean_min_max_agg() -> None:
+    np.random.seed(0)
+    idx = np.random.randint(0, 500, 1000)
+    c = np.random.randint(0, 500, 1000) > 250
+
+    df = pl.DataFrame({"idx": idx, "c": c})
+    aggs = [pl.col("c").min().alias("c_min"), pl.col("c").max().alias("c_max")]
+    assert df.groupby("idx").agg(aggs).sum().to_dict(False) == {
+        "idx": [107583],
+        "c_min": [120],
+        "c_max": [321],
+    }
+
+    nulls = np.random.randint(0, 500, 1000) < 100
+    assert df.with_columns(
+        c=pl.when(pl.lit(nulls)).then(None).otherwise(pl.col("c"))
+    ).groupby("idx").agg(aggs).sum().to_dict(False) == {
+        "idx": [107583],
+        "c_min": [133],
+        "c_max": [276],
+    }
```

### Comparing `polars_lts_cpu-0.17.3/tests/docs/run_doctest.py` & `polars_lts_cpu-0.17.4/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.17.4/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.17.4/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/parametric/test_series.py` & `polars_lts_cpu-0.17.4/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/parametric/test_testing.py` & `polars_lts_cpu-0.17.4/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/conftest.py` & `polars_lts_cpu-0.17.4/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,7 +339,15 @@
         pl.col("letter")
     ).to_dict(
         False
     ) == {
         "c_group": [2, 3],
         "letter": [[["a", "b"], ["f", "g"]], [["c", "d", "e"]]],
     }
+
+
+def test_nested_categorical_cast() -> None:
+    values = [["x"], ["y"], ["x"]]
+    dtype = pl.List(pl.Categorical)
+    s = pl.Series(values).cast(dtype)
+    assert s.dtype == dtype
+    assert s.to_list() == values
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -917,7 +917,53 @@
 def test_struct_list_cat_8235() -> None:
     df = pl.DataFrame(
         {"values": [["a", "b", "c"]]}, schema={"values": pl.List(pl.Categorical)}
     )
     assert df.select(pl.struct("values")).to_dict(False) == {
         "values": [{"values": ["a", "b", "c"]}]
     }
+
+
+def test_struct_name_passed_in_agg_apply() -> None:
+    struct_expr = pl.struct(
+        [
+            pl.col("A").min(),
+            pl.col("B").search_sorted(pl.Series([3, 4])),
+        ]
+    ).alias("index")
+
+    assert pl.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6], "C": [1, 2, 2]}).groupby(
+        "C"
+    ).agg(struct_expr).sort("C", descending=True).to_dict(False) == {
+        "C": [2, 1],
+        "index": [
+            [{"A": 2, "B": 0}, {"A": 2, "B": 0}],
+            [{"A": 1, "B": 0}, {"A": 1, "B": 0}],
+        ],
+    }
+
+    df = pl.DataFrame({"val": [-3, -2, -1, 0, 1, 2, 3], "k": [0] * 7})
+
+    assert df.groupby("k").agg(
+        pl.struct(
+            [
+                pl.col("val").value_counts(sort=True).struct.field("val").alias("val"),
+                pl.col("val")
+                .value_counts(sort=True)
+                .struct.field("counts")
+                .alias("counts"),
+            ]
+        )
+    ).to_dict(False) == {
+        "k": [0],
+        "val": [
+            [
+                {"val": -3, "counts": 1},
+                {"val": -2, "counts": 1},
+                {"val": -1, "counts": 1},
+                {"val": 0, "counts": 1},
+                {"val": 1, "counts": 1},
+                {"val": 2, "counts": 1},
+                {"val": 3, "counts": 1},
+            ]
+        ],
+    }
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.17.4/tests/unit/datatypes/test_temporal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.17.4/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.17.4/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.17.4/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.17.4/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.17.4/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_database.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_json.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_other.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.17.4/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 import polars as pl
 from polars.datatypes import DTYPE_TEMPORAL_UNITS
 from polars.exceptions import ComputeError
 from polars.testing import assert_series_equal
 
 if TYPE_CHECKING:
     from polars.type_aliases import TimeUnit
+import sys
+
+from polars.dependencies import _ZONEINFO_AVAILABLE
+
+if sys.version_info >= (3, 9):
+    from zoneinfo import ZoneInfo
+elif _ZONEINFO_AVAILABLE:
+    # Import from submodule due to typing issue with backports.zoneinfo package:
+    # https://github.com/pganssle/zoneinfo/issues/125
+    from backports.zoneinfo._zoneinfo import ZoneInfo
 
 
 @pytest.fixture()
 def series_of_int_dates() -> pl.Series:
     return pl.Series([10000, 20000, 30000], dtype=pl.Date)
 
 
@@ -262,21 +272,27 @@
     assert_series_equal(dates.dt.epoch("s"), dates.dt.timestamp("ms") // 1000)
     assert_series_equal(
         dates.dt.epoch("d"),
         (dates.dt.timestamp("ms") // (1000 * 3600 * 24)).cast(pl.Int32),
     )
 
 
-def test_date_time_combine() -> None:
+@pytest.mark.parametrize(
+    ("tzinfo", "expected_time_zone"),
+    [(None, None), (ZoneInfo("Asia/Kathmandu"), "Asia/Kathmandu")],
+)
+def test_date_time_combine(
+    tzinfo: ZoneInfo | None, expected_time_zone: str | None
+) -> None:
     # Define a DataFrame with columns for datetime, date, and time
     df = pl.DataFrame(
         {
             "dtm": [
-                datetime(2022, 12, 31, 10, 30, 45),
-                datetime(2023, 7, 5, 23, 59, 59),
+                datetime(2022, 12, 31, 10, 30, 45, tzinfo=tzinfo),
+                datetime(2023, 7, 5, 23, 59, 59, tzinfo=tzinfo),
             ],
             "dt": [
                 date(2022, 10, 10),
                 date(2022, 7, 5),
             ],
             "tm": [
                 time(1, 2, 3, 456000),
@@ -293,36 +309,76 @@
             pl.col("dt").dt.combine(time(4, 5, 6)).alias("d3"),  # date & specified time
         ]
     )
 
     # Assert that the new columns have the expected values and datatypes
     expected_dict = {
         "d1": [  # Time component should be overwritten by `tm` values
-            datetime(2022, 12, 31, 1, 2, 3, 456000),
-            datetime(2023, 7, 5, 7, 8, 9, 101000),
+            datetime(2022, 12, 31, 1, 2, 3, 456000, tzinfo=tzinfo),
+            datetime(2023, 7, 5, 7, 8, 9, 101000, tzinfo=tzinfo),
         ],
         "d2": [  # Both date and time components combined "as-is" into new datetime
             datetime(2022, 10, 10, 1, 2, 3, 456000),
             datetime(2022, 7, 5, 7, 8, 9, 101000),
         ],
         "d3": [  # New datetime should use specified time component
             datetime(2022, 10, 10, 4, 5, 6),
             datetime(2022, 7, 5, 4, 5, 6),
         ],
     }
     assert df.to_dict(False) == expected_dict
 
     expected_schema = {
-        "d1": pl.Datetime("us"),
+        "d1": pl.Datetime("us", expected_time_zone),
         "d2": pl.Datetime("us"),
         "d3": pl.Datetime("us"),
     }
     assert df.schema == expected_schema
 
 
+def test_combine_unsupported_types() -> None:
+    with pytest.raises(ComputeError, match="expected Date or Datetime, got time"):
+        pl.Series([time(1, 2)]).dt.combine(time(3, 4))
+
+
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+@pytest.mark.parametrize(
+    ("tzinfo", "expected_time_zone"),
+    [
+        (ZoneInfo("Asia/Kathmandu"), "Asia/Kathmandu"),
+        (None, None),
+    ],
+)
+def test_combine_lazy_schema_datetime(
+    tzinfo: ZoneInfo | None,
+    expected_time_zone: str | None,
+    time_unit: TimeUnit,
+) -> None:
+    df = pl.DataFrame({"ts": pl.Series([datetime(2020, 1, 1, tzinfo=tzinfo)])})
+    result = (
+        df.lazy()
+        .select(pl.col("ts").dt.combine(time(1, 2, 3), time_unit=time_unit))
+        .dtypes
+    )
+    expected = [pl.Datetime(time_unit, expected_time_zone)]
+    assert result == expected
+
+
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+def test_combine_lazy_schema_date(time_unit: TimeUnit) -> None:
+    df = pl.DataFrame({"ts": pl.Series([date(2020, 1, 1)])})
+    result = (
+        df.lazy()
+        .select(pl.col("ts").dt.combine(time(1, 2, 3), time_unit=time_unit))
+        .dtypes
+    )
+    expected = [pl.Datetime(time_unit, None)]
+    assert result == expected
+
+
 def test_is_leap_year() -> None:
     assert pl.date_range(
         datetime(1990, 1, 1), datetime(2004, 1, 1), "1y"
     ).dt.is_leap_year().to_list() == [
         False,
         False,
         True,  # 1992
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.17.4/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_join.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,7 +527,26 @@
 
     ldf = ldf.join(ldf2, on=["id", "value"])
     ldf = pl.concat([ldf, ldf2])
     result = ldf.select("id")
 
     expected = pl.DataFrame({"id": [1, 1, 3]}).lazy()
     assert_frame_equal(result, expected)
+
+
+def test_join_sorted_fast_paths_null() -> None:
+    df1 = pl.DataFrame({"x": [0, 1, 0]}).sort("x")
+    df2 = pl.DataFrame({"x": [0, None], "y": [0, 1]})
+    assert df1.join(df2, on="x", how="inner").to_dict(False) == {
+        "x": [0, 0],
+        "y": [0, 0],
+    }
+    assert df1.join(df2, on="x", how="left").to_dict(False) == {
+        "x": [0, 0, 1],
+        "y": [0, 0, None],
+    }
+    assert df1.join(df2, on="x", how="anti").to_dict(False) == {"x": [1]}
+    assert df1.join(df2, on="x", how="semi").to_dict(False) == {"x": [0, 0]}
+    assert df1.join(df2, on="x", how="outer").to_dict(False) == {
+        "x": [0, 0, 1, None],
+        "y": [0, 0, None, 1],
+    }
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,7 +642,23 @@
         3,
         4,
         6,
         1,
         8,
         9,
     ]
+
+
+def test_sort_top_k_fast_path() -> None:
+    df = pl.DataFrame(
+        {
+            "a": [1, 2, None],
+            "b": [6.0, 5.0, 4.0],
+            "c": ["a", "c", "b"],
+        }
+    )
+    # this triggers fast path as head is equal to n-rows
+    assert df.lazy().sort("b").head(3).collect().to_dict(False) == {
+        "a": [None, 2, 1],
+        "b": [4.0, 5.0, 6.0],
+        "c": ["b", "c", "a"],
+    }
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.17.4/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_api.py` & `polars_lts_cpu-0.17.4/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_arity.py` & `polars_lts_cpu-0.17.4/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_cfg.py` & `polars_lts_cpu-0.17.4/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_constructors.py` & `polars_lts_cpu-0.17.4/tests/unit/test_constructors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1163,11 +1163,42 @@
 
 
 def test_list_null_constructor() -> None:
     s = pl.Series("a", [[None], [None]], dtype=pl.List(pl.Null))
     assert s.dtype == pl.List(pl.Null)
     assert s.to_list() == [None, None]
 
+    # nested
+    dtype = pl.List(pl.List(pl.Int8))
+    values = [
+        [],
+        [[], []],
+        [[33, 112]],
+    ]
+    s = pl.Series(
+        name="colx",
+        values=values,
+        dtype=dtype,
+    )
+    assert s.dtype == dtype
+    assert s.to_list() == values
+
+    # nested
+    # small order change has influence
+    dtype = pl.List(pl.List(pl.Int8))
+    values = [
+        [[], []],
+        [],
+        [[33, 112]],
+    ]
+    s = pl.Series(
+        name="colx",
+        values=values,
+        dtype=dtype,
+    )
+    assert s.dtype == dtype
+    assert s.to_list() == values
+
 
 def test_numpy_float_construction_av() -> None:
     np_dict = {"a": np.float64(1)}
     assert_frame_equal(pl.DataFrame(np_dict), pl.DataFrame({"a": 1.0}))
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_cse.py` & `polars_lts_cpu-0.17.4/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.17.4/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_df.py` & `polars_lts_cpu-0.17.4/tests/unit/test_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -3403,14 +3403,26 @@
     assert result == expected
 
     # the default is to print to the console
     df.glimpse(return_as_string=False)
     # remove the last newline on the capsys
     assert capsys.readouterr().out[:-1] == expected
 
+    colc = "a" * 96
+    df = pl.DataFrame({colc: [11, 22, 33]})
+    result = df.glimpse(return_as_string=True)
+    expected = textwrap.dedent(
+        """\
+        Rows: 3
+        Columns: 1
+        $ aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa... <i64> 11, 22, 33
+        """
+    )
+    assert result == expected
+
 
 def test_item() -> None:
     df = pl.DataFrame({"a": [1]})
     assert df.item() == 1
 
     df = pl.DataFrame({"a": [1, 2]})
     with pytest.raises(ValueError):
@@ -3778,7 +3790,15 @@
     df = df.select(
         [
             pl.col("*"),  # select all
             pl.col("random").sum().over("groups").alias("sum[random]/groups"),
             pl.col("random").implode().over("names").alias("random/name"),
         ]
     )
+
+
+def test_sum_empty_column_names() -> None:
+    df = pl.DataFrame({"x": [], "y": []}, schema={"x": pl.Boolean, "y": pl.Boolean})
+    expected = pl.DataFrame(
+        {"x": [0], "y": [0]}, schema={"x": pl.UInt32, "y": pl.UInt32}
+    )
+    assert_frame_equal(df.sum(), expected)
```

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_empty.py` & `polars_lts_cpu-0.17.4/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_errors.py` & `polars_lts_cpu-0.17.4/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.17.4/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_exprs.py` & `polars_lts_cpu-0.17.4/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_fmt.py` & `polars_lts_cpu-0.17.4/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_functions.py` & `polars_lts_cpu-0.17.4/tests/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_interchange.py` & `polars_lts_cpu-0.17.4/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_interop.py` & `polars_lts_cpu-0.17.4/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_lazy.py` & `polars_lts_cpu-0.17.4/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.17.4/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_predicates.py` & `polars_lts_cpu-0.17.4/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_projections.py` & `polars_lts_cpu-0.17.4/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_queries.py` & `polars_lts_cpu-0.17.4/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_rows.py` & `polars_lts_cpu-0.17.4/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_schema.py` & `polars_lts_cpu-0.17.4/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_serde.py` & `polars_lts_cpu-0.17.4/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_series.py` & `polars_lts_cpu-0.17.4/tests/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_sql.py` & `polars_lts_cpu-0.17.4/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_streaming.py` & `polars_lts_cpu-0.17.4/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/test_testing.py` & `polars_lts_cpu-0.17.4/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.17.4/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.3/Cargo.lock` & `polars_lts_cpu-0.17.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
 version = "0.17.0"
-source = "git+https://github.com/ritchie46/arrow2?rev=11933119612e072a6eefaa65abec8c16241073c6#11933119612e072a6eefaa65abec8c16241073c6"
+source = "git+https://github.com/ritchie46/arrow2?rev=1491c6e8f4fd100f53c358e4f3ef1536d9e75090#1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 dependencies = [
  "ahash",
  "arrow-format",
  "avro-schema",
  "base64",
  "bytemuck",
  "chrono",
@@ -1385,16 +1385,17 @@
 dependencies = [
  "async-trait",
  "futures",
 ]
 
 [[package]]
 name = "parquet2"
-version = "0.17.0"
-source = "git+https://github.com/jorgecarleitao/parquet2?rev=9eee7eb1130aed4cd0d841e59c325cc366fc3798#9eee7eb1130aed4cd0d841e59c325cc366fc3798"
+version = "0.17.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "579fe5745f02cef3d5f236bfed216fd4693e49e4e920a13475c6132233283bce"
 dependencies = [
  "async-stream",
  "brotli",
  "flate2",
  "futures",
  "lz4",
  "parquet-format-safe",
@@ -1743,15 +1744,15 @@
 checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.3"
+version = "0.17.4"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_lts_cpu-0.17.3/PKG-INFO` & `polars_lts_cpu-0.17.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.17.3
+Version: 0.17.4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,51 +13,51 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
-Requires-Dist: fsspec; extra == 'fsspec'
 Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
+Requires-Dist: matplotlib; extra == 'matplotlib'
+Requires-Dist: fsspec; extra == 'fsspec'
 Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
 Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
+Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
 Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
 Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
-Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
-Requires-Dist: matplotlib; extra == 'matplotlib'
-Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
-Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: connectorx; extra == 'connectorx'
-Provides-Extra: pyarrow
-Provides-Extra: fsspec
+Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
+Requires-Dist: pandas; extra == 'pandas'
 Provides-Extra: xlsx2csv
+Provides-Extra: matplotlib
+Provides-Extra: fsspec
 Provides-Extra: numpy
-Provides-Extra: deltalake
-Provides-Extra: timezone
+Provides-Extra: connectorx
 Provides-Extra: xlsxwriter
-Provides-Extra: matplotlib
+Provides-Extra: deltalake
 Provides-Extra: all
-Provides-Extra: pandas
+Provides-Extra: pyarrow
+Provides-Extra: timezone
 Provides-Extra: sqlalchemy
-Provides-Extra: connectorx
+Provides-Extra: pandas
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Homepage, https://www.pola.rs/
-Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
+Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
 
 <div align="center">
@@ -97,29 +97,31 @@
   <a href="https://stackoverflow.com/questions/tagged/nodejs-polars">Node.js</a>
   |
   <a href="https://pola-rs.github.io/polars-book/">User Guide</a>
   |
   <a href="https://discord.gg/4UfP5cfBE7">Discord</a>
 </p>
 
-## Polars: Blazingly fast DataFrames in Rust, Python & Node.js
+## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL
 
-Polars is a blazingly fast DataFrames library implemented in Rust using
+Polars is a DataFrame interface on top of an OLAP Query Engine implemented in Rust using
 [Apache Arrow Columnar Format](https://arrow.apache.org/docs/format/Columnar.html) as the memory model.
 
 - Lazy | eager execution
 - Multi-threaded
 - SIMD
 - Query optimization
 - Powerful expression API
 - Hybrid Streaming (larger than RAM datasets)
 - Rust | Python | NodeJS | ...
 
 To learn more, read the [User Guide](https://pola-rs.github.io/polars-book/).
 
+## Python
+
 ```python
 >>> import polars as pl
 >>> df = pl.DataFrame(
 ...     {
 ...         "A": [1, 2, 3, 4, 5],
 ...         "fruits": ["banana", "banana", "apple", "apple", "banana"],
 ...         "B": [5, 4, 3, 2, 1],
@@ -149,14 +151,50 @@
 │ "apple"  ┆ "beetle" ┆ "fruits"     ┆ 11  ┆ 4           ┆ 7           ┆ 3           ┆ 3           │
 │ "banana" ┆ "beetle" ┆ "fruits"     ┆ 11  ┆ 4           ┆ 8           ┆ 5           ┆ 5           │
 │ "banana" ┆ "audi"   ┆ "fruits"     ┆ 11  ┆ 2           ┆ 8           ┆ 2           ┆ 2           │
 │ "banana" ┆ "beetle" ┆ "fruits"     ┆ 11  ┆ 4           ┆ 8           ┆ 1           ┆ 1           │
 └──────────┴──────────┴──────────────┴─────┴─────────────┴─────────────┴─────────────┴─────────────┘
 ```
 
+## SQL
+
+```python
+>>> # create a sql context
+>>> context = pl.SQLContext()
+>>> # register a table
+>>> table = pl.scan_ipc("file.arrow")
+>>> context.register("my_table", table)
+>>> # the query we want to run
+>>> query = """
+... SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM my_table
+... WHERE id1 = 'id016'
+... LIMIT 10
+... """
+>>> ## OPTION 1
+>>> # run query to materialization
+>>> context.query(query)
+ shape: (1, 2)
+ ┌────────┬────────┐
+ │ sum_v1 ┆ min_v2 │
+ │ ---    ┆ ---    │
+ │ i64    ┆ i64    │
+ ╞════════╪════════╡
+ │ 298268 ┆ 1      │
+ └────────┴────────┘
+>>> ## OPTION 2
+>>> # Don't materialize the query, but return as LazyFrame
+>>> # and continue in python
+>>> lf = context.execute(query)
+>>> (lf.join(other_table)
+...      .groupby("foo")
+...      .agg(
+...     pl.col("sum_v1").count()
+... ).collect())
+```
+
 ## Performance 🚀🚀
 
 ### Blazingly fast
 
 Polars is very fast. In fact, it is one of the best performing solutions available.
 See the results in [h2oai's db-benchmark](https://h2oai.github.io/db-benchmark/).
```

#### html2text {}

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.3 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.4 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
-python_version < '3.11' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
-Requires-Dist: fsspec; extra == 'fsspec' Requires-Dist: xlsx2csv >= 0.8.0;
-extra == 'xlsx2csv' Requires-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-
-Dist: deltalake >= 0.8.0; extra == 'deltalake' Requires-Dist:
+python_version < '3.11' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
+Requires-Dist: matplotlib; extra == 'matplotlib' Requires-Dist: fsspec; extra
+== 'fsspec' Requires-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist:
+connectorx; extra == 'connectorx' Requires-Dist: xlsxwriter; extra ==
+'xlsxwriter' Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake' Requires-
+Dist: polars
+[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
+extra == 'all' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist:
 backports.zoneinfo; (python_version < '3.9') and extra == 'timezone' Requires-
 Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone' Requires-
-Dist: xlsxwriter; extra == 'xlsxwriter' Requires-Dist: matplotlib; extra ==
-'matplotlib' Requires-Dist: polars
-[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
-extra == 'all' Requires-Dist: pyarrow>=7.0.0; extra == 'pandas' Requires-Dist:
-pandas; extra == 'pandas' Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
-Requires-Dist: pandas; extra == 'sqlalchemy' Requires-Dist: connectorx; extra
-== 'connectorx' Provides-Extra: pyarrow Provides-Extra: fsspec Provides-Extra:
-xlsx2csv Provides-Extra: numpy Provides-Extra: deltalake Provides-Extra:
-timezone Provides-Extra: xlsxwriter Provides-Extra: matplotlib Provides-Extra:
-all Provides-Extra: pandas Provides-Extra: sqlalchemy Provides-Extra:
-connectorx License-File: LICENSE Summary: Blazingly fast DataFrame library
-Keywords: dataframe,arrow,out-of-core Author-email: Ritchie Vink
+Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra ==
+'sqlalchemy' Requires-Dist: pyarrow>=7.0.0; extra == 'pandas' Requires-Dist:
+pandas; extra == 'pandas' Provides-Extra: xlsx2csv Provides-Extra: matplotlib
+Provides-Extra: fsspec Provides-Extra: numpy Provides-Extra: connectorx
+Provides-Extra: xlsxwriter Provides-Extra: deltalake Provides-Extra: all
+Provides-Extra: pyarrow Provides-Extra: timezone Provides-Extra: sqlalchemy
+Provides-Extra: pandas License-File: LICENSE Summary: Blazingly fast DataFrame
+library Keywords: dataframe,arrow,out-of-core Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/pola-rs/
-polars Project-URL: Homepage, https://www.pola.rs/ Project-URL: Changelog,
-https://github.com/pola-rs/polars/releases Project-URL: Documentation, https://
-pola-rs.github.io/polars/py-polars/html/reference/index.html
+polars Project-URL: Homepage, https://www.pola.rs/ Project-URL: Documentation,
+https://pola-rs.github.io/polars/py-polars/html/reference/index.html Project-
+URL: Changelog, https://github.com/pola-rs/polars/releases
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
            Latest_Release] [NPM_Latest_Release] [DOI_Latest_Release]
 Documentation: Python - Rust - Node.js | StackOverflow: Python - Rust - Node.js
                             | User_Guide | Discord
-## Polars: Blazingly fast DataFrames in Rust, Python & Node.js Polars is a
-blazingly fast DataFrames library implemented in Rust using [Apache Arrow
-Columnar Format](https://arrow.apache.org/docs/format/Columnar.html) as the
-memory model. - Lazy | eager execution - Multi-threaded - SIMD - Query
-optimization - Powerful expression API - Hybrid Streaming (larger than RAM
-datasets) - Rust | Python | NodeJS | ... To learn more, read the [User Guide]
-(https://pola-rs.github.io/polars-book/). ```python >>> import polars as pl >>>
-df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ... "fruits": ["banana",
-"banana", "apple", "apple", "banana"], ... "B": [5, 4, 3, 2, 1], ... "cars":
-["beetle", "audi", "beetle", "beetle", "beetle"], ... } ... ) # embarrassingly
-parallel execution & very expressive query language >>> df.sort
-("fruits").select( ... "fruits", ... "cars", ... pl.lit("fruits").alias
+## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL Polars
+is a DataFrame interface on top of an OLAP Query Engine implemented in Rust
+using [Apache Arrow Columnar Format](https://arrow.apache.org/docs/format/
+Columnar.html) as the memory model. - Lazy | eager execution - Multi-threaded -
+SIMD - Query optimization - Powerful expression API - Hybrid Streaming (larger
+than RAM datasets) - Rust | Python | NodeJS | ... To learn more, read the [User
+Guide](https://pola-rs.github.io/polars-book/). ## Python ```python >>> import
+polars as pl >>> df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ...
+"fruits": ["banana", "banana", "apple", "apple", "banana"], ... "B": [5, 4, 3,
+2, 1], ... "cars": ["beetle", "audi", "beetle", "beetle", "beetle"], ... } ...
+) # embarrassingly parallel execution & very expressive query language >>>
+df.sort("fruits").select( ... "fruits", ... "cars", ... pl.lit("fruits").alias
 ("literal_string_fruits"), ... pl.col("B").filter(pl.col("cars") ==
 "beetle").sum(), ... pl.col("A").filter(pl.col("B") > 2).sum().over
 ("cars").alias("sum_A_by_cars"), ... pl.col("A").sum().over("fruits").alias
 ("sum_A_by_fruits"), ... pl.col("A").reverse().over("fruits").alias
 ("rev_A_by_fruits"), ... pl.col("A").sort_by("B").over("fruits").alias
 ("sort_A_by_B_by_fruits"), ... ) shape: (5, 8)
 ââââââââââââ¬âââââââââââ¬âââââââââââââââ¬ââââââ¬ââââââââââââââ¬ââââââââââââââ¬ââââââââââââââ¬ââââââââââââââ
@@ -66,17 +66,30 @@
 ââââââââââââªâââââââââââªâââââââââââââââªââââââªââââââââââââââªââââââââââââââªââââââââââââââªââââââââââââââ¡
 â "apple" â "beetle" â "fruits" â 11 â 4 â 7 â 4 â 4 â â
 "apple" â "beetle" â "fruits" â 11 â 4 â 7 â 3 â 3 â â
 "banana" â "beetle" â "fruits" â 11 â 4 â 8 â 5 â 5 â â
 "banana" â "audi" â "fruits" â 11 â 2 â 8 â 2 â 2 â â
 "banana" â "beetle" â "fruits" â 11 â 4 â 8 â 1 â 1 â
 ââââââââââââ´âââââââââââ´âââââââââââââââ´ââââââ´ââââââââââââââ´ââââââââââââââ´ââââââââââââââ´ââââââââââââââ
-``` ## Performance ðð ### Blazingly fast Polars is very fast. In fact, it
-is one of the best performing solutions available. See the results in [h2oai's
-db-benchmark](https://h2oai.github.io/db-benchmark/). In the [TPCH benchmarks]
+``` ## SQL ```python >>> # create a sql context >>> context = pl.SQLContext()
+>>> # register a table >>> table = pl.scan_ipc("file.arrow") >>>
+context.register("my_table", table) >>> # the query we want to run >>> query =
+""" ... SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM my_table ... WHERE id1
+= 'id016' ... LIMIT 10 ... """ >>> ## OPTION 1 >>> # run query to
+materialization >>> context.query(query) shape: (1, 2)
+ââââââââââ¬âââââââââ â sum_v1 â min_v2
+â â --- â --- â â i64 â i64 â
+ââââââââââªâââââââââ¡ â 298268 â 1 â
+ââââââââââ´âââââââââ >>> ## OPTION 2 >>> #
+Don't materialize the query, but return as LazyFrame >>> # and continue in
+python >>> lf = context.execute(query) >>> (lf.join(other_table) ... .groupby
+("foo") ... .agg( ... pl.col("sum_v1").count() ... ).collect()) ``` ##
+Performance ðð ### Blazingly fast Polars is very fast. In fact, it is one
+of the best performing solutions available. See the results in [h2oai's db-
+benchmark](https://h2oai.github.io/db-benchmark/). In the [TPCH benchmarks]
 (https://www.pola.rs/benchmarks.html) polars is orders of magnitudes faster
 than pandas, dask, modin and vaex on full queries (including IO). ###
 Lightweight Polars is also very lightweight. It comes with zero required
 dependencies, and this shows in the import times: - polars: 70ms - numpy: 104ms
 - pandas: 520ms ### Handles larger than RAM data If you have data that does not
 fit into memory, polars lazy is able to process your query (or parts of your
 query) in a streaming fashion, this drastically reduces memory requirements so
```

