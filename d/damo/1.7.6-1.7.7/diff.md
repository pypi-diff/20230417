# Comparing `tmp/damo-1.7.6.tar.gz` & `tmp/damo-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.7.6.tar", last modified: Mon Apr 10 17:35:57 2023, max compression
+gzip compressed data, was "damo-1.7.7.tar", last modified: Mon Apr 17 21:31:34 2023, max compression
```

## Comparing `damo-1.7.6.tar` & `damo-1.7.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.323521 damo-1.7.6/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-10 17:35:57.323521 damo-1.7.6/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5998 2023-04-10 17:35:53.000000 damo-1.7.6/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-10 17:35:53.000000 damo-1.7.6/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-10 17:35:57.323521 damo-1.7.6/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-10 17:35:53.000000 damo-1.7.6/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.307522 damo-1.7.6/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.323521 damo-1.7.6/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34437 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9979 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8196 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17741 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17021 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20452 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3643 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5108 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1599 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1530 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3097 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2733 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      681 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      651 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5568 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.323521 damo-1.7.6/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.149330 damo-1.7.7/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-17 21:31:34.149330 damo-1.7.7/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5998 2023-04-17 21:31:29.000000 damo-1.7.7/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-17 21:31:29.000000 damo-1.7.7/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-17 21:31:34.149330 damo-1.7.7/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-17 21:31:29.000000 damo-1.7.7/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.133331 damo-1.7.7/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.145331 damo-1.7.7/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    33489 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9973 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8196 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17739 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17620 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19529 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3643 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1619 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1531 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3268 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      681 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      651 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5568 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.149330 damo-1.7.7/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.7.6/PKG-INFO` & `damo-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.6
+Version: 1.7.7
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.6/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.7/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
```

### Comparing `damo-1.7.6/README.md` & `damo-1.7.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.6/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.7/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
```

### Comparing `damo-1.7.6/setup.py` & `damo-1.7.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="damo",
-    version="1.7.6",
+    version="1.7.7",
     author="SeongJae Park",
     author_email="sj@kernel.org",
     description="DAMON user-space tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awslabs/damo",
     project_urls={
```

### Comparing `damo-1.7.6/src/damo/_damo_dist.py` & `damo-1.7.7/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damo_fmt_str.py` & `damo-1.7.7/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damo_fs.py` & `damo-1.7.7/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damo_paddr_layout.py` & `damo-1.7.7/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damo_python2_support.py` & `damo-1.7.7/src/damo/_damo_python2_support.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damo_subcmds.py` & `damo-1.7.7/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damon.py` & `damo-1.7.7/src/damo/_damon.py`

 * *Files 10% similar despite different names*

```diff
@@ -103,116 +103,150 @@
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
             ('start', _damo_fmt_str.format_nr(self.start, raw)),
             ('end', _damo_fmt_str.format_nr(self.end, raw))])
 
 class DamonTarget:
-    name = None
     pid = None
     regions = None
 
-    def __init__(self, name, pid, regions):
-        self.name = name
+    def __init__(self, pid, regions):
         self.pid = pid
         self.regions = regions
 
     def to_str(self, raw):
-        lines = ['%s (pid: %s)' % (self.name, self.pid)]
+        lines = ['pid: %s' % self.pid]
         for region in self.regions:
             lines.append('region %s' % region.to_str(raw))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return type(self) == type(other) and '%s' % self == '%s' % other
 
     @classmethod
     def from_kvpairs(cls, kvpairs):
         regions = [DamonRegion.from_kvpairs(kvp) for kvp in kvpairs['regions']]
-        return DamonTarget(kvpairs['name'], kvpairs['pid'], regions)
+        return DamonTarget(kvpairs['pid'], regions)
 
     def to_kvpairs(self, raw=False):
-        kvp = collections.OrderedDict(
-                [(attr, getattr(self, attr)) for attr in ['name', 'pid']])
+        kvp = collections.OrderedDict()
+        kvp['pid'] = self.pid
         kvp['regions'] = [r.to_kvpairs(raw) for r in self.regions]
         return kvp
 
 unit_percent = 'percent'
 unit_sample_intervals = 'sample_intervals'
 unit_usec = 'usec'
 unit_aggr_intervals = 'aggr_intervals'
 
+class DamonIntervalsBasedValUnit:
+    value = None
+    unit = None # percent, sample_intervals, usec, aggr_intervals
+
+    def __init__(self, value, unit):
+        self.value = value
+        self.unit = unit
+
+    def eq(self, other, intervals=None):
+        if intervals == None:
+            return self.value == other.value and self.unit == other.unit
+
+        return self.value == other.value_for(self.unit, intervals)
+
+    def __eq__(self, other):
+        return self.eq(other, None)
+
+    def value_for(self, new_unit, intervals):
+        if self.unit == new_unit:
+            return self.value
+        if self.unit == unit_sample_intervals and new_unit == unit_percent:
+            max_val = intervals.aggr / intervals.sample
+            return int(self.value * 100.0 / max_val)
+        elif self.unit == unit_percent and new_unit == unit_sample_intervals:
+            max_val = intervals.aggr / intervals.sample
+            return int(self.value * max_val / 100)
+        elif self.unit == unit_aggr_intervals and new_unit == unit_usec:
+            return self.value * intervals.aggr
+        elif self.unit == unit_usec and new_unit == unit_aggr_intervals:
+            return int(self.value / intervals.aggr)
+        raise Exception('unsupported unit change')
+
+    def convert_unit(self, new_unit, intervals):
+        self.value = self.value_for(new_unit, intervals)
+        self.unit = new_unit
+
+    def to_str(self, raw):
+        unit = self.unit
+
+        if unit == unit_usec:
+            return _damo_fmt_str.format_time_us_exact(self.value, raw)
+
+        if unit == unit_percent:
+            unit = '%'
+        return '%s %s' % (_damo_fmt_str.format_nr(self.value, raw), unit)
+
 class DamosAccessPattern:
     sz_bytes = None
-    nr_accesses = None
-    nr_accesses_unit = None # unit_{percent,sample_intervals}
-    age = None
-    age_unit = None #  unit_{usec,aggr_intervals}
+    nr_accesses = None # [min/max DamonIntervalsBasedValUnit]
+    age = None  # [min/max DamonIntervalsBasedValUnit]
 
     # every region by default, so that it can be used for monitoring
     def __init__(self, sz_bytes=['min', 'max'],
             nr_accesses=['min', 'max'], nr_accesses_unit=unit_percent,
             age=['min', 'max'], age_unit=unit_usec):
         self.sz_bytes = [_damo_fmt_str.text_to_bytes(sz_bytes[0]),
                 _damo_fmt_str.text_to_bytes(sz_bytes[1])]
 
-        if nr_accesses_unit == unit_percent:
-            fn = _damo_fmt_str.text_to_percent
-        elif nr_accesses_unit == unit_sample_intervals:
-            fn = _damo_fmt_str.text_to_nr
-        else:
+        parsers_for_unit = {
+                unit_percent: _damo_fmt_str.text_to_percent,
+                unit_sample_intervals: _damo_fmt_str.text_to_nr,
+                unit_usec: _damo_fmt_str.text_to_us,
+                unit_aggr_intervals: _damo_fmt_str.text_to_nr}
+
+        if not nr_accesses_unit in parsers_for_unit:
             raise Exception('invalid access pattern nr_accesses_unit \'%s\'' %
                     nr_accesses_unit)
-        self.nr_accesses = [fn(nr_accesses[0]), fn(nr_accesses[1])]
-        self.nr_accesses_unit = nr_accesses_unit
-
-        if age_unit == unit_usec:
-            fn = _damo_fmt_str.text_to_us
-        elif age_unit == unit_aggr_intervals:
-            fn = _damo_fmt_str.text_to_nr
-        else:
+        if not age_unit in parsers_for_unit:
             raise Exception('invalid access pattern age_unit \'%s\'' %
                     age_unit)
