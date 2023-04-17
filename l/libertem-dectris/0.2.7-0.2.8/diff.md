# Comparing `tmp/libertem_dectris-0.2.7.tar.gz` & `tmp/libertem_dectris-0.2.8.tar.gz`

## Comparing `libertem_dectris-0.2.7.tar` & `libertem_dectris-0.2.8.tar`

### file list

```diff
@@ -1,579 +1,579 @@
--rw-r--r--   0        0        0      214 1970-01-01 00:00:00.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/Cargo.toml
--rw-r--r--   0     1001      123     2716 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/build.rs
--rw-r--r--   0     1001      123     9165 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/src/lib.rs
--rw-r--r--   0     1001      123      249 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/dependabot.yml
--rw-r--r--   0     1001      123      219 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/flake8_cython.cfg
--rw-r--r--   0     1001      123       53 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/flake8_python.cfg
--rw-r--r--   0     1001      123      340 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/install_hdf5.sh
--rw-r--r--   0     1001      123      711 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/lint.yml
--rw-r--r--   0     1001      123     1387 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/main.yml
--rw-r--r--   0     1001      123     3272 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/wheels.yml
--rw-r--r--   0     1001      123      671 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.gitignore
--rw-r--r--   0     1001      123       72 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.gitmodules
--rw-r--r--   0     1001      123     1148 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/LICENSE
--rw-r--r--   0     1001      123      230 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/MANIFEST.in
--rw-r--r--   0     1001      123    10768 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/README.rst
--rw-r--r--   0     1001      123      908 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/__init__.py
--rw-r--r--   0     1001      123    19907 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/ext.pyx
--rw-r--r--   0     1001      123     7727 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/h5.pyx
--rw-r--r--   0     1001      123       75 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/bld.bat
--rw-r--r--   0     1001      123       94 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/build.sh
--rw-r--r--   0     1001      123      503 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/meta.yaml
--rw-r--r--   0     1001      123      503 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/setup.py.patch
--rw-r--r--   0     1001      123     1311 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/LICENSE
--rw-r--r--   0     1001      123     1522 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/README.md
--rw-r--r--   0     1001      123   105087 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.c
--rw-r--r--   0     1001      123    40861 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.h
--rw-r--r--   0     1001      123     1566 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/LICENSE.txt
--rw-r--r--   0     1001      123     2615 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/README.txt
--rw-r--r--   0     1001      123      205 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/README_bitshuffle.txt
--rw-r--r--   0     1001      123     2742 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/example.c
--rw-r--r--   0     1001      123     4413 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf.h
--rw-r--r--   0     1001      123     5448 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzfP.h
--rw-r--r--   0     1001      123     9007 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_c.c
--rw-r--r--   0     1001      123     4421 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_d.c
--rw-r--r--   0     1001      123     6928 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.c
--rw-r--r--   0     1001      123      874 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.h
--rw-r--r--   0     1001      123      223 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/pyproject.toml
--rw-r--r--   0     1001      123       70 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/requirements.txt
--rw-r--r--   0     1001      123      336 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/setup.cfg.example
--rw-r--r--   0     1001      123    14815 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/setup.py
--rw-r--r--   0     1001      123     8353 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.c
--rw-r--r--   0     1001      123     6052 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.h
--rw-r--r--   0     1001      123    65340 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.c
--rw-r--r--   0     1001      123     4533 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.h
--rw-r--r--   0     1001      123     2233 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_internals.h
--rw-r--r--   0     1001      123     8249 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.c
--rw-r--r--   0     1001      123     1612 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.h
--rw-r--r--   0     1001      123      486 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5plugin.c
--rw-r--r--   0     1001      123    10684 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/hdf5_dl.c
--rw-r--r--   0     1001      123     2483 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.c
--rw-r--r--   0     1001      123     2616 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.h
--rw-r--r--   0     1001      123      948 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/lzf_h5plugin.c
--rw-r--r--   0     1001      123   114447 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.1.3.h5
--rw-r--r--   0     1001      123   194482 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.4.0.h5
--rw-r--r--   0     1001      123     1894 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/make_regression_tdata.py
--rw-r--r--   0     1001      123    25795 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_ext.py
--rw-r--r--   0     1001      123     3536 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5filter.py
--rw-r--r--   0     1001      123     1714 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5plugin.py
--rw-r--r--   0     1001      123     1307 2023-03-22 14:09:19.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_regression.py
--rw-r--r--   0     1001      123      407 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.buckconfig
--rw-r--r--   0     1001      123       41 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.buckversion
--rw-r--r--   0     1001      123     4864 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.circleci/config.yml
--rw-r--r--   0     1001      123      348 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.circleci/images/primary/Dockerfile
--rw-r--r--   0     1001      123      334 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.cirrus.yml
--rw-r--r--   0     1001      123      348 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.gitattributes
--rw-r--r--   0     1001      123      805 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      595 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123     4489 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-long-tests.yml
--rw-r--r--   0     1001      123     5853 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-short-tests.yml
--rw-r--r--   0     1001      123     2510 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/publish-release-artifacts.yml
--rw-r--r--   0     1001      123      478 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.gitignore
--rw-r--r--   0     1001      123     4665 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.travis.yml
--rw-r--r--   0     1001      123    39607 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CHANGELOG
--rw-r--r--   0     1001      123      244 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123    29521 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CONTRIBUTING.md
--rw-r--r--   0     1001      123    18091 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/COPYING
--rw-r--r--   0     1001      123     1530 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/LICENSE
--rw-r--r--   0     1001      123    14291 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/Makefile
--rw-r--r--   0     1001      123     9743 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/README.md
--rw-r--r--   0     1001      123     1821 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/TESTING.md
--rw-r--r--   0     1001      123    12147 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/appveyor.yml
--rw-r--r--   0     1001      123      336 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/.gitignore
--rw-r--r--   0     1001      123        0 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/LICENSE
--rw-r--r--   0     1001      123     3142 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/README.md
--rw-r--r--   0     1001      123    11989 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fullbench/fullbench.vcproj
--rw-r--r--   0     1001      123    12933 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fuzzer/fuzzer.vcproj
--rw-r--r--   0     1001      123    14666 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd/zstd.vcproj
--rw-r--r--   0     1001      123     3509 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd.sln
--rw-r--r--   0     1001      123    14099 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstdlib/zstdlib.vcproj
--rw-r--r--   0     1001      123      244 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/CompileAsCpp.props
--rw-r--r--   0     1001      123     8700 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/datagen/datagen.vcxproj
--rw-r--r--   0     1001      123    12009 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench/fullbench.vcxproj
--rw-r--r--   0     1001      123    10513 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0     1001      123    12677 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fuzzer/fuzzer.vcxproj
--rw-r--r--   0     1001      123    13932 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd/libzstd.vcxproj
--rw-r--r--   0     1001      123     1473 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.rc
--rw-r--r--   0     1001      123    14335 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.vcxproj
--rw-r--r--   0     1001      123     1467 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.rc
--rw-r--r--   0     1001      123    14735 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.vcxproj
--rw-r--r--   0     1001      123     6009 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd.sln
--rw-r--r--   0     1001      123     2136 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/README.md
--rw-r--r--   0     1001      123      161 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2010.cmd
--rw-r--r--   0     1001      123      159 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2012.cmd
--rw-r--r--   0     1001      123      161 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2013.cmd
--rw-r--r--   0     1001      123      161 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2015.cmd
--rw-r--r--   0     1001      123      161 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017.cmd
--rw-r--r--   0     1001      123      179 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017Community.cmd
--rw-r--r--   0     1001      123      181 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017Enterprise.cmd
--rw-r--r--   0     1001      123      185 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017Professional.cmd
--rw-r--r--   0     1001      123     2605 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.generic.cmd
--rw-r--r--   0     1001      123      137 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/.gitignore
--rw-r--r--   0     1001      123     7740 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeLists.txt
--rw-r--r--   0     1001      123     3466 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/AddZstdCompilationFlags.cmake
--rw-r--r--   0     1001      123     2053 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/FindLibLZ4.cmake
--rw-r--r--   0     1001      123      449 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/GetZstdLibraryVersion.cmake
--rw-r--r--   0     1001      123     2294 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/README.md
--rw-r--r--   0     1001      123      510 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/CMakeLists.txt
--rw-r--r--   0     1001      123     1394 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/gen_html/CMakeLists.txt
--rw-r--r--   0     1001      123     1398 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/pzstd/CMakeLists.txt
--rw-r--r--   0     1001      123       34 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/.gitignore
--rw-r--r--   0     1001      123     6482 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/CMakeLists.txt
--rw-r--r--   0     1001      123      788 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/cmake_uninstall.cmake.in
--rw-r--r--   0     1001      123       51 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/programs/.gitignore
--rw-r--r--   0     1001      123     5642 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/programs/CMakeLists.txt
--rw-r--r--   0     1001      123       56 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/tests/.gitignore
--rw-r--r--   0     1001      123     5307 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/tests/CMakeLists.txt
--rw-r--r--   0     1001      123       55 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/zstdConfig.cmake
--rw-r--r--   0     1001      123     1303 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/GetZstdLibraryVersion.py
--rw-r--r--   0     1001      123     2120 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/InstallSymlink.py
--rw-r--r--   0     1001      123      967 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/README.md
--rw-r--r--   0     1001      123     1130 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/gen_html/meson.build
--rw-r--r--   0     1001      123      575 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/meson.build
--rw-r--r--   0     1001      123     1146 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/pzstd/meson.build
--rw-r--r--   0     1001      123     5059 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/lib/meson.build
--rw-r--r--   0     1001      123     4901 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson.build
--rw-r--r--   0     1001      123     1799 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson_options.txt
--rw-r--r--   0     1001      123     3828 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/programs/meson.build
--rw-r--r--   0     1001      123     7213 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/meson.build
--rw-r--r--   0     1001      123     3437 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/valgrindTest.py
--rw-r--r--   0     1001      123       83 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/.gitignore
--rw-r--r--   0     1001      123     2092 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/README.md
--rwxr-xr-x   0     1001      123     2052 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_decoder_test.sh
--rwxr-xr-x   0     1001      123     2252 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_library_test.sh
--rwxr-xr-x   0     1001      123     6323 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/combine.sh
--rwxr-xr-x   0     1001      123      325 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/create_single_file_decoder.sh
--rwxr-xr-x   0     1001      123      313 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/create_single_file_library.sh
--rw-r--r--   0     1001      123     1031 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/README.md
--rw-r--r--   0     1001      123     8751 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/emscripten.c
--rw-r--r--   0     1001      123     2520 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/roundtrip.c
--rw-r--r--   0     1001      123      982 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/shell.html
--rw-r--r--   0     1001      123     2309 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/simple.c
--rw-r--r--   0     1001      123   196606 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-dxt1.inl
--rw-r--r--   0     1001      123    18760 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-zstd.inl
--rwxr-xr-x   0     1001      123    12675 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard.png
--rw-r--r--   0     1001      123     2519 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstd-in.c
--rw-r--r--   0     1001      123     1720 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstddeclib-in.c
--rw-r--r--   0     1001      123      154 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/README.md
--rw-r--r--   0     1001      123     9471 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fullbench/fullbench.vcproj
--rw-r--r--   0     1001      123    10471 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fuzzer/fuzzer.vcproj
--rw-r--r--   0     1001      123    12058 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd/zstd.vcproj
--rw-r--r--   0     1001      123     3511 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd.sln
--rw-r--r--   0     1001      123    12119 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstdlib/zstdlib.vcproj
--rwxr-xr-x   0     1001      123      140 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/cleanTabs
--rw-r--r--   0     1001      123       19 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/.gitignore
--rw-r--r--   0     1001      123     1353 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/Makefile
--rw-r--r--   0     1001      123    10369 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/check_flipped_bits.c
--rw-r--r--   0     1001      123      517 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/docker/Dockerfile
--rw-r--r--   0     1001      123      368 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/docker/README.md
--rwxr-xr-x   0     1001      123    27728 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/freestanding_lib/freestanding.py
--rw-r--r--   0     1001      123       42 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/.gitignore
--rw-r--r--   0     1001      123     1611 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/Makefile
--rw-r--r--   0     1001      123     1120 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/README.md
--rwxr-xr-x   0     1001      123      531 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen-zstd-manual.sh
--rw-r--r--   0     1001      123     7581 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen_html.cpp
--rw-r--r--   0     1001      123       31 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/.gitignore
--rw-r--r--   0     1001      123     1624 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/Makefile
--rw-r--r--   0     1001      123      890 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/README.md
--rw-r--r--   0     1001      123    33620 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/largeNbDicts.c
--rw-r--r--   0     1001      123       30 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/.gitignore
--rw-r--r--   0     1001      123     3012 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/Makefile
--rw-r--r--   0     1001      123      874 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/README.md
--rwxr-xr-x   0     1001      123     2640 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-benchmark.sh
--rwxr-xr-x   0     1001      123     2926 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-extract-benchmark.sh
--rw-r--r--   0     1001      123      988 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/decompress_sources.h
--rw-r--r--   0     1001      123     1477 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux.mk
--rw-r--r--   0     1001      123    17510 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux_zstd.h
--rw-r--r--   0     1001      123     6436 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/mem.h
--rwxr-xr-x   0     1001      123     1339 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/squashfs-benchmark.sh
--rw-r--r--   0     1001      123     1605 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/Makefile
--rw-r--r--   0     1001      123     7270 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/asm/unaligned.h
--rw-r--r--   0     1001      123      569 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/compiler.h
--rw-r--r--   0     1001      123      443 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/errno.h
--rw-r--r--   0     1001      123      626 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/kernel.h
--rw-r--r--   0     1001      123      447 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/limits.h
--rw-r--r--   0     1001      123      487 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/math64.h
--rw-r--r--   0     1001      123      608 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/module.h
--rw-r--r--   0     1001      123      449 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/printk.h
--rw-r--r--   0     1001      123      447 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/stddef.h
--rw-r--r--   0     1001      123      505 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/swab.h
--rw-r--r--   0     1001      123      465 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/types.h
--rw-r--r--   0     1001      123    21388 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/xxhash.h
--rwxr-xr-x   0     1001      123     1060 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/macro-test.sh
--rw-r--r--   0     1001      123     1738 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/static_test.c
--rw-r--r--   0     1001      123     6422 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/test.c
--rw-r--r--   0     1001      123     3285 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_compress_module.c
--rw-r--r--   0     1001      123     2703 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_decompress_module.c
--rw-r--r--   0     1001      123     2838 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_deps.h
--rw-r--r--   0     1001      123     2232 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/README.md
--rw-r--r--   0     1001      123    20332 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.c
--rw-r--r--   0     1001      123     3279 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.h
--rw-r--r--   0     1001      123      196 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/premake/premake4.lua
--rw-r--r--   0     1001      123     1451 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/premake/zstd.lua
--rw-r--r--   0     1001      123       27 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/.gitignore
--rw-r--r--   0     1001      123     1579 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/BUCK
--rw-r--r--   0     1001      123     1215 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/ErrorHolder.h
--rw-r--r--   0     1001      123     1649 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Logging.h
--rw-r--r--   0     1001      123     7908 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Makefile
--rw-r--r--   0     1001      123    13795 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.cpp
--rw-r--r--   0     1001      123     2345 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.h
--rw-r--r--   0     1001      123    21110 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.cpp
--rw-r--r--   0     1001      123     5230 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.h
--rw-r--r--   0     1001      123     2921 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/README.md
--rw-r--r--   0     1001      123      962 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.cpp
--rw-r--r--   0     1001      123     1820 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.h
--rw-r--r--   0     1001      123    69804 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Cspeed.png
--rw-r--r--   0     1001      123    26335 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Dspeed.png
--rw-r--r--   0     1001      123      646 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/main.cpp
--rw-r--r--   0     1001      123      750 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/BUCK
--rw-r--r--   0     1001      123    15436 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/OptionsTest.cpp
--rw-r--r--   0     1001      123     4785 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/PzstdTest.cpp
--rw-r--r--   0     1001      123     2126 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTrip.h
--rw-r--r--   0     1001      123     2595 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTripTest.cpp
--rw-r--r--   0     1001      123     1428 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/BUCK
--rw-r--r--   0     1001      123     2625 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Buffer.h
--rw-r--r--   0     1001      123     2628 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/FileSystem.h
--rw-r--r--   0     1001      123      717 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Likely.h
--rw-r--r--   0     1001      123     3249 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Range.h
--rw-r--r--   0     1001      123     2642 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ResourcePool.h
--rw-r--r--   0     1001      123     1145 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ScopeGuard.h
--rw-r--r--   0     1001      123     1480 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ThreadPool.h
--rw-r--r--   0     1001      123     4502 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/WorkQueue.h
--rw-r--r--   0     1001      123      705 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BUCK
--rw-r--r--   0     1001      123     1950 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BufferTest.cpp
--rw-r--r--   0     1001      123     2033 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/RangeTest.cpp
--rw-r--r--   0     1001      123     1664 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ResourcePoolTest.cpp
--rw-r--r--   0     1001      123      657 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ScopeGuardTest.cpp
--rw-r--r--   0     1001      123     1705 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ThreadPoolTest.cpp
--rw-r--r--   0     1001      123     6083 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/WorkQueueTest.cpp
--rw-r--r--   0     1001      123     1300 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/Makefile
--rw-r--r--   0     1001      123     5043 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/recover_directory.c
--rw-r--r--   0     1001      123      112 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/.gitignore
--rw-r--r--   0     1001      123     1767 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/Makefile
--rw-r--r--   0     1001      123     6018 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_compression.c
--rw-r--r--   0     1001      123     5385 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_processing.c
--rw-r--r--   0     1001      123     4737 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_compression.c
--rw-r--r--   0     1001      123     3953 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression.c
--rw-r--r--   0     1001      123     4208 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression_mem.c
--rw-r--r--   0     1001      123       15 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/.gitignore
--rw-r--r--   0     1001      123     1140 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/Makefile
--rw-r--r--   0     1001      123     6367 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/seekable_tests.c
--rw-r--r--   0     1001      123    11556 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable.h
--rw-r--r--   0     1001      123     4848 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable_compression_format.md
--rw-r--r--   0     1001      123    10871 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_compress.c
--rw-r--r--   0     1001      123    18684 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_decompress.c
--rw-r--r--   0     1001      123      819 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/snap/snapcraft.yaml
--rw-r--r--   0     1001      123     1333 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/README.md
--rw-r--r--   0     1001      123       26 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/.gitignore
--rw-r--r--   0     1001      123     2180 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/Makefile
--rw-r--r--   0     1001      123     1727 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/README.md
--rw-r--r--   0     1001      123     3493 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/harness.c
--rw-r--r--   0     1001      123    90513 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.c
--rw-r--r--   0     1001      123     2558 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.h
--rw-r--r--   0     1001      123    73335 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/CSpeed2.png
--rw-r--r--   0     1001      123    69278 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DCspeed5.png
--rw-r--r--   0     1001      123    27123 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DSpeed3.png
--rw-r--r--   0     1001      123    33330 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/cdict_v136.png
--rw-r--r--   0     1001      123    90412 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cr.png
--rw-r--r--   0     1001      123    91518 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cs.png
--rw-r--r--   0     1001      123    98316 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-ds.png
--rw-r--r--   0     1001      123    93969 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_cdict_v1_3_5.png
--rw-r--r--   0     1001      123     5963 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_logo86.png
--rw-r--r--   0     1001      123    72157 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_compression_format.md
--rw-r--r--   0     1001      123   113443 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_manual.html
--rw-r--r--   0     1001      123      256 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/.gitignore
--rw-r--r--   0     1001      123     2825 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/Makefile
--rw-r--r--   0     1001      123     1891 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/README.md
--rw-r--r--   0     1001      123     7129 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/common.h
--rw-r--r--   0     1001      123     3230 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_compression.c
--rw-r--r--   0     1001      123     3743 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_decompression.c
--rw-r--r--   0     1001      123     3771 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_simple_compression.c
--rw-r--r--   0     1001      123     4446 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_streaming_compression.c
--rw-r--r--   0     1001      123     2049 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_compression.c
--rw-r--r--   0     1001      123     2302 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_decompression.c
--rw-r--r--   0     1001      123     4636 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression.c
--rw-r--r--   0     1001      123     6052 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression_thread_pool.c
--rw-r--r--   0     1001      123     3641 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_decompression.c
--rw-r--r--   0     1001      123     5828 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_memory_usage.c
--rw-r--r--   0     1001      123       48 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/.gitignore
--rw-r--r--   0     1001      123     4480 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/BUCK
--rw-r--r--   0     1001      123    15242 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/Makefile
--rw-r--r--   0     1001      123    10556 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/README.md
--rw-r--r--   0     1001      123    18187 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/bitstream.h
--rw-r--r--   0     1001      123    10147 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/compiler.h
--rw-r--r--   0     1001      123     4444 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/cpu.h
--rw-r--r--   0     1001      123      834 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.c
--rw-r--r--   0     1001      123     3752 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.h
--rw-r--r--   0     1001      123    13779 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/entropy_common.c
--rw-r--r--   0     1001      123     2998 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.c
--rw-r--r--   0     1001      123     2436 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.h
--rw-r--r--   0     1001      123    34604 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse.h
--rw-r--r--   0     1001      123    15052 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse_decompress.c
--rw-r--r--   0     1001      123    20383 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/huf.h
--rw-r--r--   0     1001      123    13694 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/mem.h
--rw-r--r--   0     1001      123    11294 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.c
--rw-r--r--   0     1001      123     2521 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.h
--rw-r--r--   0     1001      123     2941 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.c
--rw-r--r--   0     1001      123     5355 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.h
--rw-r--r--   0     1001      123    26728 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.c
--rw-r--r--   0     1001      123    11695 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.h
--rw-r--r--   0     1001      123     2717 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_common.c
--rw-r--r--   0     1001      123     2486 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_deps.h
--rw-r--r--   0     1001      123    16309 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_internal.h
--rw-r--r--   0     1001      123     4564 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_trace.h
--rw-r--r--   0     1001      123    26942 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/fse_compress.c
--rw-r--r--   0     1001      123     7439 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.c
--rw-r--r--   0     1001      123     3439 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.h
--rw-r--r--   0     1001      123    39478 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/huf_compress.c
--rw-r--r--   0     1001      123   284402 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress.c
--rw-r--r--   0     1001      123    56573 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_internal.h
--rw-r--r--   0     1001      123     6251 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.c
--rw-r--r--   0     1001      123     1210 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.h
--rw-r--r--   0     1001      123    19914 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.c
--rw-r--r--   0     1001      123     2166 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.h
--rw-r--r--   0     1001      123    28469 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.c
--rw-r--r--   0     1001      123     1159 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.h
--rw-r--r--   0     1001      123    24477 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_cwksp.h
--rw-r--r--   0     1001      123    25353 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.c
--rw-r--r--   0     1001      123     1279 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.h
--rw-r--r--   0     1001      123    22332 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.c
--rw-r--r--   0     1001      123     1199 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.h
--rw-r--r--   0     1001      123    96019 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.c
--rw-r--r--   0     1001      123     5647 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.h
--rw-r--r--   0     1001      123    28379 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.c
--rw-r--r--   0     1001      123     4449 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.h
--rw-r--r--   0     1001      123     5957 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm_geartab.h
--rw-r--r--   0     1001      123    62886 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.c
--rw-r--r--   0     1001      123     2002 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.h
--rw-r--r--   0     1001      123    78690 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.c
--rw-r--r--   0     1001      123     4430 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.h
--rw-r--r--   0     1001      123    55120 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/huf_decompress.c
--rw-r--r--   0     1001      123     9153 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.c
--rw-r--r--   0     1001      123     1310 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.h
--rw-r--r--   0     1001      123    91256 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress.c
--rw-r--r--   0     1001      123    66872 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.c
--rw-r--r--   0     1001      123     2242 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.h
--rw-r--r--   0     1001      123     8450 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_internal.h
--rw-r--r--   0     1001      123    11492 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff.h
--rw-r--r--   0     1001      123      999 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_common.c
--rw-r--r--   0     1001      123     5320 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_compress.c
--rw-r--r--   0     1001      123     1905 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_decompress.c
--rw-r--r--   0     1001      123    42474 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.c
--rw-r--r--   0     1001      123     5004 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.h
--rw-r--r--   0     1001      123    54649 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.c
--rw-r--r--   0     1001      123     2419 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.h
--rw-r--r--   0     1001      123    28242 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/fastcover.c
--rw-r--r--   0     1001      123    44423 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/zdict.c
--rw-r--r--   0     1001      123     1464 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/Makefile
--rw-r--r--   0     1001      123     2953 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/README.md
--rw-r--r--   0     1001      123      784 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/build_package.bat
--rw-r--r--   0     1001      123     1269 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.sln
--rw-r--r--   0     1001      123    10105 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.vcxproj
--rw-r--r--   0     1001      123    13898 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_legacy.h
--rw-r--r--   0     1001      123    71508 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.c
--rw-r--r--   0     1001      123     3793 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.h
--rw-r--r--   0     1001      123   128181 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.c
--rw-r--r--   0     1001      123     3702 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.h
--rw-r--r--   0     1001      123   114301 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.c
--rw-r--r--   0     1001      123     3714 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.h
--rw-r--r--   0     1001      123   135414 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.c
--rw-r--r--   0     1001      123     6432 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.h
--rw-r--r--   0     1001      123   156554 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.c
--rw-r--r--   0     1001      123     7530 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.h
--rw-r--r--   0     1001      123   166181 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.c
--rw-r--r--   0     1001      123     8068 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.h
--rw-r--r--   0     1001      123   185229 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.c
--rw-r--r--   0     1001      123     8711 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.h
--rw-r--r--   0     1001      123      417 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/libzstd.pc.in
--rw-r--r--   0     1001      123    25655 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zdict.h
--rw-r--r--   0     1001      123   145904 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd.h
--rw-r--r--   0     1001      123     3817 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd_errors.h
--rw-r--r--   0     1001      123      367 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/.gitignore
--rw-r--r--   0     1001      123      920 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/BUCK
--rw-r--r--   0     1001      123    17458 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/Makefile
--rw-r--r--   0     1001      123    17639 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/README.md
--rw-r--r--   0     1001      123     9826 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.c
--rw-r--r--   0     1001      123     8714 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.h
--rw-r--r--   0     1001      123    35448 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.c
--rw-r--r--   0     1001      123     8780 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.h
--rw-r--r--   0     1001      123     6182 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.c
--rw-r--r--   0     1001      123     1187 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.h
--rw-r--r--   0     1001      123    15321 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.c
--rw-r--r--   0     1001      123     1490 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.h
--rw-r--r--   0     1001      123   125138 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.c
--rw-r--r--   0     1001      123     7258 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.h
--rw-r--r--   0     1001      123     8836 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/platform.h
--rw-r--r--   0     1001      123     4964 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.c
--rw-r--r--   0     1001      123     2552 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.h
--rw-r--r--   0     1001      123    39814 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.c
--rw-r--r--   0     1001      123    10462 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.h
--rw-r--r--   0     1001      123      658 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/verrsrc.h
--rw-r--r--   0     1001      123     1467 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd.rc
--rw-r--r--   0     1001      123     1044 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd32.res
--rw-r--r--   0     1001      123     1044 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd64.res
--rw-r--r--   0     1001      123    28509 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1
--rw-r--r--   0     1001      123    26945 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1.md
--rw-r--r--   0     1001      123    66138 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli.c
--rw-r--r--   0     1001      123     4916 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.c
--rw-r--r--   0     1001      123      595 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.h
--rwxr-xr-x   0     1001      123     3869 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep
--rw-r--r--   0     1001      123      779 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1
--rw-r--r--   0     1001      123      726 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1.md
--rwxr-xr-x   0     1001      123       30 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdless
--rw-r--r--   0     1001      123      378 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdless.1
--rw-r--r--   0     1001      123      356 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdless.1.md
--rw-r--r--   0     1001      123      678 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/.gitignore
--rwxr-xr-x   0     1001      123    18201 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/DEPRECATED-test-zstd-speed.py
--rw-r--r--   0     1001      123    14839 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/Makefile
--rw-r--r--   0     1001      123     9619 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/README.md
--rw-r--r--   0     1001      123    13245 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/automated_benchmarking.py
--rw-r--r--   0     1001      123     4060 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/bigdict.c
--rw-r--r--   0     1001      123     1994 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/checkTag.c
--rw-r--r--   0     1001      123     4519 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/datagencli.c
--rw-r--r--   0     1001      123    69924 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/decodecorpus.c
--rw-r--r--   0     1001      123      153 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/dict-files/zero-weight-dict
--rw-r--r--   0     1001      123    34888 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fullbench.c
--rw-r--r--   0     1001      123      423 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/.gitignore
--rw-r--r--   0     1001      123     9701 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/Makefile
--rw-r--r--   0     1001      123     2993 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/README.md
--rw-r--r--   0     1001      123     1340 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_decompress.c
--rw-r--r--   0     1001      123     3153 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_round_trip.c
--rw-r--r--   0     1001      123     2198 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/decompress_dstSize_tooSmall.c
--rw-r--r--   0     1001      123     2480 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_decompress.c
--rw-r--r--   0     1001      123     3786 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_loader.c
--rw-r--r--   0     1001      123     5744 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_round_trip.c
--rw-r--r--   0     1001      123     7313 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_stream_round_trip.c
--rw-r--r--   0     1001      123     3478 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fse_read_ncount.c
--rw-r--r--   0     1001      123     1926 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.h
--rwxr-xr-x   0     1001      123    29048 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.py
--rw-r--r--   0     1001      123     2752 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.c
--rw-r--r--   0     1001      123     2664 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.h
--rw-r--r--   0     1001      123      761 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.c
--rw-r--r--   0     1001      123     2040 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.h
--rw-r--r--   0     1001      123     4144 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/raw_dictionary_round_trip.c
--rw-r--r--   0     1001      123     2683 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/regression_driver.c
--rw-r--r--   0     1001      123     3383 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/seekable_roundtrip.c
--rw-r--r--   0     1001      123    11823 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/sequence_compression_api.c
--rw-r--r--   0     1001      123     1791 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_compress.c
--rw-r--r--   0     1001      123     1422 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_decompress.c
--rw-r--r--   0     1001      123     5355 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_round_trip.c
--rw-r--r--   0     1001      123     3313 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_decompress.c
--rw-r--r--   0     1001      123     5962 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_round_trip.c
--rw-r--r--   0     1001      123     1354 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_frame_info.c
--rw-r--r--   0     1001      123     6131 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.c
--rw-r--r--   0     1001      123     1404 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.h
--rw-r--r--   0     1001      123   199849 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzzer.c
--rw-r--r--   0     1001      123     1189 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-compression/http
--rw-r--r--   0     1001      123      143 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-compression/huffman-compressed-larger
--rw-r--r--   0     1001      123       45 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-decompression/rle-first-block.zst
--rw-r--r--   0     1001      123     1000 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-dictionaries/http-dict-missing-symbols
--rw-r--r--   0     1001      123     1581 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/Makefile
--rwxr-xr-x   0     1001      123     1447 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/gzip-env.sh
--rw-r--r--   0     1001      123     1070 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/helin-segv.sh
--rw-r--r--   0     1001      123     8199 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/help-version.sh
--rw-r--r--   0     1001      123      425 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/hufts-segv.gz
--rw-r--r--   0     1001      123     1156 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/hufts.sh
--rw-r--r--   0     1001      123      178 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/init.cfg
--rw-r--r--   0     1001      123    19982 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/init.sh
--rw-r--r--   0     1001      123     1484 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/keep.sh
--rw-r--r--   0     1001      123     1032 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/list.sh
--rw-r--r--   0     1001      123     1211 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/memcpy-abuse.sh
--rw-r--r--   0     1001      123     2180 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/mixed.sh
--rw-r--r--   0     1001      123     1191 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/null-suffix-clobber.sh
--rw-r--r--   0     1001      123     1029 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/stdin.sh
--rw-r--r--   0     1001      123     4664 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/test-driver.sh
--rw-r--r--   0     1001      123     1245 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/trailing-nul.sh
--rw-r--r--   0     1001      123     1489 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/unpack-invalid.sh
--rw-r--r--   0     1001      123      995 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/z-suffix.sh
--rw-r--r--   0     1001      123     1257 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zdiff.sh
--rw-r--r--   0     1001      123     1455 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-context.sh
--rw-r--r--   0     1001      123     1362 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-f.sh
--rw-r--r--   0     1001      123     2163 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-signal.sh
--rw-r--r--   0     1001      123     1226 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/znew-k.sh
--rw-r--r--   0     1001      123     2092 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/invalidDictionaries.c
--rw-r--r--   0     1001      123    10852 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/legacy.c
--rwxr-xr-x   0     1001      123     3232 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/libzstd_partial_builds.sh
--rw-r--r--   0     1001      123     3094 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/longmatch.c
--rw-r--r--   0     1001      123   103954 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/paramgrill.c
--rwxr-xr-x   0     1001      123    61408 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/playTests.sh
--rw-r--r--   0     1001      123     6810 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/poolTests.c
--rwxr-xr-x   0     1001      123     1157 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/rateLimiter.py
--rw-r--r--   0     1001      123       44 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/.gitignore
--rw-r--r--   0     1001      123     1903 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/Makefile
--rw-r--r--   0     1001      123      895 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/README.md
--rw-r--r--   0     1001      123    19648 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.c
--rw-r--r--   0     1001      123     2459 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.h
--rw-r--r--   0     1001      123    16569 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.c
--rw-r--r--   0     1001      123     3047 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.h
--rw-r--r--   0     1001      123     1199 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/levels.h
--rw-r--r--   0     1001      123    21685 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.c
--rw-r--r--   0     1001      123     1772 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.h
--rw-r--r--   0     1001      123      934 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.c
--rw-r--r--   0     1001      123     2626 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.h
--rw-r--r--   0     1001      123   161474 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/results.csv
--rw-r--r--   0     1001      123    11030 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/test.c
--rw-r--r--   0     1001      123     7914 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/roundTripCrash.c
--rw-r--r--   0     1001      123     8022 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.c
--rw-r--r--   0     1001      123     1629 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.h
--rwxr-xr-x   0     1001      123     4344 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-license.py
--rwxr-xr-x   0     1001      123    10843 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-zstd-versions.py
--rw-r--r--   0     1001      123   126462 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/zstreamtest.c
--rw-r--r--   0     1001      123      256 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/.gitignore
--rw-r--r--   0     1001      123      433 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/BUCK
--rw-r--r--   0     1001      123     3920 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/Makefile
--rw-r--r--   0     1001      123     7889 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/README.md
--rw-r--r--   0     1001      123    18239 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example.c
--rw-r--r--   0     1001      123    17604 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example_original.c
--rw-r--r--   0     1001      123    10791 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk.c
--rw-r--r--   0     1001      123     8595 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk_original.c
--rw-r--r--   0     1001      123    15495 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/minigzip.c
--rw-r--r--   0     1001      123    46077 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/zwrapbench.c
--rw-r--r--   0     1001      123      849 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzclose.c
--rw-r--r--   0     1001      123     1873 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzcompatibility.h
--rw-r--r--   0     1001      123     7142 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzguts.h
--rw-r--r--   0     1001      123    17564 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzlib.c
--rw-r--r--   0     1001      123    22213 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzread.c
--rw-r--r--   0     1001      123    20440 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzwrite.c
--rw-r--r--   0     1001      123    42651 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.c
--rw-r--r--   0     1001      123     3648 2023-03-22 14:09:22.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.h
--rw-r--r--   0     1001      123       24 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/wrapper.h
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/Cargo.toml
--rw-r--r--   0     1001      123      247 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/README.md
--rw-r--r--   0     1001      123     2815 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/examples/consumer/main.rs
--rw-r--r--   0     1001      123     3772 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/examples/producer/main.rs
--rwxr-xr-x   0     1001      123      121 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/run-consumer.sh
--rwxr-xr-x   0     1001      123      121 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/run-producer.sh
--rw-r--r--   0     1001      123       31 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/rust-toolchain.toml
--rw-r--r--   0     1001      123     6872 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/src/backend_memfd.rs
--rw-r--r--   0     1001      123     2823 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/src/backend_shm.rs
--rw-r--r--   0     1001      123     3741 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/src/freestack.rs
--rw-r--r--   0     1001      123     1029 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/src/lib.rs
--rw-r--r--   0     1001      123    19891 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/ipc-test/src/slab.rs
--rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 libertem_dectris-0.2.7/local_dependencies/stats/Cargo.toml
--rw-r--r--   0     1001      123     2581 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/local_dependencies/stats/src/lib.rs
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 libertem_dectris-0.2.7/Cargo.toml
--rw-r--r--   0     1001      123     4626 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/README.md
--rw-r--r--   0     1001      123    13028 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/live_server.py
--rw-r--r--   0     1001      123     1408 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/passive.py
--rw-r--r--   0     1001      123     2123 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/passive_low_level.py
--rw-r--r--   0     1001      123     2191 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/simple.py
--rw-r--r--   0     1001      123     1353 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/testchunked.py
--rw-r--r--   0     1001      123     1507 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/testflame.py
--rw-r--r--   0     1001      123     1275 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/testrepeat.py
--rw-r--r--   0     1001      123     1179 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/testserialize.py
--rw-r--r--   0     1001      123     1192 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/testtooslow.py
--rw-r--r--   0     1001      123     1806 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/examples/testudf.py
--rw-r--r--   0     1001      123      449 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/pyproject.toml
--rw-r--r--   0     1001      123       31 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/rust-toolchain.toml
--rw-r--r--   0     1001      123    13277 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/cam_client.rs
--rw-r--r--   0     1001      123    10602 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/common.rs
--rw-r--r--   0     1001      123    11101 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/dectris_py.rs
--rw-r--r--   0     1001      123      413 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/exceptions.rs
--rw-r--r--   0     1001      123    12395 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/frame_stack.rs
--rw-r--r--   0     1001      123      143 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/lib.rs
--rw-r--r--   0     1001      123    10123 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/main.rs
--rw-r--r--   0     1001      123    21957 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/receiver.rs
--rw-r--r--   0     1001      123     9693 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/sim.rs
--rw-r--r--   0     1001      123      733 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/src/stats.rs
--rw-r--r--   0     1001      123    95572 2023-03-22 14:09:18.000000 libertem_dectris-0.2.7/Cargo.lock
--rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 libertem_dectris-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/Cargo.toml
+-rw-r--r--   0     1001      123      247 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/README.md
+-rw-r--r--   0     1001      123     2815 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/examples/consumer/main.rs
+-rw-r--r--   0     1001      123     3772 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/examples/producer/main.rs
+-rwxr-xr-x   0     1001      123      121 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/run-consumer.sh
+-rwxr-xr-x   0     1001      123      121 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/run-producer.sh
+-rw-r--r--   0     1001      123       31 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/rust-toolchain.toml
+-rw-r--r--   0     1001      123     6872 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/src/backend_memfd.rs
+-rw-r--r--   0     1001      123     2823 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/src/backend_shm.rs
+-rw-r--r--   0     1001      123     3741 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/src/freestack.rs
+-rw-r--r--   0     1001      123     1029 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/src/lib.rs
+-rw-r--r--   0     1001      123    19891 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/ipc-test/src/slab.rs
+-rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 libertem_dectris-0.2.8/local_dependencies/stats/Cargo.toml
+-rw-r--r--   0     1001      123     2581 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/stats/src/lib.rs
+-rw-r--r--   0        0        0      214 1970-01-01 00:00:00.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/Cargo.toml
+-rw-r--r--   0     1001      123     2716 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/build.rs
+-rw-r--r--   0     1001      123     9165 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/src/lib.rs
+-rw-r--r--   0     1001      123      249 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/dependabot.yml
+-rw-r--r--   0     1001      123      219 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/flake8_cython.cfg
+-rw-r--r--   0     1001      123       53 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/flake8_python.cfg
+-rw-r--r--   0     1001      123      340 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/install_hdf5.sh
+-rw-r--r--   0     1001      123      711 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/lint.yml
+-rw-r--r--   0     1001      123     1387 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/main.yml
+-rw-r--r--   0     1001      123     3272 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/wheels.yml
+-rw-r--r--   0     1001      123      671 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.gitignore
+-rw-r--r--   0     1001      123       72 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.gitmodules
+-rw-r--r--   0     1001      123     1148 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/LICENSE
+-rw-r--r--   0     1001      123      230 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/MANIFEST.in
+-rw-r--r--   0     1001      123    10768 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/README.rst
+-rw-r--r--   0     1001      123      908 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/__init__.py
+-rw-r--r--   0     1001      123    19907 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/ext.pyx
+-rw-r--r--   0     1001      123     7727 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/h5.pyx
+-rw-r--r--   0     1001      123       75 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/bld.bat
+-rw-r--r--   0     1001      123       94 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/build.sh
+-rw-r--r--   0     1001      123      503 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/meta.yaml
+-rw-r--r--   0     1001      123      503 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/conda-recipe/setup.py.patch
+-rw-r--r--   0     1001      123     1311 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/LICENSE
+-rw-r--r--   0     1001      123     1522 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/README.md
+-rw-r--r--   0     1001      123   105087 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.c
+-rw-r--r--   0     1001      123    40861 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.h
+-rw-r--r--   0     1001      123     1566 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/LICENSE.txt
+-rw-r--r--   0     1001      123     2615 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/README.txt
+-rw-r--r--   0     1001      123      205 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/README_bitshuffle.txt
+-rw-r--r--   0     1001      123     2742 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/example.c
+-rw-r--r--   0     1001      123     4413 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf.h
+-rw-r--r--   0     1001      123     5448 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzfP.h
+-rw-r--r--   0     1001      123     9007 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_c.c
+-rw-r--r--   0     1001      123     4421 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_d.c
+-rw-r--r--   0     1001      123     6928 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.c
+-rw-r--r--   0     1001      123      874 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.h
+-rw-r--r--   0     1001      123      223 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/pyproject.toml
+-rw-r--r--   0     1001      123       70 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/requirements.txt
+-rw-r--r--   0     1001      123      336 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/setup.cfg.example
+-rw-r--r--   0     1001      123    14815 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/setup.py
+-rw-r--r--   0     1001      123     8353 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.c
+-rw-r--r--   0     1001      123     6052 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.h
+-rw-r--r--   0     1001      123    65340 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.c
+-rw-r--r--   0     1001      123     4533 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.h
+-rw-r--r--   0     1001      123     2233 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_internals.h
+-rw-r--r--   0     1001      123     8249 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.c
+-rw-r--r--   0     1001      123     1612 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.h
+-rw-r--r--   0     1001      123      486 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5plugin.c
+-rw-r--r--   0     1001      123    10684 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/hdf5_dl.c
+-rw-r--r--   0     1001      123     2483 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.c
+-rw-r--r--   0     1001      123     2616 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.h
+-rw-r--r--   0     1001      123      948 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/lzf_h5plugin.c
+-rw-r--r--   0     1001      123   114447 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.1.3.h5
+-rw-r--r--   0     1001      123   194482 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.4.0.h5
+-rw-r--r--   0     1001      123     1894 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/make_regression_tdata.py
+-rw-r--r--   0     1001      123    25795 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_ext.py
+-rw-r--r--   0     1001      123     3536 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5filter.py
+-rw-r--r--   0     1001      123     1714 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5plugin.py
+-rw-r--r--   0     1001      123     1307 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_regression.py
+-rw-r--r--   0     1001      123      407 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.buckconfig
+-rw-r--r--   0     1001      123       41 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.buckversion
+-rw-r--r--   0     1001      123     4864 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.circleci/config.yml
+-rw-r--r--   0     1001      123      348 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.circleci/images/primary/Dockerfile
+-rw-r--r--   0     1001      123      334 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.cirrus.yml
+-rw-r--r--   0     1001      123      348 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.gitattributes
+-rw-r--r--   0     1001      123      805 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      595 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123     4489 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-long-tests.yml
+-rw-r--r--   0     1001      123     5853 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-short-tests.yml
+-rw-r--r--   0     1001      123     2510 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/publish-release-artifacts.yml
+-rw-r--r--   0     1001      123      478 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.gitignore
+-rw-r--r--   0     1001      123     4665 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.travis.yml
+-rw-r--r--   0     1001      123    39607 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CHANGELOG
+-rw-r--r--   0     1001      123      244 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123    29521 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CONTRIBUTING.md
+-rw-r--r--   0     1001      123    18091 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/COPYING
+-rw-r--r--   0     1001      123     1530 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/LICENSE
+-rw-r--r--   0     1001      123    14291 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/Makefile
+-rw-r--r--   0     1001      123     9743 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/README.md
+-rw-r--r--   0     1001      123     1821 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/TESTING.md
+-rw-r--r--   0     1001      123    12147 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/appveyor.yml
+-rw-r--r--   0     1001      123      336 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/.gitignore
+-rw-r--r--   0     1001      123        0 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/LICENSE
+-rw-r--r--   0     1001      123     3142 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/README.md
+-rw-r--r--   0     1001      123    11989 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fullbench/fullbench.vcproj
+-rw-r--r--   0     1001      123    12933 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fuzzer/fuzzer.vcproj
+-rw-r--r--   0     1001      123    14666 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd/zstd.vcproj
+-rw-r--r--   0     1001      123     3509 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd.sln
+-rw-r--r--   0     1001      123    14099 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstdlib/zstdlib.vcproj
+-rw-r--r--   0     1001      123      244 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/CompileAsCpp.props
+-rw-r--r--   0     1001      123     8700 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/datagen/datagen.vcxproj
+-rw-r--r--   0     1001      123    12009 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench/fullbench.vcxproj
+-rw-r--r--   0     1001      123    10513 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0     1001      123    12677 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0     1001      123    13932 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd/libzstd.vcxproj
+-rw-r--r--   0     1001      123     1473 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.rc
+-rw-r--r--   0     1001      123    14335 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.vcxproj
+-rw-r--r--   0     1001      123     1467 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.rc
+-rw-r--r--   0     1001      123    14735 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.vcxproj
+-rw-r--r--   0     1001      123     6009 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd.sln
+-rw-r--r--   0     1001      123     2136 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/README.md
+-rw-r--r--   0     1001      123      161 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2010.cmd
+-rw-r--r--   0     1001      123      159 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2012.cmd
+-rw-r--r--   0     1001      123      161 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2013.cmd
+-rw-r--r--   0     1001      123      161 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2015.cmd
+-rw-r--r--   0     1001      123      161 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017.cmd
+-rw-r--r--   0     1001      123      179 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017Community.cmd
+-rw-r--r--   0     1001      123      181 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017Enterprise.cmd
+-rw-r--r--   0     1001      123      185 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.VS2017Professional.cmd
+-rw-r--r--   0     1001      123     2605 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.generic.cmd
+-rw-r--r--   0     1001      123      137 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/.gitignore
+-rw-r--r--   0     1001      123     7740 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeLists.txt
+-rw-r--r--   0     1001      123     3466 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/AddZstdCompilationFlags.cmake
+-rw-r--r--   0     1001      123     2053 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/FindLibLZ4.cmake
+-rw-r--r--   0     1001      123      449 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/GetZstdLibraryVersion.cmake
+-rw-r--r--   0     1001      123     2294 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/README.md
+-rw-r--r--   0     1001      123      510 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/CMakeLists.txt
+-rw-r--r--   0     1001      123     1394 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/gen_html/CMakeLists.txt
+-rw-r--r--   0     1001      123     1398 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/pzstd/CMakeLists.txt
+-rw-r--r--   0     1001      123       34 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/.gitignore
+-rw-r--r--   0     1001      123     6482 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/CMakeLists.txt
+-rw-r--r--   0     1001      123      788 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/cmake_uninstall.cmake.in
+-rw-r--r--   0     1001      123       51 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/programs/.gitignore
+-rw-r--r--   0     1001      123     5642 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/programs/CMakeLists.txt
+-rw-r--r--   0     1001      123       56 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/tests/.gitignore
+-rw-r--r--   0     1001      123     5307 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/tests/CMakeLists.txt
+-rw-r--r--   0     1001      123       55 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/zstdConfig.cmake
+-rw-r--r--   0     1001      123     1303 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/GetZstdLibraryVersion.py
+-rw-r--r--   0     1001      123     2120 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/InstallSymlink.py
+-rw-r--r--   0     1001      123      967 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/README.md
+-rw-r--r--   0     1001      123     1130 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/gen_html/meson.build
+-rw-r--r--   0     1001      123      575 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/meson.build
+-rw-r--r--   0     1001      123     1146 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/pzstd/meson.build
+-rw-r--r--   0     1001      123     5059 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/lib/meson.build
+-rw-r--r--   0     1001      123     4901 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson.build
+-rw-r--r--   0     1001      123     1799 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson_options.txt
+-rw-r--r--   0     1001      123     3828 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/programs/meson.build
+-rw-r--r--   0     1001      123     7213 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/meson.build
+-rw-r--r--   0     1001      123     3437 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/valgrindTest.py
+-rw-r--r--   0     1001      123       83 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/.gitignore
+-rw-r--r--   0     1001      123     2092 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/README.md
+-rwxr-xr-x   0     1001      123     2052 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_decoder_test.sh
+-rwxr-xr-x   0     1001      123     2252 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_library_test.sh
+-rwxr-xr-x   0     1001      123     6323 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/combine.sh
+-rwxr-xr-x   0     1001      123      325 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/create_single_file_decoder.sh
+-rwxr-xr-x   0     1001      123      313 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/create_single_file_library.sh
+-rw-r--r--   0     1001      123     1031 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/README.md
+-rw-r--r--   0     1001      123     8751 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/emscripten.c
+-rw-r--r--   0     1001      123     2520 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/roundtrip.c
+-rw-r--r--   0     1001      123      982 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/shell.html
+-rw-r--r--   0     1001      123     2309 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/simple.c
+-rw-r--r--   0     1001      123   196606 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-dxt1.inl
+-rw-r--r--   0     1001      123    18760 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-zstd.inl
+-rwxr-xr-x   0     1001      123    12675 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard.png
+-rw-r--r--   0     1001      123     2519 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstd-in.c
+-rw-r--r--   0     1001      123     1720 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstddeclib-in.c
+-rw-r--r--   0     1001      123      154 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/README.md
+-rw-r--r--   0     1001      123     9471 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fullbench/fullbench.vcproj
+-rw-r--r--   0     1001      123    10471 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fuzzer/fuzzer.vcproj
+-rw-r--r--   0     1001      123    12058 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd/zstd.vcproj
+-rw-r--r--   0     1001      123     3511 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd.sln
+-rw-r--r--   0     1001      123    12119 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstdlib/zstdlib.vcproj
+-rwxr-xr-x   0     1001      123      140 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/cleanTabs
+-rw-r--r--   0     1001      123       19 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/.gitignore
+-rw-r--r--   0     1001      123     1353 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/Makefile
+-rw-r--r--   0     1001      123    10369 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/check_flipped_bits.c
+-rw-r--r--   0     1001      123      517 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/docker/Dockerfile
+-rw-r--r--   0     1001      123      368 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/docker/README.md
+-rwxr-xr-x   0     1001      123    27728 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/freestanding_lib/freestanding.py
+-rw-r--r--   0     1001      123       42 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/.gitignore
+-rw-r--r--   0     1001      123     1611 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/Makefile
+-rw-r--r--   0     1001      123     1120 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/README.md
+-rwxr-xr-x   0     1001      123      531 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen-zstd-manual.sh
+-rw-r--r--   0     1001      123     7581 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen_html.cpp
+-rw-r--r--   0     1001      123       31 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/.gitignore
+-rw-r--r--   0     1001      123     1624 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/Makefile
+-rw-r--r--   0     1001      123      890 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/README.md
+-rw-r--r--   0     1001      123    33620 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/largeNbDicts.c
+-rw-r--r--   0     1001      123       30 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/.gitignore
+-rw-r--r--   0     1001      123     3012 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/Makefile
+-rw-r--r--   0     1001      123      874 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/README.md
+-rwxr-xr-x   0     1001      123     2640 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-benchmark.sh
+-rwxr-xr-x   0     1001      123     2926 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-extract-benchmark.sh
+-rw-r--r--   0     1001      123      988 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/decompress_sources.h
+-rw-r--r--   0     1001      123     1477 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux.mk
+-rw-r--r--   0     1001      123    17510 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux_zstd.h
+-rw-r--r--   0     1001      123     6436 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/mem.h
+-rwxr-xr-x   0     1001      123     1339 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/squashfs-benchmark.sh
+-rw-r--r--   0     1001      123     1605 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/Makefile
+-rw-r--r--   0     1001      123     7270 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/asm/unaligned.h
+-rw-r--r--   0     1001      123      569 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/compiler.h
+-rw-r--r--   0     1001      123      443 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/errno.h
+-rw-r--r--   0     1001      123      626 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/kernel.h
+-rw-r--r--   0     1001      123      447 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/limits.h
+-rw-r--r--   0     1001      123      487 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/math64.h
+-rw-r--r--   0     1001      123      608 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/module.h
+-rw-r--r--   0     1001      123      449 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/printk.h
+-rw-r--r--   0     1001      123      447 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/stddef.h
+-rw-r--r--   0     1001      123      505 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/swab.h
+-rw-r--r--   0     1001      123      465 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/types.h
+-rw-r--r--   0     1001      123    21388 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/xxhash.h
+-rwxr-xr-x   0     1001      123     1060 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/macro-test.sh
+-rw-r--r--   0     1001      123     1738 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/static_test.c
+-rw-r--r--   0     1001      123     6422 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/test.c
+-rw-r--r--   0     1001      123     3285 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_compress_module.c
+-rw-r--r--   0     1001      123     2703 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_decompress_module.c
+-rw-r--r--   0     1001      123     2838 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_deps.h
+-rw-r--r--   0     1001      123     2232 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/README.md
+-rw-r--r--   0     1001      123    20332 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.c
+-rw-r--r--   0     1001      123     3279 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.h
+-rw-r--r--   0     1001      123      196 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/premake/premake4.lua
+-rw-r--r--   0     1001      123     1451 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/premake/zstd.lua
+-rw-r--r--   0     1001      123       27 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/.gitignore
+-rw-r--r--   0     1001      123     1579 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/BUCK
+-rw-r--r--   0     1001      123     1215 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/ErrorHolder.h
+-rw-r--r--   0     1001      123     1649 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Logging.h
+-rw-r--r--   0     1001      123     7908 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Makefile
+-rw-r--r--   0     1001      123    13795 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.cpp
+-rw-r--r--   0     1001      123     2345 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.h
+-rw-r--r--   0     1001      123    21110 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.cpp
+-rw-r--r--   0     1001      123     5230 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.h
+-rw-r--r--   0     1001      123     2921 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/README.md
+-rw-r--r--   0     1001      123      962 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.cpp
+-rw-r--r--   0     1001      123     1820 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.h
+-rw-r--r--   0     1001      123    69804 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Cspeed.png
+-rw-r--r--   0     1001      123    26335 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Dspeed.png
+-rw-r--r--   0     1001      123      646 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/main.cpp
+-rw-r--r--   0     1001      123      750 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/BUCK
+-rw-r--r--   0     1001      123    15436 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/OptionsTest.cpp
+-rw-r--r--   0     1001      123     4785 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/PzstdTest.cpp
+-rw-r--r--   0     1001      123     2126 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTrip.h
+-rw-r--r--   0     1001      123     2595 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTripTest.cpp
+-rw-r--r--   0     1001      123     1428 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/BUCK
+-rw-r--r--   0     1001      123     2625 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Buffer.h
+-rw-r--r--   0     1001      123     2628 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/FileSystem.h
+-rw-r--r--   0     1001      123      717 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Likely.h
+-rw-r--r--   0     1001      123     3249 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Range.h
+-rw-r--r--   0     1001      123     2642 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ResourcePool.h
+-rw-r--r--   0     1001      123     1145 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ScopeGuard.h
+-rw-r--r--   0     1001      123     1480 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ThreadPool.h
+-rw-r--r--   0     1001      123     4502 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/WorkQueue.h
+-rw-r--r--   0     1001      123      705 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BUCK
+-rw-r--r--   0     1001      123     1950 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BufferTest.cpp
+-rw-r--r--   0     1001      123     2033 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/RangeTest.cpp
+-rw-r--r--   0     1001      123     1664 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ResourcePoolTest.cpp
+-rw-r--r--   0     1001      123      657 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ScopeGuardTest.cpp
+-rw-r--r--   0     1001      123     1705 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ThreadPoolTest.cpp
+-rw-r--r--   0     1001      123     6083 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/WorkQueueTest.cpp
+-rw-r--r--   0     1001      123     1300 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/Makefile
+-rw-r--r--   0     1001      123     5043 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/recover_directory.c
+-rw-r--r--   0     1001      123      112 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/.gitignore
+-rw-r--r--   0     1001      123     1767 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/Makefile
+-rw-r--r--   0     1001      123     6018 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_compression.c
+-rw-r--r--   0     1001      123     5385 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_processing.c
+-rw-r--r--   0     1001      123     4737 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_compression.c
+-rw-r--r--   0     1001      123     3953 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression.c
+-rw-r--r--   0     1001      123     4208 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression_mem.c
+-rw-r--r--   0     1001      123       15 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/.gitignore
+-rw-r--r--   0     1001      123     1140 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/Makefile
+-rw-r--r--   0     1001      123     6367 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/seekable_tests.c
+-rw-r--r--   0     1001      123    11556 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable.h
+-rw-r--r--   0     1001      123     4848 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable_compression_format.md
+-rw-r--r--   0     1001      123    10871 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_compress.c
+-rw-r--r--   0     1001      123    18684 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_decompress.c
+-rw-r--r--   0     1001      123      819 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/snap/snapcraft.yaml
+-rw-r--r--   0     1001      123     1333 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/README.md
+-rw-r--r--   0     1001      123       26 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/.gitignore
+-rw-r--r--   0     1001      123     2180 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/Makefile
+-rw-r--r--   0     1001      123     1727 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/README.md
+-rw-r--r--   0     1001      123     3493 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/harness.c
+-rw-r--r--   0     1001      123    90513 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.c
+-rw-r--r--   0     1001      123     2558 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.h
+-rw-r--r--   0     1001      123    73335 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/CSpeed2.png
+-rw-r--r--   0     1001      123    69278 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DCspeed5.png
+-rw-r--r--   0     1001      123    27123 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DSpeed3.png
+-rw-r--r--   0     1001      123    33330 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/cdict_v136.png
+-rw-r--r--   0     1001      123    90412 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cr.png
+-rw-r--r--   0     1001      123    91518 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cs.png
+-rw-r--r--   0     1001      123    98316 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-ds.png
+-rw-r--r--   0     1001      123    93969 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_cdict_v1_3_5.png
+-rw-r--r--   0     1001      123     5963 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_logo86.png
+-rw-r--r--   0     1001      123    72157 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_compression_format.md
+-rw-r--r--   0     1001      123   113443 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_manual.html
+-rw-r--r--   0     1001      123      256 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/.gitignore
+-rw-r--r--   0     1001      123     2825 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/Makefile
+-rw-r--r--   0     1001      123     1891 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/README.md
+-rw-r--r--   0     1001      123     7129 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/common.h
+-rw-r--r--   0     1001      123     3230 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_compression.c
+-rw-r--r--   0     1001      123     3743 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_decompression.c
+-rw-r--r--   0     1001      123     3771 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_simple_compression.c
+-rw-r--r--   0     1001      123     4446 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_streaming_compression.c
+-rw-r--r--   0     1001      123     2049 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_compression.c
+-rw-r--r--   0     1001      123     2302 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_decompression.c
+-rw-r--r--   0     1001      123     4636 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression.c
+-rw-r--r--   0     1001      123     6052 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression_thread_pool.c
+-rw-r--r--   0     1001      123     3641 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_decompression.c
+-rw-r--r--   0     1001      123     5828 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_memory_usage.c
+-rw-r--r--   0     1001      123       48 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/.gitignore
+-rw-r--r--   0     1001      123     4480 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/BUCK
+-rw-r--r--   0     1001      123    15242 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/Makefile
+-rw-r--r--   0     1001      123    10556 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/README.md
+-rw-r--r--   0     1001      123    18187 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/bitstream.h
+-rw-r--r--   0     1001      123    10147 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/compiler.h
+-rw-r--r--   0     1001      123     4444 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/cpu.h
+-rw-r--r--   0     1001      123      834 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.c
+-rw-r--r--   0     1001      123     3752 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.h
+-rw-r--r--   0     1001      123    13779 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/entropy_common.c
+-rw-r--r--   0     1001      123     2998 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.c
+-rw-r--r--   0     1001      123     2436 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.h
+-rw-r--r--   0     1001      123    34604 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse.h
+-rw-r--r--   0     1001      123    15052 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse_decompress.c
+-rw-r--r--   0     1001      123    20383 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/huf.h
+-rw-r--r--   0     1001      123    13694 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/mem.h
+-rw-r--r--   0     1001      123    11294 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.c
+-rw-r--r--   0     1001      123     2521 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.h
+-rw-r--r--   0     1001      123     2941 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.c
+-rw-r--r--   0     1001      123     5355 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.h
+-rw-r--r--   0     1001      123    26728 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.c
+-rw-r--r--   0     1001      123    11695 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.h
+-rw-r--r--   0     1001      123     2717 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_common.c
+-rw-r--r--   0     1001      123     2486 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_deps.h
+-rw-r--r--   0     1001      123    16309 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_internal.h
+-rw-r--r--   0     1001      123     4564 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_trace.h
+-rw-r--r--   0     1001      123    26942 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/fse_compress.c
+-rw-r--r--   0     1001      123     7439 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.c
+-rw-r--r--   0     1001      123     3439 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.h
+-rw-r--r--   0     1001      123    39478 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/huf_compress.c
+-rw-r--r--   0     1001      123   284402 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress.c
+-rw-r--r--   0     1001      123    56573 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_internal.h
+-rw-r--r--   0     1001      123     6251 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.c
+-rw-r--r--   0     1001      123     1210 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.h
+-rw-r--r--   0     1001      123    19914 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.c
+-rw-r--r--   0     1001      123     2166 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.h
+-rw-r--r--   0     1001      123    28469 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.c
+-rw-r--r--   0     1001      123     1159 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.h
+-rw-r--r--   0     1001      123    24477 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_cwksp.h
+-rw-r--r--   0     1001      123    25353 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.c
+-rw-r--r--   0     1001      123     1279 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.h
+-rw-r--r--   0     1001      123    22332 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.c
+-rw-r--r--   0     1001      123     1199 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.h
+-rw-r--r--   0     1001      123    96019 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.c
+-rw-r--r--   0     1001      123     5647 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.h
+-rw-r--r--   0     1001      123    28379 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.c
+-rw-r--r--   0     1001      123     4449 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.h
+-rw-r--r--   0     1001      123     5957 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm_geartab.h
+-rw-r--r--   0     1001      123    62886 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.c
+-rw-r--r--   0     1001      123     2002 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.h
+-rw-r--r--   0     1001      123    78690 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.c
+-rw-r--r--   0     1001      123     4430 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.h
+-rw-r--r--   0     1001      123    55120 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/huf_decompress.c
+-rw-r--r--   0     1001      123     9153 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.c
+-rw-r--r--   0     1001      123     1310 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.h
+-rw-r--r--   0     1001      123    91256 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress.c
+-rw-r--r--   0     1001      123    66872 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.c
+-rw-r--r--   0     1001      123     2242 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.h
+-rw-r--r--   0     1001      123     8450 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_internal.h
+-rw-r--r--   0     1001      123    11492 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff.h
+-rw-r--r--   0     1001      123      999 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_common.c
+-rw-r--r--   0     1001      123     5320 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_compress.c
+-rw-r--r--   0     1001      123     1905 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_decompress.c
+-rw-r--r--   0     1001      123    42474 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.c
+-rw-r--r--   0     1001      123     5004 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.h
+-rw-r--r--   0     1001      123    54649 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.c
+-rw-r--r--   0     1001      123     2419 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.h
+-rw-r--r--   0     1001      123    28242 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/fastcover.c
+-rw-r--r--   0     1001      123    44423 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/zdict.c
+-rw-r--r--   0     1001      123     1464 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/Makefile
+-rw-r--r--   0     1001      123     2953 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/README.md
+-rw-r--r--   0     1001      123      784 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/build_package.bat
+-rw-r--r--   0     1001      123     1269 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.sln
+-rw-r--r--   0     1001      123    10105 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.vcxproj
+-rw-r--r--   0     1001      123    13898 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_legacy.h
+-rw-r--r--   0     1001      123    71508 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.c
+-rw-r--r--   0     1001      123     3793 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.h
+-rw-r--r--   0     1001      123   128181 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.c
+-rw-r--r--   0     1001      123     3702 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.h
+-rw-r--r--   0     1001      123   114301 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.c
+-rw-r--r--   0     1001      123     3714 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.h
+-rw-r--r--   0     1001      123   135414 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.c
+-rw-r--r--   0     1001      123     6432 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.h
+-rw-r--r--   0     1001      123   156554 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.c
+-rw-r--r--   0     1001      123     7530 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.h
+-rw-r--r--   0     1001      123   166181 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.c
+-rw-r--r--   0     1001      123     8068 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.h
+-rw-r--r--   0     1001      123   185229 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.c
+-rw-r--r--   0     1001      123     8711 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.h
+-rw-r--r--   0     1001      123      417 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/libzstd.pc.in
+-rw-r--r--   0     1001      123    25655 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zdict.h
+-rw-r--r--   0     1001      123   145904 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd.h
+-rw-r--r--   0     1001      123     3817 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd_errors.h
+-rw-r--r--   0     1001      123      367 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/.gitignore
+-rw-r--r--   0     1001      123      920 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/BUCK
+-rw-r--r--   0     1001      123    17458 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/Makefile
+-rw-r--r--   0     1001      123    17639 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/README.md
+-rw-r--r--   0     1001      123     9826 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.c
+-rw-r--r--   0     1001      123     8714 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.h
+-rw-r--r--   0     1001      123    35448 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.c
+-rw-r--r--   0     1001      123     8780 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.h
+-rw-r--r--   0     1001      123     6182 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.c
+-rw-r--r--   0     1001      123     1187 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.h
+-rw-r--r--   0     1001      123    15321 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.c
+-rw-r--r--   0     1001      123     1490 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.h
+-rw-r--r--   0     1001      123   125138 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.c
+-rw-r--r--   0     1001      123     7258 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.h
+-rw-r--r--   0     1001      123     8836 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/platform.h
+-rw-r--r--   0     1001      123     4964 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.c
+-rw-r--r--   0     1001      123     2552 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.h
+-rw-r--r--   0     1001      123    39814 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.c
+-rw-r--r--   0     1001      123    10462 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.h
+-rw-r--r--   0     1001      123      658 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/verrsrc.h
+-rw-r--r--   0     1001      123     1467 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd.rc
+-rw-r--r--   0     1001      123     1044 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd32.res
+-rw-r--r--   0     1001      123     1044 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd64.res
+-rw-r--r--   0     1001      123    28509 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1
+-rw-r--r--   0     1001      123    26945 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1.md
+-rw-r--r--   0     1001      123    66138 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli.c
+-rw-r--r--   0     1001      123     4916 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.c
+-rw-r--r--   0     1001      123      595 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.h
+-rwxr-xr-x   0     1001      123     3869 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep
+-rw-r--r--   0     1001      123      779 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1
+-rw-r--r--   0     1001      123      726 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1.md
+-rwxr-xr-x   0     1001      123       30 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdless
+-rw-r--r--   0     1001      123      378 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdless.1
+-rw-r--r--   0     1001      123      356 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdless.1.md
+-rw-r--r--   0     1001      123      678 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/.gitignore
+-rwxr-xr-x   0     1001      123    18201 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/DEPRECATED-test-zstd-speed.py
+-rw-r--r--   0     1001      123    14839 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/Makefile
+-rw-r--r--   0     1001      123     9619 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/README.md
+-rw-r--r--   0     1001      123    13245 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/automated_benchmarking.py
+-rw-r--r--   0     1001      123     4060 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/bigdict.c
+-rw-r--r--   0     1001      123     1994 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/checkTag.c
+-rw-r--r--   0     1001      123     4519 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/datagencli.c
+-rw-r--r--   0     1001      123    69924 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/decodecorpus.c
+-rw-r--r--   0     1001      123      153 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/dict-files/zero-weight-dict
+-rw-r--r--   0     1001      123    34888 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fullbench.c
+-rw-r--r--   0     1001      123      423 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/.gitignore
+-rw-r--r--   0     1001      123     9701 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/Makefile
+-rw-r--r--   0     1001      123     2993 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/README.md
+-rw-r--r--   0     1001      123     1340 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_decompress.c
+-rw-r--r--   0     1001      123     3153 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_round_trip.c
+-rw-r--r--   0     1001      123     2198 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/decompress_dstSize_tooSmall.c
+-rw-r--r--   0     1001      123     2480 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_decompress.c
+-rw-r--r--   0     1001      123     3786 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_loader.c
+-rw-r--r--   0     1001      123     5744 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_round_trip.c
+-rw-r--r--   0     1001      123     7313 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_stream_round_trip.c
+-rw-r--r--   0     1001      123     3478 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fse_read_ncount.c
+-rw-r--r--   0     1001      123     1926 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.h
+-rwxr-xr-x   0     1001      123    29048 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.py
+-rw-r--r--   0     1001      123     2752 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.c
+-rw-r--r--   0     1001      123     2664 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.h
+-rw-r--r--   0     1001      123      761 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.c
+-rw-r--r--   0     1001      123     2040 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.h
+-rw-r--r--   0     1001      123     4144 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/raw_dictionary_round_trip.c
+-rw-r--r--   0     1001      123     2683 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/regression_driver.c
+-rw-r--r--   0     1001      123     3383 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/seekable_roundtrip.c
+-rw-r--r--   0     1001      123    11823 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/sequence_compression_api.c
+-rw-r--r--   0     1001      123     1791 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_compress.c
+-rw-r--r--   0     1001      123     1422 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_decompress.c
+-rw-r--r--   0     1001      123     5355 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_round_trip.c
+-rw-r--r--   0     1001      123     3313 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_decompress.c
+-rw-r--r--   0     1001      123     5962 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_round_trip.c
+-rw-r--r--   0     1001      123     1354 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_frame_info.c
+-rw-r--r--   0     1001      123     6131 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.c
+-rw-r--r--   0     1001      123     1404 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.h
+-rw-r--r--   0     1001      123   199849 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzzer.c
+-rw-r--r--   0     1001      123     1189 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-compression/http
+-rw-r--r--   0     1001      123      143 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-compression/huffman-compressed-larger
+-rw-r--r--   0     1001      123       45 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-decompression/rle-first-block.zst
+-rw-r--r--   0     1001      123     1000 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-dictionaries/http-dict-missing-symbols
+-rw-r--r--   0     1001      123     1581 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/Makefile
+-rwxr-xr-x   0     1001      123     1447 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/gzip-env.sh
+-rw-r--r--   0     1001      123     1070 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/helin-segv.sh
+-rw-r--r--   0     1001      123     8199 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/help-version.sh
+-rw-r--r--   0     1001      123      425 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/hufts-segv.gz
+-rw-r--r--   0     1001      123     1156 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/hufts.sh
+-rw-r--r--   0     1001      123      178 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/init.cfg
+-rw-r--r--   0     1001      123    19982 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/init.sh
+-rw-r--r--   0     1001      123     1484 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/keep.sh
+-rw-r--r--   0     1001      123     1032 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/list.sh
+-rw-r--r--   0     1001      123     1211 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/memcpy-abuse.sh
+-rw-r--r--   0     1001      123     2180 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/mixed.sh
+-rw-r--r--   0     1001      123     1191 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/null-suffix-clobber.sh
+-rw-r--r--   0     1001      123     1029 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/stdin.sh
+-rw-r--r--   0     1001      123     4664 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/test-driver.sh
+-rw-r--r--   0     1001      123     1245 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/trailing-nul.sh
+-rw-r--r--   0     1001      123     1489 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/unpack-invalid.sh
+-rw-r--r--   0     1001      123      995 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/z-suffix.sh
+-rw-r--r--   0     1001      123     1257 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zdiff.sh
+-rw-r--r--   0     1001      123     1455 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-context.sh
+-rw-r--r--   0     1001      123     1362 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-f.sh
+-rw-r--r--   0     1001      123     2163 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-signal.sh
+-rw-r--r--   0     1001      123     1226 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/znew-k.sh
+-rw-r--r--   0     1001      123     2092 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/invalidDictionaries.c
+-rw-r--r--   0     1001      123    10852 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/legacy.c
+-rwxr-xr-x   0     1001      123     3232 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/libzstd_partial_builds.sh
+-rw-r--r--   0     1001      123     3094 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/longmatch.c
+-rw-r--r--   0     1001      123   103954 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/paramgrill.c
+-rwxr-xr-x   0     1001      123    61408 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/playTests.sh
+-rw-r--r--   0     1001      123     6810 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/poolTests.c
+-rwxr-xr-x   0     1001      123     1157 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/rateLimiter.py
+-rw-r--r--   0     1001      123       44 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/.gitignore
+-rw-r--r--   0     1001      123     1903 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/Makefile
+-rw-r--r--   0     1001      123      895 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/README.md
+-rw-r--r--   0     1001      123    19648 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.c
+-rw-r--r--   0     1001      123     2459 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.h
+-rw-r--r--   0     1001      123    16569 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.c
+-rw-r--r--   0     1001      123     3047 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.h
+-rw-r--r--   0     1001      123     1199 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/levels.h
+-rw-r--r--   0     1001      123    21685 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.c
+-rw-r--r--   0     1001      123     1772 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.h
+-rw-r--r--   0     1001      123      934 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.c
+-rw-r--r--   0     1001      123     2626 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.h
+-rw-r--r--   0     1001      123   161474 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/results.csv
+-rw-r--r--   0     1001      123    11030 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/test.c
+-rw-r--r--   0     1001      123     7914 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/roundTripCrash.c
+-rw-r--r--   0     1001      123     8022 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.c
+-rw-r--r--   0     1001      123     1629 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.h
+-rwxr-xr-x   0     1001      123     4344 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-license.py
+-rwxr-xr-x   0     1001      123    10843 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-zstd-versions.py
+-rw-r--r--   0     1001      123   126462 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/zstreamtest.c
+-rw-r--r--   0     1001      123      256 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/.gitignore
+-rw-r--r--   0     1001      123      433 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/BUCK
+-rw-r--r--   0     1001      123     3920 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/Makefile
+-rw-r--r--   0     1001      123     7889 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/README.md
+-rw-r--r--   0     1001      123    18239 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example.c
+-rw-r--r--   0     1001      123    17604 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example_original.c
+-rw-r--r--   0     1001      123    10791 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk.c
+-rw-r--r--   0     1001      123     8595 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk_original.c
+-rw-r--r--   0     1001      123    15495 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/minigzip.c
+-rw-r--r--   0     1001      123    46077 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/zwrapbench.c
+-rw-r--r--   0     1001      123      849 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzclose.c
+-rw-r--r--   0     1001      123     1873 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzcompatibility.h
+-rw-r--r--   0     1001      123     7142 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzguts.h
+-rw-r--r--   0     1001      123    17564 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzlib.c
+-rw-r--r--   0     1001      123    22213 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzread.c
+-rw-r--r--   0     1001      123    20440 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzwrite.c
+-rw-r--r--   0     1001      123    42651 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.c
+-rw-r--r--   0     1001      123     3648 2023-04-17 16:18:19.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.h
+-rw-r--r--   0     1001      123       24 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/wrapper.h
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 libertem_dectris-0.2.8/Cargo.toml
+-rw-r--r--   0     1001      123     4626 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/README.md
+-rw-r--r--   0     1001      123    12793 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/live_server.py
+-rw-r--r--   0     1001      123     1408 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/passive.py
+-rw-r--r--   0     1001      123     2123 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/passive_low_level.py
+-rw-r--r--   0     1001      123     2191 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/simple.py
+-rw-r--r--   0     1001      123     1353 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/testchunked.py
+-rw-r--r--   0     1001      123     1507 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/testflame.py
+-rw-r--r--   0     1001      123     1275 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/testrepeat.py
+-rw-r--r--   0     1001      123     1179 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/testserialize.py
+-rw-r--r--   0     1001      123     1192 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/testtooslow.py
+-rw-r--r--   0     1001      123     1806 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/examples/testudf.py
+-rw-r--r--   0     1001      123      449 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/pyproject.toml
+-rw-r--r--   0     1001      123       31 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/rust-toolchain.toml
+-rw-r--r--   0     1001      123    13277 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/cam_client.rs
+-rw-r--r--   0     1001      123    10602 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/common.rs
+-rw-r--r--   0     1001      123    11101 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/dectris_py.rs
+-rw-r--r--   0     1001      123      413 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/exceptions.rs
+-rw-r--r--   0     1001      123    12395 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/frame_stack.rs
+-rw-r--r--   0     1001      123      143 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/lib.rs
+-rw-r--r--   0     1001      123    10123 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/main.rs
+-rw-r--r--   0     1001      123    22099 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/receiver.rs
+-rw-r--r--   0     1001      123     9693 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/sim.rs
+-rw-r--r--   0     1001      123      733 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/src/stats.rs
+-rw-r--r--   0     1001      123    95572 2023-04-17 16:18:17.000000 libertem_dectris-0.2.8/Cargo.lock
+-rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 libertem_dectris-0.2.8/PKG-INFO
```

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/build.rs` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/build.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/src/lib.rs` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/lint.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/main.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/wheels.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/.gitignore` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/.gitignore`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/LICENSE` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/README.rst` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/README.rst`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/__init__.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/ext.pyx` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/ext.pyx`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/h5.pyx` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/bitshuffle/h5.pyx`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/LICENSE` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lz4/lz4.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/LICENSE.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/README.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/README.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/example.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/example.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzfP.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzfP.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_c.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_c.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_d.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf/lzf_d.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/lzf/lzf_filter.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/setup.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/setup.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_core.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_internals.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bitshuffle_internals.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/bshuf_h5filter.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/hdf5_dl.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/hdf5_dl.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/iochain.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/src/lzf_h5plugin.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/src/lzf_h5plugin.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.1.3.h5` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.1.3.h5`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.4.0.h5` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/data/regression_0.4.0.h5`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/make_regression_tdata.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/make_regression_tdata.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_ext.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5filter.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5filter.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5plugin.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_h5plugin.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_regression.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.circleci/config.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/bug_report.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/feature_request.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-long-tests.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-long-tests.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-short-tests.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/dev-short-tests.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/publish-release-artifacts.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.github/workflows/publish-release-artifacts.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.travis.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/.travis.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CHANGELOG` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CHANGELOG`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CONTRIBUTING.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/COPYING` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/COPYING`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/LICENSE` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/TESTING.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/TESTING.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/appveyor.yml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/appveyor.yml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fullbench/fullbench.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fullbench/fullbench.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fuzzer/fuzzer.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/fuzzer/fuzzer.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd/zstd.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd/zstd.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd.sln` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstd.sln`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstdlib/zstdlib.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2008/zstdlib/zstdlib.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/datagen/datagen.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench/fullbench.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench-dll/fullbench-dll.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fuzzer/fuzzer.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd/libzstd.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd/libzstd.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.rc` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.rc`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/libzstd-dll/libzstd-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.rc` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.rc`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd/zstd.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd.sln` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS2010/zstd.sln`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.generic.cmd` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/VS_scripts/build.generic.cmd`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeLists.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/AddZstdCompilationFlags.cmake` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/AddZstdCompilationFlags.cmake`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/FindLibLZ4.cmake` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/CMakeModules/FindLibLZ4.cmake`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/gen_html/CMakeLists.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/gen_html/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/pzstd/CMakeLists.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/contrib/pzstd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/CMakeLists.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/cmake_uninstall.cmake.in` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/lib/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/programs/CMakeLists.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/programs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/tests/CMakeLists.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/cmake/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/GetZstdLibraryVersion.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/GetZstdLibraryVersion.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/InstallSymlink.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/InstallSymlink.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/gen_html/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/gen_html/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/pzstd/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/contrib/pzstd/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/lib/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/lib/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson_options.txt` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/meson_options.txt`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/programs/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/programs/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/meson.build` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/meson.build`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/valgrindTest.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/meson/tests/valgrindTest.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_decoder_test.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_decoder_test.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_library_test.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/build_library_test.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/combine.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/combine.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/emscripten.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/emscripten.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/roundtrip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/roundtrip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/shell.html` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/shell.html`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/simple.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/simple.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-dxt1.inl` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-dxt1.inl`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-zstd.inl` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard-zstd.inl`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/examples/testcard.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstd-in.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstd-in.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstddeclib-in.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/build/single_file_libs/zstddeclib-in.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fullbench/fullbench.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fullbench/fullbench.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fuzzer/fuzzer.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/fuzzer/fuzzer.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd/zstd.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd/zstd.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd.sln` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstd.sln`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstdlib/zstdlib.vcproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/VS2005/zstdlib/zstdlib.vcproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/check_flipped_bits.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/diagnose_corruption/check_flipped_bits.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/docker/Dockerfile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/freestanding_lib/freestanding.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/freestanding_lib/freestanding.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen-zstd-manual.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen-zstd-manual.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen_html.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/gen_html/gen_html.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/largeNbDicts.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/largeNbDicts/largeNbDicts.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-benchmark.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-benchmark.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-extract-benchmark.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/btrfs-extract-benchmark.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/decompress_sources.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/decompress_sources.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux.mk` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux.mk`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux_zstd.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/linux_zstd.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/mem.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/mem.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/squashfs-benchmark.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/squashfs-benchmark.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/asm/unaligned.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/asm/unaligned.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/compiler.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/compiler.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/kernel.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/kernel.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/module.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/module.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/xxhash.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/include/linux/xxhash.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/macro-test.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/macro-test.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/static_test.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/static_test.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/test.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/test/test.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_compress_module.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_compress_module.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_decompress_module.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_decompress_module.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_deps.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/linux-kernel/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/match_finders/zstd_edist.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/premake/zstd.lua` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/premake/zstd.lua`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/BUCK` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/BUCK`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/ErrorHolder.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/ErrorHolder.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Logging.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Logging.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Options.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/Pzstd.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/SkippableFrame.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Cspeed.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Cspeed.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Dspeed.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/images/Dspeed.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/main.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/main.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/BUCK` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/BUCK`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/OptionsTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/OptionsTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/PzstdTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/PzstdTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTrip.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTrip.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTripTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/test/RoundTripTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/BUCK` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/BUCK`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Buffer.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Buffer.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/FileSystem.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/FileSystem.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Likely.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Likely.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Range.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/Range.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ResourcePool.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ResourcePool.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ScopeGuard.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ScopeGuard.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ThreadPool.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/ThreadPool.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/WorkQueue.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/WorkQueue.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BUCK` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BUCK`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BufferTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/BufferTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/RangeTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/RangeTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ResourcePoolTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ResourcePoolTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ScopeGuardTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ScopeGuardTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ThreadPoolTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/ThreadPoolTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/WorkQueueTest.cpp` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/pzstd/utils/test/WorkQueueTest.cpp`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/recover_directory.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/recovery/recover_directory.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_processing.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/parallel_processing.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression_mem.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/examples/seekable_decompression_mem.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/seekable_tests.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/tests/seekable_tests.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable_compression_format.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstd_seekable_compression_format.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/seekable_format/zstdseek_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/snap/snapcraft.yaml` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/contrib/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/harness.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/harness.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/educational_decoder/zstd_decompress.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/CSpeed2.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/CSpeed2.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DCspeed5.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DCspeed5.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DSpeed3.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/DSpeed3.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/cdict_v136.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/cdict_v136.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cr.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cr.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cs.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-cs.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-ds.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/dict-ds.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_cdict_v1_3_5.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_cdict_v1_3_5.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_logo86.png` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/images/zstd_logo86.png`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_compression_format.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_compression_format.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_manual.html` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/doc/zstd_manual.html`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/common.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/common.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_decompression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/dictionary_decompression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_simple_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_simple_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_streaming_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/multiple_streaming_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_decompression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/simple_decompression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression_thread_pool.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_compression_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_decompression.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_decompression.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_memory_usage.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/examples/streaming_memory_usage.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/BUCK` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/BUCK`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/bitstream.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/compiler.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/compiler.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/cpu.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/cpu.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/debug.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/entropy_common.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/error_private.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/huf.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/huf.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/mem.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/mem.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/pool.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/threading.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_common.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_deps.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_internal.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_trace.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/common/zstd_trace.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/fse_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/hist.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/huf_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_internal.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_cwksp.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm_geartab.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_ldm_geartab.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/huf_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_internal.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_common.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/fastcover.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/zdict.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/build_package.bat` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/build_package.bat`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.sln` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.vcxproj` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_legacy.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zdict.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zdict.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd_errors.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/lib/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/BUCK` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/BUCK`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchfn.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/benchzstd.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/datagen.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/dibio.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/platform.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/platform.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/timefn.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/util.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/verrsrc.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/verrsrc.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd.rc` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd.rc`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd32.res` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd32.res`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd64.res` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/windres/zstd64.res`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstd.1.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdcli_trace.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/programs/zstdgrep.1.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/.gitignore` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/.gitignore`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/DEPRECATED-test-zstd-speed.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/DEPRECATED-test-zstd-speed.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/automated_benchmarking.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/automated_benchmarking.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/bigdict.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/bigdict.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/checkTag.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/checkTag.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/datagencli.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/datagencli.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/decodecorpus.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/decodecorpus.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fullbench.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fullbench.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_round_trip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/block_round_trip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/decompress_dstSize_tooSmall.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/decompress_dstSize_tooSmall.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_loader.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_loader.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_round_trip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_round_trip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_stream_round_trip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/dictionary_stream_round_trip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fse_read_ncount.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fse_read_ncount.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_data_producer.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/fuzz_helpers.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/raw_dictionary_round_trip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/raw_dictionary_round_trip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/regression_driver.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/regression_driver.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/seekable_roundtrip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/seekable_roundtrip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/sequence_compression_api.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/sequence_compression_api.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_compress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_compress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_round_trip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/simple_round_trip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_decompress.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_decompress.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_round_trip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/stream_round_trip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_frame_info.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_frame_info.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzz/zstd_helpers.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzzer.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/fuzzer.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-compression/http` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-compression/http`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-dictionaries/http-dict-missing-symbols` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/golden-dictionaries/http-dict-missing-symbols`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/gzip-env.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/gzip-env.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/helin-segv.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/helin-segv.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/help-version.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/help-version.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/hufts.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/hufts.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/init.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/init.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/keep.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/keep.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/list.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/list.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/memcpy-abuse.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/memcpy-abuse.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/mixed.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/mixed.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/null-suffix-clobber.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/null-suffix-clobber.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/stdin.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/stdin.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/test-driver.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/test-driver.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/trailing-nul.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/trailing-nul.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/unpack-invalid.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/unpack-invalid.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/z-suffix.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/z-suffix.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zdiff.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zdiff.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-context.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-context.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-f.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-f.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-signal.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/zgrep-signal.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/znew-k.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/gzip/znew-k.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/invalidDictionaries.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/invalidDictionaries.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/legacy.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/legacy.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/libzstd_partial_builds.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/libzstd_partial_builds.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/longmatch.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/longmatch.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/paramgrill.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/paramgrill.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/playTests.sh` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/playTests.sh`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/poolTests.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/poolTests.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/rateLimiter.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/rateLimiter.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/config.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/data.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/levels.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/levels.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/method.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/result.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/results.csv` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/results.csv`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/test.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/regression/test.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/roundTripCrash.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/roundTripCrash.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/seqgen.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-license.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-license.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-zstd-versions.py` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/test-zstd-versions.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/zstreamtest.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/tests/zstreamtest.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/Makefile` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/Makefile`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/README.md` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example_original.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/example_original.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk_original.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/fitblk_original.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/minigzip.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/minigzip.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/zwrapbench.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/examples/zwrapbench.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzclose.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzclose.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzcompatibility.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzcompatibility.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzguts.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzguts.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzlib.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzlib.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzread.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzread.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzwrite.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/gzwrite.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.c` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.c`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.h` & `libertem_dectris-0.2.8/local_dependencies/bs_sys/vendor/bitshuffle/zstd/zlibWrapper/zstd_zlibwrapper.h`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/Cargo.toml` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/examples/consumer/main.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/examples/consumer/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/examples/producer/main.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/examples/producer/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/src/backend_memfd.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/src/backend_memfd.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/src/backend_shm.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/src/backend_shm.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/src/freestack.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/src/freestack.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/src/lib.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/ipc-test/src/slab.rs` & `libertem_dectris-0.2.8/local_dependencies/ipc-test/src/slab.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/local_dependencies/stats/src/lib.rs` & `libertem_dectris-0.2.8/local_dependencies/stats/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/Cargo.toml` & `libertem_dectris-0.2.8/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "libertem-dectris"
 authors = ["Alexander Clausen <a.clausen@fz-juelich.de>"]
 license = "MIT"
-version = "0.2.7"
+version = "0.2.8"
 edition = "2021"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "libertem_dectris"
 crate-type = ["cdylib"]
```

