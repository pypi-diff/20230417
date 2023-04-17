# Comparing `tmp/f4-0.4.3.tar.gz` & `tmp/f4-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.4.3.tar", last modified: Tue Apr 11 19:01:26 2023, max compression
+gzip compressed data, was "f4-0.5.0.tar", last modified: Mon Apr 17 18:30:13 2023, max compression
```

## Comparing `f4-0.4.3.tar` & `f4-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.277722 f4-0.4.3/
--rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.4.3/LICENSE
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-11 19:01:26.277842 f4-0.4.3/PKG-INFO
--rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.4.3/README.md
--rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.4.3/pyproject.toml
--rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-11 19:01:26.278326 f4-0.4.3/setup.cfg
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.272199 f4-0.4.3/src/
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.275648 f4-0.4.3/src/f4/
--rwxr-xr-x   0 srp33      (501) staff       (20)    38192 2023-04-11 18:58:51.000000 f4-0.4.3/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.4.3/src/f4/Parser.py
--rwxr-xr-x   0 srp33      (501) staff       (20)     8733 2023-04-04 23:15:09.000000 f4-0.4.3/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (501) staff       (20)      403 2023-03-31 04:56:48.000000 f4-0.4.3/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.277165 f4-0.4.3/src/f4.egg-info/
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.277438 f4-0.4.3/test/
--rwxr-xr-x   0 srp33      (501) staff       (20)    52520 2023-04-11 18:59:29.000000 f4-0.4.3/test/test.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.140896 f4-0.5.0/
+-rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.5.0/LICENSE
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:30:13.141029 f4-0.5.0/PKG-INFO
+-rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.5.0/README.md
+-rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.5.0/pyproject.toml
+-rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-17 18:30:13.141591 f4-0.5.0/setup.cfg
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.130260 f4-0.5.0/src/
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.137121 f4-0.5.0/src/f4/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    37708 2023-04-17 18:21:41.000000 f4-0.5.0/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.5.0/src/f4/Parser.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)     8780 2023-04-17 18:21:54.000000 f4-0.5.0/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)      446 2023-04-16 18:51:11.000000 f4-0.5.0/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.139108 f4-0.5.0/src/f4.egg-info/
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-17 18:30:13.000000 f4-0.5.0/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:30:13.139434 f4-0.5.0/test/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    52520 2023-04-17 09:22:56.000000 f4-0.5.0/test/test.py
```

### Comparing `f4-0.4.3/LICENSE` & `f4-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.4.3/PKG-INFO` & `f4-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.4.3
+Version: 0.5.0
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.4.3/setup.cfg` & `f4-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.4.3
+version = 0.5.0
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.4.3/src/f4/Builder.py` & `f4-0.5.0/src/f4/Builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .Parser import *
 from .Utilities import *
 
 #####################################################
 # Public function(s)
 #####################################################
 
-def convert_delimited_file(delimited_file_path, f4_file_path, index_columns=[], delimiter="\t", comment_prefix="#", compression_type=None, num_parallel=1, num_cols_per_chunk=None, num_rows_per_write=None, tmp_dir_path=None, verbose=False):
+def convert_delimited_file(delimited_file_path, f4_file_path, index_columns=[], delimiter="\t", comment_prefix="#", compression_type=None, num_parallel=1, num_cols_per_chunk=None, tmp_dir_path=None, verbose=False):
     if type(delimiter) != str:
         raise Exception("The delimiter value must be a string.")
 
     if delimiter not in ("\t"):
         raise Exception("Invalid delimiter. Must be \t.")
 
     delimiter = delimiter.encode()
@@ -18,23 +18,23 @@
         if type(comment_prefix) != str:
             raise Exception("The comment_prefix value must be a string.")
 
         comment_prefix = comment_prefix.encode()
 
         if comment_prefix == "":
             comment_prefix = None
-
-    # Guess an optimal value for this parameter, if not specified.
-    if not num_rows_per_write:
-        raw_num_rows = 0
-        with get_delimited_file_handle(delimited_file_path) as in_file:
-            for line in in_file:
-                raw_num_rows += 1
-
-        num_rows_per_write = ceil(raw_num_rows / (num_parallel * 2) + 1)
+    #
+    # # Guess an optimal value for this parameter, if not specified.
+    # if not num_rows_per_write:
+    #     raw_num_rows = 0
+    #     with get_delimited_file_handle(delimited_file_path) as in_file:
+    #         for line in in_file:
+    #             raw_num_rows += 1
+    #
+    #     num_rows_per_write = ceil(raw_num_rows / (num_parallel * 2) + 1)
 
     if num_parallel > 1:
         global joblib
         joblib = __import__('joblib', globals(), locals())
 
     print_message(f"Converting from {delimited_file_path}", verbose)
     tmp_dir_path_chunks, tmp_dir_path_outputs, tmp_dir_path_indexes = prepare_tmp_dirs(tmp_dir_path)
