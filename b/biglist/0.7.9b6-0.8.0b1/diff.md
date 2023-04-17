# Comparing `tmp/biglist-0.7.9b6.tar.gz` & `tmp/biglist-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.9b6.tar", last modified: Fri Apr 14 06:54:05 2023, max compression
+gzip compressed data, was "biglist-0.8.0b1.tar", last modified: Mon Apr 17 15:38:20 2023, max compression
```

## Comparing `biglist-0.7.9b6.tar` & `biglist-0.8.0b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b6/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b6/README.rst
--rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b6/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-14 06:27:24.443094 biglist-0.7.9b6/src/biglist/__init__.py
--rw-r--r--   0        0        0    17990 2023-04-14 06:46:49.671033 biglist-0.7.9b6/src/biglist/_base.py
--rw-r--r--   0        0        0    44172 2023-04-14 05:23:32.226273 biglist-0.7.9b6/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34770 2023-04-14 06:49:13.536597 biglist-0.7.9b6/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b6/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b6/src/biglist/py.typed
--rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.0b1/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.8.0b1/README.rst
+-rw-r--r--   0        0        0     1623 2023-04-15 03:17:01.146252 biglist-0.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-17 15:35:58.651653 biglist-0.8.0b1/src/biglist/__init__.py
+-rw-r--r--   0        0        0    17990 2023-04-15 03:17:01.146252 biglist-0.8.0b1/src/biglist/_base.py
+-rw-r--r--   0        0        0    44414 2023-04-15 03:17:01.146252 biglist-0.8.0b1/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34773 2023-04-17 15:34:16.400044 biglist-0.8.0b1/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-14 07:17:29.111106 biglist-0.8.0b1/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.0b1/src/biglist/py.typed
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 biglist-0.8.0b1/PKG-INFO
```

### Comparing `biglist-0.7.9b6/LICENSE` & `biglist-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b6/README.rst` & `biglist-0.8.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b6/pyproject.toml` & `biglist-0.8.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "biglist"
 authors = [
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
-    "upathlib >= 0.7.7b1",
+    "upathlib >= 0.7.7",
     "deprecation",
     "mpservice >= 0.11.9",
     "pyarrow >= 10.0.0",
     "typing-extensions",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
@@ -35,15 +35,15 @@
 lz4 = ["lz4"]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata-sphinx-theme",
 ]
 gcs = [
-    "upathlib[gcs] >= 0.7.7b1",
+    "upathlib[gcs] >= 0.7.7",
     "google-auth",
 ]
 parquet = []
 test = [
     "boltons",
     "mypy",
     "ruff",
@@ -52,15 +52,15 @@
 
 # `parquet` option became empty in 0.7.5 because `arrow` became mandatory.
 # To be removed later.
 
 
 # See https://beta.ruff.rs/docs/rules/
 [tool.ruff]
-target-version = "py310"
+target-version = "py38"
 select = ["E", "F", "S", "I001"]  # isort
 ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S608"]
 
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
```

### Comparing `biglist-0.7.9b6/src/biglist/__init__.py` & `biglist-0.8.0b1/src/biglist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.7.9b6"
+__version__ = "0.8.0b1"
```

### Comparing `biglist-0.7.9b6/src/biglist/_base.py` & `biglist-0.8.0b1/src/biglist/_base.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b6/src/biglist/_biglist.py` & `biglist-0.8.0b1/src/biglist/_biglist.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,20 +528,24 @@
         # this should almost guarantee the file name is unique, hence
         # we do not need to verify this file name does not exist in `data_files`.
         # Also include timestamp and item count in the file name, in case
         # later we decide to use these pieces of info.
         # Changes in 0.7.4: the time part changes from epoch to datetime, with guaranteed fixed length.
 
         data_file = self.data_path / filename
-        if self._file_dumper is None:
-            self._file_dumper = Dumper(self._get_thread_pool(), self._n_write_threads)
+
         if wait:
-            self._file_dumper.wait()
+            if self._file_dumper is not None:
+                self._file_dumper.wait()
             self.dump_data_file(data_file, buffer, **self._serialize_kwargs)
         else:
+            if self._file_dumper is None:
+                self._file_dumper = Dumper(
+                    self._get_thread_pool(), self._n_write_threads
+                )
             self._file_dumper.dump_file(
                 self.dump_data_file, data_file, buffer, **self._serialize_kwargs
             )
             # This call will return quickly if the dumper has queue
             # capacity for the file. The file meta data below
             # will be updated as if the saving has completed, although
             # it hasn't (it is only queued). This allows the waiting-to-be-saved
@@ -714,15 +718,16 @@
         # If task is already finished when this callback is being added,
         # then it is called immediately.
 
     def wait(self):
         """
         Wait to finish all the submitted dumping tasks.
         """
-        concurrent.futures.wait(self._tasks)
+        if self._tasks:
+            concurrent.futures.wait(self._tasks)
 
 
 class BiglistFileReader(FileReader[Element]):
     def __init__(self, path: PathType, loader: Callable[[Upath], Any]):
         """
         Parameters
         ----------
@@ -948,14 +953,15 @@
         return cls(path)
 
     def __init__(
         self,
         path: PathType,
         task_id: Optional[str] = None,
         worker_id: Optional[str] = None,
+        timeout: int | float = 120,
     ):
         """
         Create a Multiplexer object and use it to distribute the data elements that have been
         stored by :meth:`new`.
 
         Parameters
         ----------
@@ -972,14 +978,15 @@
         """
         if task_id is None:
             assert worker_id is None
         self.path = path
         self._task_id = task_id
         self._worker_id = worker_id
         self._data = None
+        self._timeout = timeout
 
     @property
     def data(self) -> Biglist:
         """
         Return the data elements stored in this Multiplexer.
         """
         if self._data is None:
@@ -1040,17 +1047,18 @@
         assert self._task_id
         if not self._worker_id:
             self._worker_id = "{} {}".format(
                 multiprocessing.current_process().name,
                 threading.current_thread().name,
             )
         worker_id = self._worker_id
+        timeout = self._timeout
         finfo = self._mux_info_file(self._task_id)
         while True:
-            with lock_to_use(finfo) as ff:
+            with lock_to_use(finfo, timeout=timeout) as ff:
                 # In concurrent use cases, I've observed
                 # `upathlib.LockAcquireError` raised here.
                 # User may want to do retry here.
                 ss = ff.read_json()
                 # In concurrent use cases, I've observed
                 # `FileNotFoundError` here. User may want
                 # to do retry here.
```

### Comparing `biglist-0.7.9b6/src/biglist/_parquet.py` & `biglist-0.8.0b1/src/biglist/_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,181 +44,14 @@
 #   gcs = pyarrow.fs.GcsFileSystem(access_token=cred.token, credential_token_expiration=cred.expiry)
 #   pfile = pyarrow.parquet.ParquetFile(gcs.open_input_file('bucket-name/path/to/file.parquet'))
 
 
 logger = logging.getLogger(__name__)
 
 
-class ParquetBiglist(BiglistBase):
-    """
-    ``ParquetBiglist`` defines a kind of "external biglist", that is,
-    it points to pre-existing Parquet files and provides facilities to read them.
-    As long as you use a ParquetBiglist object to read, it is assumed that
-    the dataset (all the data files) have not changed since the object was created
-    by :meth:`new`.
-    """
-
-    @classmethod
-    def new(
-        cls,
-        data_path: PathType | Sequence[PathType],
-        path: Optional[PathType] = None,
-        *,
-        suffix: str = ".parquet",
-        **kwargs,
-    ) -> ParquetBiglist:
-        """
-        This classmethod gathers info of the specified data files and
-        saves the info to facilitate reading the data files.
-        The data files remain "external" to the :class:`ParquetBiglist` object;
-        the "data" persisted and managed by the ParquetBiglist object
-        are the meta info about the Parquet data files.
-
-        If the number of data files is small, it's feasible to create a temporary
-        object of this class (by leaving ``path`` at the default value ``None``)
-        "on-the-fly" for one-time use.
-
-        Parameters
-        ----------
-        path
-            Passed on to :meth:`BiglistBase.new` of :class:`BiglistBase`.
-        data_path
-            Parquet file(s) or folder(s) containing Parquet files.
-
-            If this is a single path, then it's either a Parquet file or a directory.
-            If this is a list, each element is either a Parquet file or a directory;
-            there can be a mix of files and directories.
-            Directories are traversed recursively for Parquet files.
-            The paths can be local, or in the cloud, or a mix of both.
-
-            Once the info of all Parquet files are gathered,
-            their order is fixed as far as this :class:`ParquetBiglist` is concerned.
-            The data sequence represented by this ParquetBiglist follows this
-            order of the files. The order is determined as follows:
-
-                The order of the entries in ``data_path`` is preserved; if any entry is a
-                directory, the files therein (recursively) are sorted by the string
-                value of each file's full path.
-
-        suffix
-            Only files with this suffix will be included.
-            To include all files, use ``suffix='*'``.
-
-        **kwargs
-            additional arguments are passed on to ``__init__``.
-        """
-        if isinstance(data_path, (str, Path, Upath)):
-            #  TODO: in py 3.10, we will be able to do `isinstance(data_path, PathType)`
-            data_path = [resolve_path(data_path)]
-        else:
-            data_path = [resolve_path(p) for p in data_path]
-
-        def get_file_meta(p: Upath):
-            ff = ParquetFileReader.load_file(p)
-            meta = ff.metadata
-            return {
-                "path": str(p),  # str of full path
-                "num_rows": meta.num_rows,
-                # "row_groups_num_rows": [
-                #     meta.row_group(k).num_rows for k in range(meta.num_row_groups)
-                # ],
-            }
-
-        pool = _get_global_thread_pool()
-        tasks = []
-        for p in data_path:
-            if p.is_file():
-                if suffix == "*" or p.name.endswith(suffix):
-                    tasks.append(pool.submit(get_file_meta, p))
-            else:
-                tt = []
-                for pp in p.riterdir():
-                    if suffix == "*" or pp.name.endswith(suffix):
-                        tt.append((str(pp), pool.submit(get_file_meta, pp)))
-                tt.sort()
-                for p, t in tt:
-                    tasks.append(t)
-
-        assert tasks
-        datafiles = []
-        for k, t in enumerate(tasks):
-            datafiles.append(t.result())
-            if (k + 1) % 1000 == 0:
-                logger.info("processed %d files", k + 1)
-
-        datafiles_cumlength = list(
-            itertools.accumulate(v["num_rows"] for v in datafiles)
-        )
-
-        obj = super().new(path, **kwargs)  # type: ignore
-        obj.info["datapath"] = [str(p) for p in data_path]
-
-        # Removed in 0.7.4
-        # obj.info["datafiles"] = datafiles
-        # obj.info["datafiles_cumlength"] = datafiles_cumlength
-
-        # Added in 0.7.4
-        data_files_info = [
-            (a["path"], a["num_rows"], b)
-            for a, b in zip(datafiles, datafiles_cumlength)
-        ]
-        obj.info["data_files_info"] = data_files_info
-
-        obj.info["storage_format"] = "parquet"
-        obj.info["storage_version"] = 1
-        # `storage_version` is a flag for certain breaking changes in the implementation,
-        # such that certain parts of the code (mainly concerning I/O) need to
-        # branch into different treatments according to the version.
-        # This has little relation to `storage_format`.
-        # version 1 designator introduced in version 0.7.4.
-        # prior to 0.7.4 it is absent, and considered 0.
-
-        obj._info_file.write_json(obj.info, overwrite=True)
-
-        return obj
-
-    def __init__(self, *args, **kwargs):
-        """Please see doc of the base class."""
-        super().__init__(*args, **kwargs)
-        self.keep_files: bool = True
-        """Indicates whether the meta info persisted by this object should be kept or deleted when this object is garbage-collected.
-
-        This does *not* affect the external Parquet data files.
-        """
-
-        # For back compat. Added in 0.7.4.
-        if self.info and "data_files_info" not in self.info:
-            # This is not called by ``new``, instead is opening an existing dataset
-            assert self.storage_version == 0
-            data_files_info = [
-                (a["path"], a["num_rows"], b)
-                for a, b in zip(
-                    self.info["datafiles"], self.info["datafiles_cumlength"]
-                )
-            ]
-            self.info["data_files_info"] = data_files_info
-            with lock_to_use(self._info_file) as ff:
-                ff.write_json(self.info, overwrite=True)
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} at '{self.path}' with {len(self)} records in {len(self.files)} data file(s) stored at {self.info['datapath']}>"
-
-    @property
-    def storage_version(self) -> int:
-        return self.info.get("storage_version", 0)
-
-    @property
-    def files(self):
-        # This method should be cheap to call.
-        return ParquetFileSeq(
-            self.path,
-            self.info["data_files_info"],
-        )
-
-
 class ParquetFileReader(FileReader):
     @classmethod
     def get_gcsfs(cls, *, good_for_seconds=600) -> GcsFileSystem:
         """
         Obtain a `pyarrow.fs.GcsFileSystem`_ object with credentials given so that
         the GCP default process of inferring credentials (which involves
         env vars and file reading etc) will not be triggered.
@@ -560,49 +393,14 @@
             idx = self.column_names.index(name)
         z = self.file.read(columns=[name]).column(name)
         self._columns[idx] = z
         self._columns[name] = z
         return z
 
 
-class ParquetFileSeq(FileSeq[ParquetFileReader]):
-    def __init__(
-        self,
-        root_dir: Upath,
-        data_files_info: list[tuple[str, int, int]],
-    ):
-        """
-        Parameters
-        ----------
-        root_dir
-            Root directory for storage of meta info.
-        data_files_info
-            A list of data files that constitute the file sequence.
-            Each tuple in the list is comprised of a file path (relative to
-            ``root_dir``), number of data items in the file, and cumulative
-            number of data items in the files up to the one at hand.
-            Therefore, the order of the files in the list is significant.
-        """
-        self._root_dir = root_dir
-        self._data_files_info = data_files_info
-
-    @property
-    def path(self):
-        return self._root_dir
-
-    @property
-    def data_files_info(self):
-        return self._data_files_info
-
-    def __getitem__(self, idx: int):
-        return ParquetFileReader(
-            self._data_files_info[idx][0],
-        )
-
-
 class ParquetBatchData(Seq):
     """
     ``ParquetBatchData`` wraps a `pyarrow.Table`_ or `pyarrow.RecordBatch`_.
     The data is already in memory; this class does not involve file reading.
 
     :meth:`ParquetFileReader.data` and :meth:`ParquetFileReader.iter_batches` both
     return or yield ParquetBatchData.
@@ -753,14 +551,216 @@
     ----------
     path
         Path of the file.
     """
     return ParquetFileReader(path)
 
 
+class ParquetBiglist(BiglistBase):
+    """
+    ``ParquetBiglist`` defines a kind of "external biglist", that is,
+    it points to pre-existing Parquet files and provides facilities to read them.
+    As long as you use a ParquetBiglist object to read, it is assumed that
+    the dataset (all the data files) have not changed since the object was created
+    by :meth:`new`.
+    """
+
+    @classmethod
+    def new(
+        cls,
+        data_path: PathType | Sequence[PathType],
+        path: Optional[PathType] = None,
+        *,
+        suffix: str = ".parquet",
+        **kwargs,
+    ) -> ParquetBiglist:
+        """
+        This classmethod gathers info of the specified data files and
+        saves the info to facilitate reading the data files.
+        The data files remain "external" to the :class:`ParquetBiglist` object;
+        the "data" persisted and managed by the ParquetBiglist object
+        are the meta info about the Parquet data files.
+
+        If the number of data files is small, it's feasible to create a temporary
+        object of this class (by leaving ``path`` at the default value ``None``)
+        "on-the-fly" for one-time use.
+
+        Parameters
+        ----------
+        path
+            Passed on to :meth:`BiglistBase.new` of :class:`BiglistBase`.
+        data_path
+            Parquet file(s) or folder(s) containing Parquet files.
+
+            If this is a single path, then it's either a Parquet file or a directory.
+            If this is a list, each element is either a Parquet file or a directory;
+            there can be a mix of files and directories.
+            Directories are traversed recursively for Parquet files.
+            The paths can be local, or in the cloud, or a mix of both.
+
+            Once the info of all Parquet files are gathered,
+            their order is fixed as far as this :class:`ParquetBiglist` is concerned.
+            The data sequence represented by this ParquetBiglist follows this
+            order of the files. The order is determined as follows:
+
+                The order of the entries in ``data_path`` is preserved; if any entry is a
+                directory, the files therein (recursively) are sorted by the string
+                value of each file's full path.
+
+        suffix
+            Only files with this suffix will be included.
+            To include all files, use ``suffix='*'``.
+
+        **kwargs
+            additional arguments are passed on to ``__init__``.
+        """
+        if isinstance(data_path, (str, Path, Upath)):
+            #  TODO: in py 3.10, we will be able to do `isinstance(data_path, PathType)`
+            data_path = [resolve_path(data_path)]
+        else:
+            data_path = [resolve_path(p) for p in data_path]
+
+        def get_file_meta(p: Upath):
+            ff = ParquetFileReader.load_file(p)
+            meta = ff.metadata
+            return {
+                "path": str(p),  # str of full path
+                "num_rows": meta.num_rows,
+                # "row_groups_num_rows": [
+                #     meta.row_group(k).num_rows for k in range(meta.num_row_groups)
+                # ],
+            }
+
+        pool = _get_global_thread_pool()
+        tasks = []
+        for p in data_path:
+            if p.is_file():
+                if suffix == "*" or p.name.endswith(suffix):
+                    tasks.append(pool.submit(get_file_meta, p))
+            else:
+                tt = []
+                for pp in p.riterdir():
+                    if suffix == "*" or pp.name.endswith(suffix):
+                        tt.append((str(pp), pool.submit(get_file_meta, pp)))
+                tt.sort()
+                for p, t in tt:
+                    tasks.append(t)
+
+        assert tasks
+        datafiles = []
+        for k, t in enumerate(tasks):
+            datafiles.append(t.result())
+            if (k + 1) % 1000 == 0:
+                logger.info("processed %d files", k + 1)
+
+        datafiles_cumlength = list(
+            itertools.accumulate(v["num_rows"] for v in datafiles)
+        )
+
+        obj = super().new(path, **kwargs)  # type: ignore
+        obj.info["datapath"] = [str(p) for p in data_path]
+
+        # Removed in 0.7.4
+        # obj.info["datafiles"] = datafiles
+        # obj.info["datafiles_cumlength"] = datafiles_cumlength
+
+        # Added in 0.7.4
+        data_files_info = [
+            (a["path"], a["num_rows"], b)
+            for a, b in zip(datafiles, datafiles_cumlength)
+        ]
+        obj.info["data_files_info"] = data_files_info
+
+        obj.info["storage_format"] = "parquet"
+        obj.info["storage_version"] = 1
+        # `storage_version` is a flag for certain breaking changes in the implementation,
+        # such that certain parts of the code (mainly concerning I/O) need to
+        # branch into different treatments according to the version.
+        # This has little relation to `storage_format`.
+        # version 1 designator introduced in version 0.7.4.
+        # prior to 0.7.4 it is absent, and considered 0.
+
+        obj._info_file.write_json(obj.info, overwrite=True)
+
+        return obj
+
+    def __init__(self, *args, **kwargs):
+        """Please see doc of the base class."""
+        super().__init__(*args, **kwargs)
+        self.keep_files: bool = True
+        """Indicates whether the meta info persisted by this object should be kept or deleted when this object is garbage-collected.
+
+        This does *not* affect the external Parquet data files.
+        """
+
+        # For back compat. Added in 0.7.4.
+        if self.info and "data_files_info" not in self.info:
+            # This is not called by ``new``, instead is opening an existing dataset
+            assert self.storage_version == 0
+            data_files_info = [
+                (a["path"], a["num_rows"], b)
+                for a, b in zip(
+                    self.info["datafiles"], self.info["datafiles_cumlength"]
+                )
+            ]
+            self.info["data_files_info"] = data_files_info
+            with lock_to_use(self._info_file) as ff:
+                ff.write_json(self.info, overwrite=True)
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} at '{self.path}' with {len(self)} records in {len(self.files)} data file(s) stored at {self.info['datapath']}>"
+
+    @property
+    def storage_version(self) -> int:
+        return self.info.get("storage_version", 0)
+
+    @property
+    def files(self):
+        # This method should be cheap to call.
+        return ParquetFileSeq(
+            self.path,
+            self.info["data_files_info"],
+        )
+
+
+class ParquetFileSeq(FileSeq[ParquetFileReader]):
+    def __init__(
+        self,
+        root_dir: Upath,
+        data_files_info: list[tuple[str, int, int]],
+    ):
+        """
+        Parameters
+        ----------
+        root_dir
+            Root directory for storage of meta info.
+        data_files_info
+            A list of data files that constitute the file sequence.
+            Each tuple in the list is comprised of a file path (relative to
+            ``root_dir``), number of data items in the file, and cumulative
+            number of data items in the files up to the one at hand.
+            Therefore, the order of the files in the list is significant.
+        """
+        self._root_dir = root_dir
+        self._data_files_info = data_files_info
+
+    @property
+    def path(self):
+        return self._root_dir
+
+    @property
+    def data_files_info(self):
+        return self._data_files_info
+
+    def __getitem__(self, idx: int):
+        return ParquetFileReader(
+            self._data_files_info[idx][0],
+        )
+
+
 def make_parquet_type(type_spec: str | Sequence):
     """
     ``type_spec`` is a spec of arguments to one of pyarrow's data type
     `factory functions <https://arrow.apache.org/docs/python/api/datatypes.html#factory-functions>`_.
 
     For simple types, this may be just the type name (or function name), e.g. ``'bool_'``, ``'string'``, ``'float64'``.
 
@@ -912,15 +912,15 @@
         Passed on to `pyarrow.parquet.write_table() <https://arrow.apache.org/docs/python/generated/pyarrow.parquet.write_table.html>`_.
     """
     path = resolve_path(path)
     if isinstance(path, LocalUpath):
         path.parent.path.mkdir(exist_ok=True, parents=True)
     ff, pp = FileSystem.from_uri(str(path))
     if isinstance(ff, GcsFileSystem):
-        ff = ParquetBiglist.get_gcsfs()
+        ff = ParquetFileReader.get_gcsfs()
     pyarrow.parquet.write_table(table, ff.open_output_stream(pp), **kwargs)
 
 
 def write_arrays_to_parquet(
     data: Sequence[pyarrow.Array | pyarrow.ChunkedArray | Iterable],
     path: PathType,
     *,
```

### Comparing `biglist-0.7.9b6/src/biglist/_util.py` & `biglist-0.8.0b1/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b6/PKG-INFO` & `biglist-0.8.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.7.9b6
+Version: 0.8.0b1
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: upathlib >= 0.7.7b1
+Requires-Dist: upathlib >= 0.7.7
 Requires-Dist: deprecation
 Requires-Dist: mpservice >= 0.11.9
 Requires-Dist: pyarrow >= 10.0.0
 Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
-Requires-Dist: upathlib[gcs] >= 0.7.7b1 ; extra == "gcs"
+Requires-Dist: upathlib[gcs] >= 0.7.7 ; extra == "gcs"
 Requires-Dist: google-auth ; extra == "gcs"
 Requires-Dist: lz4 ; extra == "lz4"
 Requires-Dist: boltons ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: zstandard ; extra == "zstandard"
```

