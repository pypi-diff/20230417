# Comparing `tmp/syracuse-0.3.0.tar.gz` & `tmp/syracuse-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syracuse-0.3.0.tar", max compression
+gzip compressed data, was "syracuse-0.4.0.tar", max compression
```

## Comparing `syracuse-0.3.0.tar` & `syracuse-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1099 2022-01-22 18:45:23.953954 syracuse-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1076 2023-03-19 12:01:46.105507 syracuse-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7891 2023-03-11 18:16:20.000000 syracuse-0.3.0/README.md
--rw-r--r--   0        0        0     2423 2023-02-25 18:29:58.561766 syracuse-0.3.0/syracuse/__init__.py
--rw-r--r--   0        0        0    23418 2023-03-19 12:09:05.289389 syracuse-0.3.0/syracuse/core.py
--rw-r--r--   0        0        0    11227 2023-03-19 11:58:43.357534 syracuse-0.3.0/syracuse/drawing.py
--rw-r--r--   0        0        0     8716 1970-01-01 00:00:00.000000 syracuse-0.3.0/setup.py
--rw-r--r--   0        0        0     8834 1970-01-01 00:00:00.000000 syracuse-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2022-01-22 18:45:23.953954 syracuse-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1099 2023-04-17 20:26:58.854306 syracuse-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9832 2023-04-17 20:21:28.951703 syracuse-0.4.0/README_pypi.md
+-rw-r--r--   0        0        0     2438 2023-04-17 20:21:28.979688 syracuse-0.4.0/syracuse/__init__.py
+-rw-r--r--   0        0        0    23418 2023-03-19 12:09:05.289389 syracuse-0.4.0/syracuse/core.py
+-rw-r--r--   0        0        0    11227 2023-03-19 11:58:43.357534 syracuse-0.4.0/syracuse/drawing.py
+-rw-r--r--   0        0        0    13407 2023-04-17 20:21:28.980702 syracuse-0.4.0/syracuse/sequences.py
+-rw-r--r--   0        0        0    10686 1970-01-01 00:00:00.000000 syracuse-0.4.0/setup.py
+-rw-r--r--   0        0        0    10753 1970-01-01 00:00:00.000000 syracuse-0.4.0/PKG-INFO
```

### Comparing `syracuse-0.3.0/LICENSE.md` & `syracuse-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `syracuse-0.3.0/pyproject.toml` & `syracuse-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "syracuse"
-version = "0.3.0"
+version = "0.4.0"
 description = "The Syracuse problem (aka Collatz conjecture) library"
 license = "MIT"
 authors = ["devfred78 <97401939+devfred78@users.noreply.github.com>"]
-readme = "README.md"
+readme = "README_pypi.md"
 repository = "https://github.com/devfred78/syracuse"
 documentation = "https://devfred78.github.io/syracuse/"
 keywords = ["syracuse", "collatz", "3n+1", "conjecture", "ulan", "kakutani", "thwaites", "hasse", "hailstone", "wondrous"]
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Operating System :: OS Independent",
 	"Intended Audience :: Education",
@@ -18,14 +18,15 @@
 [tool.poetry.dependencies]
 python = "~3.11"
 networkx = {extras = ["default"], version = "^3.0"}
 matplotlib = "~3.6"
 numpy = "~1.24"
 pydot = "^1.4.2"
 more-itertools = "^9.1.0"
+gmpy2 = "^2.1.5"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 mkdocs-material = "^9.0.12"
```

### Comparing `syracuse-0.3.0/README.md` & `syracuse-0.4.0/README_pypi.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 - If n is odd, multiply it by 3 and add 1.
 
 Then, repeat the process with the resulting value, applying the function over and over again until the value of n eventually reaches 1.
 
 > For example, if one takes n = 6, the sequence for the Collatz conjecture would be:
 > 6, 3, 10, 5, 16, 8, 4, 2, 1.
 
