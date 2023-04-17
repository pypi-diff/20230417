# Comparing `tmp/mukkebude-0.1.1.tar.gz` & `tmp/mukkebude-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mukkebude-0.1.1.tar", max compression
+gzip compressed data, was "mukkebude-0.1.2.tar", max compression
```

## Comparing `mukkebude-0.1.1.tar` & `mukkebude-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1844 2023-04-12 20:40:50.406306 mukkebude-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/__init__.py
--rw-r--r--   0        0        0     2741 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/mapping.py
--rw-r--r--   0        0        0       99 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/model/__init__.py
--rw-r--r--   0        0        0     7127 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/model/mukke_bude_lstm.py
--rw-r--r--   0        0        0     7621 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/model/mukke_bude_transformer.py
--rw-r--r--   0        0        0      447 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/songs/generated_song_pokemon.mid
--rw-r--r--   0        0        0    17937 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/utils.py
--rw-r--r--   0        0        0     1021 2023-04-12 20:40:50.414306 mukkebude-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 mukkebude-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1889 2023-04-17 08:04:37.602001 mukkebude-0.1.2/README.md
+-rw-r--r--   0        0        0       34 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/__init__.py
+-rw-r--r--   0        0        0     2741 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/mapping.py
+-rw-r--r--   0        0        0       99 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/model/__init__.py
+-rw-r--r--   0        0        0     7127 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/model/mukke_bude_lstm.py
+-rw-r--r--   0        0        0     7621 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/model/mukke_bude_transformer.py
+-rw-r--r--   0        0        0      447 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/songs/generated_song_pokemon.mid
+-rw-r--r--   0        0        0    17937 2023-04-17 08:04:37.614001 mukkebude-0.1.2/mukkeBude/utils.py
+-rw-r--r--   0        0        0     1084 2023-04-17 08:04:37.618001 mukkebude-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 mukkebude-0.1.2/PKG-INFO
```

### Comparing `mukkebude-0.1.1/README.md` & `mukkebude-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
 Ziel der Studienarbeit ist die Komposition eines kleinen Musikstücks. Die Komposition erfolgt mittels eines Neuronalen Netzes.
 
+![](./flask-webapp/static/img/mukkebude.png)
+
 # Usage
 Hier wird beschrieben wir man das Projekt verwendet.
 
 ## Installation
 Um die unter [demos](./demos/) bereitgestellten jupyter-notebook verwenden zu können, muss das Projekt mittels pip installiert werden.
 Hierfür gibt es folgende Möglichkeiten:
 
@@ -22,23 +24,23 @@
 ```bash
 pip install mukkeBude
 ```
 
 Für die Verwendung der **Jupyter-Notebooks** muss jupyter-lab zusätzlich installiert werden!
 ```bash
 pip install jupyterlab
-``` 
+```
 
 ## Verwendung
 Nach einer erfolgreichen installtion kann das modul mittels `import mukkeBude` verwendet werden. Entsprechende Beispiele sind unter [demos](./demos/) zu finden.
 
 # Developing
 
 Hier wird beschrieben, wie man seine Entwicklungsumgebung entsprechend vorbereitet, um an dem Projekt zu entwicklen.
-Empfohlen ist die Verwendung von **Conda**, da hier die Verwendung von der GPU deutlich einfach ist. Bei der Verwendung der anderen Methoden müssen 
+Empfohlen ist die Verwendung von **Conda**, da hier die Verwendung von der GPU deutlich einfach ist. Bei der Verwendung der anderen Methoden müssen
 unter Umständen weitere Schritte unternommen werden, um die GPU zu verwenden.
 
 ## Conda
 Installation mithilfe von conda:
 
 ```bash
 conda env create -f environment.yml
@@ -64,8 +66,8 @@
 pip install -r requirements-dev.txt
 ```
 
 ## Poetry
 ```bash
 poetry install --with=dev
 poetry shell
