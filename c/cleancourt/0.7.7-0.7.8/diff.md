# Comparing `tmp/cleancourt-0.7.7.tar.gz` & `tmp/cleancourt-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancourt-0.7.7.tar", last modified: Wed Apr 12 15:18:54 2023, max compression
+gzip compressed data, was "dist/cleancourt-0.7.8.tar", last modified: Mon Apr 17 19:47:06 2023, max compression
```

## Comparing `cleancourt-0.7.7.tar` & `cleancourt-0.7.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-12 15:18:39.000000 cleancourt-0.7.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-12 15:18:54.000000 cleancourt-0.7.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-12 15:18:39.000000 cleancourt-0.7.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-12 15:18:54.000000 cleancourt-0.7.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-12 15:18:39.000000 cleancourt-0.7.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/check_spaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/clean_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/compare_companies.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/compute_ngrams.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/cosine_similarity.py
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/full_clean_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/integrate_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/parse_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/separate_parent_company.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-17 19:46:51.000000 cleancourt-0.7.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-04-17 19:47:06.000000 cleancourt-0.7.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-17 19:46:51.000000 cleancourt-0.7.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-17 19:47:06.000000 cleancourt-0.7.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-17 19:46:51.000000 cleancourt-0.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/check_spaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/clean_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/compare_companies.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/compute_ngrams.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/cosine_similarity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/full_clean_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/integrate_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/parse_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/separate_parent_company.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/top_level.txt
```

### Comparing `cleancourt-0.7.7/LICENSE.txt` & `cleancourt-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/PKG-INFO` & `cleancourt-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.7
+Version: 0.7.8
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.7.7/README.md` & `cleancourt-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/setup.py` & `cleancourt-0.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="cleancourt",
-    version="0.7.7",
+    version="0.7.8",
     description="a library for cleaning court docket entries",
     author="Logan Pratico",
     author_email="praticol@lsc.gov",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.9",
```

### Comparing `cleancourt-0.7.7/src/cleancourt/__init__.py` & `cleancourt-0.7.8/src/cleancourt/__init__.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/check_spaces.py` & `cleancourt-0.7.8/src/cleancourt/check_spaces.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/clean_data.py` & `cleancourt-0.7.8/src/cleancourt/clean_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,27 +52,38 @@
 
     string = re.sub(" corporation", " corp", string)  # shorten corporation to corp
     string = re.sub(" company", " co", string)  # shorten company to co
     string = re.sub(" maa?nage?ment", " mgmt", string)  # etc
     string = re.sub(" incorporated", " inc", string)
     string = re.sub(" apartment", " apt", string)
     string = re.sub(" square(\s|$|,)", " sq\\1", string)
+    string = re.sub("department", "dept", string)
+
+    string = re.sub("fed[^\s]{0,4} cred[^\s]{0,2} un[^\s]{0,4}", "fcu", string)
+
+    string = re.sub("home ?owners association", "hoa", string)
+    string = re.sub("home ?owners assoc[^\s]{0,3}", "hoa", string)
+    string = re.sub("hoa,? inc", "hoa", string)
+
+    string = re.sub("national association", "na", string)
 
     string = re.sub("housing authy", "housing authority", string) # this replacement is being placed before any of the other housing authority replacements because "authy" appears in both PHA and RHA names
     string = re.sub("housing authority, inc", "housing authority", string)
 
     string = re.sub("redevelopment and housing authority", "rha", string)
-    string = re.sub("redevelopment and housing auth.?", "rha", string)
+    string = re.sub("redevelopment and housing auth[^\s]?", "rha", string)
     string = re.sub("redevelopment and housing", "rha", string)
     string = re.sub("redevelopment housing authority", "rha", string)
 
     string = re.sub("public housing authority", "pha", string)
     string = re.sub("housing authority", "pha", string)
     string = re.sub("housing and redevelopment authority", "pha", string)
 
+    
+
     string = re.sub(" et\.?\s?al\.?$", "", string)
     string = re.sub(
         "p\.?c\.?$", "", string
     )  # Remove P.C. (Personal Corporation) abbreviation on the end of a name
 
     string = re.sub("\.", "", string)  # Remove any periods
