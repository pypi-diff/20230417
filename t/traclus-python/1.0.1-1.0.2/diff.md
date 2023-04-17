# Comparing `tmp/traclus-python-1.0.1.tar.gz` & `tmp/traclus-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traclus-python-1.0.1.tar", last modified: Sun Mar 26 07:25:18 2023, max compression
+gzip compressed data, was "traclus-python-1.0.2.tar", last modified: Mon Apr 17 04:04:08 2023, max compression
```

## Comparing `traclus-python-1.0.1.tar` & `traclus-python-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-03-26 07:25:18.145201 traclus-python-1.0.1/
--rw-r--r--   0 adrielamoguis   (501) staff       (20)    11357 2023-02-13 07:56:26.000000 traclus-python-1.0.1/LICENSE
--rw-r--r--   0 adrielamoguis   (501) staff       (20)     5594 2023-03-26 07:25:18.145393 traclus-python-1.0.1/PKG-INFO
--rw-r--r--   0 adrielamoguis   (501) staff       (20)     5293 2023-03-19 15:40:40.000000 traclus-python-1.0.1/README.md
--rw-r--r--   0 adrielamoguis   (501) staff       (20)      103 2023-03-26 07:25:18.145652 traclus-python-1.0.1/setup.cfg
--rw-r--r--   0 adrielamoguis   (501) staff       (20)      545 2023-03-26 07:23:11.000000 traclus-python-1.0.1/setup.py
-drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-03-26 07:25:18.142234 traclus-python-1.0.1/src/
-drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-03-26 07:25:18.143358 traclus-python-1.0.1/src/traclus/
--rw-r--r--   0 adrielamoguis   (501) staff       (20)        0 2023-03-26 07:24:35.000000 traclus-python-1.0.1/src/traclus/__init__.py
--rw-r--r--   0 adrielamoguis   (501) staff       (20)    21700 2023-03-26 06:41:34.000000 traclus-python-1.0.1/src/traclus/traclus.py
-drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-03-26 07:25:18.145061 traclus-python-1.0.1/src/traclus_python.egg-info/
--rw-r--r--   0 adrielamoguis   (501) staff       (20)     5594 2023-03-26 07:25:18.000000 traclus-python-1.0.1/src/traclus_python.egg-info/PKG-INFO
--rw-r--r--   0 adrielamoguis   (501) staff       (20)      292 2023-03-26 07:25:18.000000 traclus-python-1.0.1/src/traclus_python.egg-info/SOURCES.txt
--rw-r--r--   0 adrielamoguis   (501) staff       (20)        1 2023-03-26 07:25:18.000000 traclus-python-1.0.1/src/traclus_python.egg-info/dependency_links.txt
--rw-r--r--   0 adrielamoguis   (501) staff       (20)       19 2023-03-26 07:25:18.000000 traclus-python-1.0.1/src/traclus_python.egg-info/requires.txt
--rw-r--r--   0 adrielamoguis   (501) staff       (20)        8 2023-03-26 07:25:18.000000 traclus-python-1.0.1/src/traclus_python.egg-info/top_level.txt
+drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-04-17 04:04:08.563896 traclus-python-1.0.2/
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)    11357 2023-02-13 07:56:26.000000 traclus-python-1.0.2/LICENSE
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)     5640 2023-04-17 04:04:08.563963 traclus-python-1.0.2/PKG-INFO
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)     5339 2023-03-26 07:34:11.000000 traclus-python-1.0.2/README.md
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)      103 2023-04-17 04:04:08.564202 traclus-python-1.0.2/setup.cfg
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)      545 2023-04-17 04:03:45.000000 traclus-python-1.0.2/setup.py
+drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-04-17 04:04:08.561493 traclus-python-1.0.2/src/
+drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-04-17 04:04:08.562577 traclus-python-1.0.2/src/traclus/
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)        0 2023-03-26 07:24:35.000000 traclus-python-1.0.2/src/traclus/__init__.py
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)    21736 2023-04-17 04:00:21.000000 traclus-python-1.0.2/src/traclus/traclus.py
+drwxr-xr-x   0 adrielamoguis   (501) staff       (20)        0 2023-04-17 04:04:08.563728 traclus-python-1.0.2/src/traclus_python.egg-info/
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)     5640 2023-04-17 04:04:08.000000 traclus-python-1.0.2/src/traclus_python.egg-info/PKG-INFO
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)      292 2023-04-17 04:04:08.000000 traclus-python-1.0.2/src/traclus_python.egg-info/SOURCES.txt
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)        1 2023-04-17 04:04:08.000000 traclus-python-1.0.2/src/traclus_python.egg-info/dependency_links.txt
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)       19 2023-04-17 04:04:08.000000 traclus-python-1.0.2/src/traclus_python.egg-info/requires.txt
+-rw-r--r--   0 adrielamoguis   (501) staff       (20)        8 2023-04-17 04:04:08.000000 traclus-python-1.0.2/src/traclus_python.egg-info/top_level.txt
```

### Comparing `traclus-python-1.0.1/LICENSE` & `traclus-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `traclus-python-1.0.1/PKG-INFO` & `traclus-python-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traclus-python
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/AdrielAmoguis/TRACLUS
 Author: Adriel Isaiah Amoguis
 Author-email: adriel.isaiah.amoguis@gmail.com
 License: apache-2.0
 Keywords: Trajectory Clustering
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,25 +30,25 @@
 ---
 
 ## Installation
 
 This implementation requires Python 3.6 or higher. It is recommended to use a virtual environment to avoid
 dependency conflicts.
 
-Create a Conda Virtual Environment:
+Optionally, create a Conda Virtual Environment:
 
 ```bash
 conda create -n traclus python=3.6
 conda activate traclus
 ```
 
-Install the dependencies:
+Install the package from pip:
 
 ```bash
