# Comparing `tmp/gradoptics-0.0.2.tar.gz` & `tmp/gradoptics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "gradoptics-0.0.3.tar", last modified: Mon Apr 17 21:40:14 2023, max compression
```

## Comparing `gradoptics-0.0.2.tar` & `gradoptics-0.0.3.tar`

### file list

```diff
@@ -1,92 +1,58 @@
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 gradoptics-0.0.2/.travis.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 gradoptics-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 gradoptics-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 gradoptics-0.0.2/requirements.txt
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 gradoptics-0.0.2/setup.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 gradoptics-0.0.2/.github/workflows/main.yml
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docker/Docker.ub18.04-cuda10.2-torch1.7-jax1.64
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docker/Docker.ub18.04-cuda10.2-torch1.8-jax1.64
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/Makefile
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/api.rst
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/citations.rst
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/conf.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/distributions.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.distributions.atom_cloud.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.distributions.base_distribution.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.distributions.gaussian_distribution.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.inference.rejection_sampling.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.integrator.base_integrator.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.integrator.stratified_sampling_integrator.rst
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.light_sources.base_light_source.rst
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.light_sources.light_source_from_distribution.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.base_optics.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.bounding_sphere.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.camera.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.lens.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.mirror.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.psf.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.ray.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.sensor.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.vector.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.optics.window.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.ray_tracing.ray_tracing.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.ray_tracing.scene.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.transforms.base_transform.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.transforms.look_at_transform.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/gradoptics.transforms.simple_transform.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/index.html
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/index.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/inference.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/integrator.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/light_sources.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/make.bat
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/optical_elements.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/ray_tracing.rst
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/requirements.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/transforms.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/tutorial.rst
--rw-r--r--   0        0        0   219053 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/tutorials/Beautiful-GIF.ipynb
--rw-r--r--   0        0        0   780962 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/tutorials/Custom-Optical-Element.ipynb
--rw-r--r--   0        0        0    85493 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/tutorials/Point-Spread-Functions.ipynb
--rw-r--r--   0        0        0   487713 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/tutorials/Quick-Start.ipynb
--rw-r--r--   0        0        0   319606 2020-02-02 00:00:00.000000 gradoptics-0.0.2/docs/tutorials/Scene.ipynb
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/distributions/__init__.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/distributions/atom_cloud.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/distributions/base_distribution.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/distributions/gaussian_distribution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/inference/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/inference/rejection_sampling.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/integrator/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/integrator/base_integrator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/integrator/stratified_sampling_integrator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/light_sources/__init__.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/light_sources/base_light_source.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/light_sources/light_source_from_distribution.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/base_optics.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/bounding_box.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/bounding_shape.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/bounding_sphere.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/camera.py
--rw-r--r--   0        0        0    16601 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/lens.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/mirror.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/psf.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/ray.py
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/sensor.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/vector.py
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/optics/window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/ray_tracing/__init__.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/ray_tracing/ray_tracing.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/ray_tracing/scene.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/transforms/__init__.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/transforms/base_transform.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/transforms/look_at_transform.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 gradoptics-0.0.2/src/gradoptics/transforms/simple_transform.py
--rw-r--r--   0        0        0    26254 2020-02-02 00:00:00.000000 gradoptics-0.0.2/tests/tests.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gradoptics-0.0.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 gradoptics-0.0.2/LICENSE
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 gradoptics-0.0.2/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 gradoptics-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 gradoptics-0.0.2/PKG-INFO
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.323735 gradoptics-0.0.3/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1087 2022-07-22 00:01:52.000000 gradoptics-0.0.3/LICENSE
+-rw-r--r--   0 sgaz     (1449223128) 1704612529       34 2022-07-22 00:01:52.000000 gradoptics-0.0.3/MANIFEST.in
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4733 2023-04-17 21:40:14.323141 gradoptics-0.0.3/PKG-INFO
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2738 2023-01-30 17:18:04.000000 gradoptics-0.0.3/README.md
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      751 2023-04-17 21:39:47.000000 gradoptics-0.0.3/pyproject.toml
+-rw-r--r--   0 sgaz     (1449223128) 1704612529       38 2023-04-17 21:40:14.323928 gradoptics-0.0.3/setup.cfg
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      760 2023-04-17 21:33:43.000000 gradoptics-0.0.3/setup.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.294388 gradoptics-0.0.3/src/
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.300853 gradoptics-0.0.3/src/gradoptics/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1409 2023-04-17 21:19:43.000000 gradoptics-0.0.3/src/gradoptics/__init__.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.306364 gradoptics-0.0.3/src/gradoptics/distributions/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/distributions/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6934 2023-04-17 21:19:43.000000 gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6265 2023-04-17 21:19:43.000000 gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud_donut.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      884 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/distributions/base_distribution.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      981 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/distributions/gaussian_distribution.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.307903 gradoptics-0.0.3/src/gradoptics/inference/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/inference/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1926 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/inference/rejection_sampling.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.310094 gradoptics-0.0.3/src/gradoptics/integrator/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      116 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/integrator/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      789 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/integrator/base_integrator.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1512 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/integrator/stratified_sampling_integrator.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.311863 gradoptics-0.0.3/src/gradoptics/light_sources/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/light_sources/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1196 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/light_sources/base_light_source.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2322 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/light_sources/light_source_from_distribution.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.318530 gradoptics-0.0.3/src/gradoptics/optics/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      359 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1547 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/base_optics.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4592 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/bounding_box.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      642 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/bounding_shape.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     3686 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/bounding_sphere.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1775 2023-01-30 17:18:04.000000 gradoptics-0.0.3/src/gradoptics/optics/camera.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    16601 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/optics/lens.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     9249 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/mirror.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1275 2023-01-30 17:18:04.000000 gradoptics-0.0.3/src/gradoptics/optics/psf.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6532 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/ray.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    10692 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/optics/sensor.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4168 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/vector.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     7566 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/optics/window.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.320016 gradoptics-0.0.3/src/gradoptics/ray_tracing/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/ray_tracing/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6222 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/ray_tracing/ray_tracing.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      828 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/ray_tracing/scene.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.321924 gradoptics-0.0.3/src/gradoptics/transforms/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/transforms/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     3964 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/transforms/base_transform.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2307 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/transforms/look_at_transform.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2453 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/transforms/simple_transform.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.303481 gradoptics-0.0.3/src/gradoptics.egg-info/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4733 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/PKG-INFO
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1595 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/SOURCES.txt
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        1 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/dependency_links.txt
+-rw-r--r--   0 sgaz     (1449223128) 1704612529       11 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/top_level.txt
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.322336 gradoptics-0.0.3/tests/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    26254 2023-04-17 21:19:15.000000 gradoptics-0.0.3/tests/tests.py
```

### Comparing `gradoptics-0.0.2/setup.py` & `gradoptics-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
   name='gradoptics',