-The Collatz conjecture asserts that this sequence will always eventually reach the value 1, no matter what positive integer n one starts with. Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.
+Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.
 
 ### The compressed form
 
 *(definition partially inspired by the [relevant article on Wikipedia](https://en.wikipedia.org/wiki/Collatz_conjecture))*
 
 Since 3n+1 is even whenever n is odd, one may instead use the "compressed" form of the Collatz function:
 
@@ -86,14 +86,20 @@
 
 * pydot: version 1.4.2 or above
 
 	```sh
 	pip install pydot
 	```
 
+* more-itertools: version 9.1.0 or above
+
+	```sh
+	pip install more-itertools
+	```
+
 ### Installation
 
 Install from PyPi with:
 
 ```sh
 pip install syracuse
 ```
@@ -102,15 +108,69 @@
 
 ```sh
 pip install syracuse-X.Y.Z-py3-none-any.whl
 ```
 
 ## Usage
 
-Please refer to the [documentation](https://devfred78.github.io/syracuse/).
+Basic usage:
+
+```pycon
+>>> # Import the core library
+>>> import syracuse
+
+>>> # Create a Syracuse sequence with 27 as initial value
+>>> my_sequence = syracuse.Syracuse(27)
+
+>>> # Stopping time
+>>> my_sequence.stopping_time
+96
+>>> # Total stopping time
+>>> my_sequence.total_stopping_time
+111
+>>> # Maximum reached value
+>>> my_sequence.max
+9232
+>>> # Full sequence (until 1)
+>>> my_sequence.total_stopping_sequence
+(27, 82, 41, 124, 62, 31, 94, 47, 142, 71, 214, 107, 322, 161,
+ 484, 242, 121, 364, 182, 91, 274, 137, 412, 206, 103, 310, 155,
+ 466, 233, 700, 350, 175, 526, 263, 790, 395, 1186, 593, 1780,
+ 890, 445, 1336, 668, 334, 167, 502, 251, 754, 377, 1132, 566,
+ 283, 850, 425, 1276, 638, 319, 958, 479, 1438, 719, 2158, 1079,
+ 3238, 1619, 4858, 2429, 7288, 3644, 1822, 911, 2734, 1367, 4102,
+ 2051, 6154, 3077, 9232, 4616, 2308, 1154, 577, 1732, 866, 433,
+ 1300, 650, 325, 976, 488, 244, 122, 61, 184, 92, 46, 23, 70, 35,
+ 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1)
+
+>>> # Import the sequences library
+>>> import syracuse.sequences
+
+>>> # Create an iterator over the records of the max values (A006884)
+>>> # with all possible optimizations
+>>> max_records = syracuse.sequences.max_value_records(15)
+
+>>> # Iterate over the first 30 records
+>>> for _ in range(30):
+...		print(f"{next(max_records)}, ", end="", flush=True)
+...
+1, 2, 3, 7, 15, 27, 255, 447, 639, 703, 1819, 4255, 4591, 9663,
+20895, 26623, 31911, 60975, 77671, 113383, 138367, 159487, 270271,
+665215, 704511, 1042431, 1212415, 1441407, 1875711, 1988859,
+
+>>> # Import the drawing library
+>>> import syracuse.drawing
+
+>>> # Display the full sequence in a Matplotlib window
+>>> syracuse.drawing.single_sequence_to_matplotlib_figure(my_sequence, test=True)
+```
+
+![Matplotlib graphical view of the successive values of the sequence Syracuse(27)](https://github.com/devfred78/syracuse/blob/main/assets/graph_sequence_27_reduced.png?raw=True)
+
+For deeper explanations, please refer to the [documentation](https://devfred78.github.io/syracuse/).
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement" or "bug", according to whether you want to share a proposal of a new function, or to record an anomaly.
```

### Comparing `syracuse-0.3.0/syracuse/__init__.py` & `syracuse-0.4.0/syracuse/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Then, repeat the process with the resulting value, applying the function over and over again until the value of n eventually reaches 1.
 
 !!! example
 	
 	If one takes n = 6, the sequence for the Collatz conjecture would be:
 	6, 3, 10, 5, 16, 8, 4, 2, 1.
 
-The Collatz conjecture asserts that this sequence will always eventually reach the value 1, no matter what positive integer n one starts with. Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.
+Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.
 
 Since 3n+1 is even whenever n is odd, it is possible to define a "shortcut" (or "compressed") form for the Collatz function:
 
 - If n is even, divide it by 2.
 - If n is odd, multiply it by 3, add 1 **and divide the whole result by 2**.	
 	
 This definition yields smaller values for the stopping time and total stopping time without changing the overall dynamics of the process.
@@ -27,17 +27,19 @@
 
 The package provides the following modules:
 
 | Module    | Description                                                             |
 | --------- | ----------------------------------------------------------------------- |
 | `core`    | Provides classes to define Collatz sequences                            |
 | `drawing` | Provides tool functions to render in various ways the Collatz sequences |
+| `sequences` | Provides well-known sequences related to Collatz sequences |
 
 It is important to notice that the `core` module can be used without being imported explicitly. However, all other modules **need** to be imported explicitly.
 
 ```pycon
 >>> import syracuse # import all objects exposed by the core module
 >>> import syracuse.drawing # import objects exposed by the drawing module
+>>> import syracuse.sequences # import objects exposed by the sequences module
 ```
 
 """
 from .core import Syracuse, CompressedSyracuse
```

### Comparing `syracuse-0.3.0/syracuse/core.py` & `syracuse-0.4.0/syracuse/core.py`

 * *Files identical despite different names*

### Comparing `syracuse-0.3.0/syracuse/drawing.py` & `syracuse-0.4.0/syracuse/drawing.py`

 * *Files identical despite different names*

### Comparing `syracuse-0.3.0/setup.py` & `syracuse-0.4.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 packages = \
 ['syracuse']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.6,<3.7',
+['gmpy2>=2.1.5,<3.0.0',
+ 'matplotlib>=3.6,<3.7',
  'more-itertools>=9.1.0,<10.0.0',
  'networkx[default]>=3.0,<4.0',
  'numpy>=1.24,<1.25',
  'pydot>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'syracuse',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'The Syracuse problem (aka Collatz conjecture) library',
-    'long_description': '![PyPI - Python Version](https://img.shields.io/pypi/pyversions/syracuse)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/devfred78/syracuse)\n![GitHub](https://img.shields.io/github/license/devfred78/syracuse)\n![GitHub issues](https://img.shields.io/github/issues/devfred78/syracuse)\n![GitHub pull requests](https://img.shields.io/github/issues-pr/devfred78/syracuse)\n\n![Graph of the first 26 compressed Collatz sequences](https://github.com/devfred78/syracuse/blob/main/assets/graph_compressed_syracuse_26.png?raw=True)\n*(Graph of the first 26 compressed Collatz sequences)*\n\n# Syracuse\n\nsyracuse, The Syracuse problem (aka Collatz conjecture) library.\n\n## About the project\n\nThe syracuse library provides a way to generate Collatz sequences (either "normal" or compressed forms) and some functions to deal with.\n\n### The Collatz conjecture\n\nThe Collatz conjecture, also known as the "3n + 1 problem" or the "Syracuse problem", is an unsolved hypothesis in mathematics that concerns a sequence of operations applied to a positive integer. The conjecture states that no matter what the starting value of this integer is, the sequence will always eventually reach the value 1.\n\nMore specifically, the Collatz conjecture states that if one takes a positive integer n and applies the following function:\n\n- If n is even, divide it by 2.\n- If n is odd, multiply it by 3 and add 1.\n\nThen, repeat the process with the resulting value, applying the function over and over again until the value of n eventually reaches 1.\n\n> For example, if one takes n = 6, the sequence for the Collatz conjecture would be:\n> 6, 3, 10, 5, 16, 8, 4, 2, 1.\n\nThe Collatz conjecture asserts that this sequence will always eventually reach the value 1, no matter what positive integer n one starts with. Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.\n\n### The compressed form\n\n*(definition partially inspired by the [relevant article on Wikipedia](https://en.wikipedia.org/wiki/Collatz_conjecture))*\n\nSince 3n+1 is even whenever n is odd, one may instead use the "compressed" form of the Collatz function:\n\n- if n is even, divide it by 2.\n- if n is odd, multiply it by 3, add 1 **and divide the result by 2**.\n\nThis definition yields smaller values for the stopping time and total stopping time without changing the overall dynamics of the process. \n\n> For example, consider the Collatz sequence for the number 17:\n> 17, 52, 26, 13, 40, 20, 10, 5, 16, 8, 4, 2, 1\n>\n> The compressed form of this sequence would be:\n> 17, 26, 13, 20, 10, 5, 8, 4, 2, 1\n\nThe compressed form of the Collatz sequence has been the subject of much research, as it provides insights into the behavior of the original sequence and can be used to search for cycles and other patterns. However, the Collatz conjecture itself remains unproven, and the compressed form of the sequence does not provide a proof or disproof of the conjecture.\n\n### Why the name "syracuse" ?\n\nThe Collatz conjecture is also known as the Syracuse problem because it was first introduced by Lothar Collatz in a 1950 paper, where he credited his colleague, mathematician Helmut Hasse, with calling it the Syracuse problem. The name "Syracuse" refers to the University of Syracuse, where Collatz was working at the time.\n\nThe name "Syracuse problem" has since become a common alternative to "Collatz conjecture", especially in French and Italian-speaking countries, where it is often referred to as the "problème de Syracuse" or "problema di Syracuse", respectively.\n\nRegardless of the name used, the conjecture remains one of the most famous and challenging open problems in mathematics, and it continues to attract the attention of mathematicians and computer scientists around the world.\n\n## Getting started\n\n### Prerequisites\n\nOf course, syracuse cannot run without Python ! More precisely, it requires at least the 3.11 version of our beloved language.\n\nsyracuse depends on the following packages. The installation of syracuse should install automatically those packages if they are missing on your system. If it fails, you can install them individually:\n\n* networkx: version 3.0.0 or above\n\n\t```sh\n\tpip install networkx["default"]\n\t```\n\n* matplotlib: version 3.6.0 or above\n\n\t```sh\n\tpip install matplotlib\n\t```\n\n* numpy: version 1.24.0 or above\n\n\t```sh\n\tpip install numpy\n\t```\n\n* pydot: version 1.4.2 or above\n\n\t```sh\n\tpip install pydot\n\t```\n\n### Installation\n\nInstall from PyPi with:\n\n```sh\npip install syracuse\n```\n\nAs an alternative, you can download the `*.whl` file from the last [release on the syracuse Github repository](https://github.com/devfred78/syracuse/releases), and execute the following command (replace "X.Y.Z" by the right version number):\n\n```sh\npip install syracuse-X.Y.Z-py3-none-any.whl\n```\n\n## Usage\n\nPlease refer to the [documentation](https://devfred78.github.io/syracuse/).\n\n## Contributing\n\nContributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nIf you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement" or "bug", according to whether you want to share a proposal of a new function, or to record an anomaly.\n\nDon\'t forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n## License\n\nDistributed under the MIT License. Check out [LICENSE.md](https://github.com/devfred78/syracuse/blob/main/LICENSE.md) file for more information.\n\n## Acknowledgments\n\nI would like greatfully to thank:\n\nGraphviz [authors](https://graphviz.org/) for this impressive graph visualization software, especially for the creation of the useful [DOT Langage](https://graphviz.org/doc/info/lang.html).\n\n[The Matplotlib development team](https://matplotlib.org/) for providing a very powerful library "for creating static, animated, and interactive visualizations in Python".\n\nNumPy [community](https://numpy.org/) for this fundamental tool to be used as a priority if you want make serious scientific computations with Python.\n\n[MkDocs](https://www.mkdocs.org/), [mkdocstrings](https://mkdocstrings.github.io/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) for giving the ability to create in a very simple way an accessible documentation for either tiny or big projects.\n\n[Make a README](https://www.makeareadme.com/), [Sayan Mondal](https://medium.com/swlh/how-to-make-the-perfect-readme-md-on-github-92ed5771c061), [Hillary Nyakundi](https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/) and [othneildrew](https://github.com/othneildrew/Best-README-Template) for providing very interesting materials to write good README files (far better than I can write by myself !).\n\n[Choose an open source license](https://choosealicense.com/) for helping to choose the best suitable license for this project.\n\n[Semantic Versioning](https://semver.org/) for providing clear specifications for versioning projects.\n\n[Real Python](https://realpython.com/) for contributing really increasing skills in Python for everyone, novices or veterans.\n\n[GitHub](https://github.com/) for hosting this project, and helping to share it.\n\n[Pypi](https://pypi.org/) for providing a very convenient way to share modules and package to the entire Python community.\n\nAnd, of course, all the former, current and further contributors of this project !',
+    'long_description': '![PyPI - Python Version](https://img.shields.io/pypi/pyversions/syracuse)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/devfred78/syracuse)\n![GitHub](https://img.shields.io/github/license/devfred78/syracuse)\n![GitHub issues](https://img.shields.io/github/issues/devfred78/syracuse)\n![GitHub pull requests](https://img.shields.io/github/issues-pr/devfred78/syracuse)\n\n![Graph of the first 26 compressed Collatz sequences](https://github.com/devfred78/syracuse/blob/main/assets/graph_compressed_syracuse_26.png?raw=True)\n*(Graph of the first 26 compressed Collatz sequences)*\n\n# Syracuse\n\nsyracuse, The Syracuse problem (aka Collatz conjecture) library.\n\n## About the project\n\nThe syracuse library provides a way to generate Collatz sequences (either "normal" or compressed forms) and some functions to deal with.\n\n### The Collatz conjecture\n\nThe Collatz conjecture, also known as the "3n + 1 problem" or the "Syracuse problem", is an unsolved hypothesis in mathematics that concerns a sequence of operations applied to a positive integer. The conjecture states that no matter what the starting value of this integer is, the sequence will always eventually reach the value 1.\n\nMore specifically, the Collatz conjecture states that if one takes a positive integer n and applies the following function:\n\n- If n is even, divide it by 2.\n- If n is odd, multiply it by 3 and add 1.\n\nThen, repeat the process with the resulting value, applying the function over and over again until the value of n eventually reaches 1.\n\n> For example, if one takes n = 6, the sequence for the Collatz conjecture would be:\n> 6, 3, 10, 5, 16, 8, 4, 2, 1.\n\nAlthough the conjecture has been computationally tested for extremely large values, it remains unproven to this day.\n\n### The compressed form\n\n*(definition partially inspired by the [relevant article on Wikipedia](https://en.wikipedia.org/wiki/Collatz_conjecture))*\n\nSince 3n+1 is even whenever n is odd, one may instead use the "compressed" form of the Collatz function:\n\n- if n is even, divide it by 2.\n- if n is odd, multiply it by 3, add 1 **and divide the result by 2**.\n\nThis definition yields smaller values for the stopping time and total stopping time without changing the overall dynamics of the process. \n\n> For example, consider the Collatz sequence for the number 17:\n> 17, 52, 26, 13, 40, 20, 10, 5, 16, 8, 4, 2, 1\n>\n> The compressed form of this sequence would be:\n> 17, 26, 13, 20, 10, 5, 8, 4, 2, 1\n\nThe compressed form of the Collatz sequence has been the subject of much research, as it provides insights into the behavior of the original sequence and can be used to search for cycles and other patterns. However, the Collatz conjecture itself remains unproven, and the compressed form of the sequence does not provide a proof or disproof of the conjecture.\n\n### Why the name "syracuse" ?\n\nThe Collatz conjecture is also known as the Syracuse problem because it was first introduced by Lothar Collatz in a 1950 paper, where he credited his colleague, mathematician Helmut Hasse, with calling it the Syracuse problem. The name "Syracuse" refers to the University of Syracuse, where Collatz was working at the time.\n\nThe name "Syracuse problem" has since become a common alternative to "Collatz conjecture", especially in French and Italian-speaking countries, where it is often referred to as the "problème de Syracuse" or "problema di Syracuse", respectively.\n\nRegardless of the name used, the conjecture remains one of the most famous and challenging open problems in mathematics, and it continues to attract the attention of mathematicians and computer scientists around the world.\n\n## Getting started\n\n### Prerequisites\n\nOf course, syracuse cannot run without Python ! More precisely, it requires at least the 3.11 version of our beloved language.\n\nsyracuse depends on the following packages. The installation of syracuse should install automatically those packages if they are missing on your system. If it fails, you can install them individually:\n\n* networkx: version 3.0.0 or above\n\n\t```sh\n\tpip install networkx["default"]\n\t```\n\n* matplotlib: version 3.6.0 or above\n\n\t```sh\n\tpip install matplotlib\n\t```\n\n* numpy: version 1.24.0 or above\n\n\t```sh\n\tpip install numpy\n\t```\n\n* pydot: version 1.4.2 or above\n\n\t```sh\n\tpip install pydot\n\t```\n\n* more-itertools: version 9.1.0 or above\n\n\t```sh\n\tpip install more-itertools\n\t```\n\n### Installation\n\nInstall from PyPi with:\n\n```sh\npip install syracuse\n```\n\nAs an alternative, you can download the `*.whl` file from the last [release on the syracuse Github repository](https://github.com/devfred78/syracuse/releases), and execute the following command (replace "X.Y.Z" by the right version number):\n\n```sh\npip install syracuse-X.Y.Z-py3-none-any.whl\n```\n\n## Usage\n\nBasic usage:\n\n```pycon\n>>> # Import the core library\n>>> import syracuse\n\n>>> # Create a Syracuse sequence with 27 as initial value\n>>> my_sequence = syracuse.Syracuse(27)\n\n>>> # Stopping time\n>>> my_sequence.stopping_time\n96\n>>> # Total stopping time\n>>> my_sequence.total_stopping_time\n111\n>>> # Maximum reached value\n>>> my_sequence.max\n9232\n>>> # Full sequence (until 1)\n>>> my_sequence.total_stopping_sequence\n(27, 82, 41, 124, 62, 31, 94, 47, 142, 71, 214, 107, 322, 161,\n 484, 242, 121, 364, 182, 91, 274, 137, 412, 206, 103, 310, 155,\n 466, 233, 700, 350, 175, 526, 263, 790, 395, 1186, 593, 1780,\n 890, 445, 1336, 668, 334, 167, 502, 251, 754, 377, 1132, 566,\n 283, 850, 425, 1276, 638, 319, 958, 479, 1438, 719, 2158, 1079,\n 3238, 1619, 4858, 2429, 7288, 3644, 1822, 911, 2734, 1367, 4102,\n 2051, 6154, 3077, 9232, 4616, 2308, 1154, 577, 1732, 866, 433,\n 1300, 650, 325, 976, 488, 244, 122, 61, 184, 92, 46, 23, 70, 35,\n 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1)\n\n>>> # Import the sequences library\n>>> import syracuse.sequences\n\n>>> # Create an iterator over the records of the max values (A006884)\n>>> # with all possible optimizations\n>>> max_records = syracuse.sequences.max_value_records(15)\n\n>>> # Iterate over the first 30 records\n>>> for _ in range(30):\n...\t\tprint(f"{next(max_records)}, ", end="", flush=True)\n...\n1, 2, 3, 7, 15, 27, 255, 447, 639, 703, 1819, 4255, 4591, 9663,\n20895, 26623, 31911, 60975, 77671, 113383, 138367, 159487, 270271,\n665215, 704511, 1042431, 1212415, 1441407, 1875711, 1988859,\n\n>>> # Import the drawing library\n>>> import syracuse.drawing\n\n>>> # Display the full sequence in a Matplotlib window\n>>> syracuse.drawing.single_sequence_to_matplotlib_figure(my_sequence, test=True)\n```\n\n![Matplotlib graphical view of the successive values of the sequence Syracuse(27)](https://github.com/devfred78/syracuse/blob/main/assets/graph_sequence_27_reduced.png?raw=True)\n\nFor deeper explanations, please refer to the [documentation](https://devfred78.github.io/syracuse/).\n\n## Contributing\n\nContributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nIf you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement" or "bug", according to whether you want to share a proposal of a new function, or to record an anomaly.\n\nDon\'t forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n## License\n\nDistributed under the MIT License. Check out [LICENSE.md](https://github.com/devfred78/syracuse/blob/main/LICENSE.md) file for more information.\n\n## Acknowledgments\n\nI would like greatfully to thank:\n\nGraphviz [authors](https://graphviz.org/) for this impressive graph visualization software, especially for the creation of the useful [DOT Langage](https://graphviz.org/doc/info/lang.html).\n\n[The Matplotlib development team](https://matplotlib.org/) for providing a very powerful library "for creating static, animated, and interactive visualizations in Python".\n\nNumPy [community](https://numpy.org/) for this fundamental tool to be used as a priority if you want make serious scientific computations with Python.\n\n[MkDocs](https://www.mkdocs.org/), [mkdocstrings](https://mkdocstrings.github.io/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) for giving the ability to create in a very simple way an accessible documentation for either tiny or big projects.\n\n[Make a README](https://www.makeareadme.com/), [Sayan Mondal](https://medium.com/swlh/how-to-make-the-perfect-readme-md-on-github-92ed5771c061), [Hillary Nyakundi](https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/) and [othneildrew](https://github.com/othneildrew/Best-README-Template) for providing very interesting materials to write good README files (far better than I can write by myself !).\n\n[Choose an open source license](https://choosealicense.com/) for helping to choose the best suitable license for this project.\n\n[Semantic Versioning](https://semver.org/) for providing clear specifications for versioning projects.\n\n[Real Python](https://realpython.com/) for contributing really increasing skills in Python for everyone, novices or veterans.\n\n[GitHub](https://github.com/) for hosting this project, and helping to share it.\n\n[Pypi](https://pypi.org/) for providing a very convenient way to share modules and package to the entire Python community.\n\nAnd, of course, all the former, current and further contributors of this project !',
     'author': 'devfred78',
     'author_email': '97401939+devfred78@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/devfred78/syracuse',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `syracuse-0.3.0/PKG-INFO` & `syracuse-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: syracuse
-Version: 0.3.0
+Version: 0.4.0
 Summary: The Syracuse problem (aka Collatz conjecture) library
 Home-page: https://github.com/devfred78/syracuse
 License: MIT
 Keywords: syracuse,collatz,3n+1,conjecture,ulan,kakutani,thwaites,hasse,hailstone,wondrous
 Author: devfred78
 Author-email: 97401939+devfred78@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: gmpy2 (>=2.1.5,<3.0.0)
 Requires-Dist: matplotlib (>=3.6,<3.7)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: networkx[default] (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.24,<1.25)
 Requires-Dist: pydot (>=1.4.2,<2.0.0)
 Project-URL: Documentation, https://devfred78.github.io/syracuse/
 Project-URL: Repository, https://github.com/devfred78/syracuse
@@ -51,15 +52,15 @@
 - If n is odd, multiply it by 3 and add 1.
 
 Then, repeat the process with the resulting value, applying the function over and over again until the value of n eventually reaches 1.
 
 > For example, if one takes n = 6, the sequence for the Collatz conjecture would be:
 > 6, 3, 10, 5, 16, 8, 4, 2, 1.
 
-The Collatz conjecture asserts that this sequence will always eventually reach the value 1, no matter what positive integer n one starts with. Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.
+Although the conjecture has been computationally tested for extremely large values, it remains unproven to this day.
 
 ### The compressed form
 
 *(definition partially inspired by the [relevant article on Wikipedia](https://en.wikipedia.org/wiki/Collatz_conjecture))*
 
 Since 3n+1 is even whenever n is odd, one may instead use the "compressed" form of the Collatz function:
 
@@ -112,14 +113,20 @@
 
 * pydot: version 1.4.2 or above
 
 	```sh
 	pip install pydot
 	```
 
+* more-itertools: version 9.1.0 or above
+
+	```sh
+	pip install more-itertools
+	```
+
 ### Installation
 
 Install from PyPi with:
 
 ```sh
 pip install syracuse
 ```
@@ -128,15 +135,69 @@
 
 ```sh
 pip install syracuse-X.Y.Z-py3-none-any.whl
 ```
 
 ## Usage
 
-Please refer to the [documentation](https://devfred78.github.io/syracuse/).
+Basic usage:
+
+```pycon
+>>> # Import the core library
+>>> import syracuse
+
+>>> # Create a Syracuse sequence with 27 as initial value
+>>> my_sequence = syracuse.Syracuse(27)
+
+>>> # Stopping time
+>>> my_sequence.stopping_time
+96
+>>> # Total stopping time
+>>> my_sequence.total_stopping_time
+111
+>>> # Maximum reached value
+>>> my_sequence.max
+9232
+>>> # Full sequence (until 1)
+>>> my_sequence.total_stopping_sequence
+(27, 82, 41, 124, 62, 31, 94, 47, 142, 71, 214, 107, 322, 161,
+ 484, 242, 121, 364, 182, 91, 274, 137, 412, 206, 103, 310, 155,
+ 466, 233, 700, 350, 175, 526, 263, 790, 395, 1186, 593, 1780,
+ 890, 445, 1336, 668, 334, 167, 502, 251, 754, 377, 1132, 566,
+ 283, 850, 425, 1276, 638, 319, 958, 479, 1438, 719, 2158, 1079,
+ 3238, 1619, 4858, 2429, 7288, 3644, 1822, 911, 2734, 1367, 4102,
+ 2051, 6154, 3077, 9232, 4616, 2308, 1154, 577, 1732, 866, 433,
+ 1300, 650, 325, 976, 488, 244, 122, 61, 184, 92, 46, 23, 70, 35,
+ 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1)
+
+>>> # Import the sequences library
+>>> import syracuse.sequences
+
+>>> # Create an iterator over the records of the max values (A006884)
+>>> # with all possible optimizations
+>>> max_records = syracuse.sequences.max_value_records(15)
+
+>>> # Iterate over the first 30 records
+>>> for _ in range(30):
+...		print(f"{next(max_records)}, ", end="", flush=True)
+...
+1, 2, 3, 7, 15, 27, 255, 447, 639, 703, 1819, 4255, 4591, 9663,
+20895, 26623, 31911, 60975, 77671, 113383, 138367, 159487, 270271,
+665215, 704511, 1042431, 1212415, 1441407, 1875711, 1988859,
+
+>>> # Import the drawing library
+>>> import syracuse.drawing
+
+>>> # Display the full sequence in a Matplotlib window
+>>> syracuse.drawing.single_sequence_to_matplotlib_figure(my_sequence, test=True)
+```
+
+![Matplotlib graphical view of the successive values of the sequence Syracuse(27)](https://github.com/devfred78/syracuse/blob/main/assets/graph_sequence_27_reduced.png?raw=True)
+
+For deeper explanations, please refer to the [documentation](https://devfred78.github.io/syracuse/).
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement" or "bug", according to whether you want to share a proposal of a new function, or to record an anomaly.
```

