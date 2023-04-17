# Comparing `tmp/ensembl-prodinf-core-2.0.4.tar.gz` & `tmp/ensembl-prodinf-core-2.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ensembl-prodinf-core-2.0.4.tar", last modified: Fri Apr 29 12:47:45 2022, max compression
+gzip compressed data, was "ensembl-prodinf-core-2.0.5a2.tar", last modified: Mon Apr 17 16:54:12 2023, max compression
```

## Comparing `ensembl-prodinf-core-2.0.4.tar` & `ensembl-prodinf-core-2.0.5a2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11366 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      194 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1223 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4785 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/amqp_publishing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1939 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/app_logging.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6749 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/datachecks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7809 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/dbcopy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/event.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4613 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/handover.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4150 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3214 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3089 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/db_introspects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3701 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/db_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/compara.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2517 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21611 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/hive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2944 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/perl_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2073 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/reporting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14102 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/resource_lock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5646 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/rest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5879 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/server_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3780 2022-04-29 12:47:11.000000 ensembl-prodinf-core-2.0.4/src/ensembl/production/core/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1223 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1346 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/namespace_packages.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-04-29 12:47:45.000000 ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/
+-rw-rw-rw-   0 root         (0) root         (0)    11366 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.828649 ensembl-prodinf-core-2.0.5a2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.827649 ensembl-prodinf-core-2.0.5a2/src/ensembl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.828649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.831649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/amqp_publishing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/app_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.832649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/datachecks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/dbcopy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/handover.py
+-rw-rw-rw-   0 root         (0) root         (0)     4150 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_introspects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/es.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.832649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2849 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/compara.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    21611 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/hive.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/perl_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)    14102 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/resource_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5879 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3780 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.833649 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ensembl-prodinf-core-2.0.4/LICENSE` & `ensembl-prodinf-core-2.0.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/PKG-INFO` & `ensembl-prodinf-core-2.0.5a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: ensembl-prodinf-core
-Version: 2.0.4
+Version: 2.0.5a2
 Summary: Ensembl Production infrastructure core package
 Home-page: https://github.com/Ensembl/ensembl-prodinf-core
 Author: Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala
 Author-email: mchakiachvili@ebi.ac.uk,jallen@ebi.ac.uk,ldrf@ebi.ac.uk,vkaikala@ebi.ac.uk
 Maintainer: Ensembl Production Team
 Maintainer-email: ensembl-production@ebi.ac.uk
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -29,9 +28,7 @@
 
 Contain shared libraries used across other production team manages python packages
 
 
 
 
 
-
-
```

### Comparing `ensembl-prodinf-core-2.0.4/setup.py` & `ensembl-prodinf-core-2.0.5a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #    You may obtain a copy of the License at
 #        http://www.apache.org/licenses/LICENSE-2.0
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+import os
 import pathlib
 from setuptools import setup, find_namespace_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 readme = (here / 'README.md').read_text(encoding='utf-8')
 version = (here / 'VERSION').read_text(encoding='utf-8').strip()
 
