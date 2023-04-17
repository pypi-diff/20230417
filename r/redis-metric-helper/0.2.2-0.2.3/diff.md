# Comparing `tmp/redis-metric-helper-0.2.2.tar.gz` & `tmp/redis_metric_helper-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.2.2.tar", last modified: Fri Apr 14 14:13:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