@@ -54,22 +54,22 @@
 
     if num_cols == 0:
         raise Exception(f"No data was detected in {delimited_file_path}.")
 
     # Iterate through the lines to summarize each column.
     print_message(f"Summarizing each column in {delimited_file_path}", verbose)
     if num_parallel == 1:
-        chunk_results = [parse_columns_chunk(delimited_file_path, delimiter, comment_prefix, 0, num_cols, num_rows_per_write, compression_type, verbose)]
+        chunk_results = [parse_columns_chunk(delimited_file_path, delimiter, comment_prefix, 0, num_cols, compression_type, verbose)]
     else:
         # Guess an optimal value for this parameter, if not specified.
         if not num_cols_per_chunk:
             num_cols_per_chunk = ceil(num_cols / (num_parallel * 2) + 1)
 
         column_chunk_indices = generate_chunk_ranges(num_cols, num_cols_per_chunk)
-        chunk_results = joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(parse_columns_chunk)(delimited_file_path, delimiter, comment_prefix, column_chunk[0], column_chunk[1], num_rows_per_write, compression_type, verbose) for column_chunk in column_chunk_indices)
+        chunk_results = joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(parse_columns_chunk)(delimited_file_path, delimiter, comment_prefix, column_chunk[0], column_chunk[1], compression_type, verbose) for column_chunk in column_chunk_indices)
 
     # Summarize the column sizes and types across the chunks.
     column_sizes = []
     column_types = []
     column_compression_dicts = {}
 
     for chunk_tuple in chunk_results:
@@ -86,21 +86,21 @@
     # When each chunk was processed, we went through all rows, so we can get these numbers from just the first chunk.
     num_rows = chunk_results[0][3]
 
     if num_rows == 0:
         raise Exception(f"A header row but no data rows were detected in {delimited_file_path}")
 
     print_message(f"Parsing chunks of {delimited_file_path} and saving to temp directory ({tmp_dir_path_chunks})", verbose)
-    line_lengths_dict = get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, column_compression_dicts, num_rows, num_parallel, num_rows_per_write, verbose)
+    line_lengths_dict = get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, column_compression_dicts, num_rows, num_parallel, verbose)
 
     print_message(f"Saving meta files for {f4_file_path}", verbose)
     write_meta_files(tmp_dir_path_outputs, column_sizes, line_lengths_dict, column_names, column_types, compression_type, column_compression_dicts, num_rows)
 
     print_message(f"Combining all data into a single file for {delimited_file_path}", verbose)
-    combine_into_single_file(tmp_dir_path_chunks, tmp_dir_path_outputs, f4_file_path, num_parallel, num_rows_per_write)
+    combine_into_single_file(tmp_dir_path_chunks, tmp_dir_path_outputs, f4_file_path, num_parallel)
 
     if index_columns:
         build_indexes(f4_file_path, index_columns, tmp_dir_path_indexes, verbose)
 
     remove_tmp_dir(tmp_dir_path_chunks)
     remove_tmp_dir(tmp_dir_path_outputs)
     remove_tmp_dir(tmp_dir_path_indexes)
@@ -305,15 +305,15 @@
         # Build a map of the column types and write this to a file.
         column_types_string, max_col_type_length = build_string_map(column_types)
         write_str_to_file(f"{tmp_dir_path_outputs}ct", column_types_string)
         write_str_to_file(f"{tmp_dir_path_outputs}mctl", str(max_col_type_length).encode())
 
     write_compression_info(tmp_dir_path_outputs, compression_type, column_compression_dicts, column_index_name_dict)
 
-def parse_columns_chunk(delimited_file_path, delimiter, comment_prefix, start_index, end_index, num_rows_per_write, compression_type, verbose):
+def parse_columns_chunk(delimited_file_path, delimiter, comment_prefix, start_index, end_index, compression_type, verbose):
     with get_delimited_file_handle(delimited_file_path) as in_file:
         exclude_comments_and_header(in_file, comment_prefix)
 
         # Initialize the column sizes and types.
         # We will count how many there are of each type.
         column_sizes_dict = {}
         column_types_values_dict = {}
@@ -333,15 +333,15 @@
                 column_sizes_dict[i] = max([column_sizes_dict[i], len(line_items[i])])
 
                 inferred_type = infer_type(line_items[i])
                 column_types_values_dict[i][inferred_type] += 1
 
             num_rows += 1
 
-            if num_rows > 0 and num_rows % num_rows_per_write == 0:
+            if num_rows > 0 and num_rows % 100 == 0:
                 print_message(f"Processed line {num_rows} of {delimited_file_path} for columns {start_index} - {end_index - 1}", verbose)
 
     column_types_dict = {}
     for i in range(start_index, end_index):
         column_types_dict[i] = infer_type_for_column(column_types_values_dict[i])
 
     column_compression_dicts = {}
