# Comparing `tmp/scslat-0.2.0.tar.gz` & `tmp/scslat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scslat-0.2.0.tar", max compression
+gzip compressed data, was "scslat-0.2.1.tar", max compression
```

## Comparing `scslat-0.2.0.tar` & `scslat-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1064 2023-01-25 14:50:39.728364 scslat-0.2.0/LICENSE
--rw-r--r--   0        0        0     3669 2023-01-25 14:50:39.728364 scslat-0.2.0/README.md
--rw-r--r--   0        0        0     3278 2023-01-25 14:50:40.904428 scslat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      339 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/__init__.py
--rw-r--r--   0        0        0     9324 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/metrics.py
--rw-r--r--   0        0        0      193 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/__init__.py
--rw-r--r--   0        0        0     1969 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/batch.py
--rw-r--r--   0        0        0       70 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/graphconv/__init__.py
--rw-r--r--   0        0        0     2396 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/graphconv/combnet.py
--rw-r--r--   0        0        0     3712 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/graphmodel.py
--rw-r--r--   0        0        0    11049 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/loaddata.py
--rw-r--r--   0        0        0      476 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/loss.py
--rw-r--r--   0        0        0       39 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/prematch/__init__.py
--rw-r--r--   0        0        0     4527 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/prematch/icp.py
--rw-r--r--   0        0        0     3947 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/prematch/utils.py
--rw-r--r--   0        0        0     3183 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/preprocess.py
--rw-r--r--   0        0        0     5109 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/train.py
--rw-r--r--   0        0        0    12513 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/model/utils.py
--rw-r--r--   0        0        0     2792 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/utils.py
--rw-r--r--   0        0        0     1018 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/viz/__init__.py
--rw-r--r--   0        0        0    24344 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/viz/multi_dataset.py
--rw-r--r--   0        0        0     4331 2023-01-25 14:50:40.908428 scslat-0.2.0/scSLAT/viz/single_dataset.py
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 scslat-0.2.0/setup.py
--rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 scslat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 08:50:02.833984 scslat-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3981 2023-04-17 08:50:02.833984 scslat-0.2.1/README.md
+-rw-r--r--   0        0        0     2671 2023-04-17 08:50:04.110007 scslat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/__init__.py
+-rw-r--r--   0        0        0     9198 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/metrics.py
+-rw-r--r--   0        0        0      193 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/__init__.py
+-rw-r--r--   0        0        0     1969 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/batch.py
+-rw-r--r--   0        0        0       70 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/graphconv/__init__.py
+-rw-r--r--   0        0        0     2396 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/graphconv/combnet.py
+-rw-r--r--   0        0        0     3712 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/graphmodel.py
+-rw-r--r--   0        0        0    11049 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/loaddata.py
+-rw-r--r--   0        0        0      476 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/loss.py
+-rw-r--r--   0        0        0       39 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/prematch/__init__.py
+-rw-r--r--   0        0        0     4527 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/prematch/icp.py
+-rw-r--r--   0        0        0     3947 2023-04-17 08:50:04.110007 scslat-0.2.1/scSLAT/model/prematch/utils.py
+-rw-r--r--   0        0        0     3183 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/model/preprocess.py
+-rw-r--r--   0        0        0     5109 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/model/train.py
+-rw-r--r--   0        0        0    12513 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/model/utils.py
+-rw-r--r--   0        0        0     2792 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/utils.py
+-rw-r--r--   0        0        0      988 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/viz/__init__.py
+-rw-r--r--   0        0        0     3474 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/viz/color.py
+-rw-r--r--   0        0        0    25075 2023-04-17 08:50:04.114007 scslat-0.2.1/scSLAT/viz/multi_dataset.py
+-rw-r--r--   0        0        0     6693 1970-01-01 00:00:00.000000 scslat-0.2.1/PKG-INFO
```

### Comparing `scslat-0.2.0/LICENSE` & `scslat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/README.md` & `scslat-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 [![stars-badge](https://img.shields.io/github/stars/gao-lab/SLAT?logo=GitHub&color=yellow)](https://github.com/gao-lab/SLAT/stargazers)
 [![dev-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/xiachenrui/bc835db052fde5bd731a09270b42006c/raw/slat_version.json)](https://gist.github.com/xiachenrui/bc835db052fde5bd731a09270b42006c)
 [![build-badge](https://github.com/gao-lab/SLAT/actions/workflows/build.yml/badge.svg)](https://github.com/gao-lab/SLAT/actions/workflows/build.yml)
 [![license-badge](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![docs-badge](https://readthedocs.org/projects/slat/badge/?version=latest)](https://slat.readthedocs.io/en/latest/?badge=latest)
-
-<!-- [![pypi-badge](https://img.shields.io/pypi/v/<name>)](https://pypi.org/project/<name>) -->
-
+[![pypi-badge](https://img.shields.io/pypi/v/scslat)](https://pypi.org/project/scslat)
 <!-- [![conda-badge](https://anaconda.org/bioconda/<name>/badges/version.svg)](https://anaconda.org/bioconda/<name>) -->
 
 # scSLAT: single cell spatial alignment tools
-
 **scSLAT** package implements the **SLAT** (**S**patial **L**inked **A**lignment **T**ool) model to align single cell spatial omics data.
 
 ![Model architecture](docs/_static/Model.png)
 
 ## Directory structure
 
 ```
@@ -27,64 +24,55 @@
 ├── docs/                    # Documentation files
 ├── resource/                # Other useful resource 
 ├── pyproject.toml           # Python package metadata
 └── README.md
 ```
 
 ## Tutorial
-
-Tutorial of `scSLAT` is [here](https://slat.readthedocs.io/en/latest/), if you have any question please open an issue on github
-
+Tutorial of `scSLAT` is [here](https://slat.readthedocs.io/en/latest/tutorials.html), if you have any question please open an issue on github
 
 <img src='docs/_static/imgalignment.gif' width='400'>
 
+
 ## Installation
+
 ### Docker
+Dockerfile of `scSLAT` is available at [`env/Dockerfile`](env/Dockerfile). You can also pull the docker image directly from [here](https://hub.docker.com/repository/docker/huhansan666666/slat) by:
 
-Dockerfile of `scSLAT` is available at [`env/Dockerfile`](env/Dockerfile). You can also pull the docker image directly from [here](https://hub.docker.com/repository/docker/huhansan666666/slat) by :
-```
+``` bash
 docker pull huhansan666666/slat:latest
 ```
 
-### Development
+### PyPI
+> **Note**
 > Installing `scSLAT` within a new [conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) is recommended.
-> Warning: machine with old NVIDIA driver may raise error, please update NVIDIA driver to the latest version or use Docker.
 
-For development purpose, clone this repo and install:
+First, we create a clean environment and install `scSLAT` from PyPI. Then we also need install dependencies for `pyg` manually. We default install with CUDA 11.7. Please refer [here](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#quick-start) for CPU version or different CUDA versions.
+
+> **Warning**
+> old NVIDIA driver may raise error, please update NVIDIA driver to the latest version.
 
 ```bash
-git clone git@github.com:gao-lab/SLAT.git
-cd SLAT
-pip install -e ".[torch]"
-pip install -e ".[pyg,dev,doc]"
+conda create -n scSLAT python=3.8 -y && conda activate scSLAT
+pip install scSLAT
+pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu117.html
 ```
 
-### PyPI  (Ongoing)
-
-Fist we create a clean environment and install `scSLAT` from PyPI:
-
-> We need install dependency `torch` before install `pyg`.
+### Development version
+For development purpose, clone this repo and install:
 
 ```bash
-conda create -n scSLAT python=3.8 -y && conda activate scSLAT
-pip install scSLAT[torch]
-pip install scSLAT[pyg]
+git clone git@github.com:gao-lab/SLAT.git
+cd SLAT
+pip install -e ".[dev,docs]"
+pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu117.html
 ```
 
 ### Conda (Ongoing)
-
 We plan to provide a conda package of `scSLAT` in the near future.
 
-## Reproduce manuscript results
 
-1. Please follow the [`env/README.md`](env/README.md) to install all dependencies. Please checkout the repository to v0.1.0 before install `scSLAT`:
-
-```
-git clone git@github.com:gao-lab/SLAT.git
-git checkout tags/v0.2.0
-pip install -e ".[torch]"
-pip install -e ".[pyg,dev,doc]"
-```
-
-2. Download and pre-process data follow the [`data/README.md`](data/README.md)
-3. Whole benchmark and evaluation procedure can be found in `/benchmark` and `/evaluation`, respectively.
-4. Every case study is recorded in the `/case` directory in the form of jupyter notebook.
+## Reproduce manuscript results
+1. Please follow the [`env/README.md`](env/README.md) to install all dependencies. Please checkout the repository to v0.2.1 before install `scSLAT`.
+2. Download and pre-process data follow the [`data/README.md`](data/README.md).
+3. Whole benchmark and evaluation procedure can be found in [`/benchmark`](benchmark/README.md) and [`/evaluation`](evaluation/README.md), respectively.
+4. Every case study is recorded in the [`/case`](case/README.md) directory in the form of jupyter notebook.
```

### Comparing `scslat-0.2.0/pyproject.toml` & `scslat-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,85 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scSLAT"
 packages = [{include = "scSLAT"}]
-version = "0.2.0"
+version = "0.2.1"
 description = "A graph deep learning based tool to align single cell spatial omics data"
 readme = "README.md"
 license = "MIT"
 authors = ["Chen-Rui Xia <xiachenrui@mail.cbi.pku.edu.cn>"]
-keywords = ["bioinformatics", "graph-deep-learning", "single-cell", "spatial-omics", "alignment"]
+keywords = ["bioinformatics", "deep-learning", "graph-neural-network", "single-cell", "spatial-omics"]
 homepage = "https://github.com/gao-lab/SLAT"
 documentation = "https://slat.readthedocs.io/en/latest/"
 repository = "https://github.com/gao-lab/SLAT"
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
+    "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Bio-Informatics"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = ">1.19"
 scipy = ">1.3"
 pandas = ">1.1"
-matplotlib = ">3.1.2"
+matplotlib = ">3.1.2,<3.7"
 seaborn = ">0.9"
-dill = ">0.2.3"
-tqdm = ">4.27"
 scikit-learn = ">0.21.2"
-statsmodels = ">0.10"
-parse = ">1.3.2"
 anndata = ">0.7"
 scanpy = ">1.5"
 h5py = "*"
+leidenalg = "*"
 packaging = "*"
 joblib = "*"
 pyyaml = "*"
-harmony-pytorch = "*"
-harmonypy = "*"
 plotly = "*"
 faiss-cpu = "*"
 pynvml = "*"
 scikit-misc = "*"
-leidenalg = "*"
 opencv-python = "*"
+ipykernel = "*"
+nbformat = "*"
 
-torch = {version = "1.11.0", source="torch", optional = true}
-torch-scatter = {version = "*", source="pyg", optional = true}
-torch-sparse = {version = "*", source="pyg", optional = true}
-torch-cluster = {version = "*", source="pyg", optional = true}
-torch-geometric = {version = "*", source="pyg", optional = true}
+torch = {version = ">=2.0.0"}
+torchvision = {version = "*"}
+torchaudio = {version = "*"}
+harmony-pytorch = {version = "*"}
+torch-geometric = {version = ">=2.3.0"}
 
 sphinx = {version="*", optional = true}
 sphinx-autodoc-typehints = {version="*", optional = true}
 sphinx-copybutton = {version="*", optional = true}
 sphinx-intl = {version="*", optional = true}
 nbsphinx = {version="*", optional = true}
 sphinx-rtd-theme = {version="*", optional = true}
 sphinx_gallery = {version=">=0.8.2,<0.11", optional = true}
 jinja2 = {version="*", optional = true}
 myst-parser = {version="*", optional = true}
 
 pytest = {version="*", optional = true}
 pytest-cov = {version="*", optional = true}
 papermill = {version="*", optional = true}
-snakemake = {version="*", optional = true}
-ipykernel = {version="*", optional = true}
 ipython = {version="*", optional = true}
 jupyter = {version="*", optional = true}
 
 [tool.poetry.extras]
-torch = ["torch"]
-pyg = ["torch-geometric", "torch-cluster", "torch-sparse", "torch-scatter"]
 docs = ["sphinx", "sphinx-autodoc-typehints", "sphinx-copybutton", "sphinx-intl", "nbsphinx", "sphinx-rtd-theme",
-        "jinja2", "myst-parser", "pandoc", "ipykernel", "sphinx_gallery"]
-dev = ["pytest", "pytest-cov", "papermill", "snakemake", "ipykernel", "ipython", "jupyter"]
+        "jinja2", "myst-parser", "pandoc", "sphinx_gallery"]
+dev = ["pytest", "pytest-cov", "papermill", "ipython", "jupyter"]
 
-[[tool.poetry.source]]
-name = "torch"
-url = "https://download.pytorch.org/whl/cu113"
-secondary = false
-
-[[tool.poetry.source]]
-name = "pyg"
-url = "https://data.pyg.org/whl/torch-1.11.0%2Bcu113.html"
-secondary = false
 
 [tool.pyright]
 include = ["scSLAT"]
 exclude = ["**/conda", "**/__pycache__", "**/.**"]
 ignore = ["resource/"]
```

### Comparing `scslat-0.2.0/scSLAT/metrics.py` & `scslat-0.2.1/scSLAT/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -211,21 +211,22 @@
         adata2 with spatial
     matching
         matching result
     spatial_key
         key of spatial data in adata.obsm
     """
     # reindex adata1 and adata2 by matching then calculate the pairwise euclidean distance
-    if abs(adata1.obsm[spatial_key].max()) > 1 or abs(adata1.obsm[spatial_key].min()) > 1:
-        adata1.obsm['scale_spatial'] = adata1.obsm[spatial_key]/adata1.obsm[spatial_key].max()
-    if abs(adata2.obsm[spatial_key].max()) > 1 or abs(adata2.obsm[spatial_key].min()) > 1:
-        adata2.obsm['scale_spatial'] = adata2.obsm[spatial_key]/adata2.obsm[spatial_key].max()
-    spatial_key = 'scale_spatial'
-    coord1 = adata1.obsm[spatial_key][matching[1,:]]
-    coord2 = adata2.obsm[spatial_key]
+    for adata in [adata1, adata2]:
+        coord = adata.obsm[spatial_key]
+        if abs(coord.ptp()) > 1 or abs(coord.max()) > 1:
+            adata.obsm['scale_spatial'] = (coord - coord.min(0))/coord.ptp(0)
+        else:
+            adata.obsm['scale_spatial'] = coord
+    coord1 = adata1.obsm['scale_spatial'][matching[1,:]]
+    coord2 = adata2.obsm['scale_spatial']
     distance = np.sqrt((coord1[:,0] - coord2[:,0])**2+(coord1[:,1] - coord2[:,1])**2)
     return float(distance.sum()/distance.shape[0])
 
 
 # TODO: optimize the speed
 def calc_NMI():
     r"""
```

### Comparing `scslat-0.2.0/scSLAT/model/batch.py` & `scslat-0.2.1/scSLAT/model/batch.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/graphconv/combnet.py` & `scslat-0.2.1/scSLAT/model/graphconv/combnet.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/graphmodel.py` & `scslat-0.2.1/scSLAT/model/graphmodel.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/loaddata.py` & `scslat-0.2.1/scSLAT/model/loaddata.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/prematch/icp.py` & `scslat-0.2.1/scSLAT/model/prematch/icp.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/prematch/utils.py` & `scslat-0.2.1/scSLAT/model/prematch/utils.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/preprocess.py` & `scslat-0.2.1/scSLAT/model/preprocess.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/train.py` & `scslat-0.2.1/scSLAT/model/train.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/model/utils.py` & `scslat-0.2.1/scSLAT/model/utils.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/utils.py` & `scslat-0.2.1/scSLAT/utils.py`

 * *Files identical despite different names*

### Comparing `scslat-0.2.0/scSLAT/viz/__init__.py` & `scslat-0.2.1/scSLAT/viz/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 r"""
 Visualization modules of SLAT 
 """
 from typing import Optional
 import matplotlib.pyplot as plt
 from matplotlib import colors
 
-from .single_dataset import *
 from .multi_dataset import *
 
 
 def hist(data,
          bins: Optional[int]=100,
          cut: Optional[float]=0.9,
          cut_height: Optional[int]=200
```

### Comparing `scslat-0.2.0/scSLAT/viz/multi_dataset.py` & `scslat-0.2.1/scSLAT/viz/multi_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,57 @@
 r"""
 Vis multi dataset and their connection
 """
 from typing import List, Mapping, Optional, Union
 import random
+import math
 
 from anndata import AnnData
 from sklearn.metrics.pairwise import euclidean_distances
 import numpy as np
 import pandas as pd
 
 import matplotlib.pyplot as plt
 import plotly.graph_objects as go
 
+from .color import *
 
-def random_color(n=1,seed:int=0):
+
+def get_color(n=1, cmap:str='scanpy', seed:int=0):
     r"""
-    Get color randomly
+    Get color 
     
     Parameters
     ---------
     n
         number of colors you want
+    cmap
+        color map (use same with scanpy)
     seed
-        seed to duplicate
+        random seed to duplicate
     """
-    random.seed(seed)
-    if n==1:
-        return "#"+''.join([random.choice('0123456789ABCDEF') for j in range(6)])
-    elif n>1 :
-        return ["#"+''.join([random.choice('0123456789ABCDEF') for j in range(6)]) for i in range(n)]
+    if cmap == 'scanpy' and n <= 10:
+        step = 10 // n
+        return vega_10_scanpy[::step][:n]
+    elif cmap == 'scanpy' and n <= 20 :
+        step = 20 // n
+        return vega_20_scanpy[::step][:n]
+    elif cmap == 'scanpy' and n <= 28:
+        step = 28 // n
+        return zeileis_28[::step][:n]
+    elif cmap == 'scanpy' and n <= 102:
+        step = 102 // n
+        return godsnot_102[::step][:n]
+    else:
+        print('WARNING: Using random color')
+        random.seed(seed)
+        if n==1:
+            return "#"+''.join([random.choice('0123456789ABCDEF') for j in range(6)])
+        elif n>1 :
+            return ["#"+''.join([random.choice('0123456789ABCDEF') for j in range(6)]) for i in range(n)]
 
 
 class build_3D():
     r"""
     Build 3D pics/models from multi-datasets
     
     Parameters
@@ -106,15 +125,15 @@
         height
             height of one layer
         """
         fig = plt.figure(figsize=(size[0],size[1]))
         ax = fig.add_subplot(111, projection='3d')
         ax.set_box_aspect([5,5,8])
         # color by different cell types
-        color = random_color(len(self.celltypes))
+        color = get_color(len(self.celltypes))
         c_map = {}
         for i, celltype in enumerate(self.celltypes):
             c_map[celltype] = color[i]
         for j, mapping in enumerate(self.mappings):
             print(f"Mapping {j}th layer ")
             # plot cells
             for i, (layer, anno) in enumerate(zip(self.loc_list[j:j+2], self.anno_list[j:j+2])):
@@ -130,15 +149,15 @@
             mapping = mapping[:,np.random.choice(mapping.shape[1], self.subsample_size, replace=False)].copy()
             for k in range(mapping.shape[1]):
                 cell1_index = mapping[:,k][0]  # query
                 cell0_index = mapping[:,k][1]  # ref
                 cell0_coord = self.loc_list[j][cell0_index,:]
                 cell1_coord = self.loc_list[j+1][cell1_index,:]
                 coord = np.row_stack((cell0_coord,cell1_coord))
-                ax.plot(coord[:,0], coord[:,1], [height*j,height*(j+1)], color=line_color,
+                ax.plot(coord[:,0], coord[:,1], [height*j, height*(j+1)], color=line_color,
                         linestyle="dashed", linewidth=line_width,alpha=line_alpha)
 
         if hide_axis:
             plt.axis('off')
         plt.show()
 
 
@@ -197,17 +216,18 @@
         self.subset = subset # index of query cells to be plotted
         scale_coordinate = True if rotate != None else scale_coordinate
         
         assert all(item in dataset_A.columns.values for item in ['index','x','y'])
         assert all(item in dataset_B.columns.values for item in ['index','x','y'])
         
         if meta:
-            self.celltypes = set(self.dataset_A[meta].append(self.dataset_B[meta]))
             set1 = list(set(self.dataset_A[meta]))
             set2 = list(set(self.dataset_B[meta]))
+            self.celltypes = set1 + [x for x in set2 if x not in set1]
+            self.celltypes.sort() # make sure celltypes are in the same order
             overlap = [x for x in set2 if x in set1]
             print(f"dataset1: {len(set1)} cell types; dataset2: {len(set2)} cell types; \n\
                     Total :{len(self.celltypes)} celltypes; Overlap: {len(overlap)} cell types \n\
                     Not overlap :[{[y for y in (set1+set2) if y not in overlap]}]"
                     )
         self.expr = expr if expr else False
             
@@ -235,14 +255,15 @@
                 conf_cutoff: Optional[float]=0,
                 point_size: Optional[List[int]]=[0.1,0.1],
                 line_width: Optional[float]=0.3,
                 line_color:Optional[str]='grey',
                 line_alpha: Optional[float]=0.7,
                 hide_axis: Optional[bool]=False,
                 show_error: Optional[bool]=True,
+                show_celltype: Optional[bool]=False,
                 cmap: Optional[bool]='Reds',
                 save:Optional[str]=None
         ) -> None:
         r"""
         Draw 3D picture of two datasets
         
         Parameters:
@@ -270,15 +291,15 @@
         """
         self.conf_cutoff = conf_cutoff
         show_error = show_error if self.meta else False
         fig = plt.figure(figsize=(size[0],size[1]))
         ax = fig.add_subplot(111, projection='3d')
         # color by meta
         if self.meta:
-            color = random_color(len(self.celltypes))
+            color = get_color(len(self.celltypes))
             c_map = {}
             for i, celltype in enumerate(self.celltypes):
                 c_map[celltype] = color[i]
             if self.expr:
                 c_map = cmap
                 # expr_concat = pd.concat(self.datasets)[self.expr].to_numpy()
                 # norm = plt.Normalize(expr_concat.min(), expr_concat.max())
@@ -287,60 +308,61 @@
                     norm = plt.Normalize(dataset[self.expr].to_numpy().min(), dataset[self.expr].to_numpy().max())
                 for cell_type in self.celltypes:
                     slice = dataset[dataset[self.meta] == cell_type]
                     xs = slice['x']
                     ys = slice['y']
                     zs = i
                     if self.expr:
-                        ax.scatter(xs, ys, zs, s=point_size[i], c=slice[self.expr], cmap=c_map,norm=norm)
+                        ax.scatter(xs, ys, zs, s=point_size[i], c=slice[self.expr], cmap=c_map, norm=norm)
                     else:
                         ax.scatter(xs, ys, zs, s=point_size[i], c=c_map[cell_type])
-                    
-        # plot points  without meta
+        # plot points without meta
         else:
             for i, dataset in enumerate(self.datasets):
                 xs = dataset['x']
                 ys = dataset['y']
                 zs = i
                 ax.scatter(xs,ys,zs,s=point_size[i])
-        
         # plot line
-        self.draw_lines(ax, show_error, line_color, line_width, line_alpha)
+        self.c_map = c_map
+        self.draw_lines(ax, show_error, show_celltype, line_color, line_width, line_alpha)
         if hide_axis:
             plt.axis('off')
         if save != None:
             plt.savefig(save)
         plt.show()
 
         
-    def draw_lines(self, ax, show_error, default_color, line_width=0.3, line_alpha=0.7) -> None:
+    def draw_lines(self, ax, show_error, show_celltype, default_color, line_width=0.3, line_alpha=0.7) -> None:
         r"""
         Draw lines between paired cells in two datasets
         """
         for i in range(self.matching.shape[1]):
             if not self.conf is None and self.conf[i] < self.conf_cutoff:
                 continue
             pair = self.matching[:,i]
             default_color = default_color
             if self.meta != None:
-                if self.dataset_B.loc[self.dataset_B['index']==pair[0], self.meta].astype(str).values ==\
-                    self.dataset_A.loc[self.dataset_A['index']==pair[1], self.meta].astype(str).values:
-                    color = '#ade8f4' # blue
-                else:
-                    color = '#ffafcc'  # red
-                # if self.conf:
-                #     if color == '#ade8f4' and not self.conf[i]: # low reliability but right
-                #         color = '#588157' # green
-                #     elif color == '#ffafcc' and self.conf[i]: # high reliability but error
-                #         color = '#ffb703' # yellow
-                
+                celltype1 = self.dataset_A.loc[self.dataset_A['index']==pair[1], self.meta].astype(str).values[0]
+                celltype2 = self.dataset_B.loc[self.dataset_B['index']==pair[0], self.meta].astype(str).values[0]
+                if show_error:
+                    if celltype1 == celltype2:
+                        color = '#ade8f4' # blue
+                    else:
+                        color = '#ffafcc'  # red
+                if show_celltype:
+                    if celltype1 == celltype2:
+                        color = self.c_map[celltype1]
+                    else:
+                        color = '#696969' # celltype1 error match color
             point0 = np.append(self.dataset_A[self.dataset_A['index']==pair[1]][['x','y']], 0)
             point1 = np.append(self.dataset_B[self.dataset_B['index']==pair[0]][['x','y']], 1)
-            coord = np.row_stack((point0,point1))
-            color = color if show_error else default_color
+
+            coord = np.row_stack((point0, point1))
+            color = color if show_error or show_celltype else default_color
             ax.plot(coord[:,0], coord[:,1], coord[:,2], color=color, linestyle="dashed", linewidth=line_width, alpha=line_alpha)
 
 
 class match_3D_multi_error(match_3D_multi):
     r"""
     Highlight the error mapping between datasets, child of class:`match_3D_multi()`
     
@@ -480,15 +502,15 @@
         self.highlight_cell = highlight_cell
         
     def draw_lines(self,ax,show_error,default_color,line_width=0.3,line_alpha=0.7)-> None:
         color_index = self.highlight_celltype[0] if len(self.highlight_celltype[0]) >= len(self.highlight_celltype[1]) else self.highlight_celltype[1]
         if type(self.highlight_line) == list and len(self.highlight_line) >= len(color_index):
             cmap = self.highlight_line
         else:
-            cmap = random_color(len(color_index)) if len(color_index) > 1 else [random_color(len(color_index))]
+            cmap = get_color(len(color_index)) if len(color_index) > 1 else [get_color(len(color_index))]
         
         for i in range(self.matching.shape[1]):
             pair = self.matching[:,i]
             a = self.dataset_A.loc[self.dataset_A['index']==pair[1], self.meta].astype(str).values
             b = self.dataset_B.loc[self.dataset_B['index']==pair[0], self.meta].astype(str).values
             if a not in self.highlight_celltype[0] or b not in self.highlight_celltype[1]:
                 continue
@@ -499,15 +521,14 @@
             if self.highlight_cell:
                 ax.scatter(point0[0],point0[1],point0[2],color=self.highlight_cell,alpha=1,s=1)
                 ax.scatter(point1[0],point1[1],point1[2],color=self.highlight_cell,alpha=1,s=1)
             color = color if show_error else default_color
             ax.plot(coord[:,0], coord[:,1], coord[:,2], color=color, linestyle="dashed",linewidth=line_width, alpha=line_alpha)
 
 
-
 def Sankey(matching_table:pd.DataFrame,
            color:Optional[List[str]]='red',
            title:Optional[str]='Sankey plot',
            prefix:Optional[List[str]]=['E11.5','E12.5'],
            layout:Optional[List[int]]=[1300,900],
            font_size:Optional[float]=15,
            font_color:Optional[str]='Black'):
@@ -600,17 +621,17 @@
             for j, ref in enumerate(matching_table.columns):
                 if int(matching_table.iloc[i,j]) > 10:
                     target.append(label2index[query+'_'+str(prefix+1)])
                     source.append(label2index[ref+'_'+str(prefix)])
                     value.append(int(matching_table.iloc[i,j]))
                     
     if color == 'random':
-        color = [random_color()]*matching_tables[0].shape[0]
+        color = [get_color()]*matching_tables[0].shape[0]
         for matching_table in matching_tables:
-            color += [random_color()]*matching_table.shape[1]
+            color += [get_color()]*matching_table.shape[1]
 
     fig = go.Figure(data=[go.Sankey(
         node = dict(
           pad = 50,
           thickness = 50,
           line = dict(color="green", width=0.5),
           label = list(label_all),
```

### Comparing `scslat-0.2.0/PKG-INFO` & `scslat-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,87 @@
 Metadata-Version: 2.1
 Name: scslat
-Version: 0.2.0
+Version: 0.2.1
 Summary: A graph deep learning based tool to align single cell spatial omics data
 Home-page: https://github.com/gao-lab/SLAT
 License: MIT
-Keywords: bioinformatics,graph-deep-learning,single-cell,spatial-omics,alignment
+Keywords: bioinformatics,deep-learning,graph-neural-network,single-cell,spatial-omics
 Author: Chen-Rui Xia
 Author-email: xiachenrui@mail.cbi.pku.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: pyg
-Provides-Extra: torch
 Requires-Dist: anndata (>0.7)
-Requires-Dist: dill (>0.2.3)
 Requires-Dist: faiss-cpu
 Requires-Dist: h5py
 Requires-Dist: harmony-pytorch
-Requires-Dist: harmonypy
-Requires-Dist: ipykernel ; extra == "docs" or extra == "dev"
+Requires-Dist: ipykernel
 Requires-Dist: ipython ; extra == "dev"
 Requires-Dist: jinja2 ; extra == "docs"
 Requires-Dist: joblib
 Requires-Dist: jupyter ; extra == "dev"
 Requires-Dist: leidenalg
-Requires-Dist: matplotlib (>3.1.2)
+Requires-Dist: matplotlib (>3.1.2,<3.7)
 Requires-Dist: myst-parser ; extra == "docs"
+Requires-Dist: nbformat
 Requires-Dist: nbsphinx ; extra == "docs"
 Requires-Dist: numpy (>1.19)
 Requires-Dist: opencv-python
 Requires-Dist: packaging
 Requires-Dist: pandas (>1.1)
 Requires-Dist: papermill ; extra == "dev"
-Requires-Dist: parse (>1.3.2)
 Requires-Dist: plotly
 Requires-Dist: pynvml
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pyyaml
 Requires-Dist: scanpy (>1.5)
 Requires-Dist: scikit-learn (>0.21.2)
 Requires-Dist: scikit-misc
 Requires-Dist: scipy (>1.3)
 Requires-Dist: seaborn (>0.9)
-Requires-Dist: snakemake ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
 Requires-Dist: sphinx-copybutton ; extra == "docs"
 Requires-Dist: sphinx-intl ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: sphinx_gallery (>=0.8.2,<0.11) ; extra == "docs"
-Requires-Dist: statsmodels (>0.10)
-Requires-Dist: torch (==1.11.0) ; extra == "torch"
-Requires-Dist: torch-cluster ; extra == "pyg"
-Requires-Dist: torch-geometric ; extra == "pyg"
-Requires-Dist: torch-scatter ; extra == "pyg"
-Requires-Dist: torch-sparse ; extra == "pyg"
-Requires-Dist: tqdm (>4.27)
+Requires-Dist: torch (>=2.0.0)
+Requires-Dist: torch-geometric (>=2.3.0)
+Requires-Dist: torchaudio
+Requires-Dist: torchvision
 Project-URL: Documentation, https://slat.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/gao-lab/SLAT
 Description-Content-Type: text/markdown
 
 [![stars-badge](https://img.shields.io/github/stars/gao-lab/SLAT?logo=GitHub&color=yellow)](https://github.com/gao-lab/SLAT/stargazers)
 [![dev-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/xiachenrui/bc835db052fde5bd731a09270b42006c/raw/slat_version.json)](https://gist.github.com/xiachenrui/bc835db052fde5bd731a09270b42006c)
 [![build-badge](https://github.com/gao-lab/SLAT/actions/workflows/build.yml/badge.svg)](https://github.com/gao-lab/SLAT/actions/workflows/build.yml)
 [![license-badge](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![docs-badge](https://readthedocs.org/projects/slat/badge/?version=latest)](https://slat.readthedocs.io/en/latest/?badge=latest)
-
-<!-- [![pypi-badge](https://img.shields.io/pypi/v/<name>)](https://pypi.org/project/<name>) -->
-
+[![pypi-badge](https://img.shields.io/pypi/v/scslat)](https://pypi.org/project/scslat)
 <!-- [![conda-badge](https://anaconda.org/bioconda/<name>/badges/version.svg)](https://anaconda.org/bioconda/<name>) -->
 
 # scSLAT: single cell spatial alignment tools
-
 **scSLAT** package implements the **SLAT** (**S**patial **L**inked **A**lignment **T**ool) model to align single cell spatial omics data.
 
 ![Model architecture](docs/_static/Model.png)
 
 ## Directory structure
 
 ```
@@ -105,65 +95,56 @@
 ├── docs/                    # Documentation files
 ├── resource/                # Other useful resource 
 ├── pyproject.toml           # Python package metadata
 └── README.md
 ```
 
 ## Tutorial
-
-Tutorial of `scSLAT` is [here](https://slat.readthedocs.io/en/latest/), if you have any question please open an issue on github
-
+Tutorial of `scSLAT` is [here](https://slat.readthedocs.io/en/latest/tutorials.html), if you have any question please open an issue on github
 
 <img src='docs/_static/imgalignment.gif' width='400'>
 
+
 ## Installation
+
 ### Docker
+Dockerfile of `scSLAT` is available at [`env/Dockerfile`](env/Dockerfile). You can also pull the docker image directly from [here](https://hub.docker.com/repository/docker/huhansan666666/slat) by:
 
-Dockerfile of `scSLAT` is available at [`env/Dockerfile`](env/Dockerfile). You can also pull the docker image directly from [here](https://hub.docker.com/repository/docker/huhansan666666/slat) by :
-```
+``` bash
 docker pull huhansan666666/slat:latest
 ```
 
-### Development
+### PyPI
+> **Note**
 > Installing `scSLAT` within a new [conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) is recommended.
-> Warning: machine with old NVIDIA driver may raise error, please update NVIDIA driver to the latest version or use Docker.
 
-For development purpose, clone this repo and install:
+First, we create a clean environment and install `scSLAT` from PyPI. Then we also need install dependencies for `pyg` manually. We default install with CUDA 11.7. Please refer [here](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#quick-start) for CPU version or different CUDA versions.
+
+> **Warning**
+> old NVIDIA driver may raise error, please update NVIDIA driver to the latest version.
 
 ```bash
-git clone git@github.com:gao-lab/SLAT.git
-cd SLAT
-pip install -e ".[torch]"
-pip install -e ".[pyg,dev,doc]"
+conda create -n scSLAT python=3.8 -y && conda activate scSLAT
+pip install scSLAT
+pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu117.html
 ```
 
-### PyPI  (Ongoing)
-
-Fist we create a clean environment and install `scSLAT` from PyPI:
-
-> We need install dependency `torch` before install `pyg`.
+### Development version
+For development purpose, clone this repo and install:
 
 ```bash
-conda create -n scSLAT python=3.8 -y && conda activate scSLAT
-pip install scSLAT[torch]
-pip install scSLAT[pyg]
+git clone git@github.com:gao-lab/SLAT.git
+cd SLAT
+pip install -e ".[dev,docs]"
+pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu117.html
 ```
 
 ### Conda (Ongoing)
-
 We plan to provide a conda package of `scSLAT` in the near future.
 
-## Reproduce manuscript results
 
-1. Please follow the [`env/README.md`](env/README.md) to install all dependencies. Please checkout the repository to v0.1.0 before install `scSLAT`:
-
-```
-git clone git@github.com:gao-lab/SLAT.git
-git checkout tags/v0.2.0
-pip install -e ".[torch]"
-pip install -e ".[pyg,dev,doc]"
-```
-
-2. Download and pre-process data follow the [`data/README.md`](data/README.md)
-3. Whole benchmark and evaluation procedure can be found in `/benchmark` and `/evaluation`, respectively.
-4. Every case study is recorded in the `/case` directory in the form of jupyter notebook.
+## Reproduce manuscript results
+1. Please follow the [`env/README.md`](env/README.md) to install all dependencies. Please checkout the repository to v0.2.1 before install `scSLAT`.
+2. Download and pre-process data follow the [`data/README.md`](data/README.md).
+3. Whole benchmark and evaluation procedure can be found in [`/benchmark`](benchmark/README.md) and [`/evaluation`](evaluation/README.md), respectively.
+4. Every case study is recorded in the [`/case`](case/README.md) directory in the form of jupyter notebook.
```

