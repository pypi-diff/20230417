# Comparing `tmp/py_yettagam-0.0.2.8.tar.gz` & `tmp/py_yettagam-0.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_yettagam-0.0.2.8.tar", last modified: Sun Apr  2 03:16:27 2023, max compression
+gzip compressed data, was "py_yettagam-0.0.2.9.tar", last modified: Sun Apr  2 05:01:36 2023, max compression
```

## Comparing `py_yettagam-0.0.2.8.tar` & `py_yettagam-0.0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 03:16:27.396329 py_yettagam-0.0.2.8/
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)    11357 2023-01-28 04:59:12.000000 py_yettagam-0.0.2.8/LICENSE
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     6583 2023-04-02 03:16:27.396186 py_yettagam-0.0.2.8/PKG-INFO
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     6067 2023-04-02 03:11:52.000000 py_yettagam-0.0.2.8/README.md
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)      597 2023-04-02 03:11:47.000000 py_yettagam-0.0.2.8/pyproject.toml
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       88 2023-03-31 08:10:47.000000 py_yettagam-0.0.2.8/requirements.txt
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       38 2023-04-02 03:16:27.396365 py_yettagam-0.0.2.8/setup.cfg
-drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 03:16:27.391857 py_yettagam-0.0.2.8/src/
-drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 03:16:27.392870 py_yettagam-0.0.2.8/src/py_yettagam/
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       69 2023-03-30 05:34:21.000000 py_yettagam-0.0.2.8/src/py_yettagam/__init__.py
-drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 03:16:27.395565 py_yettagam-0.0.2.8/src/py_yettagam/substrate/
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       81 2023-03-30 05:32:52.000000 py_yettagam-0.0.2.8/src/py_yettagam/substrate/__init__.py
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)    14323 2023-04-02 03:09:12.000000 py_yettagam-0.0.2.8/src/py_yettagam/substrate/comitter.py
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     1030 2023-03-30 16:17:58.000000 py_yettagam-0.0.2.8/src/py_yettagam/substrate/decorators.py
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)      110 2023-03-30 05:15:53.000000 py_yettagam-0.0.2.8/src/py_yettagam/substrate/exceptions.py
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)    49817 2023-04-02 02:49:13.000000 py_yettagam-0.0.2.8/src/py_yettagam/substrate/listener.py
-drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 03:16:27.393865 py_yettagam-0.0.2.8/src/py_yettagam.egg-info/
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     6583 2023-04-02 03:16:27.000000 py_yettagam-0.0.2.8/src/py_yettagam.egg-info/PKG-INFO
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)      465 2023-04-02 03:16:27.000000 py_yettagam-0.0.2.8/src/py_yettagam.egg-info/SOURCES.txt
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)        1 2023-04-02 03:16:27.000000 py_yettagam-0.0.2.8/src/py_yettagam.egg-info/dependency_links.txt
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       89 2023-04-02 03:16:27.000000 py_yettagam-0.0.2.8/src/py_yettagam.egg-info/requires.txt
--rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       12 2023-04-02 03:16:27.000000 py_yettagam-0.0.2.8/src/py_yettagam.egg-info/top_level.txt
+drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 05:01:36.636078 py_yettagam-0.0.2.9/
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)    11357 2023-01-28 04:59:12.000000 py_yettagam-0.0.2.9/LICENSE
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     7355 2023-04-02 05:01:36.635931 py_yettagam-0.0.2.9/PKG-INFO
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     6839 2023-04-02 05:00:32.000000 py_yettagam-0.0.2.9/README.md
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)      597 2023-04-02 04:47:41.000000 py_yettagam-0.0.2.9/pyproject.toml
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       88 2023-03-31 08:10:47.000000 py_yettagam-0.0.2.9/requirements.txt
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       38 2023-04-02 05:01:36.636119 py_yettagam-0.0.2.9/setup.cfg
+drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 05:01:36.631999 py_yettagam-0.0.2.9/src/
+drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 05:01:36.632869 py_yettagam-0.0.2.9/src/py_yettagam/
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       69 2023-03-30 05:34:21.000000 py_yettagam-0.0.2.9/src/py_yettagam/__init__.py
+drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 05:01:36.635296 py_yettagam-0.0.2.9/src/py_yettagam/substrate/
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       81 2023-03-30 05:32:52.000000 py_yettagam-0.0.2.9/src/py_yettagam/substrate/__init__.py
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)    14323 2023-04-02 03:09:12.000000 py_yettagam-0.0.2.9/src/py_yettagam/substrate/comitter.py
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     1030 2023-03-30 16:17:58.000000 py_yettagam-0.0.2.9/src/py_yettagam/substrate/decorators.py
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)      110 2023-03-30 05:15:53.000000 py_yettagam-0.0.2.9/src/py_yettagam/substrate/exceptions.py
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)    46840 2023-04-02 04:46:17.000000 py_yettagam-0.0.2.9/src/py_yettagam/substrate/listener.py
+drwxr-xr-x   0 vigneshmeenakshisundaram   (501) staff       (20)        0 2023-04-02 05:01:36.633736 py_yettagam-0.0.2.9/src/py_yettagam.egg-info/
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)     7355 2023-04-02 05:01:36.000000 py_yettagam-0.0.2.9/src/py_yettagam.egg-info/PKG-INFO
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)      465 2023-04-02 05:01:36.000000 py_yettagam-0.0.2.9/src/py_yettagam.egg-info/SOURCES.txt
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)        1 2023-04-02 05:01:36.000000 py_yettagam-0.0.2.9/src/py_yettagam.egg-info/dependency_links.txt
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       89 2023-04-02 05:01:36.000000 py_yettagam-0.0.2.9/src/py_yettagam.egg-info/requires.txt
+-rw-r--r--   0 vigneshmeenakshisundaram   (501) staff       (20)       12 2023-04-02 05:01:36.000000 py_yettagam-0.0.2.9/src/py_yettagam.egg-info/top_level.txt
```

### Comparing `py_yettagam-0.0.2.8/LICENSE` & `py_yettagam-0.0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_yettagam-0.0.2.8/PKG-INFO` & `py_yettagam-0.0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_yettagam
-Version: 0.0.2.8
+Version: 0.0.2.9
 Summary: Python package for Metarium's Storage Layer
 Author: MetariumProject
 Project-URL: Homepage, https://github.com/MetariumProject/py-yettagam
 Project-URL: Bug Tracker, https://github.com/MetariumProject/py-yettagam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,22 +37,22 @@
 ```
 source ~/venv-yettagam/bin/activate
 ```
 
 ## 2. Dependencies
 
 ```
-pip install py-yettagam==0.0.2.8
+pip install py-yettagam==0.0.2.9
 ```
 
 ## 3. Example usage - Create a simple Yettagam Storage Sync
 
 ### 3.1. `Topic Listener`
 