```

### Comparing `cleancourt-0.7.7/src/cleancourt/compare_companies.py` & `cleancourt-0.7.8/src/cleancourt/compare_companies.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/cosine_similarity.py` & `cleancourt-0.7.8/src/cleancourt/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/filter_types.py` & `cleancourt-0.7.8/src/cleancourt/filter_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     # Think Smith, Tom A. and Smith, Tom B. -> are these people the same? A fuzzy string match would say yes. But can we be sure?
     # As such, for this its better to remove people from the output all together and deal with them later in the normalization process.
     # Fortunately the probablepeople library can be used to quickly identify strings that are people, and just ignore them.
 
     # Probable people performs poorly on bank names. Working to update training dataset but this is a quick fix for now
 
     try:
+        val = pp.tag(name)
         return (
-            (pp.tag(name)[1] != "Person")
+            (val[1] != "Person")
+            or 'CorporationNameOrganization' in val[0]
             or ("|and|" in name)
             or (name.count(" ") == 0)
             or (re.search(" bank$", name))
             or ("bennington crossing" in name)
         ) and not name[0].isdigit()
     except:
         return True
@@ -38,14 +40,15 @@
         3) The name contains spaces (mononyms are often read as people by probablepeople. But more frequently refer to company names)
     """
 
     try:
         val = pp.tag(name)
         return (
             (val[1] == "Person")
+            and 'CorporationNameOrganization' not in val[0]
             and ("|and|" not in name)
             and (name.count(" ") != 0)
             and not (re.search(" bank$", name))
             and ("bennington crossing" not in name)
         )
     except:
         return False
```

### Comparing `cleancourt-0.7.7/src/cleancourt/full_clean_names.py` & `cleancourt-0.7.8/src/cleancourt/full_clean_names.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/integrate_output.py` & `cleancourt-0.7.8/src/cleancourt/integrate_output.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/parse_names.py` & `cleancourt-0.7.8/src/cleancourt/parse_names.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,25 @@
             val = pp.tag(name)
             try:
                 firstI = val[0]["FirstInitial"]
             except KeyError:
                 firstI = ""
 
             try:
+                prefOther = val[0]["PrefixOther"]
+            except KeyError:
+                prefOther = ""
+
+
+            try: # Update 0.7.8 first names are sometimes parsed as SuffixOther in probablepeople. this attempts to correct for that error
+                sufOther = val[0]["SuffixOther"]
+            except KeyError:
+                sufOther = ""
+
+            try:
                 first = val[0]["GivenName"]
             except KeyError:
                 first = ""
 
             try:
                 middle = val[0]["MiddleName"]
             except KeyError:
@@ -56,28 +67,39 @@
 
             try:
                 last = val[0]["Surname"]
             except KeyError:
                 last = ""
 
             try:
+                lastI = val[0]["LastInitial"]
+            except KeyError:
+                lastI = ""
+
+            try:
                 suffix = val[0]["SuffixGenerational"]
             except KeyError:
                 suffix = ""
 
-            full_name = (
+            full_name = ( # Add all of the parsed names together in a standard format
                 firstI
                 + " "
+                + prefOther
+                + " "
                 + first
                 + " "
+                + sufOther
+                + " "
                 + middle
                 + " "
                 + middleI
                 + " "
                 + last
+                + " " 
+                + lastI
                 + " "
                 + suffix
             )
 
-            names_dict[name] = re.sub(" +", " ", full_name.strip())
+            names_dict[name] = re.sub(" +", " ", full_name.strip()) # Strip any extra white spaces
 
     return names_dict
```

### Comparing `cleancourt-0.7.7/src/cleancourt/separate_parent_company.py` & `cleancourt-0.7.8/src/cleancourt/separate_parent_company.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt/test_utils.py` & `cleancourt-0.7.8/src/cleancourt/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.7/src/cleancourt.egg-info/PKG-INFO` & `cleancourt-0.7.8/src/cleancourt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.7
+Version: 0.7.8
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.7.7/src/cleancourt.egg-info/SOURCES.txt` & `cleancourt-0.7.8/src/cleancourt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