### Comparing `libertem_dectris-0.2.7/README.md` & `libertem_dectris-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/live_server.py` & `libertem_dectris-0.2.8/examples/live_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from libertem.udf.sumsigudf import SumSigUDF
 from libertem.udf.masks import ApplyMasksUDF
 from libertem.executor.pipelined import PipelinedExecutor
 from libertem_live.api import LiveContext
 from libertem_live.udf.monitor import (
     SignalMonitorUDF, PartitionMonitorUDF
 )
-from libertem_live.detectors.dectris.acquisition import DectrisAcquisition, DectrisDetectorConnection
 
 from libertem.udf.base import UDFResults, UDF
 from libertem.common.async_utils import sync_to_async
 
 if typing.TYPE_CHECKING:
     from libertem.common.executor import JobExecutor
 
@@ -296,79 +295,75 @@
         }))
         for result in delta_results:
             await self.broadcast(result.compressed_data)
 
     async def acquisition_loop(self):
         min_delta = 0.05
         while True:
-            pending_acq = await sync_to_async(self.conn.wait_for_acquisition, timeout=10)
-            if pending_acq is None:
+            pending_aq = await sync_to_async(self.conn.wait_for_acquisition, timeout=10)
+            if pending_aq is None:
                 continue
-            acq_id = await self.handle_pending_acquisition(pending_acq)
+            acq_id = await self.handle_pending_acquisition(pending_aq)
             try:
                 print(f"acquisition starting with id={acq_id}")
                 t0 = time.perf_counter()
                 previous_results = None
                 partial_results = None