@@ -23,15 +24,15 @@
         return [line.strip() for line in file.readlines()]
 
 
 setup(
     name='ensembl-prodinf-core',
     description='Ensembl Production infrastructure core package',
     long_description=readme,
-    version=version,
+    version=os.getenv('CI_COMMIT_TAG', version),
     namespace_packages=['ensembl'],
     packages=find_namespace_packages(where='src', include=['ensembl*'], exclude=['test']),
     package_dir={'': 'src'},
     include_package_data=True,
     url='https://github.com/Ensembl/ensembl-prodinf-core',
     license='Apache 2.0',
     author='Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala',
```

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/amqp_publishing.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/amqp_publishing.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/app_logging.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/app_logging.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/datachecks.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/datachecks.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/dbcopy.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/dbcopy.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/event.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/event.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/handover.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/handover.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/clients/metadata.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/metadata.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/config.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/config.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/db_introspects.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_introspects.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 
 from functools import lru_cache
 import sqlalchemy as sa
 import re
 
 
 @lru_cache(maxsize=None)
-def get_engine(hostname, port='3306', user='ensro', password=''):
-    uri = 'mysql://{}:{}@{}:{}'.format(user,
-                                       password,
-                                       hostname,
-                                       port)
+def get_engine(hostname, port='3306', user='ensro', password='', database=''):
+    uri = f'mysql://{user}:{password}@{hostname}:{port}'
+    if database != '':
+        uri += f'/{database}'
     return sa.create_engine(uri, pool_recycle=3600)
 
 
 def get_schema_names(engine):
     return sa.inspect(engine).get_schema_names()
 
 
@@ -55,28 +54,34 @@
     names = set(names_list)
     if incl_filters:
         names = _filter_names(names_list, incl_filters)
     skip_names = _filter_names(names_list, skip_filters)
     return names.difference(skip_names)
 
 
-def get_database_set(
-        hostname, port, user='ensro', password='', incl_filters=None, skip_filters=None
-):
+def get_database_set(hostname, port, user='ensro', password='', incl_filters=None, skip_filters=None):
     try:
         db_engine = get_engine(hostname, port, user, password)
     except RuntimeError as e:
         raise ValueError('Invalid hostname: {} or port: {}'.format(hostname, port)) from e
     database_list = get_schema_names(db_engine)
     return _apply_filters(database_list, incl_filters, skip_filters)
 
 
-def get_table_set(
-        hostname, port, database, user='ensro', password='', incl_filters=None, skip_filters=None
-):
+def get_table_set(hostname, port, database, user='ensro', password='', incl_filters=None, skip_filters=None):
     try:
         db_engine = get_engine(hostname, port, user, password)
     except RuntimeError as e:
         raise ValueError('Invalid hostname: {} or port: {}'.format(hostname, port)) from e
     table_list = get_table_names(db_engine, database)
     return _apply_filters(table_list, incl_filters, skip_filters)
 
+
+def get_table_engines(hostname, port, database, user='ensro', password=''):
+    try:
+        db_engine = get_engine(hostname, port, user, password, database)
+        with db_engine.connect() as connection:
+            rp = connection.exec_driver_sql("SHOW TABLE STATUS")
+            # table_name => table_engine
+            return {r[0]: r[1] for r in rp}
+    except RuntimeError as e:
+        raise ValueError('Invalid hostname: {} or port: {}'.format(hostname, port)) from e
```

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/db_utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/exceptions.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/compara.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/compara.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/core.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/core.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/models/hive.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/hive.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/perl_utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/perl_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/reporting.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/reporting.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/resource_lock.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/resource_lock.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/rest.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/rest.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/server_utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/server_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl/production/core/utils.py` & `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/PKG-INFO` & `ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: ensembl-prodinf-core
-Version: 2.0.4
+Version: 2.0.5a2
 Summary: Ensembl Production infrastructure core package
 Home-page: https://github.com/Ensembl/ensembl-prodinf-core
 Author: Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala
 Author-email: mchakiachvili@ebi.ac.uk,jallen@ebi.ac.uk,ldrf@ebi.ac.uk,vkaikala@ebi.ac.uk
 Maintainer: Ensembl Production Team
 Maintainer-email: ensembl-production@ebi.ac.uk
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -29,9 +28,7 @@
 
 Contain shared libraries used across other production team manages python packages
 
 
 
 
 
-
-
```

### Comparing `ensembl-prodinf-core-2.0.4/src/ensembl_prodinf_core.egg-info/SOURCES.txt` & `ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements.txt
 setup.py
 src/ensembl/production/core/amqp_publishing.py
 src/ensembl/production/core/app_logging.py
 src/ensembl/production/core/config.py
 src/ensembl/production/core/db_introspects.py
 src/ensembl/production/core/db_utils.py
+src/ensembl/production/core/es.py
 src/ensembl/production/core/exceptions.py
 src/ensembl/production/core/perl_utils.py
 src/ensembl/production/core/reporting.py
 src/ensembl/production/core/resource_lock.py
 src/ensembl/production/core/rest.py
 src/ensembl/production/core/server_utils.py
 src/ensembl/production/core/utils.py
```

