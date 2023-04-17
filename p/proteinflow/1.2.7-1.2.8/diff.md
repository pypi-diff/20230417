# Comparing `tmp/proteinflow-1.2.7.tar.gz` & `tmp/proteinflow-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.2.7.tar", last modified: Mon Mar 27 10:21:03 2023, max compression
+gzip compressed data, was "proteinflow-1.2.8.tar", last modified: Mon Apr 17 12:02:39 2023, max compression
```

## Comparing `proteinflow-1.2.7.tar` & `proteinflow-1.2.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:21:03.440128 proteinflow-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-27 10:20:53.000000 proteinflow-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-03-27 10:21:03.440128 proteinflow-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-03-27 10:20:53.000000 proteinflow-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:21:03.436128 proteinflow-1.2.7/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    75145 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:21:03.436128 proteinflow-1.2.7/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:21:03.440128 proteinflow-1.2.7/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-03-27 10:20:53.000000 proteinflow-1.2.7/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:21:03.436128 proteinflow-1.2.7/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-03-27 10:21:03.000000 proteinflow-1.2.7/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-27 10:21:03.000000 proteinflow-1.2.7/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:21:03.000000 proteinflow-1.2.7/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 10:21:03.000000 proteinflow-1.2.7/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-27 10:21:03.000000 proteinflow-1.2.7/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-27 10:21:03.000000 proteinflow-1.2.7/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-27 10:20:53.000000 proteinflow-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 10:21:03.440128 proteinflow-1.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:21:03.440128 proteinflow-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-27 10:20:53.000000 proteinflow-1.2.7/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-27 10:20:53.000000 proteinflow-1.2.7/tests/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 12:02:27.000000 proteinflow-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-04-17 12:02:39.255886 proteinflow-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-17 12:02:27.000000 proteinflow-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    75424 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 12:02:27.000000 proteinflow-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:02:39.255886 proteinflow-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 12:02:27.000000 proteinflow-1.2.8/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 12:02:27.000000 proteinflow-1.2.8/tests/test_generate.py
```

### Comparing `proteinflow-1.2.7/LICENSE` & `proteinflow-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/PKG-INFO` & `proteinflow-1.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.2.7
+Version: 1.2.8
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Elizaveta Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
-Requires-Python: <3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ProteinFlow
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -20,27 +20,33 @@
 A data processing pipeline for all your protein design needs.
 
 [Read the documentation.](https://adaptyvbio.github.io/ProteinFlow/)
 
 ![overview](https://raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/fig_pipeline.png)
 
 ## Installation
-Recommended: create a new `conda` environment and install `proteinflow` and `mmseqs`. Note that the python version has to be between 3.8 and 3.10. 
+Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
 ```bash
-conda create --name proteinflow -y python=3.9
+conda create --name proteinflow -y
 conda activate proteinflow
-conda install -y -c conda-forge -c bioconda mmseqs2
 python -m pip install proteinflow
 ```
-In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not functioning . Follow the recommended fix:
+
+### Additional requirements
+In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
+
+First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
 ```bash
-python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
+conda install -y -c conda-forge -c bioconda mmseqs2
 ```
 
-Note that you do not need to install `mmseqs` or `rcsbsearch` if you are not planning to generate a new dataset.
+In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. Follow the recommended fix:
+```bash
+python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
+```
 
 Finally, you can use our [docker image](https://hub.docker.com/r/adaptyvbio/proteinflow/tags) as an alternative.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
 ```
 
 ## Usage
```

### Comparing `proteinflow-1.2.7/README.md` & `proteinflow-1.2.8/proteinflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: proteinflow
+Version: 1.2.8
+Summary: Versatile pipeline for processing protein structure data for deep learning applications.
+Author-email: Elizaveta Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
+License: BSD-3-Clause
+Keywords: bioinformatics,dataset,protein,PDB,deep learning
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ProteinFlow
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
@@ -9,27 +20,33 @@
 A data processing pipeline for all your protein design needs.
 
 [Read the documentation.](https://adaptyvbio.github.io/ProteinFlow/)
 
 ![overview](https://raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/fig_pipeline.png)
 
 ## Installation
-Recommended: create a new `conda` environment and install `proteinflow` and `mmseqs`. Note that the python version has to be between 3.8 and 3.10. 
+Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
 ```bash
-conda create --name proteinflow -y python=3.9
+conda create --name proteinflow -y
 conda activate proteinflow
-conda install -y -c conda-forge -c bioconda mmseqs2
 python -m pip install proteinflow
 ```
-In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not functioning . Follow the recommended fix:
+
+### Additional requirements
+In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
+
+First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
 ```bash
-python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
+conda install -y -c conda-forge -c bioconda mmseqs2
 ```
 
-Note that you do not need to install `mmseqs` or `rcsbsearch` if you are not planning to generate a new dataset.
+In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. Follow the recommended fix:
+```bash
+python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
+```
 
 Finally, you can use our [docker image](https://hub.docker.com/r/adaptyvbio/proteinflow/tags) as an alternative.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
 ```
 
 ## Usage
```

### Comparing `proteinflow-1.2.7/proteinflow/__init__.py` & `proteinflow-1.2.8/proteinflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,25 +850,27 @@
         # find longest sequence
         out = {}
         max_len = max(map(lambda x: x["S"].shape[0], batch))
 
         # pad according to max_len
         to_pad = [max_len - b["S"].shape[0] for b in batch]
         for key in batch[0].keys():
-            if key in ["chain_id", "chain_dict"]:
+            if key in ["chain_id", "chain_dict", "pdb_id"]:
                 continue
             out[key] = torch.stack(
                 [
                     torch.cat([b[key], torch.zeros((pad, *b[key].shape[1:]))], 0)
                     for b, pad in zip(batch, to_pad)
                 ],
                 0,
             )
         out["chain_id"] = torch.tensor([b["chain_id"] for b in batch])
         out["masked_res"] = self._get_masked_sequence(out)
+        out["chain_dict"] = [b["chain_dict"] for b in batch]
+        out["pdb_id"] = [b["pdb_id"] for b in batch]
         return out
 
     def __call__(self, batch):
         return self.pad_collate(batch)
 
 
 def download_data(tag, local_datasets_folder="./data", skip_splitting=False):
@@ -1483,19 +1485,16 @@
     def _process(self, filename, rewrite=False, max_length=None):
         """
         Process a proteinflow file and save it as ProteinMPNN features
         """
 
         input_file = os.path.join(self.dataset_folder, filename)
         no_extension_name = filename.split(".")[0]
-        try:
-            with open(input_file, "rb") as f:
-                data = pickle.load(f)
-        except:
-            print(f"{input_file=}")
+        with open(input_file, "rb") as f:
+            data = pickle.load(f)
         chains = sorted(data.keys())
         if self.entry_type == "biounit":
             chain_sets = [chains]
         elif self.entry_type == "chain":
             chain_sets = [[x] for x in chains]
         elif self.entry_type == "pair":
             chain_sets = list(combinations(chains, 2))
@@ -1583,14 +1582,15 @@
             out["X"] = torch.from_numpy(np.concatenate(X, 0))
             out["S"] = torch.cat(S)
             out["mask"] = torch.from_numpy(np.concatenate(mask))
             out["mask_original"] = torch.from_numpy(np.concatenate(mask_original))
             out["chain_encoding_all"] = torch.cat(chain_encoding_all)
             out["residue_idx"] = torch.cat(residue_idx)
             out["chain_dict"] = chain_dict
+            out["pdb_id"] = no_extension_name.split("-")[0]
             for key, value_list in node_features.items():
                 out[key] = torch.from_numpy(np.concatenate(value_list))
             with open(output_file, "wb") as f:
                 pickle.dump(out, f)
         return output_names
 
     def __len__(self):
@@ -1620,15 +1620,14 @@
         file = random.choice(self.files[id][chain_id])
         if self.loaded is None:
             with open(file, "rb") as f:
                 data = pickle.load(f)
         else:
             data = deepcopy(self.loaded[file])
         data["chain_id"] = data["chain_dict"][chain_id]
-        data.pop("chain_dict")
         return data
 
 
 class ProteinLoader(DataLoader):
     """
     A subclass of `torch.data.utils.DataLoader` tuned for the `proteinflow` dataset
 
@@ -1655,14 +1654,15 @@
         lower_limit=15,
         upper_limit=100,
         mask_residues=True,
         mask_whole_chains=False,
         mask_frac=None,
         force_binding_sites_frac=0,
         shuffle_batches=True,
+        collate_fn=None,
         *args,
         **kwargs,
     ):
         """
         Parameters
         ----------
         dataset : ProteinDataset
@@ -1678,26 +1678,30 @@
         force_binding_sites_frac : float, default 0
             if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
             forced to be in a binding site
         shuffle_clusters : bool, default True
             if `True`, a new representative is randomly selected for each cluster at each epoch (if `clustering_dict_path` is given)
         shuffle_batches : bool, default True
             if `True`, the batches are shuffled at each epoch
+        collate_fn : callable, optional
+            a function that takes a list of samples and returns a batch
         """
 
         super().__init__(
             dataset,
             collate_fn=_PadCollate(
                 mask_residues=mask_residues,
                 mask_whole_chains=mask_whole_chains,
                 mask_frac=mask_frac,
                 lower_limit=lower_limit,
                 upper_limit=upper_limit,
                 force_binding_sites_frac=force_binding_sites_frac,
-            ),
+            )
+            if collate_fn is None
+            else collate_fn,
             shuffle=shuffle_batches,
             *args,
             **kwargs,
         )
 
     @staticmethod
     def from_args(
```

### Comparing `proteinflow-1.2.7/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.2.8/proteinflow/scripts/proteinflow_cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow/utils/async_download.py` & `proteinflow-1.2.8/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow/utils/biotite_sse.py` & `proteinflow-1.2.8/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.2.8/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow/utils/filter_database.py` & `proteinflow-1.2.8/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.2.8/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow/utils/process_pdb.py` & `proteinflow-1.2.8/proteinflow/utils/process_pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Bio.Align import PairwiseAligner
+from Bio import pairwise2
 import numpy as np
 from typing import Dict
 import subprocess
 import urllib.request
 import os
 import numpy as np
 from biopandas.pdb import PandasPdb
@@ -351,20 +351,23 @@
         if "insertion" in chain_crd.columns:
             chain_crd["residue_number"] = chain_crd.apply(
                 lambda row: f"{row['residue_number']}_{row['insertion']}", axis=1
             )
         unique_numbers = chain_crd["residue_number"].unique()
         if len(unique_numbers) != len(pdb_seq):
             raise PDBError("Inconsistencies in the biopandas dataframe")
-        aligner = PairwiseAligner()
-        aligner.match_score = 2
-        aligner.mismatch_score = -10
-        aligner.open_gap_score = -0.5
-        aligner.extend_gap_score = -0.1
-        aligned_seq, fasta_seq = aligner.align(pdb_seq, fasta[chain])[0]
+        # aligner = PairwiseAligner()
+        # aligner.match_score = 2
+        # aligner.mismatch_score = -10
+        # aligner.open_gap_score = -0.5
+        # aligner.extend_gap_score = -0.1
+        # aligned_seq, fasta_seq = aligner.align(pdb_seq, fasta[chain])[0]
+        aligned_seq, fasta_seq, *_ = pairwise2.align.globalms(
+            pdb_seq, fasta[chain], 2, -10, -0.5, -0.1
+        )[0]
         aligned_seq_arr = np.array(list(aligned_seq))
         if "-" in fasta_seq or "".join([x for x in aligned_seq if x != "-"]) != pdb_seq:
             raise PDBError("Incorrect alignment")
         residue_numbers = np.where(aligned_seq_arr != "-")[0]
         start = residue_numbers.min()
         end = residue_numbers.max() + 1
         if start + (len(aligned_seq) - end) > max_missing_ends * len(aligned_seq):
```

### Comparing `proteinflow-1.2.7/proteinflow/utils/split_dataset.py` & `proteinflow-1.2.8/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.7/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: proteinflow
-Version: 1.2.7
-Summary: Versatile pipeline for processing protein structure data for deep learning applications.
-Author-email: Elizaveta Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
-License: BSD-3-Clause
-Keywords: bioinformatics,dataset,protein,PDB,deep learning
-Requires-Python: <3.10,>=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ProteinFlow
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
@@ -20,27 +9,33 @@
 A data processing pipeline for all your protein design needs.
 
 [Read the documentation.](https://adaptyvbio.github.io/ProteinFlow/)
 
 ![overview](https://raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/fig_pipeline.png)
 
 ## Installation
-Recommended: create a new `conda` environment and install `proteinflow` and `mmseqs`. Note that the python version has to be between 3.8 and 3.10. 
+Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
 ```bash
-conda create --name proteinflow -y python=3.9
+conda create --name proteinflow -y
 conda activate proteinflow
-conda install -y -c conda-forge -c bioconda mmseqs2
 python -m pip install proteinflow
 ```
-In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not functioning . Follow the recommended fix:
+
+### Additional requirements
+In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
+
+First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
 ```bash
-python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
+conda install -y -c conda-forge -c bioconda mmseqs2
 ```
 
-Note that you do not need to install `mmseqs` or `rcsbsearch` if you are not planning to generate a new dataset.
+In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. Follow the recommended fix:
+```bash
+python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
+```
 
 Finally, you can use our [docker image](https://hub.docker.com/r/adaptyvbio/proteinflow/tags) as an alternative.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
 ```
 
 ## Usage
```

### Comparing `proteinflow-1.2.7/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.2.8/proteinflow.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 proteinflow.egg-info/requires.txt
 proteinflow.egg-info/top_level.txt
 proteinflow/scripts/__init__.py
 proteinflow/scripts/proteinflow_cli.py
 proteinflow/utils/__init__.py
 proteinflow/utils/async_download.py
 proteinflow/utils/biotite_sse.py
+proteinflow/utils/build_pdb.py
 proteinflow/utils/cluster_and_partition.py
 proteinflow/utils/filter_database.py
 proteinflow/utils/mmcif_fix.py
 proteinflow/utils/process_pdb.py
 proteinflow/utils/split_dataset.py
 tests/test_download.py
 tests/test_generate.py
```

### Comparing `proteinflow-1.2.7/pyproject.toml` & `proteinflow-1.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.2.7"
+version = "1.2.8"
 authors = [
     {name = "Elizaveta Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
-requires-python = ">=3.8,<3.10"
+requires-python = ">=3.8"
 license = {text = "BSD-3-Clause"}
 dependencies = [
     "numpy",
     "editdistance>=0.6.0",
-    "Biopython>=1.80",
+    "Biopython==1.79",
     "click>=8.1.3",
     "biopandas>=0.4.1",
     "boto3==1.24.59",
     "p_tqdm>=1.4.0",
     "networkx==2.8.8",
     "einops>=0.6.0",
     "pandas>=1.5.2",
     "torch>=1.10.0",
     "biotite==0.35.0",
     "aiobotocore==2.4.2",
     "awscli==1.25.60",
+    "prody>=2.4",
     "rcsbsearch",
+    "sidechainnet",
 ]
 keywords = ["bioinformatics", "dataset", "protein", "PDB", "deep learning"]
 
 [project.scripts]
 proteinflow = "proteinflow.scripts.proteinflow_cli:cli"
 
 [tool.setuptools.packages]
```

### Comparing `proteinflow-1.2.7/tests/test_download.py` & `proteinflow-1.2.8/tests/test_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             "chain_id",
             "sidechain_orientation",
             "dihedral",
             "chemical",
             "secondary_structure",
             "masked_res",
             "sidechain_coords",
+            "pdb_id",
+            "chain_dict",
         }
         assert batch["X"].shape == (8, batch["X"].shape[1], 4, 3)
         assert batch["S"].shape == (8, batch["X"].shape[1])
         assert batch["dihedral"].shape == (8, batch["X"].shape[1], 2)
         assert batch["masked_res"].shape == (8, batch["X"].shape[1])
         assert batch["sidechain_coords"].shape == (8, batch["X"].shape[1], 10, 3)
         assert batch["X"].shape[1] <= 1000
```

### Comparing `proteinflow-1.2.7/tests/test_generate.py` & `proteinflow-1.2.8/tests/test_generate.py`

 * *Files identical despite different names*

