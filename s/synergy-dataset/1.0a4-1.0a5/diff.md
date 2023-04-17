# Comparing `tmp/synergy-dataset-1.0a4.tar.gz` & `tmp/synergy-dataset-1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synergy-dataset-1.0a4.tar", last modified: Sat Apr 15 20:06:00 2023, max compression
+gzip compressed data, was "synergy-dataset-1.0a5.tar", last modified: Mon Apr 17 10:50:59 2023, max compression
```

## Comparing `synergy-dataset-1.0a4.tar` & `synergy-dataset-1.0a5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:06:00.776863 synergy-dataset-1.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:06:00.772863 synergy-dataset-1.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:06:00.772863 synergy-dataset-1.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 20:06:00.776863 synergy-dataset-1.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:06:00.776863 synergy-dataset-1.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:06:00.772863 synergy-dataset-1.0a4/synergy_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/synergy_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/synergy_dataset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/synergy_dataset/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:06:00.776863 synergy-dataset-1.0a4/synergy_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 20:06:00.000000 synergy-dataset-1.0a4/synergy_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:06:00.776863 synergy-dataset-1.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-15 20:05:45.000000 synergy-dataset-1.0a4/tests/test_synergy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.071821 synergy-dataset-1.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.075821 synergy-dataset-1.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:50:59.083821 synergy-dataset-1.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/synergy_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/synergy_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/synergy_dataset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 10:50:58.000000 synergy-dataset-1.0a5/synergy_dataset/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/synergy_dataset/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/synergy_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/tests/test_synergy.py
```

### Comparing `synergy-dataset-1.0a4/.github/workflows/python-package.yml` & `synergy-dataset-1.0a5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a4/.github/workflows/python-publish.yml` & `synergy-dataset-1.0a5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a4/.gitignore` & `synergy-dataset-1.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a4/LICENSE` & `synergy-dataset-1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a4/PKG-INFO` & `synergy-dataset-1.0a5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a4
+Version: 1.0a5
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
-# synergy - Python package for the SYNERGY dataset
+# Python package for the SYNERGY dataset
 
 ![PyPI](https://img.shields.io/pypi/v/synergy-dataset)
 
 The `synergy-dataset` Python package is the easiest way to download and built
 the SYNERGY dataset to your local device.
 
 ## Installation
```

### Comparing `synergy-dataset-1.0a4/README.md` & `synergy-dataset-1.0a5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# synergy - Python package for the SYNERGY dataset
+# Python package for the SYNERGY dataset
 
 ![PyPI](https://img.shields.io/pypi/v/synergy-dataset)
 
 The `synergy-dataset` Python package is the easiest way to download and built
 the SYNERGY dataset to your local device.
 
 ## Installation
```

### Comparing `synergy-dataset-1.0a4/pyproject.toml` & `synergy-dataset-1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a4/synergy_dataset/__main__.py` & `synergy-dataset-1.0a5/synergy_dataset/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 in SYNERGY cannot be published as plaintext again. Therefore you can refer
 to the version of the SYNERGY dataset.
 
 Would you like to convert the inverted abstract to plaintext?"""
 
 
 def main():
-
     if os.getenv("SYNERGY_PATH") == "development":
         p = _get_path_raw_dataset()
         print(f"Running development version of SYNERGY dataset at {p}.")
 
     if len(sys.argv) == 1:
         info()
     elif sys.argv[1] == "list":
@@ -67,15 +66,14 @@
 
     args, _ = parser.parse_known_args()
 
     parser.print_usage()
 
 
 def build_dataset(argv):
-
     parser = argparse.ArgumentParser(
         prog="synergy",
         description="Python package for SYNERGY dataset.",
     )
     parser.add_argument(
         "-o",
         "--output",
@@ -105,62 +103,60 @@
         action="store_true",
     )
 
     args, _ = parser.parse_known_args()
 
     if not args.legal:
         user_input = input(f"{LEGAL_NOTE} ([Y]es,[N]o):\n")
-        if user_input.lower() not in ["y", "yes"]:
-
+        if user_input.lower() in ["n", "no"]:
             if _dataset_available():
                 print(
                     "SYNERGY dataset already downloaded, but not",
                     "possible to build dataset (because of answer No).",
                 )
             else:
-                print("Downloading dataset, but not possible to build dataset.")
-                print("Read more: LINK.")
-        else:
+                print(
+                    "Downloading dataset, but not"
+                    "possible to build dataset (because of answer No)."
+                )
+        elif user_input.lower() in ["y", "yes"]:
             args.legal = True
+        else:
+            print("Not a valid answer.")
+            exit(1)
 
     # download the dataset if note available
     if not _dataset_available():
         download_raw_dataset()
 
     if args.legal:
-
         print("Building dataset")
 
         if Path(args.output).exists() and any(Path(args.output).iterdir()):
             print(f"Folder '{args.output}' is not empty")
             exit(1)
 
         # create output folder
         Path(args.output).mkdir(exist_ok=True, parents=True)
 
         if args.dataset is not None:
-
             for name in args.dataset:
                 d = Dataset(name)
                 result = d.to_frame()
 
                 if args.output:
-                    result.to_csv(
-                        Path(args.output, f"{name}.csv"),
-                        index=False
-                    )
+                    result.to_csv(Path(args.output, f"{name}.csv"), index=False)
         else:
             for dataset in tqdm(list(iter_datasets())):
                 dataset.to_frame(args.vars).to_csv(
                     Path(args.output, f"{dataset.name}.csv"), index=False
                 )
 
 
 def list_datasets(argv):
-
     parser = argparse.ArgumentParser(
         prog="synergy",
         description="List datasets.",
     )
     parser.add_argument(
         "--tablefmt",
         default="simple",
@@ -186,15 +182,14 @@
 
     table_values = []
 
     n = 0
     n_incl = 0
 
     for i, dataset in enumerate(iter_datasets()):
-
         n += dataset.metadata["data"]["n_records"]
         n_incl += dataset.metadata["data"]["n_records_included"]
 
         # if "concepts" not in dataset.metadata["publication"]:
         #     print(dataset.metadata["publication"]["openalex_id"], "No concepts found")
 
         concepts = list(
@@ -240,15 +235,14 @@
     except ZeroDivisionError:
         perc = "NA"
 
     print(f"Total records = {n}, total inclusions {n_incl} ({perc}%)\n")
 
 
 def show_dataset(argv):
-
     parser = argparse.ArgumentParser(
         prog="synergy",
         description="Show dataset.",
     )
     parser.add_argument(
         "dataset",
         help="Dataset name.",
@@ -288,62 +282,63 @@
     try:
         print(f"This dataset is part of a collection: \n{d.cite_collection}")
     except FileNotFoundError:
         pass
 
 
 def attribute_dataset(argv):
-
     parser = argparse.ArgumentParser(
         prog="synergy",
         description="Attribute authors of the datasets.",
     )
     parser.add_argument(
-        "--show-url",
-        help="Show the URL to the ORCID page of the author.",
-        action="store_true",
+        "--format",
+        default="text",
+        help="Show the attribution in text or markdown. Default text.",
     )
     args = parser.parse_args(argv)
 
     # download the dataset if note available
     if not _dataset_available():
         download_raw_dataset()
 
     # without url
-    if not args.show_url:
+    if args.format == "text":
         authors = []
 
         for i, dataset in enumerate(iter_datasets()):
             for a in dataset.metadata["publication"]["authorships"]:
                 authors.append(a["author"]["display_name"])
-    else:
+    elif args.format == "markdown":
         authors = []
 
         for i, dataset in enumerate(iter_datasets()):
             for a in dataset.metadata["publication"]["authorships"]:
-
                 if "orcid" in a["author"] and a["author"]["orcid"]:
                     authors.append(
                         f"[{a['author']['display_name']}]({a['author']['orcid']})"
                     )
                 else:
                     authors.append(a["author"]["display_name"])
+    else:
+        raise ValueError(f"Format not found '{args.format}'")
 
     print(
         "\nWe would like to thank the following authors for openly",
         "sharing the data correponding their systematic review:\n",
     )
-    print(", ".join(authors), "\n")
+
+    print(", ".join(list(set(authors))), "\n")
 
     print("\nReferences to datasets:\n")
+    prefix = "" if args.format == "text" else "> "
 
     for i, dataset in enumerate(iter_datasets()):
-
         print(
-            f"[{dataset.metadata['key']}]",
+            f"{prefix}[{dataset.metadata['key']}]",
             dataset.cite,
         )
 
     print(
         "\nWe thank the authors of the following collections",
         "of systematic reviews:\n",
     )
@@ -351,12 +346,13 @@
     collections = []
     for i, dataset in enumerate(iter_datasets()):
         try:
             collections.append(dataset.cite_collection)
         except FileNotFoundError:
             pass
 
-    print("\n".join(list(set(collections))))
+    for c in sorted(list(set(collections))):
+        print(f"{prefix}{c}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `synergy-dataset-1.0a4/synergy_dataset/base.py` & `synergy-dataset-1.0a5/synergy_dataset/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,23 @@
     os.getenv("SYNERGY_VERSION") if os.getenv("SYNERGY_VERSION") else "1.0rc0"
 )
 SYNERGY_PATH = os.getenv("SYNERGY_PATH")
 SYNERGY_ROOT = Path("~", ".synergy_dataset_source").expanduser()
 
 
 def _get_path_raw_dataset(version=SYNERGY_VERSION):
-
     if SYNERGY_PATH and SYNERGY_PATH == "development":
         return Path(__file__).parent.parent.parent / "synergy-release"
     elif SYNERGY_PATH:
         return Path(SYNERGY_PATH).expanduser()
     else:
         return Path(SYNERGY_ROOT, f"systematic-review-datasets-{version}")
 
 
 def _get_download_url(version=None, source="github"):
-
     if version is None:
         version = SYNERGY_VERSION
 
     if source == "github":
         github_url = "https://github.com/asreview/systematic-review-datasets/archive/refs/tags/v{}.zip"  # noqa
         return github_url.format(version)
     else:
@@ -62,19 +60,19 @@
         url (str, optional): URL to the SYNERGY dataset.
         Defaults to latest github release.
         path (str, optional): Path to download the dataset to.
         Defaults to ~/.synergy_dataset_source.
 
     """
 
-    print(f"Downloading version {SYNERGY_VERSION} of the SYNERGY dataset")
-
     if url is None:
         url = _get_download_url()
 
+    print(f"Downloading version {SYNERGY_VERSION} of the SYNERGY dataset...")
+
     release_zip = ZipFile(BytesIO(urlopen(url).read()))
     release_zip.extractall(path=path)
 
 
 def iter_datasets():
     """Iterate over the available datasets
 
@@ -101,68 +99,78 @@
 
     @property
     def cite(self):
         """Citation for the publication"""
 
         if not hasattr(self, "_cite"):
             with open(
-                Path(_get_path_raw_dataset(), self.name, "CITATION.txt"), "r"
+                Path(_get_path_raw_dataset(), self.name, "CITATION.txt"),
+                "r",
+                encoding="utf-8",
             ) as f:
                 self._cite = f.read()
 
         return self._cite
 
     @property
     def cite_collection(self):
         """Citation for the collection"""
 
         if not hasattr(self, "_cite_collection"):
             with open(
-                Path(_get_path_raw_dataset(), self.name, "CITATION_collection.txt"), "r"
+                Path(_get_path_raw_dataset(), self.name, "CITATION_collection.txt"),
+                "r",
+                encoding="utf-8",
             ) as f:
                 self._cite_collection = f.read()
 
         return self._cite_collection
 
     @property
     def metadata(self):
         """Metadata for the dataset"""
 
         if not hasattr(self, "_metadata"):
             with open(
-                Path(_get_path_raw_dataset(), self.name, "metadata.json"), "r"
+                Path(_get_path_raw_dataset(), self.name, "metadata.json"),
+                "r",
+                encoding="utf-8",
             ) as f:
                 self._metadata = json.load(f)
             with open(
                 Path(_get_path_raw_dataset(), self.name, "metadata_publication.json"),
                 "r",
+                encoding="utf-8",
             ) as f:
                 self._metadata["publication"] = json.load(f)
 
             try:
                 with open(
                     Path(
                         _get_path_raw_dataset(), self.name, "metadata_collection.json"
                     ),
                     "r",
+                    encoding="utf-8",
                 ) as f:
                     self._metadata["collection"] = json.load(f)
             except FileNotFoundError:
                 pass
 
         return self._metadata
 
     @property
     def labels(self):
         """Metadata on the corresponding publication as work"""
 
         if not hasattr(self, "_labels"):
             self._labels = {}
             with open(
-                Path(_get_path_raw_dataset(), self.name, "labels.csv"), newline=""
+                Path(_get_path_raw_dataset(), self.name, "labels.csv"),
+                newline="",
+                encoding="utf-8",
             ) as idfile:
                 reader = csv.DictReader(idfile)
                 for row in reader:
                     self._labels[row["openalex_id"]] = int(row["label_included"])
 
             return self._labels
 
@@ -174,17 +182,15 @@
         Yields:
             Work: pyalex.Work object, label
         """
 
         p_zipped_works = str(Path(_get_path_raw_dataset(), self.name, "works_*.zip"))
 
         for f_work in glob.glob(p_zipped_works):
-
             with ZipFile(f_work, "r") as z:
-
                 for work_set in z.namelist():
                     with z.open(work_set) as f:
                         d = json.loads(f.read())
 
                         for di in d:
                             yield Work(di), self.labels[di["id"]]
 
@@ -196,25 +202,22 @@
 
         Returns:
             dict: Dictionary of the dataset
         """
 
         records = {}
         for work, label_included in self.iter():
-
             if isinstance(variables, dict):
-
                 record = {}
                 for key, value in variables.items():
                     if isinstance(value, str):
                         record[key] = work[value]
                     else:
                         record[key] = value(work)
             elif isinstance(variables, list):
-
                 record = {}
                 for key in variables:
                     record[key] = work[key]
             else:
                 record = work
 
             # remove newlines
```

### Comparing `synergy-dataset-1.0a4/synergy_dataset.egg-info/PKG-INFO` & `synergy-dataset-1.0a5/synergy_dataset.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a4
+Version: 1.0a5
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
-# synergy - Python package for the SYNERGY dataset
+# Python package for the SYNERGY dataset
 
 ![PyPI](https://img.shields.io/pypi/v/synergy-dataset)
 
 The `synergy-dataset` Python package is the easiest way to download and built
 the SYNERGY dataset to your local device.
 
 ## Installation
```

### Comparing `synergy-dataset-1.0a4/synergy_dataset.egg-info/SOURCES.txt` & `synergy-dataset-1.0a5/synergy_dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

