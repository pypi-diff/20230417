# Comparing `tmp/sleplet-1.3.5.tar.gz` & `tmp/sleplet-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.3.5.tar", last modified: Thu Apr 13 11:12:32 2023, max compression
+gzip compressed data, was "sleplet-1.3.6.tar", last modified: Mon Apr 17 09:42:23 2023, max compression
```

## Comparing `sleplet-1.3.5.tar` & `sleplet-1.3.6.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.842863 sleplet-1.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.818863 sleplet-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.822863 sleplet-1.3.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.822863 sleplet-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/licence.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/paper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 11:12:18.000000 sleplet-1.3.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-13 11:12:18.000000 sleplet-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-13 11:12:18.000000 sleplet-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 11:12:18.000000 sleplet-1.3.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-13 11:12:18.000000 sleplet-1.3.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 11:12:18.000000 sleplet-1.3.5/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-13 11:12:32.842863 sleplet-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-13 11:12:18.000000 sleplet-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.822863 sleplet-1.3.5/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-13 11:12:18.000000 sleplet-1.3.5/documentation/DOCUMENTATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-13 11:12:18.000000 sleplet-1.3.5/documentation/config.mako
--rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-04-13 11:12:18.000000 sleplet-1.3.5/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-04-13 11:12:18.000000 sleplet-1.3.5/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.818863 sleplet-1.3.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.822863 sleplet-1.3.5/examples/arbitrary/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/_denoising_slepian_wavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/_slepian_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.822863 sleplet-1.3.5/examples/arbitrary/africa/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/denoising_slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/eigenvalues_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/slepian_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/tiling_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/africa/wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/eigenvalues_combined.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.826863 sleplet-1.3.5/examples/arbitrary/south_america/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/denoising_slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/eigenvalues_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/tiling_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.826863 sleplet-1.3.5/examples/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/mesh/denoising_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/mesh/mesh_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/mesh/mesh_slepian_eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/mesh/mesh_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/mesh/produce_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.826863 sleplet-1.3.5/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/misc/_denoising_axisym.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/misc/denoising_axisym_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/misc/denoising_axisym_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/misc/denoising_axisym_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/misc/translation_normalisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/misc/wavelet_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.826863 sleplet-1.3.5/examples/polar_cap/
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/eigenfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/fried_egg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/simons_5_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/simons_5_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/polar_cap/slepian_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.826863 sleplet-1.3.5/examples/wavelets/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/wavelets/axisymmetric_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-13 11:12:18.000000 sleplet-1.3.5/examples/wavelets/axisymmetric_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.826863 sleplet-1.3.5/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-13 11:12:18.000000 sleplet-1.3.5/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-13 11:12:18.000000 sleplet-1.3.5/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-13 11:12:18.000000 sleplet-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:12:32.842863 sleplet-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.818863 sleplet-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.830863 sleplet-1.3.5/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.834863 sleplet-1.3.5/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.834863 sleplet-1.3.5/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.838863 sleplet-1.3.5/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/directional_spin_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.838863 sleplet-1.3.5/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.838863 sleplet-1.3.5/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.838863 sleplet-1.3.5/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 11:12:18.000000 sleplet-1.3.5/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.830863 sleplet-1.3.5/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 11:12:32.000000 sleplet-1.3.5/src/sleplet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:12:32.842863 sleplet-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_arbitrary_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_loading_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-13 11:12:18.000000 sleplet-1.3.5/tests/test_wavelets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.874808 sleplet-1.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.834807 sleplet-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/licence.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/paper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 09:42:10.000000 sleplet-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 09:42:10.000000 sleplet-1.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 09:42:10.000000 sleplet-1.3.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-17 09:42:10.000000 sleplet-1.3.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 09:42:10.000000 sleplet-1.3.6/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-17 09:42:23.874808 sleplet-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-17 09:42:10.000000 sleplet-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/DOCUMENTATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/config.mako
+-rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.834807 sleplet-1.3.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/examples/arbitrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/_denoising_slepian_wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/_slepian_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/examples/arbitrary/africa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/denoising_slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/eigenvalues_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/slepian_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/tiling_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/eigenvalues_combined.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/arbitrary/south_america/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/eigenvalues_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/tiling_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/denoising_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/mesh_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/mesh_slepian_eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/mesh_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/produce_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/_denoising_axisym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/denoising_axisym_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/denoising_axisym_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/denoising_axisym_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/translation_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/wavelet_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/polar_cap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/eigenfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/fried_egg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/simons_5_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/simons_5_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/slepian_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/wavelets/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/wavelets/axisymmetric_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/wavelets/axisymmetric_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-17 09:42:10.000000 sleplet-1.3.6/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-17 09:42:10.000000 sleplet-1.3.6/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-17 09:42:10.000000 sleplet-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:42:23.874808 sleplet-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.834807 sleplet-1.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.846807 sleplet-1.3.6/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.850808 sleplet-1.3.6/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.854807 sleplet-1.3.6/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.862808 sleplet-1.3.6/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/directional_spin_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.866808 sleplet-1.3.6/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.866808 sleplet-1.3.6/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.870808 sleplet-1.3.6/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.846807 sleplet-1.3.6/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.874808 sleplet-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_arbitrary_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_loading_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_wavelets.py
```

### Comparing `sleplet-1.3.5/.github/ISSUE_TEMPLATE/bug_report.md` & `sleplet-1.3.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.github/ISSUE_TEMPLATE/feature_request.md` & `sleplet-1.3.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.github/workflows/deploy.yml` & `sleplet-1.3.6/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.github/workflows/documentation.yml` & `sleplet-1.3.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.github/workflows/examples.yml` & `sleplet-1.3.6/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.github/workflows/linting.yml` & `sleplet-1.3.6/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.github/workflows/test.yml` & `sleplet-1.3.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/.pre-commit-config.yaml` & `sleplet-1.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/CONTRIBUTING.md` & `sleplet-1.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/LICENCE.md` & `sleplet-1.3.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/PKG-INFO` & `sleplet-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.3.5
+Version: 1.3.6
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
```

### Comparing `sleplet-1.3.5/README.md` & `sleplet-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/documentation/DOCUMENTATION.md` & `sleplet-1.3.6/documentation/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/documentation/config.mako` & `sleplet-1.3.6/documentation/config.mako`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png` & `sleplet-1.3.6/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png` & `sleplet-1.3.6/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/_denoising_slepian_wavelet.py` & `sleplet-1.3.6/examples/arbitrary/_denoising_slepian_wavelet.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/_slepian_wavelet_covariance.py` & `sleplet-1.3.6/examples/arbitrary/_slepian_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/denoising_slepian_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/denoising_slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/eigenvalues_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/eigenvalues_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/slepian_reconstruction_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/slepian_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/tiling_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/tiling_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/africa/wavelet_reconstruction_africa.py` & `sleplet-1.3.6/examples/arbitrary/africa/wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/eigenvalues_combined.py` & `sleplet-1.3.6/examples/arbitrary/eigenvalues_combined.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/denoising_slepian_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/eigenvalues_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/eigenvalues_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/slepian_reconstruction_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/slepian_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/tiling_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/tiling_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py` & `sleplet-1.3.6/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/mesh/denoising_slepian_mesh.py` & `sleplet-1.3.6/examples/mesh/denoising_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/mesh/mesh_region.py` & `sleplet-1.3.6/examples/mesh/mesh_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/mesh/mesh_slepian_eigenvalues.py` & `sleplet-1.3.6/examples/mesh/mesh_slepian_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/mesh/mesh_tiling.py` & `sleplet-1.3.6/examples/mesh/mesh_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/misc/_denoising_axisym.py` & `sleplet-1.3.6/examples/misc/_denoising_axisym.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/misc/denoising_axisym_africa.py` & `sleplet-1.3.6/examples/misc/denoising_axisym_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/misc/denoising_axisym_earth.py` & `sleplet-1.3.6/examples/misc/denoising_axisym_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/misc/denoising_axisym_south_america.py` & `sleplet-1.3.6/examples/misc/denoising_axisym_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/misc/translation_normalisation.py` & `sleplet-1.3.6/examples/misc/translation_normalisation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/misc/wavelet_transform.py` & `sleplet-1.3.6/examples/misc/wavelet_transform.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/eigenfunctions.py` & `sleplet-1.3.6/examples/polar_cap/eigenfunctions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/eigenvalues.py` & `sleplet-1.3.6/examples/polar_cap/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/fried_egg.py` & `sleplet-1.3.6/examples/polar_cap/fried_egg.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/simons_5_1.py` & `sleplet-1.3.6/examples/polar_cap/simons_5_1.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/simons_5_3.py` & `sleplet-1.3.6/examples/polar_cap/simons_5_3.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/slepian_coefficients.py` & `sleplet-1.3.6/examples/polar_cap/slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/polar_cap/slepian_error.py` & `sleplet-1.3.6/examples/polar_cap/slepian_error.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/wavelets/axisymmetric_tiling.py` & `sleplet-1.3.6/examples/wavelets/axisymmetric_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/examples/wavelets/axisymmetric_wavelet_covariance.py` & `sleplet-1.3.6/examples/wavelets/axisymmetric_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/paper/paper.bib` & `sleplet-1.3.6/paper/paper.bib`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
   title     = {{Slepian Scale-Discretised Wavelets on Manifolds}},
   author    = {Roddy, Patrick J. and McEwen, Jason D.},
   year      = 2023,
   publisher = {arXiv},
   url       = {https://arxiv.org/abs/2302.06006}
 }
 @software{Roddy2023a,
-  title  = {{SLEPLET}},
+  title  = {{SLEPLET: Slepian Scale-Discretised Wavelets in Python}},
   author = {Roddy, Patrick J.},
   year   = 2023,
   doi    = {10.5281/zenodo.7268074}
 }
 @article{Simons2006,
   title   = {{Spatiospectral Concentration on a Sphere}},
   author  = {Simons, Frederik J. and Dahlen, F. A. and Wieczorek, Mark A.},
```

### Comparing `sleplet-1.3.5/paper/paper.md` & `sleplet-1.3.6/paper/paper.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/pyproject.toml` & `sleplet-1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/__init__.py` & `sleplet-1.3.6/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_bool_methods.py` & `sleplet-1.3.6/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_class_lists.py` & `sleplet-1.3.6/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_convolution_methods.py` & `sleplet-1.3.6/src/sleplet/_convolution_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.3.6/src/sleplet/_data/create_earth_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.3.6/src/sleplet/_data/create_wmap_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_data/setup_pooch.py` & `sleplet-1.3.6/src/sleplet/_data/setup_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_integration_methods.py` & `sleplet-1.3.6/src/sleplet/_integration_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_mask_methods.py` & `sleplet-1.3.6/src/sleplet/_mask_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_mesh_methods.py` & `sleplet-1.3.6/src/sleplet/_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_parallel_methods.py` & `sleplet-1.3.6/src/sleplet/_parallel_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_plotly_methods.py` & `sleplet-1.3.6/src/sleplet/_plotly_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.3.6/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.3.6/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.3.6/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_smoothing.py` & `sleplet-1.3.6/src/sleplet/_smoothing.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/_string_methods.py` & `sleplet-1.3.6/src/sleplet/_string_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/__init__.py` & `sleplet-1.3.6/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/africa.py` & `sleplet-1.3.6/src/sleplet/functions/africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/coefficients.py` & `sleplet-1.3.6/src/sleplet/functions/coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/dirac_delta.py` & `sleplet-1.3.6/src/sleplet/functions/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/directional_spin_wavelets.py` & `sleplet-1.3.6/src/sleplet/functions/directional_spin_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/earth.py` & `sleplet-1.3.6/src/sleplet/functions/earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.3.6/src/sleplet/functions/elongated_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/flm.py` & `sleplet-1.3.6/src/sleplet/functions/flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/fp.py` & `sleplet-1.3.6/src/sleplet/functions/fp.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/gaussian.py` & `sleplet-1.3.6/src/sleplet/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.3.6/src/sleplet/functions/harmonic_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/identity.py` & `sleplet-1.3.6/src/sleplet/functions/identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/noise_earth.py` & `sleplet-1.3.6/src/sleplet/functions/noise_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/ridgelets.py` & `sleplet-1.3.6/src/sleplet/functions/ridgelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian.py` & `sleplet-1.3.6/src/sleplet/functions/slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_africa.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_identity.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_noise_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.3.6/src/sleplet/functions/slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/south_america.py` & `sleplet-1.3.6/src/sleplet/functions/south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.3.6/src/sleplet/functions/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.3.6/src/sleplet/functions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/functions/wmap.py` & `sleplet-1.3.6/src/sleplet/functions/wmap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/harmonic_methods.py` & `sleplet-1.3.6/src/sleplet/harmonic_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/__init__.py` & `sleplet-1.3.6/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.3.6/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_field.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/noise.py` & `sleplet-1.3.6/src/sleplet/noise.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/plot_methods.py` & `sleplet-1.3.6/src/sleplet/plot_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.3.6/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.3.6/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.3.6/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian/region.py` & `sleplet-1.3.6/src/sleplet/slepian/region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.3.6/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.3.6/src/sleplet/slepian/slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.3.6/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.3.6/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/slepian_methods.py` & `sleplet-1.3.6/src/sleplet/slepian_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet/wavelet_methods.py` & `sleplet-1.3.6/src/sleplet/wavelet_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.3.6/src/sleplet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.3.5
+Version: 1.3.6
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
```

### Comparing `sleplet-1.3.5/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.3.6/src/sleplet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/conftest.py` & `sleplet-1.3.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_arbitrary_region.py` & `sleplet-1.3.6/tests/test_arbitrary_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_arrays.py` & `sleplet-1.3.6/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_bool.py` & `sleplet-1.3.6/tests/test_bool.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_convolution.py` & `sleplet-1.3.6/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_decomposition.py` & `sleplet-1.3.6/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_harmonic.py` & `sleplet-1.3.6/tests/test_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_loading_pooch.py` & `sleplet-1.3.6/tests/test_loading_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_mesh.py` & `sleplet-1.3.6/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_plot.py` & `sleplet-1.3.6/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_region.py` & `sleplet-1.3.6/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_slepian_mesh.py` & `sleplet-1.3.6/tests/test_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_strings.py` & `sleplet-1.3.6/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_translation.py` & `sleplet-1.3.6/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.5/tests/test_wavelets.py` & `sleplet-1.3.6/tests/test_wavelets.py`

 * *Files identical despite different names*

