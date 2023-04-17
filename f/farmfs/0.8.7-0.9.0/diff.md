# Comparing `tmp/farmfs-0.8.7.tar.gz` & `tmp/farmfs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farmfs-0.8.7.tar", last modified: Sat Feb 11 18:40:01 2023, max compression
+gzip compressed data, was "farmfs-0.9.0.tar", last modified: Mon Apr 17 20:19:38 2023, max compression
```

## Comparing `farmfs-0.8.7.tar` & `farmfs-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-02-11 18:40:01.583535 farmfs-0.8.7/
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1082 2020-04-07 22:47:13.000000 farmfs-0.8.7/LICENSE
--rw-r--r--   0 andrewthomson   (501) staff       (20)     8138 2023-02-11 18:40:01.582952 farmfs-0.8.7/PKG-INFO
--rw-r--r--   0 andrewthomson   (501) staff       (20)     5679 2022-08-06 09:05:06.000000 farmfs-0.8.7/README.md
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-02-11 18:40:01.574620 farmfs-0.8.7/bin/
--rwxr-xr-x   0 andrewthomson   (501) staff       (20)      355 2021-12-06 23:58:21.000000 farmfs-0.8.7/bin/snap.sh
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-02-11 18:40:01.579251 farmfs-0.8.7/farmfs/
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1008 2022-08-14 06:55:19.000000 farmfs-0.8.7/farmfs/__init__.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)     7364 2023-02-08 08:33:15.000000 farmfs-0.8.7/farmfs/blobstore.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)    16821 2022-12-11 20:50:03.000000 farmfs-0.8.7/farmfs/fs.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)     3878 2022-08-15 07:03:25.000000 farmfs-0.8.7/farmfs/keydb.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)        0 2020-04-07 22:47:13.000000 farmfs-0.8.7/farmfs/remote.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)     5700 2022-08-14 06:55:19.000000 farmfs-0.8.7/farmfs/snapshot.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1893 2022-08-14 06:55:19.000000 farmfs-0.8.7/farmfs/transduce.py
--rwxr-xr-x   0 andrewthomson   (501) staff       (20)    21597 2023-02-08 08:33:15.000000 farmfs-0.8.7/farmfs/ui.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)     7466 2022-12-11 17:44:07.000000 farmfs-0.8.7/farmfs/util.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)    11225 2023-02-08 08:33:15.000000 farmfs-0.8.7/farmfs/volume.py
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-02-11 18:40:01.582239 farmfs-0.8.7/farmfs.egg-info/
--rw-r--r--   0 andrewthomson   (501) staff       (20)     8138 2023-02-11 18:40:01.000000 farmfs-0.8.7/farmfs.egg-info/PKG-INFO
--rw-r--r--   0 andrewthomson   (501) staff       (20)      389 2023-02-11 18:40:01.000000 farmfs-0.8.7/farmfs.egg-info/SOURCES.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)        1 2023-02-11 18:40:01.000000 farmfs-0.8.7/farmfs.egg-info/dependency_links.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)       75 2023-02-11 18:40:01.000000 farmfs-0.8.7/farmfs.egg-info/entry_points.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)       72 2023-02-11 18:40:01.000000 farmfs-0.8.7/farmfs.egg-info/requires.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)        7 2023-02-11 18:40:01.000000 farmfs-0.8.7/farmfs.egg-info/top_level.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)       38 2023-02-11 18:40:01.583678 farmfs-0.8.7/setup.cfg
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1130 2023-02-08 08:00:54.000000 farmfs-0.8.7/setup.py
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-17 20:19:38.263761 farmfs-0.9.0/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1082 2020-04-07 22:47:13.000000 farmfs-0.9.0/LICENSE
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     6217 2023-04-17 20:19:38.263282 farmfs-0.9.0/PKG-INFO
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     5679 2023-04-14 05:03:52.000000 farmfs-0.9.0/README.md
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-17 20:19:38.252668 farmfs-0.9.0/bin/
+-rwxr-xr-x   0 andrewthomson   (501) staff       (20)      355 2021-12-06 23:58:21.000000 farmfs-0.9.0/bin/snap.sh
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-17 20:19:38.257084 farmfs-0.9.0/farmfs/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1008 2023-04-14 05:03:52.000000 farmfs-0.9.0/farmfs/__init__.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     7242 2023-04-17 20:19:23.000000 farmfs-0.9.0/farmfs/blobstore.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)    18379 2023-04-17 20:19:23.000000 farmfs-0.9.0/farmfs/fs.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     3878 2023-04-14 05:03:52.000000 farmfs-0.9.0/farmfs/keydb.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)        0 2020-04-07 22:47:13.000000 farmfs-0.9.0/farmfs/remote.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     5700 2023-04-14 05:03:52.000000 farmfs-0.9.0/farmfs/snapshot.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1893 2023-04-14 05:03:52.000000 farmfs-0.9.0/farmfs/transduce.py
+-rwxr-xr-x   0 andrewthomson   (501) staff       (20)    21499 2023-04-17 20:19:23.000000 farmfs-0.9.0/farmfs/ui.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     7466 2023-04-14 05:03:52.000000 farmfs-0.9.0/farmfs/util.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)    11476 2023-04-17 20:19:23.000000 farmfs-0.9.0/farmfs/volume.py
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-17 20:19:38.259622 farmfs-0.9.0/farmfs.egg-info/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     6217 2023-04-17 20:19:38.000000 farmfs-0.9.0/farmfs.egg-info/PKG-INFO
+-rw-r--r--   0 andrewthomson   (501) staff       (20)      531 2023-04-17 20:19:38.000000 farmfs-0.9.0/farmfs.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)        1 2023-04-17 20:19:38.000000 farmfs-0.9.0/farmfs.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       74 2023-04-17 20:19:38.000000 farmfs-0.9.0/farmfs.egg-info/entry_points.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       72 2023-04-17 20:19:38.000000 farmfs-0.9.0/farmfs.egg-info/requires.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)        7 2023-04-17 20:19:38.000000 farmfs-0.9.0/farmfs.egg-info/top_level.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       38 2023-04-17 20:19:38.263875 farmfs-0.9.0/setup.cfg
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1130 2023-04-17 20:19:23.000000 farmfs-0.9.0/setup.py
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-17 20:19:38.262673 farmfs-0.9.0/tests/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)      367 2023-04-14 05:03:52.000000 farmfs-0.9.0/tests/test_blobstore.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)    20995 2023-04-17 20:19:23.000000 farmfs-0.9.0/tests/test_fs.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     2695 2023-04-14 05:03:52.000000 farmfs-0.9.0/tests/test_keydb.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     3386 2023-04-14 05:03:52.000000 farmfs-0.9.0/tests/test_transduce.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)    21637 2023-04-14 20:06:10.000000 farmfs-0.9.0/tests/test_ui.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     8927 2023-04-14 05:03:52.000000 farmfs-0.9.0/tests/test_util.py
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     4124 2023-04-14 05:03:52.000000 farmfs-0.9.0/tests/test_volume.py
```

### Comparing `farmfs-0.8.7/LICENSE` & `farmfs-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/PKG-INFO` & `farmfs-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,255 +1,255 @@
 Metadata-Version: 2.1
 Name: farmfs