-pip install -r requirements.txt
+pip install traclus-python==1.0.1
 ```
 
 ---
 
 ## Usage
 
 ### Preparing Your Trajectory Data
@@ -64,21 +64,21 @@
 ```
 
 where `x` is the x-coordinate, and `y` is the y-coordinate for each point `n`.
 
 ### Running the Algorithm in Your Own Script File
 
 ```python
-from traclus import traclus
+from traclus import traclus as tr
 
 # Your Trajectory Data
 trajectories = ...
 
 # Run the TRACLUS Algorithm
-partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories)
+partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = tr.traclus(trajectories)
 ```
 
 The `partitions` variable will contain all the trajectories that are partitioned by the algorithm into their characteristic points (cp).
 The `segments` variable will contain all the generated partitions split into segments.
 The `dist_matrix` variable will contain the distance matrix generated by the distance function as defined in the paper.
 The `clusters` variable will contain the line segment clusters generated by the algorithm.
 The `cluster_assignments` variable will contain the cluster assignments for each line segment.
@@ -99,44 +99,44 @@
 ```
 
 Additionally, the _Perpendicular Distance_ is computed differently depending on whether or not the trajectories are direction-sensitive.
 Trajectories are treated as directional by default, but this can be changed by providing the `directional` parameter to the `traclus` function.
 Such as:
 
 ```python
-partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories, directional=False)
+partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = tr.traclus(trajectories, directional=False)
 ```
 
 ### Clustering Parameters
 
 The `traclus` function takes in a `clustering_algorithm` parameter that can be used to specify the clustering algorithm to use. This is set to
 DBSCAN from Scipy by default. The `traclus` function also accepts two parameters for DBSCAN: `eps` and `min_samples`. These are set to 1 and 10 by default.
 
 ### Supporting Functions
 
 The `sub_sample_trajectory` function can be used to sub-sample a trajectory into a trajectory of the same profile but with lesser points.
 It takes `sample_n` as a parameter, which is the number of points to sub-sample the trajectory into.
 
 ```python
 
-from traclus import sub_sample_trajectory
+from traclus.traclus import sub_sample_trajectory
 
 # Your Trajectory Data
 trajectories = ...
 
 # Sub-Sample the Trajectories
 sub_sampled_trajectories = [sub_sample_trajectory(trajectory, sample_n=100) for trajectory in trajectories]
 ```
 
 In the example above, the trajectories will be sub-sampled into 100 points each. This is useful for reducing the number of points processed by the algorithm, decreasing its runtime. However, this may also reduce the accuracy of the results. It is recommended to experiment with different values of `sample_n` to find the best value for your use-case.
 
 The `smooth_trajectory` function can be used to smooth the representative trajectories generated by the algorithm.
 
 ```python
-from traclus import traclus, smooth_trajectory
+from traclus.traclus import traclus, smooth_trajectory
 
 # Your Trajectory Data
 trajectories = ...
 
 # Run the TRACLUS Algorithm
 partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories)
