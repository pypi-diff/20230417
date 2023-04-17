# Comparing `tmp/universalio-0.0.8.tar.gz` & `tmp/universalio-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\repo-work\universalio\dist\tmp2p94doa2\universalio-0.0.8.tar", last modified: Wed Jul  6 17:59:46 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