-Version: 0.8.7
+Version: 0.9.0
 Summary: tool which de-duplicates files in a filesystem by checksum.
 Home-page: http://github.com/andrewguy9/farmfs
 Author: Andrew Thomson
 Author-email: athomsonguy@gmail.com
 License: MIT
-Description: farmfs
-        ======
-        
-        Tool for creating / distributing / maintaining symlink farms.
-        
-        ## Warning
-        FarmFS is still very early stage software. 
-        
-        Please do not keep anything in it which you are not willing to lose.
-        
-        ## Installation
-        
-        ### To use Farmfs
-        
-        pip install git+https://github.com/andrewguy9/farmfs.git@master
-        
-        ### To hack on Farmfs
-        ```
-        git clone https://github.com/andrewguy9/farmfs.git
-        cd farmfs
-        python setup.py install
-        ```
-        
-        ## Usage:
-        ```
-        FarmFS
-        
-        Usage:
-          farmfs mkfs
-          farmfs (status|freeze|thaw) [<path>...]
-          farmfs snap (make|list|read|delete|restore) <snap>
-          farmfs fsck
-          farmfs count
-          farmfs similarity
-          farmfs gc
-          farmfs checksum <path>...
-          farmfs remote add <remote> <root>
-          farmfs remote remove <remote>
-          farmfs remote list
-          farmfs pull <remote> [<snap>]
-        
-        
-        Options:
-        
-        ```
-        ## What is FarmFS
-        
-        Farmfs is a git style interface to non text, usually immutable, sometimes large files.
-        It takes your files and puts them into an immutable blob store then builds symlinks from the file names into the store.
-        
-        ### Why would you do that?
-        * You can snapshot your directory structure BIG_O(num_files).
-        * You can diff two different farmfs stores with BIG_O(num_files) rather than BIG_O(sum(file_sizes))
-        * You can identify corruption of your files because all entries in the blob store are checksumed.
-        * If the same file contents appear in multiple places you only have to put it in the blob store once. (deduplication)
-        
-        ## Getting Started
-        
-        Create a Farmfs store
-        
-        ```
-        mkdir myfarm
-        cd myfarm
-        farmfs mkfs
-        ```
-        
-        Make some files
-        
-        ```
-        mkdir -p 1/2/3/4/5
-        mkdir -p a/b/c/d/e
-        echo "value1" > 1/2/3/4/5/v1
-        echo "value1" > a/b/c/d/e/v1
-        ```
-        
-        Status can show us unmanged files.
-        
-        ```
-        farmfs status
-        /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
-        /Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1
-        ```
-        
-        Add the untracked files to the blob store.
-        Notice it only needs to store "value1" once.
-        
-        ```
-        farmfs freeze
-        Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
-        Processing /Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Found a copy of file already in userdata, skipping copy
-        ```
-        
-        Edit a file.
-        First we need to thaw it, then we can change it.
-        
-        ```
-        farmfs thaw 1/2/3/4/5/v1
-        
-        farmfs status
-        /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
-        
-        echo "value2" > 1/2/3/4/5/v1
-        
-        farmfs freeze 1/2/3/4/5/v1
-        Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
-        
-        farmfs status
-        ```
-        
-        We don't want to loose our progress, so lets make a snapshot.
-        
-        ```
-        farmfs snap make mysnap
-        ```
-        
-        Now create more stuff
-        
-        ```
-        echo "oops" > mistake.txt
-        
-        farmfs freeze mistake.txt
-        Processing /Users/andrewguy9/Downloads/readme/mistake.txt with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/38a/f5c/549/26b620264ab1501150cf189
-        ```
-        
-        Well that was a mistake, lets roll back to the old snap.
-        
-        ```
-        farmfs snap restore mysnap
-        Removing /mistake.txt
-        ```
-        
-        Now that we have our files built, lets build another depot.
-        
-        ```
-        cd ..
-        mkdir copy
-        cd copy
-        farmfs mkfs
-        ```
-        
-        We want to add our prior depot as a remote.
-        
-        ```
-        farmfs remote add origin ../myfarm
-        ```
-        
-        Now lets copy our work from before.
-        
-        ```
-        farmfs pull origin
-        mkdir /1
-        mkdir /1/2
-        mkdir /1/2/3
-        mkdir /1/2/3/4
-        mkdir /1/2/3/4/5
-        mklink /1/2/3/4/5/v1 -> /4ca/8c5/ae5/e759e237bfb80c51940de7a
-        Blob missing from local, copying
-        *** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
-        mkdir /a
-        mkdir /a/b
-        mkdir /a/b/c
-        mkdir /a/b/c/d
-        mkdir /a/b/c/d/e
-        mklink /a/b/c/d/e/v1 -> /238/851/a91/77b60af767ca431ed521e55
-        Blob missing from local, copying
-        *** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55 /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
-        ```
-        
-        Lets see whats in our new depot:
-        
-        ```
-        find *
-        1
-        1/2
-        1/2/3
-        1/2/3/4
-        1/2/3/4/5
-        1/2/3/4/5/v1
-        a
-        a/b
-        a/b/c
-        a/b/c/d
-        a/b/c/d/e
-        a/b/c/d/e/v1
-        ```
-        ## Development:
-        
-        ### Testing:
-        
-        #### Regression Testing:
-        Regression tests can be run with `pytest`
-        Tests are kept in the `tests` directory, which will be detected by `pytest automatically`.
-        
-        #### Performance Optimization:
-        Performance testing cases are stored under the `perf` directory. These are useful for making development decisions are not generally useful as ongoing tests.
-        
-        These tests can by run using `pytest` or `tox`.
-        
-        `pytest`:
-        
-        To run a particular trial run:
-        * `pytest -s perf/your_test.py [-k case_pattern]`.
-        
-        Notice that the `-s` is required to get a printout of the results.
-        
-        Example: `pytest -s perf/transducer.py -k transducers`
-        
-        `tox`:
-        
-        To run a pattern in a particular environment run:
-        * `tox -e [envs] -- [-k case_pattern]`
-        
-        * Available envs are `{py37,py27,pypy,pypy3}-perf`
-        
-        Example: `tox -e py27-perf,py37-perf -- -k transducers`
-        
-        ### Debugging
-        
-        farmfs comes with a useful debugging tool `farmdbg`.
-        
-        ```
-        farmdbg
-        Usage:
-          farmdbg reverse <csum>
-          farmdbg key read <key>
-          farmdbg key write <key> <value>
-          farmdbg key delete <key>
-          farmdbg key list [<key>]
-          farmdbg walk (keys|userdata|root|snap <snapshot>)
-          farmdbg checksum <path>...
-          farmdbg fix link <file> <target>
-          farmdbg rewrite-links <target>
-        ```
-        
-        `farmdbg` can be used to dump parts of the keystore or blobstore, as well as walk and repair links.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Filesystems
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+farmfs
+======
+
+Tool for creating / distributing / maintaining symlink farms.
+
+## Warning
+FarmFS is still very early stage software. 
+
+Please do not keep anything in it which you are not willing to lose.
+
+## Installation
+
+### To use Farmfs
+
+pip install git+https://github.com/andrewguy9/farmfs.git@master
+
+### To hack on Farmfs
+```
+git clone https://github.com/andrewguy9/farmfs.git
+cd farmfs
+python setup.py install
+```
+
+## Usage:
+```
+FarmFS
+
+Usage:
+  farmfs mkfs
+  farmfs (status|freeze|thaw) [<path>...]
+  farmfs snap (make|list|read|delete|restore) <snap>
+  farmfs fsck
+  farmfs count
+  farmfs similarity
+  farmfs gc
+  farmfs checksum <path>...
+  farmfs remote add <remote> <root>
+  farmfs remote remove <remote>
+  farmfs remote list
+  farmfs pull <remote> [<snap>]
+
+
+Options:
+
+```
+## What is FarmFS
+
+Farmfs is a git style interface to non text, usually immutable, sometimes large files.
+It takes your files and puts them into an immutable blob store then builds symlinks from the file names into the store.
+
+### Why would you do that?
+* You can snapshot your directory structure BIG_O(num_files).
+* You can diff two different farmfs stores with BIG_O(num_files) rather than BIG_O(sum(file_sizes))
+* You can identify corruption of your files because all entries in the blob store are checksumed.
+* If the same file contents appear in multiple places you only have to put it in the blob store once. (deduplication)
+
+## Getting Started
+
+Create a Farmfs store
+
+```
+mkdir myfarm
+cd myfarm
+farmfs mkfs
+```
+
+Make some files
+
+```
+mkdir -p 1/2/3/4/5
+mkdir -p a/b/c/d/e
+echo "value1" > 1/2/3/4/5/v1
+echo "value1" > a/b/c/d/e/v1
+```
+
+Status can show us unmanged files.
+
+```
+farmfs status
+/Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
+/Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1
+```
+
+Add the untracked files to the blob store.
+Notice it only needs to store "value1" once.
+
+```
+farmfs freeze
+Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
+Processing /Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Found a copy of file already in userdata, skipping copy
+```
+
+Edit a file.
+First we need to thaw it, then we can change it.
+
+```
+farmfs thaw 1/2/3/4/5/v1
+
+farmfs status
+/Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
+
+echo "value2" > 1/2/3/4/5/v1
+
+farmfs freeze 1/2/3/4/5/v1
+Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
+
+farmfs status
+```
+
+We don't want to loose our progress, so lets make a snapshot.
+
+```
+farmfs snap make mysnap
+```
+
+Now create more stuff
+
+```
+echo "oops" > mistake.txt
+
+farmfs freeze mistake.txt
+Processing /Users/andrewguy9/Downloads/readme/mistake.txt with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/38a/f5c/549/26b620264ab1501150cf189
+```
+
+Well that was a mistake, lets roll back to the old snap.
+
+```
+farmfs snap restore mysnap
+Removing /mistake.txt
+```
+
+Now that we have our files built, lets build another depot.
+
+```
+cd ..
+mkdir copy
+cd copy
+farmfs mkfs
+```
+
+We want to add our prior depot as a remote.
+
+```
+farmfs remote add origin ../myfarm
+```
+
+Now lets copy our work from before.
+
+```
+farmfs pull origin
+mkdir /1
+mkdir /1/2
+mkdir /1/2/3
+mkdir /1/2/3/4
+mkdir /1/2/3/4/5
+mklink /1/2/3/4/5/v1 -> /4ca/8c5/ae5/e759e237bfb80c51940de7a
+Blob missing from local, copying
+*** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
+mkdir /a
+mkdir /a/b
+mkdir /a/b/c
+mkdir /a/b/c/d
+mkdir /a/b/c/d/e
+mklink /a/b/c/d/e/v1 -> /238/851/a91/77b60af767ca431ed521e55
+Blob missing from local, copying
+*** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55 /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
+```
+
+Lets see whats in our new depot:
+
+```
+find *
+1
+1/2
+1/2/3
+1/2/3/4
+1/2/3/4/5
+1/2/3/4/5/v1
+a
+a/b
+a/b/c
+a/b/c/d
+a/b/c/d/e
+a/b/c/d/e/v1
+```
+## Development:
+
+### Testing:
+
+#### Regression Testing:
+Regression tests can be run with `pytest`
+Tests are kept in the `tests` directory, which will be detected by `pytest automatically`.
+
+#### Performance Optimization:
+Performance testing cases are stored under the `perf` directory. These are useful for making development decisions are not generally useful as ongoing tests.
+
+These tests can by run using `pytest` or `tox`.
+
+`pytest`:
+
+To run a particular trial run:
+* `pytest -s perf/your_test.py [-k case_pattern]`.
+
+Notice that the `-s` is required to get a printout of the results.
+
+Example: `pytest -s perf/transducer.py -k transducers`
+
+`tox`:
+
+To run a pattern in a particular environment run:
+* `tox -e [envs] -- [-k case_pattern]`
+
+* Available envs are `{py37,py27,pypy,pypy3}-perf`
+
+Example: `tox -e py27-perf,py37-perf -- -k transducers`
+
+### Debugging
+
+farmfs comes with a useful debugging tool `farmdbg`.
+
+```
+farmdbg
+Usage:
+  farmdbg reverse <csum>
+  farmdbg key read <key>
+  farmdbg key write <key> <value>
+  farmdbg key delete <key>
+  farmdbg key list [<key>]
+  farmdbg walk (keys|userdata|root|snap <snapshot>)
+  farmdbg checksum <path>...
+  farmdbg fix link <file> <target>
+  farmdbg rewrite-links <target>
+```
+
+`farmdbg` can be used to dump parts of the keystore or blobstore, as well as walk and repair links.
```

### Comparing `farmfs-0.8.7/README.md` & `farmfs-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/farmfs/__init__.py` & `farmfs-0.9.0/farmfs/__init__.py`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/farmfs/blobstore.py` & `farmfs-0.9.0/farmfs/blobstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,20 +104,20 @@
         blob = self.csum_to_path(csum)
         duplicate = blob.exists()
         if not duplicate:
             ensure_link(blob, path)
             ensure_readonly(blob)
         return duplicate
 
-    def fetch_blob(self, remote, csum):
+    def fetch_blob(self, remote, csum, tmp_dir):
         src_blob = remote.csum_to_path(csum)
         dst_blob = self.csum_to_path(csum)
-        duplicate = dst_blob.exists()
-        if not duplicate:
-            ensure_copy(dst_blob, src_blob)
+        if not dst_blob.exists():
+            # Copy is able to move data across volumes.
+            ensure_copy(dst_blob, src_blob, tmp_dir)
 
     def link_to_blob(self, path, csum):
         """Forces path into a symlink to csum"""
         new_link = self.csum_to_path(csum)
         ensure_symlink(path, new_link)
         ensure_readonly(path)
 
@@ -198,13 +198,7 @@
                     # TODO put_object doesn't have a work cancellation feature.
                     result = s3.put_object(self.bucket, key, f)
             return result
         http_success = lambda status_headers: status_headers[0] >= 200 and status_headers[0] < 300
         s3_exception = lambda e: isinstance(e, ValueError)
         upload_repeater = repeater(uploader, max_tries=3, predicate=http_success, catch_predicate=s3_exception)
         return upload_repeater
-
-    def url(self, csum):
-        key = self.prefix + "/" + csum
-        s3 = s3conn(self.access_id, self.secret)
-        return s3.get_object_url(self.bucket, key)
-
```