```

### Comparing `traclus-python-1.0.1/README.md` & `traclus-python-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 ---
 
 ## Installation
 
 This implementation requires Python 3.6 or higher. It is recommended to use a virtual environment to avoid
 dependency conflicts.
 
-Create a Conda Virtual Environment:
+Optionally, create a Conda Virtual Environment:
 
 ```bash
 conda create -n traclus python=3.6
 conda activate traclus
 ```
 
-Install the dependencies:
+Install the package from pip:
 
 ```bash
-pip install -r requirements.txt
+pip install traclus-python==1.0.1
 ```
 
 ---
 
 ## Usage
 
 ### Preparing Your Trajectory Data
@@ -53,21 +53,21 @@
 ```
 
 where `x` is the x-coordinate, and `y` is the y-coordinate for each point `n`.
 
 ### Running the Algorithm in Your Own Script File
 
 ```python
-from traclus import traclus
+from traclus import traclus as tr
 
 # Your Trajectory Data
 trajectories = ...
 
 # Run the TRACLUS Algorithm
-partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories)
+partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = tr.traclus(trajectories)
 ```
 
 The `partitions` variable will contain all the trajectories that are partitioned by the algorithm into their characteristic points (cp).
 The `segments` variable will contain all the generated partitions split into segments.
 The `dist_matrix` variable will contain the distance matrix generated by the distance function as defined in the paper.
 The `clusters` variable will contain the line segment clusters generated by the algorithm.
 The `cluster_assignments` variable will contain the cluster assignments for each line segment.
@@ -88,44 +88,44 @@
 ```
 
 Additionally, the _Perpendicular Distance_ is computed differently depending on whether or not the trajectories are direction-sensitive.
 Trajectories are treated as directional by default, but this can be changed by providing the `directional` parameter to the `traclus` function.
 Such as:
 
 ```python
-partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories, directional=False)
+partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = tr.traclus(trajectories, directional=False)
 ```
 
 ### Clustering Parameters
 
 The `traclus` function takes in a `clustering_algorithm` parameter that can be used to specify the clustering algorithm to use. This is set to
 DBSCAN from Scipy by default. The `traclus` function also accepts two parameters for DBSCAN: `eps` and `min_samples`. These are set to 1 and 10 by default.
 
 ### Supporting Functions
 
 The `sub_sample_trajectory` function can be used to sub-sample a trajectory into a trajectory of the same profile but with lesser points.
 It takes `sample_n` as a parameter, which is the number of points to sub-sample the trajectory into.
 
 ```python
 
-from traclus import sub_sample_trajectory
+from traclus.traclus import sub_sample_trajectory
 
 # Your Trajectory Data
 trajectories = ...
 
 # Sub-Sample the Trajectories
 sub_sampled_trajectories = [sub_sample_trajectory(trajectory, sample_n=100) for trajectory in trajectories]
 ```
 
 In the example above, the trajectories will be sub-sampled into 100 points each. This is useful for reducing the number of points processed by the algorithm, decreasing its runtime. However, this may also reduce the accuracy of the results. It is recommended to experiment with different values of `sample_n` to find the best value for your use-case.
 
 The `smooth_trajectory` function can be used to smooth the representative trajectories generated by the algorithm.
 
 ```python
-from traclus import traclus, smooth_trajectory
+from traclus.traclus import traclus, smooth_trajectory
 
 # Your Trajectory Data
 trajectories = ...
 
 # Run the TRACLUS Algorithm
 partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories)
```

### Comparing `traclus-python-1.0.1/setup.py` & `traclus-python-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='traclus-python',
-    version='1.0.1',
+    version='1.0.2',
     license='apache-2.0',
     author="Adriel Isaiah Amoguis",
     author_email='adriel.isaiah.amoguis@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/AdrielAmoguis/TRACLUS',
     keywords='Trajectory Clustering',
```

### Comparing `traclus-python-1.0.1/src/traclus/traclus.py` & `traclus-python-1.0.2/src/traclus/traclus.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,16 @@
 # Minimum Description Length
 def minimum_desription_length(start_idx, curr_idx, trajectory, w_angular=1, w_perpendicular=1, par=True, directional=True):
     """
         Calculate the minimum description length.
     """
     LH = LDH = 0
     for i in range(start_idx, curr_idx-1):