-Create a script called `metarium-listener.py` with the following code block
+Create a script called `listener-cli.py` with the following code block
 
 ```
 import os
 from argparse import ArgumentParser
 
 from py_yettagam import (
     SubstrateListener,
@@ -78,43 +78,43 @@
     help="URL of the Listener Node's corresponding chain."
 )
 # add data-location-path, default to "/home/.metarium"
 parser.add_argument(
     "--data-location-path",
     type=str,
     default="/home/.metarium",
-    help="Path to the data location of the Listener Node."
+    help="Path to the data location of the Listener Node. Default is '/home/.metarium'."
 )
 # add writer-location-path, default to "/home/writer"
 parser.add_argument(
     "--writer-location-path",
     type=str,
     default="/home/writer",
-    help="Path to the location of the user with write-only access to the 'inbox' folder."
+    help="Path to the location of the user with write-only access to the 'inbox' folder. Default is '/home/writer'."
 )
 # add reader-location-path, default to "/home/reader"
 parser.add_argument(
     "--reader-location-path",
     type=str,
     default="/home/reader",
-    help="Path to the location of the user with read-only access to the 'outbox' folder."
+    help="Path to the location of the user with read-only access to the 'outbox' folder. Default is '/home/reader'."
 )
 # add block-threshold-404, default to 16
 parser.add_argument(
     "--block-threshold-404",
     type=int,
     default=16,
-    help="Number of blocks to wait before retrying a block retrieval."
+    help="Number of blocks to wait before retrying a block retrieval. Default is 16."
 )
 # add outbox-read-duration-seconds, default to 3600
 parser.add_argument(
     "--outbox-read-duration-seconds",
     type=int,
     default=3600,
-    help="Number of seconds for which the 'outbox' folder is open for a remote Node to read files from."
+    help="Number of seconds for which the 'outbox' folder is open for a remote Node to read files from. Default is 3600."
 )
 
 
 if __name__ == "__main__":
     # parse arguments
     args = parser.parse_args()
     # verify key-path exists
@@ -149,20 +149,20 @@
         outbox_read_duration_seconds=args.outbox_read_duration_seconds,
     )
 ```
 
 Run the cli script
 
 ```
-python metarium-listener.py -h
+python listener-cli.py -h
 ```
 
 ### 3.2. `Topic Committer`
 
