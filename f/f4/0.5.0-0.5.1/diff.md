# Comparing `tmp/f4-0.5.0.tar.gz` & `tmp/f4-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.5.0.tar", last modified: Mon Apr 17 18:30:13 2023, max compression
+gzip compressed data, was "f4-0.5.1.tar", last modified: Mon Apr 17 18:39:05 2023, max compression
```

## Comparing `f4-0.5.0.tar` & `f4-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.140896 f4-0.5.0/
--rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.5.0/LICENSE
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:30:13.141029 f4-0.5.0/PKG-INFO
--rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.5.0/README.md
--rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.5.0/pyproject.toml
--rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-17 18:30:13.141591 f4-0.5.0/setup.cfg
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.130260 f4-0.5.0/src/
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.137121 f4-0.5.0/src/f4/
--rwxr-xr-x   0 srp33      (501) staff       (20)    37708 2023-04-17 18:21:41.000000 f4-0.5.0/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.5.0/src/f4/Parser.py
--rwxr-xr-x   0 srp33      (501) staff       (20)     8780 2023-04-17 18:21:54.000000 f4-0.5.0/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (501) staff       (20)      446 2023-04-16 18:51:11.000000 f4-0.5.0/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.139108 f4-0.5.0/src/f4.egg-info/
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.139434 f4-0.5.0/test/
--rwxr-xr-x   0 srp33      (501) staff       (20)    52520 2023-04-17 09:22:56.000000 f4-0.5.0/test/test.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:39:05.912236 f4-0.5.1/
+-rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.5.1/LICENSE
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:39:05.912354 f4-0.5.1/PKG-INFO
+-rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.5.1/README.md
+-rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.5.1/pyproject.toml
+-rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-17 18:39:05.912905 f4-0.5.1/setup.cfg
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:39:05.903257 f4-0.5.1/src/
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:39:05.908878 f4-0.5.1/src/f4/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    37590 2023-04-17 18:36:18.000000 f4-0.5.1/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.5.1/src/f4/Parser.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)     8780 2023-04-17 18:38:02.000000 f4-0.5.1/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)      446 2023-04-16 18:51:11.000000 f4-0.5.1/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:39:05.910878 f4-0.5.1/src/f4.egg-info/
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:39:05.000000 f4-0.5.1/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-17 18:39:05.000000 f4-0.5.1/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-17 18:39:05.000000 f4-0.5.1/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-17 18:39:05.000000 f4-0.5.1/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-17 18:39:05.000000 f4-0.5.1/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:39:05.911201 f4-0.5.1/test/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    52520 2023-04-17 09:22:56.000000 f4-0.5.1/test/test.py
```

### Comparing `f4-0.5.0/LICENSE` & `f4-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.5.0/PKG-INFO` & `f4-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.5.0/setup.cfg` & `f4-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.5.0
+version = 0.5.1
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.5.0/src/f4/Builder.py` & `f4-0.5.1/src/f4/Builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,14 @@
         if type(comment_prefix) != str:
             raise Exception("The comment_prefix value must be a string.")
 
         comment_prefix = comment_prefix.encode()
 
         if comment_prefix == "":
             comment_prefix = None
-    #
-    # # Guess an optimal value for this parameter, if not specified.
-    # if not num_rows_per_write:
-    #     raw_num_rows = 0
-    #     with get_delimited_file_handle(delimited_file_path) as in_file:
-    #         for line in in_file:
-    #             raw_num_rows += 1
-    #
-    #     num_rows_per_write = ceil(raw_num_rows / (num_parallel * 2) + 1)
 
     if num_parallel > 1:
         global joblib
         joblib = __import__('joblib', globals(), locals())
 
     print_message(f"Converting from {delimited_file_path}", verbose)
     tmp_dir_path_chunks, tmp_dir_path_outputs, tmp_dir_path_indexes = prepare_tmp_dirs(tmp_dir_path)
@@ -85,16 +76,19 @@
 
     # When each chunk was processed, we went through all rows, so we can get these numbers from just the first chunk.
     num_rows = chunk_results[0][3]
 
     if num_rows == 0:
         raise Exception(f"A header row but no data rows were detected in {delimited_file_path}")
 
+    #num_rows_per_print = ceil(num_rows / (num_parallel * 2) + 1)
+    num_rows_per_print = 100 if num_rows < 100000 else 10000
+
     print_message(f"Parsing chunks of {delimited_file_path} and saving to temp directory ({tmp_dir_path_chunks})", verbose)