-        self.age = [fn(age[0]), fn(age[1])]
-        self.age_unit = age_unit
+
+        unit = nr_accesses_unit
+        fn = parsers_for_unit[unit]
+        self.nr_accesses = [
+                DamonIntervalsBasedValUnit(fn(nr_accesses[0]), unit),
+                DamonIntervalsBasedValUnit(fn(nr_accesses[1]), unit)]
+
+        fn = parsers_for_unit[age_unit]
+        self.age = [
+                DamonIntervalsBasedValUnit(fn(age[0]), age_unit),
+                DamonIntervalsBasedValUnit(fn(age[1]), age_unit)]
 
     def to_str(self, raw):
         lines = [
             'sz: [%s, %s]' % (_damo_fmt_str.format_sz(self.sz_bytes[0], raw),
                 _damo_fmt_str.format_sz(self.sz_bytes[1], raw)),
             ]
-        unit = self.nr_accesses_unit
-        if unit == unit_percent:
-            unit = '%'
-        lines.append('nr_accesses: [%s %s, %s %s]' % (
-                _damo_fmt_str.format_nr(self.nr_accesses[0], raw), unit,
-                _damo_fmt_str.format_nr(self.nr_accesses[1], raw), unit))
-        if self.age_unit == unit_usec:
-            min_age = _damo_fmt_str.format_time_us_exact(self.age[0], raw)
-            max_age = _damo_fmt_str.format_time_us_exact(self.age[1], raw)
-        else:
-            min_age = '%s %s' % (
-                    _damo_fmt_str.format_nr(self.age[0], raw), self.age_unit)
-            max_age = '%s %s' % (
-                    _damo_fmt_str.format_nr(self.age[1], raw), self.age_unit)
-        lines.append('age: [%s, %s]' % (min_age, max_age))
+        lines.append('nr_accesses: [%s, %s]' % (
+            self.nr_accesses[0].to_str(raw), self.nr_accesses[1].to_str(raw)))
+        lines.append('age: [%s, %s]' %
+                (self.age[0].to_str(raw), self.age[1].to_str(raw)))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return (type(self) == type(other) and
                 self.sz_bytes == other.sz_bytes and
                 self.nr_accesses == other.nr_accesses and
-                self.nr_accesses_unit == other.nr_accesses_unit and
-                self.age == other.age and self.age_unit == other.age_unit)
+                self.age == other.age)
 
     @classmethod
     def from_kvpairs(cls, kv):
         sz_bytes = [_damo_fmt_str.text_to_bytes(kv['sz_bytes']['min']),
                 _damo_fmt_str.text_to_bytes(kv['sz_bytes']['max'])]
 
         kv_ = kv['nr_accesses']
@@ -239,74 +273,34 @@
                 raise Exception('age units should be same')
             age = [min_age, max_age]
 
         return DamosAccessPattern(sz_bytes, nr_accesses, nr_accesses_unit, age,
                 age_unit)
 
     def to_kvpairs(self, raw=False):
-        unit = self.nr_accesses_unit
-        if unit == unit_percent:
-            unit = '%'
-        min_nr_accesses = '%s %s' % (
-                _damo_fmt_str.format_nr(self.nr_accesses[0], raw), unit)
-        max_nr_accesses = '%s %s' % (
-                _damo_fmt_str.format_nr(self.nr_accesses[1], raw), unit)
-        if self.age_unit == unit_usec:
-            min_age = _damo_fmt_str.format_time_us_exact(self.age[0], raw)
-            max_age = _damo_fmt_str.format_time_us_exact(self.age[1], raw)
-        else:
-            min_age = '%s %s' % (
-                    _damo_fmt_str.format_nr(self.age[0], raw), self.age_unit)
-            max_age = '%s %s' % (
-                    _damo_fmt_str.format_nr(self.age[1], raw), self.age_unit)
+        min_nr_accesses = self.nr_accesses[0].to_str(raw)
+        max_nr_accesses = self.nr_accesses[1].to_str(raw)
+        min_age = self.age[0].to_str(raw)
+        max_age = self.age[1].to_str(raw)
 
         return collections.OrderedDict([
             ('sz_bytes', (collections.OrderedDict([
                 ('min', _damo_fmt_str.format_sz(self.sz_bytes[0], raw)),
                 ('max', _damo_fmt_str.format_sz(self.sz_bytes[1], raw))]))),
             ('nr_accesses', (collections.OrderedDict([
                 ('min', min_nr_accesses), ('max', max_nr_accesses)]))),
             ('age', (collections.OrderedDict([
                 ('min', min_age), ('max', max_age)]))),
             ])
 
-    def convert_nr_accesses_unit(self, nr_accesses_unit, intervals):
-        if self.nr_accesses_unit == nr_accesses_unit:
-            return
-        max_nr_accesses_sample_intervals = intervals.aggr / intervals.sample
-        # percent to sample_intervals
-        if nr_accesses_unit == unit_sample_intervals:
-            self.nr_accesses[0] = int(self.nr_accesses[0] *
-                    max_nr_accesses_sample_intervals / 100)
-            self.nr_accesses[1] = int(self.nr_accesses[1] *
-                    max_nr_accesses_sample_intervals / 100)
-        # sample_intervals to percent
-        else:
-            self.nr_accesses[0] = int(self.nr_accesses[0] * 100.0 /
-                    max_nr_accesses_sample_intervals)
-            self.nr_accesses[1] = int(self.nr_accesses[1] * 100.0 /
-                    max_nr_accesses_sample_intervals)
-        self.nr_accesses_unit = nr_accesses_unit
-
-    def convert_age_unit(self, age_unit, intervals):
-        if self.age_unit == age_unit:
-            return
-        # aggr_intervals to usec
-        if age_unit == unit_usec:
-            self.age[0] = self.age[0] * intervals.aggr
-            self.age[1] = self.age[1] * intervals.aggr
-        # usec to aggr_intervals
-        else:
-            self.age[0] = int(self.age[0] / intervals.aggr)
-            self.age[1] = int(self.age[1] / intervals.aggr)
-        self.age_unit = age_unit
-
     def convert_for_units(self, nr_accesses_unit, age_unit, intervals):
-        self.convert_nr_accesses_unit(nr_accesses_unit, intervals)
-        self.convert_age_unit(age_unit, intervals)
+        self.nr_accesses[0].convert_unit(nr_accesses_unit, intervals)
+        self.nr_accesses[1].convert_unit(nr_accesses_unit, intervals)
+        self.age[0].convert_unit(age_unit, intervals)
+        self.age[1].convert_unit(age_unit, intervals)
 
     def converted_for_units(self, nr_accesses_unit, age_unit, intervals):
         copied = copy.deepcopy(self)
         copied.convert_for_units(nr_accesses_unit, age_unit, intervals)
         return copied
 
     def effectively_equal(self, other, intervals):
@@ -437,21 +431,19 @@
                 ('mid_permil',
                     _damo_fmt_str.format_permil(self.mid_permil, raw)),
                 ('low_permil',
                     _damo_fmt_str.format_permil(self.low_permil, raw)),
                 ])
 
 class DamosFilter:
-    name = None
     filter_type = None  # anon or memcg
     memcg_path = None
     matching = None
 
-    def __init__(self, name, filter_type, memcg_path, matching):
-        self.name = name
+    def __init__(self, filter_type, memcg_path, matching):
         self.filter_type = filter_type
         self.memcg_path = memcg_path
         self.matching = _damo_fmt_str.text_to_bool(matching)
 
     def to_str(self, raw):
         memcg_path_str = ''
         if self.filter_type == 'memcg':
@@ -463,22 +455,22 @@
         return self.to_str(False)
 
     def __eq__(self, other):
         return type(self) == type(other) and '%s' % self == '%s' % other
 
     @classmethod
     def from_kvpairs(cls, kv):
-        return DamosFilter(kv['name'], kv['filter_type'],
+        return DamosFilter(kv['filter_type'],
                 kv['memcg_path'] if kv['filter_type'] == 'memcg' else '',
                 kv['matching'])
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict(
                 [(attr, getattr(self, attr)) for attr in [
-                    'name', 'filter_type', 'memcg_path', 'matching']])
+                    'filter_type', 'memcg_path', 'matching']])
 
 class DamosStats:
     nr_tried = None
     sz_tried = None
     nr_applied = None
     sz_applied = None
     qt_exceeds = None
