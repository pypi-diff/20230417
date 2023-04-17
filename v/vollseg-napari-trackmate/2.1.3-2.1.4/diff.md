# Comparing `tmp/vollseg-napari-trackmate-2.1.3.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-448mda73/vollseg-napari-trackmate-2.1.3.tar", last modified: Sun Apr 16 18:26:27 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-ym3hr4tt/vollseg-napari-trackmate-2.1.4.tar", last modified: Sun Apr 16 18:33:10 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.1.3.tar` & `vollseg-napari-trackmate-2.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:27.409666 vollseg-napari-trackmate-2.1.3/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:25.976448 vollseg-napari-trackmate-2.1.3/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:26.235762 vollseg-napari-trackmate-2.1.3/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:26.319348 vollseg-napari-trackmate-2.1.3/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.3/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:26:27.411675 vollseg-napari-trackmate-2.1.3/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-16 18:26:27.422676 vollseg-napari-trackmate-2.1.3/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:25.999449 vollseg-napari-trackmate-2.1.3/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:26.718994 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:27.296182 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-16 18:26:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    90665 2023-04-16 18:25:34.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:27.355797 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:26:27.005304 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:26:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-16 18:26:25.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-16 18:26:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-16 18:26:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-16 18:26:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-16 18:26:24.000000 vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.3/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:10.013821 vollseg-napari-trackmate-2.1.4/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.574508 vollseg-napari-trackmate-2.1.4/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.863789 vollseg-napari-trackmate-2.1.4/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.945661 vollseg-napari-trackmate-2.1.4/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.4/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:33:10.015822 vollseg-napari-trackmate-2.1.4/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-16 18:33:10.023531 vollseg-napari-trackmate-2.1.4/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.604421 vollseg-napari-trackmate-2.1.4/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.366196 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.905729 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    90552 2023-04-16 18:32:01.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.963730 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.639610 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-16 18:33:08.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.1.3/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/.gitignore` & `vollseg-napari-trackmate-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.4/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/LICENSE` & `vollseg-napari-trackmate-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/PKG-INFO` & `vollseg-napari-trackmate-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.3
+Version: 2.1.4
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.3/README.md` & `vollseg-napari-trackmate-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/setup.cfg` & `vollseg-napari-trackmate-2.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1163,15 +1163,15 @@
                                         "Radius": cluster_radius,
                                         "Volume": cluster_volume,
                                         "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
                                         "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                         "Surface_Area": cluster_surface_area,
                                         "Class": cluster_class,
                                         "Class_Score": cluster_class_score,
-                                        "cluster_id": cluster_id,
+                                        "id": cluster_id,
                                     }
                                 )
 
                             if len(global_data_cluster_plot) == 0:
                                 global_data_cluster_plot = data_cluster_plot
                             else:
                                 global_data_cluster_plot = pd.concat(
@@ -1180,155 +1180,155 @@
                                         data_cluster_plot,
                                     ],
                                     ignore_index=True,
                                 )
 
             if len(_to_analyze) <= 2:
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Speed",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Speed")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Motion Angle",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Motion Angle")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Radial Angle",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Radial Angle")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Acceleration",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Acceleration")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Distance cell to tissue",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Distance cell to tissue")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Cell Axis Mask",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Cell Axis Mask")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Radius",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Radius")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Volume",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Volume")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Surface_Area",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Surface_Area")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_First",
                     hue="id",
                     ax=plot_ax,
                 )
 
                 plot_ax.set_title("Eccentricity Comp First")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.scatterplot(
+                sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_Second",
                     hue="id",
                     ax=plot_ax,
                 )
 
@@ -1336,24 +1336,24 @@
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 if not global_data_cluster_plot["Class"].isna().all():
                     if size_catagories_json is None:
-                        sns.scatterplot(
+                        sns.lineplot(
                             global_data_cluster_plot,
                             x="Time",
                             y="Class",
                             hue="id",
                             ax=plot_ax,
                         )
 
                     if size_catagories_json is not None:
-                        sns.scatterplot(
+                        sns.lineplot(
                             global_data_cluster_plot,
                             x="Time",
                             y="Class_Name",
                             hue="id",
                             ax=plot_ax,
                         )
 
@@ -1373,27 +1373,23 @@
             data_time_plot = pd.DataFrame(
                 {
                     "Time": unique_fft_properties[0][0],
                     "Intensity": np.sum(unique_fft_properties, axis=0)[1],
                 }
             )
 
-            sns.scatterplot(
-                data_time_plot, x="Time", y="Intensity", ax=plot_ax
-            )
+            sns.lineplot(data_time_plot, x="Time", y="Intensity", ax=plot_ax)
             plot_ax.set_title("Cell Intensity")
             plot_ax.set_xlabel("Time (min)")
             plot_ax.set_ylabel("Amplitude")
 
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
 
-            sns.scatterplot(
-                data_fft_plot, x="Frequ", y="Amplitude", ax=plot_ax
-            )
+            sns.lineplot(data_fft_plot, x="Frequ", y="Amplitude", ax=plot_ax)
             plot_ax.set_title("FFT Intensity")
             plot_ax.set_xlabel("Frequency (1/min)")
             plot_ax.set_ylabel("Amplitude")
 
     def return_color_tracks(pred):
 
         if not isinstance(pred, int):
```

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.3
+Version: 2.1.4
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.3/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.3/tox.ini` & `vollseg-napari-trackmate-2.1.4/tox.ini`

 * *Files identical despite different names*

