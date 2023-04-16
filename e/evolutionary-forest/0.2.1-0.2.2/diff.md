# Comparing `tmp/evolutionary_forest-0.2.1.tar.gz` & `tmp/evolutionary_forest-0.2.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolutionary_forest-0.2.1.tar", last modified: Sun Apr 16 04:50:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

