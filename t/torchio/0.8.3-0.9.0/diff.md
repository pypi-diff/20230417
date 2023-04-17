# Comparing `tmp/torchio-0.8.3.tar.gz` & `tmp/torchio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchio-0.8.3.tar", last modified: Fri Jan 10 18:52:59 2020, max compression
+gzip compressed data, was "dist/torchio-0.9.0.tar", last modified: Tue Jan 14 10:20:21 2020, max compression
```

## Comparing `torchio-0.8.3.tar` & `torchio-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,77 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-01-10 18:49:11.000000 torchio-0.8.3/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3511 2020-01-10 18:49:11.000000 torchio-0.8.3/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2020-01-10 18:49:11.000000 torchio-0.8.3/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2020-01-10 18:49:11.000000 torchio-0.8.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-01-10 18:49:11.000000 torchio-0.8.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    16290 2020-01-10 18:52:59.000000 torchio-0.8.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11647 2020-01-10 18:49:11.000000 torchio-0.8.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4805 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      769 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-01-10 18:49:11.000000 torchio-0.8.3/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      390 2020-01-10 18:52:59.000000 torchio-0.8.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2020-01-10 18:49:11.000000 torchio-0.8.3/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2020-01-10 18:49:11.000000 torchio-0.8.3/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3630 2020-01-10 18:49:11.000000 torchio-0.8.3/tests/test_images_dataset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2020-01-10 18:49:11.000000 torchio-0.8.3/tests/test_random_elastic_deformation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      823 2020-01-10 18:49:11.000000 torchio-0.8.3/tests/test_torchio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2020-01-10 18:49:11.000000 torchio-0.8.3/tests/test_transforms.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio/
--rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      399 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/cli.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio/dataset/
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/dataset/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4324 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/dataset/images.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio/inference/
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/inference/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2173 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/inference/aggregator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3251 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/inference/grid_sampler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/io.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4458 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/queue.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio/sampler/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/sampler/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      971 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/sampler/label.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/sampler/sampler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/torchio.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio/transforms/
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6439 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/histogram_standardization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/interpolation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3779 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_affine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3435 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_bias_field.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4254 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_elastic_deformation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1470 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_flip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8251 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_motion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_noise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2138 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/random_transform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1257 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/rescale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1160 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/transform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/transforms/z_normalization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2020-01-10 18:49:11.000000 torchio-0.8.3/torchio/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16290 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1423 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-10 18:52:59.000000 torchio-0.8.3/torchio.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-01-14 10:16:31.000000 torchio-0.9.0/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3511 2020-01-14 10:16:31.000000 torchio-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2020-01-14 10:16:31.000000 torchio-0.9.0/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2020-01-14 10:16:31.000000 torchio-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-01-14 10:16:31.000000 torchio-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16655 2020-01-14 10:20:21.000000 torchio-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11940 2020-01-14 10:16:31.000000 torchio-0.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      608 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/authors.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4805 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      769 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-01-14 10:16:31.000000 torchio-0.9.0/docs/usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      390 2020-01-14 10:20:21.000000 torchio-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1734 2020-01-14 10:16:31.000000 torchio-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       37 2020-01-14 10:16:31.000000 torchio-0.9.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3953 2020-01-14 10:16:31.000000 torchio-0.9.0/tests/test_images_dataset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2020-01-14 10:16:31.000000 torchio-0.9.0/tests/test_random_elastic_deformation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1347 2020-01-14 10:16:31.000000 torchio-0.9.0/tests/test_random_motion.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2020-01-14 10:16:31.000000 torchio-0.9.0/tests/test_torchio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2039 2020-01-14 10:16:31.000000 torchio-0.9.0/tests/test_transforms.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2228 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/cli.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/dataset/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/dataset/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4346 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/dataset/images.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/inference/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       77 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/inference/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2173 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/inference/aggregator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3251 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/inference/grid_sampler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/io.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4458 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/queue.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/sampler/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/sampler/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      971 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/sampler/label.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/sampler/sampler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/torchio.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/transforms/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/transforms/augmentation/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/transforms/augmentation/intensity/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/intensity/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3424 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/intensity/random_bias_field.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8637 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/intensity/random_motion.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      980 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/intensity/random_noise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/interpolation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/random_transform.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/transforms/augmentation/spatial/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/spatial/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3756 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/spatial/random_affine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4231 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/spatial/random_elastic_deformation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1457 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/augmentation/spatial/random_flip.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio/transforms/normalization/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      197 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/normalization/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6256 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/normalization/histogram_standardization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1751 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/normalization/normalization_transform.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/normalization/rescale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      706 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/normalization/z_normalization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1160 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/transforms/transform.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2020-01-14 10:16:31.000000 torchio-0.9.0/torchio/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16655 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-14 10:20:21.000000 torchio-0.9.0/torchio.egg-info/top_level.txt
```

### Comparing `torchio-0.8.3/CONTRIBUTING.rst` & `torchio-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/HISTORY.rst` & `torchio-0.9.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/LICENSE` & `torchio-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/PKG-INFO` & `torchio-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchio
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tools for loading, augmenting and writing 3D medical images on PyTorch.
 Home-page: https://github.com/fepegar/torchio
 Author: Fernando Perez-Garcia
 Author-email: fernando.perezgarcia.17@ucl.ac.uk
 License: MIT license
 Description: # TorchIO
         
