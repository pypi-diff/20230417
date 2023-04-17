# Comparing `tmp/bowtie_json_schema-0.82.1.tar.gz` & `tmp/bowtie_json_schema-0.9.1.tar.gz`

## Comparing `bowtie_json_schema-0.82.1.tar` & `bowtie_json_schema-0.9.1.tar`

### file list

```diff
@@ -1,49 +1,63 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.flake8
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.readthedocs.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/test-requirements.in
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/SECURITY.md
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/release.yml
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/workflows/images.yml
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/__main__.py
--rw-r--r--   0        0        0    29308 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/_cli.py
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/_commands.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/_core.py
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/cli.rst
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/implementers.rst
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/requirements.in
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/conftest.py
--rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    27441 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/README.rst
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 bowtie_json_schema-0.82.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.flake8
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/io-schema.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/noxfile.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/test-requirements.in
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/test-requirements.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.github/SECURITY.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/bowtie/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/bowtie/__main__.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/bowtie/_cli.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/bowtie/_core.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/requirements.in
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/requirements.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/dotnet-json-everything/Dockerfile
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/dotnet-json-everything/Program.cs
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/dotnet-json-everything/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/lua-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/lua-jsonschema/bowtie-jsonschema
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1737 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/python-fastjsonschema/bowtie-fastjsonschema
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1582 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/python-jsonschema/bowtie-jsonschema
+-rw-r--r--   0        0        0    30384 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/test_integration.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/cheatsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1199 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/cheatsonschema/cheatsonschema
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3887 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     1984 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/README.rst
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 bowtie_json_schema-0.9.1/PKG-INFO
```

### Comparing `bowtie_json_schema-0.82.1/test-requirements.txt` & `bowtie_json_schema-0.9.1/docs/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
+# This file is autogenerated by pip-compile with python 3.10
+# To update, run:
 #
-#    pip-compile --resolver=backtracking test-requirements.in
+#    pip-compile docs/requirements.in
 #
 aiodocker==0.21.0
     # via bowtie-json-schema
-aiohttp==3.8.4
+aiohttp==3.8.1
     # via aiodocker
-aiosignal==1.3.1
+aiosignal==1.2.0
     # via aiohttp
+alabaster==0.7.12
+    # via sphinx
 async-timeout==4.0.2
     # via aiohttp
-attrs==22.2.0
-    # via
-    #   aiohttp
-    #   bowtie-json-schema
-    #   jsonschema
-    #   pytest
+attrs==22.1.0
+    # via aiohttp
+babel==2.10.3
+    # via sphinx
+beautifulsoup4==4.11.1
+    # via furo
 file:.#egg=bowtie-json-schema
-    # via -r test-requirements.in
-certifi==2022.12.7
+    # via -r docs/requirements.in
+certifi==2022.6.15
     # via requests
-cffi==1.15.1
-    # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==2.1.1
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via bowtie-json-schema
-cryptography==40.0.1
-    # via pyjwt
-frozenlist==1.3.3
+docutils==0.19
+    # via sphinx
+frozenlist==1.3.1
     # via
     #   aiohttp
     #   aiosignal
-github3-py==3.2.0
-    # via bowtie-json-schema
-icdiff==2.0.6
-    # via pytest-icdiff
-idna==3.4
+furo==2022.6.21
+    # via -r docs/requirements.in
+idna==3.3
     # via
     #   requests
     #   yarl
-iniconfig==2.0.0
-    # via pytest
+imagesize==1.4.1
+    # via sphinx
 jinja2==3.1.2
-    # via bowtie-json-schema
-jsonschema==4.17.3
-    # via bowtie-json-schema
-markdown-it-py==2.2.0
-    # via rich
-markupsafe==2.1.2
+    # via sphinx
+markupsafe==2.1.1
     # via jinja2
-mdurl==0.1.2
-    # via markdown-it-py
-multidict==6.0.4
+multidict==6.0.2
     # via
     #   aiohttp
     #   yarl