@@ -503,31 +495,33 @@
         return self.to_str(False)
 
 class DamosTriedRegion:
     start = None
     end = None
     nr_accesses = None
     age = None
+    age_unit = None
 
-    def __init__(self, start, end, nr_accesses, age):
+    def __init__(self, start, end, nr_accesses, age, age_unit):
         self.start = start
         self.end = end
         self.nr_accesses = nr_accesses
         self.age = age
+        self.age_unit = age_unit
 
     def to_str(self, raw, intervals=None):
         age = self.age
         if raw == False and intervals != None:
             max_nr_accesses = intervals.aggr / intervals.sample
             nr_accesses = '%.2f%%' % (
                     float(self.nr_accesses) * 100 / max_nr_accesses)
             age = _damo_fmt_str.format_time_us(age * intervals.aggr, raw)
         else:
             nr_accesses = '%s' % _damo_fmt_str.format_nr(self.nr_accesses, raw)
-            age = _damo_fmt_str.format_nr(age, raw)
+            age = '%s %s' % (_damo_fmt_str.format_nr(age, raw), self.age_unit)
         return '%s: nr_accesses: %s, age: %s' % (
                 _damo_fmt_str.format_addr_range(self.start, self.end, raw),
                 nr_accesses, age)
 
     def __str__(self):
         return self.to_str(False)
 
@@ -549,54 +543,52 @@
 damos_action_hugepage = damos_actions[3]
 damos_action_nohugepage = damos_actions[4]
 damos_action_lru_prio = damos_actions[5]
 damos_action_lru_deprio = damos_actions[6]
 damos_action_stat = damos_actions[7]
 
 class Damos:
-    name = None
     access_pattern = None
     action = None
     quotas = None
     watermarks = None
     filters = None
     stats = None
     tried_regions = None
 
     # for monitoring only by default
-    def __init__(self, name='0', access_pattern=None, action=damos_action_stat,
+    def __init__(self, access_pattern=None, action=damos_action_stat,
             quotas=None, watermarks=None, filters=None, stats=None,
             tried_regions=None):
-        self.name = name
         self.access_pattern = (access_pattern
                 if access_pattern != None else DamosAccessPattern())
         if not action in damos_actions:
             raise Exception('wrong damos action: %s' % action)
         self.action = action
         self.quotas = quotas if quotas != None else DamosQuotas()
         self.watermarks = (watermarks
                 if watermarks != None else DamosWatermarks())
         self.filters = filters if filters != None else []
         self.stats = stats
         self.tried_regions = tried_regions
 
     def to_str(self, raw):
-        lines = ['%s (action: %s)' % (self.name, self.action)]
+        lines = ['action: %s' % self.action]
         lines.append('target access pattern')
         lines.append(_damo_fmt_str.indent_lines(
             self.access_pattern.to_str(raw), 4))
         lines.append('quotas')
         lines.append(_damo_fmt_str.indent_lines(self.quotas.to_str(raw), 4))
         lines.append('watermarks')
         lines.append(_damo_fmt_str.indent_lines(
             self.watermarks.to_str(raw), 4))
-        lines.append('filters')
-        for damos_filter in self.filters:
+        for idx, damos_filter in enumerate(self.filters):
+            lines.append('filter %d' % idx)
             lines.append(_damo_fmt_str.indent_lines(
-                damos_filter.to_str(raw), 8))
+                damos_filter.to_str(raw), 4))
         if self.stats != None:
             lines.append('statistics')
             lines.append(_damo_fmt_str.indent_lines(self.stats.to_str(raw), 4))
         if self.tried_regions != None:
             lines.append('tried regions')
             for region in self.tried_regions:
                 lines.append(_damo_fmt_str.indent_lines(region.to_str(raw), 4))
@@ -605,40 +597,39 @@
     def __str__(self):
         return self.to_str(False)
 
     def __repr__(self):
         return self.__str__()
 
     def __eq__(self, other):
