# Comparing `tmp/clipdetect-0.1.1.tar.gz` & `tmp/clipdetect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipdetect-0.1.1.tar", max compression
+gzip compressed data, was "clipdetect-0.1.2.tar", max compression
```

## Comparing `clipdetect-0.1.1.tar` & `clipdetect-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4922 2023-02-08 21:11:47.393768 clipdetect-0.1.1/README.md
--rw-r--r--   0        0        0     3268 2023-02-08 21:09:04.487342 clipdetect-0.1.1/clipdetect/__init__.py
--rw-r--r--   0        0        0     2676 2023-02-08 21:41:15.807994 clipdetect-0.1.1/clipdetect/cli.py
--rw-r--r--   0        0        0      488 2023-02-08 21:43:28.263734 clipdetect-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5875 1970-01-01 00:00:00.000000 clipdetect-0.1.1/setup.py
--rw-r--r--   0        0        0     5639 1970-01-01 00:00:00.000000 clipdetect-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4922 2023-02-08 21:11:47.393768 clipdetect-0.1.2/README.md
+-rw-r--r--   0        0        0     3268 2023-02-08 21:09:04.487342 clipdetect-0.1.2/clipdetect/__init__.py
+-rw-r--r--   0        0        0     2676 2023-02-08 21:41:15.807994 clipdetect-0.1.2/clipdetect/cli.py
+-rw-r--r--   0        0        0      487 2023-04-17 20:29:46.615772 clipdetect-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5866 1970-01-01 00:00:00.000000 clipdetect-0.1.2/setup.py
+-rw-r--r--   0        0        0     5630 1970-01-01 00:00:00.000000 clipdetect-0.1.2/PKG-INFO
```

### Comparing `clipdetect-0.1.1/README.md` & `clipdetect-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `clipdetect-0.1.1/clipdetect/__init__.py` & `clipdetect-0.1.2/clipdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `clipdetect-0.1.1/clipdetect/cli.py` & `clipdetect-0.1.2/clipdetect/cli.py`

 * *Files identical despite different names*

### Comparing `clipdetect-0.1.1/setup.py` & `clipdetect-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 ['clipdetect']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['loguru>=0.6.0,<0.7.0',
- 'numpy>=1.24.2,<2.0.0',
+ 'numpy>=1.22',
  'pympi-ling>=1.70.2,<2.0.0',
  'pytest>=7.2.1,<8.0.0',
  'scipy>=1.10.0,<2.0.0',
  'tqdm>=4.64.1,<5.0.0',
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['clipdetect = clipdetect.cli:app']}
 
 setup_kwargs = {
     'name': 'clipdetect',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': "# ClipDetect\n\n<!-- [![codecov](https://codecov.io/gh/roedoejet/clipdetect/branch/master/graph/badge.svg)](https://codecov.io/gh/roedoejet/clipdetect) -->\n[![Build Status](https://github.com/roedoejet/clipdetect/actions/workflows/tests.yaml/badge.svg)](https://github.com/roedoejet/clipdetect/actions)\n[![PyPI package](https://img.shields.io/pypi/v/clipdetect.svg)](https://pypi.org/project/clipdetect/)\n[![license](https://img.shields.io/badge/Licence-MIT-green)](LICENSE)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/roedoejet/clipdetect)\n\n> Detect clipping in your wav files\n\n## Table of Contents\n- [ClipDetect](#clipdetect)\n  - [Table of Contents](#table-of-contents)\n  - [Background](#background)\n  - [Install](#install)\n  - [Usage](#usage)\n  - [Maintainers](#maintainers)\n  - [Contributing](#contributing)\n  - [How to Cite](#citation)\n  - [License](#license)\n\n## Background\n\nThis library is for detecting clipping in audio even if the audio has been normalized (ie does not actually produce the maximum possible value given the bit depth). It is based on [this paper](https://www.sciencedirect.com/science/article/pii/S0167639321000832) - please cite them if you use this. I'm not the original author, I just used it in a project and wanted to package it up.\n\n## Install\n\nTo use this package just run `pip install clipdetect` or `poetry add clipdetect` if you use poetry.\n\n## Usage\n\nTo detect a single file:\n\n    clipdetect path/to/file.wav\n\nTo detect all wav files in a folder:\n\n    clipdetect path/to/folder\n\n\nResults for a folder will be written to csv format.\n\n\n### Export to TextGrid\n\nThe following will export a [Praat TextGrid](https://www.fon.hum.uva.nl/praat/) of the clipping sections\n\n    clipdetect path/to/file.wav --textgrid\n\nYou can also do it for a whole folder:\n\n    clipdetect path/to/folder --textgrid\n\n\n## Maintainers\n\n[@roedoejet](https://github.com/roedoejet).\n\n\n## Contributing\n\nFeel free to dive in! [Open an issue](https://github.com/roedoejet/clipdetect/issues/new) or submit PRs.\n\nThis repo follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.\n\nHave a look at [Contributing.md](Contributing.md) for help using our standardized formatting conventions and pre-commit hooks.\n\n## Citation\n\nIf you use this work in a project of yours and write about it, please feel free to link to this repo but also cite the authors of the algorithm using the following:\n\nHansen, John H. L., Allen Stauffer, and Wei Xia. “Nonlinear Waveform Distortion: Assessment and Detection of Clipping on Speech Data and Systems.” Speech Communication 134 (2021): 20–31. https://doi.org/10.1016/j.specom.2021.07.007.\n\n\nOr in BibTeX:\n\n```\n@article{HANSEN202120,\ntitle = {Nonlinear waveform distortion: Assessment and detection of clipping on speech data and systems},\njournal = {Speech Communication},\nvolume = {134},\npages = {20-31},\nyear = {2021},\nissn = {0167-6393},\ndoi = {https://doi.org/10.1016/j.specom.2021.07.007},\nurl = {https://www.sciencedirect.com/science/article/pii/S0167639321000832},\nauthor = {John H.L. Hansen and Allen Stauffer and Wei Xia},\nkeywords = {Audio clipping, Speech quality assessment, Non-linear distortion, Speaker recognition},\nabstract = {Speech, speaker, and language systems have traditionally relied on carefully collected speech material for training acoustic models. There is an enormous amount of freely accessible audio content. A major challenge, however, is that such data is not professionally recorded, and therefore may contain a wide diversity of background noise, nonlinear distortions, or other unknown environmental or technology-based contamination or mismatch. There is a crucial need for automatic analysis to screen such unknown datasets before acoustic model development training, or to perform input audio purity screening prior to classification. In this study, we propose a waveform based clipping detection algorithm for naturalistic audio streams and examine the impact of clipping at different severities on speech quality measurements and automatic speaker recognition systems. We use the TIMIT and NIST SRE08 corpora as case studies. The results show, as expected, that clipping introduces a nonlinear distortion into clean speech data, which reduces speech quality and performance for speaker recognition. We also investigate what degree of clipping can be present to sustain effective speech system performance. The proposed detection system, which will be released, could contribute to massive new audio collections for speech and language technology development (e.g. Google Audioset (Gemmeke et al., 2017), CRSS-UTDallas Apollo Fearless-Steps (Yu et al., 2014) (19,000\xa0h naturalistic audio from NASA Apollo missions)).}\n}\n```\n\n## License\n\nMIT. See [LICENSE](LICENSE) for the Copyright and license statements.",
     'author': 'roedoejet',
     'author_email': 'hello@aidanpine.ca',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `clipdetect-0.1.1/PKG-INFO` & `clipdetect-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: clipdetect
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: roedoejet
 Author-email: hello@aidanpine.ca
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: numpy (>=1.22)
 Requires-Dist: pympi-ling (>=1.70.2,<2.0.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
```