-Create a script called `metarium-committer.py` with the following code block
+Create a script called `committer-cli.py` with the following code block
 
 ```
 import os
 from argparse import ArgumentParser
 
 from py_yettagam import (
     SubstrateCommitter,
@@ -195,20 +195,32 @@
 )
 # add file-location-path
 parser.add_argument(
     "--file-location-path",
     type=str,
     help="Path to the file to be uploaded."
 )
+# add ssh-private-key-path
+parser.add_argument(
+    "--ssh-private-key-path",
+    type=str,
+    help="Path to the SSH private key file of the Committer Node."
+)
+# add ssh-private-key-passphrase
+parser.add_argument(
+    "--ssh-private-key-passphrase",
+    type=str,
+    help="Passphrase of the SSH private key file of the Committer Node."
+)
 # add listener-threshold, default=3
 parser.add_argument(
     "--listener-threshold",
     type=int,
     default=3,
-    help="Maximum number of corresponding Listeners to which the committed file will be uploaded."
+    help="Maximum number of corresponding Listeners to which the committed file will be uploaded. Default is 3."
 )
 
 
 if __name__ == "__main__":
     # parse arguments
     args = parser.parse_args()
     # verify key-path exists
@@ -218,31 +230,37 @@
     # verify chain-url is valid
     assert args.chain_url.startswith(
         "ws://") or args.chain_url.startswith("wss://")
     # verify topic-id is valid
     assert args.topic_id > 0
     # verify file-location-path exists
     assert os.path.exists(args.file_location_path)
+    # verify ssh-private-key-path exists
+    assert os.path.exists(args.ssh_private_key_path)
+    # verify ssh-private-key-passphrase is valid
+    assert args.ssh_private_key_passphrase is not None
     # verify listener-threshold is valid
     assert args.listener_threshold > 0
     # create committer
     committer = SubstrateCommitter(
         key_path=args.key_path,
         chain_spec_path=args.chain_spec_path,
         chain_url=args.chain_url,
         topic_id=args.topic_id,
         file_location_path=args.file_location_path,
+        ssh_private_key_path=args.ssh_private_key_path,
+        ssh_private_key_passphrase=args.ssh_private_key_passphrase,
         listener_threshold=args.listener_threshold,
     )
 ```
 
 Run the cli script
 
 ```
-python metarium-committer.py -h
+python committer-cli.py -h
 ```
 
 ## 4. Teardown
 
 Please remember to deactivate the virtual environment after usage
 
 ```
```

