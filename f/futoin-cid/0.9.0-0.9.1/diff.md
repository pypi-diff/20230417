# Comparing `tmp/futoin-cid-0.9.0.tar.gz` & `tmp/futoin-cid-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futoin-cid-0.9.0.tar", last modified: Mon Mar 27 03:24:42 2023, max compression
+gzip compressed data, was "futoin-cid-0.9.1.tar", last modified: Mon Apr 17 00:16:18 2023, max compression
```

## Comparing `futoin-cid-0.9.0.tar` & `futoin-cid-0.9.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.549332 futoin-cid-0.9.0/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    11358 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/LICENSE
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     8300 2023-03-27 03:24:42.553332 futoin-cid-0.9.0/PKG-INFO
--rwxr-xr-x   0 cfdev     (1000) cfdev     (1000)     6577 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/README.rst
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.525332 futoin-cid-0.9.0/futoin/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      702 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/__init__.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.529332 futoin-cid-0.9.0/futoin/cid/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      807 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      635 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/__main__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      961 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/buildtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    38774 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/cidtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    17797 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/cli.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1499 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/coloring.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.529332 futoin-cid-0.9.0/futoin/cid/contrib/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/contrib/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    49556 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/contrib/distro.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    19950 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/contrib/docopt.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2359 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/cte.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.533332 futoin-cid-0.9.0/futoin/cid/details/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/details/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    23093 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/details/nginx.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    11655 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/details/resourcealgo.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      763 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/migrationtool.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.533332 futoin-cid-0.9.0/futoin/cid/misc/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/misc/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3830 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/misc/releasetool.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.533332 futoin-cid-0.9.0/futoin/cid/mixins/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    18389 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/config.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1500 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/data.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    19074 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/deploy.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3245 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/lock.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1028 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/log.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3180 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/ondemand.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    17259 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/service.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    11113 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/mixins/tool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3785 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/rmstool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      710 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/runenvtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1908 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/runtimetool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5625 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/subtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      751 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/testtool.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.545332 futoin-cid-0.9.0/futoin/cid/tool/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1980 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/anttool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7336 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/archivatool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9227 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/artifactorytool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3416 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/awstool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      794 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/bashtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1274 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/bashtoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1691 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/binutilstool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1969 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/bowertool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3834 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/brewtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3364 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/bundlermixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3066 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/bundlertool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1295 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/bzip2tool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2213 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/cargotool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3353 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/cidtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3002 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/cmaketool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3774 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/composertool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1463 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/ctesttool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1026 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/curltool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1044 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/curltoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1700 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/dockercomposetool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5028 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/dockertool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1033 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/elixirtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1146 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/erlangtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      931 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/exetool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3755 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/flywaytool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1308 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/futointool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1571 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gcctool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2258 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gemtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2553 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gemtoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    12670 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gittool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3694 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gotool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1454 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gpgtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2583 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gradletool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1074 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/grunttool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1006 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gulptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2934 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gvmtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3443 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/gziptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9893 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/hgtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7161 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/javatool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1193 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/javatoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4117 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/jdktool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2736 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/jfrogtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4074 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/liquibasetool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1534 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/maketool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1992 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/maventool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3574 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/mixtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4567 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/nexus3tool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5630 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/nexustool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7382 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/nginxtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4411 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/nodetool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4954 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/npmtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2209 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/npmtoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2387 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/nvmtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2910 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/phoenixtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2589 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/phpbuildtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    10752 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/phpfpmtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    16680 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/phptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2693 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/piptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3075 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/piptoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2902 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/pumatool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3802 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/puppettool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3367 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/pythontool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    13617 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/rubytool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2042 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/rusttool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2639 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/rustuptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3306 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/rvmtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2078 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/sbttool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1256 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/scalatool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9003 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/scptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2325 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/sdkmantool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3939 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/sdkmantoolmixin.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2401 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/setuptoolstool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1324 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/sshtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)    12824 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/svntool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1294 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/tartool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2149 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/twinetool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1216 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/unziptool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4189 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/uwsgitool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4407 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/virtualenvtool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2269 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/webpacktool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1049 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/xztool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1643 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/yarntool.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      932 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/tool/ziptool.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.549332 futoin-cid-0.9.0/futoin/cid/util/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1227 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4713 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/builddep.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2684 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/configutil.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5767 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/detect.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     6690 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/executil.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1573 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/github.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.549332 futoin-cid-0.9.0/futoin/cid/util/install/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2818 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/__init__.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1933 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/apk.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3369 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/deb.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1071 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/ebuild.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1911 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/java.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4475 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/macos.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      968 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/pacman.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7828 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/install/rpm.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1176 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/log.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9170 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/pathutil.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     8907 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/phputil.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1010 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/util/versionutil.py
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2772 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/futoin/cid/vcstool.py
-drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-03-27 03:24:42.549332 futoin-cid-0.9.0/futoin_cid.egg-info/
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     8300 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/PKG-INFO
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4108 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/SOURCES.txt
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)        1 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/dependency_links.txt
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)      100 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/entry_points.txt
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)        7 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/namespace_packages.txt
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)       59 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/requires.txt
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)        7 2023-03-27 03:24:42.000000 futoin-cid-0.9.0/futoin_cid.egg-info/top_level.txt
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)       67 2023-03-27 03:24:42.553332 futoin-cid-0.9.0/setup.cfg
--rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3382 2023-03-27 03:24:41.000000 futoin-cid-0.9.0/setup.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    11358 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/LICENSE
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     8300 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/PKG-INFO
+-rwxr-xr-x   0 cfdev     (1000) cfdev     (1000)     6577 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/README.rst
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.394895 futoin-cid-0.9.1/futoin/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      702 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/__init__.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.398895 futoin-cid-0.9.1/futoin/cid/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      807 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      635 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/__main__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      961 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/buildtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    38774 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/cidtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    17797 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/cli.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1499 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/coloring.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.398895 futoin-cid-0.9.1/futoin/cid/contrib/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/contrib/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    49556 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/contrib/distro.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    19950 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/contrib/docopt.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2359 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/cte.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.398895 futoin-cid-0.9.1/futoin/cid/details/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/details/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    23093 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/details/nginx.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    11655 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/details/resourcealgo.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      763 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/migrationtool.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.398895 futoin-cid-0.9.1/futoin/cid/misc/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/misc/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3830 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/misc/releasetool.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.398895 futoin-cid-0.9.1/futoin/cid/mixins/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    18389 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/config.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1500 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/data.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    19074 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/deploy.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3245 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/lock.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1028 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/log.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3180 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/ondemand.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    17259 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/service.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    11113 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/mixins/tool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3785 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/rmstool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      710 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/runenvtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1908 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/runtimetool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5625 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/subtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      751 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/testtool.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/futoin/cid/tool/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      606 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1980 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/anttool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7336 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/archivatool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9227 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/artifactorytool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3416 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/awstool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      794 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/bashtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1274 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/bashtoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1691 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/binutilstool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1969 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/bowertool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3834 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/brewtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3364 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/bundlermixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3066 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/bundlertool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1295 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/bzip2tool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2213 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/cargotool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3353 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/cidtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3236 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/cmaketool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3774 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/composertool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1463 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/ctesttool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1026 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/curltool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1044 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/curltoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1700 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/dockercomposetool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5028 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/dockertool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1033 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/elixirtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1146 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/erlangtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      931 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/exetool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3755 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/flywaytool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1308 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/futointool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1571 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gcctool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2258 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gemtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2553 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gemtoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    12670 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gittool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3694 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gotool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1454 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gpgtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2583 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gradletool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1074 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/grunttool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1006 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gulptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2934 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gvmtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3443 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/gziptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9893 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/hgtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7161 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/javatool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1193 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/javatoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4117 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/jdktool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2736 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/jfrogtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4074 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/liquibasetool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1534 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/maketool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1992 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/maventool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3574 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/mixtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4567 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/nexus3tool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5630 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/nexustool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7382 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/nginxtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4411 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/nodetool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4954 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/npmtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2209 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/npmtoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2387 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/nvmtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2910 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/phoenixtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2589 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/phpbuildtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    10752 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/phpfpmtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    16680 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/phptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2693 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/piptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3075 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/piptoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2902 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/pumatool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3802 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/puppettool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3367 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/pythontool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    13617 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/rubytool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2042 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/rusttool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2639 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/rustuptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3306 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/rvmtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2078 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/sbttool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1256 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/scalatool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9003 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/scptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2325 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/sdkmantool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3939 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/sdkmantoolmixin.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2401 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/setuptoolstool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1324 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/sshtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)    12824 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/svntool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1294 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/tartool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2149 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/twinetool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1216 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/unziptool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4189 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/uwsgitool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4407 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/virtualenvtool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2269 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/webpacktool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1049 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/xztool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1643 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/yarntool.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      932 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/tool/ziptool.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/futoin/cid/util/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1227 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4713 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/builddep.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2684 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/configutil.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     5767 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/detect.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     6690 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/executil.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1573 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/github.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/futoin/cid/util/install/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2818 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/__init__.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1933 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/apk.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3369 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/deb.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1071 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/ebuild.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1911 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/java.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4475 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/macos.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      968 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/pacman.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     7828 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/install/rpm.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1176 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/log.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     9170 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/pathutil.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     8907 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/phputil.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     1010 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/util/versionutil.py
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     2772 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/futoin/cid/vcstool.py
+drwxr-xr-x   0 cfdev     (1000) cfdev     (1000)        0 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/futoin_cid.egg-info/
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     8300 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/PKG-INFO
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     4108 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/SOURCES.txt
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)        1 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/dependency_links.txt
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)      100 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/entry_points.txt
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)        7 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/namespace_packages.txt
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)       59 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/requires.txt
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)        7 2023-04-17 00:16:18.000000 futoin-cid-0.9.1/futoin_cid.egg-info/top_level.txt
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)       67 2023-04-17 00:16:18.406895 futoin-cid-0.9.1/setup.cfg
+-rw-r--r--   0 cfdev     (1000) cfdev     (1000)     3382 2023-04-17 00:16:17.000000 futoin-cid-0.9.1/setup.py
```

### Comparing `futoin-cid-0.9.0/LICENSE` & `futoin-cid-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/PKG-INFO` & `futoin-cid-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futoin-cid
-Version: 0.9.0
+Version: 0.9.1
 Summary: FutoIn Continuous Integration & Delivery Tool
 Home-page: https://github.com/futoin/cid-tool
 Download-URL: https://github.com/futoin/cid-tool/archive/master.zip
 Author: Andrey Galkin
 Author-email: andrey@futoin.org
 License: Apache 2.0
 Keywords: php ruby node nodejs npm gem rvm nvm grunt gulp bower  puppet build deploy futoin cmake make gradle maven java composer bundler
