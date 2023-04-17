# Comparing `tmp/jupyter-summarytools-0.2.1.tar.gz` & `tmp/jupyter-summarytools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-summarytools-0.2.1.tar", last modified: Fri Nov  4 02:05:38 2022, max compression
+gzip compressed data, was "jupyter-summarytools-0.2.3.tar", last modified: Mon Apr 17 03:03:38 2023, max compression
```

## Comparing `jupyter-summarytools-0.2.1.tar` & `jupyter-summarytools-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chaoranliu   (501) staff       (20)        0 2022-11-04 02:05:38.721888 jupyter-summarytools-0.2.1/
--rw-r--r--   0 chaoranliu   (501) staff       (20)     1073 2022-10-31 07:55:08.000000 jupyter-summarytools-0.2.1/LICENSE.txt
--rw-r--r--   0 chaoranliu   (501) staff       (20)     2796 2022-11-04 02:05:38.722124 jupyter-summarytools-0.2.1/PKG-INFO
--rw-r--r--   0 chaoranliu   (501) staff       (20)     1823 2022-11-03 03:43:34.000000 jupyter-summarytools-0.2.1/README.md
--rw-r--r--   0 chaoranliu   (501) staff       (20)      192 2022-11-03 03:17:44.000000 jupyter-summarytools-0.2.1/pyproject.toml
--rw-r--r--   0 chaoranliu   (501) staff       (20)       78 2022-11-04 02:05:38.723386 jupyter-summarytools-0.2.1/setup.cfg
--rw-r--r--   0 chaoranliu   (501) staff       (20)     8529 2022-11-04 02:05:25.000000 jupyter-summarytools-0.2.1/setup.py
-drwxr-xr-x   0 chaoranliu   (501) staff       (20)        0 2022-11-04 02:05:38.704415 jupyter-summarytools-0.2.1/src/
-drwxr-xr-x   0 chaoranliu   (501) staff       (20)        0 2022-11-04 02:05:38.716714 jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/
--rw-r--r--   0 chaoranliu   (501) staff       (20)     2796 2022-11-04 02:05:38.000000 jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/PKG-INFO
--rw-r--r--   0 chaoranliu   (501) staff       (20)      388 2022-11-04 02:05:38.000000 jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/SOURCES.txt
--rw-r--r--   0 chaoranliu   (501) staff       (20)        1 2022-11-04 02:05:38.000000 jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/dependency_links.txt
--rw-r--r--   0 chaoranliu   (501) staff       (20)      101 2022-11-04 02:05:38.000000 jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/requires.txt
--rw-r--r--   0 chaoranliu   (501) staff       (20)       13 2022-11-04 02:05:38.000000 jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/top_level.txt
-drwxr-xr-x   0 chaoranliu   (501) staff       (20)        0 2022-11-04 02:05:38.720453 jupyter-summarytools-0.2.1/src/summarytools/
--rw-r--r--   0 chaoranliu   (501) staff       (20)      102 2022-11-04 02:05:15.000000 jupyter-summarytools-0.2.1/src/summarytools/__init__.py
--rw-r--r--   0 chaoranliu   (501) staff       (20)     6025 2022-11-04 02:04:24.000000 jupyter-summarytools-0.2.1/src/summarytools/htmlwidgets.py
--rw-r--r--   0 chaoranliu   (501) staff       (20)     8085 2022-11-03 07:54:19.000000 jupyter-summarytools-0.2.1/src/summarytools/summarytools.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:03:38.764386 jupyter-summarytools-0.2.3/
+-rw-rw-rw-   0        0        0    11556 2023-04-17 02:58:14.000000 jupyter-summarytools-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3363 2023-04-17 03:03:38.764386 jupyter-summarytools-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2365 2023-04-17 02:53:14.000000 jupyter-summarytools-0.2.3/README.md
+-rw-rw-rw-   0        0        0      198 2023-04-15 01:51:35.000000 jupyter-summarytools-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-04-17 03:03:38.768386 jupyter-summarytools-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     8711 2023-04-17 03:01:17.000000 jupyter-summarytools-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:03:38.726754 jupyter-summarytools-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:03:38.760385 jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/
+-rw-rw-rw-   0        0        0     3363 2023-04-17 03:03:38.000000 jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-04-17 03:03:38.000000 jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:03:38.000000 jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-17 03:03:38.000000 jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 03:03:38.000000 jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 03:03:38.763386 jupyter-summarytools-0.2.3/src/summarytools/
+-rw-rw-rw-   0        0        0      104 2023-04-15 01:51:35.000000 jupyter-summarytools-0.2.3/src/summarytools/__init__.py
+-rw-rw-rw-   0        0        0     7367 2023-04-15 01:51:35.000000 jupyter-summarytools-0.2.3/src/summarytools/htmlwidgets.py
+-rw-rw-rw-   0        0        0     8804 2023-04-15 01:51:35.000000 jupyter-summarytools-0.2.3/src/summarytools/summarytools.py
```

### Comparing `jupyter-summarytools-0.2.1/PKG-INFO` & `jupyter-summarytools-0.2.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,102 @@
-Metadata-Version: 2.1
-Name: jupyter-summarytools
-Version: 0.2.1
-Summary: summarytools in jupyter notebook
-Home-page: https://github.com/6chaoran/jupyter-summarytools
-Author: Liu Chaoran
-Author-email: 6chaoran@gmail.com
-Project-URL: Bug Reports, https://github.com/6chaoran/jupyter-summarytools/issues
-Keywords: sample,setuptools,development
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE.txt
-
-# DataFrame Summary Tools in Jupyter Notebook
-
-This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
-
-The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
-
-* Only `dfSummary` function is made available for now
-* Added two html widgets to avoid displaying lengthy content
-    + [collapsible summary](#collapsible-summary) 
-    + [tabbed summary](#tabbed-summary)
-
-# Installation
-
-```
-pip install jupyter-summarytools
-```
-
-## Dependencies
-1. python 3.6+
-2. pandas >= 1.4.0
-
-# Quick Start
-
-the quick-start notebook is available in [here](quick-start.ipynb)
-
-out-of-box `dfSummary` function will generate a HTML based data frame summary.
-
-```py
-import pandas as pd
-from summarytools import dfSummary
-titanic = pd.read_csv('./data/titanic.csv')
-dfSummary(titanic)
-```
-![](images/dfSummary.png)
-
-## collapsible summary
-
-```py
-import pandas as pd
-from summarytools import dfSummary
-titanic = pd.read_csv('./data/titanic.csv')
-dfSummary(titanic, is_collapsible = True)
-```
-
-![](images/collapsible.gif)
-
-## tabbed summary
-
-```py
-import pandas as pd
-from summarytools import dfSummary, tabset
-titanic = pd.read_csv('./data/titanic.csv')
-vaccine = pd.read_csv('./data/country_vaccinations.csv')
-vaccine['date'] = pd.to_datetime(vaccine['date'])
-
-tabset({
-    'titanic': dfSummary(titanic).render(),
-    'vaccine': dfSummary(vaccine).render()})
-```
-
-![](images/tabbed.gif)
-
-# Export notebook as HTML
-
-when export jupyter notebook to HTML, make sure `Export Embedded HTML
-` extension is installed and enabled.
-
-![](images/embedded_html.png)
-
-Using the following bash command to retain the data frame summary in exported HTML.
-```bash
-jupyter nbconvert --to html_embed path/of/your/notebook.ipynb
-```
+Metadata-Version: 2.1
+Name: jupyter-summarytools
+Version: 0.2.3
+Summary: summarytools in jupyter notebook
+Home-page: https://github.com/6chaoran/jupyter-summarytools
+Author: Liu Chaoran
+Author-email: 6chaoran@gmail.com
+Project-URL: Bug Reports, https://github.com/6chaoran/jupyter-summarytools/issues
+Keywords: sample,setuptools,development
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE.txt
+
+![GitHub](https://img.shields.io/github/license/6chaoran/jupyter-summarytools) 
+
+![PyPI](https://img.shields.io/pypi/v/summarytools?color=blue) ![PyPI - Status](https://img.shields.io/pypi/status/summarytools?color=blue) ![PyPI - Downloads](https://img.shields.io/pypi/dm/summarytools?color=blue) ![GitHub last commit](https://img.shields.io/github/last-commit/6chaoran/jupyter-summarytools?color=blue)
+
+# DataFrame Summary Tools in Jupyter Notebook
+
+This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
+
+The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
+
+* Only `dfSummary` function is made available for now
+* Added two html widgets to avoid displaying lengthy content
+    + [collapsible summary](#collapsible-summary) 
+    + [tabbed summary](#tabbed-summary)
+
+# Installation
+
+```
+pip install jupyter-summarytools
+```
+
+## Dependencies
+1. python 3.6+
+2. pandas >= 1.4.0
+
+# Quick Start
+
+the quick-start notebook is available in [here](https://github.com/6chaoran/jupyter-summarytools/blob/master/quick-start.ipynb)
+
+out-of-box `dfSummary` function will generate a HTML based data frame summary.
+
+```py
+import pandas as pd
+from summarytools import dfSummary
+titanic = pd.read_csv('./data/titanic.csv')
+dfSummary(titanic)
+```
+![](images/dfSummary.png)
+
+## collapsible summary
+
+```py
+import pandas as pd
+from summarytools import dfSummary
+titanic = pd.read_csv('./data/titanic.csv')
+dfSummary(titanic, is_collapsible = True)
+```
+
+![](images/collapsible.gif)
+
+## tabbed summary
+
+```py
+import pandas as pd
+from summarytools import dfSummary, tabset
+titanic = pd.read_csv('./data/titanic.csv')
+vaccine = pd.read_csv('./data/country_vaccinations.csv')
+vaccine['date'] = pd.to_datetime(vaccine['date'])
+
+tabset({
+    'titanic': dfSummary(titanic).render(),
+    'vaccine': dfSummary(vaccine).render()})
+```
+
+![](images/tabbed.gif)
+
+# Export notebook as HTML
+
+when export jupyter notebook to HTML, make sure `Export Embedded HTML
+` extension is installed and enabled.
+
+![](images/embedded_html.png)
+
+Using the following bash command to retain the data frame summary in exported HTML.
+```bash
+jupyter nbconvert --to html_embed path/of/your/notebook.ipynb
+```
```

### Comparing `jupyter-summarytools-0.2.1/setup.py` & `jupyter-summarytools-0.2.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-"""A setuptools based setup module.
-
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-"""
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-# Get the long description from the README file
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-# Arguments marked as "Required" below must be included for upload to PyPI.
-# Fields marked as "Optional" may be commented out.
-
-setup(
-    # This is the name of your project. The first time you publish this
-    # package, this name will be registered for you. It will determine how
-    # users can install this project, e.g.:
-    #
-    # $ pip install sampleproject
-    #
-    # And where it will live on PyPI: https://pypi.org/project/sampleproject/
-    #
-    # There are some restrictions on what makes a valid project name
-    # specification here:
-    # https://packaging.python.org/specifications/core-metadata/#name
-    name="jupyter-summarytools",  # Required
-    # Versions should comply with PEP 440:
-    # https://www.python.org/dev/peps/pep-0440/
-    #
-    # For a discussion on single-sourcing the version across setup.py and the
-    # project code, see
-    # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.2.1",  # Required
-    # This is a one-line description or tagline of what your project does. This
-    # corresponds to the "Summary" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#summary
-    description="summarytools in jupyter notebook",  # Optional
-    # This is an optional longer description of your project that represents
-    # the body of text which users will see when they visit PyPI.
-    #
-    # Often, this is the same as your README, so you can just read it in from
-    # that file directly (as we have already done above)
-    #
-    # This field corresponds to the "Description" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#description-optional
-    long_description=long_description,  # Optional
-    # Denotes that our long_description is in Markdown; valid values are
-    # text/plain, text/x-rst, and text/markdown
-    #
-    # Optional if long_description is written in reStructuredText (rst) but
-    # required for plain-text or Markdown; if unspecified, "applications should
-    # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
-    # fall back to text/plain if it is not valid rst" (see link below)
-    #
-    # This field corresponds to the "Description-Content-Type" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
-    long_description_content_type="text/markdown",  # Optional (see note above)
-    # This should be a valid link to your project's main homepage.
-    #
-    # This field corresponds to the "Home-Page" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url="https://github.com/6chaoran/jupyter-summarytools",  # Optional
-    # This should be your name or the name of the organization which owns the
-    # project.
-    author="Liu Chaoran",  # Optional
-    # This should be a valid email address corresponding to the author listed
-    # above.
-    author_email="6chaoran@gmail.com",  # Optional
-    # Classifiers help users find your project by categorizing it.
-    #
-    # For a list of valid classifiers, see https://pypi.org/classifiers/
-    classifiers=[  # Optional
-        # How mature is this project? Common values are
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
-        # Indicate who your project is intended for
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        # Pick your license as you wish
-        "License :: OSI Approved :: MIT License",
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate you support Python 3. These classifiers are *not*
-        # checked by 'pip install'. See instead 'python_requires' below.
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-    ],
-    # This field adds keywords for your project which will appear on the
-    # project page. What does your project relate to?
-    #
-    # Note that this is a list of additional keywords, separated
-    # by commas, to be used to assist searching for the distribution in a
-    # larger catalog.
-    keywords="sample, setuptools, development",  # Optional
-    # When your source code is in a subdirectory under the project root, e.g.
-    # `src/`, it is necessary to specify the `package_dir` argument.
-    package_dir={"": "src"},  # Optional
-    # You can just specify package directories manually here if your project is
-    # simple. Or you can use find_packages().
-    #
-    # Alternatively, if you just want to distribute a single Python file, use
-    # the `py_modules` argument instead as follows, which will expect a file
-    # called `my_module.py` to exist:
-    #
-    #   py_modules=["my_module"],
-    #
-    packages=find_packages(where="src"),  # Required
-    # Specify which Python versions you support. In contrast to the
-    # 'Programming Language' classifiers above, 'pip install' will check this
-    # and refuse to install the project if the version does not match. See
-    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.6",
-    # This field lists other packages that your project depends on to run.
-    # Any package you put here will be installed by pip when your project is
-    # installed, so they must be valid existing projects.
-    #
-    # For an analysis of "install_requires" vs pip's requirements files see:
-    # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=[
-        "pandas>=1.4.0",
-        "ipython>=7.20.0",
-        "numpy>=1.18.5",
-        "matplotlib>=3.3.0"
-    ],  # Optional
-    # List additional groups of dependencies here (e.g. development
-    # dependencies). Users will be able to install these using the "extras"
-    # syntax, for example:
-    #
-    #   $ pip install sampleproject[dev]
-    #
-    # Similar to `install_requires` above, these must be valid existing
-    # projects.
-    extras_require={  # Optional
-        "dev": ["check-manifest"],
-        "test": ["coverage"],
-    },
-    # If there are data files included in your packages that need to be
-    # installed, specify them here.
-    package_data={  # Optional
-        # "sample": ["package_data.dat"],
-    },
-    # Although 'package_data' is the preferred approach, in some case you may
-    # need to place data files outside of your packages. See:
-    # http://docs.python.org/distutils/setupscript.html#installing-additional-files
-    #
-    # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
-    # data_files=[("my_data", ["data/data_file"])],  # Optional
-    # To provide executable scripts, use entry points in preference to the
-    # "scripts" keyword. Entry points provide cross-platform support and allow
-    # `pip` to create the appropriate form of executable for the target
-    # platform.
-    #
-    # For example, the following would provide a command called `sample` which
-    # executes the function `main` from this package when invoked:
-    # entry_points={  # Optional
-    #     "console_scripts": [
-    #         "sample=sample:main",
-    #     ],
-    # },
-    # List additional URLs that are relevant to your project as a dict.
-    #
-    # This field corresponds to the "Project-URL" metadata fields:
-    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-    #
-    # Examples listed include a pattern for specifying where the package tracks
-    # issues, where the source is hosted, where to say thanks to the package
-    # maintainers, and where to support the project financially. The key is
-    # what's used to render the link text on PyPI.
-    project_urls={  # Optional
-        "Bug Reports": "https://github.com/6chaoran/jupyter-summarytools/issues",
-    },
+"""A setuptools based setup module.
+
+See:
+https://packaging.python.org/guides/distributing-packages-using-setuptools/
+https://github.com/pypa/sampleproject
+"""
+
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+
+# Get the long description from the README file
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+# Arguments marked as "Required" below must be included for upload to PyPI.
+# Fields marked as "Optional" may be commented out.
+
+setup(
+    # This is the name of your project. The first time you publish this
+    # package, this name will be registered for you. It will determine how
+    # users can install this project, e.g.:
+    #
+    # $ pip install sampleproject
+    #
+    # And where it will live on PyPI: https://pypi.org/project/sampleproject/
+    #
+    # There are some restrictions on what makes a valid project name
+    # specification here:
+    # https://packaging.python.org/specifications/core-metadata/#name
+    name="jupyter-summarytools",  # Required
+    # Versions should comply with PEP 440:
+    # https://www.python.org/dev/peps/pep-0440/
+    #
+    # For a discussion on single-sourcing the version across setup.py and the
+    # project code, see
+    # https://packaging.python.org/guides/single-sourcing-package-version/
+    version="0.2.3",  # Required
+    # This is a one-line description or tagline of what your project does. This
+    # corresponds to the "Summary" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#summary
+    description="summarytools in jupyter notebook",  # Optional
+    # This is an optional longer description of your project that represents
+    # the body of text which users will see when they visit PyPI.
+    #
+    # Often, this is the same as your README, so you can just read it in from
+    # that file directly (as we have already done above)
+    #
+    # This field corresponds to the "Description" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#description-optional
+    long_description=long_description,  # Optional
+    # Denotes that our long_description is in Markdown; valid values are
+    # text/plain, text/x-rst, and text/markdown
+    #
+    # Optional if long_description is written in reStructuredText (rst) but
+    # required for plain-text or Markdown; if unspecified, "applications should
+    # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
+    # fall back to text/plain if it is not valid rst" (see link below)
+    #
+    # This field corresponds to the "Description-Content-Type" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
+    long_description_content_type="text/markdown",  # Optional (see note above)
+    # This should be a valid link to your project's main homepage.
+    #
+    # This field corresponds to the "Home-Page" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#home-page-optional
+    url="https://github.com/6chaoran/jupyter-summarytools",  # Optional
+    # This should be your name or the name of the organization which owns the
+    # project.
+    author="Liu Chaoran",  # Optional
+    # This should be a valid email address corresponding to the author listed
+    # above.
+    author_email="6chaoran@gmail.com",  # Optional
+    # Classifiers help users find your project by categorizing it.
+    #
+    # For a list of valid classifiers, see https://pypi.org/classifiers/
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        "Development Status :: 3 - Alpha",
+        # Indicate who your project is intended for
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        # Pick your license as you wish
+        "License :: OSI Approved :: MIT License",
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate you support Python 3. These classifiers are *not*
+        # checked by 'pip install'. See instead 'python_requires' below.
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+    ],
+    # This field adds keywords for your project which will appear on the
+    # project page. What does your project relate to?
+    #
+    # Note that this is a list of additional keywords, separated
+    # by commas, to be used to assist searching for the distribution in a
+    # larger catalog.
+    keywords="sample, setuptools, development",  # Optional
+    # When your source code is in a subdirectory under the project root, e.g.
+    # `src/`, it is necessary to specify the `package_dir` argument.
+    package_dir={"": "src"},  # Optional
+    # You can just specify package directories manually here if your project is
+    # simple. Or you can use find_packages().
+    #
+    # Alternatively, if you just want to distribute a single Python file, use
+    # the `py_modules` argument instead as follows, which will expect a file
+    # called `my_module.py` to exist:
+    #
+    #   py_modules=["my_module"],
+    #
+    packages=find_packages(where="src"),  # Required
+    # Specify which Python versions you support. In contrast to the
+    # 'Programming Language' classifiers above, 'pip install' will check this
+    # and refuse to install the project if the version does not match. See
+    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
+    python_requires=">=3.6",
+    # This field lists other packages that your project depends on to run.
+    # Any package you put here will be installed by pip when your project is
+    # installed, so they must be valid existing projects.
+    #
+    # For an analysis of "install_requires" vs pip's requirements files see:
+    # https://packaging.python.org/discussions/install-requires-vs-requirements/
+    install_requires=[
+        "pandas>=1.4.0",
+        "ipython>=7.20.0",
+        "numpy>=1.18.5",
+        "matplotlib>=3.3.0"
+    ],  # Optional
+    # List additional groups of dependencies here (e.g. development
+    # dependencies). Users will be able to install these using the "extras"
+    # syntax, for example:
+    #
+    #   $ pip install sampleproject[dev]
+    #
+    # Similar to `install_requires` above, these must be valid existing
+    # projects.
+    extras_require={  # Optional
+        "dev": ["check-manifest"],
+        "test": ["coverage"],
+    },
+    # If there are data files included in your packages that need to be
+    # installed, specify them here.
+    package_data={  # Optional
+        # "sample": ["package_data.dat"],
+    },
+    # Although 'package_data' is the preferred approach, in some case you may
+    # need to place data files outside of your packages. See:
+    # http://docs.python.org/distutils/setupscript.html#installing-additional-files
+    #
+    # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
+    # data_files=[("my_data", ["data/data_file"])],  # Optional
+    # To provide executable scripts, use entry points in preference to the
+    # "scripts" keyword. Entry points provide cross-platform support and allow
+    # `pip` to create the appropriate form of executable for the target
+    # platform.
+    #
+    # For example, the following would provide a command called `sample` which
+    # executes the function `main` from this package when invoked:
+    # entry_points={  # Optional
+    #     "console_scripts": [
+    #         "sample=sample:main",
+    #     ],
+    # },
+    # List additional URLs that are relevant to your project as a dict.
+    #
+    # This field corresponds to the "Project-URL" metadata fields:
+    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+    #
+    # Examples listed include a pattern for specifying where the package tracks
+    # issues, where the source is hosted, where to say thanks to the package
+    # maintainers, and where to support the project financially. The key is
+    # what's used to render the link text on PyPI.
+    project_urls={  # Optional
+        "Bug Reports": "https://github.com/6chaoran/jupyter-summarytools/issues",
+    },
 )
```

### Comparing `jupyter-summarytools-0.2.1/src/jupyter_summarytools.egg-info/PKG-INFO` & `jupyter-summarytools-0.2.3/src/jupyter_summarytools.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,102 @@
-Metadata-Version: 2.1
-Name: jupyter-summarytools
-Version: 0.2.1
-Summary: summarytools in jupyter notebook
-Home-page: https://github.com/6chaoran/jupyter-summarytools
-Author: Liu Chaoran
-Author-email: 6chaoran@gmail.com
-Project-URL: Bug Reports, https://github.com/6chaoran/jupyter-summarytools/issues
-Keywords: sample,setuptools,development
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE.txt
-
-# DataFrame Summary Tools in Jupyter Notebook
-
-This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
-
-The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
-
-* Only `dfSummary` function is made available for now
-* Added two html widgets to avoid displaying lengthy content
-    + [collapsible summary](#collapsible-summary) 
-    + [tabbed summary](#tabbed-summary)
-
-# Installation
-
-```
-pip install jupyter-summarytools
-```
-
-## Dependencies
-1. python 3.6+
-2. pandas >= 1.4.0
-
-# Quick Start
-
-the quick-start notebook is available in [here](quick-start.ipynb)
-
-out-of-box `dfSummary` function will generate a HTML based data frame summary.
-
-```py
-import pandas as pd
-from summarytools import dfSummary
-titanic = pd.read_csv('./data/titanic.csv')
-dfSummary(titanic)
-```
-![](images/dfSummary.png)
-
-## collapsible summary
-
-```py
-import pandas as pd
-from summarytools import dfSummary
-titanic = pd.read_csv('./data/titanic.csv')
-dfSummary(titanic, is_collapsible = True)
-```
-
-![](images/collapsible.gif)
-
-## tabbed summary
-
-```py
-import pandas as pd
-from summarytools import dfSummary, tabset
-titanic = pd.read_csv('./data/titanic.csv')
-vaccine = pd.read_csv('./data/country_vaccinations.csv')
-vaccine['date'] = pd.to_datetime(vaccine['date'])
-
-tabset({
-    'titanic': dfSummary(titanic).render(),
-    'vaccine': dfSummary(vaccine).render()})
-```
-
-![](images/tabbed.gif)
-
-# Export notebook as HTML
-
-when export jupyter notebook to HTML, make sure `Export Embedded HTML
-` extension is installed and enabled.
-
-![](images/embedded_html.png)
-
-Using the following bash command to retain the data frame summary in exported HTML.
-```bash
-jupyter nbconvert --to html_embed path/of/your/notebook.ipynb
-```
+Metadata-Version: 2.1
+Name: jupyter-summarytools
+Version: 0.2.3
+Summary: summarytools in jupyter notebook
+Home-page: https://github.com/6chaoran/jupyter-summarytools
+Author: Liu Chaoran
+Author-email: 6chaoran@gmail.com
+Project-URL: Bug Reports, https://github.com/6chaoran/jupyter-summarytools/issues
+Keywords: sample,setuptools,development
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE.txt
+
+![GitHub](https://img.shields.io/github/license/6chaoran/jupyter-summarytools) 
+
+![PyPI](https://img.shields.io/pypi/v/summarytools?color=blue) ![PyPI - Status](https://img.shields.io/pypi/status/summarytools?color=blue) ![PyPI - Downloads](https://img.shields.io/pypi/dm/summarytools?color=blue) ![GitHub last commit](https://img.shields.io/github/last-commit/6chaoran/jupyter-summarytools?color=blue)
+
+# DataFrame Summary Tools in Jupyter Notebook
+
+This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
+
+The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
+
+* Only `dfSummary` function is made available for now
+* Added two html widgets to avoid displaying lengthy content
+    + [collapsible summary](#collapsible-summary) 
+    + [tabbed summary](#tabbed-summary)
+
+# Installation
+
+```
+pip install jupyter-summarytools
+```
+
+## Dependencies
+1. python 3.6+
+2. pandas >= 1.4.0
+
+# Quick Start
+
+the quick-start notebook is available in [here](https://github.com/6chaoran/jupyter-summarytools/blob/master/quick-start.ipynb)
+
+out-of-box `dfSummary` function will generate a HTML based data frame summary.
+
+```py
+import pandas as pd
+from summarytools import dfSummary
+titanic = pd.read_csv('./data/titanic.csv')
+dfSummary(titanic)
+```
+![](images/dfSummary.png)
+
+## collapsible summary
+
+```py
+import pandas as pd
+from summarytools import dfSummary
+titanic = pd.read_csv('./data/titanic.csv')
+dfSummary(titanic, is_collapsible = True)
+```
+
+![](images/collapsible.gif)
+
+## tabbed summary
+
+```py
+import pandas as pd
+from summarytools import dfSummary, tabset
+titanic = pd.read_csv('./data/titanic.csv')
+vaccine = pd.read_csv('./data/country_vaccinations.csv')
+vaccine['date'] = pd.to_datetime(vaccine['date'])
+
+tabset({
+    'titanic': dfSummary(titanic).render(),
+    'vaccine': dfSummary(vaccine).render()})
+```
+
+![](images/tabbed.gif)
+
+# Export notebook as HTML
+
+when export jupyter notebook to HTML, make sure `Export Embedded HTML
+` extension is installed and enabled.
+
+![](images/embedded_html.png)
+
+Using the following bash command to retain the data frame summary in exported HTML.
+```bash
+jupyter nbconvert --to html_embed path/of/your/notebook.ipynb
+```
```

### Comparing `jupyter-summarytools-0.2.1/src/summarytools/summarytools.py` & `jupyter-summarytools-0.2.3/src/summarytools/summarytools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,239 +1,249 @@
-from pathlib import Path
-from matplotlib import pyplot as plt
-from pandas.api.types import is_datetime64_any_dtype as _is_datetime
-import numpy as np
-import pandas as pd
-from IPython.display import HTML, display
-import inspect
-from .htmlwidgets import collapsible, tabset
-
-def _is_numerical(x:pd.Series):
-    return (x.dtype == int) or (x.dtype == float)
-
-def _is_categorical(x: pd.Series, num_unique, max_level):
-    try:
-        if x.dtype == 'category':
-            return True
-    except:
-        pass
-    if x.dtype == 'object':
-        return True
-    if x.dtype in ['int', 'float']:
-        if num_unique <= max_level:
-            return True
-    return False
-
-def _is_bool(x: pd.Series):
-    return x.dtype == bool
-
-def _graph_cat_col(stats, filename, figsize):
-    fig = plt.figure(figsize=figsize)
-    pct = stats / stats.sum()
-    plt.barh(pct.index, pct, color='gray', alpha=0.3, edgecolor='black')
-    plt.gca().invert_yaxis()
-    plt.xlim(0, 1)
-    plt.axis('off')
-    fig.savefig(filename, bbox_inches='tight', pad_inches=0)
-    plt.close()
-    return f'<img src = "{filename}"></img>'
-
-
-def _graph_num_col(x, filename, figsize):
-    fig = plt.figure(figsize=figsize)
-    x = x[~x.isna()]
-    _ = plt.hist(x, bins=10, color='gray', edgecolor='black', alpha=0.3)
-    plt.axis('off')
-    plt.tight_layout()
-    fig.savefig(filename, bbox_inches='tight', pad_inches=0)
-    plt.close()
-    return f'<img src = "{filename}"></img>'
-
-
-def _graph_date_col(x: pd.Series, filename, figsize):
-    freqs = (x - x.min()).map(lambda x: x.days)
-    fig = plt.figure(figsize=figsize)
-    plt.hist(freqs, bins=10, color='gray', alpha=0.3, ec='black')
-    plt.axis('off')
-    fig.savefig(filename, bbox_inches='tight', pad_inches=0)
-    plt.close()
-    return f'<img src = "{filename}"></img>'
-
-
-def _stats_date_col(x: pd.Series, show_graph: bool, filename: str):
-
-    stats = f"Min: {x.min().strftime('%Y-%m-%d')}<br>"
-    stats += f"Max: {x.max().strftime('%Y-%m-%d')}<br>"
-    stats += f"Duration: {(x.max() - x.min()).days:,} days"
-
-    freqs = f"{x.nunique()} distinct values"
-
-    out = {
-        'Stats / Values': stats,
-        'Freqs / (% of Valid)': freqs}
-
-    if show_graph:
-        graph = _graph_date_col(x, filename, figsize=(2, 1))
-        out['Graph'] = graph
-
-    return out
-
-
-def _stats_cat_col(x: pd.Series, max_level: int, show_graph: bool, filename: str, max_str_len=30):
-
-    stats = x.astype(str).value_counts()
-    values = [f'{i+1}. {v[:max_str_len]}' for i, v in enumerate(stats.index)]
-    total = stats.values.sum()
-    freqs = stats.map(lambda i: f"{i:,} ({i/total:.1%})")
-
-    if len(stats) > max_level:
-        values = [f'{i+1}. {v[:max_str_len]}' for i,
-                  v in enumerate(stats.index[:max_level])]
-        values += [f'{max_level + 1}. other']
-        freqs = stats[:max_level].map(
-            lambda i: f"{i:,} ({i/total:.1%})").to_list()
-        freqs += [f"{stats[max_level:].sum():,} ({stats[max_level:].sum()/total:.1%})"]
-        stats = pd.concat([stats.head(max_level), 
-            pd.Series({'other': stats[max_level:].sum()})])
-
-    out = {
-        'Stats / Values': '<br>'.join(values),
-        'Freqs / (% of Valid)': '<br>'.join(freqs)}
-
-    if show_graph:
-        graph = _graph_cat_col(stats, filename, figsize=(2, 0.3 * len(stats)))
-        out['Graph'] = graph
-
-    return out
-
-
-def _stats_num_col(x: pd.Series, show_graph: bool, filename: str):
-
-    stats = f"Mean (sd) : {x.mean():.1f} ({x.std():.1f})"
-    stats += f"<br>min < med < max:"
-    stats += f"<br>{x.min():.1f} < {x.median():.1f} < {x.max():.1f}"
-    stats += f"<br>IQR (CV) : {x.quantile(0.75) - x.quantile(0.25):.1f} ({x.mean()/x.std():.1f})"
-
-    values = f"{x.nunique():,} distinct values"
-
-    out = {
-        'Stats / Values': stats,
-        'Freqs / (% of Valid)': values}
-
-    if show_graph:
-        graph = _graph_num_col(x, filename, figsize=(2, 1))
-        out['Graph'] = graph
-
-    return out
-
-
-def _var_name(var):
-    lcls = inspect.stack()[2][0].f_locals
-    for name in lcls:
-        if id(var) == id(lcls[name]):
-            return name
-    return ""
-    
-
-def dfSummary(data: pd.DataFrame, max_level: int = 10,
-              show_graph: bool = True, tmp_dir: str = './tmp',
-              is_collapsible=False):
-    """generate HTML data summary
-
-    Args:
-        data (pd.DataFrame): [input dataframe]
-        max_level (int, optional): [max level of categorical variable to be shown]. Defaults to 10.
-        show_graph (bool, optional): [flag to show Graph column]. Defaults to True.
-        tmp_dir (str, optional): [directory for temporary images]. Defaults to './tmp'.
-        is_collapsible (bool, optional): [flag for collapsible page]. Defaults to False.
-
-    Returns:
-        [Pandas.Styler]: if is_collapsible = False
-        [HTML]: if is_collapisbile = True
-
-    Examples:
-    ```
-    from summarytools import dfSummary
-    import pandas as pd
-    data = pd.read_csv('./your-data-path.csv')
-    # default summary view
-    dfSummary(data)
-    # collapsible summary
-    dfSummary(data, is_collapsible = True)
-    # tabbed summary
-    from summarytools import tabset
-    tab1 = dfSummary(data).to_html()
-    tabset({'tab1', tab1})
-    ```
-    """
-
-    tbl_name = _var_name(data)
-    tbl_dups = f"Duplicates: {data.duplicated().sum():,}"
-    tbl_dims = "Dimensions: {:,} x {:,}".format(*data.shape)
-    tbl_caption = "<strong>Data Frame Summary</strong><br>"
-    tbl_caption += tbl_name + "<br>" + tbl_dims + "<br>" + tbl_dups
-
-    nrows, ncols = data.shape
-    num_uniques = data.apply(pd.Series.nunique)
-
-    variable = data.columns.values.astype(str)
-    variable = [f'<strong>{i}</strong>' for i in variable]
-    no = np.arange(1, ncols + 1)
-    dtype = [f'<br>[{i}]' for i in data.dtypes.astype(str)]
-    variable = np.char.array(variable) + np.char.array(dtype)
-    out = pd.DataFrame({'No': no, 'Variable': variable})
-
-    tmp_dir = Path(tmp_dir)
-    if show_graph:
-        tmp_dir.mkdir(exist_ok=True, parents=True)
-
-    # Stats / Freqs / Graphs
-    stats = []
-    for i, v in enumerate(data.columns):
-        filename = tmp_dir.joinpath(f'{tbl_name}_{i:03d}.png')
-        if _is_categorical(data[v], num_uniques[v], max_level):
-            stats += [_stats_cat_col(data[v], max_level, show_graph, filename)]
-        elif _is_datetime(data[v]):
-            stats += [_stats_date_col(data[v], show_graph, filename)]
-        elif _is_bool(data[v]):
-            stats += [_stats_cat_col(data[v], max_level, show_graph, filename)]
-        elif _is_numerical(data[v]):
-            stats += [_stats_num_col(data[v], show_graph, filename)]
-        else:
-            pass
-    stats = pd.DataFrame(stats)
-    out = pd.concat([out, stats], axis=1)
-
-    # Missing
-    missing = np.char.array([f'{i:,}' for i in data.isna().sum()])
-    missing_pct = np.char.array([f'<br>({i:.1%})' for i in data.isna().mean()])
-    out['Missing'] = missing + missing_pct
-
-    # styles
-    out = (out.style
-           .set_properties(**{'text-align': 'left',
-                'font-size':'12px',
-                'vertical-align':'middle'})
-           .set_table_styles([{'selector':'thead>tr>th', 'props': 'text-align : left'}])
-           .set_properties(subset=['No'], **{'width':'5%', 
-                'max-width':'50px', 
-                'min-width':'20px'})
-           .set_properties(subset=['Variable'], **{'width':'15%',
-                'max-width':'200px',
-                'min-width':'100px',
-                'word-break':'break-word'})
-           .set_properties(subset=['Stats / Values'], **{'width':'30%', 
-                'min-width':'100px'})
-           .set_properties(subset=['Freqs / (% of Valid)'], **{'width':'25%',
-                'min-width':'100px'})\
-           .set_properties(subset=['Missing'], width='10%') \
-           .hide(axis='index')\
-           .set_caption(tbl_caption))
-    if show_graph:
-        out = out.set_properties(subset=['Graph'], **{'width':'20%', 'min-width':'150px'})
-
-    if is_collapsible:
-        out = out.to_html()
-        out = collapsible(out, tbl_name)
-        return HTML(out)
-
-    return out
+from pathlib import Path
+from matplotlib import pyplot as plt
+from pandas.api.types import is_datetime64_any_dtype as _is_datetime
+from pandas.api.types import is_numeric_dtype as _is_numerical
+
+import numpy as np
+import pandas as pd
+from IPython.display import HTML, display
+import inspect
+from .htmlwidgets import collapsible, tabset
+import base64
+
+def _is_categorical(x: pd.Series, num_unique, max_level):
+    try:
+        if x.dtype == 'category':
+            return True
+    except:
+        pass
+    if x.dtype == 'object':
+        return True
+    if x.dtype in ['int', 'float']:
+        if num_unique <= max_level:
+            return True
+    return False
+
+def _is_bool(x: pd.Series):
+    return x.dtype == bool
+
+def encode_img_base64(img):
+    with open(img, "rb") as image_file:
+        x = image_file.read()
+        encoded_string = base64.b64encode(x).decode()
+    src = f"data:image/png;base64, {encoded_string}"
+    return src
+
+def _graph_cat_col(stats, filename, figsize):
+    fig = plt.figure(figsize=figsize)
+    pct = stats / stats.sum()
+    plt.barh(pct.index, pct, color='gray', alpha=0.3, edgecolor='black')
+    plt.gca().invert_yaxis()
+    plt.xlim(0, 1)
+    plt.axis('off')
+    fig.savefig(filename, bbox_inches='tight', pad_inches=0, transparent=True)
+    plt.close()
+    base64str = encode_img_base64(filename)
+    return f'<img src = "{base64str}"></img>'
+
+
+def _graph_num_col(x, filename, figsize):
+    fig = plt.figure(figsize=figsize)
+    x = x[~x.isna()]
+    _ = plt.hist(x, bins=10, color='gray', edgecolor='black', alpha=0.3)
+    plt.axis('off')
+    plt.tight_layout()
+    fig.savefig(filename, bbox_inches='tight', pad_inches=0, transparent=True)
+    plt.close()
+    base64str = encode_img_base64(filename)
+    return f'<img src = "{base64str}"></img>'
+
+
+def _graph_date_col(x: pd.Series, filename, figsize):
+    freqs = (x - x.min()).map(lambda x: x.days)
+    fig = plt.figure(figsize=figsize)
+    plt.hist(freqs, bins=10, color='gray', alpha=0.3, ec='black')
+    plt.axis('off')
+    fig.savefig(filename, bbox_inches='tight', pad_inches=0, transparent=True)
+    plt.close()
+    base64str = encode_img_base64(filename)
+    return f'<img src = "{base64str}"></img>'
+
+
+def _stats_date_col(x: pd.Series, show_graph: bool, filename: str):
+
+    stats = f"Min: {x.min().strftime('%Y-%m-%d')}<br>"
+    stats += f"Max: {x.max().strftime('%Y-%m-%d')}<br>"
+    stats += f"Duration: {(x.max() - x.min()).days:,} days"
+
+    freqs = f"{x.nunique()} distinct values"
+
+    out = {
+        'Stats / Values': stats,
+        'Freqs / (% of Valid)': freqs}
+
+    if show_graph:
+        graph = _graph_date_col(x, filename, figsize=(2, 1))
+        out['Graph'] = graph
+
+    return out
+
+
+def _stats_cat_col(x: pd.Series, max_level: int, show_graph: bool, filename: str, max_str_len=30):
+
+    stats = x.astype(str).value_counts()
+    values = [f'{i+1}. {v[:max_str_len]}' for i, v in enumerate(stats.index)]
+    total = stats.values.sum()
+    freqs = stats.map(lambda i: f"{i:,} ({i/total:.1%})")
+
+    if len(stats) > max_level:
+        values = [f'{i+1}. {v[:max_str_len]}' for i,
+                  v in enumerate(stats.index[:max_level])]
+        values += [f'{max_level + 1}. other']
+        freqs = stats[:max_level].map(
+            lambda i: f"{i:,} ({i/total:.1%})").to_list()
+        freqs += [f"{stats[max_level:].sum():,} ({stats[max_level:].sum()/total:.1%})"]
+        stats = pd.concat([stats.head(max_level), 
+            pd.Series({'other': stats[max_level:].sum()})])
+
+    out = {
+        'Stats / Values': '<br>'.join(values),
+        'Freqs / (% of Valid)': '<br>'.join(freqs)}
+
+    if show_graph:
+        graph = _graph_cat_col(stats, filename, figsize=(2, 0.3 * len(stats)))
+        out['Graph'] = graph
+
+    return out
+
+
+def _stats_num_col(x: pd.Series, show_graph: bool, filename: str):
+
+    stats = f"Mean (sd) : {x.mean():.1f} ({x.std():.1f})"
+    stats += f"<br>min < med < max:"
+    stats += f"<br>{x.min():.1f} < {x.median():.1f} < {x.max():.1f}"
+    stats += f"<br>IQR (CV) : {x.quantile(0.75) - x.quantile(0.25):.1f} ({x.mean()/x.std():.1f})"
+
+    values = f"{x.nunique():,} distinct values"
+
+    out = {
+        'Stats / Values': stats,
+        'Freqs / (% of Valid)': values}
+
+    if show_graph:
+        graph = _graph_num_col(x, filename, figsize=(2, 1))
+        out['Graph'] = graph
+
+    return out
+
+
+def _var_name(var):
+    lcls = inspect.stack()[2][0].f_locals
+    for name in lcls:
+        if id(var) == id(lcls[name]):
+            return name
+    return ""
+    
+
+def dfSummary(data: pd.DataFrame, max_level: int = 10,
+              show_graph: bool = True, tmp_dir: str = './tmp',
+              is_collapsible=False):
+    """generate HTML data summary
+
+    Args:
+        data (pd.DataFrame): [input dataframe]
+        max_level (int, optional): [max level of categorical variable to be shown]. Defaults to 10.
+        show_graph (bool, optional): [flag to show Graph column]. Defaults to True.
+        tmp_dir (str, optional): [directory for temporary images]. Defaults to './tmp'.
+        is_collapsible (bool, optional): [flag for collapsible page]. Defaults to False.
+
+    Returns:
+        [Pandas.Styler]: if is_collapsible = False
+        [HTML]: if is_collapisbile = True
+
+    Examples:
+    ```
+    from summarytools import dfSummary
+    import pandas as pd
+    data = pd.read_csv('./your-data-path.csv')
+    # default summary view
+    dfSummary(data)
+    # collapsible summary
+    dfSummary(data, is_collapsible = True)
+    # tabbed summary
+    from summarytools import tabset
+    tab1 = dfSummary(data).to_html()
+    tabset({'tab1', tab1})
+    ```
+    """
+
+    tbl_name = _var_name(data)
+    tbl_dups = f"Duplicates: {data.duplicated().sum():,}"
+    tbl_dims = "Dimensions: {:,} x {:,}".format(*data.shape)
+    tbl_caption = "<strong>Data Frame Summary</strong><br>"
+    tbl_caption += tbl_name + "<br>" + tbl_dims + "<br>" + tbl_dups
+
+    nrows, ncols = data.shape
+    num_uniques = data.apply(pd.Series.nunique)
+
+    variable = data.columns.values.astype(str)
+    variable = [f'<strong>{i}</strong>' for i in variable]
+    no = np.arange(1, ncols + 1)
+    dtype = [f'<br>[{i}]' for i in data.dtypes.astype(str)]
+    variable = np.char.array(variable) + np.char.array(dtype)
+    out = pd.DataFrame({'No': no, 'Variable': variable})
+
+    tmp_dir = Path(tmp_dir)
+    if show_graph:
+        tmp_dir.mkdir(exist_ok=True, parents=True)
+
+    # Stats / Freqs / Graphs
+    stats = []
+    for i, v in enumerate(data.columns):
+        filename = tmp_dir.joinpath(f'{tbl_name}_{i:03d}.png')
+        if _is_categorical(data[v], num_uniques[v], max_level):
+            stats += [_stats_cat_col(data[v], max_level, show_graph, filename)]
+        elif _is_datetime(data[v]):
+            stats += [_stats_date_col(data[v], show_graph, filename)]
+        elif _is_bool(data[v]):
+            stats += [_stats_cat_col(data[v], max_level, show_graph, filename)]
+        elif _is_numerical(data[v]):
+            stats += [_stats_num_col(data[v], show_graph, filename)]
+        else:
+            stats += [{'Stats / Values': f'not supported dtype {data[v].dtype}'}]
+    stats = pd.DataFrame(stats)
+    out = pd.concat([out, stats], axis=1)
+
+    # Missing
+    missing = np.char.array([f'{i:,}' for i in data.isna().sum()])
+    missing_pct = np.char.array([f'<br>({i:.1%})' for i in data.isna().mean()])
+    out['Missing'] = missing + missing_pct
+
+    # styles
+    out = (out.style
+           .set_properties(**{'text-align': 'left',
+                'font-size':'12px',
+                'vertical-align':'middle'})
+           .set_table_styles([{'selector':'thead>tr>th', 'props': 'text-align : left'}])
+           .set_properties(subset=['No'], **{'width':'5%', 
+                'max-width':'50px', 
+                'min-width':'20px'})
+           .set_properties(subset=['Variable'], **{'width':'15%',
+                'max-width':'200px',
+                'min-width':'100px',
+                'word-break':'break-word'})
+           .set_properties(subset=['Stats / Values'], **{'width':'30%', 
+                'min-width':'100px'})
+           .set_properties(subset=['Freqs / (% of Valid)'], **{'width':'25%',
+                'min-width':'100px'})\
+           .set_properties(subset=['Missing'], width='10%') \
+           .hide(axis='index')\
+           .set_caption(tbl_caption))
+    if show_graph:
+        out = out.set_properties(subset=['Graph'], **{'width':'20%', 'min-width':'150px'})
+
+    if is_collapsible:
+        out = out.to_html()
+        out = collapsible(out, tbl_name)
+        return HTML(out)
+
+    return out
```

