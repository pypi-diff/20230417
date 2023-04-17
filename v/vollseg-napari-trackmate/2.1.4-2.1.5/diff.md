# Comparing `tmp/vollseg-napari-trackmate-2.1.4.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-ym3hr4tt/vollseg-napari-trackmate-2.1.4.tar", last modified: Sun Apr 16 18:33:10 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-fziz5mre/vollseg-napari-trackmate-2.1.5.tar", last modified: Mon Apr 17 16:09:32 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.1.4.tar` & `vollseg-napari-trackmate-2.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:10.013821 vollseg-napari-trackmate-2.1.4/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.574508 vollseg-napari-trackmate-2.1.4/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.863789 vollseg-napari-trackmate-2.1.4/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.945661 vollseg-napari-trackmate-2.1.4/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.4/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:33:10.015822 vollseg-napari-trackmate-2.1.4/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-16 18:33:10.023531 vollseg-napari-trackmate-2.1.4/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:08.604421 vollseg-napari-trackmate-2.1.4/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.366196 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.905729 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    90552 2023-04-16 18:32:01.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.963730 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:33:09.639610 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-16 18:33:08.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-16 18:33:06.000000 vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.4/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.823991 vollseg-napari-trackmate-2.1.5/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.281549 vollseg-napari-trackmate-2.1.5/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.567888 vollseg-napari-trackmate-2.1.5/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.649731 vollseg-napari-trackmate-2.1.5/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.5/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 16:09:32.825045 vollseg-napari-trackmate-2.1.5/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-17 16:09:32.834081 vollseg-napari-trackmate-2.1.5/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:31.303653 vollseg-napari-trackmate-2.1.5/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.099105 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.701047 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    91151 2023-04-17 16:08:32.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.771923 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 16:09:32.396173 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-17 16:09:31.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-17 16:09:29.000000 vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.5/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.1.4/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/.gitignore` & `vollseg-napari-trackmate-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.5/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/LICENSE` & `vollseg-napari-trackmate-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/PKG-INFO` & `vollseg-napari-trackmate-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.4
+Version: 2.1.5
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.4/README.md` & `vollseg-napari-trackmate-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/setup.cfg` & `vollseg-napari-trackmate-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1572,47 +1572,47 @@
 
             if key == track_model_type_dict[0]:
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
                 plot_ax.cla()
 
-                if model_selected_cloud_auto_encoder is not None:
-
-                    data_columns = ["Time", "Mitotic_Cluster_Class"]
-                    data = []
-
-                    for i in range(
-                        0,
-                        len(_trackmate_objects.mitotic_cluster_class),
-                        plugin_data.plot_step_size.value,
-                    ):
-                        time = _trackmate_objects.time[i]
-
-                        class_array = _trackmate_objects.mitotic_cluster_class[
-                            i
-                        ]
-                        for i in range(class_array.shape[0]):
-                            data.append([time, class_array[i]])
-                    clusters = pd.DataFrame(data, columns=data_columns)
-
-                    sns.violinplot(
-                        x="Time",
-                        y="Mitotic_Cluster_Class",
-                        data=clusters,
-                        ax=plot_ax,
-                    )
+                if _trackmate_objects.mitotic_cluster_class is not None:
+                    if len(_trackmate_objects.mitotic_cluster_class) > 0:
+                        data_columns = ["Time", "Mitotic_Cluster_Class"]
+                        data = []
+
+                        for i in range(
+                            0,
+                            len(_trackmate_objects.mitotic_cluster_class),
+                            plugin_data.plot_step_size.value,
+                        ):
+                            time = _trackmate_objects.time[i]
+
+                            class_array = (
+                                _trackmate_objects.mitotic_cluster_class[i]
+                            )
+                            for i in range(class_array.shape[0]):
+                                data.append([time, class_array[i]])
+                        clusters = pd.DataFrame(data, columns=data_columns)
+
+                        sns.violinplot(
+                            x="Time",
+                            y="Mitotic_Cluster_Class",
+                            data=clusters,
+                            ax=plot_ax,
+                        )
 
-                    plot_ax.set_xticklabels([])
+                        plot_ax.set_xticklabels([])
 
-                    plot_ax.set_xlabel("Time (min)")
-                    plot_ax.set_ylabel("Class")
+                        plot_ax.set_xlabel("Time (min)")
+                        plot_ax.set_ylabel("Class")
 
-                    stat_plot_class._repeat_after_plot()
-                    plot_ax = stat_plot_class.plot_ax
+                        stat_plot_class._repeat_after_plot()
+                        plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
                     _trackmate_objects.mitotic_mean_distance_cell_mask,
                     _trackmate_objects.mitotic_var_distance_cell_mask,
                     linestyle="None",
                     marker=".",
@@ -1740,45 +1740,47 @@
 
             if key == track_model_type_dict[1]:
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
                 plot_ax.cla()
 
-                if model_selected_cloud_auto_encoder is not None:
+                if _trackmate_objects.non_mitotic_cluster_class is not None:
 