```

### Comparing `futoin-cid-0.9.0/README.rst` & `futoin-cid-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/__init__.py` & `futoin-cid-0.9.1/futoin/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/__init__.py` & `futoin-cid-0.9.1/futoin/cid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 from .cli import run
 from .subtool import SubTool
 from .buildtool import BuildTool
 from .rmstool import RmsTool
 from .runenvtool import RunEnvTool
 from .vcstool import VcsTool
```

### Comparing `futoin-cid-0.9.0/futoin/cid/__main__.py` & `futoin-cid-0.9.1/futoin/cid/__main__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/buildtool.py` & `futoin-cid-0.9.1/futoin/cid/buildtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/cidtool.py` & `futoin-cid-0.9.1/futoin/cid/cidtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/cli.py` & `futoin-cid-0.9.1/futoin/cid/cli.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/coloring.py` & `futoin-cid-0.9.1/futoin/cid/coloring.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/contrib/distro.py` & `futoin-cid-0.9.1/futoin/cid/contrib/distro.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/contrib/docopt.py` & `futoin-cid-0.9.1/futoin/cid/contrib/docopt.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/cte.py` & `futoin-cid-0.9.1/futoin/cid/cte.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/details/__init__.py` & `futoin-cid-0.9.1/futoin/cid/details/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/details/nginx.py` & `futoin-cid-0.9.1/futoin/cid/details/nginx.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/details/resourcealgo.py` & `futoin-cid-0.9.1/futoin/cid/details/resourcealgo.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/migrationtool.py` & `futoin-cid-0.9.1/futoin/cid/migrationtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/misc/__init__.py` & `futoin-cid-0.9.1/futoin/cid/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/misc/releasetool.py` & `futoin-cid-0.9.1/futoin/cid/misc/releasetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/__init__.py` & `futoin-cid-0.9.1/futoin/cid/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/config.py` & `futoin-cid-0.9.1/futoin/cid/mixins/config.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/data.py` & `futoin-cid-0.9.1/futoin/cid/mixins/data.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/deploy.py` & `futoin-cid-0.9.1/futoin/cid/mixins/deploy.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/lock.py` & `futoin-cid-0.9.1/futoin/cid/mixins/lock.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/log.py` & `futoin-cid-0.9.1/futoin/cid/mixins/log.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/ondemand.py` & `futoin-cid-0.9.1/futoin/cid/mixins/ondemand.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/service.py` & `futoin-cid-0.9.1/futoin/cid/mixins/service.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/mixins/tool.py` & `futoin-cid-0.9.1/futoin/cid/mixins/tool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/rmstool.py` & `futoin-cid-0.9.1/futoin/cid/rmstool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/runenvtool.py` & `futoin-cid-0.9.1/futoin/cid/runenvtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/runtimetool.py` & `futoin-cid-0.9.1/futoin/cid/runtimetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/subtool.py` & `futoin-cid-0.9.1/futoin/cid/subtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/testtool.py` & `futoin-cid-0.9.1/futoin/cid/testtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/__init__.py` & `futoin-cid-0.9.1/futoin/cid/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/anttool.py` & `futoin-cid-0.9.1/futoin/cid/tool/anttool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/archivatool.py` & `futoin-cid-0.9.1/futoin/cid/tool/archivatool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/artifactorytool.py` & `futoin-cid-0.9.1/futoin/cid/tool/artifactorytool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/awstool.py` & `futoin-cid-0.9.1/futoin/cid/tool/awstool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/bashtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/bashtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/bashtoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/bashtoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/binutilstool.py` & `futoin-cid-0.9.1/futoin/cid/tool/binutilstool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/bowertool.py` & `futoin-cid-0.9.1/futoin/cid/tool/bowertool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/brewtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/brewtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/bundlermixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/bundlermixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/bundlertool.py` & `futoin-cid-0.9.1/futoin/cid/tool/bundlertool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/bzip2tool.py` & `futoin-cid-0.9.1/futoin/cid/tool/bzip2tool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/cargotool.py` & `futoin-cid-0.9.1/futoin/cid/tool/cargotool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/cidtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/cidtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/cmaketool.py` & `futoin-cid-0.9.1/futoin/cid/tool/cmaketool.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def getOrder(self):
         return -10
 
     def autoDetectFiles(self):
         return 'CMakeLists.txt'
 
     def envNames(self):