-packaging==23.0
-    # via pytest
-pluggy==1.0.0
-    # via pytest
-pprintpp==0.4.0
-    # via pytest-icdiff
-pycparser==2.21
-    # via cffi
-pygments==2.14.0
-    # via rich
-pyjwt[crypto]==2.6.0
-    # via github3-py
-pyrsistent==0.19.3
-    # via jsonschema
-pytest==7.2.2
-    # via
-    #   -r test-requirements.in
-    #   pytest-asyncio
-    #   pytest-icdiff
-pytest-asyncio==0.21.0
-    # via -r test-requirements.in
-pytest-icdiff==0.6
-    # via -r test-requirements.in
-python-dateutil==2.8.2
-    # via github3-py
-requests==2.28.2
-    # via github3-py
-rich==13.3.3
-    # via bowtie-json-schema
-six==1.16.0
-    # via python-dateutil
-structlog==22.3.0
+packaging==21.3
+    # via sphinx
+pyenchant==3.2.2
+    # via sphinxcontrib-spelling
+pygments==2.13.0
+    # via
+    #   furo
+    #   pygments-github-lexers
+    #   sphinx
+pygments-github-lexers==0.0.5
+    # via -r docs/requirements.in
+pyparsing==3.0.9
+    # via packaging
+pytz==2022.2.1
+    # via babel
+requests==2.28.1
+    # via sphinx
+snowballstemmer==2.2.0
+    # via sphinx
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
+sphinx==5.1.1
+    # via
+    #   -r docs/requirements.in
+    #   furo
+    #   sphinx-basic-ng
+    #   sphinxcontrib-spelling
+sphinx-basic-ng==0.0.1a12
+    # via furo
+sphinxcontrib-applehelp==1.0.2
+    # via sphinx
+sphinxcontrib-devhelp==1.0.2
+    # via sphinx
+sphinxcontrib-htmlhelp==2.0.0
+    # via sphinx
+sphinxcontrib-jsmath==1.0.1
+    # via sphinx
+sphinxcontrib-qthelp==1.0.3
+    # via sphinx
+sphinxcontrib-serializinghtml==1.1.5
+    # via sphinx
+sphinxcontrib-spelling==7.6.0
+    # via -r docs/requirements.in
+structlog==22.1.0
     # via bowtie-json-schema
-typing-extensions==4.5.0
+typing-extensions==4.3.0
     # via aiodocker
-uritemplate==4.1.1
-    # via github3-py
-urllib3==1.26.15
+urllib3==1.26.12
     # via requests
-yarl==1.8.2
+yarl==1.8.1
     # via aiohttp
```

### Comparing `bowtie_json_schema-0.82.1/.github/SECURITY.md` & `bowtie_json_schema-0.9.1/.github/SECURITY.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Security Policy
 
 ## Supported Versions
 
-In general, only the latest released `bowtie` version is supported and will receive updates.
+In general, only the latest released `bowtie.py` version is supported
+and will receive updates.
 
 ## Reporting a Vulnerability
 
-To report a security vulnerability, please send an email to `Julian+Security` at `GrayVines.com` with subject line `SECURITY (bowtie)`.
+To report a security vulnerability, please send an email to
+`Julian+Security` at `GrayVines.com` with subject line `SECURITY (bowtie.py)`.
 
-I will do my best to respond within 48 hours to acknowledge the message and discuss further steps.
+I will do my best to respond within 48 hours to acknowledge the message
+and discuss further steps.
 
-If the vulnerability is accepted, an advisory will be sent out via GitHub's security advisory functionality.
+If the vulnerability is accepted, an advisory will be sent out via
+GitHub's security advisory functionality.
 
-For non-sensitive discussion related to this policy itself, feel free to open an issue on the issue tracker.
+For non-sensitive discussion related to this policy itself, feel free to
+open an issue on the issue tracker.
```

### Comparing `bowtie_json_schema-0.82.1/.github/workflows/ci.yml` & `bowtie_json_schema-0.9.1/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -3,102 +3,81 @@
 on:
   push:
   pull_request:
   release:
     types: [published]
   schedule:
     # Daily at 5:12