### Comparing `py_yettagam-0.0.2.8/README.md` & `py_yettagam-0.0.2.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 ```
 source ~/venv-yettagam/bin/activate
 ```
 
 ## 2. Dependencies
 
 ```
-pip install py-yettagam==0.0.2.8
+pip install py-yettagam==0.0.2.9
 ```
 
 ## 3. Example usage - Create a simple Yettagam Storage Sync
 
 ### 3.1. `Topic Listener`
 
-Create a script called `metarium-listener.py` with the following code block
+Create a script called `listener-cli.py` with the following code block
 
 ```
 import os
 from argparse import ArgumentParser
 
 from py_yettagam import (
     SubstrateListener,
@@ -64,43 +64,43 @@
     help="URL of the Listener Node's corresponding chain."
 )
 # add data-location-path, default to "/home/.metarium"
 parser.add_argument(
     "--data-location-path",
     type=str,
     default="/home/.metarium",
-    help="Path to the data location of the Listener Node."
+    help="Path to the data location of the Listener Node. Default is '/home/.metarium'."
 )
 # add writer-location-path, default to "/home/writer"
 parser.add_argument(
     "--writer-location-path",
     type=str,
     default="/home/writer",
-    help="Path to the location of the user with write-only access to the 'inbox' folder."
+    help="Path to the location of the user with write-only access to the 'inbox' folder. Default is '/home/writer'."
 )
 # add reader-location-path, default to "/home/reader"
 parser.add_argument(
     "--reader-location-path",
     type=str,
     default="/home/reader",
-    help="Path to the location of the user with read-only access to the 'outbox' folder."
+    help="Path to the location of the user with read-only access to the 'outbox' folder. Default is '/home/reader'."
 )
 # add block-threshold-404, default to 16
 parser.add_argument(
     "--block-threshold-404",
     type=int,
     default=16,
-    help="Number of blocks to wait before retrying a block retrieval."
+    help="Number of blocks to wait before retrying a block retrieval. Default is 16."
 )
 # add outbox-read-duration-seconds, default to 3600
 parser.add_argument(
     "--outbox-read-duration-seconds",
     type=int,
     default=3600,
-    help="Number of seconds for which the 'outbox' folder is open for a remote Node to read files from."
+    help="Number of seconds for which the 'outbox' folder is open for a remote Node to read files from. Default is 3600."
 )
 
 
 if __name__ == "__main__":
     # parse arguments
     args = parser.parse_args()
     # verify key-path exists
@@ -135,20 +135,20 @@
         outbox_read_duration_seconds=args.outbox_read_duration_seconds,
     )
 ```
 
 Run the cli script
 
 ```
-python metarium-listener.py -h
+python listener-cli.py -h
 ```
 
 ### 3.2. `Topic Committer`
 
-Create a script called `metarium-committer.py` with the following code block
+Create a script called `committer-cli.py` with the following code block
 
 ```
 import os
 from argparse import ArgumentParser
 
 from py_yettagam import (
     SubstrateCommitter,
@@ -181,20 +181,32 @@
 )
 # add file-location-path
 parser.add_argument(
     "--file-location-path",
     type=str,
     help="Path to the file to be uploaded."
 )
+# add ssh-private-key-path
+parser.add_argument(
+    "--ssh-private-key-path",
+    type=str,
+    help="Path to the SSH private key file of the Committer Node."
+)
+# add ssh-private-key-passphrase
+parser.add_argument(
+    "--ssh-private-key-passphrase",
+    type=str,
+    help="Passphrase of the SSH private key file of the Committer Node."
+)
 # add listener-threshold, default=3
 parser.add_argument(
     "--listener-threshold",
     type=int,
     default=3,
-    help="Maximum number of corresponding Listeners to which the committed file will be uploaded."
+    help="Maximum number of corresponding Listeners to which the committed file will be uploaded. Default is 3."
 )
 
 
 if __name__ == "__main__":
     # parse arguments
     args = parser.parse_args()
     # verify key-path exists
