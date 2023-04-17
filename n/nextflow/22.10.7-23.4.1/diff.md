# Comparing `tmp/nextflow-22.10.7.tar.gz` & `tmp/nextflow-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextflow-22.10.7.tar", last modified: Mon Feb 20 11:01:25 2023, max compression
+gzip compressed data, was "nextflow-23.4.1.tar", last modified: Mon Apr 17 09:33:59 2023, max compression
```

## Comparing `nextflow-22.10.7.tar` & `nextflow-23.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-02-20 11:01:25.328987 nextflow-22.10.7/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1581 2023-02-20 11:01:25.328987 nextflow-22.10.7/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-22.10.7/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-02-20 11:01:25.324987 nextflow-22.10.7/launcher/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14721 2023-02-20 11:01:24.000000 nextflow-22.10.7/launcher/nextflow
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-02-20 11:01:25.328987 nextflow-22.10.7/nextflow.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1581 2023-02-20 11:01:25.000000 nextflow-22.10.7/nextflow.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2023-02-20 11:01:25.000000 nextflow-22.10.7/nextflow.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-02-20 11:01:25.000000 nextflow-22.10.7/nextflow.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-02-20 11:01:25.000000 nextflow-22.10.7/nextflow.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-02-20 11:01:25.328987 nextflow-22.10.7/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      786 2023-02-20 10:59:44.000000 nextflow-22.10.7/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-17 09:33:59.603348 nextflow-23.4.1/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2023-04-17 09:33:59.603348 nextflow-23.4.1/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-23.4.1/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-17 09:33:59.603348 nextflow-23.4.1/launcher/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14760 2023-04-17 09:33:59.000000 nextflow-23.4.1/launcher/nextflow
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-17 09:33:59.603348 nextflow-23.4.1/nextflow.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-17 09:33:59.603348 nextflow-23.4.1/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      786 2023-04-17 09:30:32.000000 nextflow-23.4.1/setup.py
```

### Comparing `nextflow-22.10.7/PKG-INFO` & `nextflow-23.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 22.10.7
+Version: 23.4.1
 Summary: A Python wrapper that installs the Nextflow launcher
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
-Description: # Nextflow launcher python package
-        
-        ## Description
-        This package is purely an installer for the Nextflow launcher (<https://nextflow.io/>) that allows
-        you to easily have the `nextflow` command line available on your system.
-        
-        ## How to install
-         - Install Nextflow launcher using `pip install nextflow`. 
-         - Now `nextflow` command is available on your path.
-         - Run `nextflow info` to force it download all the dependencies the first time (optional).
-         - Now you are ready to run a pipeline `nextflow run hello`. 
-        
-        ## Requirements
-        The Nextflow launcher requires Java and `curl` or `wget` available on your
-        system to be able to download Nextflow Java dependencies and launch Nextflow.
-        
-        ## Note
-        If you are looking for previous versions of this package that was a wrapper around the Nextflow
-        pipeline framework that lets you run pipelines from Python code, check `nextflowpy` package.
-        
 Keywords: pipeline,workflow,nextflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+
+# Nextflow launcher python package
+
+## Description
+This package is purely an installer for the Nextflow launcher (<https://nextflow.io/>) that allows
+you to easily have the `nextflow` command line available on your system.
+
+## How to install
+ - Install Nextflow launcher using `pip install nextflow`. 
+ - Now `nextflow` command is available on your path.
+ - Run `nextflow info` to force it download all the dependencies the first time (optional).
+ - Now you are ready to run a pipeline `nextflow run hello`. 
+
+## Requirements
+The Nextflow launcher requires Java and `curl` or `wget` available on your
+system to be able to download Nextflow Java dependencies and launch Nextflow.
+
+## Note
+If you are looking for previous versions of this package that was a wrapper around the Nextflow
+pipeline framework that lets you run pipelines from Python code, check `nextflowpy` package.
+
+
```

### Comparing `nextflow-22.10.7/README.md` & `nextflow-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nextflow-22.10.7/launcher/nextflow` & `nextflow-23.4.1/launcher/nextflow`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env bash
 #
-#  Copyright 2020-2022, Seqera Labs
-#  Copyright 2013-2019, Centre for Genomic Regulation (CRG)
+#  Copyright 2013-2023, Seqera Labs
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [[ "$NXF_DEBUG" == 'x' ]] && set -x
-NXF_VER=${NXF_VER:-'22.10.7'}
+NXF_VER=${NXF_VER:-'23.04.1'}
 NXF_ORG=${NXF_ORG:-'nextflow-io'}
 NXF_HOME=${NXF_HOME:-$HOME/.nextflow}
 NXF_PROT=${NXF_PROT:-'https'}
 NXF_BASE=${NXF_BASE:-$NXF_PROT://www.nextflow.io/releases}
 NXF_TEMP=${NXF_TEMP:-$TMPDIR}
 NXF_DIST=${NXF_DIST:-$NXF_HOME/framework}
 NXF_CLI="$0 $@"
@@ -60,15 +59,15 @@
   echo "$(cd "$(dirname "$1")" && pwd)/$(basename "$1")"
 }
 
 function get() {
     if command -v curl &>/dev/null; then
         GET="curl -fsSL '$1' -o '$2'"
     elif command -v wget &>/dev/null; then
-        GET="wget -q '$1' -O '$2'"
+        GET="wget '$1' -O '$2' >/dev/null 2>&1"
     else
         echo_red "ERROR: Cannot find 'curl' nor 'wget' utility --  please install one of them"
         exit 1
     fi
 
     printf "Downloading nextflow dependencies. It may require a few seconds, please wait .. "
     eval $GET; status=$?
@@ -299,28 +298,28 @@
   major=${BASH_REMATCH[1]}
   minor=${BASH_REMATCH[2]}
   # legacy version - Java 7/8 only
   if [ $major -eq 0 ] && [ $minor -lt 26 ]; then
     version_check="^(1.7|1.8)"
     version_message="Java 7 or 8"
   else
-    version_check="^(1.8|9|10|11|12|13|14|15|16|17|18)"
-    version_message="Java 8 or later (up to 18)"
+    version_check="^(1.8|9|10|11|12|13|14|15|16|17|18|19|20)"
+    version_message="Java 8 or later (up to 20)"
   fi
   if [[ ! $JAVA_VER =~ $version_check ]]; then
       echo_red "ERROR: Cannot find Java or it's a wrong version -- please make sure that $version_message is installed"
       if [[ "$NXF_JAVA_HOME" ]]; then
       echo_yellow "NOTE: Nextflow is trying to use the Java VM defined by the following environment variables:\n JAVA_CMD: $JAVA_CMD\n NXF_JAVA_HOME: $NXF_JAVA_HOME\n"
       else
       echo_yellow "NOTE: Nextflow is trying to use the Java VM defined by the following environment variables:\n JAVA_CMD: $JAVA_CMD\n JAVA_HOME: $JAVA_HOME\n"
       fi
       exit 1
   fi
-  if [[ ! $JAVA_VER =~ ^(11|12|13|14|15|16|17|18) ]]; then
-      echo_yellow "NOTE: Nextflow is not tested with Java $JAVA_VER -- It's recommended the use of version 11 up to 18\n"
+  if [[ ! $JAVA_VER =~ ^(11|12|13|14|15|16|17|18|19|20) ]]; then
+      echo_yellow "NOTE: Nextflow is not tested with Java $JAVA_VER -- It's recommended the use of version 11 up to 20\n"
   fi
   mkdir -p $(dirname "$JAVA_KEY")
   [[ -f $JAVA_VER ]] && echo $JAVA_VER > "$JAVA_KEY"
 fi
 
 # Verify nextflow jar is available
 if [ ! -f "$NXF_BIN" ]; then
@@ -401,15 +400,15 @@
     # remainder string are arguments
     # we extract first part into `cmd_base`` and remainder into `cmd_tail`` and convert them to array as previous version
     cmd_pattern='"([^"]*)"(.*)'
     [[ "${cli[@]}" =~ $cmd_pattern ]]
     cmd_base=(${BASH_REMATCH[1]})
     cmd_tail=(${BASH_REMATCH[2]})
 
-    if [[ "$JAVA_VER" =~ ^(9|10|11|12|13|14|15|16|17|18) ]]; then
+    if [[ "$JAVA_VER" =~ ^(9|10|11|12|13|14|15|16|17|18|19|20) ]]; then
       launcher="${cmd_base[@]}"
       launcher+=(--add-opens=java.base/java.lang=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.io=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.nio=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.net=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.util=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.util.concurrent.locks=ALL-UNNAMED)
@@ -418,14 +417,15 @@
       launcher+=(--add-opens=java.base/sun.nio.ch=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/sun.nio.fs=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/sun.net.www.protocol.http=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/sun.net.www.protocol.https=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/sun.net.www.protocol.ftp=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/sun.net.www.protocol.file=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/jdk.internal.misc=ALL-UNNAMED)
+      launcher+=(--add-opens=java.base/java.util.regex=ALL-UNNAMED)
       [[ "$NXF_JVM_ARGS" ]] && launcher+=($NXF_JVM_ARGS)
       launcher+=("${cmd_tail[@]}")
     else
       launcher="${cmd_base[@]}"
       [[ "$NXF_JVM_ARGS" ]] && launcher+=($NXF_JVM_ARGS)
       launcher+=("${cmd_tail[@]}")
     fi
```

### Comparing `nextflow-22.10.7/nextflow.egg-info/PKG-INFO` & `nextflow-23.4.1/nextflow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 22.10.7
+Version: 23.4.1
 Summary: A Python wrapper that installs the Nextflow launcher
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
-Description: # Nextflow launcher python package
-        
-        ## Description
-        This package is purely an installer for the Nextflow launcher (<https://nextflow.io/>) that allows
-        you to easily have the `nextflow` command line available on your system.
-        
-        ## How to install
-         - Install Nextflow launcher using `pip install nextflow`. 
-         - Now `nextflow` command is available on your path.
-         - Run `nextflow info` to force it download all the dependencies the first time (optional).
-         - Now you are ready to run a pipeline `nextflow run hello`. 
-        
-        ## Requirements
-        The Nextflow launcher requires Java and `curl` or `wget` available on your
-        system to be able to download Nextflow Java dependencies and launch Nextflow.
-        
-        ## Note
-        If you are looking for previous versions of this package that was a wrapper around the Nextflow
-        pipeline framework that lets you run pipelines from Python code, check `nextflowpy` package.
-        
 Keywords: pipeline,workflow,nextflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+
+# Nextflow launcher python package
+
+## Description
+This package is purely an installer for the Nextflow launcher (<https://nextflow.io/>) that allows
+you to easily have the `nextflow` command line available on your system.
+
+## How to install
+ - Install Nextflow launcher using `pip install nextflow`. 
+ - Now `nextflow` command is available on your path.
+ - Run `nextflow info` to force it download all the dependencies the first time (optional).
+ - Now you are ready to run a pipeline `nextflow run hello`. 
+
+## Requirements
+The Nextflow launcher requires Java and `curl` or `wget` available on your
+system to be able to download Nextflow Java dependencies and launch Nextflow.
+
+## Note
+If you are looking for previous versions of this package that was a wrapper around the Nextflow
+pipeline framework that lets you run pipelines from Python code, check `nextflowpy` package.
+
+
```

### Comparing `nextflow-22.10.7/setup.py` & `nextflow-23.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = '22.10.7'
+__version__ = '23.04.1'
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
```