-        return ['cmakeBin', 'cmakeBuildDir']
+        return ['cmakeBin', 'cmakeBuildDir', 'cmakeBuildType']
 
     def _installTool(self, env):
         self._install.deb(['build-essential'])
         self._install.rpm(['gcc', 'gcc-c++'])
         self._install.pacman(['gcc'])
         self._builddep.essential()
 
@@ -49,25 +49,30 @@
         self._install.emerge(['dev-util/cmake'])
         self._install.pacman(['cmake'])
         self._install.apk(['cmake'])
         self._install.brew('cmake')
 
     def initEnv(self, env):
         env.setdefault('cmakeBuildDir', 'build')
+        env.setdefault('cmakeBuildType', 'Debug' if env['type'] == 'dev' else 'Release')
         super(cmakeTool, self).initEnv(env)
 
     def onPrepare(self, config):
         ospath = self._ospath
         os = self._os
-        build_dir = config['env']['cmakeBuildDir']
+        env = config['env']
+        build_dir = env['cmakeBuildDir']
+        build_type = env['cmakeBuildType']
         self._pathutil.rmTree(build_dir)
 
         os.mkdir(build_dir)
-        cmd = [config['env']['cmakeBin'], '-H' +
-               config['wcDir'], '-B' + build_dir]
+        cmd = [config['env']['cmakeBin'],
+               '-H' + config['wcDir'],
+               '-B' + build_dir,
+               '-DCMAKE_BUILD_TYPE=' + build_type]
         self._executil.callMeaningful(cmd)
 
     def onBuild(self, config):
         ospath = self._ospath
         os = self._os
         build_dir = config['env']['cmakeBuildDir']