@@ -76,19 +76,20 @@
         [`torchio.Image`](torchio/dataset/images.py) instances.
         The paths suffix must be `.nii`, `.nii.gz` or `.nrrd`.
         
         ```python
         import torchio
         
         subject_a = [
-            Image('t1', '~/Dropbox/MRI/t1.nii.gz', torchio.INTENSITY),
+            Image('t1', '~/Dropbox/MRI/t1.nrrd', torchio.INTENSITY),
             Image('label', '~/Dropbox/MRI/t1_seg.nii.gz', torchio.LABEL),
         ]
         subject_b = [
             Image('t1', '/tmp/colin27_t1_tal_lin.nii.gz', torchio.INTENSITY),
+            Image('t2', '/tmp/colin27_t2_tal_lin.nii', torchio.INTENSITY),
             Image('label', '/tmp/colin27_seg1.nii.gz', torchio.LABEL),
         ]
         subjects_list = [subject_a, subject_b]
         subjects_dataset = torchio.ImagesDataset(subjects_list)
         subject_sample = subjects_dataset[0]
         ```
         
@@ -162,14 +163,22 @@
         
         ### Transforms
         
         The transforms package should remind users of
         [`torchvision.transforms`](https://pytorch.org/docs/stable/torchvision/transforms.html).
         They take as input the samples generated by an [`ImagesDataset`](#dataset).
         
+        A transform can be quickly applied to an image file using the command-line
+        tool `torchio-transform`:
+        
+        ```shell
+        $ torchio-transform input.nii.gz RandomMotion output.nii.gz --kwargs
+        "proportion_to_augment=1,num_transforms=4"
+        ```
+        
         #### Intensity
         
         ##### [MRI k-space motion artifacts](torchio/transforms/random_motion.py)
         
         Magnetic resonance images suffer from motion artifacts when the subject moves
         during image acquisition. This transform follows
         [Shaw et al., 2019](http://proceedings.mlr.press/v102/shaw19a.html) to
```

### Comparing `torchio-0.8.3/README.md` & `torchio-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -68,19 +68,20 @@
 [`torchio.Image`](torchio/dataset/images.py) instances.
 The paths suffix must be `.nii`, `.nii.gz` or `.nrrd`.
 
 ```python
 import torchio
 
 subject_a = [
-    Image('t1', '~/Dropbox/MRI/t1.nii.gz', torchio.INTENSITY),
+    Image('t1', '~/Dropbox/MRI/t1.nrrd', torchio.INTENSITY),
     Image('label', '~/Dropbox/MRI/t1_seg.nii.gz', torchio.LABEL),
 ]
 subject_b = [
     Image('t1', '/tmp/colin27_t1_tal_lin.nii.gz', torchio.INTENSITY),
+    Image('t2', '/tmp/colin27_t2_tal_lin.nii', torchio.INTENSITY),
     Image('label', '/tmp/colin27_seg1.nii.gz', torchio.LABEL),
 ]
 subjects_list = [subject_a, subject_b]
 subjects_dataset = torchio.ImagesDataset(subjects_list)
 subject_sample = subjects_dataset[0]
 ```
 
@@ -154,14 +155,22 @@
 
 ### Transforms
 
 The transforms package should remind users of
 [`torchvision.transforms`](https://pytorch.org/docs/stable/torchvision/transforms.html).
 They take as input the samples generated by an [`ImagesDataset`](#dataset).
 
+A transform can be quickly applied to an image file using the command-line
+tool `torchio-transform`:
+
+```shell
+$ torchio-transform input.nii.gz RandomMotion output.nii.gz --kwargs
+"proportion_to_augment=1,num_transforms=4"
+```
+
 #### Intensity
 
 ##### [MRI k-space motion artifacts](torchio/transforms/random_motion.py)
 
 Magnetic resonance images suffer from motion artifacts when the subject moves
 during image acquisition. This transform follows
 [Shaw et al., 2019](http://proceedings.mlr.press/v102/shaw19a.html) to
```

### Comparing `torchio-0.8.3/docs/Makefile` & `torchio-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/docs/conf.py` & `torchio-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/docs/installation.rst` & `torchio-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/docs/make.bat` & `torchio-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/setup.py` & `torchio-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,25 +42,25 @@
     ],
     description=(
         "Tools for loading, augmenting and writing 3D medical images"
         " on PyTorch."
     ),
     entry_points={
         'console_scripts': [
-            'torchio=torchio.cli:main',
+            'torchio-transform=torchio.cli:apply_transform',
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='torchio',
     name='torchio',
     packages=find_packages(include=['torchio', 'torchio.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/fepegar/torchio',
-    version='0.8.3',
+    version='0.9.0',
     zip_safe=False,
 )
```

### Comparing `torchio-0.8.3/tests/test_images_dataset.py` & `torchio-0.9.0/tests/test_images_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from pathlib import Path
 import numpy as np
 import nibabel as nib
 import torchio
 from torchio import INTENSITY, LABEL, Image
 
 
-class TestRandomElasticDeformation(unittest.TestCase):
-    """Tests for `RandomElasticDeformation`."""
+class TestImagesDataset(unittest.TestCase):
+    """Tests for `ImagesDataset`."""
 
     def setUp(self):
         """Set up test fixtures, if any."""
         self.dir = Path(tempfile.gettempdir()) / '.torchio_tests'
         self.dir.mkdir(exist_ok=True)
         random.seed(42)
         np.random.seed(42)
@@ -57,51 +57,68 @@
         nib.Nifti1Image(data, affine).to_filename(str(path))
         path = str(path) if np.random.rand() > 0.5 else path
         return path
 
     def test_images(self):
         self.iterate_dataset(self.subjects_list)
 
-    def test_wrong_subjects_list(self):
+    def test_empty_subjects_list(self):
         with self.assertRaises(ValueError):
             self.iterate_dataset([])
+
+    def test_empty_subjects_tuple(self):
         with self.assertRaises(ValueError):
             self.iterate_dataset(())
+
+    def test_wrong_subjects_type(self):
         with self.assertRaises(TypeError):
             self.iterate_dataset(0)
+
+    def test_wrong_subject_type_int(self):
         with self.assertRaises(TypeError):
             self.iterate_dataset([0])
+
+    def test_wrong_subject_type_dict(self):
         with self.assertRaises(TypeError):
             self.iterate_dataset([{}])
+
+    def test_image_not_found(self):
         with self.assertRaises(FileNotFoundError):
             self.iterate_dataset([[Image('t1', 'nopath', INTENSITY)]])
+
+    def test_wrong_path_type(self):
         with self.assertRaises(TypeError):
             self.iterate_dataset([[Image('t1', 5, INTENSITY)]])
+
+    def test_duplicate_image_name(self):
         with self.assertRaises(KeyError):
             with tempfile.NamedTemporaryFile() as f:
                 images = [
                     Image('t1', f.name, INTENSITY),
                     Image('t1', f.name, INTENSITY),
                 ]
             self.iterate_dataset([images])
+
+    def test_wrong_image_extension(self):
         with self.assertRaises(ValueError):
             path = self.dir / 'test.txt'
             path.touch()
             self.iterate_dataset([[Image('t1', path, INTENSITY)]])
 
-    def test_others(self):
+    def test_coverage(self):
         dataset = torchio.ImagesDataset(
             self.subjects_list, verbose=True, transform=lambda x: x)
         _ = len(dataset)  # for coverage
         sample = dataset[0]
         output_path = self.dir / 'test.nii.gz'
         paths_dict = {'t1': output_path}
         dataset.save_sample(sample, paths_dict)
         nii = nib.load(str(output_path))
         ndims_output = len(nii.shape)
         ndims_sample = len(sample['t1']['data'].shape)
         assert ndims_sample == ndims_output + 1
 
-    def iterate_dataset(self, subjects_list):
+    @staticmethod
+    def iterate_dataset(subjects_list):
         dataset = torchio.ImagesDataset(subjects_list)
         for _ in dataset:
             pass
```

### Comparing `torchio-0.8.3/tests/test_random_elastic_deformation.py` & `torchio-0.9.0/tests/test_random_elastic_deformation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 #!/usr/bin/env python
 
-"""Tests for `torchio` package."""
-
-
 import unittest
 import numpy as np
-from numpy.testing import assert_raises, assert_array_equal
 import torchio
 from torchio import INTENSITY, LABEL
 
 
 class TestRandomElasticDeformation(unittest.TestCase):
     """Tests for `RandomElasticDeformation`."""
```

### Comparing `torchio-0.8.3/tests/test_transforms.py` & `torchio-0.9.0/tests/test_transforms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 #!/usr/bin/env python
 
-"""Tests for `torchio` package."""
-
-
 import unittest
 import torch
 import numpy as np
 from torchio import INTENSITY, LABEL
 
 from torchio.transforms import (
     RandomFlip,
```

### Comparing `torchio-0.8.3/torchio/dataset/images.py` & `torchio-0.9.0/torchio/dataset/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
         self.path = self.parse_path(path)
         self.type = type_
 
     def parse_path(self, path):
         try:
             path = Path(path).expanduser()
         except TypeError:
-            print(f'Conversion to path not possible for variable: {path}')
-            raise
+            message = f'Conversion to path not possible for variable: {path}'
+            raise TypeError(message)
         if not path.is_file():
             message = (
                 f'File for image "{self.name}"'
                 f' not found: "{path}"'
                 )
             raise FileNotFoundError(message)
         return path
```

### Comparing `torchio-0.8.3/torchio/inference/aggregator.py` & `torchio-0.9.0/torchio/inference/aggregator.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/inference/grid_sampler.py` & `torchio-0.9.0/torchio/inference/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/io.py` & `torchio-0.9.0/torchio/io.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/queue.py` & `torchio-0.9.0/torchio/queue.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/sampler/label.py` & `torchio-0.9.0/torchio/sampler/label.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/sampler/sampler.py` & `torchio-0.9.0/torchio/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/transforms/histogram_standardization.py` & `torchio-0.9.0/torchio/transforms/normalization/histogram_standardization.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,34 @@
 
 from pathlib import Path
 import torch
 import numpy as np
 import numpy.ma as ma
 import nibabel as nib
 from tqdm import tqdm
-from .transform import Transform
-from ..utils import is_image_dict
-from ..torchio import INTENSITY
+from .normalization_transform import NormalizationTransform
 
-DEFAULT_CUTOFF = (0.01, 0.99)
+DEFAULT_CUTOFF = 0.01, 0.99
+STANDARD_RANGE = 0, 100
 
 
-class HistogramStandardization(Transform):
-    def __init__(self, landmarks_dict, verbose=False):
-        super().__init__(verbose=verbose)
+class HistogramStandardization(NormalizationTransform):
+    def __init__(self, landmarks_dict, masking_method=None, verbose=False):
+        super().__init__(masking_method=masking_method, verbose=verbose)
         self.landmarks_dict = landmarks_dict
 
-    def apply_transform(self, sample):
-        for image_name, image_dict in sample.items():
-            if not is_image_dict(image_dict):
-                continue
-            if image_dict['type'] == INTENSITY:
-                # TODO: assert that image_name is in dict
-                landmarks = self.landmarks_dict[image_name]
-                image_dict['data'] = normalize(image_dict['data'], landmarks)
-        return sample
-
+    def apply_normalization(self, sample, image_name, mask):
+        # TODO: assert that image_name is in landmarks dict
+        image_dict = sample[image_name]
+        landmarks = self.landmarks_dict[image_name]
+        image_dict['data'] = normalize(
+            image_dict['data'],
+            landmarks,
+            mask=mask,
+        )
 
 def __compute_percentiles(img, mask, cutoff):
     """
     Creates the list of percentile values to be used as landmarks for the
     linear fitting.
 
     :param img: Image on which to determine the percentiles
@@ -77,18 +75,14 @@
         cutoff[1] = np.max([cutoff[1], 0.76])
     else:
         cutoff[0] = np.min([cutoff[0], 0.09])
         cutoff[1] = np.max([cutoff[1], 0.91])
     return cutoff
 
 
-def create_standard_range():
-    return 0., 100.
-
-
 def __averaged_mapping(perc_database, s1, s2):
     """
     Map the landmarks of the database to the chosen range
     :param perc_database: perc_database over which to perform the averaging
     :param s1, s2: limits of the mapping range
     :return final_map: the average mapping
     """
@@ -101,29 +95,27 @@
     final_map = final_map + intercept
     return final_map
 
 
 def normalize(
         data,
         landmarks,
+        mask=None,
         cutoff=DEFAULT_CUTOFF,
-        masking_function=None,
         epsilon=1e-5,
         ):
     data = data.numpy()
     mapping = landmarks
 
     img = data
     image_shape = img.shape
     img = img.reshape(-1).astype(np.float32)
 
-    if masking_function is not None:
-        mask = masking_function(img)
-    else:
-        mask = np.ones_like(img, dtype=np.bool)
+    if mask is None:
+        mask = np.ones_like(img, np.bool)
     mask = mask.reshape(-1)
 
     range_to_use = [0, 1, 2, 4, 5, 6, 7, 8, 10, 11, 12]
 
     cutoff = __standardize_cutoff(cutoff)
     perc = __compute_percentiles(img, mask, cutoff)
 
@@ -177,15 +169,15 @@
                 mask = nib.load(mask_path[index]).get_fdata()
                 mask = mask > 0
             else:
                 mask = np.ones_like(data, dtype=np.bool)
         percentiles = __compute_percentiles(data, mask, cutoff)
         percentiles_database.append(percentiles)
     percentiles_database = np.vstack(percentiles_database)
-    s1, s2 = create_standard_range()
+    s1, s2 = STANDARD_RANGE
     mapping = __averaged_mapping(percentiles_database, s1, s2)
 
     if output_path is not None:
         output_path = Path(output_path).expanduser()
         extension = output_path.suffix
         if extension == '.txt':
             modality = 'image'
```

### Comparing `torchio-0.8.3/torchio/transforms/random_affine.py` & `torchio-0.9.0/torchio/transforms/augmentation/spatial/random_affine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import numpy as np
 import SimpleITK as sitk
-from ..torchio import LABEL
-from ..utils import is_image_dict
-from .interpolation import Interpolation
-from .random_transform import RandomTransform
+from ....torchio import LABEL
+from ....utils import is_image_dict
+from .. import Interpolation
+from .. import RandomTransform
 
 
 class RandomAffine(RandomTransform):
     def __init__(
             self,
             scales=(0.9, 1.1),
             degrees=10,
```

### Comparing `torchio-0.8.3/torchio/transforms/random_bias_field.py` & `torchio-0.9.0/torchio/transforms/augmentation/intensity/random_bias_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Adapted from NiftyNet
 """
 
 import numpy as np
 import torch
-from ..torchio import INTENSITY
-from ..utils import is_image_dict
-from .random_transform import RandomTransform
+from ....torchio import INTENSITY
+from ....utils import is_image_dict
+from .. import RandomTransform
 
 
 class RandomBiasField(RandomTransform):
     def __init__(
             self,
             coefficients_range=(-0.5, 0.5),
             order=3,
```

### Comparing `torchio-0.8.3/torchio/transforms/random_elastic_deformation.py` & `torchio-0.9.0/torchio/transforms/augmentation/spatial/random_elastic_deformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import SimpleITK as sitk
-from ..torchio import LABEL
-from ..utils import is_image_dict
-from .interpolation import Interpolation
-from .random_transform import RandomTransform
+from ....torchio import LABEL
+from ....utils import is_image_dict
+from .. import Interpolation
+from .. import RandomTransform
 
 
 class RandomElasticDeformation(RandomTransform):
     def __init__(
             self,
             num_control_points=4,
             deformation_std=15,
```

### Comparing `torchio-0.8.3/torchio/transforms/random_flip.py` & `torchio-0.9.0/torchio/transforms/augmentation/spatial/random_flip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import numpy as np
-from ..utils import is_image_dict
-from .random_transform import RandomTransform
+from ....utils import is_image_dict
+from .. import RandomTransform
 
 
 class RandomFlip(RandomTransform):
     def __init__(
             self,
             axes=(0,),
             flip_probability=0.5,
```

### Comparing `torchio-0.8.3/torchio/transforms/random_motion.py` & `torchio-0.9.0/torchio/transforms/augmentation/intensity/random_motion.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
     Shaw et al., 2019
     MRI k-Space Motion Artefact Augmentation:
     Model Robustness and Task-Specific Uncertainty
 
 """
 
+import warnings
 import torch
 import numpy as np
 from tqdm import tqdm
 import SimpleITK as sitk
 from scipy.linalg import logm, expm
-from ..torchio import INTENSITY
-from ..utils import is_image_dict
-from .interpolation import Interpolation
-from .random_transform import RandomTransform
+from ....torchio import INTENSITY
+from ....utils import is_image_dict
+from .. import Interpolation
+from .. import RandomTransform
 
 
 class RandomMotion(RandomTransform):
     def __init__(
             self,
             degrees=10,
             translation=10,  # in mm
@@ -55,14 +56,22 @@
                 'random_motion_translation',
                 'random_motion_do',
             )
             for key, p in zip(keys, params):
                 sample[image_name][key] = p
             if not do_it:
                 return sample
+            if (image_dict['data'][0] < 0).any():
+                message = (
+                    f'Image "{image_name}" has negative values.'
+                    ' Results can be unexpected because the transformed sample'
+                    ' is computed as the absolute values'
+                    ' of an inverse Fourier transform'
+                )
+                warnings.warn(message)
             image = self.nib_to_sitk(
                 image_dict['data'][0],
                 image_dict['affine'],
             )
             transforms = self.get_rigid_transforms(
                 degrees_params,
                 translation_params,
```

### Comparing `torchio-0.8.3/torchio/transforms/random_noise.py` & `torchio-0.9.0/torchio/transforms/augmentation/intensity/random_noise.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import torch
-from ..torchio import INTENSITY
-from ..utils import is_image_dict
-from .random_transform import RandomTransform
+from ....torchio import INTENSITY
+from ....utils import is_image_dict
+from .. import RandomTransform
 
 
 class RandomNoise(RandomTransform):
     def __init__(self, std_range=(0, 0.25), seed=None, verbose=False):
         super().__init__(seed=seed, verbose=verbose)
         self.std_range = std_range
```

### Comparing `torchio-0.8.3/torchio/transforms/random_transform.py` & `torchio-0.9.0/torchio/transforms/augmentation/random_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numbers
 from abc import abstractmethod
 
 import torch
 import SimpleITK as sitk
 
-from .transform import Transform
+from .. import Transform
 
 
 class RandomTransform(Transform):
     def __init__(self, seed=None, verbose=False):
         super().__init__(verbose=verbose)
         self.seed = seed
```

### Comparing `torchio-0.8.3/torchio/transforms/rescale.py` & `torchio-0.9.0/torchio/transforms/normalization/rescale.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import torch
 import numpy as np
-from ..torchio import INTENSITY
-from ..utils import is_image_dict
-from .transform import Transform
+from .normalization_transform import NormalizationTransform
 
 
-class Rescale(Transform):
+class Rescale(NormalizationTransform):
     def __init__(
             self,
             out_min_max=(-1, 1),
             percentiles=(1, 99),
+            masking_method=None,
             verbose=False,
             ):
-        super().__init__(verbose=verbose)
+        super().__init__(masking_method=masking_method, verbose=verbose)
         self.out_min, self.out_max = out_min_max
         self.percentiles = percentiles
 
-    def apply_transform(self, sample):
+    def apply_normalization(self, sample, image_name, mask):
         """
         This could probably be written in two or three lines
         """
-        for image_dict in sample.values():
-            if not is_image_dict(image_dict):
-                continue
-            if image_dict['type'] != INTENSITY:
-                continue
-            array = image_dict['data'].numpy()
-            pa, pb = self.percentiles
-            cutoff = np.percentile(array, (pa, pb))
-            np.clip(array, *cutoff, out=array)
-            array -= array.min()  # [0, max]
-            array /= array.max()  # [0, 1]
-            out_range = self.out_max - self.out_min
-            array *= out_range  # [0, out_range]
-            array -= self.out_min  # [out_min, out_max]
-            image_dict['data'] = torch.from_numpy(array)
-            return sample
+        image_dict = sample[image_name]
+        image_dict['data'] = self.rescale(image_dict['data'], mask)
+
+    def rescale(self, data, mask):
+        array = data.numpy()
+        mask = mask.numpy()
+        values = array[mask]
+        pa, pb = self.percentiles
+        cutoff = np.percentile(values, (pa, pb))
+        np.clip(array, *cutoff, out=array)
+        array -= array.min()  # [0, max]
+        array /= array.max()  # [0, 1]
+        out_range = self.out_max - self.out_min
+        array *= out_range  # [0, out_range]
+        array -= self.out_min  # [out_min, out_max]
+        return torch.from_numpy(array)
```

### Comparing `torchio-0.8.3/torchio/transforms/transform.py` & `torchio-0.9.0/torchio/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `torchio-0.8.3/torchio/utils.py` & `torchio-0.9.0/torchio/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,7 +88,22 @@
 
             subject_images = [
                 Image('one_modality', image_path, INTENSITY),
                 Image('segmentation', label_path, LABEL),
             ]
             subjects.append(subject_images)
     return subjects
+
+
+def apply_transform_to_file(
+        input_path,
+        transform,
+        output_path,
+        type_=INTENSITY,
+        ):
+    from . import Image, ImagesDataset
+    subject = [
+        Image('image', input_path, type_),
+    ]
+    dataset = ImagesDataset([subject], transform=transform)
+    transformed = dataset[0]
+    dataset.save_sample(transformed, dict(image=output_path))
```

### Comparing `torchio-0.8.3/torchio.egg-info/PKG-INFO` & `torchio-0.9.0/torchio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchio
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tools for loading, augmenting and writing 3D medical images on PyTorch.
 Home-page: https://github.com/fepegar/torchio
 Author: Fernando Perez-Garcia
 Author-email: fernando.perezgarcia.17@ucl.ac.uk
 License: MIT license
 Description: # TorchIO
         
@@ -76,19 +76,20 @@
         [`torchio.Image`](torchio/dataset/images.py) instances.
         The paths suffix must be `.nii`, `.nii.gz` or `.nrrd`.
         
         ```python
         import torchio
         
         subject_a = [
-            Image('t1', '~/Dropbox/MRI/t1.nii.gz', torchio.INTENSITY),
+            Image('t1', '~/Dropbox/MRI/t1.nrrd', torchio.INTENSITY),
             Image('label', '~/Dropbox/MRI/t1_seg.nii.gz', torchio.LABEL),
         ]
         subject_b = [
             Image('t1', '/tmp/colin27_t1_tal_lin.nii.gz', torchio.INTENSITY),
+            Image('t2', '/tmp/colin27_t2_tal_lin.nii', torchio.INTENSITY),
             Image('label', '/tmp/colin27_seg1.nii.gz', torchio.LABEL),
         ]
         subjects_list = [subject_a, subject_b]
         subjects_dataset = torchio.ImagesDataset(subjects_list)
         subject_sample = subjects_dataset[0]
         ```
         
@@ -162,14 +163,22 @@
         
         ### Transforms
         
         The transforms package should remind users of
         [`torchvision.transforms`](https://pytorch.org/docs/stable/torchvision/transforms.html).
         They take as input the samples generated by an [`ImagesDataset`](#dataset).
         
+        A transform can be quickly applied to an image file using the command-line
+        tool `torchio-transform`:
+        
+        ```shell
+        $ torchio-transform input.nii.gz RandomMotion output.nii.gz --kwargs
+        "proportion_to_augment=1,num_transforms=4"
+        ```
+        
         #### Intensity
         
         ##### [MRI k-space motion artifacts](torchio/transforms/random_motion.py)
         
         Magnetic resonance images suffer from motion artifacts when the subject moves
         during image acquisition. This transform follows
         [Shaw et al., 2019](http://proceedings.mlr.press/v102/shaw19a.html) to
```