-                side = int(math.sqrt(pending_acq.detector_config.get_num_frames()))
-                aq = self.ctx.prepare_from_pending(
-                    pending_acq,
+                side = int(math.sqrt(pending_aq.detector_config.get_num_frames()))
+                aq = self.ctx.make_acquisition(
                     conn=self.conn,
-                    pending_aq=pending_acq,
+                    pending_aq=pending_aq,
                     frames_per_partition=512,
                     nav_shape=(side, side),
                 )
                 last_update = 0
                 try:
                     udfs_only = list(self.udfs.values())
                     async for partial_results in self.ctx.run_udf_iter(dataset=aq, udf=udfs_only, sync=False):
                         if time.time() - last_update > min_delta:
-                            await self.handle_partial_result(partial_results, pending_acq, acq_id, previous_results)
+                            await self.handle_partial_result(partial_results, pending_aq, acq_id, previous_results)
                             previous_results = copy.deepcopy(partial_results)
                             last_update = time.time()
-                    await self.handle_partial_result(partial_results, pending_acq, acq_id, previous_results)
+                    await self.handle_partial_result(partial_results, pending_aq, acq_id, previous_results)
                 except Exception as e:
                     import traceback
                     traceback.print_exc()
                     self.ctx.close()
                     self.conn.close()
                     self.connect()
                 previous_results = copy.deepcopy(partial_results)
             finally:
-                await self.handle_acquisition_end(pending_acq, acq_id)
+                await self.handle_acquisition_end(pending_aq, acq_id)
             previous_results = None
             t1 = time.perf_counter()
             print(f"acquisition done with id={acq_id}; took {t1-t0:.3f}s")
 
     async def serve(self):
         async with websockets.serve(self, "localhost", 8444):
             try:
                 await self.acquisition_loop()
             finally:
                 self.conn.close()
                 self.ctx.close()
 
     def connect(self):
-        conn = DectrisDetectorConnection(
-            api_host='localhost',
-            api_port=8910,
-            data_host='localhost',
-            data_port=9999,
-            frame_stack_size=8,
-            bytes_per_frame=150000,
-            num_slots=3000,
-        )
         executor = PipelinedExecutor(
             spec=PipelinedExecutor.make_spec(
                 cpus=range(20), cudas=[]
             ),
             pin_workers=False,
-            # delayed_gc=False,
         )
         ctx = LiveContext(executor=executor)
+        conn = ctx.make_connection('dectris').open(
+            api_host='localhost',
+            api_port=8910,
+            data_host='localhost',
+            data_port=9999,
+            buffer_size=2048,
+        )
 
         self.conn = conn
         self.executor = executor
         self.ctx = ctx
 
 async def main():
     server = WSServer()
```

### Comparing `libertem_dectris-0.2.7/examples/passive.py` & `libertem_dectris-0.2.8/examples/passive.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/passive_low_level.py` & `libertem_dectris-0.2.8/examples/passive_low_level.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/simple.py` & `libertem_dectris-0.2.8/examples/simple.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/testchunked.py` & `libertem_dectris-0.2.8/examples/testchunked.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/testflame.py` & `libertem_dectris-0.2.8/examples/testflame.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/testrepeat.py` & `libertem_dectris-0.2.8/examples/testrepeat.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/testserialize.py` & `libertem_dectris-0.2.8/examples/testserialize.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/testtooslow.py` & `libertem_dectris-0.2.8/examples/testtooslow.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/examples/testudf.py` & `libertem_dectris-0.2.8/examples/testudf.py`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/cam_client.rs` & `libertem_dectris-0.2.8/src/cam_client.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/common.rs` & `libertem_dectris-0.2.8/src/common.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/dectris_py.rs` & `libertem_dectris-0.2.8/src/dectris_py.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/frame_stack.rs` & `libertem_dectris-0.2.8/src/frame_stack.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/main.rs` & `libertem_dectris-0.2.8/src/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/receiver.rs` & `libertem_dectris-0.2.8/src/receiver.rs`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,16 @@
             }
 
             // second message: the header itself
             recv_part(&mut msg, socket, control_channel)?;
             let detector_config: DetectorConfig =
                 serde_json::from_str(msg.as_str().unwrap()).unwrap();
 