-        LH += np.log2(d_euclidean(trajectory[i], trajectory[i+1]))
+        ed = d_euclidean(trajectory[i], trajectory[i+1])
+        LH += max(0, np.log2(ed, where=ed>0))
         if par:
             for j in range(start_idx, i-1):
                 # print()
                 # print(np.array([trajectory[start_idx], trajectory[i]]))
                 # print(np.array([trajectory[j], trajectory[j+1]]))
                 LDH += w_perpendicular * d_perpendicular(np.array([trajectory[start_idx], trajectory[i]]), np.array([trajectory[j], trajectory[j+1]]))
                 LDH += w_angular * d_angular(np.array([trajectory[start_idx], trajectory[i]]), np.array([trajectory[j], trajectory[j+1]]), directional=directional)
```

### Comparing `traclus-python-1.0.1/src/traclus_python.egg-info/PKG-INFO` & `traclus-python-1.0.2/src/traclus_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traclus-python
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/AdrielAmoguis/TRACLUS
 Author: Adriel Isaiah Amoguis
 Author-email: adriel.isaiah.amoguis@gmail.com
 License: apache-2.0
 Keywords: Trajectory Clustering
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,25 +30,25 @@
 ---
 
 ## Installation
 
 This implementation requires Python 3.6 or higher. It is recommended to use a virtual environment to avoid
 dependency conflicts.
 
-Create a Conda Virtual Environment:
+Optionally, create a Conda Virtual Environment:
 
 ```bash
 conda create -n traclus python=3.6
 conda activate traclus
 ```
 
-Install the dependencies:
+Install the package from pip:
 
 ```bash
-pip install -r requirements.txt
+pip install traclus-python==1.0.1
 ```
 
 ---
 
 ## Usage
 
 ### Preparing Your Trajectory Data
@@ -64,21 +64,21 @@
 ```
 
 where `x` is the x-coordinate, and `y` is the y-coordinate for each point `n`.
 
 ### Running the Algorithm in Your Own Script File
 
 ```python
-from traclus import traclus
+from traclus import traclus as tr
 
 # Your Trajectory Data
 trajectories = ...
 
 # Run the TRACLUS Algorithm
-partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories)
+partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = tr.traclus(trajectories)
 ```
 
 The `partitions` variable will contain all the trajectories that are partitioned by the algorithm into their characteristic points (cp).
 The `segments` variable will contain all the generated partitions split into segments.
 The `dist_matrix` variable will contain the distance matrix generated by the distance function as defined in the paper.
 The `clusters` variable will contain the line segment clusters generated by the algorithm.
 The `cluster_assignments` variable will contain the cluster assignments for each line segment.
@@ -99,44 +99,44 @@
 ```
 
 Additionally, the _Perpendicular Distance_ is computed differently depending on whether or not the trajectories are direction-sensitive.
 Trajectories are treated as directional by default, but this can be changed by providing the `directional` parameter to the `traclus` function.
 Such as:
 
 ```python
-partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories, directional=False)
+partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = tr.traclus(trajectories, directional=False)
 ```
 
 ### Clustering Parameters
 
 The `traclus` function takes in a `clustering_algorithm` parameter that can be used to specify the clustering algorithm to use. This is set to
 DBSCAN from Scipy by default. The `traclus` function also accepts two parameters for DBSCAN: `eps` and `min_samples`. These are set to 1 and 10 by default.
 
 ### Supporting Functions
 
 The `sub_sample_trajectory` function can be used to sub-sample a trajectory into a trajectory of the same profile but with lesser points.
 It takes `sample_n` as a parameter, which is the number of points to sub-sample the trajectory into.
 
 ```python
 
-from traclus import sub_sample_trajectory
+from traclus.traclus import sub_sample_trajectory
 
 # Your Trajectory Data
 trajectories = ...
 
 # Sub-Sample the Trajectories
 sub_sampled_trajectories = [sub_sample_trajectory(trajectory, sample_n=100) for trajectory in trajectories]
 ```
 
 In the example above, the trajectories will be sub-sampled into 100 points each. This is useful for reducing the number of points processed by the algorithm, decreasing its runtime. However, this may also reduce the accuracy of the results. It is recommended to experiment with different values of `sample_n` to find the best value for your use-case.
 
 The `smooth_trajectory` function can be used to smooth the representative trajectories generated by the algorithm.
 
 ```python
-from traclus import traclus, smooth_trajectory
+from traclus.traclus import traclus, smooth_trajectory
 
 # Your Trajectory Data
 trajectories = ...
 
 # Run the TRACLUS Algorithm
 partitions, segments, dist_matrix, clusters, cluster_assignments, representative_trajectories = traclus(trajectories)
```