-  version='0.0.2',
+  version='0.0.3',
   description='End-to-end differentiable optics',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Sean Gasiorowski, Michael Kagan, Maxime Vandegar',
   author_email='sgaz@slac.stanford.edu, makagan@slac.stanford.edu, maxime.vandegar@slac.stanford.edu',
   url="https://github.com/magis-slac/gradoptics",
   classifiers=[
```

### Comparing `gradoptics-0.0.2/src/gradoptics/__init__.py` & `gradoptics-0.0.3/src/gradoptics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from gradoptics.optics.vector import vector3d, batch_vector, normalize_batch_vector, normalize_vector, dot_product
 
 from gradoptics.distributions.gaussian_distribution import GaussianDistribution
 from gradoptics.distributions.base_distribution import BaseDistribution
 from gradoptics.distributions.atom_cloud import AtomCloud
+from gradoptics.distributions.atom_cloud_donut import AtomCloudDonut
 
 from gradoptics.inference.rejection_sampling import rejection_sampling
 
 from gradoptics.optics.lens import PerfectLens, ThickLens
 from gradoptics.optics.mirror import FlatMirror, CurvedMirror
 from gradoptics.optics.ray import Ray, Rays, empty_like, cat
 from gradoptics.optics.sensor import Sensor
```

### Comparing `gradoptics-0.0.2/src/gradoptics/distributions/atom_cloud.py` & `gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,44 +7,38 @@
 
 
 class AtomCloud(BaseDistribution):
     """
     Atom cloud with a sine-wave density modulation fringe pattern. Form and defaults from studies for MAGIS experiment.
     """
 
-    def __init__(self, n=int(1e6), f=2, position=[0.31, 0., 0.], w0=0.0005, h_bar=1.0546 * 1e-34, m=1.44 * 1e-25, x_a=0.,
-                 y_a=0., z_a=0., t_final_bs=3., t_extra=0.1, port_bvz=.15, k_fringe=1 / (0.00003*2), a_quad=1e-12, phi=0.1,
+    def __init__(self, n=int(1e6), f=2, position=[0.31, 0., 0.], w0=0.0005, h_bar=1.0546 * 1e-34, m=1.44 * 1e-25,
+                 t_final_bs=3., t_extra=0.1, port_bvz=.15, k_fringe=1 / (0.00003*2), a_quad=1e-12, phi=0.1,
                  phi2=math.pi / 2, proposal_distribution=GaussianDistribution(mean=0.0, std=0.0005)):
         """
         :param n: Number of atoms (:obj:`int`)
         :param position: Position of the center of the atom cloud [m] (:obj:`list`)
         :param phi: Phase of the sine-wave density modulation fringe pattern (:obj:`float`)
         :param w0: Beam width [m]. Roughly standard deviation of the atom cloud. (:obj:`float`)
         :param h_bar: Planck's constant, [kg * m^2 / s] (:obj:`float`)
         :param m: Strontium atom mass [kg] (:obj:`float`)
-        :param x_a: Atom cloud center, x [m] (:obj:`float`)
-        :param y_a: Atom cloud center, y [m] (:obj:`float`)
-        :param z_a: Atom cloud center, z [m] (:obj:`float`)
         :param t_final_bs: Time until final beam splitter [s] (:obj:`float`)
         :param k_fringe: Spatial frequency of fringe [1 / m] (:obj:`float`)
         :param a_quad: Magnitude of quadratic term (:obj:`float`)
         :param proposal_distribution: Proposal distribution used in rejection sampling for sampling from the
                                       unnormalized cloud distribution. Following units, mean, std in [m]
                                       (:py:class:`~gradoptics.distributions.base_distribution.BaseDistribution`)
         """
         super().__init__()
         self.n = n
         self.f = f
         self.position = torch.tensor(position)
         self.w0 = w0
         self.h_bar = h_bar
         self.m = m
-        self.xA = x_a
-        self.yA = y_a
-        self.zA = z_a
         self.tFinalBS = t_final_bs
         self.tExtra = t_extra
         self.portBvz = port_bvz
         self.kFringe = k_fringe
         self.aQuad = a_quad
         self.phi2 = phi2
         self.phi = phi
@@ -66,15 +60,15 @@
 
         :return: The marginal pdf function evaluated at ``x`` (:obj:`torch.tensor`)
         """
         x = x.clone().type(torch.float64)
 
         dnr = ((-1. * ((2. * self.m * self.w0 * self.w0) + (1j * self.tFinalBS * self.h_bar)) ** 1.) ** .5)
         nrc = 1j * ((2. / math.pi) ** (1. / 4.)) * ((self.m * self.w0) ** (1. / 2.))
-        psi1_x = nrc * torch.exp(-1 * self.m * ((x - self.xA) ** 2) / (
+        psi1_x = nrc * torch.exp(-1 * self.m * (x ** 2) / (
                 (4. * self.m * self.w0 * self.w0) + (2j * self.tFinalBS * self.h_bar))) / dnr
         density = torch.abs(psi1_x) ** 2
         return density
 
     def marginal_cloud_density_y(self, y):
         """
         Returns the marginal pdf function along the y axis, evaluated at ``y``
@@ -90,15 +84,15 @@
         y = y.clone().type(torch.float64)
 
         dnr = ((-1. * ((2. * self.m * self.w0 * self.w0) + (1j * self.tFinalBS * self.h_bar)) ** 1.) ** .5)
         nrc = 1j * ((2. / math.pi) ** (1. / 4.)) * ((self.m * self.w0) ** (1. / 2.))
         psi1 = nrc * ((1. / (2 ** .5)) + (torch.exp(
             (1j * self.phi) + (1j * ((self.kFringe * y) + (self.aQuad * self.kFringe * self.kFringe * y * y)))) / (
                                                   2 ** .5)))
-        psi1_y = psi1 * torch.exp(-1 * self.m * ((y - self.yA) ** 2) / (
+        psi1_y = psi1 * torch.exp(-1 * self.m * (y ** 2) / (
                 (4. * self.m * self.w0 * self.w0) + (2j * self.tFinalBS * self.h_bar))) / dnr
         density = torch.abs(psi1_y) ** 2
         return density
 
     def marginal_cloud_density_z(self, z):
         """
         Returns the marginal pdf function along the z axis, evaluated at ``z``
@@ -111,15 +105,15 @@
         :return: The marginal pdf function evaluated at ``z`` (:obj:`torch.tensor`)
         """
 
         z = z.clone().type(torch.float64)
 
         dnr = ((-1. * ((2. * self.m * self.w0 * self.w0) + (1j * self.tFinalBS * self.h_bar)) ** 1.) ** .5)
         nrc = 1j * ((2. / math.pi) ** (1. / 4.)) * ((self.m * self.w0) ** (1. / 2.))
-        psi1_z = nrc * torch.exp(-1 * self.m * ((z - self.zA) ** 2) / (
+        psi1_z = nrc * torch.exp(-1 * self.m * (z ** 2) / (
                 (4. * self.m * self.w0 * self.w0) + (2j * self.tFinalBS * self.h_bar))) / dnr
         density = torch.abs(psi1_z) ** 2
         return density
 
     def pdf(self, x):  # @Todo, refractor. x,y,z -> x
         """
         Returns the pdf function evaluated at ``x``
@@ -154,8 +148,8 @@
 
     def plot(self, ax, **kwargs):
         """
         Plots the center of the atom cloud on the provided axes.
 
         :param ax: 3d axes (:py:class:`mpl_toolkits.mplot3d.axes3d.Axes3D`)
         """
-        ax.scatter(self.position[0], self.position[1], self.position[2], **kwargs)
+        ax.scatter(self.position[0], self.position[1], self.position[2], **kwargs)
```

### Comparing `gradoptics-0.0.2/src/gradoptics/distributions/base_distribution.py` & `gradoptics-0.0.3/src/gradoptics/distributions/base_distribution.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/distributions/gaussian_distribution.py` & `gradoptics-0.0.3/src/gradoptics/distributions/gaussian_distribution.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/inference/rejection_sampling.py` & `gradoptics-0.0.3/src/gradoptics/inference/rejection_sampling.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/integrator/base_integrator.py` & `gradoptics-0.0.3/src/gradoptics/integrator/base_integrator.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/integrator/stratified_sampling_integrator.py` & `gradoptics-0.0.3/src/gradoptics/integrator/stratified_sampling_integrator.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/light_sources/base_light_source.py` & `gradoptics-0.0.3/src/gradoptics/light_sources/base_light_source.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/light_sources/light_source_from_distribution.py` & `gradoptics-0.0.3/src/gradoptics/light_sources/light_source_from_distribution.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/base_optics.py` & `gradoptics-0.0.3/src/gradoptics/optics/base_optics.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/bounding_box.py` & `gradoptics-0.0.3/src/gradoptics/optics/bounding_box.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/bounding_shape.py` & `gradoptics-0.0.3/src/gradoptics/optics/bounding_shape.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/bounding_sphere.py` & `gradoptics-0.0.3/src/gradoptics/optics/bounding_sphere.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/camera.py` & `gradoptics-0.0.3/src/gradoptics/optics/camera.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/lens.py` & `gradoptics-0.0.3/src/gradoptics/optics/lens.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/mirror.py` & `gradoptics-0.0.3/src/gradoptics/optics/mirror.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/psf.py` & `gradoptics-0.0.3/src/gradoptics/optics/psf.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/ray.py` & `gradoptics-0.0.3/src/gradoptics/optics/ray.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/sensor.py` & `gradoptics-0.0.3/src/gradoptics/optics/sensor.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/vector.py` & `gradoptics-0.0.3/src/gradoptics/optics/vector.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/optics/window.py` & `gradoptics-0.0.3/src/gradoptics/optics/window.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/ray_tracing/ray_tracing.py` & `gradoptics-0.0.3/src/gradoptics/ray_tracing/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/ray_tracing/scene.py` & `gradoptics-0.0.3/src/gradoptics/ray_tracing/scene.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/transforms/base_transform.py` & `gradoptics-0.0.3/src/gradoptics/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/transforms/look_at_transform.py` & `gradoptics-0.0.3/src/gradoptics/transforms/look_at_transform.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/src/gradoptics/transforms/simple_transform.py` & `gradoptics-0.0.3/src/gradoptics/transforms/simple_transform.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/tests/tests.py` & `gradoptics-0.0.3/tests/tests.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/LICENSE` & `gradoptics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/README.md` & `gradoptics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.2/pyproject.toml` & `gradoptics-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradoptics"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sean Gasiorowski", email="sgaz@slac.stanford.edu" },
   { name="Michael Kagan", email="makagan@slac.stanford.edu" },
   { name="Maxime Vandegar", email="maxime.vandegar@slac.stanford.edu" },
 ]
 description = "Differentiable Optics via Ray Tracing"
 readme = "README.md"
```

### Comparing `gradoptics-0.0.2/PKG-INFO` & `gradoptics-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gradoptics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Differentiable Optics via Ray Tracing
-Project-URL: Homepage, https://github.com/magis-slac/gradoptics
-Project-URL: Bug Tracker, https://github.com/pypa/magis-slac/gradoptics
+Home-page: https://github.com/magis-slac/gradoptics
+Author: Sean Gasiorowski, Michael Kagan, Maxime Vandegar
 Author-email: Sean Gasiorowski <sgaz@slac.stanford.edu>, Michael Kagan <makagan@slac.stanford.edu>, Maxime Vandegar <maxime.vandegar@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2021 Michael Kagan, Maxime Vandegar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,20 +22,23 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-License-File: LICENSE
+        
+Project-URL: Homepage, https://github.com/magis-slac/gradoptics
+Project-URL: Bug Tracker, https://github.com/pypa/magis-slac/gradoptics
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 [![Tests](https://github.com/magis-slac/gradoptics/actions/workflows/main.yml/badge.svg)](https://github.com/magis-slac/gradoptics/actions)
 [![Build Status](https://travis-ci.com/magis-slac/gradoptics.svg?token=LBAvFbnCy9PEgexzsTUS&branch=main)](https://travis-ci.com/magis-slac/gradoptics)
 [![Documentation Status](https://readthedocs.org/projects/gradoptics/badge/?version=latest)](https://gradoptics.readthedocs.io/en/latest/?badge=latest)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/magis-slac/gradoptics/blob/master/README.md)
 ![version](https://img.shields.io/badge/version-0.0.2-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