-        return (type(self) == type(other) and self.name == other.name and
+        return (type(self) == type(other) and
                 self.access_pattern == other.access_pattern and
                 self.action == other.action and self.quotas == other.quotas and
                 self.watermarks == other.watermarks and
                 self.filters == other.filters)
 
     @classmethod
     def from_kvpairs(cls, kv):
         filters = []
         if 'filters' in kv:
             for damos_filter_kv in kv['filters']:
                 filters.append(DamosFilter.from_kvpairs(damos_filter_kv))
-        return Damos(kv['name'] if 'name' in kv else '0',
-                DamosAccessPattern.from_kvpairs(kv['access_pattern'])
+        return Damos(DamosAccessPattern.from_kvpairs(kv['access_pattern'])
                     if 'access_pattern' in kv else DamosAccessPattern(),
                 kv['action'] if 'action' in kv else damos_action_stat,
                 DamosQuotas.from_kvpairs(kv['quotas'])
                     if 'quotas' in kv else DamosQuotas(),
                 DamosWatermarks.from_kvpairs(kv['watermarks'])
                     if 'watermarks' in kv else DamosWatermarks(),
                 filters,
                 None, None)
 
     def to_kvpairs(self, raw=False):
-        kv = collections.OrderedDict(
-                [(attr, getattr(self, attr)) for attr in ['name', 'action']])
+        kv = collections.OrderedDict()
+        kv['action'] = self.action
         kv['access_pattern'] = self.access_pattern.to_kvpairs(raw)
         kv['quotas'] = self.quotas.to_kvpairs(raw)
         kv['watermarks'] = self.watermarks.to_kvpairs(raw)
         filters = []
         for damos_filter in self.filters:
             filters.append(damos_filter.to_kvpairs(raw))
         kv['filters'] = filters
@@ -679,125 +670,119 @@
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict(
                 [(attr, getattr(self, attr)) for attr in
                     ['rfile_buf', 'rfile_path']])
 
 class DamonCtx:
-    name = None
     intervals = None
     nr_regions = None
     ops = None
     targets = None
     schemes = None
     # For old downstream kernels that supports record feature
     record_request = None
 
-    def __init__(self, name, intervals, nr_regions, ops, targets, schemes,
+    def __init__(self, intervals, nr_regions, ops, targets, schemes,
             record_request=None):
-        self.name = name
         self.intervals = intervals
         self.nr_regions = nr_regions
         self.ops = ops
         self.targets = targets
         self.schemes = schemes
         self.record_request = record_request
 
     def to_str(self, raw):
-        lines = ['%s (ops: %s)' % (self.name, self.ops)]
+        lines = ['ops: %s' % self.ops]
         lines.append('intervals: %s' % self.intervals.to_str(raw))
         lines.append('nr_regions: %s' % self.nr_regions.to_str(raw))
-        lines.append('targets')
-        for target in self.targets:
+        for idx, target in enumerate(self.targets):
+            lines.append('target %d' % idx)
             lines.append(_damo_fmt_str.indent_lines(target.to_str(raw), 4))
-        lines.append('schemes')
-        for scheme in self.schemes:
+        for idx, scheme in enumerate(self.schemes):
+            lines.append('scheme %d' % idx)
             lines.append(_damo_fmt_str.indent_lines(scheme.to_str(raw), 4))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return type(self) == type(other) and '%s' % self == '%s' % other
 
     def __hash__(self):
         return hash(self.__str__())
 
     @classmethod
     def from_kvpairs(cls, kv):
-        ctx = DamonCtx(kv['name'],
+        ctx = DamonCtx(
                 DamonIntervals.from_kvpairs(kv['intervals'])
                     if 'intervals' in kv else DamonIntervals(),
                 DamonNrRegionsRange.from_kvpairs(kv['nr_regions'])
                     if 'nr_regions' in kv else DAmonNrRegionsRange(),
                 kv['ops'],
                 [DamonTarget.from_kvpairs(t) for t in kv['targets']],
                 [Damos.from_kvpairs(s) for s in kv['schemes']]
                     if 'schemes' in kv else [])
         if 'record_request' in kv:
             ctx.record_request = DamonRecord.from_kvpairs(kv['record_request'])
         return ctx
 
     def to_kvpairs(self, raw=False):
         kv = collections.OrderedDict({})
-        kv['name'] = self.name
         kv['intervals'] = self.intervals.to_kvpairs(raw)
         kv['nr_regions'] = self.nr_regions.to_kvpairs(raw)
         kv['ops'] = self.ops
         kv['targets'] = [t.to_kvpairs(raw) for t in self.targets]
         kv['schemes'] = [s.to_kvpairs(raw) for s in self.schemes]
         if self.record_request:
             kv['record_request'] = self.record_request.to_kvpairs(raw)
         return kv
 
 def target_has_pid(ops):
     return ops in ['vaddr', 'fvaddr']
 
 class Kdamond:
-    name = None
     state = None
     pid = None
     contexts = None
 
-    def __init__(self, name, state, pid, contexts):
-        self.name = name
+    def __init__(self, state, pid, contexts):
         self.state = state
         self.pid = pid
         self.contexts = contexts
 
     def summary_str(self):
-        return '%s (state: %s, pid: %s)' % (self.name, self.state, self.pid)
+        return 'state: %s, pid: %s' % (self.state, self.pid)
 
     def to_str(self, raw):
         lines = [self.summary_str()]
-        for ctx in self.contexts:
-            lines.append('contexts')
+        for idx, ctx in enumerate(self.contexts):
+            lines.append('context %d' % idx)
             lines.append(_damo_fmt_str.indent_lines(ctx.to_str(raw), 4))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return type(self) == type(other) and '%s' % self == '%s' % other
 
     def __hash__(self):
         return hash(self.__str__())
 
     @classmethod
     def from_kvpairs(cls, kv):
-        return Kdamond(kv['name'],
+        return Kdamond(
                 kv['state'] if 'state' in kv else 'off',
                 kv['pid'] if 'pid' in kv else None,
                 [DamonCtx.from_kvpairs(c) for c in kv['contexts']])
 
     def to_kvpairs(self, raw=False):
         kv = collections.OrderedDict()
-        kv['name'] = self.name
         kv['state'] = self.state
         kv['pid'] = self.pid
         kv['contexts'] = [c.to_kvpairs(raw) for c in self.contexts]
         return kv
 
 import _damo_fs
 import _damon_dbgfs
@@ -923,15 +908,15 @@
         return 'debugfs interface unsupport commit_staged()'
     return _damon_fs.commit_staged(kdamond_names)
 
 def commit(kdamonds):
     err = stage_kdamonds(kdamonds)
     if err:
         return 'staging updates failed (%s)' % err
-    err = commit_staged([k.name for k in kdamonds])
+    err = commit_staged(['%s' % idx for idx, k in enumerate(kdamonds)])
     if err:
         return 'commit staged updates filed (%s)' % err
     return None
 
 def update_schemes_stats(kdamond_names=None):
     if kdamond_names == None:
         kdamond_names = running_kdamond_names()
```

### Comparing `damo-1.7.6/src/damo/_damon_args.py` & `damo-1.7.7/src/damo/_damon_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     ops = args.ops
 
     init_regions, err = init_regions_for(args)
     if err:
         return None, err
 
     try:
-        target = _damon.DamonTarget('0', args.target_pid
+        target = _damon.DamonTarget(args.target_pid
                 if _damon.target_has_pid(ops) else None, init_regions)
     except Exception as e:
         return 'Wrong \'--target_pid\' argument (%s)' % e
 
     record_request = None
     if 'rbuf' in args and args.rbuf != None:
         try:
@@ -94,16 +94,16 @@
             return None, 'Wrong record arguments (%s)' % e
 
     schemes, err = _damon_args_schemes.damos_for(args)
     if err:
         return None, err
 
     try:
-        ctx = _damon.DamonCtx('0', intervals, nr_regions, ops, [target],
-                schemes, record_request)
+        ctx = _damon.DamonCtx(intervals, nr_regions, ops, [target], schemes,
+                record_request)
         return ctx, None
     except Exception as e:
         return None, 'Creating context from arguments failed (%s)' % e
 
 def kdamonds_from_json_arg(arg):
     try:
         if os.path.isfile(arg):
@@ -153,16 +153,15 @@
         err = deduce_target_update_args(args)
         if err:
             return None, err
 
     ctx, err = damon_ctx_for(args)
     if err:
         return None, err
-    return [_damon.Kdamond(name='0', state=None, pid=None,
-        contexts=[ctx])], None
+    return [_damon.Kdamond(state=None, pid=None, contexts=[ctx])], None
 
 def self_started_target(args):
     return 'self_started_target' in args and args.self_started_target
 
 # Command line processing helpers
 
 def is_ongoing_target(args):
@@ -187,15 +186,15 @@
     return kdamonds, None
 
 def turn_damon_on(args):
     kdamonds, err = stage_kdamonds(args)
     if err:
         return err, None
     return _damon.turn_damon_on(
-            [k.name for k in kdamonds]), kdamonds
+            ['%s' % kidx for kidx, k in enumerate(kdamonds)]), kdamonds
 
 # Commandline options setup helpers
 
 def set_common_argparser(parser):
     parser.add_argument('--damon_interface',
             choices=['sysfs', 'debugfs', 'auto'],
             default='auto',
```

### Comparing `damo-1.7.6/src/damo/_damon_args_schemes.py` & `damo-1.7.7/src/damo/_damon_args_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/_damon_dbgfs.py` & `damo-1.7.7/src/damo/_damon_dbgfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             intervals)
     quotas = damos.quotas
     watermarks = damos.watermarks
 
     max_nr_accesses = intervals.aggr / intervals.sample
     v0_scheme = '%d\t%d\t%d\t%d\t%d\t%d\t%s' % (
             pattern.sz_bytes[0], pattern.sz_bytes[1],
-            pattern.nr_accesses[0], pattern.nr_accesses[1],
-            pattern.age[0], pattern.age[1],
+            pattern.nr_accesses[0].value, pattern.nr_accesses[1].value,
+            pattern.age[0].value, pattern.age[1].value,
             damos_action_to_file_input(damos.action))
     if scheme_version == 0:
         return v0_scheme
 
     v1_scheme = '%s\t%d\t%d' % (v0_scheme,
             quotas.sz_bytes, quotas.reset_interval_ms)
     if scheme_version == 1:
@@ -284,15 +284,15 @@
                 fields[i + 1], fields[i + 2]))
     ops = 'vaddr'
     is_paddr = False
     if 42 in target_ids:
         ops = 'paddr'
     targets = []
     for idx, target_id in enumerate(target_ids):
-        targets.append(_damon.DamonTarget(name='%d' % idx,
+        targets.append(_damon.DamonTarget(
             pid=target_id if not is_paddr else None,
             regions=regions_dict[idx
                 if feature_supported('init_regions_target_idx')
                 else target_id] if len(regions_dict) > 0 else []))
 
     if feature_supported('record'):
         fields = files_content['record'].strip().split()
@@ -300,20 +300,20 @@
 
     schemes = []
     for line in files_content['schemes'].split('\n'):
         if line.strip() == '':
             continue
         schemes.append(debugfs_output_to_damos(line, intervals))
 
-    ctx = _damon.DamonCtx('0', intervals, nr_regions, ops, targets, schemes)
+    ctx = _damon.DamonCtx(intervals, nr_regions, ops, targets, schemes)
     if feature_supported('record'):
         ctx.record_request = record_request
     state = files_content['monitor_on'].strip()
     pid = files_content['kdamond_pid'].strip()
-    return [_damon.Kdamond('0', state, pid, [ctx])]
+    return [_damon.Kdamond(state, pid, [ctx])]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(debugfs_damon))
 
 def current_kdamond_names():
     # TODO: Support created kdamonds
```

### Comparing `damo-1.7.6/src/damo/_damon_result.py` & `damo-1.7.7/src/damo/_damon_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 PERF_EVENT = 'damon:damon_aggregated'
 
 class DAMONRegion:
     start = None
     end = None
     nr_accesses = None
     age = None
+    age_unit = None # _damon.unit_aggr_intervals or _damon.unit_usec
 
-    def __init__(self, start, end, nr_accesses, age):
+    def __init__(self, start, end, nr_accesses, age, age_unit):
         self.start = start
         self.end = end
         self.nr_accesses = nr_accesses
         self.age = age
+        self.age_unit = age_unit
 
 class DAMONSnapshot:
     start_time = None
     end_time = None
     regions = None
 
     def __init__(self, start_time, end_time):
@@ -77,15 +79,16 @@
 def read_snapshot_from_record_file(f, start_time, end_time):
     snapshot = DAMONSnapshot(start_time, end_time)
     nr_regions = struct.unpack('I', f.read(4))[0]
     for r in range(nr_regions):
         start_addr = struct.unpack('L', f.read(8))[0]
         end_addr = struct.unpack('L', f.read(8))[0]
         nr_accesses = struct.unpack('I', f.read(4))[0]
-        region = DAMONRegion(start_addr, end_addr, nr_accesses, None)
+        region = DAMONRegion(start_addr, end_addr, nr_accesses, None,
+                _damon.unit_aggr_intervals)
         snapshot.regions.append(region)
     return snapshot
 
 # if number of snapshots is one, write_damon_record() adds a fake snapshot for
 # snapshot start time deduction.
 def is_fake_snapshot(snapshot):
     if len(snapshot.regions) != 1:
@@ -161,15 +164,16 @@
 
         start_addr, end_addr = [int(x) for x in fields[7][:-1].split('-')]
         nr_accesses = int(fields[8])
         if len(fields) == 10:
             age = int(fields[9])
         else:
             age = None
-        region = DAMONRegion(start_addr, end_addr, nr_accesses, age)
+        region = DAMONRegion(start_addr, end_addr, nr_accesses, age,
+                _damon.unit_aggr_intervals)
 
         return region, end_time, target_id, nr_regions
 
 def perf_script_to_damon_result(script_output):
     result = DAMONResult()
     snapshot = None
 
@@ -302,15 +306,16 @@
             # we cannot know start/end time of single snapshot from the file
             # to allow it with later read, write a fake snapshot
             snapshot = snapshots[0]
             snap_duration = snapshot.end_time - snapshot.start_time
             fake_snapshot = DAMONSnapshot(snapshot.end_time,
                     snapshot.end_time + snap_duration)
             # -1 nr_accesses/ -1 age means fake
-            fake_snapshot.regions = [DAMONRegion(0, 0, -1, -1)]
+            fake_snapshot.regions = [DAMONRegion(0, 0, -1, -1,
+                _damon.unit_aggr_intervals)]
             snapshots.append(fake_snapshot)
     if file_type == file_type_record:
         write_damon_record(result, file_path, 2)
     elif file_type == file_type_perf_script:
         write_damon_perf_script(result, file_path)
     else:
         print('write unsupported file type: %s' % file_type)
@@ -333,18 +338,20 @@
             if not r in nr_acc_to_add:
                 nr_acc_to_add[r] = 0
             nr_acc_to_add[r] = max(nr_acc_to_add[r], region.nr_accesses)
 
             new_regions = []
             if region.start < r.start:
                 new_regions.append(DAMONRegion(
-                    region.start, r.start, region.nr_accesses, region.age))
+                    region.start, r.start, region.nr_accesses, region.age,
+                    _damon.unit_aggr_intervals))
             if r.end < region.end:
                 new_regions.append(DAMONRegion(
-                        r.end, region.end, region.nr_accesses, region.age))
+                        r.end, region.end, region.nr_accesses, region.age,
+                        _damon.unit_aggr_intervals))
 
             for new_r in new_regions:
                 add_region(regions, new_r, nr_acc_to_add)
             return
     regions.append(region)
 
 def aggregate_snapshots(snapshots):