@@ -204,31 +216,37 @@
     # verify chain-url is valid
     assert args.chain_url.startswith(
         "ws://") or args.chain_url.startswith("wss://")
     # verify topic-id is valid
     assert args.topic_id > 0
     # verify file-location-path exists
     assert os.path.exists(args.file_location_path)
+    # verify ssh-private-key-path exists
+    assert os.path.exists(args.ssh_private_key_path)
+    # verify ssh-private-key-passphrase is valid
+    assert args.ssh_private_key_passphrase is not None
     # verify listener-threshold is valid
     assert args.listener_threshold > 0
     # create committer
     committer = SubstrateCommitter(
         key_path=args.key_path,
         chain_spec_path=args.chain_spec_path,
         chain_url=args.chain_url,
         topic_id=args.topic_id,
         file_location_path=args.file_location_path,
+        ssh_private_key_path=args.ssh_private_key_path,
+        ssh_private_key_passphrase=args.ssh_private_key_passphrase,
         listener_threshold=args.listener_threshold,
     )
 ```
 
 Run the cli script
 
 ```
-python metarium-committer.py -h
+python committer-cli.py -h
 ```
 
 ## 4. Teardown
 
 Please remember to deactivate the virtual environment after usage
 
 ```
```

### Comparing `py_yettagam-0.0.2.8/pyproject.toml` & `py_yettagam-0.0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py_yettagam"
-version = "0.0.2.8"
+version = "0.0.2.9"
 authors = [
   { name="MetariumProject" },
 ]
 description = "Python package for Metarium's Storage Layer"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `py_yettagam-0.0.2.8/src/py_yettagam/substrate/comitter.py` & `py_yettagam-0.0.2.9/src/py_yettagam/substrate/comitter.py`

 * *Files identical despite different names*

### Comparing `py_yettagam-0.0.2.8/src/py_yettagam/substrate/decorators.py` & `py_yettagam-0.0.2.9/src/py_yettagam/substrate/decorators.py`

 * *Files identical despite different names*

### Comparing `py_yettagam-0.0.2.8/src/py_yettagam.egg-info/PKG-INFO` & `py_yettagam-0.0.2.9/src/py_yettagam.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-yettagam
-Version: 0.0.2.8
+Version: 0.0.2.9
 Summary: Python package for Metarium's Storage Layer
 Author: MetariumProject
 Project-URL: Homepage, https://github.com/MetariumProject/py-yettagam
 Project-URL: Bug Tracker, https://github.com/MetariumProject/py-yettagam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,22 +37,22 @@
 ```
 source ~/venv-yettagam/bin/activate
 ```
 
 ## 2. Dependencies
 
 ```
-pip install py-yettagam==0.0.2.8
+pip install py-yettagam==0.0.2.9
 ```
 
 ## 3. Example usage - Create a simple Yettagam Storage Sync
 
 ### 3.1. `Topic Listener`
 
