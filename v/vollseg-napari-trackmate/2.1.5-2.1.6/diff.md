# Comparing `tmp/vollseg-napari-trackmate-2.1.5.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-fziz5mre/vollseg-napari-trackmate-2.1.5.tar", last modified: Mon Apr 17 16:09:32 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-f__uuw0u/vollseg-napari-trackmate-2.1.6.tar", last modified: Mon Apr 17 16:20:16 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.1.5.tar` & `vollseg-napari-trackmate-2.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.823991 vollseg-napari-trackmate-2.1.5/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.281549 vollseg-napari-trackmate-2.1.5/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.567888 vollseg-napari-trackmate-2.1.5/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.649731 vollseg-napari-trackmate-2.1.5/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.5/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 16:09:32.825045 vollseg-napari-trackmate-2.1.5/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-17 16:09:32.834081 vollseg-napari-trackmate-2.1.5/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.303653 vollseg-napari-trackmate-2.1.5/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.099105 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.701047 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    91151 2023-04-17 16:08:32.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.771923 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.396173 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-17 16:09:31.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:16.523845 vollseg-napari-trackmate-2.1.6/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:14.807767 vollseg-napari-trackmate-2.1.6/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:15.183614 vollseg-napari-trackmate-2.1.6/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:15.262215 vollseg-napari-trackmate-2.1.6/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.6/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 16:20:16.526844 vollseg-napari-trackmate-2.1.6/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-17 16:20:16.537016 vollseg-napari-trackmate-2.1.6/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:14.843829 vollseg-napari-trackmate-2.1.6/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:15.734826 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:16.388502 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-17 16:20:12.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    92928 2023-04-17 16:19:36.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:16.464809 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:20:16.064021 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 16:20:12.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-17 16:20:14.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-17 16:20:12.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-17 16:20:12.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-17 16:20:12.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-17 16:20:12.000000 vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.6/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.1.5/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/.gitignore` & `vollseg-napari-trackmate-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.6/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/LICENSE` & `vollseg-napari-trackmate-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/PKG-INFO` & `vollseg-napari-trackmate-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.5
+Version: 2.1.6
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.5/README.md` & `vollseg-napari-trackmate-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/setup.cfg` & `vollseg-napari-trackmate-2.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1179,191 +1179,207 @@
                                         global_data_cluster_plot,
                                         data_cluster_plot,
                                     ],
                                     ignore_index=True,
                                 )
 
             if len(_to_analyze) <= 2:
-
+                flatui = ["#9b59b6", "#3498db", "orange"]
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Speed",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Speed")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Motion Angle",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Motion Angle")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Radial Angle",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Radial Angle")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Acceleration",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Acceleration")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Distance cell to tissue",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Distance cell to tissue")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Cell Axis Mask",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Cell Axis Mask")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Radius",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Radius")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Volume",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Volume")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Surface_Area",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Surface_Area")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_First",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Eccentricity Comp First")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
-
+                sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_Second",
                     hue="id",
                     ax=plot_ax,
+                    legend=False,
                 )
 
                 plot_ax.set_title("Eccentricity Comp Second")
                 plot_ax.set_xlabel("Time (min)")
-
+                sns.move_legend(plot_ax, "lower right")
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 if not global_data_cluster_plot["Class"].isna().all():
                     if size_catagories_json is None:
+                        sns.set_palette(flatui)
                         sns.lineplot(
                             global_data_cluster_plot,
                             x="Time",
                             y="Class",
                             hue="id",
                             ax=plot_ax,
+                            legend=False,
                         )
 
                     if size_catagories_json is not None:
+                        sns.set_palette(flatui)
                         sns.lineplot(
                             global_data_cluster_plot,
                             x="Time",
                             y="Class_Name",
                             hue="id",
                             ax=plot_ax,
+                            legend=False,
                         )
 
                     plot_ax.set_title("Cluster class")
                     plot_ax.set_xlabel("Time (min)")
-
+                    sns.move_legend(plot_ax, "lower right")
                     phenotype_plot_class._repeat_after_plot()
                     plot_ax = phenotype_plot_class.plot_ax
 
             data_fft_plot = pd.DataFrame(
                 {
                     "Frequ": unique_fft_properties[0][2],
                     "Amplitude": np.sum(unique_fft_properties, axis=0)[3],
@@ -1373,22 +1389,24 @@
             data_time_plot = pd.DataFrame(
                 {
                     "Time": unique_fft_properties[0][0],
                     "Intensity": np.sum(unique_fft_properties, axis=0)[1],
                 }
             )
 
+            sns.set_palette(flatui)
             sns.lineplot(data_time_plot, x="Time", y="Intensity", ax=plot_ax)
             plot_ax.set_title("Cell Intensity")
             plot_ax.set_xlabel("Time (min)")
             plot_ax.set_ylabel("Amplitude")
 
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
 
+            sns.set_palette(flatui)
             sns.lineplot(data_fft_plot, x="Frequ", y="Amplitude", ax=plot_ax)
             plot_ax.set_title("FFT Intensity")
             plot_ax.set_xlabel("Frequency (1/min)")
             plot_ax.set_ylabel("Amplitude")
 
     def return_color_tracks(pred):
```

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.5
+Version: 2.1.6
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.5/tox.ini` & `vollseg-napari-trackmate-2.1.6/tox.ini`

 * *Files identical despite different names*