@@ -431,20 +438,26 @@
 def tried_regions_to_snapshot(tried_regions, aggr_interval_us):
     snapshot_end_time_ns = time.time() * 1000000000
     snapshot_start_time_ns = snapshot_end_time_ns - aggr_interval_us * 1000
     snapshot = DAMONSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
 
     for tried_region in tried_regions:
         snapshot.regions.append(DAMONRegion(tried_region.start,
-            tried_region.end, tried_region.nr_accesses, tried_region.age))
+            tried_region.end, tried_region.nr_accesses,
+            tried_region.age * aggr_interval_us,
+            _damon.unit_usec))
     return snapshot
 
 def tried_regions_to_snapshots(monitor_scheme):
-    snapshots = {} # {kdamond: {ctx: Snapshot}}
-    for kdamond in _damon.running_kdamonds():
+    snapshots = {} # {kdamond idx: {ctx: Snapshot}}
+    for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
+        if kdamond.state != 'on':
+            continue
+        # TODO: Make a cleaner way for passing the index
+        kdamond.idx = kdamond_idx
         for ctx in kdamond.contexts:
             for scheme in ctx.schemes:
                 if scheme.effectively_equal(monitor_scheme, ctx.intervals):
                     snapshot = tried_regions_to_snapshot(scheme.tried_regions,
                             ctx.intervals.aggr)
                     snapshots[kdamond] = {ctx: snapshot}
                     break
@@ -459,16 +472,16 @@
 
     monitor_scheme = _damon.Damos(access_pattern=access_pattern)
 
     installed, err = ensure_scheme_installed(running_kdamonds, monitor_scheme)
     if err:
         return None, 'monitoring scheme install failed: %s' % err
 
-    err = _damon.update_schemes_tried_regions([k.name for k in
-        running_kdamonds])
+    err = _damon.update_schemes_tried_regions(['%d' % idx for idx, k in
+        enumerate(running_kdamonds)])
     if err != None:
         if installed:
             err = _damon.commit(orig_kdamonds)
             if err:
                 return None, 'monitoring scheme uninstall failed: %s' % err
         return None, 'updating schemes tried regions fail: %s' % err
```

### Comparing `damo-1.7.6/src/damo/_damon_sysfs.py` & `damo-1.7.7/src/damo/_damon_sysfs.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,67 +21,30 @@
 
 def kdamond_dir_of(kdamond_name):
     return os.path.join(admin_dir, 'kdamonds', '%s' % kdamond_name)
 
 def state_file_of(kdamond_name):
     return os.path.join(kdamond_dir_of(kdamond_name), 'state')
 
-def nr_contexts_file_of(kdamond_name):
-    return os.path.join(
-            kdamond_dir_of(kdamond_name), 'contexts', 'nr_contexts')
-
 def ctx_dir_of(kdamond_name, context_name):
     return os.path.join(
             kdamond_dir_of(kdamond_name), 'contexts', '%s' % context_name)
 
 def schemes_dir_of(kdamond_name, context_name):
     return os.path.join(ctx_dir_of(kdamond_name, context_name), 'schemes')
 
-def nr_schemes_file_of(kdamond_name, context_name):
-    return os.path.join(
-            schemes_dir_of(kdamond_name, context_name), 'nr_schemes')
-
 def scheme_dir_of(kdamond_name, context_name, scheme_name):
     return os.path.join(
             schemes_dir_of(kdamond_name, context_name), '%s' % scheme_name)
 
 def scheme_tried_regions_dir_of(kdamond_name, context_name, scheme_name):
     return os.path.join(
             scheme_dir_of(kdamond_name, context_name, scheme_name),
             'tried_regions')
 
-def filters_dir_of(kdamond_name, context_name, scheme_name):
-    return os.path.join(
-            scheme_dir_of(kdamond_name, context_name, scheme_name), 'filters')
-
-def nr_filters_file_of(kdamond_name, context_name, scheme_name):
-    return os.path.join(
-            filters_dir_of(kdamond_name, context_name, scheme_name),
-            'nr_filters')
-
-def targets_dir_of(kdamond_name, context_name):
-    return os.path.join(ctx_dir_of(kdamond_name, context_name), 'targets')
-
-def nr_targets_file_of(kdamond_name, context_name):
-    return os.path.join(
-            targets_dir_of(kdamond_name, context_name), 'nr_targets')
-
-def target_dir_of(kdamond_name, context_name, target_name):
-    return os.path.join(ctx_dir_of(kdamond_name, context_name), 'targets',
-            '%s' % target_name)
-
-def regions_dir_of(kdamond_name, context_name, target_name):
-    return os.path.join(
-            target_dir_of(kdamond_name, context_name, target_name), 'regions')
-
-def nr_regions_file_of(kdamond_name, context_name, target_name):
-    return os.path.join(
-            regions_dir_of(kdamond_name, context_name, target_name),
-            'nr_regions')
-
 def supported():
     return os.path.isdir(kdamonds_dir)
 
 def turn_damon_on(kdamonds_names):
     # In case of vaddr, too early monitoring shows unstable mapping changes.
     # Give the process a time to have stable memory mapping.
     time.sleep(0.5)