+            debug!("detector config: {}", msg.as_str().unwrap());
+
             acquisition(
                 detector_config,
                 control_channel,
                 from_thread_s,
                 socket,
                 dheader.series,
                 frame_stack_size,
@@ -487,14 +489,16 @@
                     debug!("dheader: {dheader:?}");
 
                     // second message: the header itself
                     recv_part(&mut msg, &socket, to_thread_r)?;
                     let detector_config: DetectorConfig =
                         serde_json::from_str(msg.as_str().unwrap()).unwrap();
 
+                    debug!("detector config: {}", msg.as_str().unwrap());
+
                     match acquisition(
                         detector_config,
                         to_thread_r,
                         from_thread_s,
                         &socket,
                         series,
                         frame_stack_size,
```

### Comparing `libertem_dectris-0.2.7/src/sim.rs` & `libertem_dectris-0.2.8/src/sim.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/src/stats.rs` & `libertem_dectris-0.2.8/src/stats.rs`

 * *Files identical despite different names*

### Comparing `libertem_dectris-0.2.7/Cargo.lock` & `libertem_dectris-0.2.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1654,15 +1654,15 @@
 name = "libc"
 version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "libertem-asi-tpx3"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "bincode",
  "crossbeam",
  "crossbeam-channel",
  "env_logger",
  "ipc-test",
  "log",
@@ -1673,15 +1673,15 @@
  "tempfile",
  "uuid",
  "zerocopy",
 ]
 
 [[package]]
 name = "libertem-dectris"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "bincode",
  "bs_sys",
  "clap 3.2.23",
  "crossbeam",
  "crossbeam-channel",
  "env_logger",
```

### Comparing `libertem_dectris-0.2.7/PKG-INFO` & `libertem_dectris-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libertem-dectris
-Version: 0.2.7
+Version: 0.2.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Author: Alexander Clausen <a.clausen@fz-juelich.de>
 Author-email: Alexander Clausen <a.clausen@fz-juelich.de>
 License: MIT
 Requires-Python: >=3.7
```