-```
+```
```

### Comparing `mukkebude-0.1.1/mukkeBude/mapping.py` & `mukkebude-0.1.2/mukkeBude/mapping.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.1.1/mukkeBude/model/mukke_bude_lstm.py` & `mukkebude-0.1.2/mukkeBude/model/mukke_bude_lstm.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.1.1/mukkeBude/model/mukke_bude_transformer.py` & `mukkebude-0.1.2/mukkeBude/model/mukke_bude_transformer.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.1.1/mukkeBude/utils.py` & `mukkebude-0.1.2/mukkeBude/utils.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.1.1/pyproject.toml` & `mukkebude-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "mukkeBude"
-version = "v0.1.1"
+version = "v0.1.2"
 description = "A music generation library with transformer and lstm models',"
 authors = ["Florian Glaser <Florian.Glaser@ifm.com>", "Florian Herkommer <Florian.Herkommer@ifm.com>", "David Felder <David.Felder@ifm.com>"]
 readme = "README.md"
 homepage = "https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze"
 repository = "https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze"
 packages = [
     { include = "mukkeBude" }
 ]
 
 
 [tool.poetry.dependencies]
-python = "3.9.*"
+python = ">=3.9,<3.12"
 tensorflow = "2.10.*"
 tensorflow-text = "2.10.0"
 sacremoses = "0.0.53"
 keras-nlp = "0.4.1"
 matplotlib = "^3.7.1"
 music21 = "^8.1.0"
+tensorflow-io-gcs-filesystem = "0.31.0"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^67.6.1"
 wheel = "^0.40.0"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 autoflake = "^2.0.2"
 build = "^0.10.0"
 jupyterlab = "^3.6.3"
+pdoc = "^13.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mukkebude-0.1.1/PKG-INFO` & `mukkebude-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: mukkebude
-Version: 0.1.1
+Version: 0.1.2
 Summary: A music generation library with transformer and lstm models',
 Home-page: https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
 Author: Florian Glaser
 Author-email: Florian.Glaser@ifm.com
-Requires-Python: >=3.9.0,<3.10.0
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: keras-nlp (==0.4.1)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: music21 (>=8.1.0,<9.0.0)
 Requires-Dist: sacremoses (==0.0.53)
 Requires-Dist: tensorflow (>=2.10.0,<2.11.0)
+Requires-Dist: tensorflow-io-gcs-filesystem (==0.31.0)
 Requires-Dist: tensorflow-text (==2.10.0)
 Project-URL: Repository, https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
 Description-Content-Type: text/markdown
 
 # Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
 Ziel der Studienarbeit ist die Komposition eines kleinen Musikstücks. Die Komposition erfolgt mittels eines Neuronalen Netzes.
 
+![](./flask-webapp/static/img/mukkebude.png)
+
 # Usage
 Hier wird beschrieben wir man das Projekt verwendet.
 
 ## Installation
 Um die unter [demos](./demos/) bereitgestellten jupyter-notebook verwenden zu können, muss das Projekt mittels pip installiert werden.
 Hierfür gibt es folgende Möglichkeiten:
 
@@ -41,23 +46,23 @@
 ```bash
 pip install mukkeBude
 ```
 
 Für die Verwendung der **Jupyter-Notebooks** muss jupyter-lab zusätzlich installiert werden!
 ```bash
 pip install jupyterlab
-``` 
+```
 
 ## Verwendung
 Nach einer erfolgreichen installtion kann das modul mittels `import mukkeBude` verwendet werden. Entsprechende Beispiele sind unter [demos](./demos/) zu finden.
 
 # Developing
 
 Hier wird beschrieben, wie man seine Entwicklungsumgebung entsprechend vorbereitet, um an dem Projekt zu entwicklen.
-Empfohlen ist die Verwendung von **Conda**, da hier die Verwendung von der GPU deutlich einfach ist. Bei der Verwendung der anderen Methoden müssen 
+Empfohlen ist die Verwendung von **Conda**, da hier die Verwendung von der GPU deutlich einfach ist. Bei der Verwendung der anderen Methoden müssen
 unter Umständen weitere Schritte unternommen werden, um die GPU zu verwenden.
 
 ## Conda
 Installation mithilfe von conda:
 
 ```bash
 conda env create -f environment.yml
@@ -84,7 +89,8 @@
 ```
 
 ## Poetry
 ```bash
 poetry install --with=dev
 poetry shell
 ```
+
```