@@ -400,42 +400,39 @@
                     #column_compression_dicts[i]["map"][bigram] = int2ba(j, length = length).to01()
                     column_compression_dicts[i]["map"][bigram] = j.to_bytes(length = num_bytes, byteorder = "big")
 
                 column_sizes_dict[i] = column_max_length_dict[i] * num_bytes
 
     return column_sizes_dict, column_types_dict, column_compression_dicts, num_rows
 
-def get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, num_rows, num_parallel, num_rows_per_write, verbose):
+def get_line_lengths_dict(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, num_rows, num_parallel, verbose):
     if num_parallel == 1:
-        line_lengths_dict = write_rows_chunk(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, 0, 0, num_rows, num_rows_per_write, verbose)
+        line_lengths_dict = write_rows_chunk(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, 0, 0, num_rows, verbose)
     else:
         row_chunk_indices = generate_chunk_ranges(num_rows, ceil(num_rows / num_parallel) + 1)
 
-        # We are doing the import here because it is slow.
-        line_lengths_dicts = joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(write_rows_chunk)(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, i, row_chunk[0], row_chunk[1], num_rows_per_write, verbose) for i, row_chunk in enumerate(row_chunk_indices))
+        line_lengths_dicts = joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(write_rows_chunk)(delimited_file_path, tmp_dir_path_chunks, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, i, row_chunk[0], row_chunk[1], verbose) for i, row_chunk in enumerate(row_chunk_indices))
 
         line_lengths_dict = {}
         for x in line_lengths_dicts:
             line_lengths_dict = {**line_lengths_dict, **x}
 
     return line_lengths_dict
 
-def write_rows_chunk(delimited_file_path, tmp_dir_path, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, chunk_number, start_index, end_index, num_rows_per_write, verbose):
+def write_rows_chunk(delimited_file_path, tmp_dir_path, delimiter, comment_prefix, compression_type, column_sizes, compression_dicts, chunk_number, start_index, end_index, verbose):
     line_lengths_dict = {}
 
     if compression_type == "zstd":
         compressor = ZstdCompressor(level = 1)
 
     # Write the data to output file. Ignore the header line.
     with get_delimited_file_handle(delimited_file_path) as in_file:
         exclude_comments_and_header(in_file, comment_prefix)
 
         with open(f"{tmp_dir_path}{chunk_number}", 'wb') as chunk_file:
-            out_lines = []
-
             line_index = -1
             for line in in_file:
                 # Check whether we should process the specified line.
                 line_index += 1
                 if line_index < start_index:
                     continue
                 if line_index == end_index:
@@ -460,23 +457,19 @@
 
                 out_line = b"".join(out_items)
 
                 if compression_type == "zstd":
                     out_line = compressor.compress(out_line)
 
                 line_lengths_dict[line_index] = len(out_line)
-                out_lines.append(out_line)
 
-                if len(out_lines) % num_rows_per_write == 0:
+                if line_index % 100 == 0:
                     print_message(f"Processed chunk of {delimited_file_path} at line {line_index} (start_index = {start_index}, end_index = {end_index})", verbose)
-                    chunk_file.write(b"".join(out_lines))
-                    out_lines = []
 
-            if len(out_lines) > 0:
-                chunk_file.write(b"".join(out_lines))
+                chunk_file.write(out_line)
 
     return line_lengths_dict
 
 def exclude_comments_and_header(in_file, comment_prefix):
     # Ignore the header because we don't need column names here. Also ignore commented lines.
     if comment_prefix:
         for line in in_file:
```

### Comparing `f4-0.4.3/src/f4/Parser.py` & `f4-0.5.0/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.4.3/src/f4/Utilities.py` & `f4-0.5.0/src/f4/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 # We use these dictionaries so that when we store the file map, it takes less space on disk.
 FILE_KEY_ABBREVIATIONS_STATS = {"mccl": 3, "mctl": 6, "cnmccl": 10, "cnll": 11}
 FILE_KEY_ABBREVIATIONS_OTHER = {"ll": 4, "cmpr": 7}
 FILE_KEY_ABBREVIATIONS_NOCACHE = {"data": 1, "cc": 2, "ct": 5, "cndata": 8, "cncc": 9}
 
+def get_current_version():
+    return "0.5.0"
+
 def read_str_from_file(file_path, file_extension=""):
     with open(file_path + file_extension, 'rb') as the_file:
         return the_file.read()
 
 def write_str_to_file(file_path, the_string):
     with open(file_path, 'wb') as the_file:
         the_file.write(the_string)
```

### Comparing `f4-0.4.3/src/f4.egg-info/PKG-INFO` & `f4-0.5.0/src/f4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.4.3
+Version: 0.5.0
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.4.3/test/test.py` & `f4-0.5.0/test/test.py`

 * *Files identical despite different names*