```

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/composertool.py` & `futoin-cid-0.9.1/futoin/cid/tool/composertool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/ctesttool.py` & `futoin-cid-0.9.1/futoin/cid/tool/ctesttool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/curltool.py` & `futoin-cid-0.9.1/futoin/cid/tool/curltool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/curltoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/curltoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/dockercomposetool.py` & `futoin-cid-0.9.1/futoin/cid/tool/dockercomposetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/dockertool.py` & `futoin-cid-0.9.1/futoin/cid/tool/dockertool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/elixirtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/elixirtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/erlangtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/erlangtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/exetool.py` & `futoin-cid-0.9.1/futoin/cid/tool/exetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/flywaytool.py` & `futoin-cid-0.9.1/futoin/cid/tool/flywaytool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/futointool.py` & `futoin-cid-0.9.1/futoin/cid/tool/futointool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gcctool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gcctool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gemtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gemtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gemtoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/gemtoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gittool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gittool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gotool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gotool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gpgtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gpgtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gradletool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gradletool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/grunttool.py` & `futoin-cid-0.9.1/futoin/cid/tool/grunttool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gulptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gulptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gvmtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gvmtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/gziptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/gziptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/hgtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/hgtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/javatool.py` & `futoin-cid-0.9.1/futoin/cid/tool/javatool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/javatoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/javatoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/jdktool.py` & `futoin-cid-0.9.1/futoin/cid/tool/jdktool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/jfrogtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/jfrogtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/liquibasetool.py` & `futoin-cid-0.9.1/futoin/cid/tool/liquibasetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/maketool.py` & `futoin-cid-0.9.1/futoin/cid/tool/maketool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/maventool.py` & `futoin-cid-0.9.1/futoin/cid/tool/maventool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/mixtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/mixtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/nexus3tool.py` & `futoin-cid-0.9.1/futoin/cid/tool/nexus3tool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/nexustool.py` & `futoin-cid-0.9.1/futoin/cid/tool/nexustool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/nginxtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/nginxtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/nodetool.py` & `futoin-cid-0.9.1/futoin/cid/tool/nodetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/npmtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/npmtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/npmtoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/npmtoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/nvmtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/nvmtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/phoenixtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/phoenixtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/phpbuildtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/phpbuildtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/phpfpmtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/phpfpmtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/phptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/phptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/piptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/piptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/piptoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/piptoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/pumatool.py` & `futoin-cid-0.9.1/futoin/cid/tool/pumatool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/puppettool.py` & `futoin-cid-0.9.1/futoin/cid/tool/puppettool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/pythontool.py` & `futoin-cid-0.9.1/futoin/cid/tool/pythontool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/rubytool.py` & `futoin-cid-0.9.1/futoin/cid/tool/rubytool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/rusttool.py` & `futoin-cid-0.9.1/futoin/cid/tool/rusttool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/rustuptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/rustuptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/rvmtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/rvmtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/sbttool.py` & `futoin-cid-0.9.1/futoin/cid/tool/sbttool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/scalatool.py` & `futoin-cid-0.9.1/futoin/cid/tool/scalatool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/scptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/scptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/sdkmantool.py` & `futoin-cid-0.9.1/futoin/cid/tool/sdkmantool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/sdkmantoolmixin.py` & `futoin-cid-0.9.1/futoin/cid/tool/sdkmantoolmixin.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/setuptoolstool.py` & `futoin-cid-0.9.1/futoin/cid/tool/setuptoolstool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/sshtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/sshtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/svntool.py` & `futoin-cid-0.9.1/futoin/cid/tool/svntool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/tartool.py` & `futoin-cid-0.9.1/futoin/cid/tool/tartool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/twinetool.py` & `futoin-cid-0.9.1/futoin/cid/tool/twinetool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/unziptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/unziptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/uwsgitool.py` & `futoin-cid-0.9.1/futoin/cid/tool/uwsgitool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/virtualenvtool.py` & `futoin-cid-0.9.1/futoin/cid/tool/virtualenvtool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/webpacktool.py` & `futoin-cid-0.9.1/futoin/cid/tool/webpacktool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/xztool.py` & `futoin-cid-0.9.1/futoin/cid/tool/xztool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/yarntool.py` & `futoin-cid-0.9.1/futoin/cid/tool/yarntool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/tool/ziptool.py` & `futoin-cid-0.9.1/futoin/cid/tool/ziptool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/__init__.py` & `futoin-cid-0.9.1/futoin/cid/util/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/builddep.py` & `futoin-cid-0.9.1/futoin/cid/util/builddep.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/configutil.py` & `futoin-cid-0.9.1/futoin/cid/util/configutil.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/detect.py` & `futoin-cid-0.9.1/futoin/cid/util/detect.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/executil.py` & `futoin-cid-0.9.1/futoin/cid/util/executil.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/github.py` & `futoin-cid-0.9.1/futoin/cid/util/github.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/__init__.py` & `futoin-cid-0.9.1/futoin/cid/util/install/__init__.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/apk.py` & `futoin-cid-0.9.1/futoin/cid/util/install/apk.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/deb.py` & `futoin-cid-0.9.1/futoin/cid/util/install/deb.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/ebuild.py` & `futoin-cid-0.9.1/futoin/cid/util/install/ebuild.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/java.py` & `futoin-cid-0.9.1/futoin/cid/util/install/java.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/macos.py` & `futoin-cid-0.9.1/futoin/cid/util/install/macos.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/pacman.py` & `futoin-cid-0.9.1/futoin/cid/util/install/pacman.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/install/rpm.py` & `futoin-cid-0.9.1/futoin/cid/util/install/rpm.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/log.py` & `futoin-cid-0.9.1/futoin/cid/util/log.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/pathutil.py` & `futoin-cid-0.9.1/futoin/cid/util/pathutil.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/phputil.py` & `futoin-cid-0.9.1/futoin/cid/util/phputil.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/util/versionutil.py` & `futoin-cid-0.9.1/futoin/cid/util/versionutil.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin/cid/vcstool.py` & `futoin-cid-0.9.1/futoin/cid/vcstool.py`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/futoin_cid.egg-info/PKG-INFO` & `futoin-cid-0.9.1/futoin_cid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futoin-cid
-Version: 0.9.0
+Version: 0.9.1
 Summary: FutoIn Continuous Integration & Delivery Tool
 Home-page: https://github.com/futoin/cid-tool
 Download-URL: https://github.com/futoin/cid-tool/archive/master.zip
 Author: Andrey Galkin
 Author-email: andrey@futoin.org
 License: Apache 2.0
 Keywords: php ruby node nodejs npm gem rvm nvm grunt gulp bower  puppet build deploy futoin cmake make gradle maven java composer bundler
```

### Comparing `futoin-cid-0.9.0/futoin_cid.egg-info/SOURCES.txt` & `futoin-cid-0.9.1/futoin_cid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `futoin-cid-0.9.0/setup.py` & `futoin-cid-0.9.1/setup.py`

 * *Files identical despite different names*