-Create a script called `metarium-listener.py` with the following code block
+Create a script called `listener-cli.py` with the following code block
 
 ```
 import os
 from argparse import ArgumentParser
 
 from py_yettagam import (
     SubstrateListener,
@@ -78,43 +78,43 @@
     help="URL of the Listener Node's corresponding chain."
 )
 # add data-location-path, default to "/home/.metarium"
 parser.add_argument(
     "--data-location-path",
     type=str,
     default="/home/.metarium",
-    help="Path to the data location of the Listener Node."
+    help="Path to the data location of the Listener Node. Default is '/home/.metarium'."
 )
 # add writer-location-path, default to "/home/writer"
 parser.add_argument(
     "--writer-location-path",
     type=str,
     default="/home/writer",
-    help="Path to the location of the user with write-only access to the 'inbox' folder."
+    help="Path to the location of the user with write-only access to the 'inbox' folder. Default is '/home/writer'."
 )
 # add reader-location-path, default to "/home/reader"
 parser.add_argument(
     "--reader-location-path",
     type=str,
     default="/home/reader",
-    help="Path to the location of the user with read-only access to the 'outbox' folder."
+    help="Path to the location of the user with read-only access to the 'outbox' folder. Default is '/home/reader'."
 )
 # add block-threshold-404, default to 16
 parser.add_argument(
     "--block-threshold-404",
     type=int,
     default=16,
-    help="Number of blocks to wait before retrying a block retrieval."
+    help="Number of blocks to wait before retrying a block retrieval. Default is 16."
 )
 # add outbox-read-duration-seconds, default to 3600
 parser.add_argument(
     "--outbox-read-duration-seconds",
     type=int,
     default=3600,
-    help="Number of seconds for which the 'outbox' folder is open for a remote Node to read files from."
+    help="Number of seconds for which the 'outbox' folder is open for a remote Node to read files from. Default is 3600."
 )
 
 
 if __name__ == "__main__":
     # parse arguments
     args = parser.parse_args()
     # verify key-path exists
@@ -149,20 +149,20 @@
         outbox_read_duration_seconds=args.outbox_read_duration_seconds,
     )
 ```
 
 Run the cli script
 
 ```
-python metarium-listener.py -h
+python listener-cli.py -h
 ```
 
 ### 3.2. `Topic Committer`
 
-Create a script called `metarium-committer.py` with the following code block
+Create a script called `committer-cli.py` with the following code block
 
 ```
 import os
 from argparse import ArgumentParser
 
 from py_yettagam import (
     SubstrateCommitter,
@@ -195,20 +195,32 @@
 )
 # add file-location-path
 parser.add_argument(
     "--file-location-path",
     type=str,
     help="Path to the file to be uploaded."
 )
+# add ssh-private-key-path
+parser.add_argument(
+    "--ssh-private-key-path",
+    type=str,
+    help="Path to the SSH private key file of the Committer Node."
+)
+# add ssh-private-key-passphrase
+parser.add_argument(
+    "--ssh-private-key-passphrase",
+    type=str,
+    help="Passphrase of the SSH private key file of the Committer Node."
+)
 # add listener-threshold, default=3
 parser.add_argument(
     "--listener-threshold",
     type=int,
     default=3,
-    help="Maximum number of corresponding Listeners to which the committed file will be uploaded."
+    help="Maximum number of corresponding Listeners to which the committed file will be uploaded. Default is 3."
 )
 
 
 if __name__ == "__main__":
     # parse arguments
     args = parser.parse_args()
     # verify key-path exists
@@ -218,31 +230,37 @@
     # verify chain-url is valid
     assert args.chain_url.startswith(
         "ws://") or args.chain_url.startswith("wss://")
     # verify topic-id is valid
     assert args.topic_id > 0
     # verify file-location-path exists
     assert os.path.exists(args.file_location_path)
+    # verify ssh-private-key-path exists
+    assert os.path.exists(args.ssh_private_key_path)
+    # verify ssh-private-key-passphrase is valid
+    assert args.ssh_private_key_passphrase is not None
     # verify listener-threshold is valid
     assert args.listener_threshold > 0
     # create committer
     committer = SubstrateCommitter(
         key_path=args.key_path,
         chain_spec_path=args.chain_spec_path,
         chain_url=args.chain_url,
         topic_id=args.topic_id,
         file_location_path=args.file_location_path,
+        ssh_private_key_path=args.ssh_private_key_path,
+        ssh_private_key_passphrase=args.ssh_private_key_passphrase,
         listener_threshold=args.listener_threshold,
     )
 ```
 
 Run the cli script
 
 ```
-python metarium-committer.py -h
+python committer-cli.py -h
 ```
 
 ## 4. Teardown
 
 Please remember to deactivate the virtual environment after usage
 
 ```
```

