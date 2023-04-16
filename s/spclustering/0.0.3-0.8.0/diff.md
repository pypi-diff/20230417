# Comparing `tmp/spclustering-0.0.3.tar.gz` & `tmp/spclustering-0.8.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spclustering-0.0.3.tar", last modified: Thu Jan 12 11:18:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