-    - cron: "12 5 * * *"
-
-env:
-  PIP_DISABLE_PIP_VERSION_CHECK: "1"
-  PIP_NO_PYTHON_VERSION_WARNING: "1"
+    - cron: '12 5 * * *'
 
 jobs:
   pre-commit:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - uses: pre-commit/action@v3.0.0
-
-  list:
-    runs-on: ubuntu-latest
-    outputs:
-      noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
-    steps:
-      - uses: actions/checkout@v3
-      - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
-      - id: noxenvs-matrix
-        run: |
-          echo >>$GITHUB_OUTPUT noxenvs=$(
-            nox --list-sessions |
-            grep '^* ' |
-            cut -d ' ' -f 2- |
-            jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
-          )
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: "3.10"
+    - uses: pre-commit/action@v3.0.0
 
   ci:
-    needs: list
     runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        noxenv: ${{ fromJson(needs.list.outputs.noxenvs) }}
 
     steps:
-      - uses: actions/checkout@v3
-      - name: Install dependencies
-        run: sudo apt-get update && sudo apt-get install -y libenchant-2-dev
-        if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
-      - name: Install dependencies
-        run: brew install enchant podman
-        if: runner.os == 'macOS'
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
-      - name: Run nox
-        run: nox -s "${{ matrix.noxenv }}"
+    - uses: actions/checkout@v3
+    - name: Install dependencies
+      run: >
+        sudo apt-get update &&
+        sudo apt-get install -y libenchant-dev
+      if: runner.os == 'Linux'
+    - name: Install dependencies
+      run: brew install enchant podman
+      if: runner.os == 'macOS'
+    - name: Build Fixtures
+      run: |
+        for each in {implementations/,tests/fauxmplementations/}*; do
+          (
+            cd $each
+            podman build -f Dockerfile -t "localhost/bowtie/$(basename $each)"
+          )
+        done
+    - name: Set up nox
+      uses: wntrblm/nox@2022.8.7
+    - name: Run nox
+      run: nox
+      env:
+        REGISTRY_HTTP_ADDR: localhost
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - name: Install dependencies
-        run: python -m pip install build
-      - name: Create packages
-        run: python -m build .
-      - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
-      - name: Create shiv
-        run: mkdir shiv/ && nox -s shiv -- shiv/bowtie && chmod +x shiv/bowtie
-      - name: Tar files
-        run: tar -cvf bowtie.tar dist shiv
-      - uses: actions/upload-artifact@v3
-        with:
-          name: packages
-          path: bowtie.tar
-      - name: Publish to PyPI
-        if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
-      - name: Create a Release
-        if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-        uses: softprops/action-gh-release@v1
-        with:
-          files: |
-            shiv/bowtie
-            dist/*
-          generate_release_notes: true
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: "3.10"
+    - name: Install dependencies
+      run: python -m pip install build
+    - name: Create packages
+      run: python -m build .
+    - uses: actions/upload-artifact@v3
+      with:
+        name: dist
+        path: dist
+    - name: Publish package
+      if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
+      uses: pypa/gh-action-pypi-publish@release/v1
+      with:
+        user: __token__
+        password: ${{ secrets.pypi_password }}
+    - name: Create Release Notes
+      if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
+      uses: actions/github-script@v6
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+        script: |
+          await github.request(`POST /repos/${{ github.repository }}/releases`, {
+            tag_name: "${{ github.ref }}",
+            generate_release_notes: true
+          });
```

### Comparing `bowtie_json_schema-0.82.1/docs/Makefile` & `bowtie_json_schema-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-0.82.1/docs/index.rst` & `bowtie_json_schema-0.9.1/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -2,78 +2,51 @@
 
 ======
 Bowtie
 ======
 
 Bowtie is a *meta*-validator of the `JSON Schema specification <https://json-schema.org/>`_, by which we mean it coordinates executing *other* `validator implementations <https://json-schema.org/implementations.html>`_, collecting and reporting on their results.
 
-To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
+To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/python-jsonschema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
 
-It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``.
-Looks like a bowtie, no?
+It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``. Looks like a bowtie, no?
 Also because it's elegant – we hope.
 
 
-Contents
---------
-
-.. toctree::
-    :maxdepth: 1
-
-    cli
-    implementers
-    contributing
-
-
-Installation
-------------
-
-Via Homebrew (macOS or Linuxbrew)
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Bowtie is available in a `tap <https://docs.brew.sh/Taps>`_ which is located :github:`here <bowtie-json-schema/homebrew-tap>`, and can be installed via:
-
-.. code:: sh
-
-    brew install bowtie-json-schema/tap/bowtie
-
-Manual Installation via PyPI
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Bowtie is written in Python, and uses a container runtime to execute JSON Schema implementations, so you'll need both Python and a suitable container runtime installed.
+Execution
+---------
 
-If you have no previous container runtime installed (e.g. Docker), follow the `installation instructions for podman <https://podman.io/getting-started/installation>`_ specific to your operating system.
-Ensure you've started a Podman VM if you are on macOS.
+In general, executing ``bowtie`` consists of providing 2 pieces of input:
 
-Then follow the `pipx installation process <https://pypa.github.io/pipx/installation/>`_ to install ``pipx``, and finally use it to install Bowtie via:
+    * The names of one or more supported implementations to execute
+    * One or more test cases to run against these implementations (schemas, instances and optionally, expected validation results)
 
-.. code:: sh
+Given these, ``bowtie`` will report on the result of executing each implementation against the input schema/instance pairs.
+If expected results are provided, it will compare the results produced against the expected ones, reporting on any implementations which differ from the expected output.
 
-    pipx install bowtie-json-schema
+CLI
+===
 
-which should give you a working Bowtie installation, which you can check via:
+A sample invocation of the CLI is:
 
 .. code:: sh
 
-    bowtie --help
-
-Further usage details of the command-line interface can be found `here <cli>`.
+    $ bowtie run -i some/jsonschema-implementation/docker-image <<EOF
+    {"description": "stuff", "schema": {}, "tests": [{"description": "a test", "instance": {"foo": "bar"}}] }
+    EOF
+    {"valid": true}
 
+(TODO)
 
-Execution
----------
-
-In general, executing Bowtie consists of providing 2 pieces of input:
+Uses
+----
 
-    * The names of one or more supported implementations to execute
-    * One or more test cases to run against these implementations (schemas, instances and optionally, expected validation results)
+A key use of ``bowtie`` is in executing as input the `official test suite <https://github.com/json-schema-org/JSON-Schema-Test-Suite>`_ and comparing the results produced by implementations to the expected ones from the suite.
 
-Given these, Bowtie will report on the result of executing each implementation against the input schema/instance pairs.
-If expected results are provided, it will compare the results produced against the expected ones, reporting on any implementations which differ from the expected output.
+Of course one isn't limited to just the test cases in the test suite, as ``bowtie`` can be used to compare the validation results of any input across its supported implementations.
 
-Uses
-----
+Adding an Implementation
+------------------------
 
-A key use of Bowtie is in executing as input the `official test suite`_ and comparing the results produced by implementations to the expected ones from the suite.
+Add a ``Dockerfile`` which runs as its entry point a bowtie-compatible process to the ``implementations/`` directory in the root of this repository.
 
-Bowtie however isn't limited to just the test cases in the test suite.
-It can be used to compare the validation results of any JSON Schema input across its supported implementations.
+Name your directory ``<(ascii-compatible-name-of-)language-your-implementation-is-written-in>-<language-specific-package-identifier>``, so if your implementation is written in B++ and called ``flooblekins``, name the directory ``bpp-flooblekins``.
```

### Comparing `bowtie_json_schema-0.82.1/docs/_static/dreamed.png` & `bowtie_json_schema-0.9.1/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-0.82.1/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-0.9.1/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import io
 import json
 import sys
 
 
 @dataclass
 class Runner:
+
     _started: bool = False
     _stdout: io.TextIOWrapper = sys.stdout
     _stderr: io.TextIOWrapper = sys.stderr
 
     def run(self, stdin=sys.stdin):
         for line in stdin:
             each = json.loads(line)
@@ -28,30 +29,17 @@
         self._started = True
         return dict(
             ready=True,
             version=1,
             implementation=dict(
                 language="python",
                 name="badsonschema",
-                issues="https://github.com/bowtie-json-schema/bowtie/issues",
-                dialects=[
-                    "https://json-schema.org/draft/2020-12/schema",
-                    "https://json-schema.org/draft/2019-09/schema",
-                    "http://json-schema.org/draft-07/schema#",
-                    "http://json-schema.org/draft-06/schema#",
-                    "http://json-schema.org/draft-04/schema#",
-                    "http://json-schema.org/draft-03/schema#",
-                ],
             ),
         )
 
-    def cmd_dialect(self, dialect):
-        assert self._started, "Not started!"
-        return dict(ok=True)
-
     def cmd_run(self, case, seq):
         assert self._started, "Not started!"
 
         results = [
             {"valid": not test.get("valid", True)} for test in case["tests"]
         ]
         return dict(seq=seq, results=results)
```

### Comparing `bowtie_json_schema-0.82.1/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-0.9.1/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 """
 A bowtie runner which always gets the right answer, slowly.
 """
 from dataclasses import dataclass
 import io
 import json
+import os
 import shlex
 import sys
 import time
 
 
 class Crash(Exception):
     """
@@ -17,14 +18,15 @@
 
 
 _VALID = {"1": {"valid": True}, "0": {"valid": False}}
 
 
 @dataclass
 class Runner:
+
     _started: bool = False
     _stdout: io.TextIOWrapper = sys.stdout
     _hang_on_stop = False
 
     def run(self, stdin=sys.stdin):
         for line in stdin:
             each = json.loads(line)
@@ -32,38 +34,28 @@
             getattr(self, f"cmd_{cmd}")(**each)
 
     def send(self, **response):
         self._stdout.write(f"{json.dumps(response)}\n")
         self._stdout.flush()
 
     def cmd_start(self, version):
+        if os.environ.get("ENVSONSCHEMA_CRASH") == "1":
+            raise Crash()
+
         assert version == 1
         self._started = True
         self.send(
             ready=True,
             version=1,
             implementation=dict(
                 language="python",
                 name="envsonschema",
-                issues="https://github.com/bowtie-json-schema/bowtie/issues",
-                dialects=[
-                    "https://json-schema.org/draft/2020-12/schema",
-                    "https://json-schema.org/draft/2019-09/schema",
-                    "http://json-schema.org/draft-07/schema#",
-                    "http://json-schema.org/draft-06/schema#",
-                    "http://json-schema.org/draft-04/schema#",
-                    "http://json-schema.org/draft-03/schema#",
-                ],
             ),
         )
 
-    def cmd_dialect(self, dialect):
-        assert self._started, "Not started!"
-        return dict(ok=True)
-
     def cmd_run(self, case, seq):
         assert self._started, "Not started!"
 
         send = self.send
         for instruction, arg in instructions(case["description"]):
             if instruction == "crash":
                 raise Crash()
@@ -82,15 +74,14 @@
                 result = dict(
                     (each.split("=", 1) for each in arg.split(",")),
                     skipped=True,
                     seq=seq,
                 )
                 return self.send(**result)
             elif instruction == "split":
-
                 def send(**response):
                     dumped = json.dumps(response)
                     size = len(dumped) // 2
                     self._stdout.write(dumped[:size])
                     self._stdout.flush()
                     time.sleep(0.1)
                     self._stdout.write(dumped[size:])
@@ -108,25 +99,21 @@
                     raise Crash()
                 elif instruction == "sleep":
                     time.sleep(float(arg))
 
                 if instruction == "valid":
                     result = _VALID.get(arg, {"valid": arg})
                 elif instruction == "skip":
-                    result = dict(
-                        each.split("=", 1) for each in arg.split(",")
-                    )
+                    result = dict(each.split("=", 1) for each in arg.split(","))
                     result.update(skipped=True)
                 elif instruction == "error":
                     result = dict(
+                        (each.split("=", 1) for each in arg.split(",")),
                         errored=True,
                         seq=seq,
-                        context=dict(
-                            each.split("=", 1) for each in arg.split(",")
-                        ),
                     )
                     return self.send(**result)
 
             results["results"].append(result)
 
         send(seq=seq, **results)
```

### Comparing `bowtie_json_schema-0.82.1/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-0.9.1/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import sys
 
 import jsonschema.validators
 
 SCHEMA_PATH = Path(os.environ.get("BOWTIE_SCHEMA", "/io-schema.json"))
 SCHEMA = json.loads(SCHEMA_PATH.read_text())
 RESOLVER = jsonschema.validators.RefResolver.from_schema(SCHEMA)
-RESOLVER.store["urn:current-dialect"] = {"$ref": SCHEMA["$schema"]}
 Validator = jsonschema.validators.validator_for(SCHEMA)
 REQUEST_VALIDATOR = Validator(
     schema={"$ref": f"{SCHEMA['$id']}#/$defs/command"},
     resolver=RESOLVER,
 )
 RESPONSE_VALIDATORS = {
     k: Validator(
@@ -29,58 +28,42 @@
     )
     for k in SCHEMA["$defs"]["command"]["$defs"]
 }
 
 
 @dataclass
 class Runner:
+
     _started: bool = False
     _stdout: io.TextIOWrapper = sys.stdout
     _stderr: io.TextIOWrapper = sys.stderr
 
     def run(self, stdin=sys.stdin):
         for line in stdin:
             each = json.loads(line)
-            for error in REQUEST_VALIDATOR.iter_errors(each):
-                self._stderr.write(error.message)
-                self._stderr.write("\n")
+            REQUEST_VALIDATOR.validate(each)
             cmd = each.pop("cmd")
             response = getattr(self, f"cmd_{cmd}")(**each)
-            for error in RESPONSE_VALIDATORS[cmd].iter_errors(response):
-                self._stderr.write(error.message)
-                self._stderr.write("\n")
+            RESPONSE_VALIDATORS[cmd].validate(response)
             self._stdout.write(f"{json.dumps(response)}\n")
             self._stdout.flush()
 
     def cmd_start(self, version):
         assert version == 1
 
         self._started = True
         return dict(
             ready=True,
             version=1,
             implementation=dict(
                 language="python",
                 name="lintsonschema",
-                issues="https://github.com/bowtie-json-schema/bowtie/issues",
-                dialects=[
-                    "https://json-schema.org/draft/2020-12/schema",
-                    "https://json-schema.org/draft/2019-09/schema",
-                    "http://json-schema.org/draft-07/schema#",
-                    "http://json-schema.org/draft-06/schema#",
-                    "http://json-schema.org/draft-04/schema#",
-                    "http://json-schema.org/draft-03/schema#",
-                ],
             ),
         )
 
-    def cmd_dialect(self, dialect):
-        assert self._started, "Not started!"
-        return dict(ok=True)
-
     def cmd_run(self, case, seq):
         assert self._started, "Not started!"
 
         results = [
             {"valid": test.get("valid", True)} for test in case["tests"]
         ]
         return dict(seq=seq, results=results)
```

### Comparing `bowtie_json_schema-0.82.1/.gitignore` & `bowtie_json_schema-0.9.1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 /TODO*
-bowtie-report.html
-/badges/
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `bowtie_json_schema-0.82.1/LICENSE` & `bowtie_json_schema-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-0.82.1/README.rst` & `bowtie_json_schema-0.9.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -6,38 +6,29 @@
   :alt: Bowtie
   :target: https://pypi.org/project/bowtie-json-schema/
   :align: center
   :width: 250px
 
 |
 
-.. image:: https://zenodo.org/badge/531839193.svg
-  :alt: DOI
-  :target: https://zenodo.org/badge/latestdoi/531839193
-
 .. image:: https://img.shields.io/pypi/v/bowtie-json-schema.svg
   :alt: PyPI version
   :target: https://pypi.org/project/bowtie-json-schema/
 
 .. image:: https://img.shields.io/pypi/pyversions/bowtie-json-schema.svg
   :alt: Supported Python versions
   :target: https://pypi.org/project/bowtie-json-schema/
 
-.. image:: https://github.com/bowtie-json-schema/bowtie/workflows/CI/badge.svg
+.. image:: https://github.com/python-jsonschema/bowtie/workflows/CI/badge.svg
   :alt: Build status
-  :target: https://github.com/bowtie-json-schema/bowtie/actions?query=workflow%3ACI
-
-.. image:: https://results.pre-commit.ci/badge/github/bowtie-json-schema/bowtie/main.svg
-  :alt: pre-commit.ci status
-  :target: https://results.pre-commit.ci/latest/github/bowtie-json-schema/bowtie/main
+  :target: https://github.com/python-jsonschema/bowtie/actions?query=workflow%3ACI
 
 |
 
 Bowtie is a *meta*-validator of the `JSON Schema specification <https://json-schema.org/>`_, by which we mean it coordinates executing *other* `validator implementations <https://json-schema.org/implementations.html>`_, collecting and reporting on their results.
 
-To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
+To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/python-jsonschema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
 
-It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``.
-Looks like a bowtie, no?
+It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``. Looks like a bowtie, no?
 Also because it's elegant – we hope.
 
 For more information, see `Bowtie's documentation <https://bowtie-json-schema.readthedocs.io/>`_.
```

### Comparing `bowtie_json_schema-0.82.1/PKG-INFO` & `bowtie_json_schema-0.9.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,62 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 0.82.1
+Version: 0.9.1
 Summary: A meta-validator for the JSON Schema specification.
-Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
-Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
-Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
+Project-URL: Homepage, https://github.com/python-jsonschema/bowtie
+Project-URL: Issues, https://github.com/python-jsonschema/bowtie/issues/
+Project-URL: Source, https://github.com/python-jsonschema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
 License: MIT
-License-File: LICENSE
 Keywords: data validation,json,json schema,jsonschema,validation
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Requires-Dist: aiodocker
-Requires-Dist: attrs>=22.2.0
+Requires-Dist: attrs
 Requires-Dist: click
-Requires-Dist: github3-py
-Requires-Dist: importlib-resources; python_version < '3.9'
-Requires-Dist: jinja2
-Requires-Dist: jsonschema
-Requires-Dist: rich
 Requires-Dist: structlog
-Requires-Dist: typing-extensions; python_version < '3.11'
 Description-Content-Type: text/x-rst
 
 ======
 Bowtie
 ======
 
 .. image:: ./docs/_static/dreamed.png
   :alt: Bowtie
   :target: https://pypi.org/project/bowtie-json-schema/
   :align: center
   :width: 250px
 
 |
 
-.. image:: https://zenodo.org/badge/531839193.svg
-  :alt: DOI
-  :target: https://zenodo.org/badge/latestdoi/531839193
-
 .. image:: https://img.shields.io/pypi/v/bowtie-json-schema.svg
   :alt: PyPI version
   :target: https://pypi.org/project/bowtie-json-schema/
 
 .. image:: https://img.shields.io/pypi/pyversions/bowtie-json-schema.svg
   :alt: Supported Python versions
   :target: https://pypi.org/project/bowtie-json-schema/
 
-.. image:: https://github.com/bowtie-json-schema/bowtie/workflows/CI/badge.svg
+.. image:: https://github.com/python-jsonschema/bowtie/workflows/CI/badge.svg
   :alt: Build status
-  :target: https://github.com/bowtie-json-schema/bowtie/actions?query=workflow%3ACI
-
-.. image:: https://results.pre-commit.ci/badge/github/bowtie-json-schema/bowtie/main.svg
-  :alt: pre-commit.ci status
-  :target: https://results.pre-commit.ci/latest/github/bowtie-json-schema/bowtie/main
+  :target: https://github.com/python-jsonschema/bowtie/actions?query=workflow%3ACI
 
 |
 
 Bowtie is a *meta*-validator of the `JSON Schema specification <https://json-schema.org/>`_, by which we mean it coordinates executing *other* `validator implementations <https://json-schema.org/implementations.html>`_, collecting and reporting on their results.
 
-To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
+To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/python-jsonschema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
 
-It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``.
-Looks like a bowtie, no?
+It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``. Looks like a bowtie, no?
 Also because it's elegant – we hope.
 
 For more information, see `Bowtie's documentation <https://bowtie-json-schema.readthedocs.io/>`_.
```

