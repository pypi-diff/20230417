# Comparing `tmp/ExoPSI-1.0.2.tar.gz` & `tmp/ExoPSI-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExoPSI-1.0.2.tar", last modified: Sat Apr 15 18:42:54 2023, max compression
+gzip compressed data, was "ExoPSI-1.0.3.tar", last modified: Sun Apr 16 23:01:22 2023, max compression
```

## Comparing `ExoPSI-1.0.2.tar` & `ExoPSI-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:42:54.439152 ExoPSI-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:42:54.360786 ExoPSI-1.0.2/ExoPSI/
--rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.2/ExoPSI/__init__.py
--rw-rw-rw-   0        0        0     8081 2023-04-15 18:40:59.000000 ExoPSI-1.0.2/ExoPSI/exopsi.py
--rw-rw-rw-   0        0        0     1872 2023-04-15 18:40:14.000000 ExoPSI-1.0.2/ExoPSI/subfunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:42:54.423268 ExoPSI-1.0.2/ExoPSI.egg-info/
--rw-rw-rw-   0        0        0     6734 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-15 18:42:54.000000 ExoPSI-1.0.2/ExoPSI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     6734 2023-04-15 18:42:54.439152 ExoPSI-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 18:42:54.439152 ExoPSI-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1417 2023-04-15 18:42:07.000000 ExoPSI-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:01:22.111799 ExoPSI-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-16 23:01:22.096205 ExoPSI-1.0.3/ExoPSI/
+-rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.3/ExoPSI/__init__.py
+-rw-rw-rw-   0        0        0     8371 2023-04-16 23:00:27.000000 ExoPSI-1.0.3/ExoPSI/exopsi.py
+-rw-rw-rw-   0        0        0     1872 2023-04-15 18:40:14.000000 ExoPSI-1.0.3/ExoPSI/subfunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:01:22.111799 ExoPSI-1.0.3/ExoPSI.egg-info/
+-rw-rw-rw-   0        0        0     6734 2023-04-16 23:01:21.000000 ExoPSI-1.0.3/ExoPSI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-16 23:01:21.000000 ExoPSI-1.0.3/ExoPSI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 23:01:21.000000 ExoPSI-1.0.3/ExoPSI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-16 23:01:21.000000 ExoPSI-1.0.3/ExoPSI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 23:01:21.000000 ExoPSI-1.0.3/ExoPSI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6734 2023-04-16 23:01:22.111799 ExoPSI-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 23:01:22.111799 ExoPSI-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1417 2023-04-16 23:00:59.000000 ExoPSI-1.0.3/setup.py
```

### Comparing `ExoPSI-1.0.2/ExoPSI/exopsi.py` & `ExoPSI-1.0.3/ExoPSI/exopsi.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,29 +68,36 @@
             print(e)
 
 
 
 
     #PLOTTING FUNCTIONS
     #1.Plot Interior vs Surface PSI
-    def psi_scale(self, df, x=None, y=None):
+    def psi_scale(self, df, x=None, y=None, color=None):
 
         if (x==None and y==None):  
             #sample = random.sample(sorted(df['PSI_Global']),200)
             data_x = df['PSI_Interior']
             data_y = df['PSI_Surface']
         else:
             data_x = df[x]
             data_y = df[y]
         
-        fig,ax = plt.subplots(1)
-        scatter = ax.scatter(data_x, data_y, cmap="viridis")
-        plt.xlabel("PSI_Interior")
-        plt.ylabel("PSI_Surface")
-        plt.title("PSI Scale")
+        if (color==None):
+            fig,ax = plt.subplots(1)
+            scatter = ax.scatter(data_x, data_y, cmap="viridis")
+            plt.xlabel("PSI_Interior")
+            plt.ylabel("PSI_Surface")
+            plt.title("PSI Scale")
+        else:
+            fig,ax = plt.subplots(1)
+            scatter = ax.scatter(data_x, data_y, color=color)
+            plt.xlabel("PSI_Interior")
+            plt.ylabel("PSI_Surface")
+            plt.title("PSI Scale")
         
         #Create Annotation Object
         annotation = ax.annotate(
             text='',
             xy=(0, 0),
             xytext=(15, 15), # distance from x, y
             textcoords='offset points',
```

### Comparing `ExoPSI-1.0.2/ExoPSI/subfunctions.py` & `ExoPSI-1.0.3/ExoPSI/subfunctions.py`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.2/ExoPSI.egg-info/PKG-INFO` & `ExoPSI-1.0.3/ExoPSI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExoPSI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to calculate Planet Similarity Indexes
 Home-page: https://github.com/ExoPSI/ExoPSI
 Author: ['Aditya Rai', 'Vaibhav Garg']
 Author-email: rai.aditya01@gmail.com
 License: GNU GPL v3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ExoPSI-1.0.2/LICENSE` & `ExoPSI-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.2/PKG-INFO` & `ExoPSI-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExoPSI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to calculate Planet Similarity Indexes
 Home-page: https://github.com/ExoPSI/ExoPSI
 Author: ['Aditya Rai', 'Vaibhav Garg']
 Author-email: rai.aditya01@gmail.com
 License: GNU GPL v3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ExoPSI-1.0.2/README.md` & `ExoPSI-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.2/setup.py` & `ExoPSI-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ExoPSI",
-    version="1.0.2",
+    version="1.0.3",
     description="Library to calculate Planet Similarity Indexes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ExoPSI/ExoPSI",
     author=["Aditya Rai","Vaibhav Garg"],
     author_email="rai.aditya01@gmail.com",
     license="GNU GPL v3.0",
```