-                    data_columns = ["Time", "Non_Mitotic_Cluster_Class"]
-                    data = []
+                    if len(_trackmate_objects.non_mitotic_cluster_class) > 0:
 
-                    for i in range(
-                        0,
-                        len(_trackmate_objects.non_mitotic_cluster_class),
-                        plugin_data.plot_step_size.value,
-                    ):
-                        time = _trackmate_objects.time[i]
+                        data_columns = ["Time", "Non_Mitotic_Cluster_Class"]
+                        data = []
 
-                        class_array = (
-                            _trackmate_objects.non_mitotic_cluster_class[i]
+                        for i in range(
+                            0,
+                            len(_trackmate_objects.non_mitotic_cluster_class),
+                            plugin_data.plot_step_size.value,
+                        ):
+                            time = _trackmate_objects.time[i]
+
+                            class_array = (
+                                _trackmate_objects.non_mitotic_cluster_class[i]
+                            )
+                            for i in range(class_array.shape[0]):
+                                data.append([time, class_array[i]])
+                        clusters = pd.DataFrame(data, columns=data_columns)
+                        sns.violinplot(
+                            x="Time",
+                            y="Non_Mitotic_Cluster_Class",
+                            data=clusters,
+                            ax=plot_ax,
                         )
-                        for i in range(class_array.shape[0]):
-                            data.append([time, class_array[i]])
-                    clusters = pd.DataFrame(data, columns=data_columns)
-                    sns.violinplot(
-                        x="Time",
-                        y="Non_Mitotic_Cluster_Class",
-                        data=clusters,
-                        ax=plot_ax,
-                    )
-
-                    plot_ax.set_xticklabels([])
-                    plot_ax.set_xlabel("Time (min)")
-                    plot_ax.set_ylabel("Class")
 
-                    stat_plot_class._repeat_after_plot()
-                    plot_ax = stat_plot_class.plot_ax
+                        plot_ax.set_xticklabels([])
+                        plot_ax.set_xlabel("Time (min)")
+                        plot_ax.set_ylabel("Class")
+
+                        stat_plot_class._repeat_after_plot()
+                        plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
                     _trackmate_objects.non_mitotic_mean_distance_cell_mask,
                     _trackmate_objects.non_mitotic_var_distance_cell_mask,
                     linestyle="None",
                     marker=".",
@@ -1906,42 +1908,45 @@
 
             if key == track_model_type_dict[2]:
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
                 plot_ax.cla()
 
-                if model_selected_cloud_auto_encoder is not None:
+                if _trackmate_objects.all_cluster_class is not None:
+                    if len(_trackmate_objects.all_cluster_class) > 0:
 
-                    data_columns = ["Time", "All_CellType_Cluster_Class"]
-                    data = []
+                        data_columns = ["Time", "All_CellType_Cluster_Class"]
+                        data = []
 
-                    for i in range(
-                        0,
-                        len(_trackmate_objects.all_cluster_class),
-                        plugin_data.plot_step_size.value,
-                    ):
-                        time = _trackmate_objects.time[i]
-
-                        class_array = _trackmate_objects.all_cluster_class[i]
-                        for i in range(class_array.shape[0]):
-                            data.append([time, class_array[i]])
-                    clusters = pd.DataFrame(data, columns=data_columns)
-                    sns.violinplot(
-                        x="Time",
-                        y="All_CellType_Cluster_Class",
-                        data=clusters,
-                        ax=plot_ax,
-                    )
-                    plot_ax.set_xticklabels([])
-                    plot_ax.set_xlabel("Time (min)")
-                    plot_ax.set_ylabel("Class")
+                        for i in range(
+                            0,
+                            len(_trackmate_objects.all_cluster_class),
+                            plugin_data.plot_step_size.value,
+                        ):
+                            time = _trackmate_objects.time[i]
+
+                            class_array = _trackmate_objects.all_cluster_class[
+                                i
+                            ]
+                            for i in range(class_array.shape[0]):
+                                data.append([time, class_array[i]])
+                        clusters = pd.DataFrame(data, columns=data_columns)
+                        sns.violinplot(
+                            x="Time",
+                            y="All_CellType_Cluster_Class",
+                            data=clusters,
+                            ax=plot_ax,
+                        )
+                        plot_ax.set_xticklabels([])
+                        plot_ax.set_xlabel("Time (min)")
+                        plot_ax.set_ylabel("Class")
 
-                    stat_plot_class._repeat_after_plot()
-                    plot_ax = stat_plot_class.plot_ax
+                        stat_plot_class._repeat_after_plot()
+                        plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
                     _trackmate_objects.all_mean_distance_cell_mask,
                     _trackmate_objects.all_var_distance_cell_mask,
                     linestyle="None",
                     marker=".",
```

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.4
+Version: 2.1.5
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.4/tox.ini` & `vollseg-napari-trackmate-2.1.5/tox.ini`

 * *Files identical despite different names*