-    line_lengths_dict = get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, column_compression_dicts, num_rows, num_parallel, verbose)
+    line_lengths_dict = get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, column_compression_dicts, num_rows, num_parallel, num_rows_per_print, verbose)
 
     print_message(f"Saving meta files for {f4_file_path}", verbose)
     write_meta_files(tmp_dir_path_outputs, column_sizes, line_lengths_dict, column_names, column_types, compression_type, column_compression_dicts, num_rows)
 
     print_message(f"Combining all data into a single file for {delimited_file_path}", verbose)
     combine_into_single_file(tmp_dir_path_chunks, tmp_dir_path_outputs, f4_file_path, num_parallel)
 
@@ -400,29 +394,29 @@
                     #column_compression_dicts[i]["map"][bigram] = int2ba(j, length = length).to01()
                     column_compression_dicts[i]["map"][bigram] = j.to_bytes(length = num_bytes, byteorder = "big")
 
                 column_sizes_dict[i] = column_max_length_dict[i] * num_bytes
 
     return column_sizes_dict, column_types_dict, column_compression_dicts, num_rows
 
-def get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, num_rows, num_parallel, verbose):
+def get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, num_rows, num_parallel, num_rows_per_print, verbose):
     if num_parallel == 1:
-        line_lengths_dict = write_rows_chunk(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, 0, 0, num_rows, verbose)
+        line_lengths_dict = write_rows_chunk(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, 0, 0, num_rows, num_rows_per_print, verbose)
     else:
         row_chunk_indices = generate_chunk_ranges(num_rows, ceil(num_rows / num_parallel) + 1)
 
-        line_lengths_dicts = joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(write_rows_chunk)(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, i, row_chunk[0], row_chunk[1], verbose) for i, row_chunk in enumerate(row_chunk_indices))
+        line_lengths_dicts = joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(write_rows_chunk)(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, i, row_chunk[0], row_chunk[1], num_rows_per_print, verbose) for i, row_chunk in enumerate(row_chunk_indices))
 
         line_lengths_dict = {}
         for x in line_lengths_dicts:
             line_lengths_dict = {**line_lengths_dict, **x}
 
     return line_lengths_dict
 
-def write_rows_chunk(delimited_file_path, tmp_dir_path, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, chunk_number, start_index, end_index, verbose):
+def write_rows_chunk(delimited_file_path, tmp_dir_path, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, chunk_number, start_index, end_index, num_rows_per_print, verbose):
     line_lengths_dict = {}
 
     if compression_type == "zstd":
         compressor = ZstdCompressor(level = 1)
 
     # Write the data to output file. Ignore the header line.
     with get_delimited_file_handle(delimited_file_path) as in_file:
@@ -458,15 +452,15 @@
                 out_line = b"".join(out_items)
 
                 if compression_type == "zstd":
                     out_line = compressor.compress(out_line)
 
                 line_lengths_dict[line_index] = len(out_line)
 
-                if line_index % 100 == 0:
+                if line_index % num_rows_per_print == 0:
                     print_message(f"Processed chunk of {delimited_file_path} at line {line_index} (start_index = {start_index}, end_index = {end_index})", verbose)
 
                 chunk_file.write(out_line)
 
     return line_lengths_dict
 
 def exclude_comments_and_header(in_file, comment_prefix):
```

### Comparing `f4-0.5.0/src/f4/Parser.py` & `f4-0.5.1/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.5.0/src/f4/Utilities.py` & `f4-0.5.1/src/f4/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # We use these dictionaries so that when we store the file map, it takes less space on disk.
 FILE_KEY_ABBREVIATIONS_STATS = {"mccl": 3, "mctl": 6, "cnmccl": 10, "cnll": 11}
 FILE_KEY_ABBREVIATIONS_OTHER = {"ll": 4, "cmpr": 7}
 FILE_KEY_ABBREVIATIONS_NOCACHE = {"data": 1, "cc": 2, "ct": 5, "cndata": 8, "cncc": 9}
 
 def get_current_version():
-    return "0.5.0"
+    return "0.5.1"
 
 def read_str_from_file(file_path, file_extension=""):
     with open(file_path + file_extension, 'rb') as the_file:
         return the_file.read()
 
 def write_str_to_file(file_path, the_string):
     with open(file_path, 'wb') as the_file:
```

### Comparing `f4-0.5.0/src/f4.egg-info/PKG-INFO` & `f4-0.5.1/src/f4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.5.0/test/test.py` & `f4-0.5.1/test/test.py`

 * *Files identical despite different names*

