# Comparing `tmp/sherbystats-0.0.6.tar.gz` & `tmp/sherbystats-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherbystats-0.0.6.tar", last modified: Fri Apr 14 13:32:14 2023, max compression
+gzip compressed data, was "sherbystats-0.0.7.tar", last modified: Mon Apr 17 14:50:00 2023, max compression
```

## Comparing `sherbystats-0.0.6.tar` & `sherbystats-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-14 13:32:14.764653 sherbystats-0.0.6/
--rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-14 13:32:14.764260 sherbystats-0.0.6/PKG-INFO
--rw-r--r--   0 ryangosselin   (501) staff       (20)       38 2023-04-14 13:32:14.764832 sherbystats-0.0.6/setup.cfg
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      663 2023-04-14 13:28:30.000000 sherbystats-0.0.6/setup.py
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-14 13:32:14.760538 sherbystats-0.0.6/sherbystats/
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      173 2023-04-14 13:30:30.000000 sherbystats-0.0.6/sherbystats/__init__.py
--rwxr-xr-x   0 ryangosselin   (501) staff       (20)     4755 2022-12-02 18:57:23.000000 sherbystats-0.0.6/sherbystats/anova.py
--rw-r--r--   0 ryangosselin   (501) staff       (20)    12256 2022-11-28 21:45:55.000000 sherbystats-0.0.6/sherbystats/doe.py
--rwxr-xr-x   0 ryangosselin   (501) staff       (20)      993 2022-11-28 21:46:07.000000 sherbystats-0.0.6/sherbystats/mlr.py
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)     1839 2023-04-14 13:29:38.000000 sherbystats-0.0.6/sherbystats/normplot.py
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      700 2022-11-28 21:46:48.000000 sherbystats-0.0.6/sherbystats/xlsread.py
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-14 13:32:14.763620 sherbystats-0.0.6/sherbystats.egg-info/
--rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/PKG-INFO
--rw-r--r--   0 ryangosselin   (501) staff       (20)      278 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/SOURCES.txt
--rw-r--r--   0 ryangosselin   (501) staff       (20)        1 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/dependency_links.txt
--rw-r--r--   0 ryangosselin   (501) staff       (20)       12 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/top_level.txt
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-17 14:50:00.193025 sherbystats-0.0.7/
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-17 14:50:00.192769 sherbystats-0.0.7/PKG-INFO
+-rw-r--r--   0 ryangosselin   (501) staff       (20)       38 2023-04-17 14:50:00.193147 sherbystats-0.0.7/setup.cfg
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      663 2023-04-17 14:48:29.000000 sherbystats-0.0.7/setup.py
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-17 14:50:00.190365 sherbystats-0.0.7/sherbystats/
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      173 2023-04-14 13:30:30.000000 sherbystats-0.0.7/sherbystats/__init__.py
+-rwxr-xr-x   0 ryangosselin   (501) staff       (20)     4755 2022-12-02 18:57:23.000000 sherbystats-0.0.7/sherbystats/anova.py
+-rw-r--r--   0 ryangosselin   (501) staff       (20)    12256 2022-11-28 21:45:55.000000 sherbystats-0.0.7/sherbystats/doe.py
+-rwxr-xr-x   0 ryangosselin   (501) staff       (20)      993 2022-11-28 21:46:07.000000 sherbystats-0.0.7/sherbystats/mlr.py
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)     1846 2023-04-17 14:48:55.000000 sherbystats-0.0.7/sherbystats/normplot.py
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      700 2022-11-28 21:46:48.000000 sherbystats-0.0.7/sherbystats/xlsread.py
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-17 14:50:00.192395 sherbystats-0.0.7/sherbystats.egg-info/
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-17 14:50:00.000000 sherbystats-0.0.7/sherbystats.egg-info/PKG-INFO
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      278 2023-04-17 14:50:00.000000 sherbystats-0.0.7/sherbystats.egg-info/SOURCES.txt
+-rw-r--r--   0 ryangosselin   (501) staff       (20)        1 2023-04-17 14:50:00.000000 sherbystats-0.0.7/sherbystats.egg-info/dependency_links.txt
+-rw-r--r--   0 ryangosselin   (501) staff       (20)       12 2023-04-17 14:50:00.000000 sherbystats-0.0.7/sherbystats.egg-info/top_level.txt
```

### Comparing `sherbystats-0.0.6/setup.py` & `sherbystats-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="sherbystats",
-    version="0.0.6",
+    version="0.0.7",
     author="Ryan Gosselin",
     author_email="ryan.gosselin@usherbrooke.ca",
     url="https://www.usherbrooke.ca/gchimiquebiotech/departement/professeurs/ryan-gosselin/",
     packages=["sherbystats"],
     description="Ryan @ UdeS",
     long_description="Python for GCB140 and GCH711:\
     \n\
```

### Comparing `sherbystats-0.0.6/sherbystats/anova.py` & `sherbystats-0.0.7/sherbystats/anova.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.6/sherbystats/doe.py` & `sherbystats-0.0.7/sherbystats/doe.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.6/sherbystats/mlr.py` & `sherbystats-0.0.7/sherbystats/mlr.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.6/sherbystats/normplot.py` & `sherbystats-0.0.7/sherbystats/normplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,13 @@
     
     #transfrom them from precentile to cumulative density
     ticks_quan=[stats.norm.ppf(i/100.) for i in ticks_perc]
     
     #assign new ticks
     plt.yticks(ticks_quan,ticks_perc)
 
-    plt.xlabel('x',fontsize=20)
+    plt.xlabel('variable',fontsize=20)
     plt.ylabel('probabilite',fontsize=20)
 
     #show plot
     plt.tight_layout()
     plt.show()
```

### Comparing `sherbystats-0.0.6/sherbystats/xlsread.py` & `sherbystats-0.0.7/sherbystats/xlsread.py`

 * *Files identical despite different names*