@@ -131,16 +94,16 @@
         'memcg_path': ('%s' % damos_filter.memcg_path
             if damos_filter.memcg_path != None else ''),
         'matching': 'Y' if damos_filter.matching else 'N',
         }
 
 def wops_for_scheme_filters(filters):
     wops = {}
-    for damos_filter in filters:
-        wops[damos_filter.name] = wops_for_scheme_filter(damos_filter)
+    for idx, damos_filter in enumerate(filters):
+        wops['%d' % idx] = wops_for_scheme_filter(damos_filter)
     return wops
 
 def wops_for_scheme_watermarks(wmarks):
     if wmarks == None:
         return {}
     return {
         'metric': wmarks.metric,
@@ -173,53 +136,54 @@
 
     return {
         'sz': {
             'min': '%d' % pattern.sz_bytes[0],
             'max': '%d' % pattern.sz_bytes[1],
         },
         'nr_accesses': {
-            'min': '%d' % pattern.nr_accesses[0],
-            'max': '%d' % pattern.nr_accesses[1],
+            'min': '%d' % pattern.nr_accesses[0].value,
+            'max': '%d' % pattern.nr_accesses[1].value,
         },
         'age': {
-            'min': '%d' % pattern.age[0],
-            'max': '%d' % pattern.age[1],
+            'min': '%d' % pattern.age[0].value,
+            'max': '%d' % pattern.age[1].value,
         },
     }
 
 def wops_for_schemes(ctx):
     schemes = ctx.schemes
 
     schemes_wops = {}
-    for scheme in schemes:
-        schemes_wops[scheme.name] = {
+    for idx, scheme in enumerate(schemes):
+        scheme_dir_name = '%d' % idx
+        schemes_wops[scheme_dir_name] = {
             'access_pattern': wops_for_scheme_access_pattern(
                 scheme.access_pattern, ctx),
             'action': scheme.action,
             'quotas': wops_for_scheme_quotas(scheme.quotas),
             'watermarks': wops_for_scheme_watermarks(scheme.watermarks),
         }
         if feature_supported('schemes_filters'):
-            schemes_wops[scheme.name]['filters'] = wops_for_scheme_filters(
+            schemes_wops[scheme_dir_name]['filters'] = wops_for_scheme_filters(
                     scheme.filters)
     return schemes_wops
 
 def wops_for_regions(regions):
     return {'%d' % region_idx: {
         'start': '%d' % region.start,
         'end': '%d' % region.end}
         for region_idx, region in enumerate(regions)}
 
 def wops_for_targets(ctx):
     return {
-            target.name: {
+            '%d' % idx: {
                 'pid_target': '%s' %
                 target.pid if _damon.target_has_pid(ctx.ops) else '',
                 'regions': wops_for_regions(target.regions)
-                } for target in ctx.targets}
+                } for idx, target in enumerate(ctx.targets)}
 
 def wops_for_monitoring_attrs(ctx):
     return {
         'intervals': {
             'sample_us': '%d' % ctx.intervals.sample,
             'aggr_us': '%d' % ctx.intervals.aggr,
             'update_us': '%d' % ctx.intervals.ops_update,
@@ -238,78 +202,87 @@
             {'operations': ops},
             {'monitoring_attrs': wops_for_monitoring_attrs(ctx)},
             {'targets': wops_for_targets(ctx)},
             {'schemes': wops_for_schemes(ctx)},
     ]
 
 def wops_for_ctxs(ctxs):
-    return {ctx.name: wops_for_ctx(ctx) for ctx in ctxs}
+    return {'%d' % idx: wops_for_ctx(ctx) for idx, ctx in enumerate(ctxs)}
 
 def wops_for_kdamond(kdamond):
     return {'contexts': wops_for_ctxs(kdamond.contexts)}
 
 def wops_for_kdamonds(kdamonds):
-    return {kdamond.name: wops_for_kdamond(kdamond) for kdamond in kdamonds}
+    return {'%d' % idx: wops_for_kdamond(kdamond)
+            for idx, kdamond in enumerate(kdamonds)}
+
+def __ensure_scheme_dir_populated(scheme_dir, scheme):
+    if not feature_supported('schemes_filters'):
+        return
 
-def __ensure_scheme_dir_populated(kdamond, ctx, scheme):
-    nr_filters, err = _damo_fs.read_file(
-            nr_filters_file_of(kdamond.name, ctx.name, scheme.name))
+    nr_filters_path = os.path.join(scheme_dir, 'filters', 'nr_filters')
+
+    nr_filters, err = _damo_fs.read_file(nr_filters_path)
     if err != None:
-        raise Exception('nr_fileters read fail (%s)' % err)
+        raise Exception('nr_filters read fail (%s)' % err)
     if int(nr_filters) != len(scheme.filters):
-        _damo_fs.write_file(
-                nr_filters_file_of(kdamond.name, ctx.name, scheme.name),
-                '%d' % len(scheme.filters))
-
-def __ensure_target_dir_populated(kdamond, ctx, target):
-    nr_regions, err = _damo_fs.read_file(
-            nr_regions_file_of(kdamond.name, ctx.name, target.name))
+        _damo_fs.write_file(nr_filters_path, '%d' % len(scheme.filters))
+
+def __ensure_target_dir_populated(target_dir, target):
+    nr_regions_path = os.path.join(target_dir, 'regions', 'nr_regions')
+    nr_regions, err = _damo_fs.read_file(nr_regions_path)
     if err != None:
         raise Exception('nr_regions read fail (%s)' % err)
     if int(nr_regions) != len(target.regions):
-        _damo_fs.write_file(
-                nr_regions_file_of(kdamond.name, ctx.name, target.name),
-                '%d' % len(target.regions))
+        _damo_fs.write_file(nr_regions_path, '%d' % len(target.regions))
 
-def __ensure_kdamond_dir_populated(kdamond):
-    nr_contexts, err = _damo_fs.read_file(nr_contexts_file_of(kdamond.name))
+def __ensure_kdamond_dir_populated(kdamond_dir, kdamond):
+    contexts_dir_path = os.path.join(kdamond_dir, 'contexts')
+    nr_contexts_path = os.path.join(kdamond_dir, 'contexts', 'nr_contexts')
+    nr_contexts, err = _damo_fs.read_file(nr_contexts_path)
     if err != None:
         raise Exception('kdamond name read fail (%s)' % err)
     if int(nr_contexts) != len(kdamond.contexts):
-        _damo_fs.write_file(nr_contexts_file_of(kdamond.name),
-                '%d' % len(kdamond.contexts))
-    for ctx in kdamond.contexts:
-        nr_targets, err = _damo_fs.read_file(
-                nr_targets_file_of(kdamond.name, ctx.name))
+        _damo_fs.write_file(nr_contexts_path, '%d' % len(kdamond.contexts))
+
+    for ctx_idx, ctx in enumerate(kdamond.contexts):
+        ctx_dir_path = os.path.join(contexts_dir_path, '%d' % ctx_idx)
+        targets_dir_path = os.path.join(ctx_dir_path, 'targets')
+        nr_targets_path = os.path.join(targets_dir_path, 'nr_targets')
+        nr_targets, err = _damo_fs.read_file(nr_targets_path)
         if err != None:
             raise Exception('nr_targets read fail (%s)' % err)
         if int(nr_targets) != len(ctx.targets):
-            _damo_fs.write_file(
-                    nr_targets_file_of(kdamond.name, ctx.name),
-                    '%d' % len(ctx.targets))
-        for target in ctx.targets:
-            __ensure_target_dir_populated(kdamond, ctx, target)
-        nr_schemes, err = _damo_fs.read_file(
-                nr_schemes_file_of(kdamond.name, ctx.name))
+            _damo_fs.write_file(nr_targets_path, '%d' % len(ctx.targets))
+
+        for target_idx, target in enumerate(ctx.targets):
+            target_dir_path = os.path.join(targets_dir_path, '%d' % target_idx)
+            __ensure_target_dir_populated(target_dir_path, target)
+
+        schemes_dir_path = os.path.join(ctx_dir_path, 'schemes')
+        nr_schemes_path = os.path.join(schemes_dir_path, 'nr_schemes')
+        nr_schemes, err = _damo_fs.read_file(nr_schemes_path)
         if err != None:
             raise Exception('nr_schemes read fail (%s)' % err)
         if int(nr_schemes) != len(ctx.schemes):
-            _damo_fs.write_file(nr_schemes_file_of(kdamond.name, ctx.name),
-                    '%d' % len(ctx.schemes))
-        for scheme in ctx.schemes:
-            __ensure_scheme_dir_populated(kdamond, ctx, scheme)
+            _damo_fs.write_file(nr_schemes_path, '%d' % len(ctx.schemes))
+
+        for scheme_idx, scheme in enumerate(ctx.schemes):
+            scheme_dir_path = os.path.join(schemes_dir_path, '%d' % scheme_idx)
+            __ensure_scheme_dir_populated(scheme_dir_path, scheme)
 
 def __ensure_dirs_populated_for(kdamonds):
     nr_kdamonds, err = _damo_fs.read_file(nr_kdamonds_file)
     if err != None:
         raise Exception('nr_kdamonds_file read fail (%s)' % err)
     if int(nr_kdamonds) != len(kdamonds):
         _damo_fs.write_file(nr_kdamonds_file, '%d' % len(kdamonds))
-    for kdamond in kdamonds:
-        __ensure_kdamond_dir_populated(kdamond)
+    for idx, kdamond in enumerate(kdamonds):
+        kdamond_dir = kdamond_dir_of('%d' % idx)
+        __ensure_kdamond_dir_populated(kdamond_dir, kdamond)
 
 def ensure_dirs_populated_for(kdamonds):
     try:
         __ensure_dirs_populated_for(kdamonds)
     except Exception as e:
         print('sysfs dirs population failed (%s)' % e)
         exit(1)
@@ -354,21 +327,20 @@
             int(files_content['interval_us']),
             int(files_content['high']),
             int(files_content['mid']),
             int(files_content['low']))
 
 def files_content_to_damos_filters(files_content):
     filters = []
-    for filter_name in files_content:
-        if filter_name == 'nr_filters':
+    for filter_dir_name in files_content:
+        if filter_dir_name == 'nr_filters':
             continue
-        filter_kv = files_content[filter_name]
-        filters.append(_damon.DamosFilter(filter_name,
-            filter_kv['type'].strip(), filter_kv['memcg_path'].strip(),
-            filter_kv['matching'].strip()))
+        filter_kv = files_content[filter_dir_name]
+        filters.append(_damon.DamosFilter(filter_kv['type'].strip(),
+            filter_kv['memcg_path'].strip(), filter_kv['matching'].strip()))
     return filters
 
 def files_content_to_damos_stats(files_content):
     return _damon.DamosStats(
             int(files_content['nr_tried']),
             int(files_content['sz_tried']),
             int(files_content['nr_applied']),
@@ -382,19 +354,20 @@
         nr_region_dirs -= 1
     for i in range(nr_region_dirs):
         regions.append(_damon.DamosTriedRegion(
             int(files_content['%d' % i]['start']),
             int(files_content['%d' % i]['end']),
             int(files_content['%d' % i]['nr_accesses']),
             int(files_content['%d' % i]['age']),
+            _damon.unit_aggr_intervals
             ))
     return regions
 
-def files_content_to_scheme(scheme_name, files_content):
-    return _damon.Damos(scheme_name,
+def files_content_to_scheme(files_content):
+    return _damon.Damos(
             files_content_to_access_pattern(files_content['access_pattern']),
             files_content['action'].strip(),
             files_content_to_quotas(files_content['quotas']),
             files_content_to_watermarks(files_content['watermarks']),
             files_content_to_damos_filters(files_content['filters'])
                 if 'filters' in files_content else [],
             files_content_to_damos_stats(files_content['stats']),
@@ -407,21 +380,21 @@
     for region_idx in range(int(files_content['nr_regions'])):
         region_name = '%d' % region_idx
         regions.append(_damon.DamonRegion(
             int(files_content[region_name]['start']),
             int(files_content[region_name]['end'])))
     return regions
 
-def files_content_to_target(target_name, files_content):
+def files_content_to_target(files_content):
     try:
         pid = int(files_content['pid_target'])
     except:
         pid = None
     regions = files_content_to_regions(files_content['regions'])
-    return _damon.DamonTarget(target_name, pid, regions)
+    return _damon.DamonTarget(pid, regions)
 
 def files_content_to_context(context_name, files_content):
     mon_attrs_content = files_content['monitoring_attrs']
     intervals_content = mon_attrs_content['intervals']
     intervals = _damon.DamonIntervals(
             int(intervals_content['sample_us']),
             int(intervals_content['aggr_us']),
@@ -430,50 +403,46 @@
     nr_regions = _damon.DamonNrRegionsRange(
             int(nr_regions_content['min']),
             int(nr_regions_content['max']))
     ops = files_content['operations'].strip()
 
     targets_content = files_content['targets']
     targets = []
-    for target_name in targets_content:
-        if target_name == 'nr_targets':
+    for target_dir_name, target_content in targets_content.items():
+        if target_dir_name == 'nr_targets':
             continue
-        targets.append(files_content_to_target(target_name,
-            targets_content[target_name]))
+        targets.append(files_content_to_target(target_content))
 
     schemes_content = files_content['schemes']
     schemes = []
-    for scheme_name in schemes_content:
+    for scheme_name, scheme_content in schemes_content.items():
         if scheme_name == 'nr_schemes':
             continue
-        schemes.append(files_content_to_scheme(scheme_name,
-            schemes_content[scheme_name]))
+        schemes.append(files_content_to_scheme(scheme_content))
 
-    return _damon.DamonCtx(context_name, intervals, nr_regions, ops, targets,
-            schemes)
+    return _damon.DamonCtx(intervals, nr_regions, ops, targets, schemes)
 
-def files_content_to_kdamond(kdamond_name, files_content):
+def files_content_to_kdamond(files_content):
     contexts_content = files_content['contexts']
     contexts = []
     for ctx_name in contexts_content:
         if ctx_name == 'nr_contexts':
             continue
         contexts.append(files_content_to_context(ctx_name,
             contexts_content[ctx_name]))
     state = files_content['state'].strip()
     pid = files_content['pid'].strip()
-    return _damon.Kdamond(kdamond_name, state, pid, contexts)
+    return _damon.Kdamond(state, pid, contexts)
 
 def files_content_to_kdamonds(files_contents):
     kdamonds = []
     for kdamond_name in files_contents:
         if kdamond_name == 'nr_kdamonds':
             continue
-        kdamonds.append(files_content_to_kdamond(
-            kdamond_name, files_contents[kdamond_name]))
+        kdamonds.append(files_content_to_kdamond(files_contents[kdamond_name]))
     return kdamonds
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(kdamonds_dir))
 
 def current_kdamond_names():
@@ -540,18 +509,18 @@
         return 'damon sysfs dir (%s) not found' % kdamonds_dir
     for feature in features_sysfs_support_from_begining:
         feature_supports[feature] = True
 
     orig_kdamonds = None
     if not os.path.isdir(scheme_dir_of(0, 0, 0)):
         orig_kdamonds = current_kdamonds()
-        kdamonds_for_feature_check = [_damon.Kdamond(name='0', state=None,
-            pid=None, contexts=[_damon.DamonCtx(name='0', intervals=None,
+        kdamonds_for_feature_check = [_damon.Kdamond(state=None,
+            pid=None, contexts=[_damon.DamonCtx(intervals=None,
                 nr_regions=None, ops=None, targets=[],
-                schemes=[_damon.Damos(name='0', access_pattern=None,
+                schemes=[_damon.Damos(access_pattern=None,
                     action='stat', quotas=None, watermarks=None, filters=[],
                     stats=None)])])]
         ensure_dirs_populated_for(kdamonds_for_feature_check)
 
     if os.path.isdir(scheme_tried_regions_dir_of(0, 0, 0)):
         feature_supports['schemes_tried_regions'] = True
```

### Comparing `damo-1.7.6/src/damo/damo.py` & `damo-1.7.7/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_adjust.py` & `damo-1.7.7/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_features.py` & `damo-1.7.7/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_fmt_json.py` & `damo-1.7.7/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_heats.py` & `damo-1.7.7/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_lru_sort.py` & `damo-1.7.7/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_monitor.py` & `damo-1.7.7/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_nr_regions.py` & `damo-1.7.7/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_reclaim.py` & `damo-1.7.7/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_record.py` & `damo-1.7.7/src/damo/damo_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,16 @@
     # Now the real works
     is_ongoing = _damon_args.is_ongoing_target(args)
     if not is_ongoing:
         err, kdamonds = _damon_args.turn_damon_on(args)
         if err:
             print('could not turn DAMON on (%s)' % err)
             cleanup_exit(-2)
-        data_for_cleanup.kdamonds_names = [k.name for k in kdamonds]
+        data_for_cleanup.kdamonds_names = ['%d' % idx
+                for idx, k in enumerate(kdamonds)]
 
     if not damon_record_supported or is_ongoing:
         data_for_cleanup.perf_pipe = _damon_result.start_monitoring_record(
                 data_for_cleanup.rfile_path, data_for_cleanup.rfile_format,
                 data_for_cleanup.rfile_permission)
     print('Press Ctrl+C to stop')
```

### Comparing `damo-1.7.6/src/damo/damo_report.py` & `damo-1.7.7/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_report_raw.py` & `damo-1.7.7/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_schemes.py` & `damo-1.7.7/src/damo/damo_schemes.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     signal.signal(signal.SIGTERM, sighandler)
 
     err, kdamonds = _damon_args.turn_damon_on(args)
     if err:
         print('could not turn DAMON on (%s)' % err)
         cleanup_exit(-3)
 
-    kdamonds_names = [k.name for k in kdamonds]
+    kdamonds_names = ['%d' % idx for idx, k in enumerate(kdamonds)]
 
     print('Press Ctrl+C to stop')
     if _damon_args.self_started_target(args):
         os.waitpid(kdamonds[0].contexts[0].targets[0].pid, 0)
     # damon will turn it off by itself if the target tasks are terminated.
     _damon.wait_current_kdamonds_turned_off()
```

### Comparing `damo-1.7.6/src/damo/damo_start.py` & `damo-1.7.7/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_stat.py` & `damo-1.7.7/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_stat_kdamonds.py` & `damo-1.7.7/src/damo/damo_stat_kdamonds.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     summary = [k.summary_str() for k in kdamonds]
     if json_format:
         print(json.dumps(summary, indent=4))
         return
     print('\n'.join(summary))
 
 def update_pr_kdamonds(json_format, raw_nr):
-    err = _damon.update_schemes_stats()
+    err = _damon.update_schemes_status()
     if err:
         print(err)
         return
     kdamonds = _damon.current_kdamonds()
     if json_format:
         print(json.dumps([k.to_kvpairs(raw_nr) for k in kdamonds], indent=4))
     else:
```

### Comparing `damo-1.7.6/src/damo/damo_stat_regions.py` & `damo-1.7.7/src/damo/damo_stat_regions.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,18 @@
         prio_weights, raw_nr):
 
     if sortby == 'priority':
         regions.sort(key=lambda region: priority(region, prio_weights))
 
     total_sz = 0
     for region in regions:
+        # region is DamonRegion.  Convert to DamosTriedRegion
         region = _damon.DamosTriedRegion(region.start, region.end,
-                region.nr_accesses, region.age)
+                region.nr_accesses, region.age / intervals.aggr,
+                _damon.unit_aggr_intervals)
         if not size_only:
             print(region.to_str(raw_nr, intervals))
         else:
             total_sz += (region.end - region.start)
     if size_only:
         print('%s' % _damo_fmt_str.format_sz(total_sz, raw_nr))
 
@@ -37,15 +39,16 @@
     snapshots, err = _damon_result.get_snapshots(access_pattern)
     if snapshots == None:
         print(err)
         return
 
     for kdamond, ctx_snapshots in snapshots.items():
         for ctx, snapshot in ctx_snapshots.items():
-            print('kdamond %s ctx %s' % (kdamond.name, ctx.name))
+            ctx_idx = kdamond.contexts.index(ctx)
+            print('kdamond %s ctx %s' % (kdamond.idx, ctx_idx))
             __pr_schemes_tried_regions(snapshot.regions, ctx.intervals,
                     size_only, sortby, prio_weights, raw_nr)
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
     parser.add_argument('--sz_region', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
```

### Comparing `damo-1.7.6/src/damo/damo_stat_schemes.py` & `damo-1.7.7/src/damo/damo_stat_schemes.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import _damo_subcmds
 import _damon
 
 def pr_schemes_tried_regions(kdamonds, raw_nr):
     print('# <kdamond> <context> <scheme>')
     print('# <regions>')
     print('# ...')
-    for kdamond in kdamonds:
-        for ctx in kdamond.contexts:
-            for scheme in ctx.schemes:
-                print('%s %s %s' % (kdamond.name, ctx.name, scheme.name))
+    for kd_idx, kdamond in enumerate(kdamonds):
+        for ctx_idx, ctx in enumerate(kdamond.contexts):
+            for scheme_idx, scheme in enumerate(ctx.schemes):
+                print('%s %s %s' % (kd_idx, ctx_idx, scheme_idx))
                 print('\n'.join(
                     r.to_str(raw_nr) for r in scheme.tried_regions))
 
 def update_pr_schemes_tried_regions(raw_nr):
     err = _damon.update_schemes_tried_regions()
     if err:
         print(err)
@@ -31,30 +31,30 @@
     err = _damon.update_schemes_stats()
     if err:
         print(err)
         return
     kdamonds = _damon.current_kdamonds()
 
     print('# <kdamond> <context> <scheme> <field> <value>')
-    for kdamond in kdamonds:
-        for ctx in kdamond.contexts:
-            for scheme in ctx.schemes:
-                print('%s %s %s %s %s' % (kdamond.name, ctx.name, scheme.name,
+    for kd_idx, kdamond in enumerate(kdamonds):
+        for ctx_idx, ctx in enumerate(kdamond.contexts):
+            for scheme_idx, scheme in enumerate(ctx.schemes):
+                print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'nr_tried', _damo_fmt_str.format_nr(
                         scheme.stats.nr_tried, raw_nr)))
-                print('%s %s %s %s %s' % (kdamond.name, ctx.name, scheme.name,
+                print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'sz_tried', _damo_fmt_str.format_sz(
                         scheme.stats.sz_tried, raw_nr)))
-                print('%s %s %s %s %s' % (kdamond.name, ctx.name, scheme.name,
+                print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'nr_applied', _damo_fmt_str.format_nr(
                         scheme.stats.nr_applied, raw_nr)))
-                print('%s %s %s %s %s' % (kdamond.name, ctx.name, scheme.name,
+                print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'sz_applied', _damo_fmt_str.format_sz(
                         scheme.stats.sz_applied, raw_nr)))
-                print('%s %s %s %s %s' % (kdamond.name, ctx.name, scheme.name,
+                print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'qt_exceeds', _damo_fmt_str.format_nr(
                         scheme.stats.qt_exceeds, raw_nr)))
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
 
 def __main(args):
```

### Comparing `damo-1.7.6/src/damo/damo_stop.py` & `damo-1.7.7/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_translate_damos.py` & `damo-1.7.7/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_tune.py` & `damo-1.7.7/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_validate.py` & `damo-1.7.7/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo/damo_wss.py` & `damo-1.7.7/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.6/src/damo.egg-info/PKG-INFO` & `damo-1.7.7/src/damo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.6
+Version: 1.7.7
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.6/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.7/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
```

### Comparing `damo-1.7.6/src/damo.egg-info/SOURCES.txt` & `damo-1.7.7/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

