# Comparing `tmp/salmon-triplets-1.0.2.tar.gz` & `tmp/salmon-triplets-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salmon-triplets-1.0.2.tar", last modified: Sun Apr 16 02:18:58 2023, max compression
+gzip compressed data, was "salmon-triplets-1.0.3.tar", last modified: Mon Apr 17 12:18:39 2023, max compression
```

## Comparing `salmon-triplets-1.0.2.tar` & `salmon-triplets-1.0.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.935703 salmon-triplets-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-16 02:18:58.935703 salmon-triplets-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.935703 salmon-triplets-1.0.2/salmon/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.927703 salmon-triplets-1.0.2/salmon/_out/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/_out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-16 02:18:58.935703 salmon-triplets-1.0.2/salmon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/backend/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/backend/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/frontend/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    34081 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/frontend/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/frontend/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/frontend/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/frontend/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/frontend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/triplets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/offline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/triplets/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20276 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/_adaptive_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/_round_robin.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/_test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/_noise_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/__triplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/gram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)    19737 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon/triplets/samplers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/tests/test_rr.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/samplers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/triplets/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/salmon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.931703 salmon-triplets-1.0.2/salmon_triplets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-16 02:18:58.000000 salmon-triplets-1.0.2/salmon_triplets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-16 02:18:58.000000 salmon-triplets-1.0.2/salmon_triplets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:18:58.000000 salmon-triplets-1.0.2/salmon_triplets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-16 02:18:58.000000 salmon-triplets-1.0.2/salmon_triplets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 02:18:58.000000 salmon-triplets-1.0.2/salmon_triplets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-16 02:18:58.935703 salmon-triplets-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:58.935703 salmon-triplets-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_active_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_allowabe_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13196 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_passive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-16 02:18:45.000000 salmon-triplets-1.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-17 12:18:21.000000 salmon-triplets-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 12:18:21.000000 salmon-triplets-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-17 12:18:21.000000 salmon-triplets-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.885406 salmon-triplets-1.0.3/salmon/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.877406 salmon-triplets-1.0.3/salmon/_out/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/_out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-17 12:18:39.885406 salmon-triplets-1.0.3/salmon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.877406 salmon-triplets-1.0.3/salmon/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/backend/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/backend/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.877406 salmon-triplets-1.0.3/salmon/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/frontend/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34081 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/frontend/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/frontend/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/frontend/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/frontend/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/frontend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/triplets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/offline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/triplets/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20276 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/_adaptive_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/_round_robin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/_test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/_noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/__triplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/gram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19737 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon/triplets/samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/tests/test_rr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/samplers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/triplets/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/salmon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/salmon_triplets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-17 12:18:39.000000 salmon-triplets-1.0.3/salmon_triplets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-17 12:18:39.000000 salmon-triplets-1.0.3/salmon_triplets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:18:39.000000 salmon-triplets-1.0.3/salmon_triplets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 12:18:39.000000 salmon-triplets-1.0.3/salmon_triplets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 12:18:39.000000 salmon-triplets-1.0.3/salmon_triplets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-17 12:18:39.885406 salmon-triplets-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:39.881406 salmon-triplets-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_active_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_allowabe_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13196 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_passive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-17 12:18:22.000000 salmon-triplets-1.0.3/versioneer.py
```

### Comparing `salmon-triplets-1.0.2/LICENSE.txt` & `salmon-triplets-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/PKG-INFO` & `salmon-triplets-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salmon-triplets
-Version: 1.0.2
+Version: 1.0.3
 Summary: Efficient crowdsourcing for ordinal embeddings
 Home-page: https://docs.stsievert.com/salmon
 Author: Scott Sievert
 Author-email: salmon@stsievert.com
 License: BSD 3-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `salmon-triplets-1.0.2/README.md` & `salmon-triplets-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/backend/core.py` & `salmon-triplets-1.0.3/salmon/backend/core.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/backend/sampler.py` & `salmon-triplets-1.0.3/salmon/backend/sampler.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/frontend/plotting.py` & `salmon-triplets-1.0.3/salmon/frontend/plotting.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/frontend/private.py` & `salmon-triplets-1.0.3/salmon/frontend/private.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/frontend/public.py` & `salmon-triplets-1.0.3/salmon/frontend/public.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/frontend/utils.py` & `salmon-triplets-1.0.3/salmon/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/manager.py` & `salmon-triplets-1.0.3/salmon/triplets/manager.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/offline.py` & `salmon-triplets-1.0.3/salmon/triplets/offline.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/_adaptive_runners.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/_adaptive_runners.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/_random_sampling.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/_random_sampling.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/_round_robin.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/_round_robin.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/_validation.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/_validation.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/_embed.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/_embed.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/_noise_models.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/_noise_models.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/_score.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/_score.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/__triplets.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/__triplets.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/_search.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/_search.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/gram_utils.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/gram_utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py` & `salmon-triplets-1.0.3/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/triplets/test_config.py` & `salmon-triplets-1.0.3/salmon/triplets/test_config.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon/utils.py` & `salmon-triplets-1.0.3/salmon/utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/salmon_triplets.egg-info/PKG-INFO` & `salmon-triplets-1.0.3/salmon_triplets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salmon-triplets
-Version: 1.0.2
+Version: 1.0.3
 Summary: Efficient crowdsourcing for ordinal embeddings
 Home-page: https://docs.stsievert.com/salmon
 Author: Scott Sievert
 Author-email: salmon@stsievert.com
 License: BSD 3-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `salmon-triplets-1.0.2/salmon_triplets.egg-info/SOURCES.txt` & `salmon-triplets-1.0.3/salmon_triplets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/setup.cfg` & `salmon-triplets-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_active.py` & `salmon-triplets-1.0.3/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_active_search.py` & `salmon-triplets-1.0.3/tests/test_active_search.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_allowabe_targets.py` & `salmon-triplets-1.0.3/tests/test_allowabe_targets.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_backend.py` & `salmon-triplets-1.0.3/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_basic.py` & `salmon-triplets-1.0.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_examples.py` & `salmon-triplets-1.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_offline.py` & `salmon-triplets-1.0.3/tests/test_offline.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_passive.py` & `salmon-triplets-1.0.3/tests/test_passive.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/test_validation.py` & `salmon-triplets-1.0.3/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/tests/utils.py` & `salmon-triplets-1.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.2/versioneer.py` & `salmon-triplets-1.0.3/versioneer.py`

 * *Files identical despite different names*