### Comparing `farmfs-0.8.7/farmfs/fs.py` & `farmfs-0.9.0/farmfs/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 from os.path import normpath
 from os.path import split
 from os.path import stat as statc
 from os.path import splitext
 from shutil import copyfileobj
 from fnmatch import fnmatchcase
 from functools import total_ordering
-from farmfs.util import ingest, safetype, uncurry, first, ffilter
+from farmfs.util import ingest, safetype, uncurry, first, second, ffilter
 from future.utils import python_2_unicode_compatible
 from safeoutput import open as safeopen
+from safeoutput import _sameDir as sameDir
 from filetype import guess, Type
 import filetype
 
 ERRORS = [
     FileDoesNotExist,
     FileExists,
     DirectoryExists,
@@ -260,19 +261,46 @@
         assert isinstance(dst, Path)
         link(dst._path, self._path)
 
     def symlink(self, dst):
         assert isinstance(dst, Path)
         symlink(dst._path, self._path)
 
+    def copy_fd(self, src_fd, tmpdir=None):
+        """
+        Reads src_fd and puts the contents into a file located at self._path.
+        """
+        if tmpdir is None:
+            tmpfn = sameDir
+        else:
+            tmpfn = lambda _: tmpdir._path
+        mode = 'w'
+        if 'b' in src_fd.mode:
+            mode += 'b'
+        with safeopen(self._path, mode, useDir=tmpfn) as dst_fd:
+            copyfileobj(src_fd, dst_fd)
+
     # TODO this behavior is the opposite of what one would expect.
-    def copy(self, dst):
+    def copy_file(self, dst, tmpdir=None):
+        """
+        Copy self to path dst.
+        Does not attempt to ensure dst is a valid destination.
+        Raises IsADirectoryError and FileDoesNotExist on namespace errors.
+        The file will either be fully copied, or will not be created.
+        This is achieved via temp files and atomic swap.
+        This API works for large files, as data is read in chunks and sent
+        to the destination.
+        """
+        if tmpdir is None:
+            tmpfn = sameDir
+        else:
+            tmpfn = lambda _: tmpdir._path
         assert isinstance(dst, Path)
         with open(self._path, 'rb') as src_fd:
-            with safeopen(dst._path, 'wb') as dst_fd:
+            with safeopen(dst._path, 'wb', useDir=tmpfn) as dst_fd:
                 copyfileobj(src_fd, dst_fd)
 
     def unlink(self, clean=None):
         try:
             unlink(self._path)
         except OSError as e:
             if e.errno == FileDoesNotExist:
@@ -454,21 +482,36 @@
 
 # TODO this is used only for fsck readonly check.
 def is_readonly(path):
     mode = path.stat().st_mode
     writable = mode & write_mask
     return bool(writable)
 
-def ensure_copy(dst, src):
+def ensure_copy(dst, src, tmpdir=None):
     assert src.exists()
     parent = dst.parent()
     assert parent != dst, "dst and parent were the same!"
     ensure_dir(parent)
     ensure_absent(dst)
-    src.copy(dst)
+    src.copy_file(dst, tmpdir)
+
+def ensure_rename(dst, src):
+    parent = dst.parent()
+    src_parents = src.parents()
+    dst_parents = dst.parents()
+    if dst._path == src._path:
+        return  # No work to do.
+    elif src in dst_parents:
+        raise ValueError("src %s is a decendent of dst %s" % (src, dst))
+    elif dst in src_parents:
+        raise ValueError("dst %s is a decendent of src %s" % (dst, src))
+    else:
+        ensure_dir(parent)
+        ensure_absent(dst)
+        src.rename(dst)
 
 def ensure_symlink(path, target):
     ensure_symlink_unsafe(path, target._path)
 
 def ensure_symlink_unsafe(path, orig):
     parent = path.parent()
     assert parent != path, "Path and parent were the same!"
```

### Comparing `farmfs-0.8.7/farmfs/keydb.py` & `farmfs-0.9.0/farmfs/keydb.py`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/farmfs/snapshot.py` & `farmfs-0.9.0/farmfs/snapshot.py`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/farmfs/transduce.py` & `farmfs-0.9.0/farmfs/transduce.py`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/farmfs/ui.py` & `farmfs-0.9.0/farmfs/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,20 +53,14 @@
         return sys.stdout
 
 json_encoder = JSONEncoder(ensure_ascii=False, sort_keys=True)
 json_encode = lambda data: json_encoder.encode(data)
 json_printr = pipeline(list, json_encode, print)
 strs_printr = pipeline(fmap(print), consume)
 
-def eprint(*args, **kwargs):
-    print(*args, file=sys.stderr, **kwargs)
-
-
-debug = fmap(identify(eprint))
-
 def dict_printr(keys, d):
     print("\t".join([ingest(d.get(k, '')) for k in keys]))
 
 def dicts_printr(keys):
     return pipeline(fmap(partial(dict_printr, keys)), consume)
 
 
@@ -421,15 +415,15 @@
         b = ingest(args['<target>'])
         if not vol.bs.exists(b):
             print("blob %s doesn't exist" % b)
             if args['--remote']:
                 remote = vol.remotedb.read(args['--remote'])
             else:
                 raise ValueError("aborting due to missing blob")
-            vol.bs.fetch_blob(remote.bs, b)
+            vol.bs.fetch_blob(remote.bs, b, vol.tmp)
         else:
             pass  # b exists, can we check its checksum?
         vol.bs.link_to_blob(f, b)
     elif args['rewrite-links']:
         for item in vol.tree():
             if not item.is_link():
                 continue
```

### Comparing `farmfs-0.8.7/farmfs/util.py` & `farmfs-0.9.0/farmfs/util.py`

 * *Files identical despite different names*

### Comparing `farmfs-0.8.7/farmfs/volume.py` & `farmfs-0.9.0/farmfs/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,28 @@
 def _metadata_path(root):
     assert isinstance(root, Path)
     return root.join(".farmfs")
 
 def _keys_path(root):
     return _metadata_path(root).join("keys")
 
+def _tmp_path(root):
+    return _metadata_path(root).join("tmp")
+
 def _snaps_path(root):
     return _metadata_path(root).join("snaps")
 
 def mkfs(root, udd):
     assert isinstance(root, Path)
     assert isinstance(udd, Path)
     root.mkdir()
     _metadata_path(root).mkdir()
     _keys_path(root).mkdir()
     _snaps_path(root).mkdir()
+    _tmp_path(root).mkdir()
     kdb = KeyDB(_keys_path(root))
     # Make sure root key is removed.
     kdb.delete("root")
     kdb.write('udd', safetype(udd))
     udd.mkdir()
     kdb.write('status', {})
     FarmFSVolume(root)
@@ -72,14 +76,17 @@
 class FarmFSVolume:
     def __init__(self, root):
         assert isinstance(root, Path)
         self.root = root
         self.mdd = _metadata_path(root)
         self.keydb = KeyDB(_keys_path(root))
         self.udd = Path(self.keydb.read('udd'))
+        assert self.udd.isdir()
+        self.tmp = Path(_tmp_path(root))  # TODO maybe move to blobstore
+        assert self.tmp.isdir()
         self.bs = FileBlobstore(self.udd)
         self.snapdb = KeyDBFactory(KeyDBWindow("snaps", self.keydb), encode_snapshot, partial(decode_snapshot, self.bs.reverser))
         self.remotedb = KeyDBFactory(KeyDBWindow("remotes", self.keydb), encode_volume, decode_volume)
 
         exclude_file = Path('.farmignore', self.root)
         ignored = [safetype(self.mdd)]
         try:
@@ -121,15 +128,15 @@
         return {"path": path, "csum": csum, "was_dup": duplicate}
 
     # Note: This assumes a posix storage engine.
     def thaw(self, user_path):
         assert isinstance(user_path, Path)
         csum_path = user_path.readlink()
         user_path.unlink()
-        csum_path.copy(user_path)
+        csum_path.copy_file(user_path)
         return user_path
 
     def repair_link(self, path):
         """Find all broken links and point them back at UDD"""
         assert path.islink()
         oldlink = path.readlink()
         if oldlink.isfile():
@@ -238,15 +245,15 @@
     else:
         csum = None
     if delta.mode == delta.REMOVED:
         return (noop, partial(ensure_absent, path), ("Apply Removing %s", path))
     elif delta.mode == delta.DIR:
         return (noop, partial(ensure_dir, path), ("Apply mkdir %s", path))
     elif delta.mode == delta.LINK:
-        blob_op = partial(local_vol.bs.fetch_blob, remote_vol.bs, csum)
+        blob_op = partial(local_vol.bs.fetch_blob, remote_vol.bs, csum, local_vol.tmp)
         tree_op = partial(local_vol.bs.link_to_blob, path, csum)
         tree_desc = ("Apply mklink %s -> " + delta.csum, path)
         return (blob_op, tree_op, tree_desc)
     else:
         raise ValueError("Unknown mode in SnapDelta: %s" % delta.mode)
 
 # TODO yields lots of SnapDelta. Maybe in wrong file?
```

### Comparing `farmfs-0.8.7/farmfs.egg-info/PKG-INFO` & `farmfs-0.9.0/farmfs.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,255 +1,255 @@
 Metadata-Version: 2.1
 Name: farmfs
-Version: 0.8.7
+Version: 0.9.0
 Summary: tool which de-duplicates files in a filesystem by checksum.
 Home-page: http://github.com/andrewguy9/farmfs
 Author: Andrew Thomson
 Author-email: athomsonguy@gmail.com
 License: MIT
-Description: farmfs
-        ======
-        
-        Tool for creating / distributing / maintaining symlink farms.
-        
-        ## Warning
-        FarmFS is still very early stage software. 
-        
-        Please do not keep anything in it which you are not willing to lose.
-        
-        ## Installation
-        
-        ### To use Farmfs
-        
-        pip install git+https://github.com/andrewguy9/farmfs.git@master
-        
-        ### To hack on Farmfs
-        ```
-        git clone https://github.com/andrewguy9/farmfs.git
-        cd farmfs
-        python setup.py install
-        ```
-        
-        ## Usage:
-        ```
-        FarmFS
-        
-        Usage:
-          farmfs mkfs
-          farmfs (status|freeze|thaw) [<path>...]
-          farmfs snap (make|list|read|delete|restore) <snap>
-          farmfs fsck
-          farmfs count
-          farmfs similarity
-          farmfs gc
-          farmfs checksum <path>...
-          farmfs remote add <remote> <root>
-          farmfs remote remove <remote>
-          farmfs remote list
-          farmfs pull <remote> [<snap>]
-        
-        
-        Options:
-        
-        ```
-        ## What is FarmFS
-        
-        Farmfs is a git style interface to non text, usually immutable, sometimes large files.
-        It takes your files and puts them into an immutable blob store then builds symlinks from the file names into the store.
-        
-        ### Why would you do that?
-        * You can snapshot your directory structure BIG_O(num_files).
-        * You can diff two different farmfs stores with BIG_O(num_files) rather than BIG_O(sum(file_sizes))
-        * You can identify corruption of your files because all entries in the blob store are checksumed.
-        * If the same file contents appear in multiple places you only have to put it in the blob store once. (deduplication)
-        
-        ## Getting Started
-        
-        Create a Farmfs store
-        
-        ```
-        mkdir myfarm
-        cd myfarm
-        farmfs mkfs
-        ```
-        
-        Make some files
-        
-        ```
-        mkdir -p 1/2/3/4/5
-        mkdir -p a/b/c/d/e
-        echo "value1" > 1/2/3/4/5/v1
-        echo "value1" > a/b/c/d/e/v1
-        ```
-        
-        Status can show us unmanged files.
-        
-        ```
-        farmfs status
-        /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
-        /Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1
-        ```
-        
-        Add the untracked files to the blob store.
-        Notice it only needs to store "value1" once.
-        
-        ```
-        farmfs freeze
-        Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
-        Processing /Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Found a copy of file already in userdata, skipping copy
-        ```
-        
-        Edit a file.
-        First we need to thaw it, then we can change it.
-        
-        ```
-        farmfs thaw 1/2/3/4/5/v1
-        
-        farmfs status
-        /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
-        
-        echo "value2" > 1/2/3/4/5/v1
-        
-        farmfs freeze 1/2/3/4/5/v1
-        Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
-        
-        farmfs status
-        ```
-        
-        We don't want to loose our progress, so lets make a snapshot.
-        
-        ```
-        farmfs snap make mysnap
-        ```
-        
-        Now create more stuff
-        
-        ```
-        echo "oops" > mistake.txt
-        
-        farmfs freeze mistake.txt
-        Processing /Users/andrewguy9/Downloads/readme/mistake.txt with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
-        Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/38a/f5c/549/26b620264ab1501150cf189
-        ```
-        
-        Well that was a mistake, lets roll back to the old snap.
-        
-        ```
-        farmfs snap restore mysnap
-        Removing /mistake.txt
-        ```
-        
-        Now that we have our files built, lets build another depot.
-        
-        ```
-        cd ..
-        mkdir copy
-        cd copy
-        farmfs mkfs
-        ```
-        
-        We want to add our prior depot as a remote.
-        
-        ```
-        farmfs remote add origin ../myfarm
-        ```
-        
-        Now lets copy our work from before.
-        
-        ```
-        farmfs pull origin
-        mkdir /1
-        mkdir /1/2
-        mkdir /1/2/3
-        mkdir /1/2/3/4
-        mkdir /1/2/3/4/5
-        mklink /1/2/3/4/5/v1 -> /4ca/8c5/ae5/e759e237bfb80c51940de7a
-        Blob missing from local, copying
-        *** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
-        mkdir /a
-        mkdir /a/b
-        mkdir /a/b/c
-        mkdir /a/b/c/d
-        mkdir /a/b/c/d/e
-        mklink /a/b/c/d/e/v1 -> /238/851/a91/77b60af767ca431ed521e55
-        Blob missing from local, copying
-        *** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55 /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
-        ```
-        
-        Lets see whats in our new depot:
-        
-        ```
-        find *
-        1
-        1/2
-        1/2/3
-        1/2/3/4
-        1/2/3/4/5
-        1/2/3/4/5/v1
-        a
-        a/b
-        a/b/c
-        a/b/c/d
-        a/b/c/d/e
-        a/b/c/d/e/v1
-        ```
-        ## Development:
-        
-        ### Testing:
-        
-        #### Regression Testing:
-        Regression tests can be run with `pytest`
-        Tests are kept in the `tests` directory, which will be detected by `pytest automatically`.
-        
-        #### Performance Optimization:
-        Performance testing cases are stored under the `perf` directory. These are useful for making development decisions are not generally useful as ongoing tests.
-        
-        These tests can by run using `pytest` or `tox`.
-        
-        `pytest`:
-        
-        To run a particular trial run:
-        * `pytest -s perf/your_test.py [-k case_pattern]`.
-        
-        Notice that the `-s` is required to get a printout of the results.
-        
-        Example: `pytest -s perf/transducer.py -k transducers`
-        
-        `tox`:
-        
-        To run a pattern in a particular environment run:
-        * `tox -e [envs] -- [-k case_pattern]`
-        
-        * Available envs are `{py37,py27,pypy,pypy3}-perf`
-        
-        Example: `tox -e py27-perf,py37-perf -- -k transducers`
-        
-        ### Debugging
-        
-        farmfs comes with a useful debugging tool `farmdbg`.
-        
-        ```
-        farmdbg
-        Usage:
-          farmdbg reverse <csum>
-          farmdbg key read <key>
-          farmdbg key write <key> <value>
-          farmdbg key delete <key>
-          farmdbg key list [<key>]
-          farmdbg walk (keys|userdata|root|snap <snapshot>)
-          farmdbg checksum <path>...
-          farmdbg fix link <file> <target>
-          farmdbg rewrite-links <target>
-        ```
-        
-        `farmdbg` can be used to dump parts of the keystore or blobstore, as well as walk and repair links.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Filesystems
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+farmfs
+======
+
+Tool for creating / distributing / maintaining symlink farms.
+
+## Warning
+FarmFS is still very early stage software. 
+
+Please do not keep anything in it which you are not willing to lose.
+
+## Installation
+
+### To use Farmfs
+
+pip install git+https://github.com/andrewguy9/farmfs.git@master
+
+### To hack on Farmfs
+```
+git clone https://github.com/andrewguy9/farmfs.git
+cd farmfs
+python setup.py install
+```
+
+## Usage:
+```
+FarmFS
+
+Usage:
+  farmfs mkfs
+  farmfs (status|freeze|thaw) [<path>...]
+  farmfs snap (make|list|read|delete|restore) <snap>
+  farmfs fsck
+  farmfs count
+  farmfs similarity
+  farmfs gc
+  farmfs checksum <path>...
+  farmfs remote add <remote> <root>
+  farmfs remote remove <remote>
+  farmfs remote list
+  farmfs pull <remote> [<snap>]
+
+
+Options:
+
+```
+## What is FarmFS
+
+Farmfs is a git style interface to non text, usually immutable, sometimes large files.
+It takes your files and puts them into an immutable blob store then builds symlinks from the file names into the store.
+
+### Why would you do that?
+* You can snapshot your directory structure BIG_O(num_files).
+* You can diff two different farmfs stores with BIG_O(num_files) rather than BIG_O(sum(file_sizes))
+* You can identify corruption of your files because all entries in the blob store are checksumed.
+* If the same file contents appear in multiple places you only have to put it in the blob store once. (deduplication)
+
+## Getting Started
+
+Create a Farmfs store
+
+```
+mkdir myfarm
+cd myfarm
+farmfs mkfs
+```
+
+Make some files
+
+```
+mkdir -p 1/2/3/4/5
+mkdir -p a/b/c/d/e
+echo "value1" > 1/2/3/4/5/v1
+echo "value1" > a/b/c/d/e/v1
+```
+
+Status can show us unmanged files.
+
+```
+farmfs status
+/Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
+/Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1
+```
+
+Add the untracked files to the blob store.
+Notice it only needs to store "value1" once.
+
+```
+farmfs freeze
+Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
+Processing /Users/andrewguy9/Downloads/readme/a/b/c/d/e/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Found a copy of file already in userdata, skipping copy
+```
+
+Edit a file.
+First we need to thaw it, then we can change it.
+
+```
+farmfs thaw 1/2/3/4/5/v1
+
+farmfs status
+/Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1
+
+echo "value2" > 1/2/3/4/5/v1
+
+farmfs freeze 1/2/3/4/5/v1
+Processing /Users/andrewguy9/Downloads/readme/1/2/3/4/5/v1 with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
+
+farmfs status
+```
+
+We don't want to loose our progress, so lets make a snapshot.
+
+```
+farmfs snap make mysnap
+```
+
+Now create more stuff
+
+```
+echo "oops" > mistake.txt
+
+farmfs freeze mistake.txt
+Processing /Users/andrewguy9/Downloads/readme/mistake.txt with csum /Users/andrewguy9/Downloads/readme/.farmfs/userdata
+Putting link at /Users/andrewguy9/Downloads/readme/.farmfs/userdata/38a/f5c/549/26b620264ab1501150cf189
+```
+
+Well that was a mistake, lets roll back to the old snap.
+
+```
+farmfs snap restore mysnap
+Removing /mistake.txt
+```
+
+Now that we have our files built, lets build another depot.
+
+```
+cd ..
+mkdir copy
+cd copy
+farmfs mkfs
+```
+
+We want to add our prior depot as a remote.
+
+```
+farmfs remote add origin ../myfarm
+```
+
+Now lets copy our work from before.
+
+```
+farmfs pull origin
+mkdir /1
+mkdir /1/2
+mkdir /1/2/3
+mkdir /1/2/3/4
+mkdir /1/2/3/4/5
+mklink /1/2/3/4/5/v1 -> /4ca/8c5/ae5/e759e237bfb80c51940de7a
+Blob missing from local, copying
+*** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/4ca/8c5/ae5/e759e237bfb80c51940de7a
+mkdir /a
+mkdir /a/b
+mkdir /a/b/c
+mkdir /a/b/c/d
+mkdir /a/b/c/d/e
+mklink /a/b/c/d/e/v1 -> /238/851/a91/77b60af767ca431ed521e55
+Blob missing from local, copying
+*** /Users/andrewguy9/Downloads/copy/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55 /Users/andrewguy9/Downloads/myfarm/.farmfs/userdata/238/851/a91/77b60af767ca431ed521e55
+```
+
+Lets see whats in our new depot:
+
+```
+find *
+1
+1/2
+1/2/3
+1/2/3/4
+1/2/3/4/5
+1/2/3/4/5/v1
+a
+a/b
+a/b/c
+a/b/c/d
+a/b/c/d/e
+a/b/c/d/e/v1
+```
+## Development:
+
+### Testing:
+
+#### Regression Testing:
+Regression tests can be run with `pytest`
+Tests are kept in the `tests` directory, which will be detected by `pytest automatically`.
+
+#### Performance Optimization:
+Performance testing cases are stored under the `perf` directory. These are useful for making development decisions are not generally useful as ongoing tests.
+
+These tests can by run using `pytest` or `tox`.
+
+`pytest`:
+
+To run a particular trial run:
+* `pytest -s perf/your_test.py [-k case_pattern]`.
+
+Notice that the `-s` is required to get a printout of the results.
+
+Example: `pytest -s perf/transducer.py -k transducers`
+
+`tox`:
+
+To run a pattern in a particular environment run:
+* `tox -e [envs] -- [-k case_pattern]`
+
+* Available envs are `{py37,py27,pypy,pypy3}-perf`
+
+Example: `tox -e py27-perf,py37-perf -- -k transducers`
+
+### Debugging
+
+farmfs comes with a useful debugging tool `farmdbg`.
+
+```
+farmdbg
+Usage:
+  farmdbg reverse <csum>
+  farmdbg key read <key>
+  farmdbg key write <key> <value>
+  farmdbg key delete <key>
+  farmdbg key list [<key>]
+  farmdbg walk (keys|userdata|root|snap <snapshot>)
+  farmdbg checksum <path>...
+  farmdbg fix link <file> <target>
+  farmdbg rewrite-links <target>
+```
+
+`farmdbg` can be used to dump parts of the keystore or blobstore, as well as walk and repair links.
```

### Comparing `farmfs-0.8.7/setup.py` & `farmfs-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 import sys
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 
-requires = ['docopt', 'delnone', 'future', 'safeoutput>=2.0', 'filetype==1.0.6', "S3Lib>=1.6.1", 'tqdm']
+requires = ['docopt', 'delnone', 'future', 'safeoutput>=2.1', 'filetype==1.0.6', "S3Lib>=1.6.0", 'tqdm']
 
 test_requires = ['tox', 'pytest==4.6.8', 'tabulate']
 
 setup(
     name='farmfs',
-    version='0.8.7',
+    version='0.9.0',
     author='Andrew Thomson',
     author_email='athomsonguy@gmail.com',
     packages=['farmfs'],
     install_requires = requires,
     entry_points = {
       'console_scripts': [
         'farmfs = farmfs.ui:ui_main',
```

