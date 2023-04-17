# Comparing `tmp/abch_tree_sitter-1.0.1.tar.gz` & `tmp/abch_tree_sitter-1.1.0-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abch_tree_sitter-1.0.1.tar", last modified: Fri Apr  7 18:58:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

